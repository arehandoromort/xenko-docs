# Template

Class templating is available in XKSL. Unlike many templating system, pdxsl requires strong typed templates. The available types are:

- value types from HLSL (float, int, float2, float3, float4)
- 2D textures
- sampler states
- semantics (used to replace semantics on variables)
- link types (used to replace link annotations)

An instantiated class behaves the same way as any other class. The value, texture and sampler template parameters are accessible like any other variable. However, it's impossible to modify their value; attempting to do so results in a compilation error. If a template variable is incorrectly used (eg using a sampler as a semantic), it should result in a compilation error. However, the behavior is officially unknown.

**Code:** Templating

```cs
class TemplateClass<float speed, Texture2D myTexture, SamplerState mySampler, Semantic mySemantic, LinkType myLink>
{
	[Color]
	[Link("myLink")]
	float4 myColor;
 
	stream float2 texcoord : mySemantic;
 
	float4 GetValue()
	{
		return speed * myColor * myTexture.Sample(mySampler, streams.texcoord);
	}
};
 
// TO INSTANCIATE THE CLASS, USE A CODE AS FOLLOW
TemplateClass<1.0f, Texturing.Texture0, Texturing.Sampler0, TEXCOORD0, MyColorLink>
```

## See also

* [Effect language](../effect-language.md)
* [Shading language index](index.md)
    - [Class inheritance](classes-mixins-and-inheritance.md)
    - [Composition](composition.md)
    - [Shader stage input/output automatic management](automatic-shader-stage-input-output.md)