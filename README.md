# Reto-02

El diagrama UML modela el sistema de transporte público de Bogotá: Transmilenio. Representa las entidades principales que lo componen como buses, estaciones, rutas y usuarios, mostrando sus atributos, métodos y relaciones. Se usa la composición y herencia para reflejar cómo se conectan e interactúan las clases entre sí.

## Descripción general

El sistema está compuesto por varias clases que interactúan entre ellas para representar el transporte público:

- Transmilenio es la clase principal del sistema. Tiene elementos que son: estaciones, buses, funcionarios, usuarios, rutas y horarios.

- Las estaciones contienen componentes que son puertas anticolados, torniquetes, taquillas y puentes peatonales.

- Los buses tienen atributos como placa, tipo (troncal, alimentador, SITP, etc.) y capacidad. Cada bus sigue una ruta y opera según un horario específico.

- Las rutas definen el trayecto que sigue un bus a través de una serie de estaciones.

- Los horarios indican los días y la frecuencia con la que circulan los buses.
  
- Tipos de funcionarios que trabajan el sistema:
  - Guardias: vigilan las estaciones, atienden consultas y pitan.
  - Taquilleros: procesan pagos y atienden a los usuarios.
  - Encargados de limpieza: realizan el aseo.
  - Policías: se encargan de asegurar el orden.

- Los usuarios están clasificados en dos tipos:
  - Regulares: tienen su saldo en la tarjeta y pagan el pasaje.
  - Irregulares: evaden el pasaje.
  - 
## Relaciones principales

- Composición:
  - Transmilenio se compone de estaciones, buses, funcionarios, usuarios, rutas y horarios.
  - Las estaciones tienen elementos físicos como puertas, torniquete, taquilla y puente peatonal.

- Herencia:
  - Funcionarios es una clase base de donde se heredan los guardias, los taquilleros, el personal de limpieza y los policías.
  - Los usuarios regulares e irregulares se heredan de Usuarios.

- Relaciones:
  - Las estaciones están relacionadas con las rutas.
  - Los buses siguen rutas y se rigen por horarios.
  - Las estaciones son usadas por los usuarios y supervisadas por los funcionarios.
 
"""
drawio
<mxfile host="www.draw.io" agent="Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:137.0) Gecko/20100101 Firefox/137.0" version="26.2.14">
  <diagram name="Page-1" id="bDuRJJWdgGRRtXBBddua">
    <mxGraphModel grid="1" page="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="uGUT7fTzrwYjynbc_nDR-73" value="&lt;div&gt;Transmilenio&lt;/div&gt;" style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=26;fillColor=none;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="380" y="180" width="110" height="230" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-74" value="- Estaciones" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-73">
          <mxGeometry y="26" width="110" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-75" value="&lt;div&gt;- Buses&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-73">
          <mxGeometry y="52" width="110" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-76" value="&lt;div&gt;- Funcionarios&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-73">
          <mxGeometry y="78" width="110" height="32" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-77" value="&lt;div&gt;- Usuarios&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;&lt;div&gt;+ Rutas&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;&lt;div&gt;+ Horarios&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;&lt;div&gt;+ Rutas&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-73">
          <mxGeometry y="110" width="110" height="120" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-80" value="Estaciones" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="120" y="90" width="160" height="166" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-81" value="&lt;div&gt;- Nombre&lt;/div&gt;&lt;div&gt;- Componentes&lt;/div&gt;&lt;div&gt;- Personal&lt;/div&gt;&lt;div&gt;- Ubicación&lt;/div&gt;&lt;div&gt;&amp;nbsp;&lt;br&gt;&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-80">
          <mxGeometry y="26" width="160" height="84" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-82" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-80">
          <mxGeometry y="110" width="160" height="10" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-83" value="&lt;div&gt;+ Recibir Pasajeros&lt;/div&gt;&lt;div&gt;+ Supervisar Operaciones&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-80">
          <mxGeometry y="120" width="160" height="46" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-84" value="Buses" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="660" y="121" width="240" height="130" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-85" value="&lt;div&gt;- Placa&lt;/div&gt;&lt;div&gt;- Tipo (Troncal, Alimentador, SITP, ...)&lt;/div&gt;&lt;div&gt;- Capacidad (Número de Pasajeros)&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-84">
          <mxGeometry y="26" width="240" height="54" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-86" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-84">
          <mxGeometry y="80" width="240" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-87" value="&lt;div&gt;+ Iniciar Ruta&lt;/div&gt;&lt;div&gt;+ Realizar Parada&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-84">
          <mxGeometry y="88" width="240" height="42" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-89" value="Funcionarios" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="100" y="350" width="130" height="100" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-158" value="&lt;div&gt;- Identificación&lt;/div&gt;&lt;div&gt;- Uniforme&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-89">
          <mxGeometry y="26" width="130" height="34" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-90" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-89">
          <mxGeometry y="60" width="130" height="10" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-91" value="+ Realizar Tareas" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-89">
          <mxGeometry y="70" width="130" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-92" value="Usuarios " style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="520" y="390" width="160" height="110" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-93" value="&lt;div&gt;- Identificación&lt;/div&gt;&lt;div&gt;- Historial de Viajes&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-92">
          <mxGeometry y="26" width="160" height="34" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-94" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-92">
          <mxGeometry y="60" width="160" height="20" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-167" value="+ Usar Transporte" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-92">
          <mxGeometry y="80" width="160" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-96" value="Guardias" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-170" y="335" width="140" height="130" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-97" value="- Silbato" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-96">
          <mxGeometry y="26" width="140" height="34" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-98" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-96">
          <mxGeometry y="60" width="140" height="4" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-99" value="&lt;div&gt;&amp;nbsp;&amp;nbsp; + Accionar su silbato&amp;nbsp;&amp;nbsp;&amp;nbsp;&lt;/div&gt;&lt;div&gt;+Vigilar Estación&lt;/div&gt;&lt;div&gt;+ Atender Consultas&lt;/div&gt;" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-96">
          <mxGeometry y="64" width="140" height="66" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-100" value="Policías" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-130" y="540" width="160" height="130" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-101" value="&lt;br&gt;&lt;div&gt;+ Arma de fuego&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-100">
          <mxGeometry y="26" width="160" height="50" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-102" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-100">
          <mxGeometry y="76" width="160" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-103" value="&lt;div&gt;+ Colocar comparendos &lt;br&gt;&lt;/div&gt;&lt;div&gt;+ Asegurar Orden&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-100">
          <mxGeometry y="84" width="160" height="46" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-105" value="Taquilleros " style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="140" y="690" width="160" height="70" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-107" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-105">
          <mxGeometry y="26" width="160" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-108" value="&lt;div&gt;+ Procesar Pagos&lt;/div&gt;&lt;div&gt;+ Atender Usuarios&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-105">
          <mxGeometry y="34" width="160" height="36" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-115" value="Encargados de limpieza" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="290" y="540" width="160" height="84" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-116" value="&lt;div&gt;+ Implementos&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-115">
          <mxGeometry y="26" width="160" height="24" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-117" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-115">
          <mxGeometry y="50" width="160" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-118" value="+ Limpiar" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-115">
          <mxGeometry y="58" width="160" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-125" value="" style="endArrow=open;endFill=1;endSize=12;html=1;rounded=0;exitX=0.5;exitY=0;exitDx=0;exitDy=0;entryX=1;entryY=0.575;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-92" target="uGUT7fTzrwYjynbc_nDR-77">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="600" y="463.0000000000001" as="sourcePoint" />
            <mxPoint x="540" y="370" as="targetPoint" />
            <Array as="points">
              <mxPoint x="600" y="359" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-126" value="Regulares" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="520" y="530" width="110" height="86" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-168" value="- Saldo Tarjeta" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-126">
          <mxGeometry y="26" width="110" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-127" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-126">
          <mxGeometry y="52" width="110" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-128" value="+ Pagar el Pasaje" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-126">
          <mxGeometry y="60" width="110" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-129" value="" style="html=1;verticalAlign=bottom;endArrow=block;curved=0;rounded=0;entryX=0.455;entryY=0;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-126">
          <mxGeometry width="80" relative="1" as="geometry">
            <mxPoint x="570" y="500" as="sourcePoint" />
            <mxPoint x="550" y="520" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-130" value="" style="html=1;verticalAlign=bottom;endArrow=block;curved=0;rounded=0;entryX=0.182;entryY=0;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-131">
          <mxGeometry width="80" relative="1" as="geometry">
            <mxPoint x="660" y="500" as="sourcePoint" />
            <mxPoint x="680" y="520" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-131" value="Irregulares" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="640" y="530" width="110" height="60" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-132" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-131">
          <mxGeometry y="26" width="110" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-133" value="+ Evadir el pasaje" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-131">
          <mxGeometry y="34" width="110" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-136" value="Rutas" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="340" y="22" width="160" height="68" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-137" value="&lt;div&gt;- Nombre (B, C, D, G, F, ...)&lt;/div&gt;&lt;div&gt;- Estaciones&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-136">
          <mxGeometry y="26" width="160" height="34" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-138" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-136">
          <mxGeometry y="60" width="160" height="8" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-140" value="Horarios" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="710" y="300" width="180" height="90" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-141" value="&lt;div&gt;- Días (L-V, Sábado, Domingo)&lt;/div&gt;&lt;div&gt;- Frecuencia (cada cuanto pasan los buses)&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-140">
          <mxGeometry y="26" width="180" height="54" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-142" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-140">
          <mxGeometry y="80" width="180" height="10" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-143" value="" style="endArrow=open;endFill=1;endSize=12;html=1;rounded=0;exitX=0;exitY=-0.033;exitDx=0;exitDy=0;exitPerimeter=0;entryX=0.976;entryY=0.86;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-141" target="uGUT7fTzrwYjynbc_nDR-76">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="590" y="350" as="sourcePoint" />
            <mxPoint x="620" y="240" as="targetPoint" />
            <Array as="points">
              <mxPoint x="620" y="324" />
              <mxPoint x="620" y="286" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-145" value="Torniquete" style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=26;fillColor=none;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-120" y="-40" width="150" height="52" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-146" value="+ PermitirAcceso(tarjeta)" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-145">
          <mxGeometry y="26" width="150" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-149" value="Taquilla" style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=26;fillColor=none;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-110" y="200" width="140" height="78" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-150" value="+ Vender&amp;nbsp; Tarjetas" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-149">
          <mxGeometry y="26" width="140" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-151" value="+ Recargar Tarjetas" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-149">
          <mxGeometry y="52" width="140" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-152" value="Puente Peantonal" style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=26;fillColor=none;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="120" y="-40" width="140" height="52" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-153" value="+ Conectar Áreas" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-152">
          <mxGeometry y="26" width="140" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-155" value="Puertas Anticolados" style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=26;fillColor=none;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-110" y="90" width="140" height="70" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-156" value="+ Reducir Usuarios Irregulares" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="uGUT7fTzrwYjynbc_nDR-155">
          <mxGeometry y="26" width="140" height="44" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-78" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;exitX=1;exitY=0.5;exitDx=0;exitDy=0;entryX=-0.027;entryY=0.038;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-83" target="uGUT7fTzrwYjynbc_nDR-75">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="380" y="217.5" as="sourcePoint" />
            <mxPoint x="340" y="130" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-178" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;entryX=0;entryY=0.5;entryDx=0;entryDy=0;exitX=1;exitY=0.269;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-150" target="uGUT7fTzrwYjynbc_nDR-83">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="60" y="180" as="sourcePoint" />
            <mxPoint x="19.039999999999964" y="238.49400000000003" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-179" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;entryX=0;entryY=0.5;entryDx=0;entryDy=0;exitX=1;exitY=0.269;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="30" y="124.5" as="sourcePoint" />
            <mxPoint x="120" y="124.5" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-180" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;exitX=0.533;exitY=1.308;exitDx=0;exitDy=0;exitPerimeter=0;entryX=0.313;entryY=0;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-146" target="uGUT7fTzrwYjynbc_nDR-80">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="-40" y="40" as="sourcePoint" />
            <mxPoint x="170" y="60" as="targetPoint" />
            <Array as="points">
              <mxPoint x="-40" y="40" />
              <mxPoint x="-40" y="60" />
              <mxPoint x="80" y="60" />
              <mxPoint x="170" y="60" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-181" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;entryX=0.656;entryY=-0.024;entryDx=0;entryDy=0;exitX=0.75;exitY=1.038;exitDx=0;exitDy=0;exitPerimeter=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-153" target="uGUT7fTzrwYjynbc_nDR-80">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="230" y="40" as="sourcePoint" />
            <mxPoint x="320" y="40" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-182" value="" style="endArrow=diamondThin;endFill=1;endSize=24;html=1;rounded=0;entryX=0.288;entryY=0.913;entryDx=0;entryDy=0;exitX=0.5;exitY=0;exitDx=0;exitDy=0;entryPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-89" target="uGUT7fTzrwYjynbc_nDR-83">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="170" y="320" as="sourcePoint" />
            <mxPoint x="260" y="320" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-186" value="" style="endArrow=block;endSize=16;endFill=0;html=1;rounded=0;exitX=0.394;exitY=-0.057;exitDx=0;exitDy=0;exitPerimeter=0;entryX=0.75;entryY=1;entryDx=0;entryDy=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-105" target="uGUT7fTzrwYjynbc_nDR-89">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="210" y="510" as="sourcePoint" />
            <mxPoint x="370" y="510" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-187" value="" style="endArrow=block;endSize=16;endFill=0;html=1;rounded=0;entryX=0.546;entryY=1.067;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-91">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="120" y="590" as="sourcePoint" />
            <mxPoint x="180" y="590" as="targetPoint" />
            <Array as="points">
              <mxPoint x="30" y="590" />
              <mxPoint x="120" y="590" />
              <mxPoint x="170" y="590" />
              <mxPoint x="170" y="480" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-188" value="" style="endArrow=block;endSize=16;endFill=0;html=1;rounded=0;entryX=1.031;entryY=0.267;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-91">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="330" y="540" as="sourcePoint" />
            <mxPoint x="320" y="410" as="targetPoint" />
            <Array as="points">
              <mxPoint x="330" y="430" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-191" value="1" style="endArrow=open;html=1;endSize=12;startArrow=diamondThin;startSize=14;startFill=0;edgeStyle=orthogonalEdgeStyle;align=left;verticalAlign=bottom;rounded=0;exitX=1;exitY=0.298;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-81">
          <mxGeometry x="-1" y="3" relative="1" as="geometry">
            <mxPoint x="410" y="140" as="sourcePoint" />
            <mxPoint x="410" y="90" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-192" value="1" style="endArrow=open;html=1;endSize=12;startArrow=diamondThin;startSize=14;startFill=0;edgeStyle=orthogonalEdgeStyle;align=left;verticalAlign=bottom;rounded=0;exitX=1;exitY=0.298;exitDx=0;exitDy=0;exitPerimeter=0;entryX=-0.012;entryY=0.31;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-87">
          <mxGeometry x="-1" y="3" relative="1" as="geometry">
            <mxPoint x="490" y="221" as="sourcePoint" />
            <mxPoint x="630" y="150" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-193" value="" style="endArrow=open;endFill=1;endSize=12;html=1;rounded=0;exitX=0.417;exitY=-0.008;exitDx=0;exitDy=0;exitPerimeter=0;entryX=1;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="uGUT7fTzrwYjynbc_nDR-84" target="uGUT7fTzrwYjynbc_nDR-136">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="750" y="100" as="sourcePoint" />
            <mxPoint x="760" y="40" as="targetPoint" />
            <Array as="points">
              <mxPoint x="760" y="60" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-194" value="&lt;div&gt;Sigue una Ruta&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="600" y="30" width="100" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-195" value="" style="endArrow=open;endFill=1;endSize=12;html=1;rounded=0;entryX=1.017;entryY=0.278;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-85">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="680" y="444.5" as="sourcePoint" />
            <mxPoint x="970" y="160" as="targetPoint" />
            <Array as="points">
              <mxPoint x="960" y="445" />
              <mxPoint x="960" y="300" />
              <mxPoint x="960" y="160" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-196" value="Usa" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="790" y="420" width="100" height="26" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-198" value="" style="endArrow=open;endFill=1;endSize=12;html=1;rounded=0;entryX=0.613;entryY=-0.029;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" target="uGUT7fTzrwYjynbc_nDR-136">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="890" y="344.5" as="sourcePoint" />
            <mxPoint x="440" y="10" as="targetPoint" />
            <Array as="points">
              <mxPoint x="1000" y="345" />
              <mxPoint x="1000" />
              <mxPoint x="730" />
              <mxPoint x="438" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-199" value="Aplica a una determinada ruta" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="700" y="-39" width="120" height="50" as="geometry" />
        </mxCell>
        <mxCell id="uGUT7fTzrwYjynbc_nDR-201" value="" style="endArrow=block;endSize=16;endFill=0;html=1;rounded=0;" edge="1" parent="1">
          <mxGeometry width="160" relative="1" as="geometry">
            <mxPoint x="-30" y="410" as="sourcePoint" />
            <mxPoint x="100" y="410" as="targetPoint" />
          </mxGeometry>
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>

"""

