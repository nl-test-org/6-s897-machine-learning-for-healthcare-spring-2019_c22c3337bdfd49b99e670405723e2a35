---
about_this_resource_text: '<p>Dr. Yala discusses deep learning models for mammogram
  interpretation and triaging. While many aspects of cancer detection based on mammograms
  are similar to those of natural image classification (ImageNet), there are some
  key differences.</p> <p>Speaker: Adam Yala</p>             <p><a href="./resolveuid/85e4e6d6c379d4f033feac9ae904200e">Lecture
  13: Machine Learning for Mammography slides (PDF - 2.5MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: 2ZXYM1h9pgY
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: Video-YouTube-Stream
  type: Video
  uid: 09764f155f3cea41c0683175ab627dc9
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/2ZXYM1h9pgY/default.jpg
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 91df0462beaaf6d76b7f9b5a998f40da
- id: 3Play-3PlayYouTubeid-MP4
  media_location: 2ZXYM1h9pgY
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: 901d87ff8afc8b0aa06305524e233292
- id: 2ZXYM1h9pgY.srt
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-13-machine-learning-for-mammography/2ZXYM1h9pgY.srt
  title: 3play caption file
  type: null
  uid: 120d4b17017f1d2d2ded6735871f1e36
- id: 2ZXYM1h9pgY.pdf
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-13-machine-learning-for-mammography/2ZXYM1h9pgY.pdf
  title: 3play pdf file
  type: null
  uid: 6827cbb86b351807d8f7cbd09d995e18
- id: Caption-3Play YouTube id-SRT
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 7ea88c8147cc5dec71dda6726929be1d
- id: Transcript-3Play YouTube id-PDF
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 53a8640329eefa90a176824ca0f2fa6a
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec13_300k.mp4
  parent_uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127
  title: Video-Internet Archive-MP4
  type: Video
  uid: b7b9dbef8a10750cbb21560bdec0a91b
inline_embed_id: 17069995lecture13machinelearningformammography31036199
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-13-machine-learning-for-mammography
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-13-machine-learning-for-mammography
template_type: Tabbed
title: 'Lecture 13: Machine Learning for Mammography'
transcript: <p><span m="15690">ADAM YALA:</span> <span m="15874">OK,</span> <span
  m="16059">great.</span> <span m="16280">Well,</span> <span m="16420">thank</span>
  <span m="16600">you</span> <span m="16660">for</span> <span m="16750">the</span>
  <span m="16990">great</span> <span m="17260">setup.</span></p><p><span m="18470">So</span>
  <span m="18610">for</span> <span m="18730">this</span> <span m="18820">section,</span>
  <span m="19280">I'm gonna</span> <span m="19380">talk</span> <span m="19480">about</span>
  <span m="19840">some</span> <span m="20020">of</span> <span m="20140">our</span>
  <span m="20230">work</span> <span m="20530">in</span> <span m="20650">interpreting</span>
  <span m="21070">mammograms</span> <span m="21520">for</span> <span m="21640">cancer.</span>
  <span m="22440">Specifically</span> <span m="22850">it's</span> <span m="22930">going</span>
  <span m="23040">to</span> <span m="23110">go</span> <span m="23260">into</span>
  <span m="23530">cancer</span> <span m="23860">detection</span> <span m="24400">and</span>
  <span m="24490">triage</span> <span m="24860">mammograms.</span> <span m="25510">Next,</span>
  <span m="25950">we'll</span> <span m="26080">talk</span> <span m="26290">about</span>
  <span m="26710">our</span> <span m="27130">technical</span> <span m="27580">approach</span>
  <span m="27940">in</span> <span m="28030">breast</span> <span m="28180">cancer</span>
  <span m="28450">risk.</span> <span m="29380">And</span> <span m="29390">then</span>
  <span m="29470">finally</span> <span m="29740">close</span> <span m="30070">up</span>
  <span m="30190">in</span> <span m="30720">the</span> <span m="30880">many,</span>
  <span m="31280">many</span> <span m="31420">different</span> <span m="31660">ways</span>
  <span m="31840">to</span> <span m="31930">mess</span> <span m="32170">up</span>
  <span m="32380">and</span> <span m="32470">the</span> <span m="32560">way</span>
  <span m="32680">things</span> <span m="32830">can</span> <span m="32920">go</span>
  <span m="33040">wrong,</span> <span m="33850">and</span> <span m="33970">how</span>
  <span m="34090">does</span> <span m="34240">it</span> <span m="34420">[INAUDIBLE]</span>
  <span m="34700">clinical</span> <span m="35030">implementation.</span></p><p><span
  m="35360">So</span> <span m="35920">let's</span> <span m="36160">kind</span> <span
  m="36340">of</span> <span m="36400">look</span> <span m="36550">more</span> <span
  m="36700">closely</span> <span m="37060">at</span> <span m="37120">the</span> <span
  m="37210">numbers</span> <span m="37780">of</span> <span m="37990">the</span> <span
  m="38110">actual</span> <span m="38350">breast</span> <span m="38500">cancer</span>
  <span m="38680">screening</span> <span m="39010">workflow.</span> <span m="39550">So</span>
  <span m="39880">as</span> <span m="40030">Connie already</span> <span m="40500">said,</span>
  <span m="40800">you</span> <span m="40870">might</span> <span m="41650">see</span>
  <span m="41920">something</span> <span m="42190">like</span> <span m="42310">1,000</span>
  <span m="42700">patients.</span> <span m="43570">All</span> <span m="43750">them</span>
  <span m="43900">take</span> <span m="44050">mammograms.</span> <span m="44680">Of</span>
  <span m="45010">that</span> <span m="45190">1,000,</span> <span m="45760">on</span>
  <span m="45880">average</span> <span m="46180">maybe</span> <span m="46390">100</span>
  <span m="46780">they</span> <span m="46870">called</span> <span m="47110">back</span>
  <span m="47410">for</span> <span m="47530">additional</span> <span m="47830">imaging.</span>
  <span m="48910">Of</span> <span m="49030">that</span> <span m="49210">100,</span>
  <span m="49690">something</span> <span m="50020">like</span> <span m="50290">20</span>
  <span m="50950">will</span> <span m="51100">get</span> <span m="51220">biopsied.</span>
  <span m="52220">And</span> <span m="52520">you end up with</span> <span m="52720">maybe</span>
  <span m="52990">five</span> <span m="53260">or</span> <span m="53320">six</span>
  <span m="53590">diagnoses</span> <span m="54130">of</span> <span m="54190">breast</span>
  <span m="54340">cancer.</span></p><p><span m="55250">So</span> <span m="55330">one</span>
  <span m="55540">very</span> <span m="55750">clear</span> <span m="56020">thing</span>
  <span m="56200">you</span> <span m="56290">see</span> <span m="56530">about</span>
  <span m="56860">problems</span> <span m="57880">when</span> <span m="58000">you</span>
  <span m="58060">look</span> <span m="58180">at</span> <span m="58240">this</span>
  <span m="58390">funnel</span> <span m="59380">is</span> <span m="59530">that</span>
  <span m="60460">way</span> <span m="60820">over</span> <span m="61030">99%</span>
  <span m="62200">of</span> <span m="62410">people</span> <span m="62770">that</span>
  <span m="62860">you</span> <span m="62950">see</span> <span m="63100">in</span>
  <span m="63190">a</span> <span m="63220">given</span> <span m="63490">day</span>
  <span m="64120">are</span> <span m="64239">cancer-free.</span> <span m="64860">So
  your</span> <span m="64900">actual</span> <span m="65170">incidence</span> <span
  m="65620">is</span> <span m="65710">very</span> <span m="65980">low.</span></p><p><span
  m="67100">And</span> <span m="67900">so</span> <span m="68110">there's</span> <span
  m="68290">kind</span> <span m="68440">of</span> <span m="68500">a</span> <span m="68530">natural</span>
  <span m="68730">question</span> <span m="68920">that</span> <span m="69010">can</span>
  <span m="69130">come</span> <span m="69310">up.</span> <span m="69460">What</span>
  <span m="69610">can</span> <span m="69790">you</span> <span m="69880">do</span>
  <span m="70090">in</span> <span m="70180">terms</span> <span m="70360">of</span>
  <span m="70420">modeling</span> <span m="70860">if</span> <span m="70970">you</span>
  <span m="71210">have</span> <span m="71350">an</span> <span m="71590">even</span>
  <span m="71860">OK</span> <span m="72250">cancer</span> <span m="72580">detection</span>
  <span m="72940">model</span> <span m="73720">to</span> <span m="74080">raise</span>
  <span m="74440">the</span> <span m="74530">incidence</span> <span m="74980">of</span>
  <span m="75040">this</span> <span m="75160">population</span> <span m="75730">but</span>
  <span m="75850">automatically</span> <span m="76270">reading</span> <span m="76570">a</span>
  <span m="76630">portion</span> <span m="77020">of</span> <span m="77080">the</span>
  <span m="77140">population</span> <span m="77590">is</span> <span m="77680">healthy.</span>
  <span m="78010">Does</span> <span m="78480">everybody</span> <span m="78800">just</span>
  <span m="79000">follow</span> <span m="79270">that</span> <span m="79390">broad</span>
  <span m="79570">idea?</span> <span m="81400">OK.</span> <span m="81720">That's</span>
  <span m="82170">enough</span> <span m="82410">head</span> <span m="82810">nods.</span></p><p><span
  m="83670">So</span> <span m="83910">the</span> <span m="84060">broad</span> <span
  m="84360">idea</span> <span m="84630">here</span> <span m="84780">is you're</span>
  <span m="84870">going</span> <span m="84990">to</span> <span m="85050">train</span>
  <span m="85260">the</span> <span m="85290">cancer</span> <span m="85590">detection</span>
  <span m="86010">model</span> <span m="86280">to</span> <span m="86370">try</span>
  <span m="86520">to</span> <span m="87090">find</span> <span m="87450">cancer</span>
  <span m="87730">as</span> <span m="87840">well</span> <span m="88050">as</span>
  <span m="88140">we</span> <span m="88260">can.</span> <span m="89010">Given</span>
  <span m="89400">that,</span> <span m="89610">we're</span> <span m="89700">going</span>
  <span m="89820">to</span> <span m="89880">try</span> <span m="90000">to</span> <span
  m="90060">say,</span> <span m="90180">what's</span> <span m="90420">a</span> <span
  m="90480">threshold</span> <span m="91170">on</span> <span m="91350">a</span> <span
  m="91860">development</span> <span m="92400">set</span> <span m="92640">such</span>
  <span m="92940">that</span> <span m="93060">we</span> <span m="93180">can</span>
  <span m="93330">kind</span> <span m="93480">of</span> <span m="93540">say</span>
  <span m="94050">below</span> <span m="94380">the</span> <span m="94500">threshold</span>
  <span m="94950">no</span> <span m="95100">one</span> <span m="95220">has</span>
  <span m="95340">cancer.</span> <span m="96220">And</span> <span m="96320">if</span>
  <span m="96420">we</span> <span m="96520">use</span> <span m="96660">that</span>
  <span m="96780">at</span> <span m="96840">test</span> <span m="97080">times,</span>
  <span m="97410">simulating</span> <span m="97810">clinical</span> <span m="97890">implementation,</span>
  <span m="98970">what</span> <span m="99120">would</span> <span m="99240">that</span>
  <span m="99390">look</span> <span m="99600">like?</span> <span m="100030">And</span>
  <span m="100130">can</span> <span m="100200">we</span> <span m="100320">actually</span>
  <span m="101040">do</span> <span m="101280">better</span> <span m="101520">by</span>
  <span m="101640">doing</span> <span m="101820">this</span> <span m="101940">kind</span>
  <span m="102060">of</span> <span m="102120">process?</span></p><p><span m="103560">And</span>
  <span m="104010">the</span> <span m="104130">kind</span> <span m="104310">of</span>
  <span m="104400">broad</span> <span m="104790">plan</span> <span m="105270">of</span>
  <span m="105360">how</span> <span m="105500">I'm</span> <span m="105600">gonna</span>
  <span m="105660">talk</span> <span m="105840">about</span> <span m="106050">this--</span>
  <span m="106240">I'm</span> <span m="106370">gonna</span> <span m="106430">do</span>
  <span m="106530">this</span> <span m="106680">for</span> <span m="106770">the</span>
  <span m="106860">next</span> <span m="107040">product</span> <span m="107270">as</span>
  <span m="107370">well.</span> <span m="107700">Of course,</span> <span m="108170">we're</span>
  <span m="108300">going</span> <span m="108420">to</span> <span m="108480">talk</span>
  <span m="108600">about</span> <span m="108750">the</span> <span m="108810">kind</span>
  <span m="108960">of</span> <span m="109050">dataset</span> <span m="109410">collection</span>
  <span m="109860">and</span> <span m="109950">how</span> <span m="110040">we</span>
  <span m="110130">think</span> <span m="110280">about,</span> <span m="110430">like,</span>
  <span m="110550">you</span> <span m="110610">know,</span> <span m="110700">what</span>
  <span m="110910">is</span> <span m="111030">good</span> <span m="111270">data</span>
  <span m="112230">and</span> <span m="112320">how</span> <span m="112440">do</span>
  <span m="112500">we</span> <span m="113070">think</span> <span m="113220">about</span>
  <span m="113400">that.</span></p><p><span m="114000">Next,</span> <span m="114270">the</span>
  <span m="114330">actual</span> <span m="114540">methodology</span> <span m="115230">and</span>
  <span m="115350">go</span> <span m="115640">into</span> <span m="115800">the</span>
  <span m="115920">general</span> <span m="116370">challenges</span> <span m="116940">when</span>
  <span m="117060">you're</span> <span m="117150">modeling</span> <span m="118140">mammograms</span>
  <span m="118830">for</span> <span m="118950">any</span> <span m="119130">computer</span>
  <span m="119370">mission</span> <span m="119580">tasks,</span> <span m="119930">specifically</span>
  <span m="120510">in</span> <span m="120600">cancer,</span> <span m="121560">and</span>
  <span m="121680">also,</span> <span m="121950">obviously,</span> <span m="122280">risk.</span>
  <span m="123070">And</span> <span m="123170">lastly,</span> <span m="123520">how</span>
  <span m="123540">we</span> <span m="123600">thought</span> <span m="123750">about</span>
  <span m="123930">the</span> <span m="123990">analysis</span> <span m="124450">and</span>
  <span m="124530">some</span> <span m="124650">kind</span> <span m="124800">of</span>
  <span m="124890">objectives</span> <span m="125340">there.</span></p><p><span m="126270">So</span>
  <span m="126420">to</span> <span m="126540">kind</span> <span m="126660">of</span>
  <span m="126720">dive</span> <span m="127080">into</span> <span m="127350">it,</span>
  <span m="127740">we</span> <span m="127890">took</span> <span m="128039">consecutive</span>
  <span m="128550">mammograms.</span> <span m="129150">I'll</span> <span m="129240">get</span>
  <span m="129330">back</span> <span m="129509">into</span> <span m="129590">this</span>
  <span m="129720">later.</span> <span m="130039">This is</span> <span m="130169">actually</span>
  <span m="130380">quite</span> <span m="130530">important.</span></p><p><span m="131450">We</span>
  <span m="131460">took</span> <span m="131580">consecutive</span> <span m="131970">mammograms</span>
  <span m="132420">from</span> <span m="132540">2009</span> <span m="133200">to</span>
  <span m="133290">2016.</span> <span m="134760">This</span> <span m="134880">started</span>
  <span m="135180">off</span> <span m="135330">with</span> <span m="135450">about</span>
  <span m="136350">280,000</span> <span m="137160">cancers.</span> <span m="137740">And</span>
  <span m="137880">once</span> <span m="138120">we</span> <span m="138450">kind</span>
  <span m="138630">of</span> <span m="138690">filtered--</span> <span m="138940">so</span>
  <span m="139140">at</span> <span m="139200">least</span> <span m="139380">one</span>
  <span m="139530">year</span> <span m="139680">follow</span> <span m="140010">up,</span>
  <span m="141640">we</span> <span m="141660">ended</span> <span m="141900">up</span>
  <span m="141990">with</span> <span m="142080">this</span> <span m="142680">final</span>
  <span m="143010">setting</span> <span m="143400">where</span> <span m="143520">we</span>
  <span m="143640">had</span> <span m="144720">220,000</span> <span m="145710">mammograms</span>
  <span m="146310">for</span> <span m="146490">training</span> <span m="147660">and</span>
  <span m="147810">about</span> <span m="147990">26,000</span> <span m="148770">for</span>
  <span m="148890">development</span> <span m="149330">and</span> <span m="149400">testing.</span></p><p><span
  m="150270">And</span> <span m="150430">the way</span> <span m="150530">we</span>
  <span m="150660">had it,</span> <span m="150810">it</span> <span m="150900">all</span>
  <span m="151050">comes</span> <span m="151560">to</span> <span m="151680">say,</span>
  <span m="151880">is</span> <span m="152120">this</span> <span m="152230">a</span>
  <span m="152280">positive</span> <span m="152700">mammogram</span> <span m="153060">or</span>
  <span m="153120">not?</span> <span m="153720">We</span> <span m="153840">didn't</span>
  <span m="154020">look</span> <span m="154170">at</span> <span m="154260">what</span>
  <span m="154380">cancers</span> <span m="154770">were</span> <span m="154890">caught</span>
  <span m="155460">by</span> <span m="155670">the</span> <span m="155880">radiologists.</span>
  <span m="156220">We'd</span> <span m="156560">say, you</span> <span m="156620">know,</span>
  <span m="156720">what</span> <span m="156870">was</span> <span m="157020">cancer</span>
  <span m="157350">that</span> <span m="157440">was</span> <span m="157530">found</span>
  <span m="157710">in</span> <span m="157800">any</span> <span m="158010">means</span>
  <span m="158760">within</span> <span m="159000">a</span> <span m="159060">year?</span></p><p><span
  m="159910">And</span> <span m="160000">where we</span> <span m="160170">looked</span>
  <span m="160340">to</span> <span m="160460">was through</span> <span m="160820">the</span>
  <span m="160980">radiology,</span> <span m="161560">EHR,</span> <span m="162510">and</span>
  <span m="162720">the</span> <span m="162810">Partners--</span> <span m="163380">kind</span>
  <span m="163530">of</span> <span m="163590">five hospital</span> <span m="163950">registry.</span>
  <span m="164850">And</span> <span m="164970">there</span> <span m="165060">we</span>
  <span m="165170">were</span> <span m="165300">trying</span> <span m="165480">to</span>
  <span m="165560">save</span> <span m="165900">cancer--</span> <span m="166440">if</span>
  <span m="166710">anyway</span> <span m="167070">we</span> <span m="167160">can</span>
  <span m="167310">tell</span> <span m="167470">a</span> <span m="167520">cancer</span>
  <span m="167880">occurred,</span> <span m="168300">let's</span> <span m="168450">mart
  it</span> <span m="168720">as</span> <span m="168780">such</span> <span m="169490">regardless</span>
  <span m="169920">of what</span> <span m="170090">others</span> <span m="170300">caught</span>
  <span m="170520">on</span> <span m="170670">MRI</span> <span m="171240">or</span>
  <span m="171330">some</span> <span m="171540">kind</span> <span m="171720">of</span>
  <span m="171780">later</span> <span m="172020">stage.</span></p><p><span m="173890">And</span>
  <span m="173910">so</span> <span m="174030">the</span> <span m="174120">thing</span>
  <span m="174280">we're</span> <span m="174370">trying</span> <span m="174510">to</span>
  <span m="174600">do</span> <span m="174720">here</span> <span m="175050">is</span>
  <span m="175290">just</span> <span m="175980">mimic</span> <span m="176570">the</span>
  <span m="176670">real</span> <span m="176850">world</span> <span m="177060">of</span>
  <span m="177120">what</span> <span m="177270">are</span> <span m="177390">we</span>
  <span m="177730">trying</span> <span m="177940">to</span> <span m="178000">catch</span>
  <span m="178200">cancer.</span> <span m="179320">And</span> <span m="179370">finally,</span>
  <span m="179670">important</span> <span m="180030">details</span> <span m="180360">we</span>
  <span m="180450">always</span> <span m="180690">split</span> <span m="181800">by</span>
  <span m="181980">patient</span> <span m="182460">so</span> <span m="182580">that</span>
  <span m="183300">your</span> <span m="183630">results</span> <span m="183990">aren't</span>
  <span m="184170">just</span> <span m="184290">memorizing</span> <span m="185190">this</span>
  <span m="185290">specific</span> <span m="185670">patient</span> <span m="186000">didn't</span>
  <span m="186150">have</span> <span m="186270">cancer.</span> <span m="187030">And</span>
  <span m="187130">so</span> <span m="187260">we</span> <span m="187740">have</span>
  <span m="187860">some</span> <span m="187980">overlap</span> <span m="188190">that's
  some bad bias</span> <span m="188880">to</span> <span m="188960">have.</span></p><p><span
  m="190310">OK.</span> <span m="190630">That's</span> <span m="190810">pretty</span>
  <span m="190980">simple.</span> <span m="191350">Now</span> <span m="191490">let's</span>
  <span m="191610">go</span> <span m="191730">into</span> <span m="192030">the</span>
  <span m="192120">modeling.</span> <span m="192850">There's</span> <span m="193000">going</span>
  <span m="193120">to</span> <span m="193590">kind</span> <span m="193770">of</span>
  <span m="193830">follow</span> <span m="194070">two</span> <span m="194250">chunks.</span>
  <span m="195510">One</span> <span m="195750">chunk</span> <span m="196170">is</span>
  <span m="196320">going</span> <span m="196420">to</span> <span m="196530">be</span>
  <span m="196680">on</span> <span m="196890">the</span> <span m="196980">kind</span>
  <span m="197160">of</span> <span m="197250">general</span> <span m="197550">challenges,</span>
  <span m="198070">and</span> <span m="198160">it's</span> <span m="198240">kind</span>
  <span m="198390">of</span> <span m="198450">shared</span> <span m="198750">between</span>
  <span m="199650">the</span> <span m="199740">variety</span> <span m="200080">of</span>
  <span m="200130">projects.</span> <span m="200680">And</span> <span m="200780">next
  is</span> <span m="200850">going</span> <span m="200970">to</span> <span m="201030">be</span>
  <span m="201120">kind</span> <span m="201270">of</span> <span m="201330">more</span>
  <span m="201510">specific</span> <span m="201990">analysis</span> <span m="203190">for</span>
  <span m="203370">this</span> <span m="203490">project.</span></p><p><span m="205020">So</span>
  <span m="206010">kind</span> <span m="206160">of</span> <span m="206250">a</span>
  <span m="206280">general</span> <span m="206490">question</span> <span m="206760">you</span>
  <span m="206820">might</span> <span m="206940">be</span> <span m="207030">asking,</span>
  <span m="207990">I</span> <span m="208080">have</span> <span m="208170">some</span>
  <span m="208320">image.</span> <span m="208650">I</span> <span m="208710">have</span>
  <span m="208830">some</span> <span m="209010">outcome.</span> <span m="209430">Obviously,</span>
  <span m="209820">this</span> <span m="209960">is</span> <span m="210110">just</span>
  <span m="210330">image</span> <span m="210510">classification.</span> <span m="211470">How</span>
  <span m="211690">is</span> <span m="211830">it different</span> <span m="211940">from</span>
  <span m="212160">ImageNet?</span></p><p><span m="214330">Well,</span> <span m="214650">it's</span>
  <span m="215520">quite</span> <span m="215760">similar.</span> <span m="216090">Most</span>
  <span m="216300">lessons</span> <span m="216570">are</span> <span m="216630">shared.</span>
  <span m="217260">But</span> <span m="217410">there</span> <span m="217500">are</span>
  <span m="217560">some</span> <span m="217740">key</span> <span m="217890">differences.</span></p><p><span
  m="219190">So</span> <span m="219600">I</span> <span m="219680">gave</span> <span
  m="219810">you</span> <span m="219870">two</span> <span m="220020">examples.</span>
  <span m="220600">One</span> <span m="220700">of</span> <span m="220800">them</span>
  <span m="220830">is</span> <span m="220950">a</span> <span m="221400">scene</span>
  <span m="221670">in</span> <span m="221730">my</span> <span m="221850">kitchen.</span>
  <span m="222810">Can</span> <span m="222930">anyone</span> <span m="223110">tell</span>
  <span m="223230">me</span> <span m="223290">what</span> <span m="223380">the</span>
  <span m="223470">object</span> <span m="223800">is?</span> <span m="224040">This</span>
  <span m="224220">is</span> <span m="224550">not</span> <span m="224700">a</span>
  <span m="224760">particularly</span> <span m="225060">hard</span> <span m="225180">question.</span></p><p><span
  m="226376">AUDIENCE:</span> <span m="226593">[Intermingled voices] Dog. Bear.</span></p><p><span
  m="226810">ADAM YALA:</span> <span m="226930">Right.</span></p><p><span m="227690">AUDIENCE:</span>
  <span m="227775">Dog.</span></p><p><span m="229420">ADAM YALA:</span> <span m="229495">It</span>
  <span m="229570">is</span> <span m="229960">almost</span> <span m="230230">all</span>
  <span m="230410">of</span> <span m="230470">those</span> <span m="230650">things.</span>
  <span m="231340">So</span> <span m="231490">that</span> <span m="231610">is</span>
  <span m="231730">my</span> <span m="231970">dog,</span> <span m="232330">the</span>
  <span m="232450">best</span> <span m="232630">dog.</span> <span m="233430">OK.</span>
  <span m="233680">So</span> <span m="233860">can</span> <span m="234040">anyone</span>
  <span m="234340">tell</span> <span m="234520">me,</span> <span m="235000">now</span>
  <span m="235180">that you've</span> <span m="235300">had</span> <span m="235420">some</span>
  <span m="235540">training</span> <span m="235870">with</span> <span m="235990">Connie,</span>
  <span m="237130">if</span> <span m="237310">this</span> <span m="237460">mammogram</span>
  <span m="238280">indicates</span> <span m="238630">cancer?</span></p><p><span m="241560">Well,</span>
  <span m="241740">it</span> <span m="241830">does.</span> <span m="242310">And</span>
  <span m="242730">this</span> <span m="243360">is</span> <span m="243450">unfair</span>
  <span m="243870">for</span> <span m="243990">a</span> <span m="244020">couple</span>
  <span m="244230">of</span> <span m="244290">reasons.</span> <span m="245260">Let's</span>
  <span m="245370">go</span> <span m="245700">into,</span> <span m="245860">like,</span>
  <span m="246020">why</span> <span m="246180">this</span> <span m="246300">is</span>
  <span m="246390">hard.</span> <span m="247200">It's</span> <span m="247380">unfair</span>
  <span m="247710">in</span> <span m="247800">part</span> <span m="247920">because</span>
  <span m="248310">you</span> <span m="248370">don't</span> <span m="248520">have</span>
  <span m="248610">the</span> <span m="248670">training.</span> <span m="249000">But</span>
  <span m="249090">it's</span> <span m="249180">actually</span> <span m="249510">a</span>
  <span m="249600">much</span> <span m="249810">harder</span> <span m="250080">signal</span>
  <span m="250470">to</span> <span m="250590">learn.</span></p><p><span m="251880">So</span>
  <span m="252120">first</span> <span m="253110">let's</span> <span m="253260">kind</span>
  <span m="253410">of</span> <span m="254190">delve</span> <span m="254460">into</span>
  <span m="254730">it.</span> <span m="255630">In</span> <span m="256050">this</span>
  <span m="256260">kind</span> <span m="256410">of</span> <span m="256500">task,</span>
  <span m="256860">the</span> <span m="256950">image</span> <span m="257160">is</span>
  <span m="257220">really</span> <span m="257399">huge.</span> <span m="258180">So</span>
  <span m="258290">you</span> <span m="258360">have</span> <span m="258450">something</span>
  <span m="258660">like</span> <span m="258810">a</span> <span m="258870">3,200</span>
  <span m="259920">by</span> <span m="260390">2,600</span> <span m="260970">pixel</span>
  <span m="261480">image.</span> <span m="261810">This</span> <span m="261930">is</span>
  <span m="262019">a</span> <span m="262050">single</span> <span m="262350">view</span>
  <span m="262560">of</span> <span m="262620">a</span> <span m="262680">breast.</span>
  <span m="263460">And</span> <span m="263610">in</span> <span m="263820">that,</span>
  <span m="264150">the</span> <span m="264570">actual</span> <span m="264870">cancer</span>
  <span m="265160">they're looking for</span> <span m="265450">might</span> <span
  m="265580">be</span> <span m="265680">50</span> <span m="265890">by</span> <span
  m="266010">50</span> <span m="266220">pixels.</span> <span m="267030">So</span>
  <span m="267300">intuitively</span> <span m="267820">your</span> <span m="267900">signal</span>
  <span m="268200">to</span> <span m="268290">noise</span> <span m="268470">ratio</span>
  <span m="268670">is</span> <span m="268740">very</span> <span m="268980">different.</span></p><p><span
  m="269780">Whereas</span> <span m="269910">an</span> <span m="270000">image</span>
  <span m="270320">that--</span> <span m="270780">my</span> <span m="270990">dog</span>
  <span m="271230">is</span> <span m="271290">like</span> <span m="271440">the</span>
  <span m="271530">entire</span> <span m="271830">image.</span> <span m="272150">She's</span>
  <span m="272220">huge</span> <span m="273180">in</span> <span m="273360">real</span>
  <span m="273510">life</span> <span m="273750">and</span> <span m="273870">in</span>
  <span m="273930">that</span> <span m="274020">photo.</span></p><p><span m="275130">And</span>
  <span m="275400">the</span> <span m="275520">image</span> <span m="275760">itself</span>
  <span m="276000">is</span> <span m="276120">much</span> <span m="276240">smaller.</span>
  <span m="276720">So not</span> <span m="276900">only</span> <span m="277110">do</span>
  <span m="277170">you</span> <span m="277230">have much</span> <span m="277500">smaller</span>
  <span m="277890">images,</span> <span m="279030">but</span> <span m="279300">you're</span>
  <span m="279690">kind</span> <span m="279930">of,</span> <span m="280020">like,</span>
  <span m="280200">the</span> <span m="280290">relative</span> <span m="280680">size</span>
  <span m="280950">of the</span> <span m="281040">object</span> <span m="281410">in</span>
  <span m="281520">there</span> <span m="281670">is</span> <span m="281760">much</span>
  <span m="281940">larger.</span></p><p><span m="282615">To</span> <span m="282930">kind</span>
  <span m="283110">of</span> <span m="283170">further</span> <span m="283470">compound
  the</span> <span m="283920">difficulty,</span> <span m="284520">the</span> <span
  m="284610">pattern</span> <span m="285090">you're</span> <span m="285180">looking</span>
  <span m="285450">for</span> <span m="285840">inside</span> <span m="287100">the</span>
  <span m="287310">mammogram</span> <span m="287820">is</span> <span m="287910">really</span>
  <span m="288120">context-dependent.</span> <span m="289540">So</span> <span m="289860">if</span>
  <span m="290010">you</span> <span m="290100">saw</span> <span m="290280">that</span>
  <span m="290430">pattern</span> <span m="291420">somewhere</span> <span m="291780">else</span>
  <span m="292020">in</span> <span m="292080">the</span> <span m="292140">breast,</span>
  <span m="292440">it</span> <span m="292600">doesn't</span> <span m="292860">indicate</span>
  <span m="293190">the</span> <span m="293280">same</span> <span m="293460">thing.</span>
  <span m="294900">And</span> <span m="295020">so</span> <span m="295140">you</span>
  <span m="295230">really</span> <span m="295440">care</span> <span m="295620">about</span>
  <span m="296010">where</span> <span m="296280">in</span> <span m="296550">this</span>
  <span m="296670">kind</span> <span m="296820">of</span> <span m="296880">global</span>
  <span m="297150">context</span> <span m="297930">this</span> <span m="298080">comes</span>
  <span m="298290">out.</span> <span m="298530">And</span> <span m="298770">if</span>
  <span m="298890">you</span> <span m="299010">kind</span> <span m="299160">of</span>
  <span m="299250">take</span> <span m="299400">the</span> <span m="299490">mammogram</span>
  <span m="299910">at</span> <span m="300210">different</span> <span m="300510">times</span>
  <span m="300960">with</span> <span m="301050">different</span> <span m="301290">compressions,</span>
  <span m="302060">you</span> <span m="302180">would</span> <span m="302280">have</span>
  <span m="302400">this</span> <span m="302550">kind</span> <span m="302700">of</span>
  <span m="302760">non-rigid</span> <span m="304140">morphing</span> <span m="304650">of</span>
  <span m="304770">the</span> <span m="304920">image</span> <span m="305310">that's</span>
  <span m="305520">much</span> <span m="305760">more</span> <span m="305850">difficult</span>
  <span m="306150">to</span> <span m="306240">model.</span> <span m="306960">Whereas</span>
  <span m="307260">that's</span> <span m="307440">a</span> <span m="307470">more</span>
  <span m="307710">or</span> <span m="307740">less</span> <span m="307920">context-independent</span>
  <span m="308790">dog.</span></p><p><span m="309330">You</span> <span m="309420">see</span>
  <span m="309570">that</span> <span m="309660">kind</span> <span m="309840">of</span>
  <span m="310290">frame</span> <span m="310800">kind</span> <span m="311010">of</span>
  <span m="311100">anywhere,</span> <span m="311520">you</span> <span m="311640">know</span>
  <span m="311880">it's</span> <span m="312000">a</span> <span m="312030">dog.</span>
  <span m="312360">And</span> <span m="312450">so</span> <span m="312570">it's</span>
  <span m="312660">a</span> <span m="312690">much</span> <span m="312900">easier</span>
  <span m="313200">thing</span> <span m="313950">to</span> <span m="314100">learn</span>
  <span m="314490">in</span> <span m="314620">a</span> <span m="314910">traditional</span>
  <span m="315300">computer</span> <span m="315570">vision</span> <span m="315780">setting.</span></p><p><span
  m="317470">And</span> <span m="317490">so</span> <span m="317640">the</span> <span
  m="318000">core</span> <span m="318270">challenge</span> <span m="318660">here</span>
  <span m="318810">is</span> <span m="318880">that</span> <span m="318960">both</span>
  <span m="319230">the</span> <span m="319290">image</span> <span m="319510">is</span>
  <span m="319590">too</span> <span m="319770">big</span> <span m="320040">and</span>
  <span m="320220">too</span> <span m="320400">small.</span> <span m="321340">So</span>
  <span m="321390">if</span> <span m="321480">you're</span> <span m="321540">looking</span>
  <span m="321690">at</span> <span m="321750">just</span> <span m="322350">the</span>
  <span m="322440">number</span> <span m="322650">of</span> <span m="322710">cancers</span>
  <span m="323010">we</span> <span m="323130">have,</span> <span m="324600">the</span>
  <span m="324720">cancer</span> <span m="325080">might</span> <span m="325200">be</span>
  <span m="325290">less</span> <span m="325440">than</span> <span m="325530">1%</span>
  <span m="325920">of</span> <span m="325980">the</span> <span m="326040">mammogram</span>
  <span m="327030">and</span> <span m="327180">about</span> <span m="327420">0.7%</span>
  <span m="328410">of</span> <span m="328510">your</span> <span m="328560">images</span>
  <span m="328860">have</span> <span m="329070">cancers,</span> <span m="329610">even</span>
  <span m="329850">in</span> <span m="329910">this</span> <span m="330030">data</span>
  <span m="330220">set,</span> <span m="330420">which</span> <span m="330570">is</span>
  <span m="331590">from</span> <span m="331710">2000</span> <span m="332000">to</span>
  <span m="332130">2016</span> <span m="332560">MGH,</span> <span m="333150">a</span>
  <span m="333210">massive</span> <span m="333540">imaging</span> <span m="333810">center,</span>
  <span m="334500">in</span> <span m="334650">total</span> <span m="335070">across</span>
  <span m="335340">all</span> <span m="335550">of</span> <span m="335640">that,</span>
  <span m="335820">you will</span> <span m="336060">still</span> <span m="336360">have</span>
  <span m="336600">less</span> <span m="337500">than</span> <span m="337590">2,000</span>
  <span m="337920">cancers.</span></p><p><span m="339220">And</span> <span m="339240">this</span>
  <span m="339390">is</span> <span m="339450">super</span> <span m="339810">tiny</span>
  <span m="340230">compared</span> <span m="340560">to</span> <span m="340830">regular</span>
  <span m="341370">object</span> <span m="341670">classification</span> <span m="342120">data</span>
  <span m="342380">sets.</span> <span m="343710">And</span> <span m="343800">this</span>
  <span m="343950">is</span> <span m="344070">looking</span> <span m="344670">at</span>
  <span m="344760">over</span> <span m="344940">a</span> <span m="344970">million</span>
  <span m="345240">images</span> <span m="345630">if you</span> <span m="345690">look</span>
  <span m="345810">at</span> <span m="345870">all</span> <span m="345990">the</span>
  <span m="346080">four</span> <span m="346260">views</span> <span m="347070">of</span>
  <span m="347190">the</span> <span m="347400">exams.</span> <span m="348350">And</span>
  <span m="348480">at</span> <span m="348540">the</span> <span m="348630">same</span>
  <span m="348810">time,</span> <span m="349090">it's</span> <span m="349190">also</span>
  <span m="349260">too</span> <span m="349410">big.</span></p><p><span m="349830">So</span>
  <span m="351210">even</span> <span m="351420">if</span> <span m="351510">I</span>
  <span m="351620">downsample</span> <span m="352050">these</span> <span m="352200">images,</span>
  <span m="352740">I</span> <span m="352830">can</span> <span m="353490">only</span>
  <span m="353790">really</span> <span m="354000">fit</span> <span m="354300">three</span>
  <span m="354600">of</span> <span m="354660">them</span> <span m="354870">for</span>
  <span m="355020">a</span> <span m="355050">single</span> <span m="355340">GPU.</span>
  <span m="356670">And</span> <span m="356790">so</span> <span m="356910">this</span>
  <span m="357030">kind</span> <span m="357180">of</span> <span m="357240">limits</span>
  <span m="357510">the</span> <span m="357570">batch size</span> <span m="358050">I</span>
  <span m="358080">can</span> <span m="358230">work</span> <span m="358380">with.</span>
  <span m="359510">And</span> <span m="360090">whereas</span> <span m="360690">the</span>
  <span m="360780">kind</span> <span m="360930">of</span> <span m="360990">comparable,</span>
  <span m="361420">if I took</span> <span m="361680">just</span> <span m="361850">the</span>
  <span m="361950">regular</span> <span m="362310">image</span> <span m="362580">net</span>
  <span m="362670">size,</span> <span m="362970">I</span> <span m="363000">could</span>
  <span m="363120">fit</span> <span m="363360">batches</span> <span m="363840">of</span>
  <span m="363930">128,</span> <span m="364980">easily</span> <span m="365340">happy</span>
  <span m="365580">days</span> <span m="365880">and do</span> <span m="366030">all</span>
  <span m="366090">this</span> <span m="366220">parallelization</span> <span m="366630">stuff,</span>
  <span m="366880">and it's</span> <span m="367140">just</span> <span m="367290">much</span>
  <span m="367470">easier</span> <span m="367650">to</span> <span m="367740">play</span>
  <span m="367890">with.</span></p><p><span m="368920">And</span> <span m="368970">finally,</span>
  <span m="369770">the</span> <span m="369870">actual</span> <span m="369980">data</span>
  <span m="370220">set</span> <span m="370350">itself</span> <span m="370590">is</span>
  <span m="370680">quite</span> <span m="370860">large.</span> <span m="371130">And</span>
  <span m="371220">so you</span> <span m="371270">have</span> <span m="371370">to</span>
  <span m="371430">do</span> <span m="371580">some--</span> <span m="372490">there's</span>
  <span m="372780">nuisances</span> <span m="373230">to</span> <span m="373320">deal</span>
  <span m="373500">with</span> <span m="373650">in</span> <span m="373740">terms</span>
  <span m="373950">of,</span> <span m="374010">like,</span> <span m="374190">just</span>
  <span m="374340">setting</span> <span m="374700">up</span> <span m="374850">your</span>
  <span m="374970">server</span> <span m="375270">infrastructure</span> <span m="375720">to</span>
  <span m="375810">handle</span> <span m="376080">these</span> <span m="376200">massive</span>
  <span m="376560">data</span> <span m="376860">sets,</span> <span m="378080">also</span>
  <span m="378360">be</span> <span m="378450">able</span> <span m="378600">to</span>
  <span m="378690">train</span> <span m="378870">efficiently.</span></p><p><span m="381730">So</span>
  <span m="382510">you</span> <span m="382550">know,</span> <span m="382780">the</span>
  <span m="382840">core</span> <span m="383030">challenge</span> <span m="383410">here</span>
  <span m="383770">across</span> <span m="384070">all</span> <span m="384250">of</span>
  <span m="384310">these</span> <span m="384850">kind</span> <span m="385060">of</span>
  <span m="385120">tasks</span> <span m="385480">is,</span> <span m="385570">how</span>
  <span m="385690">do</span> <span m="385780">we</span> <span m="385840">make</span>
  <span m="385990">this</span> <span m="386110">model</span> <span m="386380">actually</span>
  <span m="386710">learn?</span> <span m="387310">The</span> <span m="387400">core</span>
  <span m="387580">problem</span> <span m="387940">is</span> <span m="388030">that</span>
  <span m="388270">our</span> <span m="388440">signal</span> <span m="388710">to noise
  ratio</span> <span m="389010">is</span> <span m="389110">quite</span> <span m="389320">low.</span>
  <span m="389690">So</span> <span m="389740">training</span> <span m="389980">ends</span>
  <span m="390100">up</span> <span m="390190">being</span> <span m="390340">quite</span>
  <span m="390590">unstable.</span></p><p><span m="391540">And</span> <span m="392290">there's</span>
  <span m="392470">a</span> <span m="392500">kind</span> <span m="392710">of</span>
  <span m="392790">a</span> <span m="393040">couple</span> <span m="393250">of</span>
  <span m="393310">simple</span> <span m="393550">levers</span> <span m="393820">you</span>
  <span m="393880">can</span> <span m="394000">play</span> <span m="394150">with.</span>
  <span m="394780">The</span> <span m="394900">first</span> <span m="395170">lever</span>
  <span m="395470">is</span> <span m="396040">often</span> <span m="396430">deep</span>
  <span m="396710">learning</span> <span m="396880">initialization.</span></p><p><span
  m="398860">Next,</span> <span m="399330">we're</span> <span m="399390">gonna</span>
  <span m="399520">talk</span> <span m="399670">about</span> <span m="399820">kind</span>
  <span m="399970">of the</span> <span m="400110">optimization</span> <span m="400720">or</span>
  <span m="400860">architecture</span> <span m="401260">choice</span> <span m="401920">and</span>
  <span m="402010">how</span> <span m="402160">this</span> <span m="402310">compares</span>
  <span m="402700">to</span> <span m="402790">what</span> <span m="402880">people</span>
  <span m="403660">often</span> <span m="403960">do</span> <span m="404260">in</span>
  <span m="404350">the</span> <span m="404410">community,</span> <span m="404990">including</span>
  <span m="405310">in</span> <span m="405430">a</span> <span m="405460">recent</span>
  <span m="405730">paper</span> <span m="405970">from</span> <span m="406150">yesterday.</span></p><p><span
  m="407600">And</span> <span m="407620">then</span> <span m="407710">finally,</span>
  <span m="408040">we're</span> <span m="408150">gonna</span> <span m="408220">talk</span>
  <span m="408400">about something</span> <span m="408700">more</span> <span m="408850">explicit</span>
  <span m="409330">for</span> <span m="409480">the</span> <span m="409570">triage</span>
  <span m="409990">idea</span> <span m="410740">and</span> <span m="410860">how</span>
  <span m="410950">we</span> <span m="411040">actually</span> <span m="411280">use</span>
  <span m="411460">this</span> <span m="411580">model</span> <span m="411820">once</span>
  <span m="411960">it's</span> <span m="412030">trained.</span></p><p><span m="413880">OK.</span>
  <span m="414220">So</span> <span m="414670">before</span> <span m="415000">I</span>
  <span m="415060">go</span> <span m="415360">into</span> <span m="415540">how</span>
  <span m="415720">we</span> <span m="415840">made</span> <span m="416050">these</span>
  <span m="416200">choices,</span> <span m="416650">I'm</span> <span m="416710">just</span>
  <span m="416800">going</span> <span m="416920">to</span> <span m="416980">say</span>
  <span m="417070">what</span> <span m="417220">we</span> <span m="417310">chose</span>
  <span m="417610">to</span> <span m="417700">give</span> <span m="417820">you</span>
  <span m="418090">context</span> <span m="418930">before</span> <span m="419230">I</span>
  <span m="419440">dive</span> <span m="419710">in.</span> <span m="420830">So</span>
  <span m="420910">we</span> <span m="421120">followed</span> <span m="421420">some</span>
  <span m="421720">image</span> <span m="421930">initialization.</span> <span m="423190">We</span>
  <span m="423310">use</span> <span m="423460">a</span> <span m="423490">relatively</span>
  <span m="423910">large</span> <span m="424150">batch</span> <span m="424330">size-ish</span>
  <span m="425320">of</span> <span m="425470">24.</span> <span m="426160">And</span>
  <span m="426420">the</span> <span m="426610">way</span> <span m="426700">we</span>
  <span m="426790">do</span> <span m="426910">that is</span> <span m="427060">by</span>
  <span m="427270">taking</span> <span m="427570">4</span> <span m="428050">GPUs</span>
  <span m="428320">and just</span> <span m="428500">stepping</span> <span m="428950">a</span>
  <span m="429010">couple</span> <span m="429190">of</span> <span m="429250">times</span>
  <span m="429490">before</span> <span m="429700">doing</span> <span m="430060">an</span>
  <span m="430150">optimizer</span> <span m="430570">step.</span></p><p><span m="431300">So</span>
  <span m="431320">when</span> <span m="431370">you</span> <span m="431470">do</span>
  <span m="431560">a</span> <span m="431590">couple</span> <span m="431810">rounds</span>
  <span m="432400">of</span> <span m="432490">back</span> <span m="432760">prop</span>
  <span m="433030">first</span> <span m="433670">to</span> <span m="433820">accumulate</span>
  <span m="434160">those</span> <span m="434340">gradients</span> <span m="434690">before</span>
  <span m="434860">doing</span> <span m="435700">optimization.</span> <span m="436710">And</span>
  <span m="436840">you</span> <span m="436900">sample</span> <span m="437170">balanced</span>
  <span m="437530">batches</span> <span m="437830">of</span> <span m="437890">training</span>
  <span m="438160">time.</span></p><p><span m="438760">And</span> <span m="438940">for</span>
  <span m="439170">backbone</span> <span m="439540">architecture</span> <span m="440020">we</span>
  <span m="440110">use</span> <span m="440320">ResNet-18.</span> <span m="440950">It's</span>
  <span m="441130">just</span> <span m="441310">kind</span> <span m="441520">of,</span>
  <span m="441580">like,</span> <span m="441880">fairly</span> <span m="442210">standard.</span></p><p><span
  m="443860">OK.</span> <span m="444250">But</span> <span m="444730">as</span> <span
  m="444850">I</span> <span m="444910">said</span> <span m="445030">before,</span>
  <span m="445550">one</span> <span m="445600">of</span> <span m="445660">the</span>
  <span m="445720">first</span> <span m="446050">key</span> <span m="446200">decisions</span>
  <span m="446770">is</span> <span m="446890">how</span> <span m="447040">do</span>
  <span m="447100">you</span> <span m="447160">think</span> <span m="447400">about
  your</span> <span m="447610">initialization?</span> <span m="449620">So</span> <span
  m="449830">this</span> <span m="450520">is</span> <span m="450610">a</span> <span
  m="450640">figure</span> <span m="451030">of</span> <span m="451900">ImageNet</span>
  <span m="452370">initialization</span> <span m="452890">versus</span> <span m="453010">random</span>
  <span m="453100">initialization.</span> <span m="453850">It's</span> <span m="454000">not</span>
  <span m="454150">any</span> <span m="454390">particular</span> <span m="454870">experiment.</span>
  <span m="456190">I've</span> <span m="456310">done</span> <span m="456460">this</span>
  <span m="456940">across</span> <span m="457210">many,</span> <span m="457550">many</span>
  <span m="457600">times.</span> <span m="457870">It's</span> <span m="457990">always</span>
  <span m="458260">like</span> <span m="458410">this.</span> <span m="459040">Where</span>
  <span m="459340">if</span> <span m="459490">you</span> <span m="459670">use</span>
  <span m="459940">image</span> <span m="460190">initialization,</span> <span m="461200">your</span>
  <span m="461320">loss</span> <span m="461650">drops</span> <span m="461920">immediately,</span>
  <span m="463240">both</span> <span m="463510">in</span> <span m="463600">train</span>
  <span m="463840">loss</span> <span m="464050">and</span> <span m="464140">development</span>
  <span m="464530">loss</span> <span m="464800">when you</span> <span m="464860">actually</span>
  <span m="465040">learn</span> <span m="465220">something.</span> <span m="466330">Whereas</span>
  <span m="466780">when</span> <span m="466870">you</span> <span m="467020">do</span>
  <span m="467080">random</span> <span m="467380">initialization,</span> <span m="468610">you</span>
  <span m="468760">kind</span> <span m="468970">of</span> <span m="469060">don't</span>
  <span m="469240">learn</span> <span m="469420">anything.</span> <span m="469940">And</span>
  <span m="470040">your</span> <span m="470140">loss</span> <span m="470230">kind</span>
  <span m="470380">of</span> <span m="470440">bounds</span> <span m="470830">around</span>
  <span m="471130">the</span> <span m="471220">top</span> <span m="471550">for</span>
  <span m="471700">a</span> <span m="471730">very</span> <span m="472000">long</span>
  <span m="472210">time</span> <span m="472420">before</span> <span m="472600">it</span>
  <span m="472690">finds</span> <span m="473620">some</span> <span m="473830">region</span>
  <span m="474190">where it</span> <span m="474340">quickly</span> <span m="474760">starts</span>
  <span m="474970">learning.</span> <span m="475300">And</span> <span m="475390">then
  it will</span> <span m="475540">plateau</span> <span m="475930">again</span> <span
  m="476140">for</span> <span m="476260">a</span> <span m="476290">long</span> <span
  m="476440">time</span> <span m="476950">before</span> <span m="477190">quickly</span>
  <span m="477430">start</span> <span m="477610">learning.</span></p><p><span m="478780">And</span>
  <span m="479380">to</span> <span m="479550">kind</span> <span m="479710">of</span>
  <span m="479770">give</span> <span m="479860">some</span> <span m="479980">context,</span>
  <span m="480460">to</span> <span m="480550">give</span> <span m="480730">about</span>
  <span m="480940">50</span> <span m="481270">epochs</span> <span m="482230">takes</span>
  <span m="482560">on</span> <span m="482650">the</span> <span m="482740">order</span>
  <span m="483130">of,</span> <span m="483220">like,</span> <span m="483790">15,</span>
  <span m="484400">16</span> <span m="484720">hours.</span> <span m="486140">And</span>
  <span m="486280">so</span> <span m="486940">to</span> <span m="487120">wait</span>
  <span m="487390">long</span> <span m="487690">enough</span> <span m="487900">to</span>
  <span m="488020">even</span> <span m="488290">see</span> <span m="488800">if</span>
  <span m="488950">random</span> <span m="489270">initialization</span> <span m="489580">could</span>
  <span m="489690">perform</span> <span m="489970">as</span> <span m="490060">well</span>
  <span m="490540">is</span> <span m="490750">beyond</span> <span m="491050">my</span>
  <span m="491170">level</span> <span m="491380">of</span> <span m="491440">patience.</span>
  <span m="492670">It</span> <span m="492760">just</span> <span m="492910">takes</span>
  <span m="493090">too</span> <span m="493180">long,</span> <span m="493510">and I
  have other</span> <span m="493660">experiments</span> <span m="494020">to</span>
  <span m="494080">be</span> <span m="494140">running.</span></p><p><span m="496010">So</span>
  <span m="496540">this</span> <span m="496720">is</span> <span m="496900">more</span>
  <span m="497050">of</span> <span m="497110">an</span> <span m="497170">empirical</span>
  <span m="497560">observation</span> <span m="498100">that</span> <span m="498400">the</span>
  <span m="498740">image</span> <span m="499080">initialization</span> <span m="499570">learns</span>
  <span m="499810">immediately.</span> <span m="500290">And</span> <span m="500380">there's</span>
  <span m="500590">some kind</span> <span m="500740">of</span> <span m="500800">questions</span>
  <span m="501130">of</span> <span m="501400">why</span> <span m="501730">is</span>
  <span m="501910">this?</span> <span m="503320">Our</span> <span m="503440">theoretical</span>
  <span m="503770">understanding</span> <span m="504000">of</span> <span m="504060">this</span>
  <span m="504190">is</span> <span m="504520">not</span> <span m="504760">that</span>
  <span m="504910">strong.</span> <span m="505330">We</span> <span m="505480">have</span>
  <span m="505600">some</span> <span m="505750">intuitions</span> <span m="506290">of</span>
  <span m="506350">why</span> <span m="506470">this</span> <span m="506590">might</span>
  <span m="506710">be</span> <span m="506800">happening.</span></p><p><span m="507710">We</span>
  <span m="508270">don't</span> <span m="508570">think</span> <span m="508780">it's</span>
  <span m="508900">anything</span> <span m="509200">about</span> <span m="509860">this</span>
  <span m="510040">particular</span> <span m="510520">filter</span> <span m="511330">of</span>
  <span m="511450">this</span> <span m="511600">dog</span> <span m="511930">is</span>
  <span m="512020">really</span> <span m="512260">great</span> <span m="512530">for</span>
  <span m="512620">breast</span> <span m="512799">cancer.</span> <span m="514030">That's</span>
  <span m="514240">quite</span> <span m="514570">implausible.</span> <span m="515080">But</span>
  <span m="515169">if</span> <span m="515230">you</span> <span m="515289">look</span>
  <span m="515429">it</span> <span m="515500">into</span> <span m="515740">a</span>
  <span m="515799">lot</span> <span m="515980">of</span> <span m="516070">the</span>
  <span m="516159">earlier</span> <span m="516500">research</span> <span m="516940">in</span>
  <span m="517030">terms</span> <span m="517299">of</span> <span m="517929">the</span>
  <span m="518049">right</span> <span m="518289">kind</span> <span m="518620">of</span>
  <span m="518710">random</span> <span m="519110">initialization</span> <span m="519700">for</span>
  <span m="519850">things</span> <span m="520059">like</span> <span m="520179">revenue</span>
  <span m="520450">networks,</span> <span m="520870">a</span> <span m="520929">lot</span>
  <span m="521110">of</span> <span m="521169">focus</span> <span m="521590">was</span>
  <span m="521740">on</span> <span m="522520">does the</span> <span m="522789">activation</span>
  <span m="523360">pattern</span> <span m="523990">not</span> <span m="524200">blow</span>
  <span m="524410">up</span> <span m="524530">as</span> <span m="524620">you</span>
  <span m="524680">go</span> <span m="524800">further</span> <span m="525040">down</span>
  <span m="525190">the</span> <span m="525280">line.</span></p><p><span m="525890">One</span>
  <span m="526030">of</span> <span m="526090">the</span> <span m="526180">benefits</span>
  <span m="526540">of</span> <span m="527350">starting</span> <span m="527620">with</span>
  <span m="527710">the</span> <span m="527770">pre-trained</span> <span m="528070">network</span>
  <span m="528460">is</span> <span m="528580">that</span> <span m="529150">a</span>
  <span m="529240">lot</span> <span m="529510">of</span> <span m="529600">those</span>
  <span m="530260">kind</span> <span m="530440">of</span> <span m="530500">dynamics
  are</span> <span m="530950">already</span> <span m="531160">figured</span> <span
  m="531400">out</span> <span m="531490">for</span> <span m="531620">a</span> <span
  m="531640">specific</span> <span m="532090">task.</span> <span m="532810">And</span>
  <span m="532930">so</span> <span m="533200">shifting</span> <span m="533590">from</span>
  <span m="533740">that</span> <span m="534040">to</span> <span m="534340">other</span>
  <span m="534580">tasks</span> <span m="535680">has</span> <span m="536050">seemed</span>
  <span m="536320">to</span> <span m="536410">be</span> <span m="536470">not</span>
  <span m="536630">that</span> <span m="536690">challenging.</span></p><p><span m="537070">Another</span>
  <span m="537280">possible</span> <span m="537750">area of</span> <span m="538060">explanation</span>
  <span m="539050">is</span> <span m="539200">actually</span> <span m="539470">in
  a</span> <span m="539550">BatchNorm</span> <span m="539920">statistics.</span> <span
  m="540530">So</span> <span m="540550">if</span> <span m="540640">you</span> <span
  m="540700">remember,</span> <span m="541130">we</span> <span m="541230">can</span>
  <span m="541330">only</span> <span m="541500">fit</span> <span m="541720">three</span>
  <span m="541990">images</span> <span m="542290">per</span> <span m="542380">GPU.</span>
  <span m="543310">And</span> <span m="543430">the</span> <span m="543490">way</span>
  <span m="543620">the</span> <span m="543710">BatchNorm</span> <span m="543990">initialization</span>
  <span m="544370">is</span> <span m="544480">implemented</span> <span m="545410">across</span>
  <span m="546370">every</span> <span m="547000">deep</span> <span m="547240">learning</span>
  <span m="547480">library</span> <span m="547780">that</span> <span m="547930">I</span>
  <span m="548050">know</span> <span m="548200">of,</span> <span m="548320">it</span>
  <span m="548380">computes</span> <span m="548740">independently</span> <span m="549300">per</span>
  <span m="549480">GPU</span> <span m="550330">to</span> <span m="550480">minimize</span>
  <span m="550930">the</span> <span m="551020">kind</span> <span m="551170">of</span>
  <span m="551260">inter-GPU</span> <span m="551800">communication.</span> <span m="552880">And</span>
  <span m="552970">so</span> <span m="553150">it's</span> <span m="553240">also</span>
  <span m="553450">less</span> <span m="553680">able</span> <span m="553930">to</span>
  <span m="554140">kind</span> <span m="554350">of</span> <span m="554990">guess</span>
  <span m="555280">from</span> <span m="555430">scratch.</span> <span m="555850">But</span>
  <span m="555970">if</span> <span m="556060">you're</span> <span m="556150">starting</span>
  <span m="556540">with</span> <span m="556670">the</span> <span m="556720">BatchNorm</span>
  <span m="557170">statistics</span> <span m="557535">to</span> <span m="557900">ImageNet</span>
  <span m="558480">and</span> <span m="558580">just</span> <span m="558680">slowly</span>
  <span m="559090">shifting</span> <span m="559420">it</span> <span m="559510">over,</span>
  <span m="559920">it</span> <span m="560170">might</span> <span m="560290">also</span>
  <span m="560560">result</span> <span m="560860">in</span> <span m="560920">some</span>
  <span m="561070">stability</span> <span m="561430">benefits.</span></p><p><span
  m="564820">But</span> <span m="564970">in</span> <span m="565060">general,</span>
  <span m="565510">or</span> <span m="565660">like,</span> <span m="566260">a</span>
  <span m="566320">true</span> <span m="566590">deeper</span> <span m="566980">theoretical</span>
  <span m="567060">understanding,</span> <span m="567570">but as</span> <span m="567760">I</span>
  <span m="567920">said,</span> <span m="568150">it still</span> <span m="568330">eludes</span>
  <span m="568660">us.</span> <span m="569110">And</span> <span m="569230">it</span>
  <span m="569470">isn't</span> <span m="570940">something</span> <span m="571210">I</span>
  <span m="571270">can</span> <span m="571690">give</span> <span m="571990">too</span>
  <span m="572140">much</span> <span m="572290">conclusions</span> <span m="572650">about,</span>
  <span m="572860">unfortunately.</span></p><p><span m="574440">OK.</span> <span m="574660">So</span>
  <span m="575080">that's</span> <span m="575410">initialization.</span> <span m="575980">And</span>
  <span m="576070">if</span> <span m="576130">you</span> <span m="576190">don't</span>
  <span m="576340">get</span> <span m="576430">this</span> <span m="576550">right,</span>
  <span m="576760">kind</span> <span m="576950">of</span> <span m="577100">nothing</span>
  <span m="577360">works</span> <span m="577570">for</span> <span m="577660">a</span>
  <span m="577690">very</span> <span m="577870">long</span> <span m="578050">time.</span>
  <span m="578690">So</span> <span m="579340">if</span> <span m="579430">you're</span>
  <span m="579490">gonna</span> <span m="579640">start a</span> <span m="579820">project</span>
  <span m="580050">in this</span> <span m="580150">space,</span> <span m="580630">try</span>
  <span m="580810">this.</span></p><p><span m="581680">Next,</span> <span m="582280">another</span>
  <span m="582610">important</span> <span m="582880">decision</span> <span m="583210">that</span>
  <span m="583300">if</span> <span m="583390">you</span> <span m="583450">don't</span>
  <span m="583660">do, it</span> <span m="583930">kind</span> <span m="584110">of</span>
  <span m="584170">breaks,</span> <span m="585220">is</span> <span m="585430">your</span>
  <span m="585530">optimization/architecture</span> <span m="586540">choice.</span>
  <span m="587740">So</span> <span m="587860">as</span> <span m="587950">I</span>
  <span m="588010">said</span> <span m="588130">before,</span> <span m="588430">kind</span>
  <span m="588580">of</span> <span m="588820">a</span> <span m="588880">core</span>
  <span m="589150">problem</span> <span m="589650">in stability</span> <span m="590140">here</span>
  <span m="590320">is</span> <span m="590440">this</span> <span m="590590">idea</span>
  <span m="590920">that</span> <span m="591570">our</span> <span m="591670">just</span>
  <span m="591820">signal</span> <span m="592140">to</span> <span m="592210">noise</span>
  <span m="592420">ratio</span> <span m="592600">is</span> <span m="592690">really</span>
  <span m="592900">low.</span> <span m="594070">And</span> <span m="594220">so</span>
  <span m="594490">a</span> <span m="594550">very</span> <span m="594760">common</span>
  <span m="595120">approach</span> <span m="595630">throughout</span> <span m="596380">a</span>
  <span m="596440">lot</span> <span m="596590">of</span> <span m="596680">the prior</span>
  <span m="596950">work</span> <span m="597190">and</span> <span m="597280">things</span>
  <span m="597460">I</span> <span m="597520">actually</span> <span m="597760">have</span>
  <span m="597850">tried</span> <span m="598030">myself</span> <span m="598300">before</span>
  <span m="599140">is</span> <span m="599590">to</span> <span m="599680">say,</span>
  <span m="600470">OK,</span> <span m="601520">let's</span> <span m="601600">just</span>
  <span m="601750">break</span> <span m="602000">down</span> <span m="602140">this</span>
  <span m="602260">problem.</span> <span m="602860">We</span> <span m="602980">can</span>
  <span m="603280">train</span> <span m="603880">at</span> <span m="604120">a</span>
  <span m="604270">patch</span> <span m="604630">level</span> <span m="604840">first.</span>
  <span m="605110">We're</span> <span m="605170">going</span> <span m="605290">to</span>
  <span m="605350">take</span> <span m="605470">just</span> <span m="605710">subsets</span>
  <span m="606340">of</span> <span m="606430">a</span> <span m="606520">mammogram</span>
  <span m="607060">in</span> <span m="607330">this</span> <span m="607600">little</span>
  <span m="607750">bonding</span> <span m="608020">box,</span> <span m="608320">have</span>
  <span m="608460">it</span> <span m="608590">annotated</span> <span m="609130">for</span>
  <span m="609280">radiology</span> <span m="609850">findings</span> <span m="610360">like</span>
  <span m="610960">benign</span> <span m="611350">masses</span> <span m="611860">or</span>
  <span m="611950">calcification</span> <span m="612250">and</span> <span m="612550">things</span>
  <span m="612730">of</span> <span m="612790">that</span> <span m="612910">sort.</span></p><p><span
  m="614020">We're</span> <span m="614170">going</span> <span m="614290">to</span>
  <span m="614410">pre-train</span> <span m="615100">on</span> <span m="615190">that</span>
  <span m="615370">task</span> <span m="615870">to</span> <span m="615990">have</span>
  <span m="616090">this</span> <span m="616240">kind</span> <span m="616360">of</span>
  <span m="616420">pixel</span> <span m="616720">level</span> <span m="616930">prediction.</span>
  <span m="617890">And</span> <span m="617980">then</span> <span m="618100">once</span>
  <span m="618220">we're</span> <span m="618300">done</span> <span m="618430">with</span>
  <span m="618550">that,</span> <span m="618800">we're</span> <span m="618900">going</span>
  <span m="619000">to</span> <span m="619100">fine</span> <span m="619330">tune</span>
  <span m="619600">that</span> <span m="619750">initialized</span> <span m="620170">model</span>
  <span m="620950">across</span> <span m="621640">the</span> <span m="622060">entire</span>
  <span m="623260">image.</span> <span m="624280">So</span> <span m="624380">you</span>
  <span m="624480">kind of</span> <span m="624580">have</span> <span m="624680">this</span>
  <span m="624780">two-stage</span> <span m="625330">training</span> <span m="625720">procedure.</span></p><p><span
  m="626860">And</span> <span m="627010">actually,</span> <span m="627280">another</span>
  <span m="627490">paper</span> <span m="627730">that</span> <span m="627820">came</span>
  <span m="628030">out</span> <span m="628510">just</span> <span m="628720">yesterday</span>
  <span m="629170">does</span> <span m="629350">the</span> <span m="629440">exact</span>
  <span m="629800">same</span> <span m="629980">approach</span> <span m="630760">with</span>
  <span m="630910">some</span> <span m="631150">slightly</span> <span m="631450">different</span>
  <span m="631690">details.</span> <span m="634600">But</span> <span m="635230">one</span>
  <span m="635380">of</span> <span m="635440">the</span> <span m="635500">things</span>
  <span m="635680">we</span> <span m="635740">wanted</span> <span m="635890">to</span>
  <span m="635960">investigate</span> <span m="636460">is</span> <span m="636590">if</span>
  <span m="636630">you</span> <span m="636700">just--</span> <span m="636970">oh,</span>
  <span m="637560">And</span> <span m="638020">the</span> <span m="638190">base</span>
  <span m="638410">architecture</span> <span m="638740">that's</span> <span m="638860">always</span>
  <span m="639100">used</span> <span m="639240">for</span> <span m="639340">this,</span>
  <span m="639940">there</span> <span m="640180">is</span> <span m="640720">quite</span>
  <span m="640960">a</span> <span m="640990">few</span> <span m="641140">valid</span>
  <span m="641470">options</span> <span m="641890">of</span> <span m="641980">things</span>
  <span m="642260">that</span> <span m="642360">just</span> <span m="643000">get</span>
  <span m="644140">reasonable</span> <span m="644470">performance</span> <span m="644830">and</span>
  <span m="644920">ImageNet,</span> <span m="645610">things</span> <span m="645760">like</span>
  <span m="645880">VGG,</span> <span m="646480">Wide</span> <span m="646780">ResNets</span>
  <span m="647200">and</span> <span m="647290">ResNets.</span> <span m="648210">In</span>
  <span m="648310">my</span> <span m="648460">experience,</span> <span m="648850">they
  all</span> <span m="648970">performed</span> <span m="649270">fairly</span> <span
  m="649600">similarly.</span> <span m="650890">So</span> <span m="651070">it's</span>
  <span m="651160">kind</span> <span m="651310">of</span> <span m="651400">a</span>
  <span m="651670">speed/benefit</span> <span m="652690">trade-off.</span></p><p><span
  m="653980">And</span> <span m="654370">there's</span> <span m="654570">an</span>
  <span m="654630">advantage</span> <span m="654950">to</span> <span m="654990">using</span>
  <span m="655210">fully</span> <span m="655420">convolutional</span> <span m="655930">architectures</span>
  <span m="656890">because</span> <span m="657160">if</span> <span m="657250">you</span>
  <span m="657340">have</span> <span m="657610">fully</span> <span m="657880">connected</span>
  <span m="658210">layers</span> <span m="658450">that</span> <span m="658570">are</span>
  <span m="658680">assumed</span> <span m="658810">specific</span> <span m="659080">dimensionality,</span>
  <span m="660550">you</span> <span m="660640">can</span> <span m="660760">convert</span>
  <span m="661030">them</span> <span m="661180">to</span> <span m="661840">convolutional</span>
  <span m="662290">layers.</span> <span m="662930">They're</span> <span m="663100">just</span>
  <span m="663340">more</span> <span m="663580">convenient</span> <span m="664000">to</span>
  <span m="664090">start</span> <span m="664330">with</span> <span m="664440">a</span>
  <span m="664480">full</span> <span m="664570">convolutional</span> <span m="665140">architecture.</span>
  <span m="666010">There's</span> <span m="666160">going</span> <span m="666270">to</span>
  <span m="666370">be</span> <span m="666760">resolution</span> <span m="667240">invariant.</span></p><p><span
  m="668290">Yes.</span></p><p><span m="668875">AUDIENCE:</span> <span m="669002">In</span>
  <span m="669130">the</span> <span m="669250">last</span> <span m="669440">slide</span>
  <span m="669560">when</span> <span m="669930">you do</span> <span m="670300">patches--</span></p><p><span
  m="671120">ADAM YALA:</span> <span m="671310">Yes.</span></p><p><span m="671500">AUDIENCE:</span>
  <span m="671622">How</span> <span m="671744">do</span> <span m="671866">you</span>
  <span m="671990">label</span> <span m="672480">every</span> <span m="672970">single</span>
  <span m="673460">patch?</span> <span m="673890">Are</span> <span m="674312">they
  just</span> <span m="674734">labeled</span> <span m="675156">with a</span> <span
  m="675580">global</span> <span m="675860">label?</span> <span m="676317">Or do</span>
  <span m="676774">you have to</span> <span m="677231">actually</span> <span m="677688">look
  and</span> <span m="678145">catch,</span> <span m="678602">and figure out</span>
  <span m="679059">what's happened?</span></p><p><span m="679980">ADAM YALA:</span>
  <span m="680090">So</span> <span m="680200">normally</span> <span m="680590">what</span>
  <span m="680680">you</span> <span m="680800">do</span> <span m="681010">is</span>
  <span m="681790">you</span> <span m="681940">have</span> <span m="682090">positive</span>
  <span m="682570">patches</span> <span m="682930">labeled.</span> <span m="683860">And</span>
  <span m="683950">then</span> <span m="684100">you</span> <span m="684190">randomly</span>
  <span m="684640">sample</span> <span m="685000">other</span> <span m="685180">patches.</span>
  <span m="685900">So</span> <span m="686350">from</span> <span m="686590">your</span>
  <span m="686680">annotation--</span> <span m="687220">so,</span> <span m="687370">for</span>
  <span m="687460">example,</span> <span m="687780">a</span> <span m="687810">lot</span>
  <span m="687910">people</span> <span m="688120">do</span> <span m="688240">this</span>
  <span m="688390">on</span> <span m="688930">public</span> <span m="689230">data</span>
  <span m="689440">sets</span> <span m="689680">like</span> <span m="689830">the</span>
  <span m="689920">Florida</span> <span m="690160">DSM</span> <span m="690670">dataset</span>
  <span m="691360">that</span> <span m="691480">has</span> <span m="691630">some</span>
  <span m="691780">entries,</span> <span m="692170">of like,</span> <span m="692320">here</span>
  <span m="692530">are</span> <span m="692650">benign</span> <span m="692800">masses,</span>
  <span m="693580">benign</span> <span m="693760">calcs,</span> <span m="693880">malignant</span>
  <span m="694650">calcs,</span> <span m="695290">et</span> <span m="695430">cetera.</span></p><p><span
  m="695920">What</span> <span m="696010">people</span> <span m="696280">do</span>
  <span m="696460">then</span> <span m="696730">is</span> <span m="696940">take</span>
  <span m="697150">those</span> <span m="697390">annotations.</span> <span m="698440">They</span>
  <span m="698560">will</span> <span m="698680">randomly</span> <span m="699550">select</span>
  <span m="699910">other</span> <span m="700150">patches</span> <span m="700510">and</span>
  <span m="700630">say,</span> <span m="701280">if</span> <span m="701380">it's</span>
  <span m="701470">not</span> <span m="701650">there,</span> <span m="701830">it's</span>
  <span m="701950">negative.</span> <span m="702750">And</span> <span m="702850">I'm</span>
  <span m="702910">going</span> <span m="702980">to</span> <span m="703090">call</span>
  <span m="703300">it</span> <span m="703360">healthy.</span></p><p><span m="704530">And</span>
  <span m="704650">then</span> <span m="704770">they'll</span> <span m="704920">say</span>
  <span m="705130">if</span> <span m="705340">this</span> <span m="705610">bonding</span>
  <span m="705970">box</span> <span m="706240">overlaps</span> <span m="706570">with</span>
  <span m="706690">patch</span> <span m="706990">by</span> <span m="707140">some</span>
  <span m="707350">marginal</span> <span m="707710">call,</span> <span m="707950">it's</span>
  <span m="708130">the</span> <span m="708220">same</span> <span m="708430">label.</span>
  <span m="709210">So</span> <span m="709330">do</span> <span m="709450">this</span>
  <span m="709670">heuristically.</span> <span m="710980">And</span> <span m="711100">other</span>
  <span m="711350">data</span> <span m="711530">sets</span> <span m="711700">that</span>
  <span m="711820">are</span> <span m="711850">proprietary</span> <span m="712480">also</span>
  <span m="712750">kind</span> <span m="712960">of</span> <span m="713020">play</span>
  <span m="713230">with</span> <span m="713320">a</span> <span m="713380">similar</span>
  <span m="713620">trick.</span> <span m="714610">In</span> <span m="714760">general,</span>
  <span m="715190">they</span> <span m="715290">don't</span> <span m="715390">actually</span>
  <span m="715690">label</span> <span m="715990">every</span> <span m="716170">single</span>
  <span m="717730">pixel</span> <span m="718030">accordingly.</span> <span m="718450">But</span>
  <span m="718560">there's</span> <span m="719500">relatively</span> <span m="719950">minor</span>
  <span m="720190">differences</span> <span m="720640">in</span> <span m="720730">how</span>
  <span m="720850">people</span> <span m="721090">do</span> <span m="721210">this.</span>
  <span m="721840">But</span> <span m="722020">the</span> <span m="722080">results</span>
  <span m="722380">are</span> <span m="722440">fairly</span> <span m="722770">similar,</span>
  <span m="723100">regardless.</span></p><p><span m="724110">Yes.</span></p><p><span
  m="724866">AUDIENCE:</span> <span m="724963">When</span> <span m="725060">you</span>
  <span m="725157">go</span> <span m="725254">from</span> <span m="725352">the</span>
  <span m="725838">patch</span> <span m="726324">level</span> <span m="726810">to
  the</span> <span m="727296">full image,</span> <span m="728268">if I understand</span>
  <span m="728754">correctly,</span> <span m="729240">the</span> <span m="729726">architecture</span>
  <span m="730220">hasn't quite</span> <span m="730360">changed</span> <span m="730800">because
  it's</span> <span m="731376">just</span> <span m="731802">convolution</span> <span
  m="732228">is</span> <span m="732654">over</span> <span m="733080">a larger--</span></p><p><span
  m="733510">ADAM YALA:</span> <span m="733667">Exactly.</span> <span m="734140">So</span>
  <span m="734320">the</span> <span m="734470">end</span> <span m="735010">thing</span>
  <span m="735310">right</span> <span m="735490">before</span> <span m="735700">we</span>
  <span m="735760">do</span> <span m="735850">the</span> <span m="735940">prediction</span>
  <span m="736750">is</span> <span m="736900">normally--</span> <span m="738010">ResNet,</span>
  <span m="738340">for</span> <span m="738430">example,</span> <span m="738760">does</span>
  <span m="738910">a</span> <span m="738970">global</span> <span m="739240">average</span>
  <span m="739510">pool.</span> <span m="740620">Channel</span> <span m="741040">lies</span>
  <span m="741280">across</span> <span m="741670">the</span> <span m="741760">entire</span>
  <span m="742060">feature</span> <span m="742300">map.</span> <span m="743260">And</span>
  <span m="743410">so</span> <span m="743680">they</span> <span m="743800">just--</span>
  <span m="744660">for</span> <span m="744810">the</span> <span m="745010">patch</span>
  <span m="745360">level they</span> <span m="745450">take</span> <span m="745630">in</span>
  <span m="745720">an</span> <span m="745840">image</span> <span m="746080">that's</span>
  <span m="746200">250</span> <span m="746590">by</span> <span m="746680">250,</span>
  <span m="747580">do</span> <span m="747700">the</span> <span m="747790">global</span>
  <span m="748030">average</span> <span m="748250">pool</span> <span m="748400">across</span>
  <span m="748690">that</span> <span m="748840">to</span> <span m="748960">make</span>
  <span m="749080">the</span> <span m="749170">prediction.</span> <span m="750160">And</span>
  <span m="750400">when</span> <span m="750580">they</span> <span m="750670">just</span>
  <span m="750850">go</span> <span m="751090">up</span> <span m="751210">to</span>
  <span m="751300">the</span> <span m="751390">full</span> <span m="751570">resolution</span>
  <span m="751930">image,</span> <span m="752220">now</span> <span m="752310">you're</span>
  <span m="752420">taking a</span> <span m="752580">global</span> <span m="752770">average</span>
  <span m="752980">pool</span> <span m="753280">over</span> <span m="754250">a</span>
  <span m="754420">3,000</span> <span m="754900">by</span> <span m="754960">2,000.</span></p><p><span
  m="756110">AUDIENCE:</span> <span m="756235">And</span> <span m="757240">presumably</span>
  <span m="758000">there</span> <span m="758230">might be some</span> <span m="758720">scaling</span>
  <span m="759310">issue</span> <span m="759670">that</span> <span m="760950">you</span>
  <span m="761170">might</span> <span m="761533">need</span> <span m="761896">to</span>
  <span m="762260">adjust.</span> <span m="763610">Do</span> <span m="763780">you
  do</span> <span m="763960">any</span> <span m="764260">of</span> <span m="764732">that?</span>
  <span m="765204">Or are</span> <span m="765676">you just--</span></p><p><span m="766150">ADAM
  YALA:</span> <span m="766330">So</span> <span m="766510">you</span> <span m="766690">feed</span>
  <span m="766945">it</span> <span m="767200">in</span> <span m="767470">at</span>
  <span m="767650">the</span> <span m="767710">full</span> <span m="767890">resolution</span>
  <span m="768280">the</span> <span m="768370">entire</span> <span m="768670">time.</span>
  <span m="769520">So</span> <span m="769620">you</span> <span m="769720">just--</span>
  <span m="770950">do you</span> <span m="771130">see</span> <span m="771220">what</span>
  <span m="771310">I</span> <span m="771370">mean?</span> <span m="771680">So</span>
  <span m="772510">you're</span> <span m="772660">taking</span> <span m="772930">a</span>
  <span m="772990">crop.</span> <span m="773710">So</span> <span m="773860">the</span>
  <span m="773920">resolution</span> <span m="774310">isn't</span> <span m="774460">changing.</span>
  <span m="775280">So</span> <span m="775300">the</span> <span m="775390">same</span>
  <span m="775600">filter</span> <span m="775970">map</span> <span m="776020">should</span>
  <span m="776200">be</span> <span m="776290">able</span> <span m="776500">to</span>
  <span m="776590">kind</span> <span m="776740">of</span> <span m="776830">scale</span>
  <span m="777130">accordingly.</span></p><p><span m="778340">But</span> <span m="778600">if</span>
  <span m="778720">you</span> <span m="778840">do</span> <span m="779020">things</span>
  <span m="779260">like</span> <span m="779410">average</span> <span m="779710">pooling,</span>
  <span m="780460">then</span> <span m="780640">you're</span> <span m="780720">kind</span>
  <span m="780880">of--</span> <span m="781660">any</span> <span m="781930">one</span>
  <span m="782320">thing that</span> <span m="782500">has</span> <span m="782620">a</span>
  <span m="782690">very</span> <span m="782800">high</span> <span m="782920">activation</span>
  <span m="783430">will</span> <span m="783550">get</span> <span m="783760">averaged</span>
  <span m="784060">down</span> <span m="784270">lower.</span> <span m="785320">And</span>
  <span m="785500">so,</span> <span m="785650">for</span> <span m="785710">example,</span>
  <span m="785970">in our work,</span> <span m="786040">we use</span> <span m="786490">max</span>
  <span m="786790">pooling</span> <span m="787120">to</span> <span m="787210">kind</span>
  <span m="787360">of</span> <span m="787420">get</span> <span m="787540">around</span>
  <span m="787780">that.</span> <span m="789240">Any</span> <span m="789490">other</span>
  <span m="789580">questions?</span></p><p><span m="790840">But</span> <span m="791140">if</span>
  <span m="791280">this looks</span> <span m="791380">complicated,</span> <span m="792130">have</span>
  <span m="792340">no</span> <span m="792430">worries</span> <span m="792670">because</span>
  <span m="793450">we</span> <span m="793600">actually</span> <span m="793780">think</span>
  <span m="793930">it's</span> <span m="794050">totally</span> <span m="794440">unnecessary.</span>
  <span m="794890">And</span> <span m="794980">this is</span> <span m="795080">the</span>
  <span m="795170">next</span> <span m="795400">slide.</span> <span m="795670">So</span>
  <span m="797380">good</span> <span m="797500">for</span> <span m="797620">you.</span></p><p><span
  m="798920">So</span> <span m="800140">as</span> <span m="800260">I</span> <span
  m="800290">said</span> <span m="800410">before,</span> <span m="800680">this</span>
  <span m="800800">kind</span> <span m="800950">of,</span> <span m="801070">what</span>
  <span m="801280">are</span> <span m="801370">the</span> <span m="801460">problems</span>
  <span m="801740">that</span> <span m="801850">signal</span> <span m="802120">to</span>
  <span m="802210">noise?</span> <span m="802810">So</span> <span m="802990">one</span>
  <span m="803290">obvious</span> <span m="803710">thing</span> <span m="803890">to</span>
  <span m="803980">kind</span> <span m="804130">of</span> <span m="804190">think</span>
  <span m="804340">about</span> <span m="804490">is,</span> <span m="804550">like,</span>
  <span m="804660">OK.</span> <span m="805630">Maybe</span> <span m="805900">doing</span>
  <span m="806140">SGD</span> <span m="806500">with</span> <span m="806600">a</span>
  <span m="806650">batch</span> <span m="806840">size</span> <span m="806980">of</span>
  <span m="807040">three</span> <span m="807640">when</span> <span m="807880">the</span>
  <span m="808060">lesion</span> <span m="808290">is</span> <span m="808420">less</span>
  <span m="808510">than</span> <span m="808600">1%</span> <span m="808870">of</span>
  <span m="808930">the</span> <span m="808990">image</span> <span m="809230">is a</span>
  <span m="809380">bad</span> <span m="809560">idea.</span></p><p><span m="810850">If</span>
  <span m="811090">I</span> <span m="811210">just</span> <span m="811360">take</span>
  <span m="811660">less</span> <span m="811900">noisy</span> <span m="812200">gradients</span>
  <span m="812590">by</span> <span m="812740">increasing</span> <span m="813160">my</span>
  <span m="813250">batch</span> <span m="813430">size,</span> <span m="814240">which</span>
  <span m="814510">means</span> <span m="814810">use</span> <span m="814990">more</span>
  <span m="815140">GPUs,</span> <span m="815650">take</span> <span m="815860">more</span>
  <span m="815980">steps</span> <span m="816270">before</span> <span m="816430">doing</span>
  <span m="817810">the</span> <span m="818170">weight</span> <span m="818470">update,</span>
  <span m="819680">we</span> <span m="819760">actually</span> <span m="820060">find</span>
  <span m="820900">that</span> <span m="821260">the</span> <span m="821380">need</span>
  <span m="821650">to</span> <span m="821770">do</span> <span m="821920">this</span>
  <span m="822100">actually</span> <span m="822340">goes</span> <span m="822520">away</span>
  <span m="822700">completely.</span> <span m="823580">So</span> <span m="823600">these</span>
  <span m="823780">are</span> <span m="823840">experiments</span> <span m="824230">I</span>
  <span m="824290">did</span> <span m="824400">in</span> <span m="824470">the</span>
  <span m="824560">publicly</span> <span m="824980">available</span> <span m="825310">data</span>
  <span m="825450">set</span> <span m="826480">a</span> <span m="826570">while</span>
  <span m="826810">back</span> <span m="827110">while</span> <span m="827260">we were</span>
  <span m="827350">figuring</span> <span m="827650">this</span> <span m="827770">out.</span></p><p><span
  m="828700">If</span> <span m="828880">you</span> <span m="828970">take</span> <span
  m="829270">this</span> <span m="829360">kind</span> <span m="829540">of</span> <span
  m="829600">[INAUDIBLE]</span> <span m="830050">architecture</span> <span m="830650">and</span>
  <span m="831100">fine</span> <span m="831430">tune</span> <span m="831760">with</span>
  <span m="831820">a</span> <span m="831880">batch</span> <span m="832160">size</span>
  <span m="832390">of</span> <span m="833050">2,</span> <span m="833440">4,</span>
  <span m="833740">10,</span> <span m="834205">16,</span> <span m="834670">and</span>
  <span m="834790">compare that to</span> <span m="834940">just</span> <span m="835630">a</span>
  <span m="835840">one-stage</span> <span m="836410">training</span> <span m="836680">where</span>
  <span m="836950">you</span> <span m="837190">just</span> <span m="837490">do</span>
  <span m="837670">the</span> <span m="837910">[INAUDIBLE]</span> <span m="838390">beginning</span>
  <span m="838830">and</span> <span m="838880">initialized</span> <span m="838950">in</span>
  <span m="839230">ImageNet</span> <span m="839790">and</span> <span m="840040">as</span>
  <span m="840150">you</span> <span m="840210">use</span> <span m="840400">different</span>
  <span m="840640">batch</span> <span m="840790">sizes,</span> <span m="841630">you</span>
  <span m="841900">quickly</span> <span m="842350">start</span> <span m="842530">to</span>
  <span m="842620">close</span> <span m="842980">the</span> <span m="843040">gap</span>
  <span m="843460">on</span> <span m="843580">the</span> <span m="843640">development</span>
  <span m="844090">AUC.</span></p><p><span m="845240">And</span> <span m="845290">so</span>
  <span m="845500">for</span> <span m="845620">all</span> <span m="845890">the</span>
  <span m="846010">experiments</span> <span m="846940">that</span> <span m="847090">we</span>
  <span m="847210">do</span> <span m="847450">broadly</span> <span m="847930">we</span>
  <span m="848050">find</span> <span m="848260">that</span> <span m="848350">we</span>
  <span m="848470">actually</span> <span m="848710">get</span> <span m="848890">reasonably</span>
  <span m="849880">stable</span> <span m="850270">training</span> <span m="850520">by
  just</span> <span m="850720">using</span> <span m="850960">a</span> <span m="851020">batch</span>
  <span m="851200">size</span> <span m="851470">of</span> <span m="852340">20</span>
  <span m="852700">and</span> <span m="852790">above.</span> <span m="853900">And</span>
  <span m="854080">this</span> <span m="854200">kind</span> <span m="854350">of</span>
  <span m="854440">comes</span> <span m="854650">down</span> <span m="854830">to</span>
  <span m="855800">if</span> <span m="855910">you use a</span> <span m="856060">batch
  size</span> <span m="856330">of</span> <span m="856390">one,</span> <span m="856540">it's</span>
  <span m="856600">just</span> <span m="856930">particularly</span> <span m="857470">unstable.</span></p><p><span
  m="858210">In</span> <span m="858350">other</span> <span m="858520">details</span>
  <span m="858940">that</span> <span m="859030">we</span> <span m="859120">always</span>
  <span m="859230">sample</span> <span m="859490">the balanced</span> <span m="859840">batches.</span>
  <span m="860290">Cause</span> <span m="860770">otherwise</span> <span m="861010">you'd</span>
  <span m="861100">be</span> <span m="861190">sampling</span> <span m="861460">like,</span>
  <span m="861940">20</span> <span m="862210">batches</span> <span m="862420">before</span>
  <span m="862490">you see a</span> <span m="862780">single</span> <span m="862990">positive</span>
  <span m="863290">sample.</span> <span m="863630">You</span> <span m="863710">just
  don't learn</span> <span m="863830">anything.</span></p><p><span m="865360">Cool.</span>
  <span m="865930">So</span> <span m="866110">that</span> <span m="866260">is</span>
  <span m="866380">like,</span> <span m="866980">if</span> <span m="867070">you</span>
  <span m="867160">do</span> <span m="867280">that,</span> <span m="867490">you</span>
  <span m="867550">don't</span> <span m="867700">do</span> <span m="867790">anything</span>
  <span m="867970">complicated.</span> <span m="868330">You</span> <span m="868390">don't</span>
  <span m="868590">do</span> <span m="868680">any</span> <span m="869290">fancy</span>
  <span m="869680">cropping</span> <span m="870280">or</span> <span m="870340">anything</span>
  <span m="870610">of</span> <span m="870700">that</span> <span m="870820">sort,</span>
  <span m="871210">or</span> <span m="871300">like,</span> <span m="871750">dealing</span>
  <span m="872080">with</span> <span m="872200">like</span> <span m="872450">VGG</span>
  <span m="872700">annotations.</span> <span m="873290">We</span> <span m="873370">found</span>
  <span m="873600">that</span> <span m="873790">the</span> <span m="873910">actual</span>
  <span m="874210">using</span> <span m="874510">VGG</span> <span m="874840">annotation</span>
  <span m="875320">for</span> <span m="875410">this</span> <span m="875500">task</span>
  <span m="875800">is</span> <span m="875890">not</span> <span m="876070">actually</span>
  <span m="876280">helpful.</span></p><p><span m="878620">OK.</span> <span m="879240">No</span>
  <span m="879360">questions?</span> <span m="880140">Yes.</span></p><p><span m="880832">AUDIENCE:</span>
  <span m="881028">So</span> <span m="881224">with</span> <span m="881616">the</span>
  <span m="882010">larger</span> <span m="882170">batch</span> <span m="882370">sizing</span>
  <span m="882925">you</span> <span m="883320">don't</span> <span m="883950">use</span>
  <span m="884230">the</span> <span m="884510">magnified</span> <span m="884890">patches?</span></p><p><span
  m="885650">ADAM YALA:</span> <span m="885715">We</span> <span m="885780">don't.</span>
  <span m="886070">We</span> <span m="886170">just</span> <span m="886290">take</span>
  <span m="886410">the</span> <span m="886500">whole</span> <span m="886680">image</span>
  <span m="886920">from</span> <span m="887040">beginning.</span> <span m="887780">Pretend</span>
  <span m="888070">you--</span> <span m="888340">like,</span> <span m="888580">can
  you</span> <span m="888710">just</span> <span m="888890">see</span> <span m="889010">the</span>
  <span m="889110">annotation</span> <span m="889620">as</span> <span m="890040">whole</span>
  <span m="890250">image,</span> <span m="891200">cancer</span> <span m="891630">with</span>
  <span m="891750">less</span> <span m="891930">than</span> <span m="892170">within</span>
  <span m="892590">a</span> <span m="892650">year.</span> <span m="894330">It's</span>
  <span m="894450">a</span> <span m="894480">much</span> <span m="894660">simpler</span>
  <span m="894960">setup.</span></p><p><span m="896145">AUDIENCE:</span> <span m="896152">I</span>
  <span m="896160">don't</span> <span m="896260">get.</span> <span m="896360">That's</span>
  <span m="896735">the same</span> <span m="897110">thing I</span> <span m="897190">thought
  you said</span> <span m="897505">you couldn't</span> <span m="897820">do for</span>
  <span m="897900">memory</span> <span m="898280">reasons.</span></p><p><span m="898980">ADAM
  YALA:</span> <span m="899085">Oh.</span> <span m="899400">So</span> <span m="899580">you</span>
  <span m="899700">just--</span> <span m="900570">instead</span> <span m="900930">of--</span>
  <span m="901260">so</span> <span m="901590">normally</span> <span m="901950">when</span>
  <span m="902070">you</span> <span m="902130">do,</span> <span m="902900">you're</span>
  <span m="903000">going</span> <span m="903140">to</span> <span m="903240">train</span>
  <span m="903450">the</span> <span m="903540">network,</span> <span m="905230">the</span>
  <span m="905340">most</span> <span m="905520">common</span> <span m="905730">approach</span>
  <span m="905990">is</span> <span m="906050">you</span> <span m="906150">do</span>
  <span m="906330">back prop</span> <span m="906600">and then</span> <span m="906720">step.</span>
  <span m="906990">Cause</span> <span m="907330">you</span> <span m="907500">do</span>
  <span m="907650">back</span> <span m="907820">prop</span> <span m="908030">several</span>
  <span m="908250">times,</span> <span m="908520">you're</span> <span m="908640">accumulating</span>
  <span m="909080">the</span> <span m="909180">gradients,</span> <span m="909630">at
  least in</span> <span m="909720">PyTorch.</span> <span m="910820">And</span> <span
  m="910970">then</span> <span m="911070">you</span> <span m="911160">can do</span>
  <span m="911250">step</span> <span m="911520">afterwards.</span> <span m="912610">So</span>
  <span m="913050">instead</span> <span m="913380">of</span> <span m="913470">doing</span>
  <span m="913920">the</span> <span m="914040">whole</span> <span m="914250">batch</span>
  <span m="914490">at</span> <span m="914560">one</span> <span m="914700">time,</span>
  <span m="915060">you</span> <span m="915130">just</span> <span m="915230">do</span>
  <span m="915390">it</span> <span m="915510">serially.</span> <span m="916290">So</span>
  <span m="916410">there</span> <span m="916560">you're</span> <span m="916650">just</span>
  <span m="916800">trading</span> <span m="917160">time</span> <span m="918750">for</span>
  <span m="918900">space.</span></p><p><span m="919950">The</span> <span m="920070">minimum,</span>
  <span m="920460">though,</span> <span m="920650">is</span> <span m="920740">you
  have</span> <span m="920850">to fit</span> <span m="921120">at</span> <span m="921210">least</span>
  <span m="921630">a</span> <span m="921690">single</span> <span m="922530">image</span>
  <span m="922830">per</span> <span m="923140">GPU.</span> <span m="924150">And</span>
  <span m="924270">in</span> <span m="924390">our</span> <span m="924540">case</span>
  <span m="924840">we</span> <span m="924930">can</span> <span m="925050">fit</span>
  <span m="925680">three.</span> <span m="926820">But</span> <span m="926970">to</span>
  <span m="927060">make</span> <span m="927180">this</span> <span m="927330">actually</span>
  <span m="927540">scale,</span> <span m="927780">we</span> <span m="927840">use</span>
  <span m="928090">four</span> <span m="928290">GPUs</span> <span m="928440">at</span>
  <span m="928530">a</span> <span m="928590">time.</span></p><p><span m="931760">Yes.</span></p><p><span
  m="932000">AUDIENCE:</span> <span m="932150">How</span> <span m="932300">much</span>
  <span m="932450">is the</span> <span m="932900">trade-off</span> <span m="933350">with
  time?</span></p><p><span m="935150">ADAM YALA:</span> <span m="935285">So</span>
  <span m="935420">if</span> <span m="935580">I'm</span> <span m="935690">gonna take</span>
  <span m="935850">one batch</span> <span m="935960">size</span> <span m="936230">any</span>
  <span m="936380">bigger,</span> <span m="937590">I</span> <span m="937730">would</span>
  <span m="937930">only</span> <span m="938000">do</span> <span m="938120">it</span>
  <span m="938240">in</span> <span m="938360">increments</span> <span m="938720">of</span>
  <span m="939140">let's</span> <span m="939290">say</span> <span m="939460">12,</span>
  <span m="940130">because</span> <span m="940400">that's</span> <span m="940520">how</span>
  <span m="940640">much</span> <span m="940790">I</span> <span m="940850">can</span>
  <span m="940970">fit</span> <span m="941150">within</span> <span m="941350">my</span>
  <span m="942050">set</span> <span m="942350">of</span> <span m="942430">GPUs</span>
  <span m="942740">at</span> <span m="942830">the</span> <span m="942890">same</span>
  <span m="943100">time.</span> <span m="944390">But</span> <span m="944600">to</span>
  <span m="944660">control</span> <span m="945050">the</span> <span m="945110">size</span>
  <span m="945350">of</span> <span m="945410">the</span> <span m="945470">experiment</span>
  <span m="945920">you</span> <span m="945980">want</span> <span m="946100">to</span>
  <span m="946160">have</span> <span m="946250">the</span> <span m="946340">kind</span>
  <span m="946490">of</span> <span m="946550">the</span> <span m="946640">same</span>
  <span m="946850">number</span> <span m="947090">of</span> <span m="947180">gradient</span>
  <span m="947480">updates</span> <span m="947930">per</span> <span m="948170">experiment.</span>
  <span m="949160">So</span> <span m="949320">if I</span> <span m="949420">want</span>
  <span m="949590">to</span> <span m="949650">use</span> <span m="949820">a batch
  size of</span> <span m="950130">48,</span> <span m="950640">so all</span> <span
  m="950770">my</span> <span m="950960">experiments,</span> <span m="951440">instead</span>
  <span m="951620">of</span> <span m="951710">taking</span> <span m="952560">about</span>
  <span m="952790">half</span> <span m="953000">a</span> <span m="953030">day,</span>
  <span m="953190">it</span> <span m="953240">takes</span> <span m="953480">about</span>
  <span m="953630">a</span> <span m="953690">day.</span></p><p><span m="955200">And</span>
  <span m="955340">so</span> <span m="955490">there's</span> <span m="955640">kind</span>
  <span m="955850">of,</span> <span m="955940">like,</span> <span m="956030">this</span>
  <span m="956180">natural</span> <span m="956780">trade-off</span> <span m="957790">as</span>
  <span m="957920">you</span> <span m="957980">go</span> <span m="958190">along.</span>
  <span m="958620">So</span> <span m="958670">one</span> <span m="958820">of</span>
  <span m="958880">the</span> <span m="958940">things</span> <span m="959390">I</span>
  <span m="959480">mentioned</span> <span m="959780">at the</span> <span m="959870">very</span>
  <span m="960080">end</span> <span m="960260">is</span> <span m="960350">we're</span>
  <span m="960470">considering</span> <span m="960800">some</span> <span m="961640">adversarial</span>
  <span m="962240">approach</span> <span m="962610">for</span> <span m="962720">something.</span>
  <span m="963500">And</span> <span m="963620">one</span> <span m="963710">of</span>
  <span m="963770">the</span> <span m="963830">annoying</span> <span m="964040">things</span>
  <span m="964220">about</span> <span m="964400">that</span> <span m="964580">is</span>
  <span m="964700">that</span> <span m="964910">if</span> <span m="965030">I</span>
  <span m="965120">have</span> <span m="965270">five</span> <span m="965610">discriminator</span>
  <span m="965880">steps,</span> <span m="966590">oh</span> <span m="966760">my</span>
  <span m="966860">god.</span> <span m="967070">My</span> <span m="967220">my experiment--</span>
  <span m="967470">I'll take</span> <span m="967610">three</span> <span m="967820">days</span>
  <span m="968000">per</span> <span m="968090">experiment.</span></p><p><span m="968930">And</span>
  <span m="969230">[INAUDIBLE]</span> <span m="969710">update of</span> <span m="970100">someone</span>
  <span m="970320">that's</span> <span m="970380">trying</span> <span m="970510">to</span>
  <span m="970630">design</span> <span m="970880">a</span> <span m="970940">better</span>
  <span m="971120">model</span> <span m="971390">becomes</span> <span m="971600">really</span>
  <span m="971930">slow</span> <span m="972890">when</span> <span m="973100">the</span>
  <span m="973160">experiments</span> <span m="973250">start</span> <span m="973470">taking</span>
  <span m="973730">this</span> <span m="973820">long.</span></p><p><span m="976220">Yes.</span></p><p><span
  m="977030">AUDIENCE:</span> <span m="977120">So</span> <span m="977210">you</span>
  <span m="977300">said</span> <span m="978680">the</span> <span m="978830">annotations</span>
  <span m="979370">did</span> <span m="979520">not</span> <span m="980430">help</span>
  <span m="980720">with</span> <span m="980870">the</span> <span m="980960">training.</span>
  <span m="981215">Is</span> <span m="981470">that</span> <span m="981860">because</span>
  <span m="984320">the</span> <span m="984470">actual</span> <span m="984770">cancer</span>
  <span m="985250">itself</span> <span m="985440">is not</span> <span m="985580">really</span>
  <span m="985850">different</span> <span m="986000">from the</span> <span m="986444">dense</span>
  <span m="986888">tissue,</span> <span m="988220">and</span> <span m="988690">the</span>
  <span m="989060">location</span> <span m="989600">of</span> <span m="989740">that</span>
  <span m="989960">matters,</span> <span m="990260">and</span> <span m="990742">not</span>
  <span m="991224">the</span> <span m="991706">actual</span> <span m="992188">granularity</span>
  <span m="992670">of the--</span> <span m="994120">what</span> <span m="994140">is
  the</span> <span m="994260">reason?</span></p><p><span m="995400">ADAM YALA:</span>
  <span m="995527">So</span> <span m="996120">in</span> <span m="996300">general</span>
  <span m="996650">when</span> <span m="996750">something</span> <span m="997050">doesn't</span>
  <span m="997220">help,</span> <span m="997550">there's</span> <span m="997830">always</span>
  <span m="998160">kind</span> <span m="998310">of</span> <span m="998370">like</span>
  <span m="998460">a</span> <span m="998520">possibility</span> <span m="999090">of</span>
  <span m="999150">two</span> <span m="999330">things.</span> <span m="1000510">One</span>
  <span m="1000680">thing</span> <span m="1000920">is</span> <span m="1001040">that</span>
  <span m="1001220">the</span> <span m="1001430">whole</span> <span m="1001700">image</span>
  <span m="1001940">signal</span> <span m="1002240">kind</span> <span m="1002390">of</span>
  <span m="1002480">subsumes</span> <span m="1003110">that</span> <span m="1003230">smaller</span>
  <span m="1003770">scale</span> <span m="1004100">signal.</span> <span m="1004890">Or</span>
  <span m="1005270">there</span> <span m="1005370">is</span> <span m="1005510">a</span>
  <span m="1005570">better</span> <span m="1005780">way</span> <span m="1005900">to</span>
  <span m="1005990">do</span> <span m="1006140">it</span> <span m="1006230">I</span>
  <span m="1006260">haven't</span> <span m="1006440">found</span> <span m="1006710">that</span>
  <span m="1006830">would</span> <span m="1006950">help.</span></p><p><span m="1008230">And</span>
  <span m="1008300">then</span> <span m="1008480">this</span> <span m="1008660">thing</span>
  <span m="1008900">looks</span> <span m="1009050">to</span> <span m="1009170">us</span>
  <span m="1009260">all</span> <span m="1009530">very</span> <span m="1009710">hard.</span>
  <span m="1011300">As</span> <span m="1011510">of</span> <span m="1011660">now,</span>
  <span m="1012320">so</span> <span m="1013460">the</span> <span m="1013550">task</span>
  <span m="1013880">we're</span> <span m="1014090">[INAUDIBLE]</span> <span m="1014330">on</span>
  <span m="1014930">is</span> <span m="1015170">whole</span> <span m="1015440">image</span>
  <span m="1015650">classification.</span> <span m="1016880">And</span> <span m="1017030">so</span>
  <span m="1017150">on</span> <span m="1017270">that</span> <span m="1017420">task</span>
  <span m="1017630">it's</span> <span m="1017720">possible</span> <span m="1018140">that</span>
  <span m="1018440">the</span> <span m="1019190">kind</span> <span m="1019370">of</span>
  <span m="1019430">surrounding</span> <span m="1019910">context--</span> <span m="1020180">so</span>
  <span m="1020450">when</span> <span m="1020570">you</span> <span m="1020630">do</span>
  <span m="1020840">a</span> <span m="1020900">patch with an</span> <span m="1021290">annotation,</span>
  <span m="1022270">you</span> <span m="1022460">kind</span> <span m="1022640">of</span>
  <span m="1022730">lose</span> <span m="1022980">the</span> <span m="1023050">context</span>
  <span m="1023390">which it</span> <span m="1023540">appears</span> <span m="1023870">in.</span>
  <span m="1024470">So</span> <span m="1024589">it's</span> <span m="1024680">possible</span>
  <span m="1025099">that</span> <span m="1025220">just</span> <span m="1025369">by</span>
  <span m="1025520">looking</span> <span m="1025849">at</span> <span m="1025940">the</span>
  <span m="1026000">whole</span> <span m="1026180">context</span> <span m="1026540">every</span>
  <span m="1026690">time,</span> <span m="1027890">it's</span> <span m="1028220">as</span>
  <span m="1028460">good--</span> <span m="1029660">you</span> <span m="1029750">don't</span>
  <span m="1029869">get</span> <span m="1029990">any</span> <span m="1030170">benefit</span>
  <span m="1030530">from</span> <span m="1030710">kind</span> <span m="1030890">of</span>
  <span m="1030980">the</span> <span m="1031700">zooming</span> <span m="1031970">boxes.</span>
  <span m="1032750">However,</span> <span m="1032920">we're</span> <span m="1033020">not</span>
  <span m="1033170">evaluating</span> <span m="1033859">on</span> <span m="1034430">kind</span>
  <span m="1034609">of</span> <span m="1034670">an</span> <span m="1035300">object</span>
  <span m="1035569">detection</span> <span m="1036079">type of</span> <span m="1036260">evaluation</span>
  <span m="1036680">metric.</span> <span m="1036930">If you say</span> <span m="1037190">how</span>
  <span m="1037339">well</span> <span m="1037490">we</span> <span m="1037730">are</span>
  <span m="1037849">catching</span> <span m="1038270">the</span> <span m="1038359">box.</span>
  <span m="1039240">And</span> <span m="1039260">if</span> <span m="1039410">we</span>
  <span m="1039560">were,</span> <span m="1039800">we'd</span> <span m="1039950">probably</span>
  <span m="1040250">have</span> <span m="1040400">much</span> <span m="1040609">better</span>
  <span m="1040819">luck</span> <span m="1041900">with</span> <span m="1042230">using</span>
  <span m="1042560">the VGG</span> <span m="1042730">annotation.</span></p><p><span
  m="1043970">Because</span> <span m="1044329">you</span> <span m="1044450">might</span>
  <span m="1044630">be</span> <span m="1044720">able</span> <span m="1044869">to</span>
  <span m="1045020">tell</span> <span m="1045920">some</span> <span m="1046160">of</span>
  <span m="1046250">those</span> <span m="1046400">discriminations</span> <span m="1046790">by</span>
  <span m="1046910">like,</span> <span m="1047089">this</span> <span m="1047240">looks</span>
  <span m="1047450">like</span> <span m="1047599">a</span> <span m="1047930">breast</span>
  <span m="1048150">that's</span> <span m="1048290">likely</span> <span m="1048560">to</span>
  <span m="1048620">develop</span> <span m="1048890">cancer</span> <span m="1049280">at</span>
  <span m="1049370">all.</span> <span m="1050420">And</span> <span m="1050930">the</span>
  <span m="1051080">ability</span> <span m="1051470">of</span> <span m="1051530">the</span>
  <span m="1051590">model</span> <span m="1051800">to</span> <span m="1051920">do</span>
  <span m="1052040">that</span> <span m="1052220">is</span> <span m="1052310">part</span>
  <span m="1052490">of</span> <span m="1052550">why</span> <span m="1052670">we</span>
  <span m="1052760">can</span> <span m="1052850">do</span> <span m="1052940">risk</span>
  <span m="1053090">modeling.</span> <span m="1053390">Which is</span> <span m="1053920">going</span>
  <span m="1053990">to</span> <span m="1054080">be</span> <span m="1054170">the</span>
  <span m="1054230">kind</span> <span m="1054380">of</span> <span m="1054440">the</span>
  <span m="1054500">last</span> <span m="1054770">bit</span> <span m="1054920">of</span>
  <span m="1054990">the</span> <span m="1055080">talk.</span></p><p><span m="1057730">Yes.</span></p><p><span
  m="1058110">AUDIENCE:</span> <span m="1058215">So</span> <span m="1058320">do</span>
  <span m="1058500">you</span> <span m="1058700">do</span> <span m="1058940">the</span>
  <span m="1059060">object</span> <span m="1059390">detection</span> <span m="1060050">after</span>
  <span m="1060470">you</span> <span m="1061040">identify</span> <span m="1061520">whether</span>
  <span m="1061850">there's</span> <span m="1062240">cancer</span> <span m="1062540">or</span>
  <span m="1062630">not?</span></p><p><span m="1063450">ADAM YALA:</span> <span m="1063490">So</span>
  <span m="1063530">as</span> <span m="1063650">of</span> <span m="1063740">now</span>
  <span m="1063950">we</span> <span m="1064070">don't</span> <span m="1064280">do</span>
  <span m="1064550">object</span> <span m="1064820">detection</span> <span m="1065210">in</span>
  <span m="1065270">part</span> <span m="1065420">because</span> <span m="1065660">we're</span>
  <span m="1065780">framing</span> <span m="1066170">the</span> <span m="1066230">problem</span>
  <span m="1066620">as</span> <span m="1066770">triage.</span> <span m="1067550">So</span>
  <span m="1067910">there</span> <span m="1068120">is</span> <span m="1068300">quite</span>
  <span m="1068570">a</span> <span m="1068600">few</span> <span m="1069050">tool kits</span>
  <span m="1069410">out</span> <span m="1069500">there</span> <span m="1069620">to</span>
  <span m="1069710">draw</span> <span m="1069880">more</span> <span m="1070010">boxes</span>
  <span m="1070370">on</span> <span m="1070460">the</span> <span m="1070520">mammogram.</span>
  <span m="1071460">But</span> <span m="1071660">the</span> <span m="1071810">insight</span>
  <span m="1072070">is</span> <span m="1072170">that</span> <span m="1072290">if</span>
  <span m="1072890">there's</span> <span m="1073100">1,000</span> <span m="1073460">things</span>
  <span m="1073580">to</span> <span m="1073670">look</span> <span m="1073820">at,</span>
  <span m="1074660">looking</span> <span m="1074990">at</span> <span m="1075110">2,000</span>
  <span m="1075660">things</span> <span m="1075870">you</span> <span m="1076090">drew</span>
  <span m="1076820">more</span> <span m="1077060">boxes</span> <span m="1077390">per</span>
  <span m="1077540">image.</span> <span m="1077680">And</span> <span m="1077940">it</span>
  <span m="1078190">isn't</span> <span m="1078380">necessarily</span> <span m="1078950">the</span>
  <span m="1079310">problem we're</span> <span m="1079640">trying</span> <span m="1079790">to</span>
  <span m="1079850">look</span> <span m="1080000">at.</span> <span m="1080190">There's</span>
  <span m="1080420">quite</span> <span m="1080630">a</span> <span m="1080660">bit</span>
  <span m="1081200">of</span> <span m="1081290">effort</span> <span m="1081500">there.</span>
  <span m="1082680">And it's</span> <span m="1082890">something</span> <span m="1083090">we</span>
  <span m="1083150">might</span> <span m="1083300">look</span> <span m="1083450">into</span>
  <span m="1083900">later</span> <span m="1084140">in</span> <span m="1084230">the</span>
  <span m="1084290">future.</span> <span m="1084660">But</span> <span m="1084760">it's</span>
  <span m="1084860">not</span> <span m="1084890">the</span> <span m="1084950">focus</span>
  <span m="1085280">of</span> <span m="1085340">this</span> <span m="1085490">work.</span></p><p><span
  m="1086860">Yes.</span></p><p><span m="1087400">AUDIENCE:</span> <span m="1087520">So</span>
  <span m="1087640">Connie</span> <span m="1087970">was</span> <span m="1088780">saying</span>
  <span m="1089260">that</span> <span m="1089980">the</span> <span m="1090070">same</span>
  <span m="1090490">pattern</span> <span m="1090970">appearing</span> <span m="1091490">in</span>
  <span m="1091630">different</span> <span m="1092020">parts</span> <span m="1092410">of</span>
  <span m="1092770">the</span> <span m="1093130">breast</span> <span m="1093490">can</span>
  <span m="1093770">mean</span> <span m="1094030">different</span> <span m="1094390">things.</span>
  <span m="1096820">But</span> <span m="1097900">when</span> <span m="1098140">you're</span>
  <span m="1098290">looking</span> <span m="1098740">at</span> <span m="1098890">the</span>
  <span m="1099040">entire</span> <span m="1099580">image</span> <span m="1099950">as</span>
  <span m="1100130">once,</span> <span m="1103175">I</span> <span m="1103640">would</span>
  <span m="1103965">worry</span> <span m="1104730">intuitively</span> <span m="1105695">about</span>
  <span m="1105960">whether</span> <span m="1106700">the</span> <span m="1106980">convolutional</span>
  <span m="1107860">architecture</span> <span m="1109150">is</span> <span m="1109390">going</span>
  <span m="1109660">to</span> <span m="1109810">be</span> <span m="1109990">able</span>
  <span m="1110230">to</span> <span m="1110380">pick</span> <span m="1110650">that</span>
  <span m="1110910">up</span> <span m="1111710">or</span> <span m="1111980">whether--</span>
  <span m="1112990">because</span> <span m="1113380">you</span> <span m="1113470">were</span>
  <span m="1113560">looking</span> <span m="1114340">for</span> <span m="1114610">a</span>
  <span m="1114670">very</span> <span m="1114910">small</span> <span m="1115270">cancer</span>
  <span m="1115840">on</span> <span m="1115950">a</span> <span m="1116020">very</span>
  <span m="1116260">large</span> <span m="1116650">image.</span> <span m="1117590">And</span>
  <span m="1118170">then</span> <span m="1118450">you</span> <span m="1118570">were</span>
  <span m="1118660">looking</span> <span m="1119200">for</span> <span m="1120110">the</span>
  <span m="1120220">significance</span> <span m="1121120">of</span> <span m="1121250">that</span>
  <span m="1121480">very</span> <span m="1121730">small</span> <span m="1122210">cancer</span>
  <span m="1123370">in</span> <span m="1123700">different</span> <span m="1124120">parts</span>
  <span m="1124630">of</span> <span m="1124750">the</span> <span m="1124900">image</span>
  <span m="1125360">or in</span> <span m="1125610">different</span> <span m="1125950">contexts</span>
  <span m="1126315">of</span> <span m="1126680">the</span> <span m="1127090">image.</span>
  <span m="1127910">And</span> <span m="1128050">I'm</span> <span m="1128200">just--</span>
  <span m="1129340">I</span> <span m="1129400">mean,</span> <span m="1129770">it's</span>
  <span m="1130510">a</span> <span m="1130570">pleasant</span> <span m="1130990">surprise</span>
  <span m="1131750">that</span> <span m="1132030">this</span> <span m="1132220">works.</span></p><p><span
  m="1133310">ADAM YALA:</span> <span m="1133365">So</span> <span m="1133420">there</span>
  <span m="1133540">is</span> <span m="1133630">kind</span> <span m="1133810">of</span>
  <span m="1133870">like</span> <span m="1134020">two</span> <span m="1134260">pieces</span>
  <span m="1134620">that</span> <span m="1134770">can</span> <span m="1134920">help</span>
  <span m="1135100">explain</span> <span m="1135400">that.</span> <span m="1136030">So</span>
  <span m="1136180">the</span> <span m="1136270">first</span> <span m="1136540">is</span>
  <span m="1136630">that</span> <span m="1136680">if</span> <span m="1136750">you</span>
  <span m="1136810">look</span> <span m="1137050">at,</span> <span m="1137170">like,</span>
  <span m="1137970">the</span> <span m="1138100">receptive</span> <span m="1138490">fields
  of</span> <span m="1138850">any</span> <span m="1139060">given</span> <span m="1139360">last</span>
  <span m="1139660">receptive</span> <span m="1140050">map</span> <span m="1140320">at</span>
  <span m="1140410">the</span> <span m="1140470">very</span> <span m="1140650">end</span>
  <span m="1140950">of</span> <span m="1141010">the</span> <span m="1141100">network,</span>
  <span m="1142120">each</span> <span m="1142360">of</span> <span m="1142450">those</span>
  <span m="1142630">summarizes</span> <span m="1143410">through</span> <span m="1143650">these</span>
  <span m="1143800">convolutions</span> <span m="1144960">a</span> <span m="1145030">fairly</span>
  <span m="1145390">sizable</span> <span m="1146080">part</span> <span m="1146440">of</span>
  <span m="1146530">the</span> <span m="1146620">image.</span> <span m="1147350">And</span>
  <span m="1147370">so</span> <span m="1147490">you</span> <span m="1147610">are</span>
  <span m="1147820">kind</span> <span m="1148060">of,</span> <span m="1148150">like,</span>
  <span m="1148930">each</span> <span m="1149110">pixel</span> <span m="1149540">at</span>
  <span m="1149590">the</span> <span m="1149650">very</span> <span m="1149830">end</span>
  <span m="1150090">ends</span> <span m="1150230">up</span> <span m="1150300">being</span>
  <span m="1150530">like</span> <span m="1150700">something</span> <span m="1150910">like
  a</span> <span m="1151100">50</span> <span m="1151360">by</span> <span m="1151480">50</span>
  <span m="1151900">image.</span> <span m="1152620">That's</span> <span m="1152800">by</span>
  <span m="1152950">five</span> <span m="1153180">total</span> <span m="1153370">dimensions.</span></p><p><span
  m="1154730">And</span> <span m="1154810">so</span> <span m="1155440">each</span>
  <span m="1155650">part</span> <span m="1156040">does</span> <span m="1156250">summarize</span>
  <span m="1156600">this</span> <span m="1156760">local</span> <span m="1157030">context</span>
  <span m="1157450">decently</span> <span m="1157780">well.</span> <span m="1158370">And</span>
  <span m="1158470">when</span> <span m="1158560">you</span> <span m="1158680">do</span>
  <span m="1158770">maximum</span> <span m="1159210">at the</span> <span m="1159310">very
  end,</span> <span m="1159580">and</span> <span m="1159910">you</span> <span m="1160000">get</span>
  <span m="1160180">some</span> <span m="1161170">not</span> <span m="1161440">perfect</span>
  <span m="1162100">but</span> <span m="1162490">OK</span> <span m="1162910">global</span>
  <span m="1163350">summary,</span> <span m="1163690">what</span> <span m="1163780">is</span>
  <span m="1163840">the</span> <span m="1163900">context</span> <span m="1164320">of</span>
  <span m="1164410">this</span> <span m="1164530">image?</span> <span m="1165440">So</span>
  <span m="1165610">something</span> <span m="1165910">like,</span> <span m="1166090">let's</span>
  <span m="1166240">say,</span> <span m="1167590">some</span> <span m="1167800">of</span>
  <span m="1167860">the</span> <span m="1167950">lower</span> <span m="1168220">dimensions</span>
  <span m="1168850">can</span> <span m="1168970">summarize,</span> <span m="1169330">like,</span>
  <span m="1169480">is</span> <span m="1169600">this</span> <span m="1169750">a</span>
  <span m="1169810">dense</span> <span m="1170080">breast</span> <span m="1170410">or</span>
  <span m="1170500">kind</span> <span m="1170650">of</span> <span m="1170740">some</span>
  <span m="1170890">of</span> <span m="1170950">the</span> <span m="1171340">other</span>
  <span m="1171550">pattern</span> <span m="1171880">information</span> <span m="1172480">that</span>
  <span m="1172600">might</span> <span m="1172780">tell</span> <span m="1172990">you</span>
  <span m="1173500">what</span> <span m="1173590">kind</span> <span m="1173740">of</span>
  <span m="1173800">breast</span> <span m="1173930">this</span> <span m="1174080">is.</span>
  <span m="1174640">Whereas</span> <span m="1174910">any</span> <span m="1175080">one</span>
  <span m="1175220">of</span> <span m="1175280">them</span> <span m="1175420">can</span>
  <span m="1175540">tell</span> <span m="1175720">you</span> <span m="1178210">this</span>
  <span m="1178540">looks</span> <span m="1178780">like</span> <span m="1178900">a</span>
  <span m="1178960">cancer</span> <span m="1179200">given</span> <span m="1179380">its</span>
  <span m="1179470">local</span> <span m="1179680">context.</span></p><p><span m="1180590">So</span>
  <span m="1180730">do</span> <span m="1180840">you</span> <span m="1180910">have</span>
  <span m="1181060">some</span> <span m="1181210">level</span> <span m="1181400">summarization,</span>
  <span m="1182020">both</span> <span m="1182230">because</span> <span m="1182500">of</span>
  <span m="1182590">the</span> <span m="1183160">channel-wise</span> <span m="1183760">maxim</span>
  <span m="1184040">of</span> <span m="1184210">the</span> <span m="1184360">end,</span>
  <span m="1184900">and</span> <span m="1185020">because</span> <span m="1185680">each</span>
  <span m="1185890">point</span> <span m="1186400">through</span> <span m="1186640">the</span>
  <span m="1186970">many,</span> <span m="1187340">many</span> <span m="1187450">convolutions</span>
  <span m="1189030">of</span> <span m="1189160">different</span> <span m="1189460">strides</span>
  <span m="1190270">gives</span> <span m="1190540">you</span> <span m="1190630">some</span>
  <span m="1190750">of</span> <span m="1190810">that</span> <span m="1190930">summary</span>
  <span m="1191170">effect.</span> <span m="1193830">OK,</span> <span m="1194140">great.</span>
  <span m="1194710">I'm</span> <span m="1194810">going</span> <span m="1194850">to</span>
  <span m="1195060">jump</span> <span m="1195300">forward.</span></p><p><span m="1196690">So</span>
  <span m="1197180">we've</span> <span m="1197320">talked</span> <span m="1197550">about</span>
  <span m="1198180">how</span> <span m="1198300">to</span> <span m="1198390">make</span>
  <span m="1198480">this</span> <span m="1198630">learn.</span> <span m="1198900">It's</span>
  <span m="1199020">actually</span> <span m="1199920">not</span> <span m="1200130">that</span>
  <span m="1200250">tricky</span> <span m="1200550">if we</span> <span m="1200990">just
  do</span> <span m="1201150">it</span> <span m="1201210">carefully</span> <span m="1201780">and</span>
  <span m="1201870">tune.</span> <span m="1202680">Now</span> <span m="1203100">I'll</span>
  <span m="1203310">talk</span> <span m="1203460">about</span> <span m="1203580">how</span>
  <span m="1203670">to</span> <span m="1203760">use</span> <span m="1203940">this</span>
  <span m="1204060">model</span> <span m="1204330">to</span> <span m="1204390">actually</span>
  <span m="1204810">deliver</span> <span m="1205200">on</span> <span m="1205290">this</span>
  <span m="1205580">triage</span> <span m="1205890">idea.</span></p><p><span m="1207600">So</span>
  <span m="1208140">some</span> <span m="1208360">of</span> <span m="1208490">my</span>
  <span m="1208560">choices</span> <span m="1208860">again,</span> <span m="1209630">ImageNet</span>
  <span m="1210020">initialization</span> <span m="1210540">is</span> <span m="1210640">going</span>
  <span m="1210680">to</span> <span m="1210750">make</span> <span m="1210870">your</span>
  <span m="1210930">life</span> <span m="1211110">a</span> <span m="1211170">happier</span>
  <span m="1211440">time.</span> <span m="1212540">Use</span> <span m="1212720">bigger</span>
  <span m="1212920">batch</span> <span m="1213120">sizes.</span> <span m="1214080">And</span>
  <span m="1214380">architecture</span> <span m="1214650">choice</span> <span m="1214950">doesn't</span>
  <span m="1215140">really</span> <span m="1215280">matter</span> <span m="1215460">if</span>
  <span m="1215550">it's</span> <span m="1215670">convolutional.</span></p><p><span
  m="1217536">And</span> <span m="1218010">the</span> <span m="1218130">overall</span>
  <span m="1218520">setup</span> <span m="1218820">that</span> <span m="1218910">we</span>
  <span m="1219000">do</span> <span m="1219210">through</span> <span m="1219450">this</span>
  <span m="1219630">work</span> <span m="1220080">and</span> <span m="1220200">across</span>
  <span m="1220500">many</span> <span m="1220710">other</span> <span m="1220860">projects</span>
  <span m="1221610">we're</span> <span m="1221700">training</span> <span m="1222060">independently</span>
  <span m="1222600">per</span> <span m="1222810">image.</span> <span m="1223580">Now</span>
  <span m="1223590">this</span> <span m="1223740">is</span> <span m="1223830">a</span>
  <span m="1223890">harder</span> <span m="1224220">task</span> <span m="1225540">because</span>
  <span m="1225870">you</span> <span m="1225930">don't</span> <span m="1226050">actually</span>
  <span m="1226290">have</span> <span m="1226470">the--</span> <span m="1226870">you're</span>
  <span m="1226970">not</span> <span m="1226980">taking</span> <span m="1227170">any</span>
  <span m="1227230">of the</span> <span m="1227370">other</span> <span m="1227550">view,</span>
  <span m="1227720">you're not</span> <span m="1227860">taking</span> <span m="1228120">prior</span>
  <span m="1228330">mammograms.</span> <span m="1228870">But</span> <span m="1229050">this</span>
  <span m="1229200">is</span> <span m="1229290">for</span> <span m="1229410">kind</span>
  <span m="1229590">of</span> <span m="1230250">more</span> <span m="1230400">harder</span>
  <span m="1230670">reasons</span> <span m="1230970">than</span> <span m="1231050">that.</span></p><p><span
  m="1231745">We're</span> <span m="1232220">going</span> <span m="1232400">to</span>
  <span m="1232500">get</span> <span m="1232650">the</span> <span m="1232740">prediction</span>
  <span m="1233130">for</span> <span m="1233220">the</span> <span m="1233280">whole</span>
  <span m="1233460">exam</span> <span m="1233910">by</span> <span m="1234180">taking</span>
  <span m="1234390">the</span> <span m="1234480">maximum</span> <span m="1235080">across</span>
  <span m="1235410">the</span> <span m="1235470">different</span> <span m="1235680">images.</span>
  <span m="1236590">So</span> <span m="1236610">if</span> <span m="1236700">I</span>
  <span m="1236760">say</span> <span m="1236970">this</span> <span m="1237270">breast
  has</span> <span m="1237630">cancer,</span> <span m="1238230">the</span> <span m="1238350">exam</span>
  <span m="1238650">has</span> <span m="1238770">cancer.</span> <span m="1239160">So</span>
  <span m="1239520">you</span> <span m="1239790">should</span> <span m="1239910">get</span>
  <span m="1240030">it</span> <span m="1240090">checked</span> <span m="1240480">up.</span></p><p><span
  m="1241710">And</span> <span m="1242820">at</span> <span m="1242970">each</span>
  <span m="1243120">development</span> <span m="1243540">epoch</span> <span m="1244050">we're</span>
  <span m="1244170">going</span> <span m="1244290">to</span> <span m="1244360">evaluate</span>
  <span m="1244740">the</span> <span m="1244860">ability</span> <span m="1245310">of</span>
  <span m="1245370">the</span> <span m="1245430">model</span> <span m="1245670">to</span>
  <span m="1245790">do</span> <span m="1246030">triage</span> <span m="1246420">task,</span>
  <span m="1246880">which I'll</span> <span m="1247170">step</span> <span m="1247410">into</span>
  <span m="1247590">in a</span> <span m="1247620">second.</span> <span m="1248420">And</span>
  <span m="1248460">we're</span> <span m="1248580">going</span> <span m="1248680">to</span>
  <span m="1248760">kind</span> <span m="1248940">of</span> <span m="1249000">take</span>
  <span m="1249150">the</span> <span m="1249240">best</span> <span m="1249930">model</span>
  <span m="1250320">that</span> <span m="1250440">can</span> <span m="1250560">do</span>
  <span m="1250690">triage.</span></p><p><span m="1251490">So</span> <span m="1251610">you're</span>
  <span m="1251700">always</span> <span m="1251970">kind</span> <span m="1252120">of</span>
  <span m="1252210">like,</span> <span m="1253140">your</span> <span m="1253260">true</span>
  <span m="1253620">end</span> <span m="1253830">metric</span> <span m="1254370">is</span>
  <span m="1254520">what</span> <span m="1254640">you're</span> <span m="1254730">measuring</span>
  <span m="1255180">during</span> <span m="1255390">training.</span> <span m="1255850">And</span>
  <span m="1255950">you're</span> <span m="1256050">going</span> <span m="1256150">to</span>
  <span m="1256250">do</span> <span m="1256620">model</span> <span m="1256950">selection</span>
  <span m="1257220">and</span> <span m="1257360">kind</span> <span m="1257470">of</span>
  <span m="1257540">hyper</span> <span m="1257950">patching</span> <span m="1258360">based</span>
  <span m="1258540">on</span> <span m="1258660">that.</span></p><p><span m="1259830">And</span>
  <span m="1260520">the</span> <span m="1260670">way</span> <span m="1261210">we're</span>
  <span m="1261360">going</span> <span m="1261490">to</span> <span m="1261530">do</span>
  <span m="1261630">triage</span> <span m="1262080">and</span> <span m="1262200">our</span>
  <span m="1262290">goal</span> <span m="1262530">here</span> <span m="1262800">is</span>
  <span m="1264410">to</span> <span m="1264660">mark</span> <span m="1264930">as</span>
  <span m="1265020">many</span> <span m="1265860">people</span> <span m="1266250">as</span>
  <span m="1266340">healthy</span> <span m="1266580">without</span> <span m="1266730">missing</span>
  <span m="1267120">a</span> <span m="1267150">single</span> <span m="1267480">cancer</span>
  <span m="1267900">that</span> <span m="1268050">we</span> <span m="1268220">always</span>
  <span m="1268400">would</span> <span m="1268490">have</span> <span m="1268620">caught.</span>
  <span m="1269460">So</span> <span m="1269730">intuitively</span> <span m="1270035">kind
  of by</span> <span m="1271040">taking</span> <span m="1271350">all</span> <span
  m="1271500">the</span> <span m="1271590">cancers</span> <span m="1271920">that the</span>
  <span m="1271980">radiologist</span> <span m="1272150">would</span> <span m="1272400">have</span>
  <span m="1272610">caught,</span> <span m="1273270">what's</span> <span m="1273450">the</span>
  <span m="1273540">probability</span> <span m="1274170">of</span> <span m="1274260">cancer</span>
  <span m="1274650">across</span> <span m="1274920">these</span> <span m="1275550">images,</span>
  <span m="1276360">and just</span> <span m="1276540">take</span> <span m="1276690">the</span>
  <span m="1276780">minimum</span> <span m="1276950">of those</span> <span m="1277110">and</span>
  <span m="1277200">call</span> <span m="1277380">that</span> <span m="1277470">the</span>
  <span m="1277530">threshold.</span> <span m="1278340">That's</span> <span m="1278460">exactly</span>
  <span m="1278790">what</span> <span m="1278910">we</span> <span m="1279000">do.</span></p><p><span
  m="1281010">And</span> <span m="1281460">another</span> <span m="1281970">detail</span>
  <span m="1282420">that's</span> <span m="1282900">quite</span> <span m="1283170">relevant</span>
  <span m="1283710">often</span> <span m="1284280">is</span> <span m="1285210">if</span>
  <span m="1285330">you</span> <span m="1285420">want</span> <span m="1285600">these</span>
  <span m="1285750">models</span> <span m="1285960">to</span> <span m="1286080">output</span>
  <span m="1286740">a</span> <span m="1286830">reasonable</span> <span m="1287130">probability</span>
  <span m="1287550">like</span> <span m="1287700">this is</span> <span m="1287850">the</span>
  <span m="1287910">probability</span> <span m="1288270">of</span> <span m="1288330">cancer,</span>
  <span m="1289050">and</span> <span m="1289140">you</span> <span m="1289230">train</span>
  <span m="1289680">on</span> <span m="1289800">a</span> <span m="1289940">50/50</span>
  <span m="1290830">sample</span> <span m="1291320">the</span> <span m="1291400">batches,</span>
  <span m="1292320">by</span> <span m="1292530">default</span> <span m="1292920">your</span>
  <span m="1293370">model</span> <span m="1293700">thinks</span> <span m="1294000">that</span>
  <span m="1294180">the</span> <span m="1294360">average</span> <span m="1294630">incidence</span>
  <span m="1294900">is</span> <span m="1294960">50%.</span> <span m="1295570">So</span>
  <span m="1295900">it's</span> <span m="1296040">crazy</span> <span m="1296310">confidence</span>
  <span m="1296670">all</span> <span m="1296760">the</span> <span m="1296850">time.</span></p><p><span
  m="1297540">So</span> <span m="1297660">to</span> <span m="1297780">calibrate</span>
  <span m="1298200">that</span> <span m="1298380">one</span> <span m="1298530">really</span>
  <span m="1298710">simple</span> <span m="1298980">trick</span> <span m="1299310">is</span>
  <span m="1299460">you</span> <span m="1299790">do</span> <span m="1299940">something</span>
  <span m="1300090">called</span> <span m="1300210">Platt's</span> <span m="1300480">Method</span>
  <span m="1301580">where</span> <span m="1301760">you</span> <span m="1301860">basically</span>
  <span m="1302220">just</span> <span m="1302370">fit</span> <span m="1303120">like</span>
  <span m="1303270">a</span> <span m="1303300">two-parameter</span> <span m="1303810">sigmoid</span>
  <span m="1304200">or</span> <span m="1304280">just</span> <span m="1304500">scale</span>
  <span m="1304770">and</span> <span m="1304860">a</span> <span m="1304890">shift</span>
  <span m="1305580">to</span> <span m="1305730">just--</span> <span m="1306230">on</span>
  <span m="1306560">the</span> <span m="1306630">development</span> <span m="1306990">sets</span>
  <span m="1307230">to</span> <span m="1307320">make</span> <span m="1307470">it</span>
  <span m="1307560">actually</span> <span m="1307800">fit</span> <span m="1308010">the</span>
  <span m="1308070">distribution.</span> <span m="1309250">That</span> <span m="1309420">way</span>
  <span m="1309540">the</span> <span m="1309630">average</span> <span m="1310020">probability</span>
  <span m="1310560">you</span> <span m="1310650">would</span> <span m="1310740">expect</span>
  <span m="1311140">to</span> <span m="1311250">actually</span> <span m="1311460">fit</span>
  <span m="1311610">the</span> <span m="1311670">incidence.</span> <span m="1312430">And</span>
  <span m="1312520">you</span> <span m="1312580">don't</span> <span m="1312780">get</span>
  <span m="1312900">this</span> <span m="1313020">kind</span> <span m="1313140">of</span>
  <span m="1313230">like</span> <span m="1313410">crazy</span> <span m="1314550">off-kilter</span>
  <span m="1315510">probabilities.</span></p><p><span m="1316800">OK.</span> <span
  m="1317370">So</span> <span m="1317760">analysis.</span> <span m="1319480">The</span>
  <span m="1319620">objectives</span> <span m="1320340">of</span> <span m="1320460">what</span>
  <span m="1320550">we</span> <span m="1320670">would</span> <span m="1320760">try</span>
  <span m="1320950">to</span> <span m="1321030">do</span> <span m="1321180">here</span>
  <span m="1321330">is</span> <span m="1321420">kind</span> <span m="1321570">of</span>
  <span m="1321630">similar</span> <span m="1321870">across</span> <span m="1322080">all</span>
  <span m="1322140">the</span> <span m="1322200">projects.</span> <span m="1323130">One,</span>
  <span m="1323520">does</span> <span m="1323730">this</span> <span m="1323850">thing</span>
  <span m="1324000">work?</span> <span m="1324770">Two,</span> <span m="1325060">does
  this</span> <span m="1325230">thing</span> <span m="1325440">work</span> <span m="1325770">across</span>
  <span m="1326160">all</span> <span m="1326250">the</span> <span m="1326340">people</span>
  <span m="1326610">it's</span> <span m="1326700">supposed</span> <span m="1326850">to</span>
  <span m="1326910">work</span> <span m="1327040">for?</span></p><p><span m="1328290">So</span>
  <span m="1328530">we</span> <span m="1328650">did</span> <span m="1328800">a</span>
  <span m="1328860">subgroup</span> <span m="1329220">analysis.</span> <span m="1329580">First</span>
  <span m="1329890">we</span> <span m="1329990">looked</span> <span m="1330090">at</span>
  <span m="1330190">the</span> <span m="1330360">AUC</span> <span m="1330480">in</span>
  <span m="1330720">this</span> <span m="1330840">model.</span> <span m="1331170">So</span>
  <span m="1331440">the</span> <span m="1331560">ability</span> <span m="1331910">to</span>
  <span m="1332310">discriminate</span> <span m="1332520">cancer</span> <span m="1332970">is</span>
  <span m="1333090">not.</span> <span m="1333840">We</span> <span m="1333960">did</span>
  <span m="1334110">it</span> <span m="1334230">across</span> <span m="1334620">races.</span>
  <span m="1335140">We</span> <span m="1335160">have</span> <span m="1335950">across</span>
  <span m="1336030">MGH,</span> <span m="1336780">age</span> <span m="1336990">groups,</span>
  <span m="1337290">and</span> <span m="1337410">density</span> <span m="1337710">categories.</span>
  <span m="1339270">And</span> <span m="1339420">finally,</span> <span m="1339880">how</span>
  <span m="1339980">does</span> <span m="1339990">this</span> <span m="1340110">relate</span>
  <span m="1340440">to</span> <span m="1340530">radiologist's</span> <span m="1340870">assessments?</span>
  <span m="1342360">And</span> <span m="1343110">if</span> <span m="1343260">we</span>
  <span m="1343380">actually</span> <span m="1343710">use</span> <span m="1343980">this</span>
  <span m="1344470">at</span> <span m="1344580">test</span> <span m="1344820">time</span>
  <span m="1345030">on</span> <span m="1345090">the</span> <span m="1345180">test</span>
  <span m="1345400">set,</span> <span m="1345510">what</span> <span m="1345630">would</span>
  <span m="1345710">have</span> <span m="1345810">happened?</span> <span m="1346560">Kind</span>
  <span m="1346740">of</span> <span m="1346800">a</span> <span m="1346820">simulation</span>
  <span m="1347095">before</span> <span m="1347370">a</span> <span m="1347790">full</span>
  <span m="1348000">clinical</span> <span m="1348300">implementation.</span></p><p><span
  m="1351700">So</span> <span m="1352120">overall</span> <span m="1352435">AUC</span>
  <span m="1353080">here</span> <span m="1353380">was</span> <span m="1353610">82</span>
  <span m="1354900">with</span> <span m="1355030">some</span> <span m="1355870">confident</span>
  <span m="1356150">from</span> <span m="1356350">80 to</span> <span m="1356590">85.</span>
  <span m="1357160">And</span> <span m="1357250">we</span> <span m="1357460">did</span>
  <span m="1357640">our</span> <span m="1357760">analysis</span> <span m="1358240">by</span>
  <span m="1358390">age.</span> <span m="1359210">We</span> <span m="1359230">found</span>
  <span m="1359410">that</span> <span m="1359530">the</span> <span m="1359590">performance</span>
  <span m="1360370">was</span> <span m="1360550">pretty</span> <span m="1360820">similar</span>
  <span m="1361120">across</span> <span m="1361360">every</span> <span m="1361540">age</span>
  <span m="1361720">group.</span></p><p><span m="1362440">What's</span> <span m="1362650">not</span>
  <span m="1362860">shown</span> <span m="1363070">here</span> <span m="1363310">is</span>
  <span m="1363400">the</span> <span m="1363460">confidence</span> <span m="1363850">intervals.</span>
  <span m="1365210">So</span> <span m="1365290">for</span> <span m="1365380">example--</span>
  <span m="1366280">but</span> <span m="1366670">the</span> <span m="1366820">kind</span>
  <span m="1367000">of</span> <span m="1367090">key</span> <span m="1367220">core</span>
  <span m="1367420">takeaway</span> <span m="1367720">here</span> <span m="1367900">is</span>
  <span m="1367990">that</span> <span m="1369790">there</span> <span m="1370180">was</span>
  <span m="1370300">no</span> <span m="1370450">noticeable</span> <span m="1370900">gap</span>
  <span m="1371290">in</span> <span m="1371350">terms</span> <span m="1371590">of</span>
  <span m="1371650">by</span> <span m="1371830">age</span> <span m="1372040">group.</span>
  <span m="1372790">We</span> <span m="1372880">repeated</span> <span m="1373210">this</span>
  <span m="1373360">analysis</span> <span m="1373870">by</span> <span m="1374020">race,</span>
  <span m="1374470">and</span> <span m="1374590">we</span> <span m="1374680">saw</span>
  <span m="1375730">the</span> <span m="1375850">same</span> <span m="1376060">trend</span>
  <span m="1376240">again.</span> <span m="1376730">The</span> <span m="1376760">performance</span>
  <span m="1377230">kind</span> <span m="1377350">of</span> <span m="1377440">ranged</span>
  <span m="1378550">generally</span> <span m="1378970">around</span> <span m="1379330">82.</span>
  <span m="1381000">And</span> <span m="1381190">in</span> <span m="1381280">places</span>
  <span m="1381580">where</span> <span m="1381820">the</span> <span m="1381940">gap</span>
  <span m="1382300">was</span> <span m="1382420">bigger,</span> <span m="1382960">the</span>
  <span m="1383140">just</span> <span m="1383300">confidence</span> <span m="1383710">interval</span>
  <span m="1384100">was</span> <span m="1384280">bigger</span> <span m="1384550">accordingly</span>
  <span m="1385960">due</span> <span m="1386080">to</span> <span m="1386170">smaller</span>
  <span m="1386500">sample</span> <span m="1386770">sizes,</span> <span m="1387190">cause</span>
  <span m="1387400">MGH</span> <span m="1387490">is</span> <span m="1387910">80%</span>
  <span m="1388360">white.</span></p><p><span m="1389740">We</span> <span m="1389890">saw</span>
  <span m="1390130">the</span> <span m="1390250">exact</span> <span m="1390580">same</span>
  <span m="1390850">trend</span> <span m="1391360">by</span> <span m="1391570">density.</span>
  <span m="1392290">The</span> <span m="1392410">outlier</span> <span m="1392770">here</span>
  <span m="1393100">is</span> <span m="1393250">very</span> <span m="1393550">dense</span>
  <span m="1393760">breasts.</span> <span m="1394420">But</span> <span m="1394660">there's</span>
  <span m="1394870">only</span> <span m="1395110">like</span> <span m="1395270">100</span>
  <span m="1395590">of</span> <span m="1395650">those</span> <span m="1395830">on</span>
  <span m="1396020">test set.</span> <span m="1396310">So</span> <span m="1396640">this</span>
  <span m="1396760">confidence</span> <span m="1397120">actually</span> <span m="1397300">goes</span>
  <span m="1397420">from</span> <span m="1397540">like,</span> <span m="1398260">60</span>
  <span m="1398620">to</span> <span m="1398710">90.</span> <span m="1399670">So</span>
  <span m="1400390">as</span> <span m="1400510">far</span> <span m="1400660">as</span>
  <span m="1400750">we</span> <span m="1400870">know</span> <span m="1401110">for</span>
  <span m="1401260">the</span> <span m="1401440">other</span> <span m="1401650">three</span>
  <span m="1401830">categories,</span> <span m="1402430">it</span> <span m="1402550">is</span>
  <span m="1403300">very</span> <span m="1403840">much</span> <span m="1404050">tied</span>
  <span m="1404220">to</span> <span m="1404290">confidence</span> <span m="1404560">interval</span>
  <span m="1404860">and</span> <span m="1404980">very</span> <span m="1405130">similar,</span>
  <span m="1405460">once</span> <span m="1405640">again,</span> <span m="1405850">around</span>
  <span m="1406870">82.</span></p><p><span m="1409180">OK.</span> <span m="1409500">So</span>
  <span m="1409620">we</span> <span m="1409740">have</span> <span m="1409890">a</span>
  <span m="1409980">decent</span> <span m="1410370">idea</span> <span m="1410760">that</span>
  <span m="1411450">this</span> <span m="1411630">model</span> <span m="1412260">seems</span>
  <span m="1412570">at</span> <span m="1412630">least</span> <span m="1412770">with</span>
  <span m="1412890">a</span> <span m="1412960">publish</span> <span m="1413360">of</span>
  <span m="1413430">MGH</span> <span m="1415050">actually</span> <span m="1415410">serve</span>
  <span m="1415650">the</span> <span m="1415740">relevant</span> <span m="1415970">populations</span>
  <span m="1417930">that</span> <span m="1418050">exist</span> <span m="1418290">as</span>
  <span m="1418380">far</span> <span m="1418500">as</span> <span m="1418590">we</span>
  <span m="1418650">know</span> <span m="1418770">so</span> <span m="1418890">far.</span>
  <span m="1420280">The</span> <span m="1420300">next</span> <span m="1420510">question</span>
  <span m="1420810">is,</span> <span m="1421930">how</span> <span m="1421980">does</span>
  <span m="1422150">the</span> <span m="1422190">model</span> <span m="1422500">assessment</span>
  <span m="1422820">relate</span> <span m="1423030">to</span> <span m="1423120">the</span>
  <span m="1423220">radiologist's</span> <span m="1423570">assessment?</span></p><p><span
  m="1423990">So</span> <span m="1424410">to</span> <span m="1424560">look</span>
  <span m="1424740">at</span> <span m="1424830">that</span> <span m="1425000">we</span>
  <span m="1425100">looked</span> <span m="1425280">at</span> <span m="1425400">on</span>
  <span m="1425520">the</span> <span m="1425610">test,</span> <span m="1425940">if</span>
  <span m="1426030">you</span> <span m="1426090">look</span> <span m="1426180">at</span>
  <span m="1426240">the</span> <span m="1426300">radiologist's</span> <span m="1426630">true</span>
  <span m="1426840">positives,</span> <span m="1428310">false</span> <span m="1428640">positives,</span>
  <span m="1429720">true</span> <span m="1429900">negatives,</span> <span m="1430260">false</span>
  <span m="1430410">negatives.</span> <span m="1431220">Where</span> <span m="1431400">do</span>
  <span m="1431490">they</span> <span m="1431610">fall</span> <span m="1431870">within</span>
  <span m="1432030">the</span> <span m="1432120">model</span> <span m="1432350">distribution</span>
  <span m="1433080">of</span> <span m="1433350">percentile</span> <span m="1433890">risk?</span>
  <span m="1434790">And</span> <span m="1435180">if</span> <span m="1435330">there</span>
  <span m="1435400">is</span> <span m="1435510">below</span> <span m="1435750">the</span>
  <span m="1435870">threshold,</span> <span m="1436260">we've</span> <span m="1436350">got</span>
  <span m="1436470">to</span> <span m="1436530">color</span> <span m="1436820">it</span>
  <span m="1436890">in</span> <span m="1436980">this</span> <span m="1437100">kind</span>
  <span m="1437250">of</span> <span m="1437340">cyan</span> <span m="1437700">color.</span>
  <span m="1438580">And</span> <span m="1438780">if</span> <span m="1438870">it's</span>
  <span m="1438990">above</span> <span m="1439200">the</span> <span m="1439290">threshold,</span>
  <span m="1439680">we're</span> <span m="1439770">going</span> <span m="1439890">to</span>
  <span m="1439950">color it</span> <span m="1440400">in</span> <span m="1440550">this</span>
  <span m="1441420">purple</span> <span m="1441690">color.</span> <span m="1442480">So</span>
  <span m="1442500">this</span> <span m="1442650">is</span> <span m="1442800">kind</span>
  <span m="1442950">of</span> <span m="1443010">triage,</span> <span m="1443370">not</span>
  <span m="1443520">triage.</span></p><p><span m="1444670">The</span> <span m="1444770">first</span>
  <span m="1444840">thing</span> <span m="1444930">to</span> <span m="1445060">notice--</span>
  <span m="1445530">this</span> <span m="1445680">is</span> <span m="1445740">the</span>
  <span m="1445830">true</span> <span m="1446010">positives--</span> <span m="1446940">is</span>
  <span m="1447090">that</span> <span m="1447300">there</span> <span m="1447470">is</span>
  <span m="1447570">like</span> <span m="1447720">a</span> <span m="1447780">pretty</span>
  <span m="1448860">kind</span> <span m="1449080">of</span> <span m="1449160">steep</span>
  <span m="1449520">drop-off.</span> <span m="1451050">And</span> <span m="1451200">so</span>
  <span m="1452650">there</span> <span m="1452940">is</span> <span m="1453220">only</span>
  <span m="1453490">one</span> <span m="1453820">true</span> <span m="1454000">positive</span>
  <span m="1454410">fell</span> <span m="1454570">below</span> <span m="1454780">the</span>
  <span m="1454870">threshold</span> <span m="1455320">in</span> <span m="1455410">a</span>
  <span m="1455470">test</span> <span m="1455670">set</span> <span m="1455740">of</span>
  <span m="1455830">26,000</span> <span m="1456520">exams.</span> <span m="1457330">So</span>
  <span m="1457450">none</span> <span m="1457630">of</span> <span m="1457810">this</span>
  <span m="1458230">difference</span> <span m="1458650">was</span> <span m="1458910">statistically</span>
  <span m="1459190">significant.</span> <span m="1460540">And</span> <span m="1460870">the</span>
  <span m="1460990">vast</span> <span m="1461230">majority</span> <span m="1461650">of</span>
  <span m="1461740">them</span> <span m="1462040">are</span> <span m="1462190">kind</span>
  <span m="1462370">of</span> <span m="1462490">this</span> <span m="1462700">top</span>
  <span m="1463000">10%.</span></p><p><span m="1463750">But</span> <span m="1463870">you</span>
  <span m="1463960">kind</span> <span m="1464140">of</span> <span m="1464230">see,</span>
  <span m="1464410">like,</span> <span m="1464530">there's</span> <span m="1464680">a</span>
  <span m="1464740">clear</span> <span m="1464950">trend</span> <span m="1465160">here</span>
  <span m="1465730">that</span> <span m="1465880">they</span> <span m="1465970">kind</span>
  <span m="1466090">of</span> <span m="1466180">get</span> <span m="1466630">piled</span>
  <span m="1467050">up</span> <span m="1467170">towards</span> <span m="1467470">the</span>
  <span m="1467560">higher</span> <span m="1467770">percentages.</span> <span m="1469630">Whereas
  if</span> <span m="1469930">you</span> <span m="1469990">look</span> <span m="1470110">at</span>
  <span m="1470170">the</span> <span m="1470230">false</span> <span m="1470460">positive</span>
  <span m="1470740">assessments,</span> <span m="1471470">this</span> <span m="1471640">trend</span>
  <span m="1471970">is</span> <span m="1472060">much</span> <span m="1472240">weaker.</span>
  <span m="1473000">So</span> <span m="1473020">you</span> <span m="1473110">still</span>
  <span m="1473290">see</span> <span m="1473440">that</span> <span m="1473590">there</span>
  <span m="1473750">is</span> <span m="1473860">some</span> <span m="1475630">correlation</span>
  <span m="1476200">that</span> <span m="1476290">there's</span> <span m="1476470">going</span>
  <span m="1476590">to</span> <span m="1476680">more</span> <span m="1476980">false</span>
  <span m="1477220">positives</span> <span m="1477580">the</span> <span m="1477670">higher</span>
  <span m="1477910">amounts,</span> <span m="1478810">but</span> <span m="1479080">much</span>
  <span m="1479380">less</span> <span m="1479770">stark.</span> <span m="1480530">And</span>
  <span m="1480610">this</span> <span m="1480760">actually</span> <span m="1481030">means</span>
  <span m="1481210">that</span> <span m="1481330">a</span> <span m="1481390">lot</span>
  <span m="1481660">of</span> <span m="1481760">radiologist's</span> <span m="1482080">false</span>
  <span m="1482350">positives</span> <span m="1483220">we</span> <span m="1483310">actually</span>
  <span m="1483490">place</span> <span m="1483670">below</span> <span m="1483970">the</span>
  <span m="1484060">threshold.</span></p><p><span m="1484960">And</span> <span m="1485080">so</span>
  <span m="1485350">because</span> <span m="1485770">these</span> <span m="1486070">assessments</span>
  <span m="1486470">are</span> <span m="1486580">completely</span> <span m="1486910">concordant</span>
  <span m="1487390">and</span> <span m="1487480">we're</span> <span m="1487570">not</span>
  <span m="1487690">just</span> <span m="1487840">modeling</span> <span m="1488590">what</span>
  <span m="1488770">the</span> <span m="1488860">radiologist</span> <span m="1489040">would</span>
  <span m="1489190">have</span> <span m="1489280">said,</span> <span m="1490240">we</span>
  <span m="1490450">get</span> <span m="1491260">an</span> <span m="1491440">anticipated</span>
  <span m="1491860">benefit</span> <span m="1492280">of</span> <span m="1492370">actually</span>
  <span m="1492610">reducing</span> <span m="1493480">the</span> <span m="1493570">false</span>
  <span m="1493780">positives</span> <span m="1495040">significantly</span> <span
  m="1495760">because</span> <span m="1496570">of</span> <span m="1496690">the</span>
  <span m="1496780">weight</span> <span m="1496930">of</span> <span m="1497020">disagreeing.</span></p><p><span
  m="1498340">And</span> <span m="1498490">finally,</span> <span m="1498880">kind</span>
  <span m="1499060">of</span> <span m="1500410">aiding</span> <span m="1500650">that</span>
  <span m="1500800">further,</span> <span m="1501830">if</span> <span m="1501930">you</span>
  <span m="1502030">look</span> <span m="1502130">at</span> <span m="1502230">the</span>
  <span m="1502330">true</span> <span m="1502430">negative</span> <span m="1502480">assessments,</span>
  <span m="1503790">there</span> <span m="1504100">is</span> <span m="1504220">not</span>
  <span m="1504370">that</span> <span m="1504490">much</span> <span m="1505390">trending</span>
  <span m="1505930">between</span> <span m="1506350">where</span> <span m="1506590">it</span>
  <span m="1506680">falls</span> <span m="1506920">within</span> <span m="1507100">this.</span>
  <span m="1507370">So</span> <span m="1507610">it</span> <span m="1507730">shows</span>
  <span m="1508060">that</span> <span m="1510380">they're</span> <span m="1510590">kind</span>
  <span m="1510830">of</span> <span m="1511910">picking</span> <span m="1512210">up</span>
  <span m="1512330">on</span> <span m="1512390">different</span> <span m="1512660">things</span>
  <span m="1512960">and</span> <span m="1513050">they're--</span> <span m="1513200">where</span>
  <span m="1513440">they</span> <span m="1513560">disagree</span> <span m="1514050">gives
  them</span> <span m="1514220">both</span> <span m="1514400">areas</span> <span m="1514600">to</span>
  <span m="1514670">improve</span> <span m="1515360">and</span> <span m="1515650">ancillary</span>
  <span m="1516080">benefits</span> <span m="1517220">because</span> <span m="1518090">now</span>
  <span m="1518240">we</span> <span m="1518440">can</span> <span m="1518450">reduce</span>
  <span m="1518630">false</span> <span m="1518780">positives.</span></p><p><span m="1520150">This</span>
  <span m="1520580">directly</span> <span m="1520940">leads</span> <span m="1521110">into</span>
  <span m="1521270">assimilating</span> <span m="1521780">the</span> <span m="1521900">impact.</span>
  <span m="1522990">So</span> <span m="1523040">one</span> <span m="1523190">of</span>
  <span m="1523250">the</span> <span m="1523350">things</span> <span m="1523400">we</span>
  <span m="1523460">did,</span> <span m="1523580">we just</span> <span m="1523670">said,</span>
  <span m="1523980">OK.</span> <span m="1524090">If</span> <span m="1524210">people</span>
  <span m="1524960">retrospective</span> <span m="1525470">on</span> <span m="1525560">the</span>
  <span m="1525620">test</span> <span m="1525830">set</span> <span m="1526040">as</span>
  <span m="1526190">a</span> <span m="1526270">simulation</span> <span m="1526760">before</span>
  <span m="1527000">which</span> <span m="1527180">truly</span> <span m="1527360">plug</span>
  <span m="1527570">it</span> <span m="1527630">in,</span> <span m="1528410">if</span>
  <span m="1528560">people</span> <span m="1529010">didn't</span> <span m="1529340">rebuild</span>
  <span m="1529690">the</span> <span m="1529790">triage</span> <span m="1530210">threshold--</span>
  <span m="1531030">so</span> <span m="1531080">we</span> <span m="1531200">can't</span>
  <span m="1531380">catch</span> <span m="1531560">any</span> <span m="1531670">more</span>
  <span m="1531830">cancer</span> <span m="1532100">this</span> <span m="1532290">way,
  but we</span> <span m="1532460">can</span> <span m="1532550">reduce</span> <span
  m="1532790">false</span> <span m="1532970">positives--</span> <span m="1533910">what</span>
  <span m="1533990">would</span> <span m="1534080">have</span> <span m="1534170">happened?</span></p><p><span
  m="1534920">So</span> <span m="1535370">at</span> <span m="1535460">the</span> <span
  m="1535520">top</span> <span m="1536430">we</span> <span m="1536480">have</span>
  <span m="1536690">the</span> <span m="1536810">original</span> <span m="1537290">performance.</span>
  <span m="1538290">So</span> <span m="1538310">this</span> <span m="1538460">is</span>
  <span m="1538550">looking</span> <span m="1538800">at</span> <span m="1538940">100%
  of</span> <span m="1539180">mammograms,</span> <span m="1539630">sensitivity</span>
  <span m="1540140">was</span> <span m="1541160">98.6</span> <span m="1541940">with</span>
  <span m="1542030">specificity</span> <span m="1542450">of</span> <span m="1542510">93.</span>
  <span m="1543530">And</span> <span m="1544040">in</span> <span m="1544160">the</span>
  <span m="1544250">simulation</span> <span m="1545360">the</span> <span m="1545480">sensitivity</span>
  <span m="1545990">dropped</span> <span m="1546845">not</span> <span m="1547250">significantly</span>
  <span m="1547700">to</span> <span m="1547820">90.1,</span> <span m="1549410">but</span>
  <span m="1549590">significantly</span> <span m="1550040">improved</span> <span m="1550240">to</span>
  <span m="1550310">93.7</span> <span m="1551450">while</span> <span m="1551630">looking</span>
  <span m="1551900">at</span> <span m="1552860">81%</span> <span m="1553340">of</span>
  <span m="1553400">the</span> <span m="1553460">mammograms.</span> <span m="1554660">So</span>
  <span m="1554810">this</span> <span m="1554960">is</span> <span m="1555080">like</span>
  <span m="1555740">promising</span> <span m="1556190">preliminary</span> <span m="1556700">data.</span>
  <span m="1557120">But</span> <span m="1557270">to</span> <span m="1557330">reevaluate</span>
  <span m="1557990">this</span> <span m="1558170">and</span> <span m="1558260">go</span>
  <span m="1558380">forward,</span> <span m="1559070">our</span> <span m="1559310">next</span>
  <span m="1559610">step--</span> <span m="1560170">let's</span> <span m="1560430">see</span>
  <span m="1560620">if--</span> <span m="1560770">oh.</span> <span m="1561340">I'm</span>
  <span m="1561440">going</span> <span m="1561560">to</span> <span m="1561770">get</span>
  <span m="1561950">to</span> <span m="1562040">that</span> <span m="1562190">in</span>
  <span m="1562250">a</span> <span m="1562280">second.</span></p><p><span m="1562640">Our</span>
  <span m="1562730">next</span> <span m="1562940">step</span> <span m="1563090">is</span>
  <span m="1563180">we need</span> <span m="1563400">to</span> <span m="1563500">do</span>
  <span m="1563720">clinical</span> <span m="1564050">implementation</span> <span
  m="1565070">to</span> <span m="1565190">really</span> <span m="1565370">figure</span>
  <span m="1565640">out--</span> <span m="1566750">because</span> <span m="1566900">there's</span>
  <span m="1567020">a</span> <span m="1567260">core</span> <span m="1567440">assumption</span>
  <span m="1567740">here</span> <span m="1567920">is</span> <span m="1568040">that</span>
  <span m="1568220">people</span> <span m="1568520">read</span> <span m="1568670">it</span>
  <span m="1568730">the</span> <span m="1568820">same</span> <span m="1569030">way.</span>
  <span m="1569670">But</span> <span m="1569720">if</span> <span m="1569810">you</span>
  <span m="1569900">have</span> <span m="1570050">this</span> <span m="1570170">higher</span>
  <span m="1570410">incidence,</span> <span m="1570950">what</span> <span m="1571130">does</span>
  <span m="1571250">that</span> <span m="1571370">mean?</span> <span m="1572370">Can</span>
  <span m="1572390">you</span> <span m="1572450">focus</span> <span m="1572750">more</span>
  <span m="1573170">on</span> <span m="1573320">the</span> <span m="1573410">people</span>
  <span m="1573680">that</span> <span m="1573770">are</span> <span m="1573860">more</span>
  <span m="1574040">suspicious?</span> <span m="1575000">And</span> <span m="1575750">is</span>
  <span m="1575900">the</span> <span m="1575990">right</span> <span m="1576230">way</span>
  <span m="1576410">to</span> <span m="1576500">do</span> <span m="1576620">this</span>
  <span m="1576860">just</span> <span m="1577070">a</span> <span m="1577160">single</span>
  <span m="1577490">threshold</span> <span m="1577850">to</span> <span m="1577950">not</span>
  <span m="1578150">read?</span> <span m="1578780">Or</span> <span m="1578960">have</span>
  <span m="1579140">a</span> <span m="1579170">double</span> <span m="1579430">ended</span>
  <span m="1579590">with</span> <span m="1579710">the</span> <span m="1579780">seniors</span>
  <span m="1580040">cause</span> <span m="1580100">they're much</span> <span m="1580280">more</span>
  <span m="1580370">likely</span> <span m="1580520">to</span> <span m="1580610">have</span>
  <span m="1580760">cancer.</span></p><p><span m="1581670">And</span> <span m="1581690">so</span>
  <span m="1581810">there</span> <span m="1581990">is</span> <span m="1582860">quite</span>
  <span m="1583100">a</span> <span m="1583160">bit</span> <span m="1583250">of</span>
  <span m="1583310">exploration</span> <span m="1583730">here</span> <span m="1583880">to</span>
  <span m="1584000">say,</span> <span m="1584570">given</span> <span m="1584810">we</span>
  <span m="1584900">have</span> <span m="1585050">these</span> <span m="1585170">tools</span>
  <span m="1585410">that</span> <span m="1585500">give</span> <span m="1585620">us</span>
  <span m="1585680">some</span> <span m="1585830">probability</span> <span m="1586190">of</span>
  <span m="1586280">cancer,</span> <span m="1587120">that's</span> <span m="1587330">not</span>
  <span m="1587510">perfect,</span> <span m="1587900">but</span> <span m="1587990">gives</span>
  <span m="1588170">us</span> <span m="1588230">something.</span> <span m="1588750">How</span>
  <span m="1588880">well</span> <span m="1588980">can</span> <span m="1589130">we</span>
  <span m="1589220">do</span> <span m="1589340">that</span> <span m="1589590">to</span>
  <span m="1589660">improve</span> <span m="1589910">care</span> <span m="1590090">today?</span></p><p><span
  m="1591600">So</span> <span m="1591710">as</span> <span m="1591830">a</span> <span
  m="1592460">quiz,</span> <span m="1592970">can</span> <span m="1593120">you</span>
  <span m="1593210">tell</span> <span m="1593390">which</span> <span m="1593630">of</span>
  <span m="1593720">these</span> <span m="1593930">will</span> <span m="1594050">be</span>
  <span m="1594140">triaged?</span> <span m="1595430">So</span> <span m="1595670">this</span>
  <span m="1595820">is</span> <span m="1595940">no</span> <span m="1596090">cherry-picking.</span>
  <span m="1596630">I</span> <span m="1596690">randomly</span> <span m="1597080">picked</span>
  <span m="1597620">four</span> <span m="1597890">mammograms</span> <span m="1599180">that</span>
  <span m="1599330">were</span> <span m="1599660">below</span> <span m="1600110">and</span>
  <span m="1600230">above</span> <span m="1600410">the</span> <span m="1600530">threshold.</span>
  <span m="1601610">Can</span> <span m="1601700">anyone</span> <span m="1601940">guess</span>
  <span m="1602180">which</span> <span m="1602390">side--</span> <span m="1602930">left</span>
  <span m="1603140">or</span> <span m="1603200">right--</span> <span m="1604100">was</span>
  <span m="1604910">triaged?</span></p><p><span m="1608192">This is</span> <span m="1608670">not</span>
  <span m="1608850">graded,</span> <span m="1609190">Chris,</span> <span m="1609540">so</span>
  <span m="1609900">you</span> <span m="1610430">know.</span></p><p><span m="1610590">AUDIENCE:</span>
  <span m="1610836">Raise</span> <span m="1611082">your hand</span> <span m="1611574">for--</span></p><p><span
  m="1612066">ADAM YALA:</span> <span m="1612230">Oh</span> <span m="1612394">yeah.</span>
  <span m="1612560">Raise</span> <span m="1612750">your</span> <span m="1612870">hand</span>
  <span m="1612990">for the</span> <span m="1613110">left.</span> <span m="1615620">OK.</span>
  <span m="1615950">Raise</span> <span m="1616130">your</span> <span m="1616190">hand</span>
  <span m="1616320">for</span> <span m="1616420">right.</span> <span m="1619580">Here</span>
  <span m="1619800">we</span> <span m="1619920">go.</span> <span m="1621160">Well</span>
  <span m="1621260">done.</span> <span m="1621480">Well</span> <span m="1621660">done.</span></p><p><span
  m="1622840">OK.</span> <span m="1623670">And</span> <span m="1624080">then</span>
  <span m="1624420">next</span> <span m="1624680">step,</span> <span m="1624810">as</span>
  <span m="1624900">I</span> <span m="1624960">said</span> <span m="1625080">before,</span>
  <span m="1625410">is</span> <span m="1625530">we</span> <span m="1625630">need</span>
  <span m="1625770">to</span> <span m="1625980">kind</span> <span m="1626100">of</span>
  <span m="1626160">push</span> <span m="1626360">to the</span> <span m="1626480">clinical</span>
  <span m="1626910">implementation</span> <span m="1627120">because</span> <span m="1627300">that's</span>
  <span m="1627420">where</span> <span m="1627540">the</span> <span m="1628440">rubber</span>
  <span m="1628680">hits</span> <span m="1628860">the</span> <span m="1628950">road.</span>
  <span m="1629340">We</span> <span m="1629590">identify</span> <span m="1630130">is</span>
  <span m="1630160">there</span> <span m="1630270">any</span> <span m="1630480">biases</span>
  <span m="1630960">we</span> <span m="1631110">didn't</span> <span m="1631260">detect?</span>
  <span m="1631910">And we</span> <span m="1632080">need to</span> <span m="1632460">say,</span>
  <span m="1633600">can</span> <span m="1633810">we</span> <span m="1633900">deliver</span>
  <span m="1634230">this</span> <span m="1634380">value?</span></p><p><span m="1636160">So</span>
  <span m="1636210">the</span> <span m="1636300">next</span> <span m="1636510">project</span>
  <span m="1637050">is</span> <span m="1637440">on</span> <span m="1637890">assessing</span>
  <span m="1638310">breast</span> <span m="1638460">cancer</span> <span m="1638760">risk.</span>
  <span m="1640360">So</span> <span m="1640980">this</span> <span m="1641250">is</span>
  <span m="1641520">the</span> <span m="1641640">same</span> <span m="1641900">mammogram</span>
  <span m="1642040">I</span> <span m="1642160">showed</span> <span m="1642320">you</span>
  <span m="1642390">earlier.</span> <span m="1643010">It</span> <span m="1643080">was</span>
  <span m="1643200">diagnosed with</span> <span m="1643590">breast</span> <span m="1643740">cancer</span>
  <span m="1644010">in</span> <span m="1644070">2014.</span> <span m="1644670">It's</span>
  <span m="1644760">actually</span> <span m="1646050">my</span> <span m="1646170">advisor,</span>
  <span m="1646500">Regina's.</span></p><p><span m="1647260">And</span> <span m="1648120">you</span>
  <span m="1648210">can</span> <span m="1648360">see</span> <span m="1648660">that</span>
  <span m="1650400">in</span> <span m="1650600">2013</span> <span m="1651060">you</span>
  <span m="1651180">see</span> <span m="1651280">it's</span> <span m="1651370">there.</span>
  <span m="1651550">In</span> <span m="1651640">2012</span> <span m="1652090">it</span>
  <span m="1652150">looks</span> <span m="1652360">much</span> <span m="1652570">less</span>
  <span m="1654190">prominence.</span> <span m="1654790">And</span> <span m="1655420">five</span>
  <span m="1655750">years</span> <span m="1655960">ago,</span> <span m="1656310">really</span>
  <span m="1656510">looking</span> <span m="1656890">at</span> <span m="1657910">breast</span>
  <span m="1658120">cancer</span> <span m="1658450">risk.</span></p><p><span m="1658880">So</span>
  <span m="1658980">if</span> <span m="1659080">you</span> <span m="1659180">can</span>
  <span m="1659280">tell</span> <span m="1659680">from</span> <span m="1659890">an</span>
  <span m="1659980">image</span> <span m="1660280">that</span> <span m="1660430">is</span>
  <span m="1660580">going</span> <span m="1660730">to</span> <span m="1660790">be</span>
  <span m="1660850">healthy</span> <span m="1661060">for</span> <span m="1661210">a</span>
  <span m="1661240">long</span> <span m="1661390">time,</span> <span m="1662790">you're
  really</span> <span m="1663020">trying</span> <span m="1663190">to</span> <span
  m="1663250">model</span> <span m="1663550">what's</span> <span m="1663790">the</span>
  <span m="1663850">likelihood</span> <span m="1664120">of</span> <span m="1664210">this</span>
  <span m="1664450">breast</span> <span m="1664780">developing</span> <span m="1665260">cancer</span>
  <span m="1665620">in</span> <span m="1665680">the</span> <span m="1665740">future.</span></p><p><span
  m="1666760">Now</span> <span m="1667700">modeling</span> <span m="1668130">breast</span>
  <span m="1668260">cancer</span> <span m="1668530">risk,</span> <span m="1668800">as</span>
  <span m="1668900">Connie earlier</span> <span m="1669280">said,</span> <span m="1669520">is</span>
  <span m="1669610">not</span> <span m="1669850">a</span> <span m="1670660">new</span>
  <span m="1670930">problem.</span> <span m="1671430">It's</span> <span m="1671680">been</span>
  <span m="1671860">a</span> <span m="1671920">quite</span> <span m="1673750">researched</span>
  <span m="1674140">one</span> <span m="1674260">in</span> <span m="1674320">the</span>
  <span m="1674380">community.</span> <span m="1674950">And</span> <span m="1675160">the</span>
  <span m="1675310">more</span> <span m="1675490">classical</span> <span m="1675910">approach</span>
  <span m="1676280">that we're</span> <span m="1676350">gonna</span> <span m="1676460">look</span>
  <span m="1676630">at</span> <span m="1677200">other</span> <span m="1677440">kind</span>
  <span m="1677590">of</span> <span m="1677650">global</span> <span m="1677890">health</span>
  <span m="1678080">factors--</span> <span m="1678430">the</span> <span m="1678490">person's</span>
  <span m="1678850">age,</span> <span m="1679450">their</span> <span m="1679600">family</span>
  <span m="1679900">history,</span> <span m="1681050">whether</span> <span m="1681130">or</span>
  <span m="1681160">not</span> <span m="1681280">they've</span> <span m="1681430">had</span>
  <span m="1681550">menopause,</span> <span m="1682510">and</span> <span m="1682630">kind</span>
  <span m="1682750">of</span> <span m="1682840">any</span> <span m="1683050">other</span>
  <span m="1683330">of</span> <span m="1683400">these</span> <span m="1683560">kind</span>
  <span m="1683680">of</span> <span m="1683770">facts</span> <span m="1684010">we</span>
  <span m="1684070">can</span> <span m="1684640">sort</span> <span m="1684790">of</span>
  <span m="1684850">say</span> <span m="1685000">are</span> <span m="1685090">markers</span>
  <span m="1685510">of</span> <span m="1685600">their</span> <span m="1685690">health</span>
  <span m="1686320">to</span> <span m="1686440">try</span> <span m="1686560">to</span>
  <span m="1686650">predict</span> <span m="1686950">whether</span> <span m="1687220">this</span>
  <span m="1687340">person's</span> <span m="1687610">at</span> <span m="1687700">risk</span>
  <span m="1687910">of</span> <span m="1688030">developing</span> <span m="1688360">breast</span>
  <span m="1688510">cancer.</span></p><p><span m="1689260">People</span> <span m="1689470">have</span>
  <span m="1689540">thought</span> <span m="1689830">that</span> <span m="1689890">the</span>
  <span m="1689980">image</span> <span m="1690220">contains</span> <span m="1690580">something</span>
  <span m="1690820">before.</span> <span m="1691630">The</span> <span m="1691720">way</span>
  <span m="1691840">they've</span> <span m="1691960">thought</span> <span m="1692170">about</span>
  <span m="1692380">this</span> <span m="1692530">is</span> <span m="1692620">through</span>
  <span m="1692800">this</span> <span m="1692920">kind</span> <span m="1693070">of</span>
  <span m="1693130">subjective</span> <span m="1693670">breast</span> <span m="1693820">density</span>
  <span m="1694150">marker.</span> <span m="1695020">And</span> <span m="1695560">the</span>
  <span m="1695740">improvements</span> <span m="1696400">seen</span> <span m="1696970">across</span>
  <span m="1697330">this</span> <span m="1697660">are</span> <span m="1697870">kind</span>
  <span m="1698050">of</span> <span m="1698110">marginal</span> <span m="1698530">from</span>
  <span m="1698680">61</span> <span m="1699130">to</span> <span m="1699190">63.</span></p><p><span
  m="1700690">And</span> <span m="1701820">as</span> <span m="1702250">before,</span>
  <span m="1702610">the</span> <span m="1702700">kind</span> <span m="1702850">of</span>
  <span m="1702940">sketch</span> <span m="1703220">we're going</span> <span m="1703340">to</span>
  <span m="1703410">go</span> <span m="1703540">through</span> <span m="1703770">is</span>
  <span m="1704380">dataset</span> <span m="1704710">collection,</span> <span m="1705310">modeling,</span>
  <span m="1705790">and</span> <span m="1705880">analysis.</span> <span m="1707620">And</span>
  <span m="1707770">dataset</span> <span m="1708130">collection</span> <span m="1708610">we</span>
  <span m="1708730">followed</span> <span m="1708940">a</span> <span m="1708970">very</span>
  <span m="1709150">similar</span> <span m="1709420">template.</span> <span m="1710860">We</span>
  <span m="1710980">saw</span> <span m="1711190">from</span> <span m="1711430">consecutive</span>
  <span m="1711940">mammograms</span> <span m="1712440">from</span> <span m="1712510">2009</span>
  <span m="1712990">to</span> <span m="1713080">2012</span> <span m="1714880">we</span>
  <span m="1715120">took</span> <span m="1715360">outcomes</span> <span m="1715900">from</span>
  <span m="1716170">the</span> <span m="1716550">EHR,</span> <span m="1717190">once</span>
  <span m="1717370">again,</span> <span m="1717880">and</span> <span m="1718060">the</span>
  <span m="1718240">Partners</span> <span m="1718540">Registry.</span></p><p><span
  m="1719530">We</span> <span m="1719680">didn't</span> <span m="1719860">do</span>
  <span m="1719950">exclusions</span> <span m="1720430">based</span> <span m="1720670">on</span>
  <span m="1721120">race</span> <span m="1721450">or</span> <span m="1721480">anything</span>
  <span m="1721890">of</span> <span m="1721980">that</span> <span m="1722120">sort,
  or</span> <span m="1722400">implants.</span> <span m="1723580">But</span> <span
  m="1723730">we</span> <span m="1723850">did</span> <span m="1724000">exclude</span>
  <span m="1724510">negatives</span> <span m="1725050">for</span> <span m="1725230">followup.</span>
  <span m="1725980">So</span> <span m="1726100">if</span> <span m="1726160">someone</span>
  <span m="1726430">didn't</span> <span m="1726610">have</span> <span m="1726730">cancer</span>
  <span m="1727000">in</span> <span m="1727060">three</span> <span m="1727240">years,</span>
  <span m="1727570">but</span> <span m="1727870">disappeared</span> <span m="1728250">from</span>
  <span m="1728380">the</span> <span m="1728440">system,</span> <span m="1728860">we</span>
  <span m="1729240">didn't</span> <span m="1729460">count them</span> <span m="1729750">as</span>
  <span m="1729900">negatives</span> <span m="1730270">that</span> <span m="1730390">we</span>
  <span m="1730540">have</span> <span m="1730690">some</span> <span m="1730810">certainty</span>
  <span m="1731380">in</span> <span m="1731500">both</span> <span m="1731630">the</span>
  <span m="1731680">modeling</span> <span m="1732070">and</span> <span m="1732160">the</span>
  <span m="1732250">analysis.</span> <span m="1733550">And</span> <span m="1734170">as</span>
  <span m="1734290">always,</span> <span m="1734620">we</span> <span m="1734920">split</span>
  <span m="1735070">patients</span> <span m="1735550">into</span> <span m="1735940">train,</span>
  <span m="1736210">dev,</span> <span m="1736360">test.</span></p><p><span m="1738030">The</span>
  <span m="1738160">modeling</span> <span m="1739000">is</span> <span m="1739570">very</span>
  <span m="1739960">similar.</span> <span m="1740420">It's</span> <span m="1740680">the</span>
  <span m="1740800">same</span> <span m="1741310">kind</span> <span m="1741550">of</span>
  <span m="1741610">templated</span> <span m="1742110">lessons</span> <span m="1742630">as</span>
  <span m="1742750">from</span> <span m="1742900">triage,</span> <span m="1744010">except</span>
  <span m="1744490">we</span> <span m="1744700">experimented</span> <span m="1745240">with</span>
  <span m="1745360">a</span> <span m="1745480">model</span> <span m="1745840">that's</span>
  <span m="1745950">only</span> <span m="1746200">the</span> <span m="1746290">image.</span>
  <span m="1747250">And</span> <span m="1747520">for</span> <span m="1747790">the</span>
  <span m="1748150">sake of</span> <span m="1748510">analysis,</span> <span m="1748795">a</span>
  <span m="1749080">model</span> <span m="1749320">that's</span> <span m="1749470">the</span>
  <span m="1750040">image</span> <span m="1750350">model</span> <span m="1750440">I
  just</span> <span m="1750610">talked to you</span> <span m="1750880">before</span>
  <span m="1751660">concatenated</span> <span m="1752230">with</span> <span m="1752350">those</span>
  <span m="1752410">traditional</span> <span m="1752740">risk</span> <span m="1752860">factors</span>
  <span m="1753220">at</span> <span m="1753280">the</span> <span m="1753370">last</span>
  <span m="1753580">layer</span> <span m="1753820">and</span> <span m="1753910">trained</span>
  <span m="1754240">jointly.</span> <span m="1755180">That</span> <span m="1755380">make</span>
  <span m="1755500">sense</span> <span m="1755620">for</span> <span m="1755680">everyone?</span>
  <span m="1756500">So</span> <span m="1756520">I'm</span> <span m="1756640">going
  to</span> <span m="1756680">call</span> <span m="1756880">that</span> <span m="1757480">ImageOnly</span>
  <span m="1758230">an</span> <span m="1758470">Image+RF</span> <span m="1759340">or</span>
  <span m="1759550">hybrid.</span> <span m="1760842">OK.</span> <span m="1761278">Cool?</span></p><p><span
  m="1762590">Our</span> <span m="1763120">kind</span> <span m="1763300">of</span>
  <span m="1763390">goals</span> <span m="1763690">for</span> <span m="1763780">the</span>
  <span m="1763870">analysis.</span> <span m="1764350">As</span> <span m="1764500">before,</span>
  <span m="1764900">we</span> <span m="1764950">want</span> <span m="1765070">to</span>
  <span m="1765130">see</span> <span m="1766270">does</span> <span m="1766630">this</span>
  <span m="1766780">model</span> <span m="1767110">actually</span> <span m="1767440">serve</span>
  <span m="1768040">the</span> <span m="1768790">whole</span> <span m="1768910">population?</span>
  <span m="1769210">Is</span> <span m="1769510">it</span> <span m="1769650">going</span>
  <span m="1769750">to</span> <span m="1769840">be</span> <span m="1769900">discriminative</span>
  <span m="1770500">across</span> <span m="1771280">race,</span> <span m="1771640">menopause</span>
  <span m="1772040">status,</span> <span m="1772330">the</span> <span m="1772420">family</span>
  <span m="1772660">history?</span> <span m="1773910">And</span> <span m="1774070">how</span>
  <span m="1774190">does</span> <span m="1774320">it</span> <span m="1774400">relate</span>
  <span m="1774670">to</span> <span m="1774730">kind</span> <span m="1774940">of</span>
  <span m="1775030">classical</span> <span m="1775390">portions</span> <span m="1775660">of</span>
  <span m="1775750">risk?</span> <span m="1776080">And</span> <span m="1776200">are</span>
  <span m="1776320">we</span> <span m="1776440">actually</span> <span m="1776620">doing</span>
  <span m="1776860">any</span> <span m="1777010">better?</span></p><p><span m="1778380">And</span>
  <span m="1778500">so</span> <span m="1778770">just</span> <span m="1779010">diving</span>
  <span m="1779400">directly</span> <span m="1779700">into</span> <span m="1779900">that,</span>
  <span m="1780360">assuming</span> <span m="1780630">there's</span> <span m="1780780">no</span>
  <span m="1780900">questions.</span> <span m="1782440">Good.</span></p><p><span m="1783260">Just</span>
  <span m="1783350">to kind</span> <span m="1783640">of</span> <span m="1783730">remind</span>
  <span m="1783970">you,</span> <span m="1784110">this</span> <span m="1784270">is</span>
  <span m="1784350">the</span> <span m="1784390">kind</span> <span m="1784540">of</span>
  <span m="1784610">the</span> <span m="1784650">setting.</span> <span m="1785280">One</span>
  <span m="1785310">thing</span> <span m="1785470">I</span> <span m="1785530">forgot</span>
  <span m="1785800">to</span> <span m="1785890">mention--</span> <span m="1786210">that's</span>
  <span m="1786300">why</span> <span m="1786520">I</span> <span m="1786580">had</span>
  <span m="1786700">the</span> <span m="1786760">slide here to</span> <span m="1787090">remind</span>
  <span m="1787330">me--</span> <span m="1788010">is</span> <span m="1788320">that</span>
  <span m="1788500">we</span> <span m="1788740">excluded</span> <span m="1789250">cancers</span>
  <span m="1789700">from</span> <span m="1789880">the</span> <span m="1789970">first</span>
  <span m="1790240">year</span> <span m="1790690">from</span> <span m="1790870">the</span>
  <span m="1790930">test</span> <span m="1791110">set.</span> <span m="1791720">So</span>
  <span m="1791740">there</span> <span m="1791800">is</span> <span m="1791890">truly</span>
  <span m="1792190">a</span> <span m="1792250">negative</span> <span m="1792700">screening</span>
  <span m="1793000">population.</span> <span m="1793900">That</span> <span m="1794140">way
  we</span> <span m="1794620">kind</span> <span m="1794770">of</span> <span m="1794830">disentangle</span>
  <span m="1795310">cancer</span> <span m="1795580">detection</span> <span m="1796030">from</span>
  <span m="1796180">cancer</span> <span m="1796450">risk.</span> <span m="1797570">OK.</span>
  <span m="1797730">Cool.</span></p><p><span m="1799360">So</span> <span m="1800230">Tyrer-Cuzick</span>
  <span m="1800860">is</span> <span m="1800980">the</span> <span m="1801040">kind</span>
  <span m="1801250">of</span> <span m="1801320">prior</span> <span m="1801705">state-of-the-art</span>
  <span m="1802090">model.</span> <span m="1802470">It's</span> <span m="1802620">a
  model</span> <span m="1802730">based</span> <span m="1802900">out</span> <span m="1803020">of</span>
  <span m="1803080">the</span> <span m="1803140">UK.</span> <span m="1805310">Their</span>
  <span m="1806040">developer is</span> <span m="1806660">someone</span> <span m="1806980">named</span>
  <span m="1807190">Sir</span> <span m="1808420">Cuzick,</span> <span m="1808675">who</span>
  <span m="1808930">was</span> <span m="1809080">knighted</span> <span m="1809380">for</span>
  <span m="1809470">this</span> <span m="1809590">work.</span> <span m="1809850">It's</span>
  <span m="1809980">very</span> <span m="1810160">commonly</span> <span m="1810460">used.</span></p><p><span
  m="1811270">So</span> <span m="1811390">that</span> <span m="1811540">one had</span>
  <span m="1811660">an</span> <span m="1811780">AUC</span> <span m="1812020">of</span>
  <span m="1812140">62.</span> <span m="1813160">Our</span> <span m="1813310">image-only</span>
  <span m="1813820">model</span> <span m="1814750">had</span> <span m="1814930">an</span>
  <span m="1815020">AUC</span> <span m="1815320">about</span> <span m="1815500">68.</span>
  <span m="1816940">And</span> <span m="1817270">hybrid</span> <span m="1817690">one</span>
  <span m="1817990">had</span> <span m="1818110">an</span> <span m="1818200">AUC</span>
  <span m="1818440">of</span> <span m="1818500">70.</span></p><p><span m="1819250">So</span>
  <span m="1819370">you</span> <span m="1819430">know,</span> <span m="1819520">what</span>
  <span m="1819700">is</span> <span m="1819850">this</span> <span m="1819970">kind</span>
  <span m="1820120">of</span> <span m="1820230">AUC</span> <span m="1820540">thing</span>
  <span m="1820690">gives</span> <span m="1820910">you</span> <span m="1821000">when</span>
  <span m="1821070">you</span> <span m="1821150">look</span> <span m="1821320">using</span>
  <span m="1821590">a</span> <span m="1821620">risk</span> <span m="1821800">model.</span>
  <span m="1822430">What</span> <span m="1822580">it</span> <span m="1822640">gives</span>
  <span m="1822880">you</span> <span m="1823030">is</span> <span m="1823140">the</span>
  <span m="1823200">ability</span> <span m="1823500">to build</span> <span m="1823570">better</span>
  <span m="1823810">high-risk</span> <span m="1824350">and</span> <span m="1824420">low-risk</span>
  <span m="1824710">cohorts.</span> <span m="1825880">So</span> <span m="1826090">in</span>
  <span m="1826180">terms of</span> <span m="1826320">looking</span> <span m="1826540">at</span>
  <span m="1826600">high-risk</span> <span m="1826960">cohorts,</span> <span m="1827470">our</span>
  <span m="1827560">best</span> <span m="1827800">model</span> <span m="1828040">place</span>
  <span m="1828250">about</span> <span m="1828400">30%</span> <span m="1828970">of</span>
  <span m="1829090">all</span> <span m="1829270">the</span> <span m="1829360">cancers</span>
  <span m="1829900">in</span> <span m="1829990">the</span> <span m="1830050">population</span>
  <span m="1831040">in</span> <span m="1831130">the</span> <span m="1831220">top</span>
  <span m="1831400">10%,</span> <span m="1832840">and</span> <span m="1832990">3%</span>
  <span m="1833530">of</span> <span m="1833620">all</span> <span m="1833690">the</span>
  <span m="1833740">cancers</span> <span m="1834070">in</span> <span m="1834130">the</span>
  <span m="1834190">bottom</span> <span m="1834370">10%</span> <span m="1835210">compared</span>
  <span m="1835570">to</span> <span m="1835720">18</span> <span m="1836590">and</span>
  <span m="1836860">5</span> <span m="1837730">to</span> <span m="1837850">the</span>
  <span m="1837990">prior</span> <span m="1838180">state</span> <span m="1838390">of</span>
  <span m="1838450">the</span> <span m="1838540">art.</span></p><p><span m="1839720">And</span>
  <span m="1839770">so</span> <span m="1839950">what</span> <span m="1840100">this</span>
  <span m="1840220">enables</span> <span m="1840580">you</span> <span m="1840640">to</span>
  <span m="1840730">do,</span> <span m="1840880">if</span> <span m="1840940">you're</span>
  <span m="1841030">going</span> <span m="1841140">to</span> <span m="1841210">say</span>
  <span m="1841390">that</span> <span m="1841480">this</span> <span m="1841840">10%</span>
  <span m="1842290">should</span> <span m="1842500">actually</span> <span m="1842800">qualify</span>
  <span m="1843070">for</span> <span m="1843190">MRI,</span> <span m="1844120">you</span>
  <span m="1844270">can</span> <span m="1844420">start</span> <span m="1844660">fighting</span>
  <span m="1845050">this</span> <span m="1845140">problem</span> <span m="1845530">of</span>
  <span m="1846090">majority of</span> <span m="1846400">people</span> <span m="1846610">that</span>
  <span m="1846700">get</span> <span m="1846820">cancer</span> <span m="1847130">don't</span>
  <span m="1847270">have</span> <span m="1847390">MRI,</span> <span m="1847810">and</span>
  <span m="1848500">the</span> <span m="1848610">majority</span> <span m="1849010">of</span>
  <span m="1849110">people</span> <span m="1849250">that</span> <span m="1849550">get</span>
  <span m="1849760">it</span> <span m="1849880">don't</span> <span m="1850030">need</span>
  <span m="1850210">it.</span> <span m="1850960">It's</span> <span m="1851140">all</span>
  <span m="1851290">about,</span> <span m="1851590">is</span> <span m="1851800">your</span>
  <span m="1851890">risk</span> <span m="1852070">model</span> <span m="1852310">actually</span>
  <span m="1852730">place</span> <span m="1853000">the</span> <span m="1853060">right</span>
  <span m="1853240">people</span> <span m="1853540">into</span> <span m="1853690">the</span>
  <span m="1853780">right</span> <span m="1853900">buckets.</span></p><p><span m="1855670">Now</span>
  <span m="1855880">we</span> <span m="1856000">saw</span> <span m="1856180">that</span>
  <span m="1856300">this</span> <span m="1856450">trend</span> <span m="1856750">of</span>
  <span m="1856900">outperforming</span> <span m="1858040">the</span> <span m="1858100">prior</span>
  <span m="1858310">state</span> <span m="1858460">of</span> <span m="1858520">the</span>
  <span m="1858640">art</span> <span m="1858910">held</span> <span m="1859180">across</span>
  <span m="1859450">races.</span> <span m="1859880">And</span> <span m="1859970">one</span>
  <span m="1860060">of</span> <span m="1860120">the</span> <span m="1860160">things</span>
  <span m="1860320">that</span> <span m="1860410">was</span> <span m="1861100">kind</span>
  <span m="1861280">of</span> <span m="1861340">astonishing</span> <span m="1862390">was</span>
  <span m="1862570">that</span> <span m="1862810">though</span> <span m="1863170">Tyrer-Cuzick</span>
  <span m="1863610">performed</span> <span m="1863860">on</span> <span m="1863980">white</span>
  <span m="1864140">women,</span> <span m="1864500">which</span> <span m="1864580">makes</span>
  <span m="1864760">sense</span> <span m="1864940">because</span> <span m="1865110">it
  was</span> <span m="1865210">developed</span> <span m="1865540">only</span> <span
  m="1865760">using</span> <span m="1866050">white</span> <span m="1866200">women</span>
  <span m="1866530">in</span> <span m="1866620">the</span> <span m="1866710">UK.</span>
  <span m="1867880">It</span> <span m="1868000">was</span> <span m="1868120">worse</span>
  <span m="1868360">than</span> <span m="1868480">random</span> <span m="1868810">[INAUDIBLE]</span>
  <span m="1868990">for</span> <span m="1869260">African-American</span> <span m="1869800">women.</span></p><p><span
  m="1870490">And</span> <span m="1870610">so</span> <span m="1870760">this</span>
  <span m="1870880">kind</span> <span m="1871030">of</span> <span m="1872590">emphasizes</span>
  <span m="1873040">the</span> <span m="1873100">importance</span> <span m="1873530">of
  this</span> <span m="1873640">kind</span> <span m="1873820">of</span> <span m="1873880">analysis</span>
  <span m="1874330">to</span> <span m="1874420">make</span> <span m="1874570">sure</span>
  <span m="1874750">that</span> <span m="1875470">the</span> <span m="1875560">kind</span>
  <span m="1875710">of</span> <span m="1875800">data</span> <span m="1876100">that</span>
  <span m="1876280">you</span> <span m="1876370">have</span> <span m="1876580">is</span>
  <span m="1876670">reflective</span> <span m="1877090">of</span> <span m="1877150">the</span>
  <span m="1877210">population that you're</span> <span m="1877630">trying</span>
  <span m="1877780">to</span> <span m="1877840">serve</span> <span m="1878500">and</span>
  <span m="1878590">actually</span> <span m="1878800">doing</span> <span m="1879220">the</span>
  <span m="1879370">analysis</span> <span m="1880720">accordingly.</span> <span m="1881530">So</span>
  <span m="1881680">we</span> <span m="1881770">saw</span> <span m="1881920">that</span>
  <span m="1882070">our</span> <span m="1882100">model</span> <span m="1882400">kind</span>
  <span m="1882580">of</span> <span m="1882640">held</span> <span m="1882940">across</span>
  <span m="1884500">races</span> <span m="1885030">and</span> <span m="1885190">as</span>
  <span m="1885280">well</span> <span m="1885520">across--</span> <span m="1885970">we</span>
  <span m="1886210">see</span> <span m="1886330">this</span> <span m="1886450">trend</span>
  <span m="1886780">from</span> <span m="1887440">across</span> <span m="1888450">pre-postmenopausal</span>
  <span m="1889045">and</span> <span m="1889390">with and</span> <span m="1889570">without</span>
  <span m="1889770">family</span> <span m="1890020">history.</span></p><p><span m="1892360">One</span>
  <span m="1892600">thing</span> <span m="1892750">we</span> <span m="1892870">did</span>
  <span m="1893020">in</span> <span m="1893080">terms</span> <span m="1893290">of</span>
  <span m="1893440">a</span> <span m="1893500">more</span> <span m="1893650">granular</span>
  <span m="1894100">comparison</span> <span m="1894530">of</span> <span m="1894580">performance,</span>
  <span m="1895570">if we</span> <span m="1896010">just</span> <span m="1896170">look</span>
  <span m="1896280">at</span> <span m="1896380">kind</span> <span m="1896560">of</span>
  <span m="1896620">like</span> <span m="1896740">the</span> <span m="1896830">risk</span>
  <span m="1897140">thirds</span> <span m="1898120">for</span> <span m="1898450">our</span>
  <span m="1898630">model</span> <span m="1898900">and</span> <span m="1899170">the</span>
  <span m="1899490">Tyrer-Cuzick</span> <span m="1899860">model,</span> <span m="1900910">what's</span>
  <span m="1901180">the</span> <span m="1901270">trend</span> <span m="1901540">that</span>
  <span m="1901630">you</span> <span m="1901750">see</span> <span m="1901990">or</span>
  <span m="1902080">the</span> <span m="1902170">cases</span> <span m="1902500">where</span>
  <span m="1903220">kind</span> <span m="1903430">of</span> <span m="1903520">like</span>
  <span m="1903680">which</span> <span m="1903910">one</span> <span m="1904060">is</span>
  <span m="1904150">right</span> <span m="1904370">that's</span> <span m="1904480">kind</span>
  <span m="1904660">of</span> <span m="1905350">ambiguous.</span> <span m="1906730">And</span>
  <span m="1906910">what</span> <span m="1907010">I</span> <span m="1907060">should</span>
  <span m="1907150">show</span> <span m="1907370">in</span> <span m="1907540">these</span>
  <span m="1907660">boxes</span> <span m="1908110">is</span> <span m="1908200">the</span>
  <span m="1908260">cancer</span> <span m="1908590">incidence</span> <span m="1909700">prevalence</span>
  <span m="1910210">in</span> <span m="1910300">the</span> <span m="1910360">population.</span>
  <span m="1911480">So</span> <span m="1911500">the</span> <span m="1911590">darker</span>
  <span m="1911890">the</span> <span m="1911980">box,</span> <span m="1912730">the</span>
  <span m="1912820">higher</span> <span m="1913180">the</span> <span m="1913270">incidence.</span></p><p><span
  m="1913870">And</span> <span m="1914170">on</span> <span m="1914380">the</span>
  <span m="1914560">right-hand</span> <span m="1914770">side</span> <span m="1914920">are</span>
  <span m="1915080">just</span> <span m="1915250">random</span> <span m="1915670">images</span>
  <span m="1916480">from</span> <span m="1916880">cases</span> <span m="1917130">that</span>
  <span m="1917300">fit</span> <span m="1917470">within</span> <span m="1917680">those</span>
  <span m="1917830">boxes.</span> <span m="1918250">Does</span> <span m="1918300">that</span>
  <span m="1918400">make</span> <span m="1918500">sense</span> <span m="1918640">for</span>
  <span m="1918700">everyone?</span> <span m="1920230">Great.</span></p><p><span m="1921020">So</span>
  <span m="1921210">a</span> <span m="1921240">clear</span> <span m="1921510">trend</span>
  <span m="1921660">that</span> <span m="1921780">you</span> <span m="1921900">see</span>
  <span m="1922140">is</span> <span m="1922260">that,</span> <span m="1922540">for</span>
  <span m="1922640">example,</span> <span m="1923080">if</span> <span m="1923980">TCv8</span>
  <span m="1924900">calls</span> <span m="1925230">you</span> <span m="1926000">a</span>
  <span m="1926820">high</span> <span m="1927120">risk</span> <span m="1927360">but</span>
  <span m="1927450">we</span> <span m="1927540">call</span> <span m="1927780">it</span>
  <span m="1927840">low,</span> <span m="1928260">that</span> <span m="1928470">is</span>
  <span m="1928650">a</span> <span m="1928770">lower</span> <span m="1929250">incidence</span>
  <span m="1930180">than</span> <span m="1930360">if</span> <span m="1930480">we</span>
  <span m="1930540">called</span> <span m="1930810">it</span> <span m="1931650">medium
  and</span> <span m="1932100">they</span> <span m="1932190">call</span> <span m="1932430">it</span>
  <span m="1932490">low.</span> <span m="1933000">So</span> <span m="1933180">kind</span>
  <span m="1933330">of</span> <span m="1933390">like</span> <span m="1933510">you</span>
  <span m="1933600">kind</span> <span m="1933750">of</span> <span m="1933810">see</span>
  <span m="1933930">this</span> <span m="1934170">straight</span> <span m="1934980">column-wise</span>
  <span m="1935700">pattern</span> <span m="1936450">showing</span> <span m="1936810">that</span>
  <span m="1936900">discrimination</span> <span m="1937470">truly</span> <span m="1937680">does</span>
  <span m="1937950">follow</span> <span m="1938790">the</span> <span m="1938940">deep
  learning</span> <span m="1939390">model</span> <span m="1939690">and</span> <span
  m="1939810">not</span> <span m="1939960">the</span> <span m="1940050">classical</span>
  <span m="1940440">approach.</span></p><p><span m="1941240">And</span> <span m="1941450">by</span>
  <span m="1941560">looking</span> <span m="1941820">at</span> <span m="1941880">the</span>
  <span m="1942120">random</span> <span m="1942480">images</span> <span m="1942780">that</span>
  <span m="1942900">were</span> <span m="1943020">selected</span> <span m="1943470">in</span>
  <span m="1943530">case</span> <span m="1943710">where</span> <span m="1943800">we</span>
  <span m="1943980">disagree,</span> <span m="1945120">it</span> <span m="1945270">supports</span>
  <span m="1945600">the</span> <span m="1945630">notion</span> <span m="1945870">that</span>
  <span m="1945960">it's</span> <span m="1946020">not</span> <span m="1946140">just</span>
  <span m="1946680">that</span> <span m="1946820">the</span> <span m="1946890">column</span>
  <span m="1947310">is</span> <span m="1947360">just</span> <span m="1947490">the</span>
  <span m="1947580">most</span> <span m="1947760">dense,</span> <span m="1948120">crazy,</span>
  <span m="1948450">dense</span> <span m="1948690">looking</span> <span m="1948900">breast,</span>
  <span m="1949230">that</span> <span m="1949350">there's</span> <span m="1949470">something</span>
  <span m="1949680">more</span> <span m="1949800">subtle</span> <span m="1950230">it's</span>
  <span m="1950250">picking</span> <span m="1950520">up</span> <span m="1950970">that's</span>
  <span m="1951120">actually</span> <span m="1951480">indicative</span> <span m="1952080">of</span>
  <span m="1952140">breast</span> <span m="1952290">cancer</span> <span m="1952590">risk.</span></p><p><span
  m="1954590">Kind</span> <span m="1954770">of</span> <span m="1954830">a</span> <span
  m="1954860">very</span> <span m="1955040">similar</span> <span m="1955430">analysis
  we</span> <span m="1955760">looked at</span> <span m="1956150">as</span> <span m="1956420">if</span>
  <span m="1956540">we</span> <span m="1956630">look</span> <span m="1956870">at</span>
  <span m="1957800">just</span> <span m="1957980">by</span> <span m="1958160">a</span>
  <span m="1958220">traditional</span> <span m="1958580">breast</span> <span m="1958730">density</span>
  <span m="1959180">as</span> <span m="1959330">labeled</span> <span m="1960080">by</span>
  <span m="1960260">the</span> <span m="1960330">original</span> <span m="1960620">radiologist</span>
  <span m="1961250">on</span> <span m="1961430">the</span> <span m="1961580">development</span>
  <span m="1962030">set or</span> <span m="1962350">on</span> <span m="1962510">the</span>
  <span m="1962600">test</span> <span m="1962830">set,</span> <span m="1964250">we</span>
  <span m="1964370">end</span> <span m="1964550">up</span> <span m="1964640">seeing</span>
  <span m="1964820">the</span> <span m="1964880">same</span> <span m="1965090">trend</span>
  <span m="1965420">where</span> <span m="1965600">if</span> <span m="1965660">someone</span>
  <span m="1965960">is</span> <span m="1966870">non-dense</span> <span m="1967460">we</span>
  <span m="1967520">call</span> <span m="1967670">them</span> <span m="1967760">high</span>
  <span m="1967940">risk.</span> <span m="1968270">They're</span> <span m="1968360">much</span>
  <span m="1968540">higher</span> <span m="1968870">risk</span> <span m="1969140">than</span>
  <span m="1969230">someone</span> <span m="1969430">that</span> <span m="1969560">is</span>
  <span m="1969740">dense</span> <span m="1969990">than</span> <span m="1970130">we</span>
  <span m="1970190">call</span> <span m="1970370">low</span> <span m="1970550">risk.</span></p><p><span
  m="1973900">And</span> <span m="1974260">as</span> <span m="1974410">before,</span>
  <span m="1974740">the</span> <span m="1974830">kind</span> <span m="1975010">of</span>
  <span m="1975100">real</span> <span m="1975280">next</span> <span m="1975550">step</span>
  <span m="1975670">here</span> <span m="1975910">to</span> <span m="1976030">make</span>
  <span m="1976210">this</span> <span m="1976780">truly</span> <span m="1977110">valuable</span>
  <span m="1977590">and</span> <span m="1977680">truly</span> <span m="1977980">useful</span>
  <span m="1978850">is</span> <span m="1979450">actually</span> <span m="1979930">implementing</span>
  <span m="1980360">a</span> <span m="1980410">clinically</span> <span m="1980920">seamless</span>
  <span m="1981280">prospectively</span> <span m="1982060">and</span> <span m="1982570">with</span>
  <span m="1982720">more</span> <span m="1982870">centers</span> <span m="1983290">and</span>
  <span m="1983380">kind</span> <span m="1983490">of</span> <span m="1983560">more</span>
  <span m="1983740">population</span> <span m="1984250">to</span> <span m="1984310">see</span>
  <span m="1984910">does</span> <span m="1985150">this</span> <span m="1985300">work</span>
  <span m="1985630">and</span> <span m="1985720">does</span> <span m="1985880">it</span>
  <span m="1986320">deliver</span> <span m="1986680">the</span> <span m="1986740">kind</span>
  <span m="1986920">of</span> <span m="1986980">benefits</span> <span m="1987310">that</span>
  <span m="1987400">we</span> <span m="1987490">care</span> <span m="1987640">about.</span>
  <span m="1988390">And</span> <span m="1988510">viewing</span> <span m="1988930">what</span>
  <span m="1989080">is</span> <span m="1989170">the</span> <span m="1989230">leverage</span>
  <span m="1989610">of</span> <span m="1989680">change</span> <span m="1990030">once</span>
  <span m="1990100">you</span> <span m="1990190">know</span> <span m="1990320">that</span>
  <span m="1990360">someone</span> <span m="1990580">is</span> <span m="1990670">high</span>
  <span m="1990820">risk?</span> <span m="1991630">Perhaps</span> <span m="1991990">MRI,</span>
  <span m="1992260">perhaps</span> <span m="1993160">more</span> <span m="1993400">frequent</span>
  <span m="1993700">screening.</span> <span m="1994000">And</span> <span m="1994090">so</span>
  <span m="1994390">this</span> <span m="1994570">is</span> <span m="1994660">the</span>
  <span m="1994750">kind</span> <span m="1994960">of</span> <span m="1995410">gap</span>
  <span m="1995650">between</span> <span m="1995920">having</span> <span m="1996190">a</span>
  <span m="1996250">useful</span> <span m="1996580">technology</span> <span m="1997660">on</span>
  <span m="1997750">the</span> <span m="1997810">paper</span> <span m="1998080">side</span>
  <span m="1998500">to</span> <span m="1998680">an</span> <span m="1998770">actual</span>
  <span m="1999040">useful</span> <span m="1999230">technology</span> <span m="1999640">in</span>
  <span m="1999730">real</span> <span m="1999880">life.</span></p><p><span m="2001360">So</span>
  <span m="2002080">I</span> <span m="2002370">am</span> <span m="2002820">moving</span>
  <span m="2003240">on</span> <span m="2003390">schedule.</span> <span m="2004240">So</span>
  <span m="2004380">now</span> <span m="2004550">I'm</span> <span m="2004630">gonna</span>
  <span m="2004690">talk</span> <span m="2004860">about</span> <span m="2005010">how</span>
  <span m="2005130">to</span> <span m="2005220">mess</span> <span m="2005400">up.</span>
  <span m="2005760">And</span> <span m="2006870">it's</span> <span m="2007020">actually</span>
  <span m="2007230">quite</span> <span m="2007410">interesting.</span> <span m="2007760">There</span>
  <span m="2007860">is</span> <span m="2007980">like,</span> <span m="2008100">so</span>
  <span m="2008310">many</span> <span m="2008520">ways.</span> <span m="2009490">And</span>
  <span m="2010080">I</span> <span m="2010170">fall</span> <span m="2010380">into</span>
  <span m="2010590">them</span> <span m="2010890">a</span> <span m="2010950">few</span>
  <span m="2011100">times</span> <span m="2011310">myself,</span> <span m="2011730">and</span>
  <span m="2011850">it</span> <span m="2011940">happens.</span></p><p><span m="2013230">And</span>
  <span m="2013470">kind</span> <span m="2013650">of</span> <span m="2013710">following</span>
  <span m="2014040">the</span> <span m="2014160">sketch,</span> <span m="2014550">you</span>
  <span m="2014640">can</span> <span m="2014760">mess</span> <span m="2014910">up</span>
  <span m="2015000">in</span> <span m="2015090">dataset</span> <span m="2015400">collection.</span>
  <span m="2015780">That's</span> <span m="2015900">probably</span> <span m="2016140">the</span>
  <span m="2016200">most</span> <span m="2016380">common</span> <span m="2016650">by</span>
  <span m="2016740">far.</span> <span m="2017050">You</span> <span m="2017390">can
  mess</span> <span m="2017630">up</span> <span m="2017780">in</span> <span m="2017840">modeling,</span>
  <span m="2018970">which</span> <span m="2019020">I'm</span> <span m="2019080">doing</span>
  <span m="2019440">right</span> <span m="2019620">now.</span> <span m="2019990">And</span>
  <span m="2020010">it's</span> <span m="2020100">very</span> <span m="2020250">sad.</span>
  <span m="2021040">And</span> <span m="2021230">you</span> <span m="2021300">can</span>
  <span m="2021390">mess</span> <span m="2021540">up</span> <span m="2021630">in</span>
  <span m="2021720">analysis,</span> <span m="2022170">which</span> <span m="2022290">is</span>
  <span m="2022380">really</span> <span m="2022620">preventable.</span></p><p><span
  m="2024130">So</span> <span m="2024270">in</span> <span m="2024440">dataset</span>
  <span m="2024700">collection,</span> <span m="2026300">enriched</span> <span m="2026530">data</span>
  <span m="2026810">sets</span> <span m="2027120">are</span> <span m="2027240">the</span>
  <span m="2027300">kind</span> <span m="2027480">of</span> <span m="2027570">the</span>
  <span m="2027660">most</span> <span m="2028020">common</span> <span m="2028350">thing</span>
  <span m="2028470">you</span> <span m="2028590">see</span> <span m="2028800">in</span>
  <span m="2028890">this</span> <span m="2028970">space.</span> <span m="2029670">You</span>
  <span m="2029760">find</span> <span m="2029960">in a</span> <span m="2030030">public</span>
  <span m="2030420">data</span> <span m="2030570">set</span> <span m="2030750">that's</span>
  <span m="2030900">most</span> <span m="2031080">likely</span> <span m="2031260">going
  to</span> <span m="2031350">be</span> <span m="2031440">like</span> <span m="2031560">50-50</span>
  <span m="2032130">cancer,</span> <span m="2032420">not</span> <span m="2032550">cancer.</span></p><p><span
  m="2034140">And</span> <span m="2035770">oftentimes</span> <span m="2036340">these</span>
  <span m="2036430">datasets</span> <span m="2036910">collect</span> <span m="2037310">can</span>
  <span m="2037600">have</span> <span m="2037810">some</span> <span m="2037960">sort</span>
  <span m="2038110">of</span> <span m="2038170">bias</span> <span m="2038560">within</span>
  <span m="2038860">the</span> <span m="2038950">way</span> <span m="2039250">it was</span>
  <span m="2039400">collected.</span> <span m="2040370">So</span> <span m="2040390">it</span>
  <span m="2040450">might</span> <span m="2040630">be</span> <span m="2040750">that</span>
  <span m="2040960">you</span> <span m="2041080">have</span> <span m="2041320">negative</span>
  <span m="2041650">cases</span> <span m="2042130">from</span> <span m="2043840">less</span>
  <span m="2044080">centers</span> <span m="2044560">than</span> <span m="2044650">you</span>
  <span m="2044710">have</span> <span m="2044800">positive</span> <span m="2045190">cases.</span>
  <span m="2045940">Or</span> <span m="2046090">they're</span> <span m="2046210">collected</span>
  <span m="2046480">from</span> <span m="2046630">different</span> <span m="2046840">years.</span></p><p><span
  m="2047200">And</span> <span m="2047290">actually,</span> <span m="2047530">this</span>
  <span m="2047610">is</span> <span m="2047680">something</span> <span m="2047890">we</span>
  <span m="2047950">ran</span> <span m="2048100">into</span> <span m="2048610">earlier</span>
  <span m="2048929">in</span> <span m="2049000">our</span> <span m="2049090">own</span>
  <span m="2049239">work.</span> <span m="2050199">Once</span> <span m="2050409">upon</span>
  <span m="2050620">a</span> <span m="2050679">time,</span> <span m="2051159">Connie</span>
  <span m="2051630">and I</span> <span m="2051900">were</span> <span m="2052000">in</span>
  <span m="2052120">Shanghai</span> <span m="2054460">for</span> <span m="2054610">the</span>
  <span m="2054730">opening</span> <span m="2054949">of</span> <span m="2055010">a</span>
  <span m="2055060">cancer</span> <span m="2055300">center</span> <span m="2055540">there.</span>
  <span m="2056090">And</span> <span m="2056800">at</span> <span m="2056920">that</span>
  <span m="2057070">time</span> <span m="2057310">we</span> <span m="2057400">had</span>
  <span m="2057520">all</span> <span m="2057699">the</span> <span m="2057790">cancers</span>
  <span m="2058060">from</span> <span m="2058330">the</span> <span m="2058420">MGH</span>
  <span m="2058540">dataset,</span> <span m="2059000">about</span> <span m="2059170">2,000.</span>
  <span m="2060100">But</span> <span m="2060370">the</span> <span m="2061120">mammograms</span>
  <span m="2061540">were</span> <span m="2061600">still</span> <span m="2061810">being</span>
  <span m="2061960">collected</span> <span m="2062409">annually</span> <span m="2062770">from</span>
  <span m="2062889">2012--</span> <span m="2063550">from</span> <span m="2063730">2009.</span></p><p><span
  m="2065110">So</span> <span m="2065320">at</span> <span m="2065409">that</span>
  <span m="2065530">time,</span> <span m="2065900">we</span> <span m="2066000">only</span>
  <span m="2066100">had,</span> <span m="2066280">like,</span> <span m="2066489">half</span>
  <span m="2066909">of</span> <span m="2067030">the</span> <span m="2067120">negatives</span>
  <span m="2068020">by</span> <span m="2068260">year,</span> <span m="2068960">but</span>
  <span m="2069040">all</span> <span m="2069219">of</span> <span m="2069280">the</span>
  <span m="2069370">cancers.</span> <span m="2070659">And</span> <span m="2070929">all
  of</span> <span m="2071320">a sudden</span> <span m="2071500">I had to--</span>
  <span m="2071670">you</span> <span m="2071750">know,</span> <span m="2071860">I</span>
  <span m="2072239">came from</span> <span m="2072540">the</span> <span m="2072610">slightly</span>
  <span m="2072850">more</span> <span m="2073000">complicated</span> <span m="2073449">model,</span>
  <span m="2073810">as</span> <span m="2073960">one</span> <span m="2074080">often</span>
  <span m="2074320">does.</span> <span m="2074850">I looked</span> <span m="2075080">at</span>
  <span m="2075219">several</span> <span m="2075330">images</span> <span m="2075670">at</span>
  <span m="2075760">the</span> <span m="2075820">same</span> <span m="2076000">time.</span>
  <span m="2076330">And</span> <span m="2076420">my</span> <span m="2076540">AUC</span>
  <span m="2076810">went</span> <span m="2076929">up to</span> <span m="2077050">like,</span>
  <span m="2077199">95.</span> <span m="2078320">And</span> <span m="2078429">I</span>
  <span m="2078489">had</span> <span m="2078639">all</span> <span m="2078820">this,</span>
  <span m="2079060">like,</span> <span m="2079210">bouncing</span> <span m="2079570">off</span>
  <span m="2079659">the</span> <span m="2079750">wall.</span></p><p><span m="2080560">And</span>
  <span m="2080710">then</span> <span m="2081100">in--</span> <span m="2082070">you</span>
  <span m="2082130">know,</span> <span m="2082199">I</span> <span m="2082239">had</span>
  <span m="2082360">some</span> <span m="2082480">suspicion</span> <span m="2082750">of</span>
  <span m="2082870">like,</span> <span m="2083090">wait</span> <span m="2083139">a</span>
  <span m="2083170">second.</span> <span m="2083500">This</span> <span m="2083679">is</span>
  <span m="2083770">too</span> <span m="2083920">high.</span> <span m="2084460">This</span>
  <span m="2084880">is</span> <span m="2085000">too</span> <span m="2085150">good.</span></p><p><span
  m="2086350">And</span> <span m="2086860">we</span> <span m="2087100">completely</span>
  <span m="2087449">realized</span> <span m="2087659">that</span> <span m="2088270">all</span>
  <span m="2088400">these</span> <span m="2088550">numbers</span> <span m="2088780">were</span>
  <span m="2089050">kind</span> <span m="2089170">of</span> <span m="2089260">a</span>
  <span m="2089290">myth.</span> <span m="2090159">But</span> <span m="2090429">this</span>
  <span m="2090639">level</span> <span m="2091000">of--</span> <span m="2091510">kind</span>
  <span m="2091690">of</span> <span m="2092020">if</span> <span m="2092139">you</span>
  <span m="2092230">do</span> <span m="2092380">these</span> <span m="2092530">kind</span>
  <span m="2092739">of</span> <span m="2092830">case</span> <span m="2093040">control</span>
  <span m="2093340">things,</span> <span m="2094060">you</span> <span m="2094179">can</span>
  <span m="2095110">oftentimes,</span> <span m="2096310">unless</span> <span m="2096580">you're</span>
  <span m="2096670">very</span> <span m="2096969">careful</span> <span m="2097360">about</span>
  <span m="2097540">the</span> <span m="2097600">way</span> <span m="2097860">it</span>
  <span m="2097920">was</span> <span m="2098050">constructed,</span> <span m="2098760">you</span>
  <span m="2098870">could</span> <span m="2098980">easily</span> <span m="2099220">run</span>
  <span m="2099340">into</span> <span m="2099490">these</span> <span m="2099640">issues.</span>
  <span m="2100060">And</span> <span m="2100180">your</span> <span m="2100300">testing</span>
  <span m="2100600">set</span> <span m="2100720">won't</span> <span m="2100830">protect</span>
  <span m="2101080">you</span> <span m="2101140">from</span> <span m="2101290">that.</span></p><p><span
  m="2102380">And</span> <span m="2102430">so</span> <span m="2103120">having</span>
  <span m="2103480">a</span> <span m="2103540">clean</span> <span m="2103870">dataset</span>
  <span m="2104320">that</span> <span m="2104590">truly</span> <span m="2105370">follows</span>
  <span m="2105930">the</span> <span m="2106000">kind</span> <span m="2106150">of</span>
  <span m="2107070">spectrum we</span> <span m="2107380">expect</span> <span m="2107620">to</span>
  <span m="2107680">use</span> <span m="2107800">it</span> <span m="2107890">in--</span>
  <span m="2108400">i.e.,</span> <span m="2108700">a</span> <span m="2108910">natural</span>
  <span m="2109270">distribution,</span> <span m="2110220">collected</span> <span
  m="2110480">through</span> <span m="2110620">routine</span> <span m="2110860">clinical</span>
  <span m="2111190">care</span> <span m="2111400">is</span> <span m="2111460">important</span>
  <span m="2111880">to</span> <span m="2111970">say</span> <span m="2112840">will</span>
  <span m="2112990">it</span> <span m="2113050">behave</span> <span m="2113620">as</span>
  <span m="2113770">we actually</span> <span m="2114040">want it</span> <span m="2114250">to</span>
  <span m="2114340">be</span> <span m="2114430">used.</span></p><p><span m="2116530">In</span>
  <span m="2116650">general,</span> <span m="2116990">the</span> <span m="2117070">only--</span>
  <span m="2117700">some</span> <span m="2117910">of</span> <span m="2117970">this</span>
  <span m="2118120">you</span> <span m="2118180">can</span> <span m="2118280">think</span>
  <span m="2118450">through</span> <span m="2118580">in</span> <span m="2118630">first</span>
  <span m="2118840">principle.</span> <span m="2120070">But</span> <span m="2120280">it</span>
  <span m="2120430">kind</span> <span m="2120640">of</span> <span m="2120700">stresses</span>
  <span m="2121090">the</span> <span m="2121150">importance</span> <span m="2121630">of</span>
  <span m="2122620">actually</span> <span m="2122890">testing</span> <span m="2123160">this</span>
  <span m="2123280">prospectively</span> <span m="2123820">in</span> <span m="2123910">external</span>
  <span m="2124210">validation</span> <span m="2124630">to</span> <span m="2124720">try</span>
  <span m="2124840">to</span> <span m="2124930">see</span> <span m="2125560">does</span>
  <span m="2125830">this</span> <span m="2125980">work</span> <span m="2126310">when</span>
  <span m="2126460">I</span> <span m="2126550">take</span> <span m="2126820">away</span>
  <span m="2127090">some</span> <span m="2127270">of</span> <span m="2127330">the</span>
  <span m="2127450">biases</span> <span m="2127870">in</span> <span m="2127930">my</span>
  <span m="2128020">dataset,</span> <span m="2128760">and</span> <span m="2128860">being</span>
  <span m="2129010">really</span> <span m="2129250">careful</span> <span m="2129580">about</span>
  <span m="2129790">that.</span> <span m="2130550">The</span> <span m="2130660">common</span>
  <span m="2130960">approach</span> <span m="2131270">of just</span> <span m="2131440">controlling</span>
  <span m="2131860">by</span> <span m="2132040">age</span> <span m="2132370">or</span>
  <span m="2132470">by</span> <span m="2132540">density</span> <span m="2133330">is</span>
  <span m="2133450">not</span> <span m="2133630">enough</span> <span m="2133960">when</span>
  <span m="2134110">the</span> <span m="2134170">model</span> <span m="2134380">can</span>
  <span m="2134570">catch</span> <span m="2134740">really</span> <span m="2134890">fine-grained</span>
  <span m="2135250">signals.</span></p><p><span m="2138620">How to</span> <span m="2138830">mess</span>
  <span m="2139000">up</span> <span m="2139090">in</span> <span m="2139160">modeling.</span>
  <span m="2139580">So</span> <span m="2140090">there's</span> <span m="2140300">been</span>
  <span m="2140450">adventures</span> <span m="2140810">in</span> <span m="2140900">this</span>
  <span m="2141130">space</span> <span m="2141440">as</span> <span m="2141530">well.</span>
  <span m="2142410">One</span> <span m="2142460">of</span> <span m="2142520">the</span>
  <span m="2142580">things</span> <span m="2142760">I've</span> <span m="2142880">recently</span>
  <span m="2143210">discovered</span> <span m="2143690">is</span> <span m="2143840">that</span>
  <span m="2145340">the</span> <span m="2145520">actual</span> <span m="2145820">mammography</span>
  <span m="2146330">machine</span> <span m="2146720">device</span> <span m="2147890">that</span>
  <span m="2148100">the</span> <span m="2148160">machine</span> <span m="2148400">was</span>
  <span m="2148520">captured</span> <span m="2148850">on--</span> <span m="2149120">so</span>
  <span m="2149250">you saw</span> <span m="2149330">a bunch</span> <span m="2149420">of</span>
  <span m="2149610">mammograms</span> <span m="2149865">probably</span> <span m="2150120">from</span>
  <span m="2150290">different</span> <span m="2150440">machines--</span> <span m="2151250">has</span>
  <span m="2151910">an</span> <span m="2152702">unexpected</span> <span m="2153500">impact</span>
  <span m="2153860">on</span> <span m="2153920">the</span> <span m="2153980">model.</span></p><p><span
  m="2154710">So</span> <span m="2154820">the</span> <span m="2154910">actual</span>
  <span m="2155150">probability</span> <span m="2155600">distribution--</span> <span
  m="2156790">the</span> <span m="2156890">distribution</span> <span m="2157310">of</span>
  <span m="2157400">cancer</span> <span m="2157730">probabilities</span> <span m="2158380">by</span>
  <span m="2158630">the</span> <span m="2158750">model</span> <span m="2159500">is</span>
  <span m="2159680">not</span> <span m="2160040">independent</span> <span m="2160700">of</span>
  <span m="2160820">the</span> <span m="2160910">device.</span> <span m="2161750">That's</span>
  <span m="2161860">something</span> <span m="2161970">we're</span> <span m="2162100">going</span>
  <span m="2162350">through</span> <span m="2162530">now.</span> <span m="2162740">We</span>
  <span m="2162890">actually</span> <span m="2163100">ran</span> <span m="2163270">into</span>
  <span m="2163370">this</span> <span m="2163670">while</span> <span m="2163820">working</span>
  <span m="2164270">on</span> <span m="2164427">clinical</span> <span m="2164585">implementation</span>
  <span m="2165440">is</span> <span m="2165800">like</span> <span m="2165980">this</span>
  <span m="2166130">kind</span> <span m="2166310">of</span> <span m="2166370">conditional</span>
  <span m="2166730">adversarial</span> <span m="2167390">training</span> <span m="2167720">set</span>
  <span m="2167820">up</span> <span m="2167960">to</span> <span m="2168050">try</span>
  <span m="2168170">to</span> <span m="2168260">rectify</span> <span m="2168620">this</span>
  <span m="2168740">issue.</span></p><p><span m="2170300">It's</span> <span m="2170450">important.</span>
  <span m="2171030">So</span> <span m="2171050">this</span> <span m="2171200">is</span>
  <span m="2171410">much</span> <span m="2171650">harder</span> <span m="2171920">to</span>
  <span m="2172010">catch</span> <span m="2172790">based</span> <span m="2172970">on</span>
  <span m="2173060">first</span> <span m="2173240">principle.</span> <span m="2174290">But</span>
  <span m="2174440">it's</span> <span m="2174530">important</span> <span m="2174800">to</span>
  <span m="2174890">think</span> <span m="2175070">through</span> <span m="2175490">as</span>
  <span m="2175610">you</span> <span m="2175700">kind</span> <span m="2175850">of</span>
  <span m="2176060">really</span> <span m="2176330">start</span> <span m="2177490">demoing</span>
  <span m="2178000">out</span> <span m="2178100">your</span> <span m="2178370">computations.</span>
  <span m="2179140">This</span> <span m="2179320">will</span> <span m="2179450">kind</span>
  <span m="2179600">of--</span> <span m="2179690">these</span> <span m="2179810">issues</span>
  <span m="2180080">pop</span> <span m="2180350">up</span> <span m="2180470">easily,</span>
  <span m="2180800">and they're</span> <span m="2181070">harder</span> <span m="2181310">to</span>
  <span m="2181460">avoid.</span></p><p><span m="2182990">And</span> <span m="2183140">lastly,</span>
  <span m="2183560">and</span> <span m="2183650">I</span> <span m="2183680">think</span>
  <span m="2183860">probably</span> <span m="2185420">one</span> <span m="2185600">that's</span>
  <span m="2186920">probably</span> <span m="2187310">the</span> <span m="2187430">most</span>
  <span m="2187610">important</span> <span m="2188120">is</span> <span m="2188270">messing</span>
  <span m="2188540">up</span> <span m="2188630">in</span> <span m="2188740">analysis.</span>
  <span m="2190020">So</span> <span m="2190100">it's</span> <span m="2190190">quite</span>
  <span m="2190400">common</span> <span m="2190880">in</span> <span m="2191000">the</span>
  <span m="2191390">previous</span> <span m="2192320">section</span> <span m="2192560">in</span>
  <span m="2192620">this</span> <span m="2192740">field--</span> <span m="2193310">yes.</span></p><p><span
  m="2193620">AUDIENCE:</span> <span m="2193760">With</span> <span m="2193900">the</span>
  <span m="2194041">adversarial</span> <span m="2194462">up there,</span> <span m="2195304">just</span>
  <span m="2195725">to understand</span> <span m="2196260">what</span> <span m="2196660">you</span>
  <span m="2196760">do,</span> <span m="2197060">do</span> <span m="2197300">you</span>
  <span m="2197725">that</span> <span m="2198150">discriminate</span> <span m="2198810">or</span>
  <span m="2199020">predict</span> <span m="2199300">the</span> <span m="2199580">machine?</span>
  <span m="2200320">And</span> <span m="2200480">then</span> <span m="2201860">you</span>
  <span m="2202820">train</span> <span m="2203150">against</span> <span m="2203510">that?</span></p><p><span
  m="2204020">ADAM YALA:</span> <span m="2204230">So</span> <span m="2204440">my</span>
  <span m="2204590">answer is</span> <span m="2204820">going</span> <span m="2204910">to</span>
  <span m="2205010">be</span> <span m="2205130">two</span> <span m="2205310">parts.</span>
  <span m="2205590">One,</span> <span m="2206040">it</span> <span m="2206540">doesn't</span>
  <span m="2206750">work</span> <span m="2207440">as</span> <span m="2207560">well</span>
  <span m="2207650">as</span> <span m="2207740">I</span> <span m="2207770">want it</span>
  <span m="2207950">to</span> <span m="2208040">yet.</span> <span m="2208350">So</span>
  <span m="2208430">really</span> <span m="2208670">who</span> <span m="2208790">knows?</span></p><p><span
  m="2209330">But</span> <span m="2209580">my</span> <span m="2209750">best</span>
  <span m="2209990">hunch</span> <span m="2210590">in</span> <span m="2210710">terms</span>
  <span m="2211010">of</span> <span m="2211820">what's</span> <span m="2212000">been</span>
  <span m="2212090">done</span> <span m="2212210">before</span> <span m="2212570">for</span>
  <span m="2212690">other</span> <span m="2212990">kind</span> <span m="2213230">of</span>
  <span m="2213980">work,</span> <span m="2214280">specifically in</span> <span m="2214760">radio</span>
  <span m="2215000">signals,</span> <span m="2216020">is</span> <span m="2216140">they</span>
  <span m="2216230">use</span> <span m="2216440">a</span> <span m="2216500">conditional</span>
  <span m="2216920">adversarial.</span> <span m="2217410">So</span> <span m="2217430">you're</span>
  <span m="2217520">free</span> <span m="2217790">to</span> <span m="2217850">discriminate</span>
  <span m="2217940">at both</span> <span m="2218390">the</span> <span m="2218510">label</span>
  <span m="2218960">and the</span> <span m="2219290">image</span> <span m="2219380">presentation.</span>
  <span m="2219980">You</span> <span m="2220070">have</span> <span m="2220220">to</span>
  <span m="2220280">try</span> <span m="2220400">to</span> <span m="2220490">predict</span>
  <span m="2220880">out the</span> <span m="2220940">device</span> <span m="2221690">to</span>
  <span m="2221780">try</span> <span m="2221930">to</span> <span m="2222050">take</span>
  <span m="2222290">away</span> <span m="2223130">the</span> <span m="2223250">information</span>
  <span m="2223790">that's</span> <span m="2223940">not</span> <span m="2224090">just</span>
  <span m="2224210">contained</span> <span m="2224450">within</span> <span m="2224660">the</span>
  <span m="2224720">label</span> <span m="2224960">distribution.</span></p><p><span
  m="2226250">And</span> <span m="2226280">that's</span> <span m="2226430">been</span>
  <span m="2226580">shown</span> <span m="2226790">to</span> <span m="2226880">be</span>
  <span m="2226970">very</span> <span m="2227150">helpful</span> <span m="2227540">for</span>
  <span m="2227660">people</span> <span m="2227930">trying</span> <span m="2228110">to</span>
  <span m="2228200">do</span> <span m="2229150">[INAUDIBLE]</span> <span m="2229570">detection</span>
  <span m="2230060">based</span> <span m="2230270">off</span> <span m="2230660">on</span>
  <span m="2231920">Wi-Fi--</span> <span m="2232540">or</span> <span m="2232640">not</span>
  <span m="2232790">Wi-Fi--</span> <span m="2233030">but</span> <span m="2233140">like,</span>
  <span m="2233450">radio</span> <span m="2233710">waves.</span> <span m="2234390">And</span>
  <span m="2234640">the</span> <span m="2234810">[INAUDIBLE]</span> <span m="2235250">but</span>
  <span m="2235370">also,</span> <span m="2235920">it</span> <span m="2236020">seems</span>
  <span m="2236090">to</span> <span m="2236180">be</span> <span m="2236300">the</span>
  <span m="2236540">most</span> <span m="2236690">common</span> <span m="2236960">approach</span>
  <span m="2237170">I've</span> <span m="2237260">seen</span> <span m="2237380">in</span>
  <span m="2237500">literature.</span> <span m="2238440">So</span> <span m="2238540">it's</span>
  <span m="2238640">something</span> <span m="2238820">that</span> <span m="2239000">I'm</span>
  <span m="2239090">going</span> <span m="2239210">to</span> <span m="2239300">try</span>
  <span m="2239770">soon.</span> <span m="2240120">I</span> <span m="2240160">haven't</span>
  <span m="2240350">implemented</span> <span m="2240770">it. It</span> <span m="2240850">was</span>
  <span m="2241100">just</span> <span m="2241520">GPU</span> <span m="2241880">time</span>
  <span m="2242180">and</span> <span m="2242270">kind</span> <span m="2242420">of</span>
  <span m="2242510">waiting</span> <span m="2242810">to</span> <span m="2243110">queue</span>
  <span m="2243280">up the</span> <span m="2243440">experiment.</span></p><p><span
  m="2245750">And</span> <span m="2245960">the</span> <span m="2246080">last</span>
  <span m="2246320">part</span> <span m="2248020">in</span> <span m="2248400">terms</span>
  <span m="2248530">of</span> <span m="2248590">how</span> <span m="2248670">to</span>
  <span m="2248750">mess</span> <span m="2248870">up</span> <span m="2249020">is</span>
  <span m="2249110">this</span> <span m="2249230">kind</span> <span m="2249380">of</span>
  <span m="2249470">analysis.</span> <span m="2250770">One</span> <span m="2250880">thing</span>
  <span m="2251000">that's</span> <span m="2251120">common is</span> <span m="2251420">people</span>
  <span m="2251600">assume</span> <span m="2251960">that's it</span> <span m="2252110">kind</span>
  <span m="2252290">of</span> <span m="2252380">like</span> <span m="2252530">synthetic</span>
  <span m="2252920">experiments</span> <span m="2253810">or</span> <span m="2253880">the</span>
  <span m="2253940">same</span> <span m="2254120">thing</span> <span m="2254260">as
  clinical</span> <span m="2254470">implementation.</span> <span m="2255360">Like,</span>
  <span m="2255530">people</span> <span m="2255740">do</span> <span m="2255860">reader</span>
  <span m="2256210">studies</span> <span m="2256370">very</span> <span m="2256490">often.</span>
  <span m="2257330">And</span> <span m="2257450">it's</span> <span m="2257540">quite</span>
  <span m="2257720">common</span> <span m="2258020">to</span> <span m="2258080">see</span>
  <span m="2258290">that</span> <span m="2258410">when</span> <span m="2258500">you</span>
  <span m="2258620">do</span> <span m="2258680">reader</span> <span m="2258920">studies</span>
  <span m="2259350">that it</span> <span m="2259490">doesn't</span> <span m="2259730">actually--</span>
  <span m="2260750">like,</span> <span m="2260900">you</span> <span m="2260990">might</span>
  <span m="2261140">find</span> <span m="2261380">that</span> <span m="2261470">computer</span>
  <span m="2261780">detection</span> <span m="2262160">does</span> <span m="2262280">a</span>
  <span m="2262340">huge</span> <span m="2262640">difference</span> <span m="2262940">in</span>
  <span m="2263000">reader</span> <span m="2263180">studies.</span> <span m="2264020">And</span>
  <span m="2264140">it's--</span> <span m="2264420">Connie actual</span> <span m="2264840">showed</span>
  <span m="2265010">it</span> <span m="2265070">was</span> <span m="2265190">harmful</span>
  <span m="2265550">in</span> <span m="2265610">real</span> <span m="2265760">life.</span></p><p><span
  m="2266480">And</span> <span m="2266510">it's</span> <span m="2266600">important</span>
  <span m="2266930">to</span> <span m="2267020">kind</span> <span m="2267200">of</span>
  <span m="2268400">like,</span> <span m="2268820">do</span> <span m="2269720">these</span>
  <span m="2269900">real</span> <span m="2270140">world</span> <span m="2270320">experiments</span>
  <span m="2270800">that</span> <span m="2270890">we can</span> <span m="2271040">say</span>
  <span m="2271220">what</span> <span m="2271430">is</span> <span m="2271520">happening</span>
  <span m="2271890">and</span> <span m="2272070">just</span> <span m="2272190">them</span>
  <span m="2272300">the</span> <span m="2272360">real</span> <span m="2272540">benefit</span>
  <span m="2272840">that I</span> <span m="2272930">expected.</span> <span m="2274520">And</span>
  <span m="2275270">a</span> <span m="2276050">hopefully</span> <span m="2276440">less</span>
  <span m="2276620">common</span> <span m="2276890">nowadays</span> <span m="2277880">mistake</span>
  <span m="2278270">is</span> <span m="2278390">that</span> <span m="2278840">oftentimes</span>
  <span m="2279350">people</span> <span m="2279620">exclude</span> <span m="2280190">all</span>
  <span m="2280310">inconvenient</span> <span m="2280640">cases.</span> <span m="2281510">So</span>
  <span m="2281750">there</span> <span m="2281840">was</span> <span m="2281930">a</span>
  <span m="2281990">paper</span> <span m="2282230">yesterday</span> <span m="2282800">that</span>
  <span m="2282920">just</span> <span m="2283070">came</span> <span m="2283250">out</span>
  <span m="2283760">that</span> <span m="2284090">the</span> <span m="2284240">cancer</span>
  <span m="2284540">detection</span> <span m="2285050">used</span> <span m="2285220">a</span>
  <span m="2285260">kind</span> <span m="2285410">of</span> <span m="2285500">patched-up</span>
  <span m="2285980">architecture</span> <span m="2286850">which</span> <span m="2287000">would</span>
  <span m="2287090">read</span> <span m="2287240">more</span> <span m="2287360">closely</span>
  <span m="2287660">into</span> <span m="2287900">their</span> <span m="2288020">details,</span>
  <span m="2288860">they</span> <span m="2288980">excluded</span> <span m="2289490">all</span>
  <span m="2289700">women</span> <span m="2290390">with</span> <span m="2290570">breasts</span>
  <span m="2290780">that</span> <span m="2290900">they</span> <span m="2290990">considered</span>
  <span m="2291320">too</span> <span m="2291470">small</span> <span m="2291770">by</span>
  <span m="2291890">some</span> <span m="2292010">threshold</span> <span m="2292760">for</span>
  <span m="2292970">like</span> <span m="2293120">modeling</span> <span m="2293420">convenience.</span>
  <span m="2294260">But</span> <span m="2294440">that</span> <span m="2294590">might</span>
  <span m="2294800">disproportionately</span> <span m="2295370">affect</span> <span
  m="2296840">specifically</span> <span m="2297320">Asian</span> <span m="2297560">women</span>
  <span m="2298790">in</span> <span m="2298940">that</span> <span m="2299060">population.</span>
  <span m="2299680">And</span> <span m="2299780">so</span> <span m="2300050">they</span>
  <span m="2300200">didn't</span> <span m="2300440">do</span> <span m="2300620">a</span>
  <span m="2300650">subgroup</span> <span m="2300950">analysis</span> <span m="2301790">for</span>
  <span m="2302030">all</span> <span m="2302150">the</span> <span m="2302240">different</span>
  <span m="2302450">races,</span> <span m="2302670">so</span> <span m="2302750">it's</span>
  <span m="2302840">hard</span> <span m="2302990">to</span> <span m="2303080">know</span>
  <span m="2303290">what</span> <span m="2303470">is</span> <span m="2303560">happening</span>
  <span m="2303890">there.</span></p><p><span m="2304920">If</span> <span m="2305000">your</span>
  <span m="2305090">population</span> <span m="2305600">is</span> <span m="2305690">mostly</span>
  <span m="2305960">white,</span> <span m="2306230">which</span> <span m="2306410">it</span>
  <span m="2306500">is</span> <span m="2306620">at</span> <span m="2306700">MGH,</span>
  <span m="2307090">and</span> <span m="2307220">is</span> <span m="2307340">at a</span>
  <span m="2307370">lot</span> <span m="2307670">of</span> <span m="2307730">the</span>
  <span m="2307820">centers</span> <span m="2308570">that</span> <span m="2308690">these</span>
  <span m="2308820">colleges</span> <span m="2309040">have</span> <span m="2309170">developed,</span>
  <span m="2310450">are</span> <span m="2310850">reporting</span> <span m="2311270">the</span>
  <span m="2311360">average that</span> <span m="2311750">you see</span> <span m="2312080">isn't</span>
  <span m="2312320">enough</span> <span m="2312500">to</span> <span m="2312620">really</span>
  <span m="2312830">validate</span> <span m="2313190">that.</span> <span m="2313470">And</span>
  <span m="2313570">so</span> <span m="2313670">you</span> <span m="2313770">can</span>
  <span m="2313870">have</span> <span m="2313880">things</span> <span m="2314120">like</span>
  <span m="2314230">Tyrer-Cuzick</span> <span m="2314660">model</span> <span m="2315260">that</span>
  <span m="2315410">are</span> <span m="2315470">worse</span> <span m="2315750">than</span>
  <span m="2315860">random</span> <span m="2316310">and</span> <span m="2316430">especially</span>
  <span m="2316820">harmful</span> <span m="2317450">for</span> <span m="2317540">African-American</span>
  <span m="2318050">women.</span></p><p><span m="2318680">And</span> <span m="2318770">so</span>
  <span m="2318890">guarding</span> <span m="2319150">against</span> <span m="2319400">that</span>
  <span m="2319550">is</span> <span m="2321020">you</span> <span m="2321140">can</span>
  <span m="2321260">do</span> <span m="2321440">a</span> <span m="2321500">lot</span>
  <span m="2321680">of</span> <span m="2321740">that</span> <span m="2321830">based</span>
  <span m="2321980">on</span> <span m="2322070">first</span> <span m="2322220">principle.</span>
  <span m="2323300">But</span> <span m="2323480">some</span> <span m="2323660">of</span>
  <span m="2323720">these</span> <span m="2323870">things</span> <span m="2324050">you</span>
  <span m="2324110">can</span> <span m="2324200">only</span> <span m="2324350">really</span>
  <span m="2324530">find</span> <span m="2324800">out</span> <span m="2324980">by</span>
  <span m="2325370">actively</span> <span m="2325760">monitoring</span> <span m="2326190">to</span>
  <span m="2326300">say,</span> <span m="2326540">is</span> <span m="2326660">there</span>
  <span m="2326780">any</span> <span m="2326960">subpopulation</span> <span m="2328430">that</span>
  <span m="2328580">I</span> <span m="2328640">didn't</span> <span m="2328820">think</span>
  <span m="2328940">about</span> <span m="2329290">a</span> <span m="2329420">priority</span>
  <span m="2329900">that</span> <span m="2330020">could</span> <span m="2330140">be</span>
  <span m="2330260">harmed?</span></p><p><span m="2331770">And</span> <span m="2331940">finally,</span>
  <span m="2332840">so I</span> <span m="2333000">talked</span> <span m="2333260">about</span>
  <span m="2333410">clinical</span> <span m="2333650">deployments.</span> <span m="2334160">We've</span>
  <span m="2334280">actually</span> <span m="2334490">done</span> <span m="2334610">this</span>
  <span m="2334760">a</span> <span m="2334820">couple</span> <span m="2335030">times.</span>
  <span m="2335830">And</span> <span m="2335960">I'm</span> <span m="2336020">going</span>
  <span m="2336130">to</span> <span m="2336210">switch</span> <span m="2336440">over</span>
  <span m="2336590">to</span> <span m="2336650">Connie</span> <span m="2336920">real</span>
  <span m="2337040">soon.</span></p><p><span m="2339110">In</span> <span m="2339260">general,</span>
  <span m="2340490">what</span> <span m="2340910">you</span> <span m="2341060">want</span>
  <span m="2341240">to</span> <span m="2341300">do</span> <span m="2341420">is</span>
  <span m="2341480">you</span> <span m="2341570">want</span> <span m="2341690">to</span>
  <span m="2341750">make</span> <span m="2341840">it</span> <span m="2341960">as</span>
  <span m="2342470">easy</span> <span m="2342920">as</span> <span m="2343220">plausible</span>
  <span m="2343940">and</span> <span m="2344060">possible</span> <span m="2344540">for</span>
  <span m="2344660">the</span> <span m="2345920">in-house</span> <span m="2346640">IT</span>
  <span m="2347040">team</span> <span m="2347390">to</span> <span m="2347540">use</span>
  <span m="2347750">your</span> <span m="2347840">tool.</span> <span m="2348980">We've</span>
  <span m="2349160">gone</span> <span m="2349340">through</span> <span m="2349520">this</span>
  <span m="2349730">with--</span> <span m="2351070">not</span> <span m="2351290">like--</span>
  <span m="2352040">I</span> <span m="2352100">don't--</span> <span m="2352220">depends</span>
  <span m="2352340">on</span> <span m="2352400">how</span> <span m="2352520">you</span>
  <span m="2352640">count.</span> <span m="2352990">It's like</span> <span m="2353150">once</span>
  <span m="2353330">for</span> <span m="2353410">density</span> <span m="2353840">and</span>
  <span m="2353930">then</span> <span m="2354000">like</span> <span m="2354110">three</span>
  <span m="2354290">times</span> <span m="2354470">at</span> <span m="2354530">the</span>
  <span m="2354590">same</span> <span m="2354800">time.</span> <span m="2355360">But</span>
  <span m="2355490">I</span> <span m="2355550">spent,</span> <span m="2355730">like,</span>
  <span m="2355880">many</span> <span m="2356150">hours</span> <span m="2356420">sitting</span>
  <span m="2356660">there.</span></p><p><span m="2357950">And</span> <span m="2358190">the</span>
  <span m="2358280">broad</span> <span m="2359560">way</span> <span m="2359780">that</span>
  <span m="2359900">we</span> <span m="2359960">set</span> <span m="2360140">it</span>
  <span m="2360230">up</span> <span m="2360320">so</span> <span m="2360470">far</span>
  <span m="2360830">is</span> <span m="2360980">we</span> <span m="2361070">just</span>
  <span m="2361190">have</span> <span m="2361400">a</span> <span m="2362000">kind</span>
  <span m="2362210">of</span> <span m="2362720">docker</span> <span m="2363050">as</span>
  <span m="2363380">container</span> <span m="2364340">to</span> <span m="2364580">manage</span>
  <span m="2364970">a</span> <span m="2365030">web</span> <span m="2365240">app</span>
  <span m="2365470">that holds</span> <span m="2365620">the</span> <span m="2365820">model.</span>
  <span m="2366860">This</span> <span m="2367040">web</span> <span m="2367250">app</span>
  <span m="2367400">has</span> <span m="2367610">kind</span> <span m="2367730">of</span>
  <span m="2367790">a</span> <span m="2367850">backup</span> <span m="2368105">processing</span>
  <span m="2368450">toolkit.</span> <span m="2369140">So</span> <span m="2369260">the</span>
  <span m="2369320">kind</span> <span m="2369470">of</span> <span m="2369530">steps</span>
  <span m="2369920">that</span> <span m="2370310">all</span> <span m="2370490">of</span>
  <span m="2370550">our</span> <span m="2370610">deployments</span> <span m="2370970">follow</span>
  <span m="2371630">and</span> <span m="2371720">I</span> <span m="2371780">look</span>
  <span m="2372020">under</span> <span m="2372210">unified</span> <span m="2372590">framework</span>
  <span m="2373370">is</span> <span m="2373520">the</span> <span m="2373610">IT</span>
  <span m="2373790">application</span> <span m="2374330">would</span> <span m="2374480">get</span>
  <span m="2374660">some</span> <span m="2374780">images</span> <span m="2375080">out</span>
  <span m="2375200">of</span> <span m="2375260">the</span> <span m="2375320">PAC</span>
  <span m="2375560">system.</span> <span m="2376850">It</span> <span m="2376970">will</span>
  <span m="2377060">send it</span> <span m="2377420">over to</span> <span m="2377570">application.</span>
  <span m="2378260">We're</span> <span m="2378380">going</span> <span m="2378500">to</span>
  <span m="2378560">convert</span> <span m="2378860">to</span> <span m="2378980">the</span>
  <span m="2379100">PNG</span> <span m="2379480">in</span> <span m="2379560">the</span>
  <span m="2379640">way</span> <span m="2379760">that</span> <span m="2379850">we</span>
  <span m="2379970">expect,</span> <span m="2380390">because</span> <span m="2380570">we</span>
  <span m="2380660">kind</span> <span m="2380840">of</span> <span m="2382130">encapsulate</span>
  <span m="2382670">this</span> <span m="2382750">functionality.</span> <span m="2383410">Run</span>
  <span m="2383600">for</span> <span m="2383690">the</span> <span m="2383780">models,</span>
  <span m="2384110">send it</span> <span m="2384250">back,</span> <span m="2384530">and</span>
  <span m="2384620">then</span> <span m="2384700">write</span> <span m="2384850">it</span>
  <span m="2384910">back</span> <span m="2385070">to</span> <span m="2385160">the</span>
  <span m="2385260">EHR.</span></p><p><span m="2386270">One</span> <span m="2386420">of</span>
  <span m="2386480">the</span> <span m="2386540">things</span> <span m="2386720">I</span>
  <span m="2386810">ran</span> <span m="2386990">into</span> <span m="2387260">was</span>
  <span m="2387410">that</span> <span m="2388480">they</span> <span m="2388530">didn't</span>
  <span m="2388760">actually</span> <span m="2389000">know</span> <span m="2389120">how</span>
  <span m="2389210">to</span> <span m="2389300">use</span> <span m="2389510">things</span>
  <span m="2389660">like</span> <span m="2389810">HTTP</span> <span m="2390950">because</span>
  <span m="2391220">it's</span> <span m="2391310">not</span> <span m="2391490">actually</span>
  <span m="2391760">normal</span> <span m="2392180">within</span> <span m="2392480">their</span>
  <span m="2392600">infrastructure.</span> <span m="2393930">And</span> <span m="2393980">so</span>
  <span m="2394130">being</span> <span m="2394340">cognizant</span> <span m="2394810">that</span>
  <span m="2395060">some</span> <span m="2395300">of</span> <span m="2395360">these</span>
  <span m="2396200">more,</span> <span m="2396410">like,</span> <span m="2396620">tech</span>
  <span m="2396890">standard</span> <span m="2397730">things</span> <span m="2398130">like</span>
  <span m="2398260">just</span> <span m="2398480">HTTP</span> <span m="2398810">requests</span>
  <span m="2399230">and</span> <span m="2399500">responses</span> <span m="2399920">and</span>
  <span m="2400010">stuff</span> <span m="2401240">is</span> <span m="2401450">less</span>
  <span m="2401690">standard</span> <span m="2402020">within</span> <span m="2402770">the</span>
  <span m="2402950">inside</span> <span m="2404390">of</span> <span m="2404510">their</span>
  <span m="2404810">infrastructure</span> <span m="2405620">and</span> <span m="2405890">kind</span>
  <span m="2406040">of</span> <span m="2406100">looking</span> <span m="2406340">up</span>
  <span m="2406460">how</span> <span m="2406580">to</span> <span m="2406640">actually</span>
  <span m="2406850">do</span> <span m="2406970">these</span> <span m="2407090">things</span>
  <span m="2407330">in</span> <span m="2407420">like</span> <span m="2407530">C</span>
  <span m="2407700">Sharp, or</span> <span m="2407960">whatever</span> <span m="2408140">language</span>
  <span m="2408410">they</span> <span m="2408500">have,</span> <span m="2409130">has</span>
  <span m="2409310">been</span> <span m="2409460">really</span> <span m="2409700">what's</span>
  <span m="2409850">enabled</span> <span m="2410180">us</span> <span m="2410300">to</span>
  <span m="2410660">end</span> <span m="2410810">block</span> <span m="2411110">these</span>
  <span m="2411260">things</span> <span m="2411470">and</span> <span m="2411560">actually</span>
  <span m="2411770">plug</span> <span m="2411980">it</span> <span m="2412040">in.</span></p><p><span
  m="2413450">And</span> <span m="2413780">that</span> <span m="2413990">is</span>
  <span m="2414230">it</span> <span m="2414410">for</span> <span m="2414550">my</span>
  <span m="2414680">part.</span> <span m="2414950">So I'm</span> <span m="2415130">gonna</span>
  <span m="2415220">hand it</span> <span m="2415400">back--</span> <span m="2415620">oh,</span>
  <span m="2415920">yes.</span></p><p><span m="2416160">AUDIENCE:</span> <span m="2416350">So</span>
  <span m="2416540">you're</span> <span m="2416890">writing</span> <span m="2417150">stuff</span>
  <span m="2417580">in</span> <span m="2417700">the</span> <span m="2417840">IT</span>
  <span m="2418220">application</span> <span m="2419220">in</span> <span m="2419330">C</span>
  <span m="2419685">Sharp</span> <span m="2420040">to</span> <span m="2420320">do</span>
  <span m="2420680">API</span> <span m="2420980">requests?</span></p><p><span m="2421970">ADAM
  YALA:</span> <span m="2422105">So</span> <span m="2422510">they're</span> <span
  m="2422750">writing</span> <span m="2423080">it.</span> <span m="2424030">I</span>
  <span m="2424160">just</span> <span m="2424330">meet</span> <span m="2424490">them</span>
  <span m="2424610">to</span> <span m="2424700">tell</span> <span m="2424850">them</span>
  <span m="2424970">how</span> <span m="2425060">to</span> <span m="2425150">write</span>
  <span m="2425330">it.</span> <span m="2425900">But</span> <span m="2426380">yes.</span></p><p><span
  m="2428070">So</span> <span m="2428250">like,</span> <span m="2428790">in</span>
  <span m="2429060">general,</span> <span m="2429390">like,</span> <span m="2429840">there's</span>
  <span m="2429990">libraries.</span> <span m="2430610">So</span> <span m="2430770">like,</span>
  <span m="2431430">the</span> <span m="2431520">entire</span> <span m="2431790">environment</span>
  <span m="2432120">is in</span> <span m="2432300">Windows.</span> <span m="2433200">And</span>
  <span m="2433350">Windows</span> <span m="2433620">has</span> <span m="2433690">a</span>
  <span m="2433710">very</span> <span m="2433860">poor</span> <span m="2434070">support</span>
  <span m="2434670">for</span> <span m="2434820">lots</span> <span m="2435030">of</span>
  <span m="2435120">things</span> <span m="2435310">you</span> <span m="2435350">would</span>
  <span m="2435450">expect</span> <span m="2435790">it</span> <span m="2435870">to</span>
  <span m="2435990">have</span> <span m="2436140">a</span> <span m="2436170">good</span>
  <span m="2436290">support</span> <span m="2436560">for.</span> <span m="2437130">So</span>
  <span m="2437370">there</span> <span m="2437550">was</span> <span m="2437670">like,</span>
  <span m="2438240">if</span> <span m="2438360">you</span> <span m="2438450">wanted</span>
  <span m="2438630">to</span> <span m="2438720">send</span> <span m="2438930">HP</span>
  <span m="2439200">requests</span> <span m="2439530">for</span> <span m="2439620">like</span>
  <span m="2439740">a</span> <span m="2440100">multipart</span> <span m="2440520">form</span>
  <span m="2441660">and</span> <span m="2441780">just</span> <span m="2441930">put</span>
  <span m="2442190">the</span> <span m="2442230">images</span> <span m="2442560">in</span>
  <span m="2442650">that</span> <span m="2442800">form,</span> <span m="2443430">apparently</span>
  <span m="2444000">that</span> <span m="2444360">has</span> <span m="2444510">bugs</span>
  <span m="2444810">in</span> <span m="2444930">it</span> <span m="2445050">in</span>
  <span m="2445200">like,</span> <span m="2445350">Windows</span> <span m="2446460">whatever</span>
  <span m="2447000">version</span> <span m="2447240">they</span> <span m="2447330">use</span>
  <span m="2447480">today.</span></p><p><span m="2448620">And</span> <span m="2448770">so</span>
  <span m="2449070">that</span> <span m="2449310">vanilla</span> <span m="2449670">version</span>
  <span m="2449970">didn't</span> <span m="2450180">work.</span> <span m="2450450">Windows</span>
  <span m="2450600">for</span> <span m="2450750">Docker</span> <span m="2451230">also</span>
  <span m="2451470">has</span> <span m="2451620">bugs.</span> <span m="2452370">And</span>
  <span m="2452490">I</span> <span m="2452580">had to</span> <span m="2452760">set</span>
  <span m="2453000">up</span> <span m="2453120">this</span> <span m="2453240">kind</span>
  <span m="2453360">of</span> <span m="2453450">locking</span> <span m="2453720">function</span>
  <span m="2454530">for</span> <span m="2454680">them</span> <span m="2454830">to</span>
  <span m="2454950">like,</span> <span m="2455270">automatically</span> <span m="2455730">table</span>
  <span m="2456040">locks</span> <span m="2456360">inside</span> <span m="2456630">the</span>
  <span m="2456720">container.</span> <span m="2457530">And</span> <span m="2457620">it</span>
  <span m="2457700">just</span> <span m="2457830">doesn't</span> <span m="2458220">work</span>
  <span m="2458590">in</span> <span m="2458690">Windows</span> <span m="2458820">for</span>
  <span m="2458900">Docker.</span></p><p><span m="2459070">AUDIENCE:</span> <span
  m="2459125">[INAUDIBLE]</span> <span m="2459180">questions</span> <span m="2459566">because</span>
  <span m="2459952">he is short on</span> <span m="2460340">time.</span></p><p><span
  m="2460940">ADAM YALA:</span> <span m="2461015">Yeah.</span> <span m="2461810">So</span>
  <span m="2462330">we</span> <span m="2462420">can</span> <span m="2462510">get</span>
  <span m="2462600">to</span> <span m="2462690">this</span> <span m="2462810">at</span>
  <span m="2462870">the</span> <span m="2462960">end.</span> <span m="2463110">I</span>
  <span m="2463170">want</span> <span m="2463290">to</span> <span m="2463380">hand</span>
  <span m="2463560">off</span> <span m="2463650">to</span> <span m="2463740">Connie.</span>
  <span m="2464700">If</span> <span m="2464820">you</span> <span m="2464880">have</span>
  <span m="2464970">any</span> <span m="2465090">questions,</span> <span m="2465790">grab</span>
  <span m="2466020">me</span> <span m="2466320">after.</span></p><p>&nbsp;</p>
type: course
uid: b6cd8c0c9d7e8c0a1a9e7a4f799cd127

---
None