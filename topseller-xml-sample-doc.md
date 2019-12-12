# Topseller xml séma
Ez a dokumentáció a topseller.hu termékek importálásához való xml sémát mutatja be.

1. [product_id](#product_id)
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

## product_id
```xml
<product_id>ABC123</product_id>
```
Ezt az azonosítót a saját webáruházadból kell megadnod, hogy később betudd azonosítani melyik terméket rendelték meg.

## name
```xml
<name>Fali polc</name>
```
Termék megnevezése.

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
Ha a termékre nem érvényes semmilyen akció akkor 0 értéket kell megadni.

## images
```xml
<images></images>
```
Ehhez a részhez kell megadni a termékekhez való képeket.

### image
```xml
<image>https://example.com/img.png</image>
```
A termékhez való képet itt lehet hozzáadni.
Minden képet külön `image` tag közé kell tenni.

## category
```xml
<category>27</category>
```
Itt kell besorolni a terméket a topseller.hu által létrehozott kategóriák közé.
[Kategóriák listája](categories.md)

## attributes
```xml
<attributes></attributes>
```
A termékekre vonatkozó tulajdonságok.

### attribute_id
```xml
<attribute_id>3</attribute_id>
```
Itt kell megadni a termékre vonatkozó tulajdonság azonosítóját.
Tulajdonságok listája:

### attribute_value
```xml
<attribute_value>zöld</attribute_value>
```
Itt kell megadni a termékre vonatkozó tulajdonságnak az értékét.

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
                <attribute_id>Hosszúság (cm)</attribute_id>
                <attribute_value>90</attribute_value>
            </attribute>
            <attribute>
                <key>Szélesség (cm)</key>
                <attribute_value>23</attribute_value>
            </attribute>
            <attribute>
                <attribute_id>Anyag</attribute_id>
                <attribute_value>MDF</attribute_value>
            </attribute>
        </attributes>
        <description>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.</description>
    </product>
</products>
```
