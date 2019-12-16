### Tartalomjegyzék
1. [id](#id)
1. [name](#name)
1. [description](#description)
1. [price](#price)
1. [discount_price](#discount_price)
1. [images](#images)
1. [category](#category)
1. [attributes](#attributes)
1. [Példa xml](#példa-xml)

## id
```xml
<id>ABC123</id>
```
Ezt az azonosítót a saját webáruházából kell megadnia, hogy később betudja azonosítani melyik terméket rendelték meg illetve al terméket tudjon hozzáadni.
Fontos, hogy egyedi azonosító legyen tehát ne ismétlődjön kétszer ugyanaz az azonosító.

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
Termék bruttó forintban értendő ára.

## discount_price
```xml
<discount_price>10000</discount_price>
```
Termék forintban értendő akciós ára.
Ha a termékre nincs érvényes leárazás akkor a mezőt nem kell megadni.

## images
```xml
<images>
   <image>https://example.com/image1.png</image>
   <image>https://example.com/image2.png</image>
   <image>https://example.com/image3.png</image>
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
        <product_id>ABC123</product_id>
        <name>Fali polc</name>
        <price>12500</price>
        <discount_price>10000</discount_price>
        <images>
            <image>https://example.com/image1.png</image>
            <image>https://example.com/image2.png</image>
            <image>https://example.com/image3.png</image>
        </images>
        <category>Bútor > Nappali > Fali polc</category>
        <attributes>
           <attribute>
                <name>Szín</name>
                <value>zöld</value>
            </attribute>
            <attribute>
                <name>Anyag</name>
                <value>MDF</value>
            </attribute>
        </attributes>
        <description>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.</description>
       <delivery_cost>3000</delivery_cost>
    </product>
</products>
```
