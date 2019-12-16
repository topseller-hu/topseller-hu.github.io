# Topseller xml séma
Ez a dokumentáció a topseller.hu termékek importálásához való xml sémát mutatja be.

### Tartalomjegyzék
1. [id](#id)
1. [name](#name)
1. [description](#description)
1. [price](#price)
1. [discount_price](#discount_price)
1. [images](#images)
    * [image](#image)
1. [category](#category)
1. [attributes](#attributes)
    1. [attribute_id](#attribute_id)
    1. [attribute_value](#attribute_value)
1. [Példa xml](#példa-xml)

## id
```xml
<id>ABC123</id>
```
Ezt az azonosítót a saját webáruházából kell megadnia, hogy később betudja azonosítani melyik terméket rendelték meg.

## name
```xml
<name>Fali polc</name>
```
Termék neve.

## description
```xml
<description>Modern fali polc Stilista® márkájú termék sorozatból</description>
```
Termék leírása.

## price
```xml
<price>12000</price>
```
Termék bruttó ára.

## discount_price
```xml
<discount_price>10000</discount_price>
```
Termék akciós ára.
Ha a termékre nincs érvényes leárazás akkor a mezőt nem kell megadni.

## images
```xml
<images>
   <image>https://example.com/img01.png</image>
   <image>https://example.com/img02.png</image>
   <image>https://example.com/img03.png</image>
</images>
```
A termékekhez való képeket itt lehet megadni.
Minden képet külön `image` tag közé kell tenni.

## category
```xml
<category>Bútor > Nappali > Fali polc</category>
```
A terméket itt kell besorolni egy kategória alá.

## attributes
```xml
<attributes>
   <attribute>
      <name>Szín</name>
      <value>zöld</value>
   </attribute>
   <attribute>
      <name></name>
      <value>zöld</value>
   </attribute>
</attributes>
```
A termékekre vonatkozó tulajdonságok.

## delivery_cost
```xml
<delivery_cost>3000</delivery_cost>
```
A termék szállítási költsége.
Az ár forintban értendő.

## Példa xml
```xml
<products>
    <product>
        <product_id>AB123</product_id>
        <name>Fali polc</name>
        <price>12500</price>
        <discount_price>10000</discount_price>
        <images>
            <image>http://example.com/image1.png</image>
            <image>http://example.com/image2.png</image>
            <image>http://example.com/image3.png</image>
        </images>
        <category>38</category>
        <attributes>
            <attribute>
                <attribute_id>4</attribute_id>
                <attribute_value>90</attribute_value>
            </attribute>
            <attribute>
                <attribute_id>7</attribute_id>
                <attribute_value>23</attribute_value>
            </attribute>
            <attribute>
                <attribute_id>9</attribute_id>
                <attribute_value>MDF</attribute_value>
            </attribute>
        </attributes>
        <description>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.</description>
    </product>
</products>
```
