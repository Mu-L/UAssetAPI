# FInterfaceProperty

Namespace: UAssetAPI.FieldTypes

```csharp
public class FInterfaceProperty : FProperty
```

Inheritance [Object](https://docs.microsoft.com/en-us/dotnet/api/system.object) → [FField](./uassetapi.fieldtypes.ffield.md) → [FProperty](./uassetapi.fieldtypes.fproperty.md) → [FInterfaceProperty](./uassetapi.fieldtypes.finterfaceproperty.md)

## Fields

### **InterfaceClass**

```csharp
public FPackageIndex InterfaceClass;
```

### **ArrayDim**

```csharp
public EArrayDim ArrayDim;
```

### **ElementSize**

```csharp
public int ElementSize;
```

### **PropertyFlags**

```csharp
public EPropertyFlags PropertyFlags;
```

### **RepIndex**

```csharp
public ushort RepIndex;
```

### **RepNotifyFunc**

```csharp
public FName RepNotifyFunc;
```

### **BlueprintReplicationCondition**

```csharp
public ELifetimeCondition BlueprintReplicationCondition;
```

### **RawValue**

```csharp
public object RawValue;
```

### **UsmapPropertyTypeOverrides**

```csharp
public IDictionary<string, EPropertyType> UsmapPropertyTypeOverrides;
```

### **SerializedType**

```csharp
public FName SerializedType;
```

### **Name**

```csharp
public FName Name;
```

### **Flags**

```csharp
public EObjectFlags Flags;
```

### **MetaDataMap**

```csharp
public TMap<FName, FString> MetaDataMap;
```

## Constructors

### **FInterfaceProperty()**

```csharp
public FInterfaceProperty()
```

## Methods

### **Read(AssetBinaryReader)**

```csharp
public void Read(AssetBinaryReader reader)
```

#### Parameters

`reader` [AssetBinaryReader](./uassetapi.assetbinaryreader.md)<br>

### **Write(AssetBinaryWriter)**

```csharp
public void Write(AssetBinaryWriter writer)
```

#### Parameters

`writer` [AssetBinaryWriter](./uassetapi.assetbinarywriter.md)<br>
