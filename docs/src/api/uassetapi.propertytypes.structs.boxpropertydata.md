# BoxPropertyData

Namespace: UAssetAPI.PropertyTypes.Structs

```csharp
public class BoxPropertyData : UAssetAPI.PropertyTypes.Objects.PropertyData`1[[UAssetAPI.PropertyTypes.Structs.VectorPropertyData[], UAssetAPI, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]], System.ICloneable
```

Inheritance [Object](https://docs.microsoft.com/en-us/dotnet/api/system.object) → [PropertyData](./uassetapi.propertytypes.objects.propertydata.md) → [PropertyData&lt;VectorPropertyData[]&gt;](./uassetapi.propertytypes.objects.propertydata-1.md) → [BoxPropertyData](./uassetapi.propertytypes.structs.boxpropertydata.md)<br>
Implements [ICloneable](https://docs.microsoft.com/en-us/dotnet/api/system.icloneable)

## Fields

### **IsValid**

```csharp
public bool IsValid;
```

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
public VectorPropertyData[] Value { get; set; }
```

#### Property Value

[VectorPropertyData[]](./uassetapi.propertytypes.structs.vectorpropertydata.md)<br>

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

### **BoxPropertyData(FName)**

```csharp
public BoxPropertyData(FName name)
```

#### Parameters

`name` [FName](./uassetapi.unrealtypes.fname.md)<br>

### **BoxPropertyData()**

```csharp
public BoxPropertyData()
```

## Methods

### **Read(AssetBinaryReader, Boolean, Int64, Int64)**

```csharp
public void Read(AssetBinaryReader reader, bool includeHeader, long leng1, long leng2)
```

#### Parameters

`reader` [AssetBinaryReader](./uassetapi.assetbinaryreader.md)<br>

`includeHeader` [Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

`leng1` [Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64)<br>

`leng2` [Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64)<br>

### **ResolveAncestries(UnrealPackage, AncestryInfo)**

```csharp
public void ResolveAncestries(UnrealPackage asset, AncestryInfo ancestrySoFar)
```

#### Parameters

`asset` [UnrealPackage](./uassetapi.unrealpackage.md)<br>

`ancestrySoFar` [AncestryInfo](./uassetapi.propertytypes.objects.ancestryinfo.md)<br>

### **Write(AssetBinaryWriter, Boolean)**

```csharp
public int Write(AssetBinaryWriter writer, bool includeHeader)
```

#### Parameters

`writer` [AssetBinaryWriter](./uassetapi.assetbinarywriter.md)<br>

`includeHeader` [Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean)<br>

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

### **HandleCloned(PropertyData)**

```csharp
protected void HandleCloned(PropertyData res)
```

#### Parameters

`res` [PropertyData](./uassetapi.propertytypes.objects.propertydata.md)<br>