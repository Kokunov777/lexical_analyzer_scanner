[Диаграмма без названия.drawio](https://github.com/user-attachments/files/26486198/default.drawio)### Часть 1 https://github.com/Kokunov777/User_interfce
### часть 3 

 # Лабораторная работа 2: Разработка лексического анализатора (сканера)

## Цель работы
Изучить назначение и принципы работы лексического анализатора в структуре компилятора. Спроектировать алгоритм (диаграмму состояний) и выполнить программную реализацию сканера для выделения лексем из входного текста. Интегрировать разработанный модуль в ранее созданный графический интерфейс языкового процессора.

## Сведения об авторе
- **ФИО**: kokunov Andrey
- **Группа**: АВТ 313
- **Дата**: 2026 год

## Постановка задачи
Разработать лексический анализатор (сканер) в соответствии с индивидуальным вариантом задания, интегрировать его в приложение из лабораторной работы №1 и обеспечить наглядный вывод результатов.

## Вариант задания
**Вариант 5**: Объявление комплексного числа с инициализацией на языке Rust

## Диаграмма состояний

[Uploadi<mxfile host="app.diagrams.net">
  <diagram name="Страница-1" id="uqbs2_lWaPZVfHCOd3IZ">
    <mxGraphModel dx="1414" dy="751" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="lCe6HePWFv0YYvxvvdeH-1" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="&lt;span id=&quot;docs-internal-guid-46ac5935-7fff-7d24-7f1b-107b7463b4a8&quot;&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(166, 38, 164); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;let&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(15, 17, 21); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt; complex_num2 &lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(64, 120, 242); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;=&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(15, 17, 21); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt; num&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;::&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(15, 17, 21); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;complex&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;::&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(183, 107, 1); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;Complex&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;::&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(64, 120, 242); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;new&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;(&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(183, 107, 1); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;3.1&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;,&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(15, 17, 21); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt; &lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(64, 120, 242); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;-&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(183, 107, 1); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;4.2&lt;/span&gt;&lt;span style=&quot;font-size: 14pt; font-family: &amp;quot;Times New Roman&amp;quot;, serif; color: rgb(56, 58, 66); background-color: transparent; font-variant-numeric: normal; font-variant-east-asian: normal; font-variant-alternates: normal; font-variant-position: normal; font-variant-emoji: normal; vertical-align: baseline; white-space-collapse: preserve;&quot;&gt;);&lt;/span&gt;&lt;/span&gt;" vertex="1">
          <mxGeometry height="30" width="520" x="160" y="10" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-2" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-3" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" target="lCe6HePWFv0YYvxvvdeH-5">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-3" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="start" vertex="1">
          <mxGeometry height="60" width="90" x="37.5" y="60" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-4" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-5" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;" target="lCe6HePWFv0YYvxvvdeH-6">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-5" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="0" vertex="1">
          <mxGeometry height="80" width="85" x="40" y="170" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-6" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="1" vertex="1">
          <mxGeometry height="100" width="110" x="210" y="165" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-7" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="letter" vertex="1">
          <mxGeometry height="30" width="60" x="150" y="180" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-8" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-6" style="curved=1;endArrow=classic;html=1;rounded=0;exitX=0;exitY=0;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" target="lCe6HePWFv0YYvxvvdeH-6" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <Array as="points">
              <mxPoint x="240" y="120" />
              <mxPoint x="270" y="130" />
            </Array>
            <mxPoint x="380" y="300" as="sourcePoint" />
            <mxPoint x="380" y="190" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-9" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="letter" vertex="1">
          <mxGeometry height="30" width="60" x="220" y="90" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-10" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="290" y="170" as="sourcePoint" />
            <mxPoint x="400" y="150" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-11" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="let" vertex="1">
          <mxGeometry height="30" width="60" x="290" y="130" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-12" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 1 ключевое слово - let" vertex="1">
          <mxGeometry height="30" width="186" x="400" y="130" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-13" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;exitX=1;exitY=0.5;exitDx=0;exitDy=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="322.9999999999998" y="194.71" as="sourcePoint" />
            <mxPoint x="410" y="180" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-14" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;rotation=-10;" value="complex_num2" vertex="1">
          <mxGeometry height="20" width="80" x="320" y="170" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-15" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 2 идентификатор&amp;nbsp; - complex_num2" vertex="1">
          <mxGeometry height="30" width="270" x="400" y="165" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-16" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;exitX=1;exitY=0.5;exitDx=0;exitDy=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="330" y="220" as="sourcePoint" />
            <mxPoint x="410" y="210" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-17" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;rotation=-15;" value="num" vertex="1">
          <mxGeometry height="20" width="80" x="320" y="195" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-18" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 2 идентификатор&amp;nbsp; - num" vertex="1">
          <mxGeometry height="30" width="205" x="400" y="195" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-19" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;exitX=1;exitY=0.5;exitDx=0;exitDy=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="320" y="245" as="sourcePoint" />
            <mxPoint x="400" y="235" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-20" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 2 идентификатор&amp;nbsp; - complex" vertex="1">
          <mxGeometry height="30" width="220" x="390" y="220" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-21" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;rotation=-10;" value="complex" vertex="1">
          <mxGeometry height="20" width="80" x="319.9952235025879" y="220.00202006699152" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-22" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-6" style="endArrow=classic;html=1;rounded=0;exitX=1;exitY=1;exitDx=0;exitDy=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="315" y="285" as="sourcePoint" />
            <mxPoint x="395" y="275" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-23" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 2 идентификатор&amp;nbsp; - complex" vertex="1">
          <mxGeometry height="30" width="220" x="385" y="260" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-24" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;rotation=15;" value="complex" vertex="1">
          <mxGeometry height="20" width="80" x="319.9987918971576" y="250.0040046367993" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-25" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-6" style="endArrow=classic;html=1;rounded=0;exitX=0.671;exitY=0.973;exitDx=0;exitDy=0;exitPerimeter=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="310" y="290" as="sourcePoint" />
            <mxPoint x="391" y="310" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-26" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 2 идентификатор&amp;nbsp; - new" vertex="1">
          <mxGeometry height="30" width="220" x="381" y="295" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-27" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;rotation=20;" value="new" vertex="1">
          <mxGeometry height="20" width="70" x="315" y="270" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-28" edge="1" parent="1" style="endArrow=none;html=1;rounded=0;entryX=0.5;entryY=1;entryDx=0;entryDy=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1510" as="sourcePoint" />
            <mxPoint x="72.5" y="249" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-29" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="369.71" as="sourcePoint" />
            <mxPoint x="170" y="369.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-30" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-31" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="380" y="370" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-31" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="2" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="330" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-32" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="_" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="340" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-33" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="549.71" as="sourcePoint" />
            <mxPoint x="170" y="549.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-34" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="550" as="sourcePoint" />
            <mxPoint x="380" y="550" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-35" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="_" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="520" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-36" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="4" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="510" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-37" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code&amp;nbsp; = 10 разделитель (пробел)" vertex="1">
          <mxGeometry height="35" width="249" x="361" y="352.5" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-38" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 3 оператор" vertex="1">
          <mxGeometry height="30" width="150" x="386" y="445" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-39" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="639.71" as="sourcePoint" />
            <mxPoint x="170" y="639.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-40" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="640" as="sourcePoint" />
            <mxPoint x="380" y="640" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-41" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value=":" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="610" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-42" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="5" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="600" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-43" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 4 двоеточие" vertex="1">
          <mxGeometry height="30" width="150" x="370" y="625" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-44" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="839.71" as="sourcePoint" />
            <mxPoint x="170" y="839.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-45" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="840" as="sourcePoint" />
            <mxPoint x="380" y="840" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-46" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="(" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="810" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-47" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="7" vertex="1">
          <mxGeometry height="80" width="85" x="165" y="790" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-48" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 8 разделитель" vertex="1">
          <mxGeometry height="30" width="150" x="370" y="825" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-49" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="85" y="944.71" as="sourcePoint" />
            <mxPoint x="175" y="944.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-50" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="260" y="945" as="sourcePoint" />
            <mxPoint x="385" y="945" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-51" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="material" vertex="1">
          <mxGeometry height="30" width="60" x="95" y="915" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-52" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="8" vertex="1">
          <mxGeometry height="80" width="85" x="175" y="905" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-53" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 7 Вещественное число" vertex="1">
          <mxGeometry height="30" width="200" x="370" y="930" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-54" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-52" style="curved=1;endArrow=classic;html=1;rounded=0;exitX=0;exitY=0;exitDx=0;exitDy=0;entryX=1;entryY=0;entryDx=0;entryDy=0;" target="lCe6HePWFv0YYvxvvdeH-52" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <Array as="points">
              <mxPoint x="190" y="870" />
              <mxPoint x="210" y="880" />
              <mxPoint x="230" y="870" />
            </Array>
            <mxPoint x="176" y="915" as="sourcePoint" />
            <mxPoint x="215" y="900" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-55" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="material" vertex="1">
          <mxGeometry height="30" width="60" x="230" y="870" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-56" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1039.71" as="sourcePoint" />
            <mxPoint x="170" y="1039.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-57" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="1040" as="sourcePoint" />
            <mxPoint x="380" y="1040" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-58" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="," vertex="1">
          <mxGeometry height="30" width="60" x="90" y="1010" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-59" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 8 Разделитель" vertex="1">
          <mxGeometry height="30" width="150" x="370" y="1025" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-60" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="7" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="1000" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-61" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1339.71" as="sourcePoint" />
            <mxPoint x="170" y="1339.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-62" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="1340" as="sourcePoint" />
            <mxPoint x="380" y="1340" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-63" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value=")" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="1310" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-64" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="8" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="1300" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-65" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 8 разделитель" vertex="1">
          <mxGeometry height="30" width="150" x="370" y="1325" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-66" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1439.71" as="sourcePoint" />
            <mxPoint x="170" y="1439.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-67" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="1440" as="sourcePoint" />
            <mxPoint x="380" y="1440" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-68" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value=";" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="1410" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-69" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="9" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="1400" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-70" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 9 конец оператора" vertex="1">
          <mxGeometry height="30" width="160" x="381" y="1425" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-71" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1510" as="sourcePoint" />
            <mxPoint x="180" y="1510" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-72" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="Error&amp;nbsp; недопустимый символ" vertex="1">
          <mxGeometry height="30" width="200" x="165" y="1490" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-73" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="459.71" as="sourcePoint" />
            <mxPoint x="170" y="459.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-74" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-75" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="380" y="460" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-75" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="3" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="420" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-76" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="=" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="430" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-77" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code&amp;nbsp; = 10 разделитель (пробел)" vertex="1">
          <mxGeometry height="35" width="249" x="356" y="532.5" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-78" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="729.71" as="sourcePoint" />
            <mxPoint x="170" y="729.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-79" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="255" y="730" as="sourcePoint" />
            <mxPoint x="380" y="730" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-80" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value=":" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="700" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-81" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="6" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="690" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-82" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 4 двоеточие" vertex="1">
          <mxGeometry height="30" width="150" x="370" y="715" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-83" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 3 оператор" vertex="1">
          <mxGeometry height="30" width="150" x="386" y="1114" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-84" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="80" y="1128.71" as="sourcePoint" />
            <mxPoint x="170" y="1128.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-85" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-86" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="380" y="1129" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-86" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="3" vertex="1">
          <mxGeometry height="80" width="85" x="170" y="1089" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-87" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="-" vertex="1">
          <mxGeometry height="30" width="60" x="90" y="1099" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-88" edge="1" parent="1" style="endArrow=classic;html=1;rounded=0;" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <mxPoint x="77.5" y="1249.71" as="sourcePoint" />
            <mxPoint x="167.5" y="1249.71" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-89" edge="1" parent="1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="252.5" y="1250" as="sourcePoint" />
            <mxPoint x="377.5" y="1250" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-90" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="material" vertex="1">
          <mxGeometry height="30" width="60" x="87.5" y="1220" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-91" parent="1" style="ellipse;whiteSpace=wrap;html=1;" value="8" vertex="1">
          <mxGeometry height="80" width="85" x="167.5" y="1210" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-92" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="code = 7 Вещественное число" vertex="1">
          <mxGeometry height="30" width="200" x="362.5" y="1235" as="geometry" />
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-93" edge="1" parent="1" source="lCe6HePWFv0YYvxvvdeH-91" style="curved=1;endArrow=classic;html=1;rounded=0;exitX=0;exitY=0;exitDx=0;exitDy=0;entryX=1;entryY=0;entryDx=0;entryDy=0;" target="lCe6HePWFv0YYvxvvdeH-91" value="">
          <mxGeometry height="50" relative="1" width="50" as="geometry">
            <Array as="points">
              <mxPoint x="190" y="1169" />
              <mxPoint x="210" y="1179" />
              <mxPoint x="230" y="1169" />
            </Array>
            <mxPoint x="176" y="1214" as="sourcePoint" />
            <mxPoint x="215" y="1199" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="lCe6HePWFv0YYvxvvdeH-94" parent="1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;" value="material" vertex="1">
          <mxGeometry height="30" width="60" x="230" y="1169" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
ng Диаграмма без названия.drawio…]()




## Тестовые примеры
### Пример 1: 
**Вход:** `let complex_num2 = num::complex::Complex::new(3.1, -4.2);`

| Условный код | Тип лексемы        | Лексема        | Местоположение |
|--------------|--------------------|----------------|----------------|
| 1            | Ключевое слово     | let            | 1:1-1:3        |
| 10           | Разделитель пробел | (пробел)       | 1:4-1:4        |
| 2            | Идентификатор      | complex_num2   | 1:5-1:16       |
| 10           | Разделитель пробел | (пробел)       | 1:17-1:17      |
| 3            | Оператор           | =              | 1:18-1:18      |
| 10           | Разделитель пробел | (пробел)       | 1:19-1:19      |
| 2            | Идентификатор      | num            | 1:20-1:22      |
| 4            | Разделитель пути   | :              | 1:23-1:24      |
| 4            | Разделитель пути   | :              | 1:23-1:24      |
| 2            | Идентификатор      | complex        | 1:25-1:31      |
| 4            | Разделитель пути   | :              | 1:32-1:33      |
| 4            | Разделитель пути   | :              | 1:32-1:33      |
| 2            | Идентификатор      | Complex        | 1:34-1:40      |
| 4            | Разделитель пути   | :              | 1:41-1:42      |
| 4            | Разделитель пути   | :              | 1:32-1:33      |
| 2            | Идентификатор      | new            | 1:43-1:45      |
| 8            | Разделитель        | (              | 1:46-1:46      |
| 7            | Вещественное число | 3.1            | 1:47-1:49      |
| 8            | Разделитель        | ,              | 1:50-1:50      |
| 10           | Разделитель пробел | (пробел)       | 1:51-1:51      |
| 7            | Вещественное число | -4.2           | 1:52-1:55      |
| 8            | Разделитель        | )              | 1:56-1:56      |
| 9            | Конец оператора    | ;              | 1:57-1:57      |


### Пример 2: Строка с недопустимым символом
**Вход:** `let x = @;`


| Условный код | Тип лексемы        | Лексема | Местоположение |
|--------------|--------------------|---------|----------------|
| 1            | Ключевое слово     | let     | 1:1-1:3        |
| 10           | Разделитель пробел | (пробел)| 1:4-1:4        |
| 2            | Идентификатор      | x       | 1:5-1:5        |
| 10           | Разделитель пробел | (пробел)| 1:6-1:6        |
| 3            | Оператор           | =       | 1:7-1:7        |
| 10           | Разделитель пробел | (пробел)| 1:8-1:8        |

**Ошибки:**

| Строка | Позиция | Сообщение               |
|--------|---------|-------------------------|
| 1      | 9       | Недопустимый символ '@' |

### Пример 3: Многострочный пример
**Вход:**
```
let a = num::complex::Complex::new(1, 2);
let b = 3.14;
```

| Условный код | Тип лексемы        | Лексема      | Местоположение |
|--------------|--------------------|--------------|----------------|
| 1            | Ключевое слово     | let          | 1:1-1:3        |
| 10           | Разделитель пробел | (пробел)     | 1:4-1:4        |
| 2            | Идентификатор      | a            | 1:5-1:5        |
| ... (пропущено для краткости) | ... | ... | ... |
| 9            | Конец оператора    | ;            | 1:36-1:36      |
| 10           | Разделитель пробел | (перевод строки) | 1:37-2:0   |
| 1            | Ключевое слово     | let          | 2:1-2:3        |
| 10           | Разделитель пробел | (пробел)     | 2:4-2:4        |
| 2            | Идентификатор      | b            | 2:5-2:5        |
| ... | ... | ... | ... |
