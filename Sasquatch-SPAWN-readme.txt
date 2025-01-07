Sasquatch has been added to the new files already  but............. if you adjust CE files you'll need to RE-ADD lines 3-24 to  Zombie_territories.xml

<territory color="4278190080">
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="3780" z="3530" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="2467.5" z="4677.5" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="4535" z="2040" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="730" z="4840" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="7435" z="2270" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="5365" z="6550" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="4253.33" z="3807.22" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="530" z="9925" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="7540" z="10005" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="8345" z="3910" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="6135" z="4405" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="6370" z="1365" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="1770" z="6355" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="5115" z="9990" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="6605" z="7010" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="4910" z="8130" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="785" z="6055" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="595" z="7580" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="650" z="1110" r="180"/>
        <zone name="InfectedSasquatch" smin="0" smax="0" dmin="0" dmax="1" x="9570" z="1865" r="180"/>
    </territory>


Add the above ^ to  Zombie_territories.xml



<event name="InfectedSasquatch">
        <nominal>3</nominal>
        <min>1</min>
        <max>1</max>
        <lifetime>3</lifetime>
        <restock>0</restock>
        <saferadius>100</saferadius>
        <distanceradius>50</distanceradius>
        <cleanupradius>100</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>player</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="3" min="3" type="PNW_Sasquatch_NEW"/>
        </children>
    </event> (edited)

Add the above to events.xml



<type name="PNW_Sasquatch_NEW">
        <nominal>0</nominal>
        <lifetime>1800</lifetime>
        <restock>0</restock>
        <min>1</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="0" deloot="0"/>
    </type>
    <type name="Sasquatch_ghillie">
        <nominal>0</nominal>
        <lifetime>28800</lifetime>
        <restock>0</restock>
        <min>0</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="1" deloot="0"/>
        <category name="clothes"/>
    </type>
    <type name="Sasquatch_mask">
        <nominal>0</nominal>
        <lifetime>28800</lifetime>
        <restock>0</restock>
        <min>0</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="1" deloot="0"/>
        <category name="clothes"/>
    </type>
    <type name="SasquatchSteakMeat">
        <nominal>0</nominal>
        <lifetime>28800</lifetime>
        <restock>0</restock>
        <min>0</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="1" deloot="0"/>
        <category name="food"/>
    </type>
        <type name="Sasquatch_Action_Figure">
        <nominal>0</nominal>
        <lifetime>28800</lifetime>
        <restock>0</restock>
        <min>0</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="1" deloot="0"/>
        <category name="tools"/>
    </type> 
	
	
Add the above ^ to  Types.xml