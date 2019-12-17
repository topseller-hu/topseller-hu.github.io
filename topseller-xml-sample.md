### Tartalomjegyzék

* [id](#id)
* [name](#name)
* [description](#description)
* [price](#price)
* [images](#images)
* [category](#category)
* [discount_price](#discount_price)
* [attributes](#attributes)
* [delivery_cost](#delivery_cost)
* [parent_id](#parent_id)
* [Példa xml](#példa-xml)

## id

``` xml
<id>ABC123</id>
```
Ezt az azonosítót a saját webáruházából kell megadnia, hogy később betudja azonosítani melyik terméket rendelték meg illetve al terméket tudjon hozzáadni.
Fontos, hogy egyedi azonosító legyen tehát ne ismétlődjön kétszer ugyanaz az azonosító.

## name

``` xml
<name>Fali polc</name>
```
Termék neve.

## description

``` xml
<description>Modern fali polc Stilista® márkájú termék sorozatból</description>
```
Termék leírása.

## price

``` xml
<price>12000</price>
```
Termék bruttó forintban értendő ára.

## discount_price

``` xml
<discount_price>10000</discount_price>
```
Termék forintban értendő akciós ára.  
Ha a termékre nincs érvényes leárazás akkor a mezőt nem kell megadni.

## images

``` xml
<images>
   <image>https://example.com/image1.png</image>
   <image>https://example.com/image2.png</image>
   <image>https://example.com/image3.png</image>
</images>
```
A termékekhez tartozó képek.  
Minden képet külön `image` tag közé kell tenni.

## category

``` xml
<category_id>37</category_id>
<category_name>Bútor > Nappali > Fali polc</category_name>
```
A termék kategóriába való helyezése.  
A `category_name` taget csak abban az esetben kell hozzáadni ha ez a kategória még nincs átirányítva megfelelően a rendszerünkben.

## attributes

``` xml
<attributes>
    <attribute>
        <id>45</id>
        <name>Szín</name>
        <value>zöld</value>
    </attribute>
    <attribute>
        <id>59</id>
        <name>Anyag</name>
        <value>zöld</value>
    </attribute>
</attributes>
```
A termékekre vonatkozó tulajdonságok.  
Minden tulajdonságot külön `attribute` tag közé kell helyezni.  
A `name` taget csak abban az esetben kell hozzáadni ha ez a tulajdonság még nincs átirányítva megfelelően a rendszerünkben.

## delivery_cost

``` xml
<delivery_cost>3000</delivery_cost>
```
A termék szállítási költsége.  
Az ár forintban értendő.

## parent_id

``` xml
<parent_id>ABC123</parent_id>
```

Ha egy terméknek különböző változatai vannak akkor a `parent_id` tag közé annak a terméknek az azonosítóját kell megadni amelyik termék alatt megszeretnénk jeleníteni a többit.

## Példa xml

``` xml
<products>
    <product>
        <id>ABC123</id>
        <name>Fali polc</name>
        <price>12500</price>
        <discount_price>10000</discount_price>
        <images>
            <image>https://example.com/image1.png</image>
            <image>https://example.com/image2.png</image>
            <image>https://example.com/image3.png</image>
        </images>
        <category_id>37</category_id>
        <category_name>Bútor > Nappali > Fali polc</category_name>
        <attributes>
           <attribute>
                <id>45</id>
                <name>Szín</name>
                <value>zöld</value>
            </attribute>
            <attribute>
                <id>59</id>
                <name>Anyag</name>
                <value>MDF</value>
            </attribute>
        </attributes>
        <description>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.</description>
       <delivery_cost>3000</delivery_cost>
    </product>
   <product>
        <id>DEF456</id>
        <parent_id>ABC123</parent_id>
        <name>Fali polc</name>
        <price>10000</price>
        <discount_price>7000</discount_price>
        <images>
            <image>https://example.com/image4.png</image>
            <image>https://example.com/image5.png</image>
            <image>https://example.com/image6.png</image>
        </images>
        <category_id>37</category_id>
        <category_name>Bútor > Nappali > Fali polc</category_name>
        <attributes>
            <attribute>
                <id>45</id>
                <name>Szín</name>
                <value>piros</value>
            </attribute>
            <attribute>
                <id>59</id>
                <name>Anyag</name>
                <value>MDF</value>
            </attribute>
        </attributes>
        <description>Modern fali polc Stilista® márkájú termék sorozatból VOLATO köszönhetően a lebegtető hatásnak gyönyörű kelléke lesz a szobának. Polc szélessége 3,8 cm és max. teherbírása 10 kg függően a fal anyagától, amelyre a polc el lesz helyezve.</description>
       <delivery_cost>3000</delivery_cost>
    </product>
</products>
```

