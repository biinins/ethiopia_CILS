# Домашнее задание № 6. VoyantTools #

![загружено](https://user-images.githubusercontent.com/63372538/147607984-6ec70e31-0ea6-49ea-82f9-06748d97af76.png)


Согласно **Summary** корпуса документов, можно сделать вывод, что самыми объемными являются корпуса eng (12793), it (12287), ar (10078), jp (8089) и no (7580), а короткими - amh (4349), es (4405), hu (4490), ch (4839) и ru (5768);


Вкладка **Terms** демонстрирует нам следующие результаты частотности слов в корпусе (показаны первые десять значений):

<table>
	<thead>
		<tr>
			<td>Term</td>
			<td>Count</td>
			<td>Trend</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>ethiopia</td>
			<td>1178</td>
			<td>0.016095655,0.016669974,0.017772267,0.015399046,0.015891032,0.01528314,0.0095768375,0.01155693,0.013969588,0.011741425,0.018203884</td>
		</tr>
		<tr>
			<td>ethiopian</td>
			<td>645</td>
			<td>0.00436882,0.007342727,0.008059517,0.0064097554,0.009988649,0.012709138,0.0066815144,0.008138684,0.010013599,0.005672823,0.009361997</td>
		</tr>
		<tr>
			<td>country</td>
			<td>340</td>
			<td>0.0068981373,0.002679103,0.006406282,0.0027358711,0.001816118,0.0035392535,0.0066815144,0.003906568,0.0034614909,0.007783641,0.003814147</td>
		</tr>
		<tr>
			<td>government</td>
			<td>229</td>
			<td>0.0011496895,0.0035721373,0.0026865054,0.0044555617,0.001816118,0.0038610038,0.0008908686,0.002929926,0.0029669923,0.0014511873,0.0019070735</td>
		</tr>
		<tr>
			<td>addis</td>
			<td>200</td>
			<td>0.0013796275,0.002679103,0.0037197769,0.0025013678,0.002043133,0.0011261262,0.0024498887,0.0027671524,0.002719743,0.003298153,0.0015603328</td>
		</tr>
		<tr>
			<td>ababa</td>
			<td>194</td>
			<td>0.0013796275,0.002679103,0.0037197769,0.0024232003,0.001816118,0.0011261262,0.0024498887,0.0027671524,0.0025961183,0.0030343009,0.0013869626</td>
		</tr>
		<tr>
			<td>population</td>
			<td>170</td>
			<td>0.00068981375,0.0021829729,0.0035131224,0.0014851872,0.0029511917,0.0012870013,0.004454343,0.0023602182,0.0008653727,0.0023746702,0.0024271845</td>
		</tr>
		<tr>
			<td>eritrea</td>
			<td>168</td>
			<td>0.0011496895,0.0015876166,0.0033064683,0.0013288517,0.0034052213,0.00064350065,0.0013363028,0.0017091235,0.005068612,0.001978892,0.0020804438</td>
		</tr>
		<tr>
			<td>people</td>
			<td>163</td>
			<td>0.002529317,0.0011907124,0.0035131224,0.0023450325,0.0015891033,0.00096525095,0.00155902,0.0018718971,0.0039559896,0.0009234829,0.0019070735</td>
		</tr>
		<tr>
			<td>years</td>
			<td>162</td>
			<td>0.002299379,0.0013891645,0.0037197769,0.0016415227,0.001816118,0.0014478764,0.0026726057,0.0025229917,0.0019779948,0.001978892,0.0013869626</td>
		</tr>
		</tbody>
</table>


В целом, **Terms** топ 10 отражает общую тематику корпуса, однако, изучив данные, можно заметить одно странное явление: вхождений слова addis на 6 больше, чем вхождений ababa, что фактически не представляется релевантным, потому что слово addis, скорее всего, должно использоваться в паре с ababa (addis ababa - наименование столицы), потому что само по себе addis с амхарского на английский переводилось бы как "new", но, тем не менее, в данном корпусе текстов оно было использовано в транслитерированной форме. Но при этом, обратив внимание на таблицу **Collocations**, составленную на основе приведенных выше 10ти слов и представленную ниже, можно отметить, что, непосредственно, словосочетаний addis ababa насчитывается 281 (честно говоря, я так и не поняла, почему так вышло, это же невозможно).
Более того, в топ 10 **Collocates** входят в основном очень странные сочетания, например, ethiopia ethiopia, ethiopia ethiopian, ethiopian ethiopia и так далее, что, как мне кажется связано с тем, что корпус был переведен на английский язык посредством Google Translate.


<table>
	<thead>
		<tr>
			<td>Term</td>
			<td>Collocate</td>
			<td>Count (context)</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>ethiopia</td>
			<td>ethiopia</td>
			<td>1198</td>
		</tr>
		<tr>
			<td>ethiopia</td>
			<td>ethiopian</td>
			<td>549</td>
		</tr>
		<tr>
			<td>ethiopian</td>
			<td>ethiopia</td>
			<td>543</td>
		</tr>
		<tr>
			<td>ethiopian</td>
			<td>ethiopian</td>
			<td>438</td>
		</tr>
		<tr>
			<td>country</td>
			<td>ethiopia</td>
			<td>322</td>
		</tr>
		<tr>
			<td>ethiopia</td>
			<td>country</td>
			<td>317</td>
		</tr>
		<tr>
			<td>addis</td>
			<td>ababa</td>
			<td>281</td>
		</tr>
		<tr>
			<td>ethiopia</td>
			<td>eritrea</td>
			<td>209</td>
		</tr>
		<tr>
			<td>eritrea</td>
			<td>ethiopia</td>
			<td>206</td>
		</tr>
		<tr>
			<td>ethiopia</td>
			<td>main</td>
			<td>201</td>
		</tr>
	</tbody>
</table>

На данном этапе я поняла, что подобные сочетания (ethiopia ethiopia, ethiopia ethiopian, ethiopian ethiopia) логичны, так как часто используются, поэтому я решила редактировать **Options** и добавить в **stop list** слова ethiopia и ethiopian, однако это не улучшило ситуацию (см. таблицу ниже).


<table>
	<thead>
		<tr>
			<td>Term</td>
			<td>Collocate</td>
			<td>Count (context)</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>addis</td>
			<td>ababa</td>
			<td>281</td>
		</tr>
		<tr>
			<td>population</td>
			<td>population</td>
			<td>163</td>
		</tr>
		<tr>
			<td>country</td>
			<td>country</td>
			<td>126</td>
		</tr>
		<tr>
			<td>government</td>
			<td>government</td>
			<td>118</td>
		</tr>
		<tr>
			<td>years</td>
			<td>years</td>
			<td>98</td>
		</tr>
		<tr>
			<td>addis</td>
			<td>addis</td>
			<td>94</td>
		</tr>
		<tr>
			<td>ababa</td>
			<td>addis</td>
			<td>91</td>
		</tr>
		<tr>
			<td>population</td>
			<td>million</td>
			<td>90</td>
		</tr>
		<tr>
			<td>ababa</td>
			<td>ababa</td>
			<td>88</td>
		</tr>
		<tr>
			<td>eritrea</td>
			<td>eritrea</td>
			<td>87</td>
		</tr>
	</tbody>
</table>


![график](https://user-images.githubusercontent.com/63372538/147612176-e1aeceac-53f5-4285-9c08-4957afcc6d28.png)
- синий - ethiopia
- зелёный - ethiopian
- розовый - country
- фиолетовый - government
- голубой - addis

Изучив график, мы можем сделать вывод о том, что
1) частотность ethiopia хоть и является высокой, тем не менее, нестабильна. Имеет наибольшие результаты в ch и ru, наименьшие - hu и no;
2) частотность ethiopian имеет еще более нестабильные соотношения в документах корпуса. Наибольшая частотность наблюдается в he, jp и ru, наименьшая - amh, eng, no, hu;
3) частотность country предстает зигзагоподной линией, однако остается в одних пределах. БОльшая частотность наблюдается в amh, ch, hu и no, остальные документы корпуса имеют относительно равные частотности;
4) частотность government и addis представляет низкие показатели во всех документах корпуса.


![scatter](https://user-images.githubusercontent.com/63372538/147609774-1292648f-d615-4a75-a86a-a82f74103ef2.png)
Рассматривая **ScatterPlot** корпуса, можно отметить интересную закономерность: большинство приведенных слов корпуса в более частотной мере используются во всех документах корпуса, кроме amh, который на визуализации занимает отдаленную позицию, находясь рядом со словами amharic, language, nations и selassie. А empire и kingdom впринципе занимают довольно отдаленную позицию от всех документов корпуса.

![загружено (1)](https://user-images.githubusercontent.com/63372538/147613079-b4ee3487-5ff6-490f-a27c-96c4aed35810.png)

Визуализация через **DreamScape** позволяет увидеть основные регионы повествования корпуса, что дает возможность не только лучше идентифицировать корпус, но и проанализировать параллели, проходящие между **Terms** и **Collocates**, как они соотносятся и почему. Например, слова country и government затрагивают действия и характеристики государства, включая взаимодействия с другими странами, как мы это видим на карте. Слова population и people затрагивают, непосредственно, аспекты населения и народов, проживающих на территории Эфиопии и не только. Слово eritrea говорит нам о тесных международных связях с северо-восточным соседствующим государством.  
