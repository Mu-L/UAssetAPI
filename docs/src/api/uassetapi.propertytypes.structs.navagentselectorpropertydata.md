# NavAgentSelectorPropertyData

Namespace: UAssetAPI.PropertyTypes.Structs

```csharp
public class NavAgentSelectorPropertyData : UAssetAPI.PropertyTypes.Objects.PropertyData`1[[UAssetAPI.PropertyTypes.Structs.FNavAgentSelector, UAssetAPI, Version=1.0.1.0, Culture=neutral, PublicKeyToken=null]], System.ICloneable
```

Inheritance [Object](https://docs.microsoft.com/en-us/dotnet/api/system.object) → [PropertyData](./uassetapi.propertytypes.objects.propertydata.md) → [PropertyData&lt;FNavAgentSelector&gt;](./uassetapi.propertytypes.objects.propertydata-1.md) → [NavAgentSelectorPropertyData](./uassetapi.propertytypes.structs.navagentselectorpropertydata.md)<br>
Implements [ICloneable](https://docs.microsoft.com/en-us/dotnet/api/system.icloneable)

## Fields

### **Name**

The name of this property.

```csharp
public FName Name;
```

### **Ancestry**

The ancestry of this property. Contains information about all the classes/structs that this property is contained within. Not serialized.

```csharp
public AncestryInfo Ancestry;
```

### **DuplicationIndex**

The duplication index of this property. Used to distinguish properties with the same name in the same struct.

```csharp
public int DuplicationIndex;
```

### **PropertyGuid**

An optional property GUID. Nearly always null.

```csharp
public Nullable<Guid> PropertyGuid;
```

### **IsZero**

Whether or not this property is "zero," meaning that its body can be skipped during unversioned property serialization because it consists solely of null bytes.



This field will always be treated as if it is false if [PropertyData.CanBeZero(UnrealPackage)](./uassetapi.propertytypes.objects.propertydata.md#canbezerounrealpackage) does not return true.

```csharp
public bool IsZero;
```

### **Offset**

The offset of this property on disk. This is for the user only, and has no bearing in the API itself.

```csharp
public long Offset;
```

### **Tag**

An optional tag which can be set on any property in memory. This is for the user only, and has no bearing in the API itself.

```csharp
public object Tag;
```

## Properties

### **HasCustomStructSerialization**

```csharp
public bool HasCustomStructSerialization { get; }
```

#### Property Value

[Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

### **PropertyType**

```csharp
public FString PropertyType { get; }
```

#### Property Value

[FString](./uassetapi.unrealtypes.fstring.md)<br>

### **Value**

The "main value" of this property, if such a concept is applicable to the property in question. Properties may contain other values as well, in which case they will be present as other fields in the child class.

```csharp
public FNavAgentSelector Value { get; set; }
```

#### Property Value

[FNavAgentSelector](./uassetapi.propertytypes.structs.fnavagentselector.md)<br>

### **RawValue**

```csharp
public object RawValue { get; set; }
```

#### Property Value

[Object](https://docs.microsoft.com/en-us/dotnet/api/system.object)<br>

### **ShouldBeRegistered**

Determines whether or not this particular property should be registered in the property registry and automatically used when parsing assets.

```csharp
public bool ShouldBeRegistered { get; }
```

#### Property Value

[Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

### **DefaultValue**

The default value of this property, used as a fallback when no value is defined. Null by default.

```csharp
public object DefaultValue { get; }
```

#### Property Value

[Object](https://docs.microsoft.com/en-us/dotnet/api/system.object)<br>

## Constructors

### **NavAgentSelectorPropertyData(FName)**

```csharp
public NavAgentSelectorPropertyData(FName name)
```

#### Parameters

`name` [FName](./uassetapi.unrealtypes.fname.md)<br>

### **NavAgentSelectorPropertyData()**

```csharp
public NavAgentSelectorPropertyData()
```

## Methods

### **Read(AssetBinaryReader, Boolean, Int64, Int64, PropertySerializationContext)**

```csharp
public void Read(AssetBinaryReader reader, bool includeHeader, long leng1, long leng2, PropertySerializationContext serializationContext)
```

#### Parameters

`reader` [AssetBinaryReader](./uassetapi.assetbinaryreader.md)<br>

`includeHeader` [Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

`leng1` [Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64)<br>

`leng2` [Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64)<br>

`serializationContext` [PropertySerializationContext](./uassetapi.propertytypes.objects.propertyserializationcontext.md)<br>

### **Write(AssetBinaryWriter, Boolean, PropertySerializationContext)**

```csharp
public int Write(AssetBinaryWriter writer, bool includeHeader, PropertySerializationContext serializationContext)
```

#### Parameters

`writer` [AssetBinaryWriter](./uassetapi.assetbinarywriter.md)<br>

`includeHeader` [Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

`serializationContext` [PropertySerializationContext](./uassetapi.propertytypes.objects.propertyserializationcontext.md)<br>

#### Returns

[Int32](https://docs.microsoft.com/en-us/dotnet/api/system.int32)<br>

### **FromString(String[], UAsset)**

```csharp
public void FromString(String[] d, UAsset asset)
```

#### Parameters

`d` [String[]](https://docs.microsoft.com/en-us/dotnet/api/system.string)<br>

`asset` [UAsset](./uassetapi.uasset.md)<br>

### **ToString()**

```csharp
public string ToString()
```

#### Returns

[String](https://docs.microsoft.com/en-us/dotnet/api/system.string)<br>