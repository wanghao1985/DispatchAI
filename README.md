"DispatchAI" 

修改记录：
1、“\<attribute name="belongs" deviceType="transformer" />   --->  \<attribute name="belongs" deviceType="transformer" value="NULL" />”
2、定语按离名词距离从远到近在文件中按从上到下的方式排序

20180504-hxl
1.多个设备的请求由<entity>标签分割
<subject name="property" valueType="p" method="sum" value="?">
 <entity>
  <attribute name="belongs" deviceType="acline" value="安故Ⅰ路ID"/>
 </entity>
 <entity>
  <attribute name="belongs" deviceType="acline" value="安故ⅠⅠ路ID"/>
 </entity>
</subject>
2.越接近主语的定语，在结构里里subject也越近
<subject name="property" valueType="oil_temperature" method="max" value="?">
 <attribute name="belongs" deviceType="st" value="丹巴ID"/>
 <attribute name="belongs" deviceType="transformer" value="2#主变ID"/>
</subject>
改成：
<subject name="property" valueType="oil_temperature" method="max" value="?">
 <attribute name="belongs" deviceType="transformer" value="2#主变ID"/>
 <attribute name="belongs" deviceType="st" value="丹巴ID"/>
</subject>