---
about_this_resource_text: '<p>Prof. Sontag continues with the topic of risk stratification.
  He discusses the derivation of labels for data, evaluation of model performance,
  and the subtleties with machine learning-based risk stratification. The lecture
  finishes with survival modeling.</p> <p>Speaker: David Sontag</p>             <p><a
  href="./resolveuid/476c3cdeaf64631d2fb0332832ff6250">Lecture 5: Risk Stratification,
  Part 2 slides (PDF - 2.2MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: wqI_z1yumzY
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: Video-YouTube-Stream
  type: Video
  uid: 31e10787c8a477e7e3917bd314ebf163
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/wqI_z1yumzY/default.jpg
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 1e1d0fed76fc34aedb0ab8a4190f8496
- id: 3Play-3PlayYouTubeid-MP4
  media_location: wqI_z1yumzY
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: fa2da0696fa60b7ecdfc7d09437023a6
- id: wqI_z1yumzY.srt
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-5-risk-stratification-part-2/wqI_z1yumzY.srt
  title: 3play caption file
  type: null
  uid: 673dac5ea865fb380176d5d80f9e6852
- id: wqI_z1yumzY.pdf
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-5-risk-stratification-part-2/wqI_z1yumzY.pdf
  title: 3play pdf file
  type: null
  uid: 30da27b0e0ec8388dc8d715904e43d85
- id: Caption-3Play YouTube id-SRT
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 94cda293dfccb23f107dbd231989c9af
- id: Transcript-3Play YouTube id-PDF
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 7fb0fef8512e43d27d608b0e29c9079b
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec05_300k.mp4
  parent_uid: b923017e9d4756e7bd74deb4ab63c6fa
  title: Video-Internet Archive-MP4
  type: Video
  uid: 2dbce1b1d751c5af7ab14c8aab16d1b9
inline_embed_id: 69271808lecture5riskstratificationpart246571317
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-5-risk-stratification-part-2
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-5-risk-stratification-part-2
template_type: Tabbed
title: 'Lecture 5: Risk Stratification, Part 2'
transcript: <p><span m="1461">[CLICK]</span></p><p><span m="2435">[SQUEAK]</span></p><p><span
  m="3409">[PAGES RUSTLING]</span></p><p><span m="4383">[MOUSE DOUBLE-CLICKS]</span></p><p><span
  m="15590">PROFESSOR:</span> <span m="15665">So</span> <span m="15740">today</span>
  <span m="16030">we'll be</span> <span m="16180">continuing</span> <span m="16610">along</span>
  <span m="16820">the</span> <span m="16910">theme</span> <span m="17150">of</span>
  <span m="17240">risk</span> <span m="17360">stratification.</span> <span m="18320">I'll</span>
  <span m="18440">spend</span> <span m="18980">the</span> <span m="19250">first</span>
  <span m="19700">half</span> <span m="20060">to</span> <span m="20180">2/3</span>
  <span m="20600">of</span> <span m="20720">today's</span> <span m="21020">lecture</span>
  <span m="22430">continuing</span> <span m="22910">where</span> <span m="23000">we</span>
  <span m="23120">left</span> <span m="23390">off</span> <span m="23600">last</span>
  <span m="23960">week</span> <span m="25010">before</span> <span m="25310">the</span>
  <span m="25430">discussion.</span> <span m="27230">I'll</span> <span m="27290">talk</span>
  <span m="27470">about</span> <span m="27620">how</span> <span m="28220">does</span>
  <span m="28340">one</span> <span m="28550">derive</span> <span m="28940">the</span>
  <span m="29060">labels</span> <span m="29570">that</span> <span m="29690">one</span>
  <span m="29870">uses</span> <span m="30200">within</span> <span m="30440">a</span>
  <span m="30500">supervised</span> <span m="30920">machine</span> <span m="31160">learning</span>
  <span m="31370">approach.</span> <span m="32270">I'll</span> <span m="32360">continue</span>
  <span m="32750">talking</span> <span m="33080">about</span> <span m="33530">how</span>
  <span m="33710">one</span> <span m="33890">evaluates</span> <span m="34610">risk</span>
  <span m="34790">stratification</span> <span m="35300">models.</span> <span m="36440">And</span>
  <span m="36560">then</span> <span m="36650">I'll</span> <span m="36710">talk</span>
  <span m="36890">about</span> <span m="37040">some</span> <span m="37160">of</span>
  <span m="37220">the</span> <span m="37310">subtleties</span> <span m="38270">that</span>
  <span m="38420">arise</span> <span m="38900">when</span> <span m="39050">you</span>
  <span m="39110">want</span> <span m="39260">to</span> <span m="39350">use</span>
  <span m="39500">machine</span> <span m="39770">learning</span> <span m="39980">for</span>
  <span m="40070">health</span> <span m="40380">care,</span> <span m="40520">specifically</span>
  <span m="41000">for</span> <span m="41150">risk</span> <span m="41330">stratification.</span>
  <span m="42530">And</span> <span m="42620">I</span> <span m="42680">think</span>
  <span m="42800">that's</span> <span m="42950">going</span> <span m="43130">to</span>
  <span m="43220">be</span> <span m="43310">one</span> <span m="43400">of</span> <span
  m="43460">the</span> <span m="43520">most</span> <span m="43670">interesting</span>
  <span m="44030">parts</span> <span m="44240">of</span> <span m="44300">today's</span>
  <span m="44570">lecture.</span> <span m="46070">In</span> <span m="46160">the</span>
  <span m="46220">last</span> <span m="46490">third</span> <span m="46760">of</span>
  <span m="46850">today's</span> <span m="47120">lecture,</span> <span m="47630">I'll</span>
  <span m="47720">be</span> <span m="47840">talking</span> <span m="48200">about</span>
  <span m="49400">how</span> <span m="49760">one</span> <span m="50030">can</span>
  <span m="50210">rethink</span> <span m="51040">the</span> <span m="51170">supervised</span>
  <span m="51690">machine</span> <span m="51920">learning</span> <span m="52130">problem,</span>
  <span m="52820">not</span> <span m="53120">to</span> <span m="53240">be</span> <span
  m="53360">a</span> <span m="53420">classification</span> <span m="54290">problem,</span>
  <span m="54750">but</span> <span m="54770">be</span> <span m="54890">something</span>
  <span m="55190">closer</span> <span m="55610">to</span> <span m="55760">a</span>
  <span m="55790">regression</span> <span m="56390">problem.</span></p><p><span m="57320">And</span>
  <span m="57740">one</span> <span m="58250">now</span> <span m="58550">thinks</span>
  <span m="58910">about</span> <span m="59180">not</span> <span m="59630">will</span>
  <span m="59840">someone,</span> <span m="60230">for</span> <span m="60350">example,</span>
  <span m="60900">develop</span> <span m="61130">diabetes</span> <span m="61640">within</span>
  <span m="62240">one</span> <span m="62510">to</span> <span m="62630">three</span>
  <span m="62840">years</span> <span m="63020">from</span> <span m="63130">now,</span>
  <span m="63420">but</span> <span m="63560">when</span> <span m="64129">precisely</span>
  <span m="65060">will</span> <span m="65150">they</span> <span m="65239">develop</span>
  <span m="65519">diabetes--</span> <span m="66340">so the</span> <span m="66530">time</span>
  <span m="67010">to</span> <span m="67250">event.</span> <span m="68750">Then</span>
  <span m="69080">one</span> <span m="69200">has</span> <span m="69350">to</span>
  <span m="69410">start</span> <span m="69590">to</span> <span m="69680">really</span>
  <span m="69890">think</span> <span m="70310">very</span> <span m="70730">carefully</span>
  <span m="71300">about</span> <span m="71450">the</span> <span m="71540">censoring</span>
  <span m="72230">issues</span> <span m="72650">that</span> <span m="72770">I</span>
  <span m="72950">alluded</span> <span m="73370">to</span> <span m="73550">last</span>
  <span m="73880">week.</span> <span m="74660">And</span> <span m="74780">so</span>
  <span m="75050">I'll</span> <span m="75200">formalize</span> <span m="75860">those</span>
  <span m="76040">notions</span> <span m="76490">in</span> <span m="76580">the</span>
  <span m="76640">language</span> <span m="77000">of</span> <span m="77060">survival</span>
  <span m="77600">modeling.</span> <span m="78590">And</span> <span m="78680">I'll</span>
  <span m="78770">talk</span> <span m="79010">about</span> <span m="79190">how</span>
  <span m="79370">one</span> <span m="79580">can</span> <span m="79700">do</span>
  <span m="79790">maximum</span> <span m="80120">likelihood</span> <span m="80510">estimation</span>
  <span m="80990">in that</span> <span m="81140">setting,</span> <span m="81770">and</span>
  <span m="81890">how</span> <span m="82010">one</span> <span m="82160">should</span>
  <span m="82280">do</span> <span m="82400">evaluation</span> <span m="82960">in</span>
  <span m="83030">that</span> <span m="83150">setting.</span></p><p><span m="86780">So</span>
  <span m="87560">in</span> <span m="87770">our</span> <span m="87860">lecture</span>
  <span m="88430">last</span> <span m="88790">week,</span> <span m="89250">I</span>
  <span m="89270">gave</span> <span m="89510">you</span> <span m="89570">this</span>
  <span m="89750">example</span> <span m="90380">of</span> <span m="90560">risk</span>
  <span m="90800">stratification</span> <span m="91400">for</span> <span m="91490">type</span>
  <span m="91700">2</span> <span m="91820">diabetes.</span> <span m="92990">The</span>
  <span m="93080">goal,</span> <span m="93500">just</span> <span m="93650">to</span>
  <span m="93710">remind</span> <span m="94130">you,</span> <span m="94280">was</span>
  <span m="94490">as</span> <span m="94580">follows.</span> <span m="95660">25%</span>
  <span m="96440">of</span> <span m="96500">people</span> <span m="96860">in</span>
  <span m="96950">the</span> <span m="97010">United</span> <span m="97250">States</span>
  <span m="98000">have</span> <span m="98390">undiagnosed</span> <span m="99350">type</span>
  <span m="99590">2</span> <span m="99710">diabetes.</span> <span m="100970">If</span>
  <span m="101140">we</span> <span m="101220">could</span> <span m="101360">take</span>
  <span m="102500">health</span> <span m="102770">insurance</span> <span m="103340">claims</span>
  <span m="103850">data</span> <span m="104270">that's</span> <span m="104480">available</span>
  <span m="105140">for</span> <span m="105410">everyone</span> <span m="105950">who</span>
  <span m="106040">has</span> <span m="106190">health</span> <span m="106400">insurance,</span>
  <span m="107660">and</span> <span m="107810">use</span> <span m="108170">that</span>
  <span m="108530">to</span> <span m="108680">predict</span> <span m="109370">who,</span>
  <span m="110030">in</span> <span m="110180">the</span> <span m="110310">near-term--</span>
  <span m="111110">next</span> <span m="111380">one</span> <span m="111680">to</span>
  <span m="111800">three</span> <span m="112040">years--</span> <span m="112460">is</span>
  <span m="112610">likely</span> <span m="113060">to</span> <span m="113420">be</span>
  <span m="113570">newly</span> <span m="114110">diagnosed</span> <span m="114830">with</span>
  <span m="115010">type</span> <span m="115190">2</span> <span m="115310">diabetes,</span>
  <span m="116360">then</span> <span m="116510">we</span> <span m="116620">could</span>
  <span m="116750">use</span> <span m="116960">it</span> <span m="117050">to</span>
  <span m="117200">risk-stratify</span> <span m="118640">patient</span> <span m="118910">population.</span>
  <span m="119540">We</span> <span m="119660">could</span> <span m="119780">use</span>
  <span m="119930">that,</span> <span m="120110">then,</span> <span m="120260">to</span>
  <span m="120350">figure</span> <span m="120530">out</span> <span m="120640">who</span>
  <span m="120720">is</span> <span m="120830">most</span> <span m="121100">at</span>
  <span m="121160">risk,</span> <span m="122030">do</span> <span m="122180">interventions</span>
  <span m="122840">for</span> <span m="122960">those</span> <span m="123140">patients,</span>
  <span m="123620">to</span> <span m="123740">try</span> <span m="123890">to</span>
  <span m="124340">get</span> <span m="124550">them</span> <span m="124730">diagnosed</span>
  <span m="125330">and</span> <span m="125420">get</span> <span m="125570">them</span>
  <span m="125930">started</span> <span m="126260">on</span> <span m="126380">treatment</span>
  <span m="126770">if</span> <span m="126890">relevant.</span></p><p><span m="129080">But</span>
  <span m="129259">what</span> <span m="129410">I</span> <span m="129500">didn't</span>
  <span m="129919">talk</span> <span m="130160">much</span> <span m="130370">about</span>
  <span m="130669">was</span> <span m="131210">where</span> <span m="131540">did</span>
  <span m="131720">those</span> <span m="131930">labels</span> <span m="132290">come</span>
  <span m="132530">from.</span> <span m="133380">How</span> <span m="133550">do</span>
  <span m="133670">we</span> <span m="133820">know</span> <span m="135020">that</span>
  <span m="135260">someone</span> <span m="135620">had</span> <span m="135830">a</span>
  <span m="135890">diabetes</span> <span m="136550">onset</span> <span m="137650">in</span>
  <span m="137780">that</span> <span m="137960">window</span> <span m="138320">that</span>
  <span m="138440">I</span> <span m="138530">show</span> <span m="138800">up</span>
  <span m="138920">there</span> <span m="139100">on</span> <span m="139190">the</span>
  <span m="139250">top?</span> <span m="142520">So</span> <span m="143270">what</span>
  <span m="143420">are the</span> <span m="143540">answers?</span> <span m="143870">I</span>
  <span m="143960">mean,</span> <span m="144130">all of you</span> <span m="144230">should</span>
  <span m="144380">have</span> <span m="144470">read</span> <span m="144830">the</span>
  <span m="145580">paper</span> <span m="145850">by</span> <span m="146000">Razavian.</span>
  <span m="146490">And then</span> <span m="146630">also</span> <span m="147110">you</span>
  <span m="147800">should</span> <span m="147950">hopefully</span> <span m="148280">have</span>
  <span m="148400">some</span> <span m="148580">ideas.</span> <span m="149670">Thoughts?</span>
  <span m="151630">A</span> <span m="152040">hint--</span> <span m="152440">it was
  in</span> <span m="152540">supplementary</span> <span m="152990">material.</span></p><p><span
  m="157630">How</span> <span m="157810">did</span> <span m="157930">we</span> <span
  m="158050">define</span> <span m="159370">a</span> <span m="159430">positive</span>
  <span m="160030">case</span> <span m="160660">in</span> <span m="160750">that</span>
  <span m="160900">paper?</span> <span m="168120">Yep.</span></p><p><span m="168713">AUDIENCE:</span>
  <span m="168813">Drugs</span> <span m="168913">they</span> <span m="169013">were</span>
  <span m="169116">on.</span></p><p><span m="169520">PROFESSOR:</span> <span m="169620">Drugs</span>
  <span m="169720">they</span> <span m="169820">were</span> <span m="170150">on.</span>
  <span m="170750">OK,</span> <span m="171020">yeah,</span> <span m="171240">so</span>
  <span m="172350">for</span> <span m="172500">example,</span> <span m="173460">metformin,</span>
  <span m="174510">glucose--</span> <span m="175860">sorry,</span> <span m="176100">insulin.</span></p><p><span
  m="176975">AUDIENCE:</span> <span m="177088">I</span> <span m="177201">think</span>
  <span m="177314">they</span> <span m="177430">did include</span> <span m="177885">metformin</span>
  <span m="178340">actually.</span></p><p><span m="180620">PROFESSOR:</span> <span
  m="180757">Metformin</span> <span m="181170">is</span> <span m="181270">a</span>
  <span m="181320">tricky</span> <span m="181650">case.</span> <span m="182550">Because</span>
  <span m="182790">metformin</span> <span m="183180">is</span> <span m="183300">often</span>
  <span m="183660">used</span> <span m="184590">for</span> <span m="185730">alternative</span>
  <span m="186270">indications.</span> <span m="187320">But</span> <span m="187500">there</span>
  <span m="187590">are</span> <span m="187740">many</span> <span m="188010">medications,</span>
  <span m="189420">such</span> <span m="189630">as</span> <span m="189720">insulin,</span>
  <span m="190570">which</span> <span m="190650">are</span> <span m="190770">used</span>
  <span m="191640">pretty</span> <span m="191880">exclusively</span> <span m="192600">for</span>
  <span m="192900">treating</span> <span m="193230">diabetes.</span> <span m="193950">And</span>
  <span m="194070">so</span> <span m="194160">you</span> <span m="194250">can</span>
  <span m="194340">look</span> <span m="194490">to</span> <span m="194580">see,</span>
  <span m="195610">does</span> <span m="195630">a</span> <span m="195720">patient</span>
  <span m="196920">have</span> <span m="197790">a</span> <span m="197880">record</span>
  <span m="198630">of</span> <span m="198840">taking</span> <span m="199260">one</span>
  <span m="199440">of</span> <span m="199500">these</span> <span m="199650">diabetic</span>
  <span m="200070">medications</span> <span m="201030">in</span> <span m="201300">that</span>
  <span m="201750">window</span> <span m="202380">that</span> <span m="202530">we're</span>
  <span m="202650">using</span> <span m="203160">to</span> <span m="203280">define</span>
  <span m="203760">the</span> <span m="203910">outcome?</span> <span m="205590">If</span>
  <span m="205710">you</span> <span m="205830">see</span> <span m="206100">a</span>
  <span m="206160">record</span> <span m="206640">of</span> <span m="206760">a</span>
  <span m="206790">medication,</span> <span m="207480">you</span> <span m="207540">might</span>
  <span m="208200">conjecture,</span> <span m="209100">this</span> <span m="209250">patient</span>
  <span m="209520">probably</span> <span m="209850">has</span> <span m="210090">diabetes.</span></p><p><span
  m="211680">But</span> <span m="211770">what</span> <span m="211860">about</span>
  <span m="212010">it</span> <span m="212100">they</span> <span m="212220">don't</span>
  <span m="212670">have</span> <span m="212880">any</span> <span m="213030">medication</span>
  <span m="213810">listed</span> <span m="214170">in</span> <span m="214230">that</span>
  <span m="214350">time</span> <span m="214620">window?</span> <span m="215610">What</span>
  <span m="215730">could</span> <span m="215880">you</span> <span m="216330">conclude</span>
  <span m="216810">then?</span> <span m="217470">Any</span> <span m="217620">ideas?</span>
  <span m="218730">Yeah.</span></p><p><span m="219220">AUDIENCE:</span> <span m="219385">If</span>
  <span m="219550">you look</span> <span m="219750">at</span> <span m="220235">the</span>
  <span m="221205">HBA1C</span> <span m="221690">value,</span> <span m="222660">and
  you</span> <span m="223145">know the</span> <span m="223630">normal range,</span>
  <span m="224115">and</span> <span m="225570">if you</span> <span m="226055">see</span>
  <span m="226540">the</span> <span m="227025">[INAUDIBLE]</span> <span m="227510">above</span>
  <span m="227995">like</span> <span m="228480">7.5</span> <span m="228965">or</span>
  <span m="229450">7.</span></p><p><span m="229950">PROFESSOR:</span> <span m="230025">So</span>
  <span m="230100">you're</span> <span m="230220">giving</span> <span m="230490">me</span>
  <span m="230550">an</span> <span m="230640">alternative</span> <span m="231270">approach,</span>
  <span m="232260">not</span> <span m="232560">looking</span> <span m="232800">at</span>
  <span m="232860">medications,</span> <span m="233370">but</span> <span m="233460">looking</span>
  <span m="233670">at</span> <span m="233760">laboratory</span> <span m="234270">test</span>
  <span m="234540">results.</span> <span m="235020">Look</span> <span m="235200">at</span>
  <span m="235320">their</span> <span m="235870">HBA1C</span> <span m="236910">results,</span>
  <span m="237870">which</span> <span m="238080">measures</span> <span m="239730">approximately</span>
  <span m="240600">an</span> <span m="240720">average</span> <span m="241140">of</span>
  <span m="241230">three-month</span> <span m="241650">glucose</span> <span m="242070">values.</span>
  <span m="243120">And</span> <span m="243240">if</span> <span m="243330">that's</span>
  <span m="243510">out</span> <span m="243720">of</span> <span m="243840">range,</span>
  <span m="244260">then</span> <span m="244710">they're</span> <span m="244890">diabetic.</span>
  <span m="245460">And</span> <span m="245560">that's,</span> <span m="246070">in</span>
  <span m="246750">fact,</span> <span m="246930">usually</span> <span m="247320">used</span>
  <span m="247530">as</span> <span m="247650">a</span> <span m="247680">definition</span>
  <span m="248460">of</span> <span m="248760">diabetes.</span></p><p><span m="250020">But</span>
  <span m="251130">that</span> <span m="251190">didn't</span> <span m="251370">answer</span>
  <span m="251640">my</span> <span m="251790">original</span> <span m="252030">question.</span>
  <span m="252490">Why</span> <span m="253020">is</span> <span m="253140">just</span>
  <span m="253290">looking</span> <span m="253500">at</span> <span m="253560">diabetic</span>
  <span m="253920">medications</span> <span m="254490">not</span> <span m="254670">enough?</span></p><p><span
  m="258394">AUDIENCE:</span> <span m="258551">Some</span> <span m="258708">of</span>
  <span m="258866">the diabetic</span> <span m="259810">medications</span> <span m="260282">can
  be</span> <span m="260754">used to</span> <span m="261226">treat other</span> <span
  m="261698">conditions.</span></p><p><span m="262650">PROFESSOR:</span> <span m="262890">Sometimes</span>
  <span m="263130">there's</span> <span m="263250">ambiguity</span> <span m="263880">in</span>
  <span m="263970">diabetic</span> <span m="264840">medications.</span> <span m="265530">But</span>
  <span m="265680">we've</span> <span m="265950">sort</span> <span m="266220">of</span>
  <span m="266310">dealt</span> <span m="266550">with</span> <span m="266700">that</span>
  <span m="266850">already</span> <span m="267090">by</span> <span m="267180">trying</span>
  <span m="267360">to</span> <span m="267450">choose</span> <span m="267690">an</span>
  <span m="267810">unambiguous</span> <span m="268410">set.</span> <span m="269610">What
  are</span> <span m="269730">other</span> <span m="269880">reasons?</span></p><p><span
  m="271491">AUDIENCE:</span> <span m="271690">You're</span> <span m="271890">starting</span>
  <span m="272270">with</span> <span m="272430">the</span> <span m="272510">medicine</span>
  <span m="272980">at</span> <span m="273280">the</span> <span m="273400">onset</span>
  <span m="273730">of</span> <span m="273850">diabetes</span> <span m="274590">[INAUDIBLE].</span></p><p><span
  m="277130">PROFESSOR:</span> <span m="277245">Oh,</span> <span m="277360">that's</span>
  <span m="277500">a</span> <span m="277560">really</span> <span m="278040">interesting</span>
  <span m="278490">point--</span> <span m="278970">not</span> <span m="279150">the</span>
  <span m="279240">one</span> <span m="279390">I</span> <span m="279420">was</span>
  <span m="279510">thinking</span> <span m="279810">about,</span> <span m="279990">but</span>
  <span m="280080">I</span> <span m="280140">like</span> <span m="280410">it--</span>
  <span m="281220">which</span> <span m="281430">is</span> <span m="281580">that</span>
  <span m="282270">a</span> <span m="282330">patient</span> <span m="282630">might</span>
  <span m="282780">have</span> <span m="282870">been</span> <span m="282990">diagnosed</span>
  <span m="283560">with</span> <span m="283680">type</span> <span m="283890">2</span>
  <span m="284010">diabetes,</span> <span m="284610">but</span> <span m="284820">they,</span>
  <span m="285480">for</span> <span m="285690">whatever</span> <span m="286140">reason,</span>
  <span m="287210">in</span> <span m="287370">that</span> <span m="287520">communication</span>
  <span m="288120">between</span> <span m="288390">provider</span> <span m="288870">and</span>
  <span m="288960">patient,</span> <span m="289260">they</span> <span m="289380">decided</span>
  <span m="289890">we're</span> <span m="290040">not</span> <span m="290190">going</span>
  <span m="290310">to</span> <span m="290370">start</span> <span m="290550">treatment</span>
  <span m="290850">yet.</span> <span m="292050">So</span> <span m="293010">they</span>
  <span m="293130">might</span> <span m="293400">not</span> <span m="293730">yet</span>
  <span m="293970">be</span> <span m="294150">on</span> <span m="294360">treatment</span>
  <span m="294810">for</span> <span m="294960">diabetes,</span> <span m="295800">yet</span>
  <span m="296160">the</span> <span m="296370">whole</span> <span m="296700">health</span>
  <span m="296890">care</span> <span m="297210">system</span> <span m="297570">might</span>
  <span m="297720">be</span> <span m="297870">very</span> <span m="298260">well</span>
  <span m="298440">aware</span> <span m="298710">that</span> <span m="298840">the</span>
  <span m="298890">patient</span> <span m="299190">is</span> <span m="299250">diabetic,</span>
  <span m="299640">in</span> <span m="299700">which</span> <span m="299850">case</span>
  <span m="300770">doing</span> <span m="301200">these</span> <span m="301350">interventions</span>
  <span m="301920">for</span> <span m="301980">that</span> <span m="302100">patient</span>
  <span m="302370">might</span> <span m="302490">be</span> <span m="302640">irrelevant.</span>
  <span m="303960">Yep,</span> <span m="304110">another</span> <span m="304350">reason?</span></p><p><span
  m="304620">AUDIENCE:</span> <span m="304715">So</span> <span m="304810">a</span>
  <span m="304890">lot</span> <span m="305160">of people</span> <span m="305660">are
  just</span> <span m="305880">not</span> <span m="306090">diagnosed</span> <span
  m="306730">for diabetes.</span> <span m="307530">So</span> <span m="307650">they
  have it.</span> <span m="308200">So</span> <span m="308310">one</span> <span m="308580">label</span>
  <span m="308910">means</span> <span m="309270">that</span> <span m="309410">they</span>
  <span m="309510">have</span> <span m="309720">diabetes,</span> <span m="310280">and</span>
  <span m="310370">the</span> <span m="310470">other</span> <span m="310650">label</span>
  <span m="311160">is</span> <span m="311390">a</span> <span m="311420">combination</span>
  <span m="311740">of</span> <span m="312060">people</span> <span m="312220">who</span>
  <span m="312665">have</span> <span m="313110">and</span> <span m="313555">don't</span>
  <span m="314000">have</span> <span m="314445">diabetes.</span></p><p><span m="314890">PROFESSOR:</span>
  <span m="314975">So</span> <span m="315060">the</span> <span m="315150">point</span>
  <span m="315370">was,</span> <span m="315570">often</span> <span m="315870">you</span>
  <span m="315960">just</span> <span m="316140">might</span> <span m="316320">not</span>
  <span m="316470">be</span> <span m="316590">diagnosed</span> <span m="317220">for</span>
  <span m="317340">diabetes.</span> <span m="318840">That,</span> <span m="319050">unfortunately,</span>
  <span m="319560">is</span> <span m="319650">not</span> <span m="319770">something</span>
  <span m="319990">that</span> <span m="320080">we're</span> <span m="320170">going</span>
  <span m="320240">to</span> <span m="320310">able</span> <span m="320430">to</span>
  <span m="320490">solve</span> <span m="320820">here.</span> <span m="321640">It</span>
  <span m="322170">is</span> <span m="322290">an</span> <span m="322380">issue,</span>
  <span m="322770">but</span> <span m="323340">we</span> <span m="323490">have</span>
  <span m="323640">no</span> <span m="323790">solution</span> <span m="324180">for</span>
  <span m="324330">it.</span></p><p><span m="325410">No,</span> <span m="325810">rather</span>
  <span m="326100">there's</span> <span m="326280">a</span> <span m="326310">different</span>
  <span m="326640">point</span> <span m="326910">that</span> <span m="327030">I</span>
  <span m="327090">want</span> <span m="327240">to</span> <span m="327330">get</span>
  <span m="327570">at,</span> <span m="327750">which</span> <span m="327960">is</span>
  <span m="328110">that</span> <span m="328410">this</span> <span m="328590">data</span>
  <span m="328860">has</span> <span m="329040">biases</span> <span m="329580">in</span>
  <span m="329700">it.</span> <span m="329950">So</span> <span m="330420">even</span>
  <span m="330750">if</span> <span m="330870">a</span> <span m="330930">patient</span>
  <span m="331680">is</span> <span m="332220">on</span> <span m="332580">a</span>
  <span m="332640">diabetes</span> <span m="333150">medication,</span> <span m="335160">for</span>
  <span m="335370">whatever</span> <span m="335640">reason--</span> <span m="336130">maybe</span>
  <span m="336450">they</span> <span m="336810">are</span> <span m="337080">paying</span>
  <span m="337500">cash</span> <span m="338010">for</span> <span m="338130">those</span>
  <span m="338280">medications.</span> <span m="339180">If</span> <span m="339660">they're</span>
  <span m="339780">paying</span> <span m="340020">cash</span> <span m="340410">for</span>
  <span m="340530">those</span> <span m="340680">medications,</span> <span m="341910">then</span>
  <span m="342030">there's</span> <span m="342180">not</span> <span m="342360">going</span>
  <span m="342510">to</span> <span m="342600">be</span> <span m="342750">any</span>
  <span m="342990">record</span> <span m="343710">for</span> <span m="343860">the</span>
  <span m="343950">patient</span> <span m="344250">taking</span> <span m="344520">those</span>
  <span m="344640">medications</span> <span m="345510">in</span> <span m="345840">the</span>
  <span m="346320">health</span> <span m="346590">insurance</span> <span m="347070">claims.</span>
  <span m="347730">Because</span> <span m="347970">the</span> <span m="348060">health</span>
  <span m="348300">insurer</span> <span m="348750">didn't</span> <span m="348990">have</span>
  <span m="349140">to</span> <span m="349230">pay</span> <span m="349440">for</span>
  <span m="349620">it.</span></p><p><span m="351120">But</span> <span m="351480">the</span>
  <span m="351660">reason</span> <span m="351900">that</span> <span m="351990">you</span>
  <span m="352080">gave</span> <span m="352290">is</span> <span m="352380">also a</span>
  <span m="352620">very</span> <span m="352800">interesting</span> <span m="353130">reason.</span>
  <span m="353520">And</span> <span m="353790">both</span> <span m="354000">of</span>
  <span m="354060">them</span> <span m="354180">are</span> <span m="354270">valid.</span>
  <span m="354720">So</span> <span m="354780">for</span> <span m="354960">all</span>
  <span m="355260">of</span> <span m="355350">these</span> <span m="355560">reasons,</span>
  <span m="356550">just</span> <span m="356820">looking</span> <span m="357060">at</span>
  <span m="357120">the</span> <span m="357180">medications</span> <span m="357840">alone</span>
  <span m="358200">is</span> <span m="358320">going</span> <span m="358470">to</span>
  <span m="358530">be</span> <span m="358590">insufficient.</span> <span m="359280">And</span>
  <span m="359490">as</span> <span m="359640">was</span> <span m="359760">just</span>
  <span m="359910">suggested</span> <span m="360300">a</span> <span m="360330">moment</span>
  <span m="360600">ago,</span> <span m="361200">looking</span> <span m="361440">at</span>
  <span m="361590">other</span> <span m="361890">indicators,</span> <span m="362550">like,</span>
  <span m="363030">for</span> <span m="363150">example,</span> <span m="363600">does</span>
  <span m="363750">the</span> <span m="363810">patient</span> <span m="365160">have</span>
  <span m="365370">an</span> <span m="365490">abnormal</span> <span m="366090">blood</span>
  <span m="366300">glucose</span> <span m="366600">value</span> <span m="366900">or</span>
  <span m="368320">HBA1C</span> <span m="369000">value</span> <span m="369780">would</span>
  <span m="370110">also</span> <span m="370500">provide</span> <span m="370770">information.</span></p><p><span
  m="371640">So</span> <span m="372630">it's</span> <span m="372840">non-trivial,</span>
  <span m="373620">right?</span> <span m="373860">And</span> <span m="373980">part</span>
  <span m="374250">of</span> <span m="374340">what</span> <span m="374430">you're</span>
  <span m="374520">going</span> <span m="374580">to</span> <span m="374640">be</span>
  <span m="374730">doing</span> <span m="375060">in</span> <span m="375150">your</span>
  <span m="375210">next</span> <span m="375420">problem</span> <span m="375660">set,</span>
  <span m="375870">problem</span> <span m="376140">set</span> <span m="376260">2,</span>
  <span m="376560">is</span> <span m="376680">going</span> <span m="376830">to</span>
  <span m="376890">be</span> <span m="376980">thinking</span> <span m="377400">through</span>
  <span m="377790">how</span> <span m="378120">does</span> <span m="378270">one</span>
  <span m="378450">actually</span> <span m="378720">do</span> <span m="378840">this</span>
  <span m="378990">cohort</span> <span m="379410">construction,</span> <span m="380550">not</span>
  <span m="380760">just</span> <span m="380940">what</span> <span m="381060">is</span>
  <span m="381180">your</span> <span m="381270">inclusion/exclusion</span> <span m="382200">criteria,</span>
  <span m="382650">but</span> <span m="382770">also</span> <span m="382980">how</span>
  <span m="383220">do</span> <span m="383280">you</span> <span m="383340">really</span>
  <span m="383670">derive</span> <span m="384300">those</span> <span m="384510">labels</span>
  <span m="385080">from</span> <span m="385680">that</span> <span m="385860">data</span>
  <span m="386080">set.</span></p><p><span m="386880">Now</span> <span m="388470">the</span>
  <span m="388560">traditional</span> <span m="389040">answer</span> <span m="389310">to</span>
  <span m="389370">this</span> <span m="389940">has</span> <span m="390150">two</span>
  <span m="390360">steps</span> <span m="390690">to</span> <span m="390870">it.</span>
  <span m="391350">Step</span> <span m="391650">1</span> <span m="392700">is</span>
  <span m="393270">to</span> <span m="393480">actually</span> <span m="393840">manually</span>
  <span m="394500">label</span> <span m="394860">some</span> <span m="395070">patients.</span>
  <span m="395800">So</span> <span m="396660">you</span> <span m="396750">take</span>
  <span m="396930">a</span> <span m="396960">few hundred</span> <span m="397170">patients,</span>
  <span m="398530">and</span> <span m="398550">you</span> <span m="398880">go</span>
  <span m="399210">through</span> <span m="399510">their</span> <span m="399720">data.</span>
  <span m="400050">You</span> <span m="400170">actually</span> <span m="400500">look</span>
  <span m="400830">at</span> <span m="400950">their</span> <span m="401100">data,</span>
  <span m="401550">and</span> <span m="401670">decide,</span> <span m="402660">is</span>
  <span m="402810">this</span> <span m="402990">patient</span> <span m="403350">diabetic</span>
  <span m="403920">or</span> <span m="403950">are</span> <span m="404040">they</span>
  <span m="404190">not</span> <span m="404460">diabetic?</span> <span m="406170">And</span>
  <span m="406290">the</span> <span m="406330">reason</span> <span m="406590">why</span>
  <span m="406740">you</span> <span m="406800">have</span> <span m="406950">to</span>
  <span m="407010">do</span> <span m="407130">that</span> <span m="407280">is</span>
  <span m="407370">because</span> <span m="407580">often</span> <span m="407970">what</span>
  <span m="408150">you</span> <span m="408270">might</span> <span m="408480">think</span>
  <span m="408870">of</span> <span m="409020">is</span> <span m="409170">obvious--</span>
  <span m="409680">like,</span> <span m="410010">oh,</span> <span m="410410">if</span>
  <span m="410430">they're</span> <span m="410520">on</span> <span m="410640">diabetes</span>
  <span m="410940">medication,</span> <span m="411510">they're</span> <span m="411660">diabetic--</span>
  <span m="412830">has</span> <span m="413050">flaws</span> <span m="413430">to</span>
  <span m="413610">it.</span> <span m="414060">And</span> <span m="414180">until</span>
  <span m="414390">you</span> <span m="414510">really</span> <span m="414780">dig</span>
  <span m="415110">down</span> <span m="415380">and</span> <span m="415470">look</span>
  <span m="415710">at</span> <span m="415770">the</span> <span m="415860">data,</span>
  <span m="416290">you</span> <span m="416310">might</span> <span m="416430">not</span>
  <span m="416550">recognize</span> <span m="417210">that</span> <span m="417360">that</span>
  <span m="417540">criteria</span> <span m="418080">has</span> <span m="418230">a</span>
  <span m="418290">flaw</span> <span m="418590">in</span> <span m="418710">it.</span>
  <span m="419220">So</span> <span m="419340">that</span> <span m="419460">chart</span>
  <span m="419820">review</span> <span m="420090">is</span> <span m="420180">really</span>
  <span m="420330">an</span> <span m="420420">essential</span> <span m="420930">part</span>
  <span m="421200">of</span> <span m="422310">this</span> <span m="422460">process.</span></p><p><span
  m="423510">Then</span> <span m="423660">the</span> <span m="423750">second</span>
  <span m="424110">step</span> <span m="424380">is,</span> <span m="424570">how</span>
  <span m="424590">do</span> <span m="424640">you</span> <span m="424730">generalize</span>
  <span m="426090">to</span> <span m="426240">get</span> <span m="426510">that</span>
  <span m="426720">label</span> <span m="427270">now</span> <span m="427530">for</span>
  <span m="427830">everyone</span> <span m="428400">in</span> <span m="428490">your</span>
  <span m="428610">population.</span> <span m="429910">And</span> <span m="429930">again,</span>
  <span m="430290">there, there</span> <span m="430730">are</span> <span m="430830">usually</span>
  <span m="431160">two</span> <span m="431370">different</span> <span m="431610">types</span>
  <span m="431910">of</span> <span m="432000">approaches.</span> <span m="433090">The</span>
  <span m="433110">first</span> <span m="433440">approach</span> <span m="434280">is</span>
  <span m="434400">to</span> <span m="434460">come</span> <span m="434580">up</span>
  <span m="434670">with</span> <span m="434760">some</span> <span m="434970">simple</span>
  <span m="435450">rule</span> <span m="436380">to</span> <span m="436590">try</span>
  <span m="437070">to</span> <span m="437430">then</span> <span m="437640">extrapolate</span>
  <span m="438390">to</span> <span m="438510">everyone.</span> <span m="438970">For</span>
  <span m="439020">example,</span> <span m="439720">if</span> <span m="439770">they</span>
  <span m="439890">have,</span> <span m="440940">A,</span> <span m="441180">diabetes</span>
  <span m="441930">medication,</span> <span m="442830">or</span> <span m="443280">an</span>
  <span m="443490">abnormal</span> <span m="444060">lab</span> <span m="444330">test</span>
  <span m="444600">result,</span> <span m="445020">that</span> <span m="445140">would</span>
  <span m="445260">be</span> <span m="445350">an</span> <span m="445410">example</span>
  <span m="445780">of</span> <span m="445830">a</span> <span m="445890">rule.</span>
  <span m="446820">And</span> <span m="446910">then</span> <span m="447000">you</span>
  <span m="447060">could</span> <span m="447180">then</span> <span m="447330">apply</span>
  <span m="447630">that</span> <span m="447810">to</span> <span m="448080">everyone.</span></p><p><span
  m="449970">But</span> <span m="450150">even</span> <span m="450510">those</span>
  <span m="450840">rules</span> <span m="451800">can</span> <span m="451980">be</span>
  <span m="452100">really</span> <span m="452370">tricky</span> <span m="452850">to</span>
  <span m="453000">derive.</span> <span m="453470">And</span> <span m="453940">I'll</span>
  <span m="454050">show</span> <span m="454180">you</span> <span m="454230">some</span>
  <span m="454380">examples</span> <span m="454645">of</span> <span m="454910">that</span>
  <span m="455170">in</span> <span m="455340">just</span> <span m="455610">a</span>
  <span m="455640">moment.</span> <span m="457990">And</span> <span m="459570">as</span>
  <span m="459780">we</span> <span m="459900">know,</span> <span m="460710">machine</span>
  <span m="461130">learning</span> <span m="461430">is</span> <span m="461700">sometimes</span>
  <span m="462150">good</span> <span m="462960">as</span> <span m="463140">an</span>
  <span m="463200">alternative</span> <span m="463710">for</span> <span m="464100">coming</span>
  <span m="464330">up</span> <span m="464400">with</span> <span m="464520">a</span>
  <span m="464560">rule.</span> <span m="464850">So</span> <span m="465500">there's</span>
  <span m="465700">often</span> <span m="466140">now</span> <span m="466320">a</span>
  <span m="466410">second</span> <span m="466970">approach</span> <span m="467320">to</span>
  <span m="467410">this</span> <span m="467550">being</span> <span m="467790">more</span>
  <span m="468180">and</span> <span m="468270">more</span> <span m="468390">commonly</span>
  <span m="468870">used</span> <span m="469260">in</span> <span m="469350">the</span>
  <span m="469440">literature,</span> <span m="470560">which</span> <span m="470670">is</span>
  <span m="470850">to</span> <span m="470970">actually</span> <span m="471330">use</span>
  <span m="471510">machine</span> <span m="471900">learning</span> <span m="472140">itself</span>
  <span m="472830">to</span> <span m="472980">derive</span> <span m="473430">the</span>
  <span m="473520">labels.</span></p><p><span m="474800">And</span> <span m="475300">this</span>
  <span m="475350">is</span> <span m="475440">a</span> <span m="475470">bit</span>
  <span m="475620">subtle,</span> <span m="476210">because</span> <span m="476280">it's</span>
  <span m="476400">machine</span> <span m="476700">learning</span> <span m="477060">for</span>
  <span m="477330">machine</span> <span m="477720">learning.</span> <span m="478020">So</span>
  <span m="478110">I</span> <span m="478170">want</span> <span m="478290">to</span>
  <span m="478350">break</span> <span m="478560">that</span> <span m="478710">down</span>
  <span m="478950">for</span> <span m="479040">one</span> <span m="479190">second.</span>
  <span m="481470">When</span> <span m="481620">you're</span> <span m="481710">trying</span>
  <span m="481920">to</span> <span m="481980">derive</span> <span m="482250">the</span>
  <span m="482370">labels,</span> <span m="482950">what</span> <span m="482970">you</span>
  <span m="483060">want</span> <span m="483180">to</span> <span m="483270">know</span>
  <span m="483540">is</span> <span m="484290">not,</span> <span m="485220">at</span>
  <span m="485490">time</span> <span m="486000">T,</span> <span m="486390">what's</span>
  <span m="486630">going</span> <span m="486750">to</span> <span m="486810">happen</span>
  <span m="487140">at</span> <span m="487230">time</span> <span m="487560">T</span>
  <span m="487800">plus</span> <span m="488070">W</span> <span m="488460">and</span>
  <span m="488580">onwards--</span> <span m="489120">that's</span> <span m="489360">the</span>
  <span m="489480">original</span> <span m="490110">machine</span> <span m="490440">learning</span>
  <span m="490650">task</span> <span m="491010">that</span> <span m="491130">we</span>
  <span m="491220">set</span> <span m="491400">out</span> <span m="491520">to</span>
  <span m="491610">solve--</span> <span m="492750">but</span> <span m="492900">rather,</span>
  <span m="493410">given</span> <span m="493860">everything</span> <span m="494520">you</span>
  <span m="494640">know</span> <span m="494920">about</span> <span m="495120">the</span>
  <span m="495240">patient,</span> <span m="495700">including</span> <span m="496080">the</span>
  <span m="496170">future</span> <span m="496680">data,</span> <span m="498060">is</span>
  <span m="498240">this</span> <span m="498420">patient</span> <span m="498900">newly</span>
  <span m="499410">diagnosed with</span> <span m="499800">diabetes</span> <span m="500400">in</span>
  <span m="500520">that</span> <span m="500700">window</span> <span m="501090">that</span>
  <span m="501230">I</span> <span m="501280">show</span> <span m="501480">in</span>
  <span m="501710">black</span> <span m="502030">there,</span> <span m="502170">between</span>
  <span m="502500">T</span> <span m="502800">plus</span> <span m="503280">W</span>
  <span m="503760">and</span> <span m="503880">onward.</span> <span m="504700">OK?</span></p><p><span
  m="506250">So</span> <span m="506460">for</span> <span m="506640">example,</span>
  <span m="508230">this</span> <span m="508620">machine</span> <span m="508920">learning</span>
  <span m="509160">problem,</span> <span m="509370">this</span> <span m="509490">new</span>
  <span m="509700">machine</span> <span m="509970">learning</span> <span m="510120">problem,</span>
  <span m="510360">could</span> <span m="510480">take,</span> <span m="510660">as</span>
  <span m="510780">input,</span> <span m="511110">lab</span> <span m="511380">test</span>
  <span m="511620">results,</span> <span m="512340">and</span> <span m="512820">medications,</span>
  <span m="513450">and</span> <span m="513539">a</span> <span m="513570">whole</span>
  <span m="513690">bunch</span> <span m="513900">of</span> <span m="513960">other</span>
  <span m="514200">data.</span> <span m="515190">And</span> <span m="515460">you</span>
  <span m="515700">then</span> <span m="516000">use</span> <span m="516570">the</span>
  <span m="516990">few</span> <span m="517440">examples</span> <span m="518610">you</span>
  <span m="518799">labeled</span> <span m="519210">in</span> <span m="519299">step</span>
  <span m="519600">1</span> <span m="520230">to</span> <span m="520380">try</span>
  <span m="520559">to</span> <span m="520679">predict,</span> <span m="521460">is</span>
  <span m="521580">this</span> <span m="521700">patient</span> <span m="522179">currently</span>
  <span m="522870">diabetic</span> <span m="523440">or</span> <span m="523500">not.</span>
  <span m="524460">You</span> <span m="524560">then</span> <span m="524730">use</span>
  <span m="524910">that</span> <span m="525090">model</span> <span m="525360">to</span>
  <span m="525480">extrapolate</span> <span m="525930">to</span> <span m="525990">the</span>
  <span m="526080">whole</span> <span m="526260">population.</span> <span m="526890">And</span>
  <span m="526980">now</span> <span m="527160">you</span> <span m="527280">have</span>
  <span m="527550">your</span> <span m="527760">outcome</span> <span m="528180">label.</span>
  <span m="528990">It</span> <span m="529290">might</span> <span m="529500">be</span>
  <span m="529590">a</span> <span m="529650">little</span> <span m="529830">bit</span>
  <span m="529920">imperfect,</span> <span m="530550">but</span> <span m="530730">hopefully</span>
  <span m="531060">it's</span> <span m="531210">much</span> <span m="531450">better</span>
  <span m="531720">than</span> <span m="531970">what</span> <span m="532180">you</span>
  <span m="532260">could</span> <span m="532350">have</span> <span m="532440">gotten</span>
  <span m="532650">with</span> <span m="532790">a</span> <span m="532830">rule.</span>
  <span m="533700">And</span> <span m="533820">then,</span> <span m="534330">now</span>
  <span m="534540">using</span> <span m="534780">those</span> <span m="534990">outcome</span>
  <span m="535710">labels,</span> <span m="536340">you</span> <span m="536820">solve</span>
  <span m="537120">your</span> <span m="537180">original</span> <span m="537570">machine</span>
  <span m="537870">learning</span> <span m="538140">problem.</span> <span m="539940">Is</span>
  <span m="540030">that</span> <span m="540120">clear?</span> <span m="540460">Any</span>
  <span m="540480">questions?</span></p><p><span m="542960">AUDIENCE:</span> <span
  m="543121">I </span> <span m="543282">have</span> <span m="543445">one. </span></p><p><span
  m="543930">PROFESSOR:</span> <span m="543955">Yep.</span></p><p><span m="544270">AUDIENCE:</span>
  <span m="544360">How</span> <span m="544450">do</span> <span m="544510">you</span>
  <span m="544690">evaluate</span> <span m="545170">yourself</span> <span m="545490">then,</span>
  <span m="546400">if</span> <span m="546520">you</span> <span m="546610">have</span>
  <span m="546730">these</span> <span m="546880">labels</span> <span m="547240">that</span>
  <span m="547360">were</span> <span m="547480">produced</span> <span m="547810">with</span>
  <span m="547960">machine</span> <span m="548270">learning,</span> <span m="548430">which
  are</span> <span m="548890">probabilistic?</span></p><p><span m="550270">PROFESSOR:</span>
  <span m="550375">So</span> <span m="550480">that's</span> <span m="550750">where</span>
  <span m="550900">this</span> <span m="551110">first</span> <span m="551380">step</span>
  <span m="551620">is</span> <span m="551740">really</span> <span m="551980">important.</span>
  <span m="552880">You've</span> <span m="553030">got</span> <span m="553200">to</span>
  <span m="553330">get</span> <span m="553540">ground</span> <span m="553840">truth</span>
  <span m="554110">somehow.</span> <span m="556000">And</span> <span m="557200">of</span>
  <span m="557320">course</span> <span m="557740">once</span> <span m="558070">you</span>
  <span m="558160">get</span> <span m="558370">that</span> <span m="558550">ground</span>
  <span m="558820">truth,</span> <span m="559210">you</span> <span m="559420">create</span>
  <span m="559780">a</span> <span m="559900">train-and-validate</span> <span m="561100">set</span>
  <span m="561880">of</span> <span m="562030">that</span> <span m="562210">ground</span>
  <span m="562480">truth.</span> <span m="562810">You</span> <span m="562930">run</span>
  <span m="563110">your</span> <span m="563200">machine</span> <span m="563440">learning</span>
  <span m="563710">algorithm</span> <span m="563840">with the</span> <span m="563920">trained</span>
  <span m="564160">one.</span> <span m="564340">You'd</span> <span m="564400">look</span>
  <span m="564610">at</span> <span m="564690">its</span> <span m="564790">performance</span>
  <span m="565270">metrics</span> <span m="565810">on</span> <span m="565960">that</span>
  <span m="566140">validate</span> <span m="566620">set</span> <span m="567460">for</span>
  <span m="567700">the</span> <span m="567940">label</span> <span m="568330">prediction</span>
  <span m="568750">problem.</span> <span m="569260">And</span> <span m="569360">that's</span>
  <span m="569410">how</span> <span m="569500">you</span> <span m="569590">get</span>
  <span m="569740">confidence</span> <span m="570190">in</span> <span m="570280">it.</span></p><p><span
  m="571640">But</span> <span m="571780">let's</span> <span m="571900">try</span>
  <span m="571990">to</span> <span m="572080">break</span> <span m="572230">this</span>
  <span m="572320">down</span> <span m="572470">a</span> <span m="572530">little</span>
  <span m="572680">bit.</span> <span m="572960">So</span> <span m="573310">first</span>
  <span m="573580">of</span> <span m="573640">all,</span> <span m="573830">what</span>
  <span m="573920">does</span> <span m="574060">this</span> <span m="574510">chart</span>
  <span m="574810">review</span> <span m="575140">step</span> <span m="575410">look</span>
  <span m="575620">like?</span> <span m="576440">Well,</span> <span m="576730">if</span>
  <span m="576880">it's</span> <span m="577020">an</span> <span m="577120">electronic</span>
  <span m="577570">health</span> <span m="577810">record</span> <span m="578110">system,</span>
  <span m="578560">what</span> <span m="578680">you</span> <span m="578770">often</span>
  <span m="579100">do</span> <span m="579340">is</span> <span m="579910">you</span>
  <span m="580090">will</span> <span m="580210">pull</span> <span m="580420">up</span>
  <span m="580600">Epic,</span> <span m="580750">or</span> <span m="581080">Cerner,</span>
  <span m="581335">or</span> <span m="581590">whatever</span> <span m="581860">the</span>
  <span m="581920">commercial</span> <span m="582250">EHR</span> <span m="583000">system</span>
  <span m="583360">is.</span> <span m="584110">And</span> <span m="584320">you</span>
  <span m="584430">will</span> <span m="584620">actually</span> <span m="584920">start</span>
  <span m="585140">looking</span> <span m="585430">at</span> <span m="585490">the</span>
  <span m="585550">patient</span> <span m="585820">data.</span> <span m="586060">You'll</span>
  <span m="586210">read</span> <span m="586450">notes</span> <span m="586810">written</span>
  <span m="587050">by</span> <span m="587410">previous</span> <span m="587770">doctors</span>
  <span m="588220">about</span> <span m="588370">this</span> <span m="588490">patient.</span>
  <span m="588850">And</span> <span m="588930">you'll</span> <span m="589030">look</span>
  <span m="589240">at</span> <span m="589300">their</span> <span m="589420">blood</span>
  <span m="589690">test</span> <span m="589930">results</span> <span m="590260">across</span>
  <span m="590560">time,</span> <span m="591220">medications</span> <span m="591790">that</span>
  <span m="591910">they're</span> <span m="592030">on.</span> <span m="592750">And</span>
  <span m="592840">from</span> <span m="592990">that</span> <span m="593170">you</span>
  <span m="593260">can</span> <span m="593380">usually</span> <span m="593620">tell</span>
  <span m="593920">pretty</span> <span m="594190">coherent</span> <span m="594700">story</span>
  <span m="595130">what's</span> <span m="595300">going</span> <span m="595450">on</span>
  <span m="595510">with</span> <span m="595600">your</span> <span m="595660">patient.</span></p><p><span
  m="596920">Of</span> <span m="596970">course</span> <span m="597160">even</span>
  <span m="597400">better--</span> <span m="597760">or the</span> <span m="597850">best</span>
  <span m="598090">way</span> <span m="598210">to</span> <span m="598300">get</span>
  <span m="598420">data</span> <span m="598660">is</span> <span m="598750">to</span>
  <span m="598840">do</span> <span m="598960">a</span> <span m="599020">prospective</span>
  <span m="599740">study.</span> <span m="600210">So</span> <span m="600400">you</span>
  <span m="600520">actually</span> <span m="600790">have</span> <span m="600910">a</span>
  <span m="600940">research</span> <span m="601300">assistant</span> <span m="603010">standing</span>
  <span m="603520">in</span> <span m="603610">the</span> <span m="603700">room</span>
  <span m="603970">when</span> <span m="604120">a</span> <span m="604150">patient</span>
  <span m="604450">walks</span> <span m="604780">into</span> <span m="605110">a</span>
  <span m="605170">provider.</span> <span m="606010">And</span> <span m="606220">they</span>
  <span m="606490">talk</span> <span m="607510">to</span> <span m="607600">the</span>
  <span m="607660">patient,</span> <span m="608080">and</span> <span m="608430">they</span>
  <span m="608590">take</span> <span m="608800">down</span> <span m="609100">really</span>
  <span m="609940">very</span> <span m="611410">clear</span> <span m="611770">notes</span>
  <span m="612160">what</span> <span m="612340">this</span> <span m="612460">patient</span>
  <span m="612730">has,</span> <span m="612910">what</span> <span m="613000">they</span>
  <span m="613090">don't</span> <span m="613300">have.</span> <span m="613930">But</span>
  <span m="614020">that's</span> <span m="614200">usually</span> <span m="614410">too</span>
  <span m="614560">expensive</span> <span m="614980">to</span> <span m="615100">do</span>
  <span m="615280">prospectively.</span> <span m="615940">So</span> <span m="616090">usually</span>
  <span m="616390">what</span> <span m="616480">we</span> <span m="616570">do</span>
  <span m="616690">is</span> <span m="616780">do</span> <span m="616900">this</span>
  <span m="617380">retrospectively.</span></p><p><span m="619030">Now,</span> <span
  m="619240">if</span> <span m="619390">you're</span> <span m="619750">working</span>
  <span m="619960">with</span> <span m="620080">health</span> <span m="620320">insurance</span>
  <span m="620680">claims</span> <span m="620980">data,</span> <span m="621300">you</span>
  <span m="621390">usually</span> <span m="621700">don't</span> <span m="621850">have</span>
  <span m="621940">the</span> <span m="622030">luxury</span> <span m="622480">of</span>
  <span m="622570">looking</span> <span m="622810">at</span> <span m="622930">notes.</span>
  <span m="623710">And</span> <span m="623800">so</span> <span m="624400">what,</span>
  <span m="625270">in</span> <span m="625330">my</span> <span m="625480">group,</span>
  <span m="625820">we</span> <span m="625930">type</span> <span m="626290">typically</span>
  <span m="626620">do</span> <span m="626770">is</span> <span m="626860">we</span>
  <span m="626980">build,</span> <span m="627430">actually,</span> <span m="627760">a</span>
  <span m="627790">visualization</span> <span m="628360">tool.</span> <span m="629770">And</span>
  <span m="629870">by</span> <span m="629970">the</span> <span m="630070">way,</span>
  <span m="630220">I'm</span> <span m="630370">a</span> <span m="630400">machine</span>
  <span m="630640">learning</span> <span m="630850">person.</span> <span m="631690">I</span>
  <span m="631720">don't</span> <span m="631840">know</span> <span m="631990">anything</span>
  <span m="632380">about</span> <span m="632530">visualization.</span> <span m="634060">Neither</span>
  <span m="634360">do</span> <span m="634450">I</span> <span m="634540">claim</span>
  <span m="634930">to</span> <span m="635110">be</span> <span m="635230">good</span>
  <span m="635410">at</span> <span m="635530">it.</span></p><p><span m="636460">But</span>
  <span m="636970">you</span> <span m="637090">can't</span> <span m="637480">do</span>
  <span m="637720">the</span> <span m="637810">machine</span> <span m="638110">learning</span>
  <span m="638410">work</span> <span m="638890">unless</span> <span m="639160">you</span>
  <span m="639250">really</span> <span m="639430">understand</span> <span m="639790">your</span>
  <span m="639880">data.</span> <span m="640600">So</span> <span m="640990">we</span>
  <span m="641170">had</span> <span m="641440">to</span> <span m="641560">build</span>
  <span m="641830">this</span> <span m="641980">tool</span> <span m="642370">in</span>
  <span m="642490">order</span> <span m="642580">to</span> <span m="642700">look</span>
  <span m="642940">at</span> <span m="643030">the</span> <span m="643120">data,</span>
  <span m="643570">in</span> <span m="643720">order</span> <span m="643810">to</span>
  <span m="643930">try</span> <span m="644080">to</span> <span m="644200">do</span>
  <span m="644410">that</span> <span m="644590">first</span> <span m="644860">step</span>
  <span m="645160">of</span> <span m="645250">understanding,</span> <span m="646240">did</span>
  <span m="646390">we</span> <span m="646480">even</span> <span m="646660">characterize</span>
  <span m="647260">diabetes</span> <span m="647680">correctly.</span></p><p><span
  m="648690">So I'm</span> <span m="648820">not</span> <span m="648970">going</span>
  <span m="649130">go</span> <span m="649270">deep</span> <span m="649540">into</span>
  <span m="649720">it.</span> <span m="649810">By</span> <span m="649900">the</span>
  <span m="649990">way,</span> <span m="650570">you</span> <span m="650590">can</span>
  <span m="650740">download</span> <span m="651070">this.</span> <span m="651250">It's</span>
  <span m="651370">an</span> <span m="651460">open</span> <span m="651700">source</span>
  <span m="652390">tool.</span> <span m="653530">But</span> <span m="653830">ballpark</span>
  <span m="654340">what</span> <span m="654460">I'm</span> <span m="654550">showing</span>
  <span m="654760">you</span> <span m="654880">here</span> <span m="655060">is</span>
  <span m="655180">one</span> <span m="655420">patient's</span> <span m="655810">data.</span>
  <span m="656910">I'm</span> <span m="657040">showing</span> <span m="657250">on</span>
  <span m="657340">this</span> <span m="657490">x-axis,</span> <span m="658210">time,</span>
  <span m="658720">going</span> <span m="659020">from</span> <span m="659350">April</span>
  <span m="659830">to</span> <span m="660160">December.</span> <span m="661450">And</span>
  <span m="661690">on</span> <span m="661810">the</span> <span m="661900">y-axis,</span>
  <span m="662740">I'm</span> <span m="662860">showing</span> <span m="663220">events</span>
  <span m="663790">as</span> <span m="664000">they</span> <span m="664150">occurred.</span></p><p><span
  m="665180">So</span> <span m="665410">in</span> <span m="665680">orange</span> <span
  m="666280">are</span> <span m="666430">diagnosis</span> <span m="667240">codes</span>
  <span m="667540">that</span> <span m="667690">were</span> <span m="667960">recorded</span>
  <span m="668380">for</span> <span m="668440">the</span> <span m="668500">patient.</span>
  <span m="669130">In</span> <span m="669370">green</span> <span m="669790">are</span>
  <span m="669880">procedure</span> <span m="670420">codes.</span> <span m="670960">In</span>
  <span m="671140">blue</span> <span m="671470">are</span> <span m="671590">laboratory</span>
  <span m="672130">tests.</span> <span m="673030">And</span> <span m="673150">if</span>
  <span m="673240">you</span> <span m="673390">see,</span> <span m="674260">on</span>
  <span m="674380">a</span> <span m="674440">given</span> <span m="674800">line,</span>
  <span m="675220">multiple</span> <span m="675700">dots</span> <span m="676060">along</span>
  <span m="676300">that</span> <span m="676450">same</span> <span m="676690">line,</span>
  <span m="677390">it</span> <span m="677410">means</span> <span m="678630">that</span>
  <span m="678790">same</span> <span m="679210">lab</span> <span m="679480">test</span>
  <span m="679790">was</span> <span m="679900">performed</span> <span m="680350">multiple</span>
  <span m="680740">times.</span> <span m="681220">And</span> <span m="681310">you</span>
  <span m="681400">could</span> <span m="681520">click</span> <span m="681850">on</span>
  <span m="682000">it</span> <span m="682060">to</span> <span m="682180">see</span>
  <span m="682330">what</span> <span m="682450">the</span> <span m="682510">results</span>
  <span m="682900">were.</span> <span m="683430">And</span> <span m="683560">in</span>
  <span m="683620">this</span> <span m="683800">way,</span> <span m="684010">you</span>
  <span m="684100">could</span> <span m="684220">start</span> <span m="684400">to</span>
  <span m="684490">tell</span> <span m="684700">a</span> <span m="684760">coherent</span>
  <span m="685150">story</span> <span m="685600">what's</span> <span m="685780">going
  on</span> <span m="685910">with</span> <span m="685990">your</span> <span m="686050">patient.</span></p><p><span
  m="686855">All</span> <span m="687210">right,</span> <span m="687390">so</span>
  <span m="687480">tools</span> <span m="687870">like</span> <span m="688060">this</span>
  <span m="688240">is</span> <span m="688330">what</span> <span m="688480">you're</span>
  <span m="688570">going</span> <span m="688720">to</span> <span m="688810">need</span>
  <span m="689080">to</span> <span m="689200">able</span> <span m="689560">to</span>
  <span m="689710">do</span> <span m="689830">that</span> <span m="689980">first</span>
  <span m="690310">step</span> <span m="690700">from</span> <span m="691090">something</span>
  <span m="691360">like</span> <span m="691480">health</span> <span m="691690">insurance</span>
  <span m="692080">claims</span> <span m="692410">data.</span></p><p><span m="694180">Now,</span>
  <span m="694570">traditionally,</span> <span m="695590">that</span> <span m="695800">first</span>
  <span m="696160">step,</span> <span m="697910">which</span> <span m="698020">then</span>
  <span m="699370">leads</span> <span m="699730">you</span> <span m="699820">to</span>
  <span m="699940">label</span> <span m="700210">some</span> <span m="700420">data,</span>
  <span m="701090">and</span> <span m="701140">then,</span> <span m="701440">from</span>
  <span m="701710">there,</span> <span m="702130">you</span> <span m="702310">go</span>
  <span m="702970">and</span> <span m="703480">come</span> <span m="703690">up</span>
  <span m="703780">with</span> <span m="703900">these</span> <span m="704050">rules,</span>
  <span m="704470">or</span> <span m="704560">do</span> <span m="704660">a</span>
  <span m="704680">machine</span> <span m="704980">learning</span> <span m="705280">algorithm</span>
  <span m="705640">to</span> <span m="705730">get</span> <span m="705850">the</span>
  <span m="705970">label,</span> <span m="706810">usually</span> <span m="707080">that's</span>
  <span m="707240">a</span> <span m="707320">paper</span> <span m="707620">in</span>
  <span m="707710">itself.</span> <span m="708850">Of</span> <span m="708940">course,</span>
  <span m="709150">not</span> <span m="709300">of</span> <span m="709360">interest</span>
  <span m="709580">to</span> <span m="709620">the</span> <span m="709690">computer</span>
  <span m="709930">science</span> <span m="710290">community,</span> <span m="710710">but</span>
  <span m="710890">of</span> <span m="711070">extreme</span> <span m="711640">interest</span>
  <span m="712270">to</span> <span m="712420">the</span> <span m="712480">health</span>
  <span m="712690">care</span> <span m="712900">community.</span> <span m="713860">So</span>
  <span m="714460">usually</span> <span m="714910">there's</span> <span m="715090">a</span>
  <span m="715150">first</span> <span m="715600">paper,</span> <span m="716050">academic</span>
  <span m="716500">paper,</span> <span m="716830">which</span> <span m="716980">evaluates</span>
  <span m="717880">this</span> <span m="718090">process</span> <span m="719110">for</span>
  <span m="719350">deriving</span> <span m="719770">the</span> <span m="719860">label,</span>
  <span m="720700">and</span> <span m="720850">then</span> <span m="721090">there</span>
  <span m="721220">are</span> <span m="721330">much</span> <span m="721600">later</span>
  <span m="721990">papers</span> <span m="722410">which</span> <span m="722590">talk</span>
  <span m="722770">about</span> <span m="722950">what</span> <span m="723070">you</span>
  <span m="723160">could</span> <span m="723280">do</span> <span m="723460">with</span>
  <span m="723580">that</span> <span m="723700">label,</span> <span m="724030">such</span>
  <span m="724300">as</span> <span m="724510">the</span> <span m="724600">machine</span>
  <span m="724840">learning</span> <span m="725110">problem</span> <span m="725620">we</span>
  <span m="725770">originally</span> <span m="726070">set</span> <span m="726250">out</span>
  <span m="726340">to</span> <span m="726430">solve.</span></p><p><span m="727790">So</span>
  <span m="727810">let's</span> <span m="728050">look</span> <span m="728200">at</span>
  <span m="728260">an</span> <span m="728320">example</span> <span m="728710">of</span>
  <span m="728770">one</span> <span m="728890">of</span> <span m="728950">those</span>
  <span m="729100">rules.</span> <span m="730540">Here</span> <span m="731020">is</span>
  <span m="731470">a</span> <span m="731560">rule,</span> <span m="732430">to</span>
  <span m="732580">derive</span> <span m="733270">from</span> <span m="734350">health</span>
  <span m="734650">insurance</span> <span m="735130">claims</span> <span m="735760">data</span>
  <span m="736500">whether</span> <span m="736770">a</span> <span m="736810">patient</span>
  <span m="737170">has</span> <span m="737380">type</span> <span m="737650">2</span>
  <span m="737800">diabetes.</span> <span m="739250">Now,</span> <span m="739510">this</span>
  <span m="739660">isn't</span> <span m="740260">quite</span> <span m="743860">the</span>
  <span m="743980">same</span> <span m="744340">one</span> <span m="744640">that</span>
  <span m="744760">we</span> <span m="744940">used</span> <span m="745210">in</span>
  <span m="745270">that</span> <span m="745420">paper,</span> <span m="745910">but</span>
  <span m="745920">it</span> <span m="745990">gets</span> <span m="746200">the</span>
  <span m="746290">idea</span> <span m="746620">across.</span> <span m="747730">First</span>
  <span m="748060">you</span> <span m="748120">look</span> <span m="748270">to</span>
  <span m="748390">see,</span> <span m="748650">did</span> <span m="748720">the</span>
  <span m="748810">patient</span> <span m="749050">have</span> <span m="749200">a</span>
  <span m="749260">diagnosis</span> <span m="749950">code</span> <span m="750340">for</span>
  <span m="750640">type</span> <span m="751060">1</span> <span m="751810">diabetes.</span>
  <span m="754780">If</span> <span m="754930">the</span> <span m="755050">answer</span>
  <span m="755740">is</span> <span m="756460">no,</span> <span m="757270">you</span>
  <span m="757420">continue.</span> <span m="757990">If</span> <span m="758080">the</span>
  <span m="758140">answer</span> <span m="758410">is</span> <span m="758570">yes,</span>
  <span m="759060">you've</span> <span m="759220">sort</span> <span m="759400">of</span>
  <span m="759490">ruled</span> <span m="759760">out.</span> <span m="760080">Because
  you</span> <span m="760150">say,</span> <span m="760330">OK,</span> <span m="760990">this</span>
  <span m="761140">patient's</span> <span m="762310">abnormal</span> <span m="762760">blood</span>
  <span m="763000">test</span> <span m="763290">results</span> <span m="763420">are</span>
  <span m="763660">because</span> <span m="763930">they</span> <span m="764080">have</span>
  <span m="764470">type</span> <span m="764680">1</span> <span m="764980">diabetes,</span>
  <span m="765340">not</span> <span m="765520">type</span> <span m="765730">2</span>
  <span m="765940">diabetes.</span> <span m="767260">Type</span> <span m="767440">1</span>
  <span m="767590">diabetes</span> <span m="768010">usually</span> <span m="769210">is</span>
  <span m="769810">what</span> <span m="770020">you</span> <span m="770110">can</span>
  <span m="770200">think</span> <span m="770350">of</span> <span m="770470">as</span>
  <span m="770860">juvenile</span> <span m="771400">diabetes,</span> <span m="771820">is</span>
  <span m="771910">diagnosed</span> <span m="772360">much</span> <span m="772540">earlier.</span>
  <span m="773480">And</span> <span m="773590">there's</span> <span m="773740">a different</span>
  <span m="773980">mechanism</span> <span m="774370">behind</span> <span m="774640">it.</span></p><p><span
  m="775660">Then</span> <span m="775870">you</span> <span m="775960">look</span>
  <span m="776140">at</span> <span m="776230">other</span> <span m="776410">things--</span>
  <span m="776740">OK,</span> <span m="777280">is</span> <span m="777430">there</span>
  <span m="777580">a</span> <span m="777640">diagnosis</span> <span m="778420">code</span>
  <span m="778600">for</span> <span m="778720">type</span> <span m="778900">2</span>
  <span m="778990">diabetes</span> <span m="779380">somewhere</span> <span m="779680">in
  the</span> <span m="779770">patient's</span> <span m="780070">data?</span> <span
  m="780920">If</span> <span m="780970">so,</span> <span m="781460">you</span> <span
  m="781560">go</span> <span m="781660">to</span> <span m="781760">the</span> <span
  m="781860">right,</span> <span m="781990">and</span> <span m="782080">you</span>
  <span m="782140">look</span> <span m="782260">to</span> <span m="782350">see,</span>
  <span m="782500">is</span> <span m="782650">there</span> <span m="782770">a</span>
  <span m="782830">medication,</span> <span m="783490">an</span> <span m="783610">Rx,</span>
  <span m="784630">for</span> <span m="785080">type</span> <span m="785350">1</span>
  <span m="785710">diabetes</span> <span m="786190">in</span> <span m="786280">the</span>
  <span m="786340">data.</span> <span m="787480">If</span> <span m="787660">the</span>
  <span m="787750">answer</span> <span m="788260">is</span> <span m="788860">no,</span>
  <span m="789430">you</span> <span m="789550">continue</span> <span m="790030">down</span>
  <span m="790240">this</span> <span m="790420">way.</span> <span m="790620">If</span>
  <span m="790690">the</span> <span m="790750">answer</span> <span m="791020">is</span>
  <span m="791170">yes,</span> <span m="791660">you</span> <span m="791760">go</span>
  <span m="791830">this</span> <span m="792070">way.</span> <span m="793030">A</span>
  <span m="793500">yes</span> <span m="794160">of</span> <span m="794290">a</span>
  <span m="794340">type</span> <span m="794590">1</span> <span m="794800">diabetes</span>
  <span m="795130">medication</span> <span m="795520">doesn't</span> <span m="795850">alone</span>
  <span m="796330">rule</span> <span m="796540">out</span> <span m="796750">the</span>
  <span m="796810">patient.</span> <span m="797440">Because</span> <span m="797770">maybe</span>
  <span m="798130">the</span> <span m="798250">same</span> <span m="798490">medications</span>
  <span m="799030">are</span> <span m="799100">used</span> <span m="799330">for</span>
  <span m="799450">type</span> <span m="799630">1</span> <span m="799840">as</span>
  <span m="799960">for</span> <span m="800050">type</span> <span m="800230">2.</span>
  <span m="800770">So</span> <span m="800920">there's</span> <span m="801040">some</span>
  <span m="801160">other</span> <span m="801400">things</span> <span m="801640">you</span>
  <span m="801700">need</span> <span m="801820">to</span> <span m="801910">do</span>
  <span m="802060">there.</span></p><p><span m="802860">Right,</span> <span m="803150">you</span>
  <span m="803260">can</span> <span m="803380">see</span> <span m="803500">that</span>
  <span m="803620">this</span> <span m="803770">starts</span> <span m="804160">to</span>
  <span m="804310">really</span> <span m="804610">quickly</span> <span m="804940">become</span>
  <span m="805210">complicated.</span> <span m="806650">And</span> <span m="807040">these</span>
  <span m="807250">manual-based</span> <span m="808060">approaches</span> <span m="809830">end</span>
  <span m="810130">up</span> <span m="810490">having</span> <span m="811540">pretty</span>
  <span m="811870">bad</span> <span m="812380">positive--</span> <span m="813370">so</span>
  <span m="813670">they're</span> <span m="813850">designed</span> <span m="814360">usually</span>
  <span m="814530">to</span> <span m="814630">have</span> <span m="814780">pretty</span>
  <span m="815050">high</span> <span m="815320">positive</span> <span m="815770">predictive</span>
  <span m="816130">value.</span> <span m="816550">But</span> <span m="816670">they</span>
  <span m="816730">end</span> <span m="816850">up</span> <span m="816940">having</span>
  <span m="817180">pretty</span> <span m="817390">bad</span> <span m="817580">recall,</span>
  <span m="818490">in</span> <span m="818590">that</span> <span m="818710">they</span>
  <span m="818830">don't</span> <span m="818950">end</span> <span m="819040">up</span>
  <span m="819130">finding</span> <span m="819670">all</span> <span m="819850">of</span>
  <span m="819970">the</span> <span m="820060">patients.</span> <span m="821060">And</span>
  <span m="821160">that's</span> <span m="821230">really</span> <span m="821440">why</span>
  <span m="821750">the</span> <span m="821920">machine-learning-based</span> <span
  m="822730">approaches</span> <span m="823210">end</span> <span m="823390">up</span>
  <span m="823480">being</span> <span m="823690">very</span> <span m="823900">important</span>
  <span m="824380">for</span> <span m="824530">this</span> <span m="824650">type</span>
  <span m="824830">of</span> <span m="824890">problem.</span></p><p><span m="826570">Now,</span>
  <span m="827020">this</span> <span m="827260">is</span> <span m="827380">just</span>
  <span m="827560">one</span> <span m="827890">example</span> <span m="828290">of</span>
  <span m="828370">what</span> <span m="828490">I</span> <span m="828550">call a</span>
  <span m="828820">phenotype.</span> <span m="830030">I</span> <span m="830130">call</span>
  <span m="830200">this</span> <span m="830380">a</span> <span m="830440">phenotype.</span>
  <span m="831762">That's</span> <span m="832110">just</span> <span m="832510">what</span>
  <span m="832600">the</span> <span m="832660">literature</span> <span m="832930">calls</span>
  <span m="833230">it.</span> <span m="833590">It's</span> <span m="833710">a</span>
  <span m="833740">phenotype</span> <span m="834280">for</span> <span m="834550">type</span>
  <span m="834850">2</span> <span m="835000">diabetes.</span> <span m="835900">And</span>
  <span m="836830">the</span> <span m="836920">word,</span> <span m="837070">phenotype,</span>
  <span m="837430">in</span> <span m="837490">this</span> <span m="837580">context</span>
  <span m="837910">is</span> <span m="838000">exactly</span> <span m="838330">the</span>
  <span m="838390">same</span> <span m="838570">thing</span> <span m="838720">as</span>
  <span m="838810">the</span> <span m="838930">label.</span> <span m="839440">Yep.</span></p><p><span
  m="840005">AUDIENCE:</span> <span m="840156">What</span> <span m="840307">is</span>
  <span m="840460">abnormal</span> <span m="840915">mean?</span></p><p><span m="842280">PROFESSOR:</span>
  <span m="842340">For</span> <span m="842400">example,</span> <span m="843580">if</span>
  <span m="843990">the</span> <span m="844530">HA1C</span> <span m="845430">result</span>
  <span m="845940">is</span> <span m="846840">6.5</span> <span m="847770">or</span>
  <span m="847860">higher,</span> <span m="848340">you</span> <span m="848460">might</span>
  <span m="848640">say</span> <span m="848760">the</span> <span m="848820">patient</span>
  <span m="849210">has</span> <span m="849540">diabetes.</span></p><p><span m="850230">AUDIENCE:</span>
  <span m="850477">OK,</span> <span m="850725">so</span> <span m="851220">this</span>
  <span m="851370">is</span> <span m="851490">a</span> <span m="851580">lab</span>
  <span m="851760">result,</span> <span m="852176">not a</span> <span m="853008">medical--</span></p><p><span
  m="853840">PROFESSOR:</span> <span m="854007">Correct,</span> <span m="854510">yeah,</span>
  <span m="855180">thanks.</span> <span m="855520">Other</span> <span m="855640">questions.</span></p><p><span
  m="855930">AUDIENCE:</span> <span m="856016">What's the</span> <span m="856102">phenotype,</span>
  <span m="856620">which</span> <span m="856860">part</span> <span m="856980">exactly</span>
  <span m="857370">is the</span> <span m="857830">phenotype,</span> <span m="858290">like,
  the whole thing?</span></p><p><span m="858750">PROFESSOR:</span> <span m="858780">The</span>
  <span m="858810">whole</span> <span m="858930">thing,</span> <span m="859200">yeah.</span>
  <span m="859440">So</span> <span m="859590">the</span> <span m="859680">construction,</span>
  <span m="860370">where</span> <span m="860490">you</span> <span m="860580">say--</span>
  <span m="861300">you</span> <span m="861450">follow</span> <span m="861780">this</span>
  <span m="862890">decision</span> <span m="863310">tree,</span> <span m="863440">and</span>
  <span m="863540">you</span> <span m="863610">get</span> <span m="863760">to</span>
  <span m="864060">a</span> <span m="864480">conclusion,</span> <span m="865030">which</span>
  <span m="865110">is</span> <span m="865590">case,</span> <span m="866110">which</span>
  <span m="866190">means,</span> <span m="866460">yes</span> <span m="866700">they're</span>
  <span m="866910">type</span> <span m="867120">2</span> <span m="867210">diabetic.</span>
  <span m="868080">And</span> <span m="868200">if</span> <span m="868980">ever</span>
  <span m="869220">you</span> <span m="869310">don't</span> <span m="869550">reach</span>
  <span m="869760">this</span> <span m="869940">point,</span> <span m="870210">then</span>
  <span m="870360">the</span> <span m="870420">answer</span> <span m="870580">is</span>
  <span m="870690">no,</span> <span m="870930">they're</span> <span m="871050">not</span>
  <span m="871230">type</span> <span m="871410">2</span> <span m="871530">diabetic.</span>
  <span m="873060">That's</span> <span m="873240">what</span> <span m="873360">I</span>
  <span m="873420">mean</span> <span m="873570">by--</span> <span m="873810">so</span>
  <span m="874200">that</span> <span m="874380">labeling</span> <span m="875070">is</span>
  <span m="875190">what</span> <span m="875310">we're</span> <span m="875400">calling</span>
  <span m="875610">the</span> <span m="875700">phenotype</span> <span m="876300">of</span>
  <span m="876420">type</span> <span m="876570">2</span> <span m="876660">diabetes.</span></p><p><span
  m="877540">Now</span> <span m="878220">later</span> <span m="878820">in</span> <span
  m="879000">the</span> <span m="879060">semester,</span> <span m="879480">people
  will</span> <span m="879810">use</span> <span m="880080">the</span> <span m="880200">word,</span>
  <span m="880410">phenotype,</span> <span m="881040">to</span> <span m="881190">mean</span>
  <span m="881370">something</span> <span m="881700">else.</span> <span m="883740">It's</span>
  <span m="883890">an</span> <span m="883980">overloaded</span> <span m="884430">term.</span>
  <span m="884770">But</span> <span m="884880">this</span> <span m="885030">is</span>
  <span m="885090">what</span> <span m="885210">it's</span> <span m="885300">called</span>
  <span m="885480">in</span> <span m="885540">this</span> <span m="885660">context</span>
  <span m="885990">as</span> <span m="886080">well.</span></p><p><span m="887370">Now</span>
  <span m="888570">here's</span> <span m="888870">an</span> <span m="888960">example</span>
  <span m="889500">of</span> <span m="889590">a</span> <span m="889680">website--</span>
  <span m="890850">it's</span> <span m="891150">from</span> <span m="891390">the</span>
  <span m="891480">PheKB</span> <span m="892140">project--</span> <span m="893130">where</span>
  <span m="893340">you</span> <span m="893540">will</span> <span m="893730">find</span>
  <span m="895590">tens</span> <span m="896280">to</span> <span m="896430">close</span>
  <span m="896670">to</span> <span m="896810">100</span> <span m="897450">of</span>
  <span m="897600">these</span> <span m="897870">phenotypes</span> <span m="898650">that</span>
  <span m="898860">have</span> <span m="899040">been</span> <span m="899550">arduously</span>
  <span m="900240">created</span> <span m="901140">for</span> <span m="901380">a</span>
  <span m="901470">whole</span> <span m="902040">range</span> <span m="902310">of</span>
  <span m="902370">different</span> <span m="902640">conditions.</span> <span m="903500">OK,</span>
  <span m="903750">so</span> <span m="903930">if</span> <span m="904620">you</span>
  <span m="904680">go</span> <span m="904770">to</span> <span m="904830">this</span>
  <span m="904950">website,</span> <span m="905820">and</span> <span m="905940">you</span>
  <span m="906030">click</span> <span m="906330">on</span> <span m="906450">any</span>
  <span m="906660">one</span> <span m="906810">of</span> <span m="906870">these</span>
  <span m="907020">conditions,</span> <span m="907530">like</span> <span m="907740">appendicitis,</span>
  <span m="908640">autism,</span> <span m="909300">cataracts,</span> <span m="910380">you'll</span>
  <span m="910530">see</span> <span m="910740">a</span> <span m="910770">different</span>
  <span m="911250">diagram</span> <span m="911970">of</span> <span m="912060">this</span>
  <span m="912180">sort</span> <span m="912430">I</span> <span m="912480">just</span>
  <span m="912660">showed</span> <span m="912960">you.</span> <span m="913800">So</span>
  <span m="913890">this</span> <span m="914070">is</span> <span m="914160">a</span>
  <span m="914220">real</span> <span m="914520">thing.</span> <span m="914920">This</span>
  <span m="914940">is</span> <span m="915000">something</span> <span m="915240">that</span>
  <span m="915330">the</span> <span m="915420">medical</span> <span m="915780">community</span>
  <span m="916560">really</span> <span m="916920">needs</span> <span m="917130">to</span>
  <span m="917250">do</span> <span m="917610">in</span> <span m="917690">order</span>
  <span m="917790">to</span> <span m="917910">try</span> <span m="918090">to</span>
  <span m="918180">derive</span> <span m="918840">the</span> <span m="919020">label</span>
  <span m="919830">that</span> <span m="920010">we</span> <span m="920220">can</span>
  <span m="920400">then</span> <span m="920580">use</span> <span m="920820">in</span>
  <span m="920940">our</span> <span m="921090">machine</span> <span m="921450">learning</span>
  <span m="921720">task.</span></p><p><span m="924342">AUDIENCE:</span> <span m="924461">I'm</span>
  <span m="924580">just</span> <span m="924699">curious,</span> <span m="924818">is
  the</span> <span m="925294">lab</span> <span m="925770">value</span> <span m="926246">ground</span>
  <span m="927500">truth?</span> <span m="927910">Like</span> <span m="928320">if</span>
  <span m="928730">somebody</span> <span m="929090">has</span> <span m="929460">diabetes,</span>
  <span m="929630">then</span> <span m="930050">they must</span> <span m="930470">have</span>
  <span m="930890">[INAUDIBLE].</span> <span m="932570">It means</span> <span m="932985">they
  have been</span> <span m="933400">diagnosed,</span> <span m="933872">and</span>
  <span m="934344">they must</span> <span m="934816">have--</span></p><p><span m="935288">PROFESSOR:</span>
  <span m="935524">Well,</span> <span m="935760">so,</span> <span m="935910">for</span>
  <span m="936060">example,</span> <span m="936850">you</span> <span m="937230">might</span>
  <span m="937440">have</span> <span m="937620">an</span> <span m="937710">abnormal</span>
  <span m="938190">glucose</span> <span m="938670">value</span> <span m="939030">for</span>
  <span m="939330">a</span> <span m="939390">variety</span> <span m="939960">of</span>
  <span m="940020">reasons.</span> <span m="940600">One</span> <span m="940740">reason</span>
  <span m="941040">is</span> <span m="941160">because</span> <span m="941430">you</span>
  <span m="941490">might</span> <span m="941730">have</span> <span m="943530">what's</span>
  <span m="943680">called</span> <span m="943950">gestational</span> <span m="944580">diabetes,</span>
  <span m="945220">which</span> <span m="945270">is</span> <span m="945360">diabetes</span>
  <span m="945840">that's</span> <span m="945960">induced</span> <span m="946530">due</span>
  <span m="946830">to</span> <span m="947040">pregnancy.</span> <span m="948360">But</span>
  <span m="948450">those</span> <span m="948600">patients</span> <span m="948960">typically--</span>
  <span m="949490">well,</span> <span m="949890">although</span> <span m="950100">it's
  a</span> <span m="950220">predictive</span> <span m="950610">factor,</span> <span
  m="951090">they</span> <span m="951390">don't</span> <span m="951540">always</span>
  <span m="951870">have</span> <span m="952080">long-term</span> <span m="952740">type</span>
  <span m="952890">2</span> <span m="952980">diabetes.</span> <span m="954190">So</span>
  <span m="954690">even</span> <span m="955020">the</span> <span m="955110">laboratory</span>
  <span m="955710">test</span> <span m="956010">alone</span> <span m="957780">doesn't</span>
  <span m="957960">tell</span> <span m="958080">the</span> <span m="958170">whole</span>
  <span m="958260">story.</span></p><p><span m="959056">AUDIENCE:</span> <span m="959172">You</span>
  <span m="959288">could</span> <span m="959404">be</span> <span m="959522">diagnosed</span>
  <span m="960454">without</span> <span m="960920">having</span> <span m="961386">abnormal</span>
  <span m="962318">diabetic?</span></p><p><span m="963720">PROFESSOR:</span> <span
  m="963900">That's</span> <span m="964080">much</span> <span m="964410">less</span>
  <span m="964620">common</span> <span m="965220">here.</span> <span m="966630">The</span>
  <span m="966750">story</span> <span m="967080">will</span> <span m="967260">change</span>
  <span m="967560">in</span> <span m="967620">the</span> <span m="967680">future,</span>
  <span m="968010">because</span> <span m="968430">there</span> <span m="968580">will</span>
  <span m="968730">be</span> <span m="968850">a</span> <span m="968940">whole</span>
  <span m="969210">range</span> <span m="969480">of</span> <span m="969570">new</span>
  <span m="969690">diagnosis</span> <span m="970320">techniques</span> <span m="971310">that</span>
  <span m="971490">might</span> <span m="971700">use</span> <span m="972030">new</span>
  <span m="972180">modalities,</span> <span m="973290">like</span> <span m="975540">gene</span>
  <span m="975750">expression,</span> <span m="976170">for</span> <span m="976260">example.</span>
  <span m="978220">But</span> <span m="978450">typically,</span> <span m="978900">today,</span>
  <span m="979140">the</span> <span m="979190">answer</span> <span m="979370">is</span>
  <span m="979490">yes to</span> <span m="979700">that.</span> <span m="981390">Yep.</span></p><p><span
  m="981520">AUDIENCE:</span> <span m="981632">So</span> <span m="981744">if</span>
  <span m="981856">these</span> <span m="981970">are made by</span> <span m="982430">doctors,</span>
  <span m="982770">does that mean,</span> <span m="983090">for</span> <span m="983240">every</span>
  <span m="983390">single</span> <span m="983630">disease,</span> <span m="983925">there's</span>
  <span m="984220">one</span> <span m="984470">definitive</span> <span m="984880">phenotype?</span></p><p><span
  m="985700">PROFESSOR:</span> <span m="985805">These</span> <span m="985910">are</span>
  <span m="985970">usually</span> <span m="986360">made</span> <span m="986780">by</span>
  <span m="988130">health</span> <span m="988430">outcomes</span> <span m="988880">researchers,</span>
  <span m="991070">which</span> <span m="991430">usually</span> <span m="991730">have</span>
  <span m="992000">clinicians</span> <span m="992510">on</span> <span m="992570">their</span>
  <span m="992690">team.</span> <span m="993840">But</span> <span m="994130">the</span>
  <span m="994220">type</span> <span m="994490">of</span> <span m="994580">people</span>
  <span m="994910">who</span> <span m="995120">often</span> <span m="995390">work</span>
  <span m="995580">on</span> <span m="995690">these</span> <span m="995960">often</span>
  <span m="996260">come</span> <span m="996500">from</span> <span m="996620">the</span>
  <span m="996680">field</span> <span m="996980">of</span> <span m="997040">epidemiology,</span>
  <span m="998160">for</span> <span m="998260">example.</span> <span m="1000650">And</span>
  <span m="1000730">so</span> <span m="1001210">what</span> <span m="1001420">was</span>
  <span m="1001510">your</span> <span m="1001600">question</span> <span m="1001860">again?</span></p><p><span
  m="1002860">AUDIENCE:</span> <span m="1002975">Is</span> <span m="1003090">there
  just</span> <span m="1003370">one</span> <span m="1003560">phenotype</span> <span
  m="1003660">for</span> <span m="1003700">every</span> <span m="1004070">single</span>
  <span m="1004440">disease?</span></p><p><span m="1004810">PROFESSOR:</span> <span
  m="1004885">Is</span> <span m="1004960">there</span> <span m="1005050">one</span>
  <span m="1005260">phenotype</span> <span m="1005660">for</span> <span m="1005710">every</span>
  <span m="1005890">different</span> <span m="1006640">disease?</span> <span m="1007690">In</span>
  <span m="1007840">the</span> <span m="1007900">ideal</span> <span m="1008320">world,</span>
  <span m="1008750">you'd</span> <span m="1008800">have</span> <span m="1008980">at</span>
  <span m="1009070">least</span> <span m="1009370">one</span> <span m="1009550">phenotype</span>
  <span m="1009970">for every</span> <span m="1010180">single</span> <span m="1010450">disease</span>
  <span m="1010780">that</span> <span m="1010870">could</span> <span m="1010960">possibly</span>
  <span m="1011350">exist.</span> <span m="1012550">Now,</span> <span m="1012700">of</span>
  <span m="1012790">course,</span> <span m="1013030">you</span> <span m="1013120">might</span>
  <span m="1013240">be</span> <span m="1013330">interested</span> <span m="1013630">in</span>
  <span m="1013690">different</span> <span m="1013960">aspects.</span> <span m="1014560">Like</span>
  <span m="1014740">you</span> <span m="1014800">might</span> <span m="1014920">be</span>
  <span m="1015010">interested</span> <span m="1015310">in</span> <span m="1015370">not</span>
  <span m="1015550">knowing</span> <span m="1015850">just</span> <span m="1016660">does</span>
  <span m="1016870">the</span> <span m="1016960">patient</span> <span m="1017260">have</span>
  <span m="1017440">autism,</span> <span m="1017920">but</span> <span m="1018070">where</span>
  <span m="1018340">they</span> <span m="1018550">are</span> <span m="1018790">on</span>
  <span m="1018880">their</span> <span m="1018970">autism</span> <span m="1019330">spectrum.</span>
  <span m="1020250">You</span> <span m="1020410">might</span> <span m="1020560">not</span>
  <span m="1020680">be</span> <span m="1020800">interested</span> <span m="1021310">in</span>
  <span m="1021460">knowing</span> <span m="1021730">just,</span> <span m="1022360">do</span>
  <span m="1022510">they</span> <span m="1022660">have</span> <span m="1023020">it</span>
  <span m="1023110">now,</span> <span m="1023600">but</span> <span m="1023620">you</span>
  <span m="1023680">also</span> <span m="1023860">might</span> <span m="1024010">want</span>
  <span m="1024130">to</span> <span m="1024190">know</span> <span m="1024400">when</span>
  <span m="1024790">did</span> <span m="1024940">they</span> <span m="1025060">get</span>
  <span m="1025300">it.</span> <span m="1025480">So</span> <span m="1025660">there's</span>
  <span m="1025839">a</span> <span m="1025869">lot</span> <span m="1026020">of</span>
  <span m="1026079">subtleties</span> <span m="1026530">that</span> <span m="1026650">could</span>
  <span m="1026920">go</span> <span m="1027130">into</span> <span m="1027369">this.</span></p><p><span
  m="1029140">But</span> <span m="1029319">building</span> <span m="1029740">these</span>
  <span m="1029920">up</span> <span m="1030069">is</span> <span m="1030220">really</span>
  <span m="1030730">slow.</span> <span m="1031750">And</span> <span m="1032560">validating</span>
  <span m="1033160">them</span> <span m="1033310">to</span> <span m="1033400">make</span>
  <span m="1033550">sure</span> <span m="1033700">that</span> <span m="1033849">they're</span>
  <span m="1033970">going</span> <span m="1034069">to</span> <span m="1034150">work</span>
  <span m="1034450">across</span> <span m="1034750">multiple</span> <span m="1034990">data</span>
  <span m="1035250">sets</span> <span m="1035410">is</span> <span m="1035560">really</span>
  <span m="1036130">challenging,</span> <span m="1036550">and</span> <span m="1036640">usually</span>
  <span m="1036900">is</span> <span m="1037000">a</span> <span m="1037060">negative</span>
  <span m="1037359">result.</span> <span m="1038750">And</span> <span m="1038859">so</span>
  <span m="1039579">it's</span> <span m="1039760">been</span> <span m="1039910">a</span>
  <span m="1039970">very</span> <span m="1040270">slow</span> <span m="1040510">process</span>
  <span m="1040869">to</span> <span m="1040990">do</span> <span m="1041050">this</span>
  <span m="1041230">manually,</span> <span m="1041750">which</span> <span m="1041770">has</span>
  <span m="1041890">led</span> <span m="1042670">me</span> <span m="1043060">and</span>
  <span m="1043150">many</span> <span m="1043420">others</span> <span m="1043869">to</span>
  <span m="1043960">start</span> <span m="1044200">thinking</span> <span m="1044470">about</span>
  <span m="1044740">the</span> <span m="1044890">machine</span> <span m="1045190">learning</span>
  <span m="1045460">approaches</span> <span m="1045880">for</span> <span m="1045940">how</span>
  <span m="1046030">to</span> <span m="1046119">do</span> <span m="1046210">it</span>
  <span m="1046270">automatically.</span></p><p><span m="1048430">AUDIENCE:</span>
  <span m="1048555">Just</span> <span m="1048680">as</span> <span m="1048805">a</span>
  <span m="1048930">follow-up,</span> <span m="1049930">is</span> <span m="1050060">there</span>
  <span m="1050180">any</span> <span m="1050300">case</span> <span m="1050500">where</span>
  <span m="1050650">there's,</span> <span m="1050840">like,</span> <span m="1051710">five</span>
  <span m="1052130">autism</span> <span m="1052520">phenotypes,</span> <span m="1053120">for</span>
  <span m="1053180">example,</span> <span m="1053720">or</span> <span m="1054117">multiple</span>
  <span m="1054514">competing ones?</span></p><p><span m="1055310">PROFESSOR:</span>
  <span m="1055535">Yes.</span> <span m="1055760">So</span> <span m="1056030">there</span>
  <span m="1056120">are</span> <span m="1056180">often</span> <span m="1056540">many</span>
  <span m="1056810">different</span> <span m="1057530">such</span> <span m="1058520">rule-based</span>
  <span m="1059090">systems</span> <span m="1059540">that</span> <span m="1059660">give</span>
  <span m="1059900">you</span> <span m="1060050">conflicting</span> <span m="1060590">results.</span>
  <span m="1061760">Yes,</span> <span m="1061970">that</span> <span m="1062090">happens</span>
  <span m="1062390">all</span> <span m="1062480">the</span> <span m="1062570">time.</span></p><p><span
  m="1064460">AUDIENCE:</span> <span m="1064595">Can</span> <span m="1064730">these</span>
  <span m="1064890">rule-based</span> <span m="1065210">systems</span> <span m="1065630">provide</span>
  <span m="1066390">an</span> <span m="1066500">estimate</span> <span m="1066840">of</span>
  <span m="1067010">when</span> <span m="1068232">their</span> <span m="1068678">condition
  was</span> <span m="1069124">onset? </span></p><p><span m="1069570">PROFESSOR:</span>
  <span m="1069690">Right,</span> <span m="1069810">so</span> <span m="1069900">that's</span>
  <span m="1070170">getting</span> <span m="1070390">at</span> <span m="1070470">one</span>
  <span m="1070560">of</span> <span m="1070620">the</span> <span m="1070680">subtleties</span>
  <span m="1071020">I</span> <span m="1071070">just</span> <span m="1071220">mentioned--</span>
  <span m="1071950">can these</span> <span m="1072360">tell</span> <span m="1072570">you</span>
  <span m="1072750">when</span> <span m="1073470">the</span> <span m="1073650">onset</span>
  <span m="1074070">happened?</span> <span m="1075510">They're</span> <span m="1075630">not</span>
  <span m="1075810">typically</span> <span m="1076200">designed</span> <span m="1076620">to</span>
  <span m="1076770">do</span> <span m="1076890">that,</span> <span m="1077170">but</span>
  <span m="1077270">one</span> <span m="1077340">can</span> <span m="1077880">come</span>
  <span m="1078060">up</span> <span m="1078150">with</span> <span m="1078330">one</span>
  <span m="1078540">to</span> <span m="1079200">do</span> <span m="1079380">it.</span>
  <span m="1079660">And</span> <span m="1079680">so</span> <span m="1079830">one</span>
  <span m="1080070">way</span> <span m="1080160">to</span> <span m="1080250">try</span>
  <span m="1080430">to</span> <span m="1080490">do</span> <span m="1080580">that</span>
  <span m="1080760">is</span> <span m="1081260">you</span> <span m="1081390">change</span>
  <span m="1081750">those</span> <span m="1082680">rules</span> <span m="1083400">to</span>
  <span m="1083550">have</span> <span m="1083760">a</span> <span m="1083850">time</span>
  <span m="1084180">period</span> <span m="1084620">associate</span> <span m="1084930">to</span>
  <span m="1085080">it.</span> <span m="1086340">And</span> <span m="1086490">then</span>
  <span m="1086610">you</span> <span m="1086700">can</span> <span m="1086820">imagine</span>
  <span m="1087570">applying</span> <span m="1088230">those</span> <span m="1088440">rules</span>
  <span m="1088710">in</span> <span m="1088830">a</span> <span m="1088890">sliding</span>
  <span m="1089370">window</span> <span m="1089670">to</span> <span m="1089760">the</span>
  <span m="1089850">patient</span> <span m="1090150">data</span> <span m="1090450">to</span>
  <span m="1090540">see,</span> <span m="1090720">when</span> <span m="1090840">is</span>
  <span m="1090930">the</span> <span m="1091020">first</span> <span m="1091290">time</span>
  <span m="1091470">that</span> <span m="1091590">it</span> <span m="1091650">triggers.</span>
  <span m="1093420">And</span> <span m="1093720">that</span> <span m="1093900">would</span>
  <span m="1093990">be</span> <span m="1094080">one</span> <span m="1094320">way</span>
  <span m="1094440">to</span> <span m="1094530">try</span> <span m="1094710">to</span>
  <span m="1094800">get</span> <span m="1094920">a</span> <span m="1094950">sense</span>
  <span m="1095250">of</span> <span m="1095340">when</span> <span m="1095520">onset</span>
  <span m="1095910">was.</span> <span m="1096740">But</span> <span m="1097080">there's</span>
  <span m="1097260">a</span> <span m="1097290">lot</span> <span m="1097440">of</span>
  <span m="1097500">subtleties</span> <span m="1097920">to</span> <span m="1097980">that,</span>
  <span m="1098130">too.</span></p><p><span m="1099290">So</span> <span m="1099750">I'm</span>
  <span m="1100210">going</span> <span m="1100340">to</span> <span m="1100410">move</span>
  <span m="1100590">on</span> <span m="1100710">now.</span> <span m="1101900">I</span>
  <span m="1101970">just</span> <span m="1102090">want</span> <span m="1102240">to</span>
  <span m="1102300">give</span> <span m="1102420">it</span> <span m="1102500">some</span>
  <span m="1102810">sense</span> <span m="1103200">of</span> <span m="1103440">what</span>
  <span m="1103710">that</span> <span m="1103920">deriving</span> <span m="1104400">the</span>
  <span m="1104490">labels</span> <span m="1104970">ends</span> <span m="1105150">up</span>
  <span m="1105270">looking</span> <span m="1105540">like.</span> <span m="1107010">Let's</span>
  <span m="1107190">now</span> <span m="1108030">turn</span> <span m="1108330">to</span>
  <span m="1108460">evaluation.</span> <span m="1111090">So</span> <span m="1111600">a</span>
  <span m="1111750">very</span> <span m="1112050">commonly</span> <span m="1112650">used</span>
  <span m="1112830">approach</span> <span m="1113190">in</span> <span m="1113280">this</span>
  <span m="1113460">field</span> <span m="1113910">is</span> <span m="1114090">to</span>
  <span m="1114300">compute</span> <span m="1114780">what's</span> <span m="1114990">known</span>
  <span m="1115170">as</span> <span m="1115290">the</span> <span m="1115410">Receiver-Operator</span>
  <span m="1116580">Curve,</span> <span m="1117910">or</span> <span m="1118110">ROC</span>
  <span m="1118620">curve.</span></p><p><span m="1120060">And</span> <span m="1120390">what</span>
  <span m="1120510">this</span> <span m="1120690">looks</span> <span m="1120900">at</span>
  <span m="1120990">is</span> <span m="1121080">the</span> <span m="1121170">following.</span>
  <span m="1121540">First</span> <span m="1121650">of</span> <span m="1121710">all,</span>
  <span m="1121890">this</span> <span m="1122280">is</span> <span m="1122550">well-defined</span>
  <span m="1123300">for a</span> <span m="1123630">binary</span> <span m="1124140">classification</span>
  <span m="1124800">problem.</span> <span m="1126900">For a</span> <span m="1127170">binary</span>
  <span m="1127470">classification</span> <span m="1127950">problem</span> <span m="1128670">when</span>
  <span m="1129120">you're</span> <span m="1129240">using</span> <span m="1129750">a</span>
  <span m="1130350">model</span> <span m="1130830">that</span> <span m="1131040">outputs,</span>
  <span m="1131430">let's</span> <span m="1131520">say,</span> <span m="1131700">a
  probability</span> <span m="1132450">or</span> <span m="1132600">some</span> <span
  m="1132810">continuous</span> <span m="1133500">value,</span> <span m="1134310">then</span>
  <span m="1134460">you</span> <span m="1134550">could</span> <span m="1134670">use</span>
  <span m="1134880">that</span> <span m="1135180">continuous</span> <span m="1135900">valid</span>
  <span m="1136230">prediction.</span> <span m="1137490">If</span> <span m="1137580">you</span>
  <span m="1137640">wanted</span> <span m="1137820">to</span> <span m="1137910">make</span>
  <span m="1138060">a</span> <span m="1138120">prediction,</span> <span m="1138390">you
  usually</span> <span m="1138660">threshold</span> <span m="1139130">it,</span> <span
  m="1139230">right?</span> <span m="1139450">So you</span> <span m="1139570">say,
  if</span> <span m="1139740">it's</span> <span m="1139830">greater</span> <span m="1140040">than</span>
  <span m="1140160">0.5,</span> <span m="1140790">it's</span> <span m="1140960">a</span>
  <span m="1141030">prediction</span> <span m="1141360">of</span> <span m="1141450">1.</span>
  <span m="1141750">If</span> <span m="1141840">it's</span> <span m="1141960">less</span>
  <span m="1142110">than</span> <span m="1142230">0.5,</span> <span m="1142590">prediction
  of</span> <span m="1142900">zero.</span></p><p><span m="1144510">But</span> <span
  m="1145350">here</span> <span m="1145650">we</span> <span m="1145770">might</span>
  <span m="1145860">be</span> <span m="1145940">interested</span> <span m="1146210">in</span>
  <span m="1146280">not</span> <span m="1146490">just</span> <span m="1147210">what</span>
  <span m="1147390">minimizes,</span> <span m="1147645">let's</span> <span m="1147900">say,</span>
  <span m="1148290">0-1</span> <span m="1148800">loss,</span> <span m="1149070">but</span>
  <span m="1149370">you</span> <span m="1149530">might</span> <span m="1149760">also</span>
  <span m="1149970">be</span> <span m="1150060">interested</span> <span m="1150570">in</span>
  <span m="1151740">trading</span> <span m="1152250">off,</span> <span m="1152630">let's</span>
  <span m="1152780">say,</span> <span m="1152910">false</span> <span m="1153210">positives</span>
  <span m="1153750">for</span> <span m="1153840">false</span> <span m="1154140">negatives.</span>
  <span m="1155130">And</span> <span m="1155220">so</span> <span m="1155310">you</span>
  <span m="1155400">might</span> <span m="1155580">choose</span> <span m="1156000">different</span>
  <span m="1156360">thresholds.</span> <span m="1157580">And</span> <span m="1157680">you</span>
  <span m="1157740">might</span> <span m="1157860">want</span> <span m="1157980">to</span>
  <span m="1158040">quantify</span> <span m="1159450">how</span> <span m="1159810">do</span>
  <span m="1159960">those</span> <span m="1160170">trade-offs</span> <span m="1160590">look</span>
  <span m="1160860">for</span> <span m="1161010">different</span> <span m="1161310">choices</span>
  <span m="1161730">of</span> <span m="1161790">those</span> <span m="1162060">thresholds</span>
  <span m="1162660">of</span> <span m="1162750">this</span> <span m="1162870">continuous</span>
  <span m="1163380">value</span> <span m="1163710">prediction.</span> <span m="1164740">And</span>
  <span m="1164840">that's</span> <span m="1164880">what</span> <span m="1165000">the</span>
  <span m="1165090">ROC</span> <span m="1165390">curve</span> <span m="1165640">will</span>
  <span m="1165810">show</span> <span m="1166020">you.</span></p><p><span m="1166620">So</span>
  <span m="1166830">as</span> <span m="1167040">you</span> <span m="1167130">move</span>
  <span m="1167460">along</span> <span m="1167790">the</span> <span m="1167910">threshold,</span>
  <span m="1168630">you</span> <span m="1168720">can</span> <span m="1168870">compute,</span>
  <span m="1169260">for</span> <span m="1169410">every</span> <span m="1169620">single</span>
  <span m="1169920">threshold,</span> <span m="1170460">what</span> <span m="1170640">is</span>
  <span m="1170760">the</span> <span m="1170910">true</span> <span m="1171150">positive</span>
  <span m="1171540">rate,</span> <span m="1171750">and what</span> <span m="1171810">is</span>
  <span m="1171990">the</span> <span m="1172050">false</span> <span m="1172320">positive</span>
  <span m="1172620">rate.</span> <span m="1173260">And</span> <span m="1173360">that</span>
  <span m="1173400">gives</span> <span m="1173700">you</span> <span m="1173820">a</span>
  <span m="1173910">number.</span> <span m="1175080">And</span> <span m="1175170">you</span>
  <span m="1175230">try</span> <span m="1175470">all</span> <span m="1175620">possible</span>
  <span m="1175920">thresholds,</span> <span m="1176550">that</span> <span m="1176760">gives</span>
  <span m="1177030">you</span> <span m="1177150">a</span> <span m="1177210">curve.</span>
  <span m="1178470">And</span> <span m="1178560">then</span> <span m="1178650">you</span>
  <span m="1178740">can</span> <span m="1178860">compare</span> <span m="1180570">curves</span>
  <span m="1180960">from</span> <span m="1181110">different</span> <span m="1181500">machine</span>
  <span m="1181800">learning</span> <span m="1182190">algorithms.</span></p><p><span
  m="1183250">For</span> <span m="1183270">example,</span> <span m="1183630">here,</span>
  <span m="1184350">I'm</span> <span m="1184500">showing</span> <span m="1184770">you,</span>
  <span m="1184890">in</span> <span m="1185040">the</span> <span m="1185160">green</span>
  <span m="1185580">line,</span> <span m="1186330">the</span> <span m="1187170">predictive</span>
  <span m="1187620">model</span> <span m="1188190">obtained</span> <span m="1188610">by</span>
  <span m="1188760">using</span> <span m="1189270">what</span> <span m="1189450">we're</span>
  <span m="1189540">calling</span> <span m="1189810">the</span> <span m="1189900">traditional</span>
  <span m="1190530">risk</span> <span m="1190800">factors,</span> <span m="1191310">so</span>
  <span m="1191730">something</span> <span m="1192060">like</span> <span m="1192270">eight</span>
  <span m="1192570">or</span> <span m="1192690">10</span> <span m="1193080">different</span>
  <span m="1194610">risk</span> <span m="1194940">factors</span> <span m="1195570">for</span>
  <span m="1195840">type</span> <span m="1196020">2</span> <span m="1196110">diabetes</span>
  <span m="1196620">that</span> <span m="1196740">are</span> <span m="1196860">very</span>
  <span m="1197190">commonly</span> <span m="1197640">used</span> <span m="1197880">in</span>
  <span m="1197970">the</span> <span m="1198030">literature.</span> <span m="1199050">Versus</span>
  <span m="1199410">in</span> <span m="1199530">blue,</span> <span m="1200070">it's</span>
  <span m="1200220">showing</span> <span m="1200580">you</span> <span m="1200700">what</span>
  <span m="1200850">you'd</span> <span m="1201000">get</span> <span m="1201280">if</span>
  <span m="1201300">you</span> <span m="1201390">just</span> <span m="1201660">used</span>
  <span m="1202400">a</span> <span m="1202680">naive</span> <span m="1203340">L1-regularized</span>
  <span m="1204630">logistic</span> <span m="1204990">regression</span> <span m="1205380">model</span>
  <span m="1206100">with</span> <span m="1206490">no</span> <span m="1206700">domain</span>
  <span m="1207030">knowledge,</span> <span m="1207430">just</span> <span m="1207530">sort</span>
  <span m="1207690">of</span> <span m="1207810">throw</span> <span m="1208100">in</span>
  <span m="1208200">the</span> <span m="1208260">bag</span> <span m="1208390">of </span>
  <span m="1208530">features.</span></p><p><span m="1210660">And</span> <span m="1210780">you</span>
  <span m="1210870">want</span> <span m="1211110">to</span> <span m="1211170">be</span>
  <span m="1211350">up</span> <span m="1211500">there.</span> <span m="1212010">You</span>
  <span m="1212100">want</span> <span m="1212310">to</span> <span m="1212370">be</span>
  <span m="1212700">in</span> <span m="1212790">that</span> <span m="1212940">top</span>
  <span m="1213420">left</span> <span m="1213810">corner.</span> <span m="1215530">That's</span>
  <span m="1215700">the</span> <span m="1215790">goal</span> <span m="1216030">here.</span>
  <span m="1216640">So</span> <span m="1216840">you</span> <span m="1216960">would</span>
  <span m="1217080">like</span> <span m="1217670">that</span> <span m="1217820">blue</span>
  <span m="1218040">curve</span> <span m="1218280">to</span> <span m="1218370">be</span>
  <span m="1218520">up</span> <span m="1218730">there,</span> <span m="1219310">and</span>
  <span m="1219410">then</span> <span m="1219450">all</span> <span m="1219600">the</span>
  <span m="1219660">way</span> <span m="1219840">to</span> <span m="1219990">the</span>
  <span m="1220080">right.</span></p><p><span m="1222360">Now,</span> <span m="1222960">one</span>
  <span m="1223200">way</span> <span m="1223290">to</span> <span m="1223410">try</span>
  <span m="1223650">to</span> <span m="1224070">quantify</span> <span m="1225810">in</span>
  <span m="1226230">a</span> <span m="1226320">single</span> <span m="1226950">number</span>
  <span m="1227940">how</span> <span m="1228270">useful</span> <span m="1229080">any</span>
  <span m="1229350">one</span> <span m="1229710">ROC</span> <span m="1230310">curve</span>
  <span m="1230910">is</span> <span m="1231255">is</span> <span m="1231600">by</span>
  <span m="1231750">looking</span> <span m="1232170">at</span> <span m="1232350">what's</span>
  <span m="1232560">called</span> <span m="1232770">the</span> <span m="1233100">area</span>
  <span m="1233730">under</span> <span m="1233940">the</span> <span m="1234030">ROC</span>
  <span m="1234360">curve.</span> <span m="1234960">And</span> <span m="1235050">mathematically,</span>
  <span m="1235335">this</span> <span m="1235620">is</span> <span m="1235680">exactly</span>
  <span m="1236070">what</span> <span m="1236160">you'd</span> <span m="1236280">expect.</span>
  <span m="1237870">This</span> <span m="1238230">area</span> <span m="1239880">is</span>
  <span m="1240570">the</span> <span m="1240720">area</span> <span m="1241050">under</span>
  <span m="1241120">the</span> <span m="1241170">ROC</span> <span m="1241530">curve.</span>
  <span m="1242340">So</span> <span m="1242460">you</span> <span m="1242520">could
  just</span> <span m="1242730">integrate</span> <span m="1243150">the</span> <span
  m="1243240">curve,</span> <span m="1244170">and</span> <span m="1244290">you</span>
  <span m="1244380">get</span> <span m="1244500">that</span> <span m="1244680">number</span>
  <span m="1245010">out.</span> <span m="1246570">Now,</span> <span m="1246960">remember,</span>
  <span m="1247230">I</span> <span m="1247290">told</span> <span m="1247500">you</span>
  <span m="1247560">you</span> <span m="1247650">want</span> <span m="1247800">to</span>
  <span m="1247860">be</span> <span m="1247980">in</span> <span m="1248070">the</span>
  <span m="1249570">upper</span> <span m="1249780">left</span> <span m="1249990">quadrant.</span>
  <span m="1250680">And</span> <span m="1250800">so</span> <span m="1251100">the</span>
  <span m="1251220">goal</span> <span m="1251590">was</span> <span m="1251760">to</span>
  <span m="1251850">get</span> <span m="1251970">an</span> <span m="1252060">area</span>
  <span m="1252540">under</span> <span m="1252840">the</span> <span m="1252960">ROC</span>
  <span m="1253290">curve</span> <span m="1253730">of</span> <span m="1253900">a</span>
  <span m="1254010">1.</span></p><p><span m="1256110">Now,</span> <span m="1256680">what</span>
  <span m="1256890">would</span> <span m="1257040">a</span> <span m="1257550">random</span>
  <span m="1258540">prediction</span> <span m="1259410">give</span> <span m="1259680">you?</span>
  <span m="1260600">Any</span> <span m="1260760">idea?</span> <span m="1261430">So</span>
  <span m="1261540">if</span> <span m="1261630">you're</span> <span m="1261740">to</span>
  <span m="1261830">just</span> <span m="1262020">flip</span> <span m="1262470">a</span>
  <span m="1262530">coin</span> <span m="1264360">and</span> <span m="1264720">guess--</span>
  <span m="1266730">what do</span> <span m="1266820">you</span> <span m="1266880">think?</span></p><p><span
  m="1267060">AUDIENCE:</span> <span m="1267210">0.5.</span></p><p><span m="1267660">PROFESSOR:</span>
  <span m="1267870">0.5?</span></p><p><span m="1269940">AUDIENCE:</span> <span m="1270180">[INAUDIBLE]</span></p><p><span
  m="1272340">PROFESSOR:</span> <span m="1272445">Well,</span> <span m="1272550">so</span>
  <span m="1273060">I</span> <span m="1273270">was</span> <span m="1273390">a</span>
  <span m="1273480">little</span> <span m="1273630">bit</span> <span m="1274320">misleading</span>
  <span m="1274950">when</span> <span m="1275070">I</span> <span m="1275160">said</span>
  <span m="1275370">you just</span> <span m="1275570">flip</span> <span m="1275690">a</span>
  <span m="1275790">coin.</span> <span m="1276210">You</span> <span m="1276260">got</span>
  <span m="1276340">to</span> <span m="1276420">flip</span> <span m="1276690">a</span>
  <span m="1276720">coin</span> <span m="1277110">with</span> <span m="1277440">sort</span>
  <span m="1277620">of</span> <span m="1277680">different</span> <span m="1280830">noise</span>
  <span m="1281190">rates.</span> <span m="1282210">And</span> <span m="1282450">each</span>
  <span m="1282660">one</span> <span m="1282780">of</span> <span m="1282840">those</span>
  <span m="1282990">will</span> <span m="1283080">get</span> <span m="1283230">you</span>
  <span m="1283320">sort</span> <span m="1283470">of</span> <span m="1283530">a</span>
  <span m="1283590">different</span> <span m="1283860">place</span> <span m="1284070">along</span>
  <span m="1284280">this</span> <span m="1284430">curve.</span> <span m="1285970">And</span>
  <span m="1286620">if</span> <span m="1286740">you</span> <span m="1286800">look</span>
  <span m="1286950">at</span> <span m="1287040">the</span> <span m="1287130">curve</span>
  <span m="1287880">that</span> <span m="1288000">you</span> <span m="1288120">get</span>
  <span m="1288360">from</span> <span m="1288630">these</span> <span m="1289170">random</span>
  <span m="1289710">guesses,</span> <span m="1290310">it's</span> <span m="1290490">going</span>
  <span m="1290570">to</span> <span m="1290670">be</span> <span m="1290800">the</span>
  <span m="1290880">straight</span> <span m="1291240">line</span> <span m="1291600">from</span>
  <span m="1291900">0</span> <span m="1292290">to</span> <span m="1292440">1.</span>
  <span m="1292740">And</span> <span m="1292830">as</span> <span m="1293010">you</span>
  <span m="1293100">said,</span> <span m="1293820">that will then</span> <span m="1294290">have</span>
  <span m="1294540">an</span> <span m="1294930">AUC</span> <span m="1295590">of</span>
  <span m="1295740">0.5.</span> <span m="1297040">So</span> <span m="1297170">0.5</span>
  <span m="1297810">is</span> <span m="1297900">going to</span> <span m="1298020">be</span>
  <span m="1298080">random</span> <span m="1298320">guessing.</span> <span m="1298800">1</span>
  <span m="1299160">is</span> <span m="1299280">perfect.</span> <span m="1299970">And</span>
  <span m="1300300">your</span> <span m="1300450">algorithm</span> <span m="1300860">is</span>
  <span m="1300930">going to</span> <span m="1301020">be</span> <span m="1301130">somewhere</span>
  <span m="1301470">in</span> <span m="1301560">between.</span></p><p><span m="1304860">Now,</span>
  <span m="1305750">of</span> <span m="1306000">relevance</span> <span m="1306480">to</span>
  <span m="1306600">the</span> <span m="1306930">rest</span> <span m="1307380">of</span>
  <span m="1307470">today's</span> <span m="1307740">lecture</span> <span m="1308550">is</span>
  <span m="1308670">going</span> <span m="1308910">to</span> <span m="1309000">be</span>
  <span m="1309090">an</span> <span m="1309180">alternative</span> <span m="1309840">definition--</span>
  <span m="1310890">alternative</span> <span m="1311520">way</span> <span m="1312030">of</span>
  <span m="1312540">computing</span> <span m="1313200">the</span> <span m="1313320">area</span>
  <span m="1313550">under</span> <span m="1313710">the</span> <span m="1313920">ROC</span>
  <span m="1314340">curve.</span> <span m="1315000">So</span> <span m="1315180">one</span>
  <span m="1315420">way</span> <span m="1315540">to</span> <span m="1315630">compute</span>
  <span m="1315990">it</span> <span m="1316440">is</span> <span m="1316590">literally</span>
  <span m="1316890">as</span> <span m="1316980">I</span> <span m="1317070">said.</span>
  <span m="1317340">You</span> <span m="1318120">create</span> <span m="1318480">that</span>
  <span m="1318630">curve,</span> <span m="1319020">and</span> <span m="1319140">you</span>
  <span m="1319410">integrate</span> <span m="1319860">to</span> <span m="1319980">get</span>
  <span m="1320100">the</span> <span m="1320270">area</span> <span m="1320790">under</span>
  <span m="1321060">it.</span> <span m="1321960">But</span> <span m="1322620">one</span>
  <span m="1322860">can</span> <span m="1322980">show</span> <span m="1323130">mathematically--</span>
  <span m="1323700">I'm not</span> <span m="1323790">going</span> <span m="1323850">to</span>
  <span m="1323970">give</span> <span m="1324090">you</span> <span m="1324150">the</span>
  <span m="1324210">derivation</span> <span m="1324660">here,</span> <span m="1324900">but</span>
  <span m="1325020">you</span> <span m="1325080">can</span> <span m="1325200">look</span>
  <span m="1325320">it</span> <span m="1325380">up</span> <span m="1325470">on</span>
  <span m="1325560">Wikipedia.</span> <span m="1326550">One</span> <span m="1326790">can</span>
  <span m="1326970">show</span> <span m="1327150">mathematically</span> <span m="1327930">that</span>
  <span m="1328140">an</span> <span m="1328260">equivalent</span> <span m="1329550">way</span>
  <span m="1329820">of</span> <span m="1329910">computing</span> <span m="1330390">the</span>
  <span m="1330510">area</span> <span m="1330870">under</span> <span m="1331110">the</span>
  <span m="1331230">ROC</span> <span m="1331710">curve</span> <span m="1332670">is</span>
  <span m="1332820">to</span> <span m="1332940">compute</span> <span m="1333360">the</span>
  <span m="1333450">probability</span> <span m="1334740">that</span> <span m="1334890">an</span>
  <span m="1335010">algorithm</span> <span m="1335490">will</span> <span m="1335610">rank</span>
  <span m="1336150">a</span> <span m="1336210">positive-labeled</span> <span m="1337350">patient</span>
  <span m="1337770">over</span> <span m="1338010">a</span> <span m="1338040">negative-labeled</span>
  <span m="1338880">patient.</span></p><p><span m="1340510">So</span> <span m="1341070">mathematically</span>
  <span m="1341760">what</span> <span m="1341850">I'm</span> <span m="1341910">talking</span>
  <span m="1342150">about</span> <span m="1342300">is</span> <span m="1342360">the</span>
  <span m="1342420">following</span> <span m="1342810">thing.</span> <span m="1343760">You're</span>
  <span m="1343940">going</span> <span m="1344090">to</span> <span m="1344160">sum</span>
  <span m="1345870">over</span> <span m="1346440">pairs</span> <span m="1346860">of</span>
  <span m="1346920">patients</span> <span m="1348360">where--</span> <span m="1349530">I'm</span>
  <span m="1349590">going</span> <span m="1349710">to</span> <span m="1349770">call</span>
  <span m="1351840">x1</span> <span m="1353490">is</span> <span m="1353970">a</span>
  <span m="1354030">patient</span> <span m="1354600">with</span> <span m="1355080">label</span>
  <span m="1355860">y1</span> <span m="1356730">equals</span> <span m="1357480">1.</span>
  <span m="1358470">And</span> <span m="1358680">x2</span> <span m="1359610">is</span>
  <span m="1359760">a</span> <span m="1359820">patient</span> <span m="1360390">with</span>
  <span m="1360630">label</span> <span m="1361290">y--</span> <span m="1364050">actually,</span>
  <span m="1364140">I'll</span> <span m="1364320">call</span> <span m="1364530">it--</span>
  <span m="1365520">yeah,</span> <span m="1366720">with</span> <span m="1366900">label</span>
  <span m="1367350">x2</span> <span m="1367780">equals</span> <span m="1368340">1.</span>
  <span m="1368790">So</span> <span m="1368940">these</span> <span m="1369120">are</span>
  <span m="1369300">two</span> <span m="1369600">different</span> <span m="1369960">patients.</span></p><p><span
  m="1373360">I</span> <span m="1373420">think I'm</span> <span m="1373570">going</span>
  <span m="1373690">to</span> <span m="1373750">rewrite</span> <span m="1374050">it</span>
  <span m="1374110">like</span> <span m="1374230">this--</span> <span m="1374560">xi</span>
  <span m="1375670">and</span> <span m="1376090">xj,</span> <span m="1377320">just</span>
  <span m="1377770">for</span> <span m="1377890">generality's</span> <span m="1378690">sake.</span>
  <span m="1379960">So</span> <span m="1380350">we're</span> <span m="1380440">going</span>
  <span m="1380520">to</span> <span m="1380590">sum</span> <span m="1380860">this</span>
  <span m="1381070">up</span> <span m="1381270">over</span> <span m="1381450">all</span>
  <span m="1381760">choices</span> <span m="1382180">of</span> <span m="1384190">i</span>
  <span m="1384520">and</span> <span m="1384670">j</span> <span m="1385540">such</span>
  <span m="1385840">that</span> <span m="1386980">yi</span> <span m="1387850">and</span>
  <span m="1388000">yj</span> <span m="1388750">have</span> <span m="1389500">different</span>
  <span m="1390010">labels.</span> <span m="1390580">So</span> <span m="1390730">that</span>
  <span m="1390830">should</span> <span m="1391000">say</span> <span m="1391410">yj</span>
  <span m="1391690">equals</span> <span m="1392070">0.</span></p><p><span m="1393070">And</span>
  <span m="1393160">then</span> <span m="1393270">you're</span> <span m="1393350">going</span>
  <span m="1393440">to</span> <span m="1393520">look</span> <span m="1393760">at--</span>
  <span m="1394390">what</span> <span m="1395020">you</span> <span m="1395110">want</span>
  <span m="1395350">to</span> <span m="1395440">happen,</span> <span m="1396070">like</span>
  <span m="1396250">suppose</span> <span m="1396670">that</span> <span m="1396790">you're</span>
  <span m="1397000">using</span> <span m="1397270">a</span> <span m="1397330">linear</span>
  <span m="1397630">model</span> <span m="1397960">here.</span> <span m="1398290">So</span>
  <span m="1398590">your</span> <span m="1398710">prediction</span> <span m="1399160">is</span>
  <span m="1399280">given</span> <span m="1399550">to</span> <span m="1399700">you</span>
  <span m="1399880">by,</span> <span m="1401320">let's</span> <span m="1401500">say,</span>
  <span m="1402310">w.xj.</span> <span m="1410020">What</span> <span m="1410170">you</span>
  <span m="1410260">want</span> <span m="1410680">is</span> <span m="1410830">that</span>
  <span m="1411010">this</span> <span m="1411580">should</span> <span m="1411760">be</span>
  <span m="1411880">smaller</span> <span m="1412990">than</span> <span m="1413230">w.xi.</span>
  <span m="1417850">So</span> <span m="1419080">the</span> <span m="1419320">j</span>
  <span m="1420130">data</span> <span m="1420430">point,</span> <span m="1420760">remember,</span>
  <span m="1421180">was</span> <span m="1421540">the</span> <span m="1421630">one</span>
  <span m="1422140">that</span> <span m="1422290">got</span> <span m="1422440">the</span>
  <span m="1422580">0-th</span> <span m="1423820">and</span> <span m="1423950">the</span>
  <span m="1424120">i-th</span> <span m="1424480">data</span> <span m="1424690">point</span>
  <span m="1424990">is</span> <span m="1425140">the</span> <span m="1425230">one</span>
  <span m="1425470">that</span> <span m="1425620">got</span> <span m="1425860">the</span>
  <span m="1425980">1</span> <span m="1426280">label.</span> <span m="1427430">So</span>
  <span m="1427480">we</span> <span m="1427540">want</span> <span m="1427720">the</span>
  <span m="1427870">score</span> <span m="1431110">of</span> <span m="1431230">the</span>
  <span m="1431290">data</span> <span m="1431470">point</span> <span m="1431590">that</span>
  <span m="1431680">should've</span> <span m="1431840">been</span> <span m="1431950">1</span>
  <span m="1432460">to</span> <span m="1432580">be</span> <span m="1432700">higher</span>
  <span m="1433240">than</span> <span m="1433390">the</span> <span m="1433480">score</span>
  <span m="1434110">of</span> <span m="1434230">the</span> <span m="1434800">data</span>
  <span m="1435040">point</span> <span m="1435340">which</span> <span m="1435640">should've</span>
  <span m="1435880">gotten</span> <span m="1436060">the</span> <span m="1436150">label</span>
  <span m="1436390">0.</span> <span m="1437290">And</span> <span m="1437380">you just</span>
  <span m="1437560">count</span> <span m="1438070">up--</span> <span m="1438280">this
  is</span> <span m="1438400">an</span> <span m="1438490">indicator</span> <span m="1438850">function.</span>
  <span m="1438950">You just</span> <span m="1439330">count</span> <span m="1439660">up</span>
  <span m="1439810">how</span> <span m="1439990">many</span> <span m="1440230">of</span>
  <span m="1440290">those</span> <span m="1440500">were</span> <span m="1440650">correctly</span>
  <span m="1441310">ordered.</span> <span m="1442330">And</span> <span m="1442450">then</span>
  <span m="1443230">you're</span> <span m="1443320">just</span> <span m="1443470">going</span>
  <span m="1443550">to</span> <span m="1443620">normalize</span> <span m="1444190">by</span>
  <span m="1444310">the</span> <span m="1444400">total</span> <span m="1444700">number</span>
  <span m="1445900">of</span> <span m="1446020">comparisons</span> <span m="1446590">that</span>
  <span m="1446710">you</span> <span m="1446800">do.</span> <span m="1447850">And</span>
  <span m="1447940">it</span> <span m="1448000">turns</span> <span m="1448270">out</span>
  <span m="1448360">that</span> <span m="1448480">that</span> <span m="1448690">is</span>
  <span m="1448840">exactly</span> <span m="1449380">equal</span> <span m="1449710">to</span>
  <span m="1449830">the</span> <span m="1449920">area</span> <span m="1450130">under</span>
  <span m="1450280">the</span> <span m="1450370">ROC</span> <span m="1450700">curve.</span>
  <span m="1451450">And</span> <span m="1451540">it</span> <span m="1451630">really</span>
  <span m="1451810">makes</span> <span m="1452080">clear</span> <span m="1452470">that</span>
  <span m="1452620">this</span> <span m="1452830">is</span> <span m="1452920">a</span>
  <span m="1452980">notion</span> <span m="1453400">that</span> <span m="1453550">really</span>
  <span m="1453850">cares</span> <span m="1454210">about</span> <span m="1454540">ranking.</span>
  <span m="1455320">Are</span> <span m="1455410">you</span> <span m="1455500">getting</span>
  <span m="1455740">the</span> <span m="1455830">ranking</span> <span m="1457720">of</span>
  <span m="1458710">patients</span> <span m="1459370">correct?</span> <span m="1460630">Are</span>
  <span m="1460720">you</span> <span m="1460870">ranking</span> <span m="1461500">the</span>
  <span m="1461620">ones</span> <span m="1462040">who</span> <span m="1462640">should</span>
  <span m="1462880">have</span> <span m="1462970">been</span> <span m="1463510">given</span>
  <span m="1463840">1</span> <span m="1464830">higher</span> <span m="1465190">than</span>
  <span m="1465340">the</span> <span m="1465430">ones</span> <span m="1465670">that</span>
  <span m="1465850">should</span> <span m="1466050">have</span> <span m="1466180">gotten</span>
  <span m="1466360">the</span> <span m="1466420">label</span> <span m="1466690">0.</span></p><p><span
  m="1468490">And</span> <span m="1469150">importantly,</span> <span m="1470470">this</span>
  <span m="1470740">whole</span> <span m="1470980">measure</span> <span m="1471520">is</span>
  <span m="1471820">actually</span> <span m="1472270">invariant</span> <span m="1473110">to</span>
  <span m="1473380">the</span> <span m="1473500">label</span> <span m="1473920">imbalance.</span>
  <span m="1475240">So</span> <span m="1475480">you</span> <span m="1475600">might</span>
  <span m="1475720">have</span> <span m="1475870">a</span> <span m="1475900">very</span>
  <span m="1476290">imbalanced</span> <span m="1476880">data</span> <span m="1477260">set.</span>
  <span m="1478300">But</span> <span m="1479590">if</span> <span m="1479740">you</span>
  <span m="1479830">were</span> <span m="1479920">to</span> <span m="1480070">re-sample</span>
  <span m="1480850">with</span> <span m="1481030">now</span> <span m="1481210">making</span>
  <span m="1481480">it</span> <span m="1482140">a</span> <span m="1482230">balanced</span>
  <span m="1482750">data</span> <span m="1482990">set,</span> <span m="1483250">your</span>
  <span m="1483440">AUC</span> <span m="1483910">of</span> <span m="1484060">your</span>
  <span m="1484150">predictive</span> <span m="1484450">model</span> <span m="1484720">wouldn't</span>
  <span m="1484990">change.</span> <span m="1486350">And</span> <span m="1486580">that's</span>
  <span m="1486760">a</span> <span m="1486820">nice</span> <span m="1487210">property</span>
  <span m="1487630">to</span> <span m="1487750">have</span> <span m="1488500">when</span>
  <span m="1488710">it</span> <span m="1488770">comes</span> <span m="1489190">to</span>
  <span m="1490210">evaluating</span> <span m="1491050">settings</span> <span m="1492040">where</span>
  <span m="1492310">you</span> <span m="1492430">might</span> <span m="1492580">have</span>
  <span m="1492760">artificially</span> <span m="1493570">created</span> <span m="1495160">a</span>
  <span m="1495220">balanced</span> <span m="1495640">data</span> <span m="1495860">set</span>
  <span m="1496090">for</span> <span m="1496270">computational</span> <span m="1496960">concerns.</span>
  <span m="1497590">Even</span> <span m="1497890">though</span> <span m="1498070">the</span>
  <span m="1498160">true</span> <span m="1498460">setting</span> <span m="1498820">is</span>
  <span m="1499000">imbalanced,</span> <span m="1500110">there</span> <span m="1500350">at</span>
  <span m="1500440">least</span> <span m="1500680">you</span> <span m="1500740">know</span>
  <span m="1500890">that</span> <span m="1500980">the</span> <span m="1501070">numbers</span>
  <span m="1501370">are</span> <span m="1501400">going</span> <span m="1501460">to</span>
  <span m="1501520">be</span> <span m="1501580">the</span> <span m="1501670">same</span>
  <span m="1501940">in</span> <span m="1502030">both</span> <span m="1502210">settings.</span></p><p><span
  m="1503230">On</span> <span m="1503300">the</span> <span m="1503340">other</span>
  <span m="1503500">hand,</span> <span m="1503710">it also</span> <span m="1503920">has</span>
  <span m="1504100">lots</span> <span m="1504280">of</span> <span m="1504340">disadvantages.</span>
  <span m="1505120">Because</span> <span m="1505360">often</span> <span m="1505720">you</span>
  <span m="1505810">don't</span> <span m="1505930">care</span> <span m="1506260">about</span>
  <span m="1506560">the</span> <span m="1506650">performance</span> <span m="1507310">of</span>
  <span m="1507490">the</span> <span m="1507640">whole</span> <span m="1507940">entire</span>
  <span m="1508330">curve.</span> <span m="1509350">Often</span> <span m="1509650">you</span>
  <span m="1509740">care</span> <span m="1510010">about</span> <span m="1510760">particular</span>
  <span m="1511240">parts</span> <span m="1511600">along</span> <span m="1511840">the</span>
  <span m="1511930">curve.</span> <span m="1512780">So</span> <span m="1512860">for</span>
  <span m="1512980">example,</span> <span m="1514680">in</span> <span m="1514870">last</span>
  <span m="1515140">week's</span> <span m="1515320">lecture,</span> <span m="1516130">I</span>
  <span m="1516280">argued</span> <span m="1516850">that</span> <span m="1517420">really</span>
  <span m="1518380">what</span> <span m="1518560">we</span> <span m="1518680">often</span>
  <span m="1519040">care</span> <span m="1519250">about</span> <span m="1519400">is</span>
  <span m="1519520">just</span> <span m="1519670">the</span> <span m="1519760">positive</span>
  <span m="1520240">predictive</span> <span m="1520600">value</span> <span m="1520900">for</span>
  <span m="1521050">a</span> <span m="1521110">particular</span> <span m="1521590">threshold.</span>
  <span m="1522780">And</span> <span m="1522910">we</span> <span m="1523000">want</span>
  <span m="1523180">that</span> <span m="1523330">to</span> <span m="1523420">be</span>
  <span m="1523510">as</span> <span m="1523600">high</span> <span m="1523750">as</span>
  <span m="1523870">possible</span> <span m="1524350">for</span> <span m="1524650">as</span>
  <span m="1524890">few</span> <span m="1525190">people</span> <span m="1525430">as</span>
  <span m="1525520">possible.</span> <span m="1526020">Like,</span> <span m="1526570">find
  the</span> <span m="1526870">100</span> <span m="1527290">most</span> <span m="1527560">risky</span>
  <span m="1527860">people,</span> <span m="1528540">and</span> <span m="1528640">look</span>
  <span m="1528790">at</span> <span m="1528850">what</span> <span m="1529000">fraction</span>
  <span m="1529480">of</span> <span m="1529540">them</span> <span m="1529690">actually</span>
  <span m="1530140">developed</span> <span m="1530620">type</span> <span m="1530860">2</span>
  <span m="1530980">diabetes.</span> <span m="1532270">And</span> <span m="1532390">that</span>
  <span m="1532630">setting,</span> <span m="1532930">what</span> <span m="1533050">you're</span>
  <span m="1533140">really</span> <span m="1533350">looking</span> <span m="1533620">at</span>
  <span m="1533740">is</span> <span m="1533890">this</span> <span m="1534160">part</span>
  <span m="1534430">of</span> <span m="1534490">the</span> <span m="1534580">curve.</span></p><p><span
  m="1535580">And</span> <span m="1535600">so</span> <span m="1536080">it</span> <span
  m="1536140">turns</span> <span m="1536350">out</span> <span m="1536470">there</span>
  <span m="1536620">are</span> <span m="1538090">generalizations</span> <span m="1538960">of</span>
  <span m="1539140">area</span> <span m="1539350">under</span> <span m="1539500">the</span>
  <span m="1539560">curve</span> <span m="1539950">that</span> <span m="1540100">focus</span>
  <span m="1540940">on</span> <span m="1541270">parts</span> <span m="1541690">of</span>
  <span m="1541750">the</span> <span m="1541870">curve.</span> <span m="1542510">And</span>
  <span m="1542650">that</span> <span m="1542770">goes</span> <span m="1542920">by</span>
  <span m="1543010">the</span> <span m="1543070">name</span> <span m="1543250">of</span>
  <span m="1543370">partial</span> <span m="1544090">AUC.</span> <span m="1544930">For</span>
  <span m="1545020">example,</span> <span m="1545420">if</span> <span m="1545520">you</span>
  <span m="1545620">just</span> <span m="1545680">integrated</span> <span m="1546250">from</span>
  <span m="1546460">0</span> <span m="1547120">to,</span> <span m="1547330">let's</span>
  <span m="1547480">say,</span> <span m="1548020">0.1</span> <span m="1549280">of</span>
  <span m="1549430">the</span> <span m="1549520">curve,</span> <span m="1550340">then</span>
  <span m="1550900">you</span> <span m="1551020">could</span> <span m="1551140">still</span>
  <span m="1551380">get</span> <span m="1551500">a</span> <span m="1551560">number</span>
  <span m="1551830">to</span> <span m="1551920">compare</span> <span m="1552280">two</span>
  <span m="1552460">different</span> <span m="1552700">curves,</span> <span m="1553220">but</span>
  <span m="1553320">it's</span> <span m="1553480">focusing</span> <span m="1553990">on</span>
  <span m="1554080">the</span> <span m="1554170">area</span> <span m="1554440">of</span>
  <span m="1554490">that</span> <span m="1554590">curve</span> <span m="1554800">that's</span>
  <span m="1554950">actually</span> <span m="1555220">relevant</span> <span m="1555640">for</span>
  <span m="1555790">your</span> <span m="1555880">predictive</span> <span m="1556240">purposes,</span>
  <span m="1557070">for</span> <span m="1557200">your</span> <span m="1557320">task</span>
  <span m="1558100">at</span> <span m="1558310">hand.</span></p><p><span m="1560510">So</span>
  <span m="1562180">that's</span> <span m="1562420">all</span> <span m="1562510">I</span>
  <span m="1562570">want</span> <span m="1562720">to</span> <span m="1562810">say</span>
  <span m="1562960">about</span> <span m="1563490">receiver-operator</span> <span
  m="1564340">characteristic</span> <span m="1564880">curves.</span> <span m="1565330">Any</span>
  <span m="1565540">questions?</span> <span m="1568330">Yep.</span></p><p><span m="1568400">AUDIENCE:</span>
  <span m="1568620">Could</span> <span m="1568840">you talk</span> <span m="1569280">more</span>
  <span m="1569480">about</span> <span m="1570110">what</span> <span m="1570560">the</span>
  <span m="1570680">drawbacks</span> <span m="1571220">were</span> <span m="1571950">of</span>
  <span m="1572520">using</span> <span m="1572950">this.</span> <span m="1573570">Does</span>
  <span m="1573800">the class</span> <span m="1574165">imbalance--</span> <span m="1574530">is
  the</span> <span m="1574800">class</span> <span m="1575030">imbalance,</span> <span
  m="1575370">then, always</span> <span m="1575850">a positive effect?</span></p><p><span
  m="1577290">PROFESSOR:</span> <span m="1577490">So</span> <span m="1578960">the</span>
  <span m="1579020">thing</span> <span m="1579230">is,</span> <span m="1579320">when</span>
  <span m="1579860">you</span> <span m="1579920">want</span> <span m="1580070">to</span>
  <span m="1580190">use</span> <span m="1580580">this</span> <span m="1581030">approach,</span>
  <span m="1583850">depending</span> <span m="1584240">on</span> <span m="1584360">how</span>
  <span m="1584540">you're</span> <span m="1584690">using</span> <span m="1584940">the</span>
  <span m="1585070">[INAUDIBLE],</span> <span m="1585500">you</span> <span m="1585770">might</span>
  <span m="1585950">not</span> <span m="1586100">be</span> <span m="1586160">able</span>
  <span m="1586280">to</span> <span m="1586370">tolerate</span> <span m="1587030">a</span>
  <span m="1587780">0.8</span> <span m="1588410">false</span> <span m="1588650">positive</span>
  <span m="1589040">rate.</span> <span m="1590400">So</span> <span m="1590480">in</span>
  <span m="1590540">some</span> <span m="1590690">sense,</span> <span m="1591140">what's</span>
  <span m="1591350">going</span> <span m="1591530">on</span> <span m="1591680">in</span>
  <span m="1591770">this</span> <span m="1591950">part</span> <span m="1592130">of</span>
  <span m="1592190">the</span> <span m="1592250">curve</span> <span m="1592610">might</span>
  <span m="1592760">be</span> <span m="1592850">completely</span> <span m="1593420">irrelevant</span>
  <span m="1594680">for</span> <span m="1594920">your</span> <span m="1595580">task.</span>
  <span m="1596960">And</span> <span m="1597080">so</span> <span m="1597590">one</span>
  <span m="1598970">of</span> <span m="1599030">the</span> <span m="1599090">algorithms--</span>
  <span m="1599560">so</span> <span m="1599630">one</span> <span m="1599780">of</span>
  <span m="1599840">these</span> <span m="1599960">curves--</span> <span m="1600320">might</span>
  <span m="1600500">look</span> <span m="1600680">like</span> <span m="1600860">it's</span>
  <span m="1601010">doing</span> <span m="1601280">really,</span> <span m="1601740">really</span>
  <span m="1601910">well</span> <span m="1602150">over</span> <span m="1602330">here,</span>
  <span m="1602750">and</span> <span m="1602840">pretty</span> <span m="1603050">poorly</span>
  <span m="1603410">over</span> <span m="1603560">here.</span> <span m="1603860">But</span>
  <span m="1603980">if</span> <span m="1604070">you're</span> <span m="1604160">looking</span>
  <span m="1604400">at</span> <span m="1604490">the</span> <span m="1604690">full</span>
  <span m="1605660">area</span> <span m="1605930">under</span> <span m="1606080">the</span>
  <span m="1606170">ROC</span> <span m="1606470">curve,</span> <span m="1608210">you</span>
  <span m="1608330">won't</span> <span m="1608450">notice</span> <span m="1608760">that.</span>
  <span m="1609480">And</span> <span m="1609920">so</span> <span m="1610010">that's</span>
  <span m="1610190">one</span> <span m="1610340">of</span> <span m="1610400">the</span>
  <span m="1610490">big</span> <span m="1610640">problems.</span> <span m="1611340">Yeah.</span></p><p><span
  m="1611890">AUDIENCE:</span> <span m="1611937">And</span> <span m="1613870">when</span>
  <span m="1614010">would</span> <span m="1614110">you</span> <span m="1614210">use</span>
  <span m="1614500">this</span> <span m="1614710">versus</span> <span m="1615100">precision</span>
  <span m="1615725">recall</span> <span m="1616170">or--</span></p><p><span m="1616700">PROFESSOR:</span>
  <span m="1616760">Yeah,</span> <span m="1617180">so</span> <span m="1617330">a</span>
  <span m="1617360">lot</span> <span m="1617570">of</span> <span m="1617660">the</span>
  <span m="1617720">community</span> <span m="1618030">is</span> <span m="1618260">interested</span>
  <span m="1618680">in</span> <span m="1619610">precision</span> <span m="1619910">recall</span>
  <span m="1620180">curves.</span> <span m="1620510">And</span> <span m="1621150">precision</span>
  <span m="1621500">recall</span> <span m="1621740">curves,</span> <span m="1621980">as</span>
  <span m="1622160">opposed</span> <span m="1622580">to</span> <span m="1622830">receiver-operator</span>
  <span m="1623510">curves,</span> <span m="1623810">have</span> <span m="1623960">the</span>
  <span m="1624050">property</span> <span m="1624380">that</span> <span m="1624530">they</span>
  <span m="1624650">are</span> <span m="1624770">not</span> <span m="1625940">invariant</span>
  <span m="1626510">to</span> <span m="1626690">class</span> <span m="1626900">imbalance,</span>
  <span m="1628160">which</span> <span m="1628670">in</span> <span m="1628760">many</span>
  <span m="1628940">settings</span> <span m="1629420">is</span> <span m="1629570">of</span>
  <span m="1629660">interest,</span> <span m="1630080">because</span> <span m="1630320">it
  will</span> <span m="1630380">allow</span> <span m="1630620">you</span> <span m="1630710">to</span>
  <span m="1630770">capture</span> <span m="1631130">these</span> <span m="1631280">types</span>
  <span m="1631490">of</span> <span m="1631580">quantities.</span> <span m="1632710">I'm</span>
  <span m="1632840">not</span> <span m="1632940">going</span> <span m="1633080">to</span>
  <span m="1633110">go</span> <span m="1633200">into</span> <span m="1633350">depth</span>
  <span m="1633620">about</span> <span m="1633900">your</span> <span m="1634040">reasons</span>
  <span m="1634590">for</span> <span m="1634610">one</span> <span m="1634790">or</span>
  <span m="1634850">the</span> <span m="1634940">other.</span> <span m="1635300">But</span>
  <span m="1636210">that's</span> <span m="1636410">something</span> <span m="1636620">that</span>
  <span m="1636890">you</span> <span m="1636950">could</span> <span m="1637130">read</span>
  <span m="1637340">up</span> <span m="1637490">about,</span> <span m="1637820">and</span>
  <span m="1638030">I</span> <span m="1638180">encourage</span> <span m="1638510">you</span>
  <span m="1638570">to</span> <span m="1638660">post</span> <span m="1638850">to</span>
  <span m="1638900">Piazza</span> <span m="1639200">about,</span> <span m="1639410">and</span>
  <span m="1639500">we</span> <span m="1639590">have</span> <span m="1639720">discussion</span>
  <span m="1640080">on</span> <span m="1640150">Piazza.</span></p><p><span m="1644630">So</span>
  <span m="1644860">the</span> <span m="1645370">last</span> <span m="1648070">evaluation</span>
  <span m="1648880">quantity</span> <span m="1649300">that I</span> <span m="1649390">want</span>
  <span m="1649540">to</span> <span m="1649630">talk</span> <span m="1649810">about</span>
  <span m="1650080">is</span> <span m="1650260">known</span> <span m="1650490">as</span>
  <span m="1650800">calibration.</span> <span m="1652450">And</span> <span m="1652780">calibration,</span>
  <span m="1653350">as</span> <span m="1653500">I've</span> <span m="1653590">defined</span>
  <span m="1653710">it</span> <span m="1654010">here,</span> <span m="1654310">has</span>
  <span m="1654490">to</span> <span m="1654580">do</span> <span m="1654640">with</span>
  <span m="1654910">binary</span> <span m="1655300">classification</span> <span m="1655900">problems.</span>
  <span m="1658690">Now,</span> <span m="1659290">before</span> <span m="1659620">you</span>
  <span m="1660160">dig</span> <span m="1660460">into</span> <span m="1660670">this</span>
  <span m="1660850">figure,</span> <span m="1661280">which</span> <span m="1661360">I'll</span>
  <span m="1661450">explain</span> <span m="1661750">in</span> <span m="1661840">a</span>
  <span m="1661870">moment,</span> <span m="1662600">let</span> <span m="1662620">me</span>
  <span m="1662680">just</span> <span m="1662800">give</span> <span m="1662950">you</span>
  <span m="1663010">the</span> <span m="1663100">gist</span> <span m="1663460">of</span>
  <span m="1663550">what</span> <span m="1663700">I</span> <span m="1663760">mean</span>
  <span m="1663910">by</span> <span m="1664000">calibration.</span> <span m="1667140">Suppose
  that</span> <span m="1667640">your</span> <span m="1667740">model</span> <span m="1669110">outputs</span>
  <span m="1669450">a</span> <span m="1669480">probability.</span> <span m="1670410">So</span>
  <span m="1670620">you</span> <span m="1670710">do</span> <span m="1670830">logistic</span>
  <span m="1671190">regression.</span> <span m="1671780">You</span> <span m="1671900">get</span>
  <span m="1672030">a</span> <span m="1672090">probability</span> <span m="1672510">out.</span>
  <span m="1673830">And</span> <span m="1675060">your</span> <span m="1675210">model</span>
  <span m="1675480">says,</span> <span m="1675870">for</span> <span m="1677190">these</span>
  <span m="1678330">10</span> <span m="1678660">patients,</span> <span m="1679410">that</span>
  <span m="1679830">their</span> <span m="1680100">likelihood</span> <span m="1680970">of</span>
  <span m="1681990">dying</span> <span m="1682590">in</span> <span m="1682680">the</span>
  <span m="1682740">next</span> <span m="1684270">48</span> <span m="1684750">hours</span>
  <span m="1685410">is</span> <span m="1686400">0.7.</span> <span m="1688890">Suppose</span>
  <span m="1689280">that's</span> <span m="1689490">what</span> <span m="1689610">your</span>
  <span m="1689700">model</span> <span m="1689970">output.</span> <span m="1691770">If</span>
  <span m="1691890">you</span> <span m="1692020">were</span> <span m="1692080">on</span>
  <span m="1692120">the</span> <span m="1692190">receiving</span> <span m="1692820">end</span>
  <span m="1693120">of</span> <span m="1693210">that</span> <span m="1693600">result,</span>
  <span m="1694360">so</span> <span m="1694440">you</span> <span m="1694590">heard</span>
  <span m="1694890">that,</span> <span m="1695040">0.7,</span> <span m="1696690">what</span>
  <span m="1696900">should</span> <span m="1697140">you</span> <span m="1697320">expect</span>
  <span m="1698250">about</span> <span m="1698760">those</span> <span m="1699210">10</span>
  <span m="1699540">people?</span> <span m="1701010">What</span> <span m="1701160">fraction
  of</span> <span m="1701580">them</span> <span m="1701730">should</span> <span m="1701910">actually</span>
  <span m="1702480">die</span> <span m="1703020">in</span> <span m="1703140">the</span>
  <span m="1703230">next</span> <span m="1703980">48</span> <span m="1704310">hours?</span>
  <span m="1705900">Everyone</span> <span m="1706140">could</span> <span m="1706230">scream</span>
  <span m="1706500">out</span> <span m="1706560">loud.</span></p><p><span m="1707300">[INTERPOSING
  VOICES]</span></p><p><span m="1709500">PROFESSOR:</span> <span m="1709590">So</span>
  <span m="1710250">seven</span> <span m="1710760">of</span> <span m="1710970">them.</span>
  <span m="1711720">Seven</span> <span m="1712050">of</span> <span m="1712110">the</span>
  <span m="1712200">10</span> <span m="1712890">you</span> <span m="1712980">would</span>
  <span m="1713070">expect</span> <span m="1713580">to</span> <span m="1713730">die</span>
  <span m="1714060">in</span> <span m="1714180">the</span> <span m="1714240">next</span>
  <span m="1714840">48</span> <span m="1715140">hours</span> <span m="1715860">if</span>
  <span m="1716010">the</span> <span m="1716130">probability</span> <span m="1716820">for</span>
  <span m="1716970">all</span> <span m="1717270">of</span> <span m="1717360">them</span>
  <span m="1717570">that</span> <span m="1717690">was</span> <span m="1717810">output</span>
  <span m="1718140">was</span> <span m="1718290">0.7.</span> <span m="1719435">All</span>
  <span m="1719920">right,</span> <span m="1720030">that's</span> <span m="1720210">what</span>
  <span m="1720330">I</span> <span m="1720390">mean</span> <span m="1720480">by</span>
  <span m="1720600">calibration.</span></p><p><span m="1721710">So</span> <span m="1721890">if,</span>
  <span m="1722010">on</span> <span m="1722070">the</span> <span m="1722120">other</span>
  <span m="1722310">hand,</span> <span m="1722650">what</span> <span m="1722670">you</span>
  <span m="1722760">found</span> <span m="1723150">was</span> <span m="1723360">that</span>
  <span m="1724260">only</span> <span m="1724470">one</span> <span m="1724620">of</span>
  <span m="1724680">them</span> <span m="1724830">died,</span> <span m="1725660">then</span>
  <span m="1726620">it</span> <span m="1726890">would</span> <span m="1726980">be</span>
  <span m="1727080">a</span> <span m="1727110">very</span> <span m="1727440">weird</span>
  <span m="1727890">number</span> <span m="1728280">that</span> <span m="1728910">you're</span>
  <span m="1729080">outputting.</span> <span m="1729730">And</span> <span m="1729810">so</span>
  <span m="1730410">the</span> <span m="1730470">reason</span> <span m="1730770">why</span>
  <span m="1731220">this</span> <span m="1731400">notion</span> <span m="1731730">of</span>
  <span m="1731790">calibration,</span> <span m="1732330">which</span> <span m="1732480">I'll</span>
  <span m="1732570">define</span> <span m="1733020">formally</span> <span m="1733350">in</span>
  <span m="1733410">a</span> <span m="1733440">second,</span> <span m="1733770">is</span>
  <span m="1733860">so</span> <span m="1734010">important,</span> <span m="1734640">is</span>
  <span m="1735180">when</span> <span m="1735360">you're</span> <span m="1735510">out</span>
  <span m="1735720">putting</span> <span m="1736020">a</span> <span m="1736080">probability,</span>
  <span m="1737230">and</span> <span m="1737370">when</span> <span m="1737490">you</span>
  <span m="1737580">don't</span> <span m="1737850">really</span> <span m="1738210">know</span>
  <span m="1738510">how</span> <span m="1738660">that</span> <span m="1738780">probability</span>
  <span m="1739070">is</span> <span m="1739190">going</span> <span m="1739260">to</span>
  <span m="1739340">be</span> <span m="1739410">used.</span> <span m="1740640">If</span>
  <span m="1740820">you</span> <span m="1740970">knew--</span> <span m="1741510">if</span>
  <span m="1741600">you</span> <span m="1741720">had</span> <span m="1741870">some</span>
  <span m="1742050">task</span> <span m="1742560">loss</span> <span m="1742920">in</span>
  <span m="1743040">mind.</span> <span m="1744180">And</span> <span m="1744300">you</span>
  <span m="1744390">knew</span> <span m="1744720">that</span> <span m="1745470">all</span>
  <span m="1745650">that</span> <span m="1745800">mattered</span> <span m="1746130">was</span>
  <span m="1746310">the</span> <span m="1746400">actual</span> <span m="1746700">prediction,</span>
  <span m="1748170">1</span> <span m="1748620">or</span> <span m="1748770">0,</span>
  <span m="1750240">then</span> <span m="1750420">that</span> <span m="1750540">would</span>
  <span m="1750630">be</span> <span m="1750720">fine.</span></p><p><span m="1750990">But</span>
  <span m="1751140">often</span> <span m="1752370">predictions</span> <span m="1753150">in</span>
  <span m="1753240">machine</span> <span m="1753510">learning</span> <span m="1753870">are</span>
  <span m="1753960">used</span> <span m="1754320">in a</span> <span m="1754440">much</span>
  <span m="1754590">more</span> <span m="1754710">subtle</span> <span m="1754980">way.</span>
  <span m="1755260">Like</span> <span m="1755370">for</span> <span m="1755460">example,</span>
  <span m="1755870">often</span> <span m="1757050">your</span> <span m="1757230">doctor</span>
  <span m="1758010">might</span> <span m="1758250">have</span> <span m="1758460">more</span>
  <span m="1758730">information</span> <span m="1759300">than</span> <span m="1759440">your</span>
  <span m="1760050">computer</span> <span m="1760380">has.</span> <span m="1760980">And</span>
  <span m="1761070">so</span> <span m="1761190">often</span> <span m="1761490">they</span>
  <span m="1761580">might</span> <span m="1761730">want</span> <span m="1761880">to</span>
  <span m="1761940">take</span> <span m="1763110">the</span> <span m="1763470">result</span>
  <span m="1764160">that</span> <span m="1764340">your</span> <span m="1764490">computer</span>
  <span m="1765180">predicts,</span> <span m="1766380">and</span> <span m="1766620">weigh</span>
  <span m="1767040">that</span> <span m="1767220">against</span> <span m="1767520">other</span>
  <span m="1767820">evidence.</span> <span m="1768930">Or</span> <span m="1769730">in</span>
  <span m="1769970">some</span> <span m="1770150">settings,</span> <span m="1770430">it's</span>
  <span m="1770550">not</span> <span m="1770670">just</span> <span m="1770880">weighting</span>
  <span m="1771180">about</span> <span m="1771480">other</span> <span m="1771660">evidence.</span>
  <span m="1772020">Maybe</span> <span m="1772290">it's</span> <span m="1772370">also</span>
  <span m="1772560">about</span> <span m="1772860">making</span> <span m="1773190">a</span>
  <span m="1773220">decision.</span> <span m="1774300">And</span> <span m="1774420">that</span>
  <span m="1774500">decision</span> <span m="1774960">might</span> <span m="1775380">take</span>
  <span m="1775590">exertion--</span> <span m="1776420">a</span> <span m="1776520">utility,</span>
  <span m="1777630">for</span> <span m="1777780">example,</span> <span m="1778780">a</span>
  <span m="1778880">patient</span> <span m="1779130">preference</span> <span m="1780090">for</span>
  <span m="1781680">suffering</span> <span m="1783660">versus</span> <span m="1786630">getting</span>
  <span m="1786990">a</span> <span m="1787110">treatment</span> <span m="1787560">that</span>
  <span m="1787710">could</span> <span m="1787890">have</span> <span m="1788580">big,</span>
  <span m="1788880">adverse</span> <span m="1789810">consequences.</span></p><p><span
  m="1791160">And</span> <span m="1791350">that's</span> <span m="1791460">something</span>
  <span m="1791780">that</span> <span m="1792010">Pete</span> <span m="1792270">is</span>
  <span m="1792360">going</span> <span m="1792480">to</span> <span m="1792540">talk</span>
  <span m="1792690">about</span> <span m="1792960">much</span> <span m="1793230">more</span>
  <span m="1793830">later</span> <span m="1794070">in</span> <span m="1794130">the</span>
  <span m="1794220">semester,</span> <span m="1795130">I</span> <span m="1795230">think,</span>
  <span m="1796810">how</span> <span m="1796920">to</span> <span m="1797020">formalize</span>
  <span m="1797520">that</span> <span m="1797640">notion.</span> <span m="1798060">But</span>
  <span m="1798480">at</span> <span m="1798570">this</span> <span m="1798750">point,</span>
  <span m="1798930">I</span> <span m="1798990">just</span> <span m="1799110">want</span>
  <span m="1799230">to</span> <span m="1800000">sort</span> <span m="1800210">of</span>
  <span m="1800280">get</span> <span m="1800460">out</span> <span m="1800820">the</span>
  <span m="1801030">point</span> <span m="1801360">that</span> <span m="1801630">the</span>
  <span m="1801960">probabilities</span> <span m="1802470">themselves</span> <span
  m="1802860">could</span> <span m="1803010">be</span> <span m="1803100">important.</span>
  <span m="1803610">And</span> <span m="1803730">having</span> <span m="1804150">the</span>
  <span m="1804270">probabilities</span> <span m="1804690">be</span> <span m="1804780">meaningful</span>
  <span m="1805650">is</span> <span m="1805740">something</span> <span m="1805980">that</span>
  <span m="1806100">one</span> <span m="1806250">can</span> <span m="1806320">now</span>
  <span m="1806460">quantify.</span></p><p><span m="1807160">So</span> <span m="1807330">how</span>
  <span m="1807480">do</span> <span m="1807540">we</span> <span m="1807630">quantify</span>
  <span m="1808110">it?</span> <span m="1808940">Well,</span> <span m="1813150">one</span>
  <span m="1813420">way</span> <span m="1813540">to</span> <span m="1813630">try</span>
  <span m="1813750">to</span> <span m="1813840">quantify</span> <span m="1814320">it</span>
  <span m="1814470">is</span> <span m="1814590">to</span> <span m="1814680">create</span>
  <span m="1814920">the</span> <span m="1815010">following</span> <span m="1815400">prompt.</span>
  <span m="1818105">Actually,</span> <span m="1818640">we'll</span> <span m="1819030">call</span>
  <span m="1819360">it a</span> <span m="1819430">histogram.</span> <span m="1822970">So</span>
  <span m="1823810">on</span> <span m="1823930">the</span> <span m="1823990">x-axis</span>
  <span m="1824860">is</span> <span m="1825160">the</span> <span m="1825340">predicted</span>
  <span m="1826120">probability.</span> <span m="1834650">So</span> <span m="1834830">that's</span>
  <span m="1835040">what</span> <span m="1835160">I</span> <span m="1835220">meant</span>
  <span m="1835460">by</span> <span m="1836030">p-hat.</span> <span m="1837500">On</span>
  <span m="1837650">the</span> <span m="1837710">y-axis</span> <span m="1838730">is</span>
  <span m="1839480">the</span> <span m="1839660">true</span> <span m="1840170">probability.</span>
  <span m="1840920">It's</span> <span m="1841160">what</span> <span m="1841400">I</span>
  <span m="1841490">mean</span> <span m="1841670">when</span> <span m="1841790">I</span>
  <span m="1841880">say</span> <span m="1842000">the</span> <span m="1842090">fraction</span>
  <span m="1842660">of</span> <span m="1842750">individuals</span> <span m="1843740">with</span>
  <span m="1843920">that</span> <span m="1844070">predicted</span> <span m="1844520">probability</span>
  <span m="1845390">that</span> <span m="1845580">actually</span> <span m="1846140">got</span>
  <span m="1846470">the</span> <span m="1847010">positive</span> <span m="1847580">outcome.</span>
  <span m="1848120">That's</span> <span m="1848330">going</span> <span m="1848450">to</span>
  <span m="1848510">be</span> <span m="1848570">the</span> <span m="1848660">y-axis.</span>
  <span m="1849510">So</span> <span m="1849560">I'll</span> <span m="1849620">call</span>
  <span m="1849830">that</span> <span m="1850700">the</span> <span m="1850940">true</span>
  <span m="1851720">probability.</span></p><p><span m="1857630">And</span> <span m="1857750">what</span>
  <span m="1857870">we</span> <span m="1857970">would</span> <span m="1858110">like</span>
  <span m="1858350">to</span> <span m="1858530">see</span> <span m="1859610">is</span>
  <span m="1859850">that</span> <span m="1860540">this</span> <span m="1861110">is</span>
  <span m="1863030">a</span> <span m="1863090">line,</span> <span m="1864090">a</span>
  <span m="1864320">straight</span> <span m="1864620">line,</span> <span m="1865140">meaning</span>
  <span m="1865340">these</span> <span m="1865580">two</span> <span m="1865760">should</span>
  <span m="1865940">always</span> <span m="1866210">be</span> <span m="1866330">equal.</span>
  <span m="1867480">And</span> <span m="1867930">in</span> <span m="1868070">the</span>
  <span m="1868130">example</span> <span m="1868610">I</span> <span m="1868760">gave,</span>
  <span m="1869600">remember</span> <span m="1869840">I</span> <span m="1869930">said</span>
  <span m="1870350">that</span> <span m="1870590">there</span> <span m="1870710">were</span>
  <span m="1870830">a</span> <span m="1870860">bunch</span> <span m="1871160">of</span>
  <span m="1871220">people</span> <span m="1872030">with</span> <span m="1872630">0.7</span>
  <span m="1873350">probability</span> <span m="1874160">predicted,</span> <span m="1875150">but</span>
  <span m="1875810">for</span> <span m="1876020">whom</span> <span m="1877190">only</span>
  <span m="1877550">one</span> <span m="1878210">out</span> <span m="1878540">of</span>
  <span m="1878660">them</span> <span m="1879830">actually</span> <span m="1880310">got</span>
  <span m="1880520">the</span> <span m="1880610">positive</span> <span m="1881050">end.</span>
  <span m="1881670">So</span> <span m="1881900">that</span> <span m="1882080">would</span>
  <span m="1882230">have</span> <span m="1882320">been</span> <span m="1882530">something</span>
  <span m="1882860">like</span> <span m="1883040">over</span> <span m="1883250">here.</span>
  <span m="1886550">Whereas</span> <span m="1886880">you</span> <span m="1886970">would</span>
  <span m="1887060">have</span> <span m="1887180">expected</span> <span m="1887690">it</span>
  <span m="1887780">to</span> <span m="1887900">be</span> <span m="1887990">over</span>
  <span m="1888170">there.</span></p><p><span m="1889460">So</span> <span m="1890060">you</span>
  <span m="1890180">might</span> <span m="1890360">ask,</span> <span m="1890750">how</span>
  <span m="1890960">do</span> <span m="1891110">I</span> <span m="1891230">create</span>
  <span m="1892430">such</span> <span m="1892730">a</span> <span m="1892790">plot</span>
  <span m="1893210">from</span> <span m="1893540">finite</span> <span m="1893900">data?</span>
  <span m="1894800">Well, a</span> <span m="1894980">common</span> <span m="1895340">way</span>
  <span m="1895460">to</span> <span m="1895550">do</span> <span m="1895730">so</span>
  <span m="1895910">is</span> <span m="1896030">to</span> <span m="1896180">bin</span>
  <span m="1896780">your</span> <span m="1897020">data.</span> <span m="1897530">So</span>
  <span m="1898640">you'll</span> <span m="1898760">create</span> <span m="1899330">intervals.</span>
  <span m="1900440">So</span> <span m="1900890">this</span> <span m="1901340">bin</span>
  <span m="1902300">is</span> <span m="1902480">the</span> <span m="1902600">bin</span>
  <span m="1903170">from</span> <span m="1903650">0</span> <span m="1904370">to</span>
  <span m="1904610">0.1.</span> <span m="1906290">This</span> <span m="1906590">bin</span>
  <span m="1907610">is</span> <span m="1907790">the</span> <span m="1907880">bin</span>
  <span m="1908270">from</span> <span m="1909380">0.1</span> <span m="1909480">to</span>
  <span m="1910580">0.2,</span> <span m="1911360">and</span> <span m="1911480">so</span>
  <span m="1911720">on.</span></p><p><span m="1912620">And</span> <span m="1912740">then</span>
  <span m="1912860">you'll</span> <span m="1912950">look</span> <span m="1913070">to</span>
  <span m="1913160">see,</span> <span m="1913440">OK,</span> <span m="1913890">how</span>
  <span m="1914060">many</span> <span m="1914330">people</span> <span m="1915680">for</span>
  <span m="1915890">whom</span> <span m="1916160">the</span> <span m="1916280">predicted</span>
  <span m="1916880">probability</span> <span m="1917390">was</span> <span m="1917510">between</span>
  <span m="1918170">0</span> <span m="1918560">and</span> <span m="1918650">0.1</span>
  <span m="1920510">actually</span> <span m="1921110">died?</span> <span m="1921770">And</span>
  <span m="1921890">you'll</span> <span m="1922010">get</span> <span m="1922100">a</span>
  <span m="1922160">number</span> <span m="1922550">out.</span> <span m="1923940">And</span>
  <span m="1924160">now</span> <span m="1924410">here's</span> <span m="1924650">where</span>
  <span m="1924740">I</span> <span m="1924770">can</span> <span m="1924910">go</span>
  <span m="1924980">to</span> <span m="1925070">this</span> <span m="1925200">plot.</span>
  <span m="1925490">That's</span> <span m="1925700">exactly</span> <span m="1926030">what</span>
  <span m="1926090">I'm</span> <span m="1926180">showing</span> <span m="1926360">you</span>
  <span m="1926450">here.</span></p><p><span m="1926690">So</span> <span m="1927110">for</span>
  <span m="1927260">now,</span> <span m="1927470">ignore</span> <span m="1927860">the</span>
  <span m="1928010">bar</span> <span m="1928490">charts</span> <span m="1928920">and</span>
  <span m="1929000">the</span> <span m="1929090">bottom,</span> <span m="1929330">and</span>
  <span m="1929420">just</span> <span m="1929540">look</span> <span m="1929690">at</span>
  <span m="1929750">the</span> <span m="1929840">line.</span> <span m="1931930">So</span>
  <span m="1932660">let's</span> <span m="1932840">focus</span> <span m="1933290">on</span>
  <span m="1933440">just</span> <span m="1933680">the</span> <span m="1933770">green</span>
  <span m="1934190">line.</span> <span m="1934520">Here</span> <span m="1934730">I'm</span>
  <span m="1934820">showing</span> <span m="1935030">you</span> <span m="1935120">several</span>
  <span m="1935420">different</span> <span m="1935630">models.</span> <span m="1935990">For</span>
  <span m="1936140">now,</span> <span m="1936390">just</span> <span m="1936500">focus</span>
  <span m="1936800">on</span> <span m="1936860">the</span> <span m="1936950">green</span>
  <span m="1937160">line.</span> <span m="1938580">So</span> <span m="1938630">the</span>
  <span m="1938690">green</span> <span m="1938930">line,</span> <span m="1939200">by</span>
  <span m="1939320">the</span> <span m="1939410">way,</span> <span m="1939870">notice</span>
  <span m="1941420">it</span> <span m="1941600">looks</span> <span m="1941750">pretty</span>
  <span m="1941990">good.</span> <span m="1942170">It's</span> <span m="1942380">almost</span>
  <span m="1943070">a</span> <span m="1943130">straight</span> <span m="1943430">line.</span>
  <span m="1944630">So</span> <span m="1944780">how</span> <span m="1944930">did</span>
  <span m="1945080">I</span> <span m="1945170">compute</span> <span m="1945470">it?</span>
  <span m="1945560">Well,</span> <span m="1945680">first</span> <span m="1945890">of</span>
  <span m="1945950">all,</span> <span m="1946020">notice</span> <span m="1946370">the</span>
  <span m="1946760">number</span> <span m="1947000">of</span> <span m="1947090">ticks</span>
  <span m="1947510">are</span> <span m="1947660">1,</span> <span m="1948060">2,</span>
  <span m="1948330">3,</span> <span m="1948590">4,</span> <span m="1948920">5,</span>
  <span m="1949170">6,</span> <span m="1949490">7,</span> <span m="1949850">8,</span>
  <span m="1950120">9,</span> <span m="1950390">10.</span> <span m="1950510">OK,</span>
  <span m="1950690">so</span> <span m="1950780">there</span> <span m="1950870">are</span>
  <span m="1950930">10</span> <span m="1952190">points</span> <span m="1952700">along</span>
  <span m="1952940">this</span> <span m="1953090">line.</span> <span m="1953810">And</span>
  <span m="1953930">each</span> <span m="1954080">of</span> <span m="1954140">those</span>
  <span m="1954350">corresponds</span> <span m="1954980">to</span> <span m="1955280">one</span>
  <span m="1955550">of</span> <span m="1955640">these</span> <span m="1955880">bins.</span>
  <span m="1956330">So</span> <span m="1956510">the</span> <span m="1956630">first</span>
  <span m="1957140">point</span> <span m="1957530">is</span> <span m="1958130">the</span>
  <span m="1958250">0 to</span> <span m="1958580">0.1</span> <span m="1959270">bin.</span>
  <span m="1959810">The</span> <span m="1959900">second</span> <span m="1960230">point</span>
  <span m="1960590">is</span> <span m="1960740">the</span> <span m="1960830">0.1</span>
  <span m="1961070">to</span> <span m="1961310">0.2</span> <span m="1961760">bin,</span>
  <span m="1962000">and</span> <span m="1962120">so</span> <span m="1962330">on.</span>
  <span m="1962930">So</span> <span m="1962990">that's</span> <span m="1963200">how</span>
  <span m="1963320">it</span> <span m="1963380">computed</span> <span m="1963740">this.</span></p><p><span
  m="1965540">The</span> <span m="1965630">next</span> <span m="1965900">thing</span>
  <span m="1966050">you</span> <span m="1966140">notice</span> <span m="1966470">is</span>
  <span m="1966560">that</span> <span m="1966710">I</span> <span m="1966830">have</span>
  <span m="1967580">confidence</span> <span m="1968150">intervals.</span> <span m="1969710">And</span>
  <span m="1970400">the</span> <span m="1970520">reason</span> <span m="1970820">I</span>
  <span m="1970970">compute</span> <span m="1971270">these</span> <span m="1971390">confidence</span>
  <span m="1971780">intervals</span> <span m="1972500">is</span> <span m="1972680">because</span>
  <span m="1973890">sometimes</span> <span m="1974360">you</span> <span m="1974470">just</span>
  <span m="1974660">might</span> <span m="1974810">not</span> <span m="1975020">have</span>
  <span m="1975230">that</span> <span m="1975380">much</span> <span m="1975620">data</span>
  <span m="1975950">in</span> <span m="1976040">one</span> <span m="1976190">of</span>
  <span m="1976250">these</span> <span m="1976430">bins.</span> <span m="1977060">So</span>
  <span m="1977150">for</span> <span m="1977240">example,</span> <span m="1977510">suppose</span>
  <span m="1977840">your</span> <span m="1978020">algorithm</span> <span m="1978860">almost</span>
  <span m="1979370">never</span> <span m="1979880">said</span> <span m="1980690">that</span>
  <span m="1980870">someone</span> <span m="1981200">has</span> <span m="1981410">a</span>
  <span m="1981470">predictive</span> <span m="1981830">probability</span> <span m="1982250">of</span>
  <span m="1982370">0.99.</span> <span m="1984560">Then</span> <span m="1985990">until</span>
  <span m="1986180">you</span> <span m="1986240">get</span> <span m="1986360">a</span>
  <span m="1986420">ton</span> <span m="1986660">of</span> <span m="1986750">data,</span>
  <span m="1987020">you're</span> <span m="1987140">not</span> <span m="1987260">going</span>
  <span m="1987390">to</span> <span m="1987430">know</span> <span m="1987590">what</span>
  <span m="1987710">fraction</span> <span m="1988190">of</span> <span m="1988250">those</span>
  <span m="1988400">individuals</span> <span m="1988910">actually</span> <span m="1989330">went</span>
  <span m="1989630">on</span> <span m="1989780">to</span> <span m="1989900">develop</span>
  <span m="1990200">the</span> <span m="1990290">event.</span></p><p><span m="1992120">And</span>
  <span m="1993030">you</span> <span m="1993140">should</span> <span m="1993260">be</span>
  <span m="1993350">looking</span> <span m="1993590">at</span> <span m="1993680">sort</span>
  <span m="1993770">of</span> <span m="1993840">the</span> <span m="1993920">confidence</span>
  <span m="1994610">interval</span> <span m="1995480">of</span> <span m="1995630">this</span>
  <span m="1995870">line,</span> <span m="1997090">which</span> <span m="1997400">should</span>
  <span m="1997550">take</span> <span m="1997790">that</span> <span m="1997940">into</span>
  <span m="1998090">consideration.</span> <span m="1999310">And</span> <span m="1999440">a</span>
  <span m="1999500">different</span> <span m="1999800">way</span> <span m="1999950">to</span>
  <span m="2000040">try</span> <span m="2000280">to</span> <span m="2000460">understand</span>
  <span m="2001120">that</span> <span m="2001270">notion,</span> <span m="2001640">now</span>
  <span m="2001720">looking</span> <span m="2001960">at</span> <span m="2002020">the</span>
  <span m="2002110">numbers,</span> <span m="2002530">is</span> <span m="2002620">what</span>
  <span m="2002740">I'm</span> <span m="2002830">showing</span> <span m="2003040">you</span>
  <span m="2003100">in</span> <span m="2003160">the</span> <span m="2003220">bar</span>
  <span m="2003490">charts</span> <span m="2003820">in</span> <span m="2003890">the</span>
  <span m="2003970">bottom.</span> <span m="2004660">On</span> <span m="2004780">the</span>
  <span m="2004840">bar</span> <span m="2005050">charts,</span> <span m="2005380">I'm</span>
  <span m="2005470">showing</span> <span m="2005860">you</span> <span m="2007790">the</span>
  <span m="2007840">number</span> <span m="2008290">of</span> <span m="2008380">individuals</span>
  <span m="2009100">or</span> <span m="2009160">the</span> <span m="2009250">fraction</span>
  <span m="2009700">of</span> <span m="2009790">individuals</span> <span m="2010510">who</span>
  <span m="2010660">actually</span> <span m="2010990">got</span> <span m="2011260">that</span>
  <span m="2011410">predicted</span> <span m="2012760">probability.</span></p><p><span
  m="2013550">So</span> <span m="2014800">now</span> <span m="2014980">let's</span>
  <span m="2015080">start</span> <span m="2015310">comparing</span> <span m="2015670">the</span>
  <span m="2015730">lines.</span> <span m="2016210">So</span> <span m="2016990">the</span>
  <span m="2019030">blue</span> <span m="2019480">line</span> <span m="2019840">shown</span>
  <span m="2020170">here</span> <span m="2020950">is</span> <span m="2021610">a</span>
  <span m="2022210">machine</span> <span m="2022600">learning</span> <span m="2023230">algorithm</span>
  <span m="2024260">which</span> <span m="2024520">is</span> <span m="2024850">predicting</span>
  <span m="2025870">infection</span> <span m="2026560">in the</span> <span m="2026650">emergency</span>
  <span m="2026980">rooms.</span> <span m="2027220">It's</span> <span m="2027330">a</span>
  <span m="2027370">slightly</span> <span m="2027730">different</span> <span m="2027940">problem</span>
  <span m="2028270">than</span> <span m="2028510">the</span> <span m="2028750">diabetes</span>
  <span m="2029230">one</span> <span m="2029350">we</span> <span m="2029440">looked</span>
  <span m="2029560">at</span> <span m="2029650">earlier.</span> <span m="2030520">And</span>
  <span m="2030640">it's</span> <span m="2030790">using</span> <span m="2031030">a</span>
  <span m="2031090">bag</span> <span m="2031360">of</span> <span m="2031450">words</span>
  <span m="2031750">model</span> <span m="2032410">from</span> <span m="2032650">clinical</span>
  <span m="2032950">text.</span> <span m="2034960">The</span> <span m="2035590">red</span>
  <span m="2036640">line</span> <span m="2037690">is</span> <span m="2038500">using</span>
  <span m="2039040">just</span> <span m="2039970">chief</span> <span m="2040360">complaint.</span>
  <span m="2041020">So</span> <span m="2041200">it's</span> <span m="2041320">using</span>
  <span m="2042070">one</span> <span m="2042430">piece</span> <span m="2042760">of</span>
  <span m="2042850">structured</span> <span m="2043330">data</span> <span m="2043600">that</span>
  <span m="2043720">you</span> <span m="2043840">get</span> <span m="2044110">at</span>
  <span m="2044290">one</span> <span m="2044590">point</span> <span m="2044800">of</span>
  <span m="2044860">time</span> <span m="2045040">in the</span> <span m="2045150">ER.</span>
  <span m="2045400">So</span> <span m="2045670">it's</span> <span m="2046330">using</span>
  <span m="2046780">very</span> <span m="2047740">little</span> <span m="2048280">information.</span>
  <span m="2050960">And</span> <span m="2050980">you</span> <span m="2051070">can</span>
  <span m="2051219">see</span> <span m="2051489">that</span> <span m="2051790">both</span>
  <span m="2053230">models</span> <span m="2054489">are</span> <span m="2055510">somewhat</span>
  <span m="2055929">well</span> <span m="2056469">calibrated.</span></p><p><span m="2057199">But</span>
  <span m="2057420">the</span> <span m="2058630">intervals--</span> <span m="2059230">the</span>
  <span m="2059320">confidence</span> <span m="2059800">intervals</span> <span m="2060730">of</span>
  <span m="2061150">both</span> <span m="2061420">the</span> <span m="2061510">red</span>
  <span m="2061780">and</span> <span m="2061900">the</span> <span m="2061989">purple</span>
  <span m="2062320">lines</span> <span m="2062679">gets</span> <span m="2063070">really</span>
  <span m="2063520">big</span> <span m="2063810">towards</span> <span m="2064120">the</span>
  <span m="2064210">end.</span> <span m="2065389">And</span> <span m="2065500">if</span>
  <span m="2065590">you</span> <span m="2065679">look</span> <span m="2066100">at</span>
  <span m="2066310">these</span> <span m="2066520">bar</span> <span m="2066730">charts,</span>
  <span m="2066969">it</span> <span m="2067030">explains</span> <span m="2067540">why,</span>
  <span m="2067989">because</span> <span m="2068770">the</span> <span m="2069489">models</span>
  <span m="2069760">that</span> <span m="2069850">use</span> <span m="2070090">less</span>
  <span m="2070330">information</span> <span m="2071020">end</span> <span m="2071199">up</span>
  <span m="2071290">being</span> <span m="2071650">much</span> <span m="2072159">more</span>
  <span m="2073389">risk-averse.</span> <span m="2075190">So</span> <span m="2075340">they</span>
  <span m="2075489">will</span> <span m="2075610">never</span> <span m="2076150">predict</span>
  <span m="2076900">a</span> <span m="2076960">very</span> <span m="2077230">high</span>
  <span m="2077409">probability.</span> <span m="2078010">They will</span> <span m="2078130">always</span>
  <span m="2078400">sort</span> <span m="2078639">of</span> <span m="2078699">stay</span>
  <span m="2079050">in</span> <span m="2079150">this</span> <span m="2079330">lower</span>
  <span m="2079659">regime.</span> <span m="2081250">And</span> <span m="2081429">that's</span>
  <span m="2081550">why</span> <span m="2081670">we</span> <span m="2081760">have</span>
  <span m="2081850">very</span> <span m="2082000">big</span> <span m="2082120">confidence</span>
  <span m="2082480">intervals</span> <span m="2082810">there.</span></p><p><span m="2086340">OK,</span>
  <span m="2086739">so</span> <span m="2086800">that's</span> <span m="2087010">all</span>
  <span m="2087219">I</span> <span m="2087280">want</span> <span m="2087460">to</span>
  <span m="2087520">say</span> <span m="2087790">about</span> <span m="2088420">evaluation.</span>
  <span m="2090159">And</span> <span m="2090760">I</span> <span m="2090850">won't</span>
  <span m="2091030">take</span> <span m="2091210">any</span> <span m="2091360">questions</span>
  <span m="2091690">on</span> <span m="2091750">this</span> <span m="2091900">right</span>
  <span m="2092020">now,</span> <span m="2092320">because I</span> <span m="2092380">really</span>
  <span m="2092590">want</span> <span m="2092710">to</span> <span m="2092770">get</span>
  <span m="2092889">on</span> <span m="2092949">to</span> <span m="2093070">the</span>
  <span m="2093159">rest</span> <span m="2093300">of</span> <span m="2093360">the</span>
  <span m="2093400">lecture.</span> <span m="2095560">But</span> <span m="2095920">again,</span>
  <span m="2096190">if</span> <span m="2096370">you</span> <span m="2096429">have</span>
  <span m="2096550">any</span> <span m="2096760">questions,</span> <span m="2097240">post</span>
  <span m="2097480">to</span> <span m="2097580">Piazza,</span> <span m="2097960">and</span>
  <span m="2098200">I'm</span> <span m="2098350">happy</span> <span m="2098620">to</span>
  <span m="2098740">discuss</span> <span m="2099070">them</span> <span m="2099220">with</span>
  <span m="2099370">you</span> <span m="2099460">offline.</span></p><p><span m="2103210">So,</span>
  <span m="2104200">in</span> <span m="2104350">summary,</span> <span m="2105200">we've</span>
  <span m="2105280">talked</span> <span m="2105640">about</span> <span m="2106660">how</span>
  <span m="2106990">to</span> <span m="2107140">reduce</span> <span m="2108670">risk</span>
  <span m="2108850">stratification</span> <span m="2109660">to</span> <span m="2109810">binary</span>
  <span m="2110170">classification.</span> <span m="2111610">I've</span> <span m="2111730">told</span>
  <span m="2111970">you</span> <span m="2112030">how</span> <span m="2112210">to</span>
  <span m="2112300">derive</span> <span m="2112630">the</span> <span m="2112720">labels.</span>
  <span m="2113470">I've</span> <span m="2113610">given</span> <span m="2113890">you</span>
  <span m="2114010">one</span> <span m="2114250">example</span> <span m="2114730">of</span>
  <span m="2114820">machine</span> <span m="2115150">learning</span> <span m="2115360">algorithm</span>
  <span m="2115880">you</span> <span m="2115980">can</span> <span m="2115990">use,</span>
  <span m="2116245">and</span> <span m="2116500">I</span> <span m="2116560">talked</span>
  <span m="2116830">to</span> <span m="2116910">you</span> <span m="2116980">about</span>
  <span m="2117130">how</span> <span m="2117280">to</span> <span m="2117370">evaluate</span>
  <span m="2117910">it.</span> <span m="2119440">What</span> <span m="2119650">could</span>
  <span m="2119830">possibly</span> <span m="2120370">go</span> <span m="2120490">wrong?</span></p><p><span
  m="2123570">So</span> <span m="2123620">let's</span> <span m="2123800">look</span>
  <span m="2123950">at</span> <span m="2124040">some</span> <span m="2124370">examples.</span>
  <span m="2126890">And</span> <span m="2127040">these</span> <span m="2127250">are</span>
  <span m="2127350">a</span> <span m="2127370">small</span> <span m="2127790">number</span>
  <span m="2127970">of</span> <span m="2128030">examples</span> <span m="2128390">of</span>
  <span m="2128450">what</span> <span m="2128540">could</span> <span m="2128630">possibly</span>
  <span m="2128960">go</span> <span m="2129050">wrong.</span> <span m="2129780">There</span>
  <span m="2129880">are</span> <span m="2129980">many</span> <span m="2130040">more.</span></p><p><span
  m="2131680">So</span> <span m="2131810">here's</span> <span m="2132020">some</span>
  <span m="2132200">data.</span> <span m="2133340">I'm</span> <span m="2133490">showing</span>
  <span m="2133970">you--</span> <span m="2134870">for</span> <span m="2135050">the</span>
  <span m="2135140">same</span> <span m="2135620">problem</span> <span m="2135950">we</span>
  <span m="2136040">looked</span> <span m="2136190">at</span> <span m="2136310">before,</span>
  <span m="2136640">diabetes</span> <span m="2137090">onset,</span> <span m="2138170">I'm</span>
  <span m="2138260">showing</span> <span m="2138650">you</span> <span m="2139010">the</span>
  <span m="2139790">prevalence</span> <span m="2140780">of</span> <span m="2141620">type</span>
  <span m="2141920">2</span> <span m="2142070">diabetes</span> <span m="2142880">as</span>
  <span m="2143210">recorded</span> <span m="2143720">by,</span> <span m="2144050">let's</span>
  <span m="2144230">say,</span> <span m="2144440">diagnosis</span> <span m="2145130">codes</span>
  <span m="2146000">across</span> <span m="2146360">time.</span> <span m="2147926">All
  right, so</span> <span m="2148330">over</span> <span m="2148550">here</span> <span
  m="2148760">is</span> <span m="2148850">1980.</span> <span m="2149450">Over</span>
  <span m="2149600">here</span> <span m="2149780">is</span> <span m="2149870">2012.</span>
  <span m="2153290">Look</span> <span m="2153430">at</span> <span m="2153860">that.</span>
  <span m="2154340">It</span> <span m="2154420">is</span> <span m="2154580">not</span>
  <span m="2154880">a</span> <span m="2154940">flat</span> <span m="2155310">line.</span>
  <span m="2156430">Now,</span> <span m="2156500">what</span> <span m="2156620">does</span>
  <span m="2156710">that</span> <span m="2156830">mean?</span> <span m="2157130">Does</span>
  <span m="2157250">that</span> <span m="2157400">mean</span> <span m="2157760">that</span>
  <span m="2158120">the</span> <span m="2158300">population</span> <span m="2160460">is</span>
  <span m="2160880">eating</span> <span m="2161270">much</span> <span m="2161510">more</span>
  <span m="2161720">unhealthy</span> <span m="2163010">from</span> <span m="2163190">1980</span>
  <span m="2163850">to</span> <span m="2163910">2012,</span> <span m="2165980">and</span>
  <span m="2166130">so</span> <span m="2166340">more</span> <span m="2166550">people</span>
  <span m="2166810">are</span> <span m="2166850">becoming</span> <span m="2167210">diabetic?</span>
  <span m="2168890">That</span> <span m="2168980">would</span> <span m="2169070">be</span>
  <span m="2169160">one</span> <span m="2169370">plausible</span> <span m="2169790">answer.</span></p><p><span
  m="2171230">Another</span> <span m="2171920">plausible</span> <span m="2172280">explanation</span>
  <span m="2174410">is</span> <span m="2174860">that</span> <span m="2175520">something</span>
  <span m="2176120">has</span> <span m="2176330">changed.</span> <span m="2177660">So</span>
  <span m="2177740">in</span> <span m="2177830">fact</span> <span m="2178130">I'm</span>
  <span m="2178760">showing</span> <span m="2179270">you</span> <span m="2179390">with</span>
  <span m="2179540">these</span> <span m="2179780">blue</span> <span m="2180350">lines,</span>
  <span m="2181500">well,</span> <span m="2181670">in</span> <span m="2181730">fact,</span>
  <span m="2182030">there</span> <span m="2182150">was</span> <span m="2182270">a</span>
  <span m="2182330">change</span> <span m="2182930">in</span> <span m="2183080">the</span>
  <span m="2183170">diagnostic</span> <span m="2184070">criteria</span> <span m="2185240">for</span>
  <span m="2185720">diabetes.</span></p><p><span m="2187790">And</span> <span m="2187910">so</span>
  <span m="2188000">now</span> <span m="2188240">the</span> <span m="2188360">patient</span>
  <span m="2188810">population</span> <span m="2189410">actually</span> <span m="2189740">didn't</span>
  <span m="2189980">change</span> <span m="2190370">much</span> <span m="2190670">between,</span>
  <span m="2191120">let's say,</span> <span m="2191390">this</span> <span m="2191540">time</span>
  <span m="2191780">point</span> <span m="2191930">at</span> <span m="2191990">that</span>
  <span m="2192140">time</span> <span m="2192350">point.</span> <span m="2193130">But</span>
  <span m="2193310">what</span> <span m="2193460">really</span> <span m="2194300">led</span>
  <span m="2194720">it</span> <span m="2194780">to</span> <span m="2194960">this</span>
  <span m="2195170">big</span> <span m="2195530">uptick,</span> <span m="2197390">according</span>
  <span m="2197690">to</span> <span m="2197810">one</span> <span m="2198020">theory,</span>
  <span m="2198920">is</span> <span m="2199040">because</span> <span m="2199280">the</span>
  <span m="2199370">diagnostic</span> <span m="2199850">criteria</span> <span m="2200300">changed.</span>
  <span m="2201460">So</span> <span m="2201590">who</span> <span m="2201740">we're</span>
  <span m="2201890">calling</span> <span m="2202250">diabetic</span> <span m="2202700">has</span>
  <span m="2202850">changed.</span> <span m="2203240">Because</span> <span m="2203780">diseases</span>
  <span m="2205100">are,</span> <span m="2205520">at</span> <span m="2205790">the
  end of</span> <span m="2206085">the</span> <span m="2206380">day,</span> <span m="2206460">a</span>
  <span m="2206600">human-made</span> <span m="2207350">concept,</span> <span m="2208190">you</span>
  <span m="2208260">know,</span> <span m="2208460">what</span> <span m="2208700">do</span>
  <span m="2208790">we</span> <span m="2208910">call</span> <span m="2209420">some</span>
  <span m="2209660">disease.</span></p><p><span m="2211760">And</span> <span m="2211880">so</span>
  <span m="2212600">the</span> <span m="2212690">data</span> <span m="2213110">is</span>
  <span m="2213260">changing,</span> <span m="2214850">as</span> <span m="2215000">you</span>
  <span m="2215090">see</span> <span m="2215270">here.</span> <span m="2215780">Let</span>
  <span m="2215900">me</span> <span m="2215990">show</span> <span m="2216140">you</span>
  <span m="2216260">another</span> <span m="2216530">example.</span> <span m="2217080">Oh,</span>
  <span m="2217160">by</span> <span m="2217280">the</span> <span m="2217340">way,</span>
  <span m="2217700">so</span> <span m="2218180">the</span> <span m="2218360">consequence</span>
  <span m="2218900">of</span> <span m="2218960">that</span> <span m="2219200">is</span>
  <span m="2219380">that</span> <span m="2220070">automatically-derived</span> <span
  m="2221090">labels--</span> <span m="2221720">for</span> <span m="2221810">example,</span>
  <span m="2222360">if</span> <span m="2222380">you</span> <span m="2222500">use</span>
  <span m="2222830">one</span> <span m="2222980">of</span> <span m="2223040">those</span>
  <span m="2223850">phenotyping</span> <span m="2224125">algorithms</span> <span m="2224790">I</span>
  <span m="2224870">showed</span> <span m="2225050">you</span> <span m="2225140">earlier,</span>
  <span m="2225570">the</span> <span m="2225670">rules--</span> <span m="2228770">what</span>
  <span m="2229160">the</span> <span m="2229310">label</span> <span m="2229730">is</span>
  <span m="2229910">derived</span> <span m="2230300">for</span> <span m="2230480">over</span>
  <span m="2230690">here</span> <span m="2231680">might</span> <span m="2232010">be</span>
  <span m="2232250">very</span> <span m="2232580">different</span> <span m="2233030">from</span>
  <span m="2233360">the</span> <span m="2233480">label</span> <span m="2233810">that's</span>
  <span m="2233990">derived</span> <span m="2234260">from</span> <span m="2234440">over</span>
  <span m="2234620">here,</span> <span m="2235040">particularly</span> <span m="2235460">if</span>
  <span m="2235520">it's</span> <span m="2235640">using</span> <span m="2235970">data</span>
  <span m="2236720">such</span> <span m="2236930">as</span> <span m="2237080">diagnosis</span>
  <span m="2237620">codes</span> <span m="2238490">that</span> <span m="2238880">have</span>
  <span m="2239060">changed</span> <span m="2239480">in</span> <span m="2239570">meaning</span>
  <span m="2240170">over</span> <span m="2240350">the</span> <span m="2240470">years.</span>
  <span m="2241080">So</span> <span m="2241180">that's</span> <span m="2241280">one</span>
  <span m="2241520">consequence.</span> <span m="2242030">There'll</span> <span m="2242150">be</span>
  <span m="2242240">other</span> <span m="2242390">consequences</span> <span m="2243240">I'll</span>
  <span m="2243260">tell</span> <span m="2243380">you</span> <span m="2243440">about</span>
  <span m="2243560">later.</span></p><p><span m="2244940">Here's</span> <span m="2245180">another</span>
  <span m="2245480">example.</span> <span m="2245720">And by</span> <span m="2245810">the</span>
  <span m="2245870">way,</span> <span m="2245970">this</span> <span m="2246140">notion</span>
  <span m="2246530">is</span> <span m="2246620">called</span> <span m="2246860">non-stationarity,</span>
  <span m="2247970">that</span> <span m="2248150">the</span> <span m="2248240">data</span>
  <span m="2248580">is</span> <span m="2248690">changing</span> <span m="2249200">across</span>
  <span m="2249530">time.</span> <span m="2250080">It's</span> <span m="2250130">not</span>
  <span m="2250400">stationary.</span></p><p><span m="2252170">Here's</span> <span
  m="2252350">another</span> <span m="2252590">example.</span> <span m="2254650">On</span>
  <span m="2254810">the</span> <span m="2254870">x-axis</span> <span m="2255410">again</span>
  <span m="2255620">I'm</span> <span m="2255740">showing</span> <span m="2256160">you</span>
  <span m="2256910">time.</span> <span m="2258490">Here</span> <span m="2258950">each</span>
  <span m="2259490">column</span> <span m="2259980">is</span> <span m="2260780">a</span>
  <span m="2260840">month,</span> <span m="2261290">from</span> <span m="2261440">2005</span>
  <span m="2261775">to</span> <span m="2262110">2014.</span> <span m="2264800">And</span>
  <span m="2265310">on</span> <span m="2265460">the</span> <span m="2265550">y-axis,</span>
  <span m="2268100">for</span> <span m="2268250">every</span> <span m="2268550">sort</span>
  <span m="2268760">of</span> <span m="2268850">row</span> <span m="2269270">of</span>
  <span m="2269390">this</span> <span m="2269540">table,</span> <span m="2269930">I'm</span>
  <span m="2270050">showing</span> <span m="2270380">you</span> <span m="2270530">a</span>
  <span m="2270710">laboratory</span> <span m="2271340">test.</span> <span m="2274170">And</span>
  <span m="2274190">here</span> <span m="2274370">we're</span> <span m="2274460">not</span>
  <span m="2274610">looking</span> <span m="2274940">at</span> <span m="2275060">the</span>
  <span m="2275150">results</span> <span m="2275630">of</span> <span m="2275690">the</span>
  <span m="2275810">lab</span> <span m="2276020">test,</span> <span m="2276440">we're</span>
  <span m="2276560">only</span> <span m="2276800">looking</span> <span m="2277190">at</span>
  <span m="2278030">what</span> <span m="2278330">fraction</span> <span m="2279080">of--</span>
  <span m="2279290">at</span> <span m="2279770">how</span> <span m="2280040">many</span>
  <span m="2280460">lab</span> <span m="2280730">tests</span> <span m="2281270">of</span>
  <span m="2281480">that</span> <span m="2281690">type</span> <span m="2282110">were</span>
  <span m="2282260">performed</span> <span m="2283340">at</span> <span m="2283460">this</span>
  <span m="2283640">point</span> <span m="2283880">in</span> <span m="2283970">time.</span></p><p><span
  m="2286426">And</span> <span m="2286790">now</span> <span m="2286940">you</span>
  <span m="2287060">might</span> <span m="2287240">expect</span> <span m="2287900">that,</span>
  <span m="2288560">broadly</span> <span m="2289010">speaking,</span> <span m="2290510">the</span>
  <span m="2290630">number</span> <span m="2290960">of</span> <span m="2291050">glucose</span>
  <span m="2291590">tests,</span> <span m="2292100">the</span> <span m="2292190">number</span>
  <span m="2292430">of</span> <span m="2292520">white</span> <span m="2292700">blood</span>
  <span m="2292940">cell</span> <span m="2293150">count</span> <span m="2293450">tests,</span>
  <span m="2293900">the</span> <span m="2294020">number</span> <span m="2294620">of</span>
  <span m="2299120">neutrophil</span> <span m="2299810">tests</span> <span m="2300470">and</span>
  <span m="2300590">so</span> <span m="2300860">on</span> <span m="2301040">might</span>
  <span m="2301210">be</span> <span m="2301280">pretty</span> <span m="2301520">constant</span>
  <span m="2301970">across</span> <span m="2302240">time,</span> <span m="2303320">on</span>
  <span m="2303470">average,</span> <span m="2303860">because</span> <span m="2304010">you're</span>
  <span m="2304100">averaging</span> <span m="2304430">over</span> <span m="2304580">lots</span>
  <span m="2304780">of</span> <span m="2304840">people.</span> <span m="2306200">But</span>
  <span m="2306470">indeed</span> <span m="2306800">what</span> <span m="2306920">you</span>
  <span m="2307040">see</span> <span m="2307340">here</span> <span m="2307730">is</span>
  <span m="2307910">that,</span> <span m="2308520">in</span> <span m="2308620">fact,</span>
  <span m="2309090">there</span> <span m="2309230">is</span> <span m="2309410">a</span>
  <span m="2309440">huge</span> <span m="2309950">amount</span> <span m="2310160">of</span>
  <span m="2310250">non-stationarity.</span> <span m="2311210">Which</span> <span
  m="2311510">tests</span> <span m="2312320">are</span> <span m="2312620">ordered</span>
  <span m="2313610">dramatically</span> <span m="2314360">changes</span> <span m="2314840">across</span>
  <span m="2315230">time.</span> <span m="2316230">So</span> <span m="2316310">for</span>
  <span m="2316400">example</span> <span m="2316820">you</span> <span m="2316910">see</span>
  <span m="2317090">this</span> <span m="2317240">one</span> <span m="2317450">line</span>
  <span m="2317630">over</span> <span m="2317750">here,</span> <span m="2319310">where</span>
  <span m="2320180">it's</span> <span m="2320510">all</span> <span m="2320720">blue,</span>
  <span m="2321110">meaning</span> <span m="2321410">no</span> <span m="2321590">one</span>
  <span m="2321680">is</span> <span m="2321800">ordering</span> <span m="2322130">the</span>
  <span m="2322220">test,</span> <span m="2323240">until</span> <span m="2323570">this</span>
  <span m="2323780">point</span> <span m="2323990">in</span> <span m="2324080">time,</span>
  <span m="2324470">when</span> <span m="2324620">people</span> <span m="2324830">start</span>
  <span m="2325040">using</span> <span m="2325370">it.</span> <span m="2326360">What</span>
  <span m="2326480">could</span> <span m="2326630">that</span> <span m="2326810">be?</span>
  <span m="2327550">Any</span> <span m="2328020">ideas?</span> <span m="2329970">Yeah.</span></p><p><span
  m="2330818">AUDIENCE:</span> <span m="2331067">[INAUDIBLE]</span></p><p><span m="2334810">PROFESSOR:</span>
  <span m="2334875">So</span> <span m="2334940">the</span> <span m="2335000">test</span>
  <span m="2335270">was</span> <span m="2335420">used</span> <span m="2335630">less,</span>
  <span m="2335870">or</span> <span m="2336020">really,</span> <span m="2336230">in</span>
  <span m="2336290">this</span> <span m="2336440">case,</span> <span m="2336650">not</span>
  <span m="2336800">used</span> <span m="2337010">at</span> <span m="2337100">all.</span>
  <span m="2337320">And</span> <span m="2337410">then</span> <span m="2337520">suddenly</span>
  <span m="2337830">it</span> <span m="2337880">was</span> <span m="2338030">used.</span>
  <span m="2338330">Why</span> <span m="2338630">might</span> <span m="2338810">that</span>
  <span m="2338990">happen?</span> <span m="2339320">In</span> <span m="2339680">the</span>
  <span m="2339810">back.</span></p><p><span m="2339940">AUDIENCE:</span> <span m="2340113">A</span>
  <span m="2340286">new</span> <span m="2340632">test.</span></p><p><span m="2341690">PROFESSOR:</span>
  <span m="2341720">A</span> <span m="2341750">new</span> <span m="2341900">test,</span>
  <span m="2342500">right,</span> <span m="2343130">because</span> <span m="2343310">technology</span>
  <span m="2343790">changes.</span> <span m="2345090">Suddenly</span> <span m="2345400">we</span>
  <span m="2345500">come</span> <span m="2345620">up</span> <span m="2345680">with</span>
  <span m="2345800">a</span> <span m="2345860">new</span> <span m="2346130">diagnostic</span>
  <span m="2346850">test,</span> <span m="2347220">a</span> <span m="2347320">new</span>
  <span m="2347390">lab</span> <span m="2347660">test.</span> <span m="2348770">And</span>
  <span m="2349940">we</span> <span m="2350070">can</span> <span m="2350150">start</span>
  <span m="2350300">using</span> <span m="2350570">it, where it</span> <span m="2350840">didn't</span>
  <span m="2351020">exist</span> <span m="2351290">before.</span> <span m="2351620">So
  obviously</span> <span m="2351920">there was</span> <span m="2352100">no</span>
  <span m="2352220">data</span> <span m="2352400">on</span> <span m="2352520">it</span>
  <span m="2352580">before.</span> <span m="2353010">What's</span> <span m="2353030">another</span>
  <span m="2353300">reason</span> <span m="2353630">why</span> <span m="2353850">it</span>
  <span m="2353930">might</span> <span m="2354260">have</span> <span m="2354470">suddenly</span>
  <span m="2354770">showed</span> <span m="2355010">up?</span> <span m="2357014">Yep.</span></p><p><span
  m="2357926">AUDIENCE:</span> <span m="2358040">It</span> <span m="2358154">could</span>
  <span m="2358268">be</span> <span m="2358382">like</span> <span m="2359020">annual</span>
  <span m="2359790">check-ups</span> <span m="2360270">become</span> <span m="2361406">mandatory,</span>
  <span m="2362894">or</span> <span m="2363390">that</span> <span m="2363870">it's</span>
  <span m="2364070">part</span> <span m="2364340">of</span> <span m="2364560">the</span>
  <span m="2364997">test</span> <span m="2365434">admission</span> <span m="2365871">at</span>
  <span m="2366310">hospital.</span> <span m="2366510">Like,</span> <span m="2366968">it's</span>
  <span m="2367426">an</span> <span m="2367884">additional test.</span></p><p><span
  m="2368800">PROFESSOR:</span> <span m="2368845">I'll</span> <span m="2368890">stick</span>
  <span m="2369100">with</span> <span m="2369190">your</span> <span m="2369280">first</span>
  <span m="2369550">example.</span> <span m="2371020">Maybe</span> <span m="2371500">that</span>
  <span m="2371650">test</span> <span m="2371950">becomes</span> <span m="2372400">mandatory.</span>
  <span m="2373420">OK,</span> <span m="2373810">so</span> <span m="2373990">maybe</span>
  <span m="2374410">there's</span> <span m="2374590">a</span> <span m="2374650">clinical</span>
  <span m="2375100">guideline</span> <span m="2375880">that</span> <span m="2377110">is</span>
  <span m="2377230">created</span> <span m="2377890">at</span> <span m="2378010">this</span>
  <span m="2378190">point</span> <span m="2378400">in</span> <span m="2378520">time,</span>
  <span m="2380050">right</span> <span m="2380290">there.</span> <span m="2381490">And</span>
  <span m="2382000">health</span> <span m="2382330">insurers</span> <span m="2383230">decide</span>
  <span m="2384070">we're</span> <span m="2384250">going</span> <span m="2384490">to</span>
  <span m="2384610">reimburse</span> <span m="2385450">for</span> <span m="2385630">this</span>
  <span m="2385840">test</span> <span m="2386710">at</span> <span m="2386830">this</span>
  <span m="2386980">point</span> <span m="2387160">in</span> <span m="2387250">time.</span>
  <span m="2387895">And</span> <span m="2388210">the</span> <span m="2388300">test</span>
  <span m="2388510">might've</span> <span m="2388660">been</span> <span m="2388750">really</span>
  <span m="2388930">expensive.</span> <span m="2389480">So</span> <span m="2389500">no</span>
  <span m="2389830">one</span> <span m="2390130">would</span> <span m="2390250">have</span>
  <span m="2390370">done</span> <span m="2390610">it</span> <span m="2390700">beforehand.</span>
  <span m="2391670">And</span> <span m="2391690">now</span> <span m="2391870">that</span>
  <span m="2392020">the</span> <span m="2392110">health</span> <span m="2392290">insurance</span>
  <span m="2392590">companies</span> <span m="2392830">are</span> <span m="2392860">going</span>
  <span m="2392970">to</span> <span m="2393040">pay</span> <span m="2393220">for</span>
  <span m="2393400">it,</span> <span m="2393580">now</span> <span m="2393790">people</span>
  <span m="2394030">start</span> <span m="2394210">doing</span> <span m="2394390">it.</span>
  <span m="2394480">So</span> <span m="2394580">it</span> <span m="2394620">might</span>
  <span m="2394750">have</span> <span m="2394840">existed</span> <span m="2395290">beforehand.</span>
  <span m="2396190">But</span> <span m="2396610">if</span> <span m="2396700">no</span>
  <span m="2396820">one</span> <span m="2396910">would</span> <span m="2396970">pay</span>
  <span m="2397150">for</span> <span m="2397270">it,</span> <span m="2397430">no</span>
  <span m="2397530">one</span> <span m="2397540">would</span> <span m="2397630">use</span>
  <span m="2397810">it.</span></p><p><span m="2399790">What's</span> <span m="2400210">another</span>
  <span m="2400720">reason</span> <span m="2401080">why</span> <span m="2401260">you</span>
  <span m="2401350">might</span> <span m="2401560">see</span> <span m="2401770">something</span>
  <span m="2402100">like</span> <span m="2402280">this,</span> <span m="2402460">or</span>
  <span m="2402520">maybe</span> <span m="2402730">even</span> <span m="2402940">a</span>
  <span m="2403000">gap</span> <span m="2403450">like</span> <span m="2403690">this?</span>
  <span m="2404380">Notice,</span> <span m="2404650">here in</span> <span m="2404770">the</span>
  <span m="2404860">middle,</span> <span m="2405170">there's</span> <span m="2405220">this</span>
  <span m="2405370">huge</span> <span m="2405700">gap</span> <span m="2406030">in</span>
  <span m="2406120">the</span> <span m="2406180">middle.</span> <span m="2406370">What</span>
  <span m="2406570">might</span> <span m="2406720">have</span> <span m="2406840">explained</span>
  <span m="2407290">that?</span></p><p><span m="2416580">AUDIENCE:</span> <span m="2416650">[INAUDIBLE]</span></p><p><span
  m="2417070">PROFESSOR:</span> <span m="2417173">Hold</span> <span m="2417276">on.</span>
  <span m="2417710">Yep, over</span> <span m="2418070">here.</span></p><p><span m="2419910">AUDIENCE:</span>
  <span m="2420063">Maybe</span> <span m="2420216">your</span> <span m="2420370">patient</span>
  <span m="2420700">population</span> <span m="2421490">is</span> <span m="2421670">mostly
  of</span> <span m="2422120">a</span> <span m="2422250">certain</span> <span m="2422660">age,</span>
  <span m="2422925">and</span> <span m="2423790">coverage</span> <span m="2424290">for</span>
  <span m="2424748">something</span> <span m="2425206">changes</span> <span m="2426122">once</span>
  <span m="2427038">your age</span> <span m="2427496">crosses a</span> <span m="2427954">threshold.</span></p><p><span
  m="2428870">PROFESSOR:</span> <span m="2429055">Yeah,</span> <span m="2429240">so</span>
  <span m="2429550">one</span> <span m="2429790">explanation--</span> <span m="2430540">I</span>
  <span m="2430630">think</span> <span m="2431260">it's</span> <span m="2431500">not</span>
  <span m="2431710">plausible</span> <span m="2432070">in</span> <span m="2432130">this</span>
  <span m="2432280">data</span> <span m="2432450">set,</span> <span m="2432610">but</span>
  <span m="2432700">it</span> <span m="2432760">is</span> <span m="2432850">plausible</span>
  <span m="2433150">for</span> <span m="2433240">some</span> <span m="2433420">data</span>
  <span m="2433690">sets--</span> <span m="2434410">is</span> <span m="2434650">that</span>
  <span m="2435220">maybe</span> <span m="2438400">your</span> <span m="2438580">patients</span>
  <span m="2439570">at</span> <span m="2439720">time</span> <span m="2440030">0</span>
  <span m="2440380">were</span> <span m="2440650">all</span> <span m="2440910">of</span>
  <span m="2440980">exactly</span> <span m="2441460">the</span> <span m="2441550">same</span>
  <span m="2442000">age.</span> <span m="2442970">So</span> <span m="2443080">maybe</span>
  <span m="2443290">there's</span> <span m="2443410">some</span> <span m="2443590">amount</span>
  <span m="2443800">of</span> <span m="2443890">alignment.</span> <span m="2444610">And</span>
  <span m="2444850">suddenly,</span> <span m="2445420">at</span> <span m="2445540">this</span>
  <span m="2445750">point</span> <span m="2445990">in</span> <span m="2446110">time,</span>
  <span m="2447970">let's</span> <span m="2448180">say,</span> <span m="2449740">women</span>
  <span m="2450040">only</span> <span m="2450280">get,</span> <span m="2450520">let's</span>
  <span m="2450700">say,</span> <span m="2450970">their</span> <span m="2451720">annual</span>
  <span m="2452020">mammography</span> <span m="2452590">once</span> <span m="2452770">they</span>
  <span m="2452860">turn</span> <span m="2453070">a</span> <span m="2453100">certain</span>
  <span m="2453310">age.</span> <span m="2453700">And</span> <span m="2454200">so</span>
  <span m="2454300">that</span> <span m="2454720">might</span> <span m="2454840">be</span>
  <span m="2454960">one</span> <span m="2455140">reason</span> <span m="2455500">why</span>
  <span m="2455920">you</span> <span m="2456040">would</span> <span m="2456160">see</span>
  <span m="2456370">nothing</span> <span m="2457420">until</span> <span m="2458410">one</span>
  <span m="2458620">point</span> <span m="2458770">in</span> <span m="2458860">time.</span>
  <span m="2459160">And</span> <span m="2459250">maybe</span> <span m="2459430">that</span>
  <span m="2459550">would</span> <span m="2459670">change</span> <span m="2460030">across</span>
  <span m="2460330">time</span> <span m="2460510">as</span> <span m="2460570">well.</span>
  <span m="2460720">Maybe</span> <span m="2460870">they'll</span> <span m="2460960">stop</span>
  <span m="2461230">getting</span> <span m="2461470">it at</span> <span m="2461560">some</span>
  <span m="2461740">point</span> <span m="2461920">after</span> <span m="2463260">menopause.</span>
  <span m="2463840">That's</span> <span m="2463990">not</span> <span m="2464200">true,</span>
  <span m="2464500">but</span> <span m="2464830">let's</span> <span m="2464980">say.</span></p><p><span
  m="2467770">So</span> <span m="2467950">that's</span> <span m="2468130">one</span>
  <span m="2468310">explanation.</span> <span m="2468610">In</span> <span m="2468670">this</span>
  <span m="2468820">case,</span> <span m="2469140">it</span> <span m="2469240">doesn't</span>
  <span m="2469330">make</span> <span m="2469480">sense,</span> <span m="2469750">because</span>
  <span m="2470460">the</span> <span m="2471070">patient</span> <span m="2471340">population</span>
  <span m="2471880">is</span> <span m="2471970">very</span> <span m="2472150">mixed.</span>
  <span m="2472690">So</span> <span m="2473050">you</span> <span m="2473170">could</span>
  <span m="2473290">think</span> <span m="2473440">about</span> <span m="2473540">it</span>
  <span m="2473660">as</span> <span m="2473770">being</span> <span m="2473980">roughly</span>
  <span m="2474260">at</span> <span m="2474320">steady</span> <span m="2474610">state.</span>
  <span m="2475060">So</span> <span m="2475240">they're</span> <span m="2475330">not--</span>
  <span m="2475570">you'll</span> <span m="2475830">have</span> <span m="2476210">patients</span>
  <span m="2476530">of</span> <span m="2476620">all</span> <span m="2476800">ages</span>
  <span m="2477190">here.</span></p><p><span m="2478060">What's</span> <span m="2478240">another</span>
  <span m="2478450">reason?</span> <span m="2479280">Someone</span> <span m="2479530">raised</span>
  <span m="2479740">their</span> <span m="2479830">hand</span> <span m="2479950">over</span>
  <span m="2480100">here.</span> <span m="2480990">Yep.</span></p><p><span m="2481520">AUDIENCE:</span>
  <span m="2481595">Yeah,</span> <span m="2481670">I</span> <span m="2481720">was</span>
  <span m="2481840">just</span> <span m="2481960">going</span> <span m="2482080">to</span>
  <span m="2482140">say,</span> <span m="2483600">maybe</span> <span m="2483870">the</span>
  <span m="2484220">EMR</span> <span m="2484630">shut</span> <span m="2484900">down</span>
  <span m="2485140">for</span> <span m="2485320">awhile,</span> <span m="2485610">and</span>
  <span m="2485890">so</span> <span m="2486100">they</span> <span m="2486200">were</span>
  <span m="2486310">only</span> <span m="2486550">doing</span> <span m="2486760">stuff</span>
  <span m="2487000">on</span> <span m="2487210">paper,</span> <span m="2487660">and</span>
  <span m="2488070">they only</span> <span m="2488480">were able to record 4 things.</span></p><p><span
  m="2489710">PROFESSOR:</span> <span m="2489810">Ding</span> <span m="2489910">ding</span>
  <span m="2490090">ding</span> <span m="2490250">ding</span> <span m="2490470">ding.</span>
  <span m="2490840">Yes,</span> <span m="2491620">that's</span> <span m="2491770">right.</span>
  <span m="2492340">So</span> <span m="2493840">maybe</span> <span m="2494350">the</span>
  <span m="2494540">EMR</span> <span m="2495460">shut</span> <span m="2495700">down.</span>
  <span m="2496740">Or</span> <span m="2496840">in</span> <span m="2496930">this</span>
  <span m="2497110">case,</span> <span m="2498250">we</span> <span m="2498580">had</span>
  <span m="2498730">data</span> <span m="2499030">issues.</span> <span m="2500100">So</span>
  <span m="2502030">this</span> <span m="2502420">data</span> <span m="2502660">was</span>
  <span m="2502780">acquired</span> <span m="2503170">somehow.</span> <span m="2503830">For</span>
  <span m="2503980">example,</span> <span m="2504880">maybe</span> <span m="2505180">it</span>
  <span m="2505240">was</span> <span m="2505450">required</span> <span m="2505930">through</span>
  <span m="2506140">a</span> <span m="2506170">contract</span> <span m="2506890">with</span>
  <span m="2507130">something</span> <span m="2507460">like</span> <span m="2507680">Webquest</span>
  <span m="2509200">or</span> <span m="2509290">LabCorp.</span> <span m="2510460">And</span>
  <span m="2511270">maybe,</span> <span m="2512200">during</span> <span m="2512650">that</span>
  <span m="2512950">four-month</span> <span m="2513490">interval,</span> <span m="2514510">there</span>
  <span m="2514660">was</span> <span m="2514810">contract</span> <span m="2515170">negotiation.</span>
  <span m="2516390">And</span> <span m="2516490">so</span> <span m="2516610">suddenly</span>
  <span m="2516970">we</span> <span m="2517090">couldn't</span> <span m="2517390">get</span>
  <span m="2517570">the</span></p><p><span m="2517660">Data</span> <span m="2517870">for</span>
  <span m="2517960">that</span> <span m="2518080">time</span> <span m="2518290">period.</span>
  <span m="2519100">Or</span> <span m="2519280">maybe</span> <span m="2519940">our</span>
  <span m="2520030">databases</span> <span m="2520660">crashed,</span> <span m="2521070">and</span>
  <span m="2521130">we</span> <span m="2521200">suddenly</span> <span m="2521470">lost</span>
  <span m="2522010">all</span> <span m="2522180">the</span> <span m="2522220">data</span>
  <span m="2522520">for</span> <span m="2522610">that</span> <span m="2522730">time</span>
  <span m="2522940">period.</span> <span m="2523480">This</span> <span m="2523720">happens,</span>
  <span m="2524050">and</span> <span m="2524140">this</span> <span m="2524260">happens</span>
  <span m="2524830">all</span> <span m="2525220">the</span> <span m="2525340">time,</span>
  <span m="2525850">and</span> <span m="2526000">not</span> <span m="2526150">just</span>
  <span m="2526330">the</span> <span m="2526390">health</span> <span m="2526490">care</span>
  <span m="2526750">industry,</span> <span m="2527150">but</span> <span m="2527170">other</span>
  <span m="2527320">industries</span> <span m="2527740">as</span> <span m="2527860">well.</span></p><p><span
  m="2529060">And</span> <span m="2529310">as</span> <span m="2529360">a</span> <span
  m="2529390">result</span> <span m="2529780">of</span> <span m="2529870">those</span>
  <span m="2530050">systemic-type</span> <span m="2531220">changes,</span> <span m="2532210">your</span>
  <span m="2532360">data</span> <span m="2532660">is</span> <span m="2532780">also</span>
  <span m="2533050">going</span> <span m="2533170">to</span> <span m="2533230">be</span>
  <span m="2533290">non-stationary</span> <span m="2534700">across</span> <span m="2535030">time.</span>
  <span m="2536180">So</span> <span m="2536280">now</span> <span m="2536350">we've</span>
  <span m="2536500">seen</span> <span m="2536710">three</span> <span m="2536980">or</span>
  <span m="2537040">four</span> <span m="2537220">different</span> <span m="2537790">explanations</span>
  <span m="2538420">for</span> <span m="2538600">why</span> <span m="2538840">this</span>
  <span m="2538990">happens.</span> <span m="2539540">And</span> <span m="2539680">the</span>
  <span m="2539770">reality</span> <span m="2540160">is</span> <span m="2540280">really</span>
  <span m="2540490">a</span> <span m="2540520">mixture</span> <span m="2540850">of</span>
  <span m="2540970">all</span> <span m="2541150">of</span> <span m="2541240">these.</span></p><p><span
  m="2543720">And</span> <span m="2543850">just</span> <span m="2544030">as</span>
  <span m="2544150">in</span> <span m="2544240">the</span> <span m="2544300">previous--</span>
  <span m="2545230">so</span> <span m="2545350">in</span> <span m="2545410">the</span>
  <span m="2545470">previous</span> <span m="2545740">example,</span> <span m="2546290">notice</span>
  <span m="2546550">how</span> <span m="2546730">what</span> <span m="2546940">really</span>
  <span m="2547120">changed</span> <span m="2547420">here</span> <span m="2547540">is</span>
  <span m="2547630">that</span> <span m="2547750">the</span> <span m="2547850">derived</span>
  <span m="2548260">labels</span> <span m="2548860">might</span> <span m="2549010">change</span>
  <span m="2549280">meaning</span> <span m="2549500">across</span> <span m="2549790">time.</span>
  <span m="2550830">Now</span> <span m="2553330">the</span> <span m="2553450">significance</span>
  <span m="2554110">of</span> <span m="2554230">the</span> <span m="2554350">features</span>
  <span m="2554930">used</span> <span m="2555140">in</span> <span m="2555220">the</span>
  <span m="2555280">machine</span> <span m="2555580">learning</span> <span m="2555940">models</span>
  <span m="2556690">would</span> <span m="2556870">really</span> <span m="2557050">change</span>
  <span m="2557350">across</span> <span m="2557680">time.</span> <span m="2558200">And</span>
  <span m="2558300">that's</span> <span m="2558430">one</span> <span m="2558610">of</span>
  <span m="2558700">the</span> <span m="2558790">consequences</span> <span m="2559480">of</span>
  <span m="2559600">this,</span> <span m="2559840">particular</span> <span m="2560210">if
  you're</span> <span m="2560320">driving</span> <span m="2561220">features</span>
  <span m="2561700">from</span> <span m="2561880">lab</span> <span m="2562090">test</span>
  <span m="2562570">values.</span></p><p><span m="2564090">Here's</span> <span m="2564550">one</span>
  <span m="2564850">last</span> <span m="2565120">example.</span> <span m="2567790">Again,</span>
  <span m="2568180">on</span> <span m="2568270">the x-axis</span> <span m="2568780">here,</span>
  <span m="2568900">I</span> <span m="2568990">have</span> <span m="2569170">time.</span>
  <span m="2570430">On</span> <span m="2570580">the</span> <span m="2570670">y-axis</span>
  <span m="2571300">here,</span> <span m="2571540">I'm</span> <span m="2571660">showing</span>
  <span m="2572110">the</span> <span m="2572230">number</span> <span m="2572710">of</span>
  <span m="2572830">times</span> <span m="2573460">that</span> <span m="2573640">you</span>
  <span m="2574780">observed</span> <span m="2575620">some</span> <span m="2576430">diagnosis</span>
  <span m="2577090">code</span> <span m="2577390">of</span> <span m="2577540">some</span>
  <span m="2577780">kind.</span> <span m="2578780">This</span> <span m="2579160">cyan</span>
  <span m="2579730">line</span> <span m="2580120">is</span> <span m="2580270">ICD-9</span>
  <span m="2581020">codes.</span> <span m="2581530">And</span> <span m="2581770">this</span>
  <span m="2582100">red</span> <span m="2582640">line</span> <span m="2583080">are</span>
  <span m="2583240">ICD-10</span> <span m="2584230">codes.</span> <span m="2585220">You</span>
  <span m="2585310">might</span> <span m="2585460">remember</span> <span m="2585790">that</span>
  <span m="2586150">Pete</span> <span m="2586420">mentioned</span> <span m="2586750">in</span>
  <span m="2586810">an</span> <span m="2586900">earlier</span> <span m="2587170">lecture</span>
  <span m="2587590">that</span> <span m="2587740">there</span> <span m="2587860">was</span>
  <span m="2587980">a</span> <span m="2588040">big</span> <span m="2588220">shift</span>
  <span m="2588670">from</span> <span m="2588940">ICD-9</span> <span m="2589540">coding</span>
  <span m="2589900">to</span> <span m="2589990">ICD-10</span> <span m="2590590">coding</span>
  <span m="2591340">at</span> <span m="2591490">some</span> <span m="2591670">point.</span>
  <span m="2592060">When</span> <span m="2592270">was</span> <span m="2592360">that</span>
  <span m="2592480">time?</span> <span m="2592840">It</span> <span m="2592930">was</span>
  <span m="2593110">precisely</span> <span m="2594160">this</span> <span m="2594370">time.</span></p><p><span
  m="2595820">And</span> <span m="2595920">so</span> <span m="2596020">if</span> <span
  m="2596120">you</span> <span m="2596220">think</span> <span m="2596230">about</span>
  <span m="2596410">the</span> <span m="2596500">feature</span> <span m="2596860">vector</span>
  <span m="2597280">that</span> <span m="2597460">you</span> <span m="2597590">would</span>
  <span m="2597670">derive</span> <span m="2598150">for</span> <span m="2598280">your</span>
  <span m="2598360">machine</span> <span m="2598690">learning</span> <span m="2598930">problem,</span>
  <span m="2600010">you</span> <span m="2600130">would</span> <span m="2600220">have</span>
  <span m="2600760">one</span> <span m="2601030">feature</span> <span m="2601450">for</span>
  <span m="2601600">all</span> <span m="2601780">ICD-9</span> <span m="2602440">codes,</span>
  <span m="2602950">and</span> <span m="2603040">one--</span> <span m="2603740">a</span>
  <span m="2603780">whole</span> <span m="2603880">set</span> <span m="2604060">of</span>
  <span m="2604120">features</span> <span m="2604450">for</span> <span m="2604540">all</span>
  <span m="2604660">ICD-10</span> <span m="2605230">codes.</span> <span m="2606190">And</span>
  <span m="2606550">those</span> <span m="2606760">ICD-9-based</span> <span m="2607520">features</span>
  <span m="2607870">are</span> <span m="2607930">going</span> <span m="2608200">to</span>
  <span m="2608320">be--</span> <span m="2608710">they're</span> <span m="2609250">going</span>
  <span m="2609370">to</span> <span m="2609440">be</span> <span m="2609510">used</span>
  <span m="2609790">quite</span> <span m="2610000">a</span> <span m="2610030">bit</span>
  <span m="2610120">in</span> <span m="2610210">this</span> <span m="2610330">time</span>
  <span m="2610570">period.</span> <span m="2611000">And</span> <span m="2611100">then</span>
  <span m="2611200">suddenly</span> <span m="2611470">they're</span> <span m="2611560">going</span>
  <span m="2611710">to</span> <span m="2611770">be</span> <span m="2611860">completely</span>
  <span m="2612640">sparse</span> <span m="2613480">in</span> <span m="2613570">this</span>
  <span m="2613690">time</span> <span m="2613870">period.</span> <span m="2614690">And</span>
  <span m="2614800">ICD-10</span> <span m="2615430">features</span> <span m="2615790">start</span>
  <span m="2616060">to</span> <span m="2616150">become</span> <span m="2616450">used.</span>
  <span m="2617820">And</span> <span m="2617980">you</span> <span m="2618040">could</span>
  <span m="2618130">imagine</span> <span m="2618580">that</span> <span m="2618790">if</span>
  <span m="2618910">you</span> <span m="2619000">did</span> <span m="2619210">machine</span>
  <span m="2619570">learning</span> <span m="2619990">using</span> <span m="2622260">just</span>
  <span m="2622480">ICD-9</span> <span m="2623380">data,</span> <span m="2623890">and</span>
  <span m="2624010">then</span> <span m="2624130">you</span> <span m="2624340">tried</span>
  <span m="2624580">to</span> <span m="2624640">apply</span> <span m="2624970">your</span>
  <span m="2625090">model</span> <span m="2626020">at</span> <span m="2626110">this</span>
  <span m="2626290">point</span> <span m="2626500">in</span> <span m="2626560">time,</span>
  <span m="2627340">it's</span> <span m="2627460">going</span> <span m="2627540">to</span>
  <span m="2627670">do</span> <span m="2627790">horribly,</span> <span m="2628330">because</span>
  <span m="2628660">it's</span> <span m="2628840">expecting</span> <span m="2629260">features</span>
  <span m="2629590">that</span> <span m="2629710">it</span> <span m="2629770">no</span>
  <span m="2629890">longer</span> <span m="2630100">has</span> <span m="2630280">access</span>
  <span m="2630670">to.</span> <span m="2631780">And</span> <span m="2632230">this</span>
  <span m="2632440">happens</span> <span m="2632920">all</span> <span m="2633010">the</span>
  <span m="2633100">time.</span></p><p><span m="2633370">And</span> <span m="2633460">in</span>
  <span m="2633550">fact,</span> <span m="2634160">what</span> <span m="2634210">I'm</span>
  <span m="2634270">describing</span> <span m="2634660">here</span> <span m="2634900">is</span>
  <span m="2635020">actually</span> <span m="2635290">a</span> <span m="2635350">major</span>
  <span m="2635950">problem</span> <span m="2636340">for</span> <span m="2636460">the</span>
  <span m="2636520">whole</span> <span m="2636730">health care</span> <span m="2637090">industry.</span>
  <span m="2638020">For</span> <span m="2638140">the</span> <span m="2638200">next</span>
  <span m="2638440">five</span> <span m="2638770">years,</span> <span m="2639130">everyone</span>
  <span m="2639520">is</span> <span m="2639590">going</span> <span m="2639670">to</span>
  <span m="2639760">grapple</span> <span m="2640060">with</span> <span m="2640180">this</span>
  <span m="2640330">problem,</span> <span m="2640990">because</span> <span m="2641230">they</span>
  <span m="2641350">want</span> <span m="2641590">to</span> <span m="2641710">use</span>
  <span m="2642010">their</span> <span m="2642100">historical</span> <span m="2642640">data</span>
  <span m="2642850">for</span> <span m="2642940">machine</span> <span m="2643240">learning,</span>
  <span m="2643510">but</span> <span m="2643750">their</span> <span m="2643870">historical</span>
  <span m="2644320">data</span> <span m="2644500">is</span> <span m="2644590">very</span>
  <span m="2644770">different</span> <span m="2645100">from</span> <span m="2645250">their</span>
  <span m="2645490">recent</span> <span m="2645820">data.</span></p><p><span m="2648270">So</span>
  <span m="2650090">now,</span> <span m="2651170">in</span> <span m="2651290">the</span>
  <span m="2651350">face</span> <span m="2651770">of</span> <span m="2651950">all</span>
  <span m="2652130">of</span> <span m="2652220">this</span> <span m="2652370">non-stationarity</span>
  <span m="2653200">that</span> <span m="2653320">I</span> <span m="2653390">just</span>
  <span m="2653540">described,</span> <span m="2655040">did</span> <span m="2655190">we</span>
  <span m="2655310">do</span> <span m="2655490">anything</span> <span m="2655940">wrong</span>
  <span m="2656710">in</span> <span m="2656840">the</span> <span m="2656930">diabetes</span>
  <span m="2657560">risk</span> <span m="2657760">stratification</span> <span m="2658220">problem</span>
  <span m="2658610">that</span> <span m="2658850">I</span> <span m="2659870">told</span>
  <span m="2660170">you</span> <span m="2660230">about</span> <span m="2660500">earlier?</span>
  <span m="2662070">Thoughts.</span> <span m="2665300">That</span> <span m="2665420">was</span>
  <span m="2665510">my</span> <span m="2665690">paper,</span> <span m="2665930">by</span>
  <span m="2665990">the</span> <span m="2666060">way.</span> <span m="2666300">Did</span>
  <span m="2666320">I</span> <span m="2666410">make</span> <span m="2666620">an</span>
  <span m="2666710">error?</span> <span m="2669110">Thoughts.</span> <span m="2676990">Don't</span>
  <span m="2677170">be</span> <span m="2677260">afraid.</span> <span m="2677850">I'm</span>
  <span m="2678280">often</span> <span m="2678550">wrong.</span> <span m="2686300">I'm</span>
  <span m="2686420">just</span> <span m="2686570">asking</span> <span m="2686900">specifically</span>
  <span m="2687350">about</span> <span m="2687500">the</span> <span m="2687560">way</span>
  <span m="2687710">I</span> <span m="2687800">evaluated</span> <span m="2688490">the</span>
  <span m="2688580">models.</span> <span m="2691490">Yep.</span></p><p><span m="2691700">AUDIENCE:</span>
  <span m="2691838">This</span> <span m="2691976">wasn't</span> <span m="2692116">an
  error,</span> <span m="2692950">but</span> <span m="2693210">one thing,</span> <span
  m="2694551">like</span> <span m="2694998">if I</span> <span m="2695445">was a doctor</span>
  <span m="2695892">I would</span> <span m="2696340">like</span> <span m="2696650">to
  see</span> <span m="2696920">is</span> <span m="2697150">the</span> <span m="2697626">sensitivity</span>
  <span m="2698102">to--</span> <span m="2699054">like, the</span> <span m="2699530">inclusion</span>
  <span m="2700006">criteria</span> <span m="2700482">if</span> <span m="2700958">I</span>
  <span m="2701434">remove</span> <span m="2701910">the</span> <span m="2702386">HBA1C</span>
  <span m="2703350">for instance.</span> <span m="2704710">Like</span> <span m="2705110">most</span>
  <span m="2705260">people,</span> <span m="2705660">they</span> <span m="2706060">have</span>
  <span m="2706460">compared</span> <span m="2706860">to</span> <span m="2707040">having</span>
  <span m="2707512">either</span> <span m="2707984">Rx</span> <span m="2708456">or</span>
  <span m="2708928">[INAUDIBLE]</span> <span m="2709872">then</span> <span m="2710816">kind
  of</span> <span m="2711288">evaluating</span> <span m="2711760">the--</span></p><p><span
  m="2712240">PROFESSOR:</span> <span m="2712380">So</span> <span m="2712520">understanding</span>
  <span m="2712940">the</span> <span m="2713000">robustness</span> <span m="2713720">to</span>
  <span m="2714110">changing</span> <span m="2714590">the</span> <span m="2714650">data</span>
  <span m="2714935">a bit</span> <span m="2715220">is</span> <span m="2715310">something</span>
  <span m="2715610">that</span> <span m="2715730">would</span> <span m="2715910">be</span>
  <span m="2716110">of</span> <span m="2716600">a</span> <span m="2716630">lot</span>
  <span m="2716810">of</span> <span m="2716900">interest.</span> <span m="2717350">I</span>
  <span m="2717450">agree.</span> <span m="2718580">But</span> <span m="2718760">that's</span>
  <span m="2718910">not</span> <span m="2719090">immediately</span> <span m="2719510">suggested</span>
  <span m="2719960">by</span> <span m="2720080">the</span> <span m="2720140">non-stationarity</span>
  <span m="2720830">results.</span> <span m="2721720">Not</span> <span m="2721880">something</span>
  <span m="2722120">that's</span> <span m="2722300">suggested</span> <span m="2722750">by</span>
  <span m="2722840">non-stationarity</span> <span m="2723380">results.</span></p><p><span
  m="2725480">Our TA</span> <span m="2725870">in</span> <span m="2725960">the</span>
  <span m="2726020">front</span> <span m="2726200">row</span> <span m="2726380">has</span>
  <span m="2726500">an</span> <span m="2726560">idea.</span> <span m="2726830">Yeah,</span>
  <span m="2727010">let's</span> <span m="2727160">hear</span> <span m="2727310">it.</span></p><p><span
  m="2727830">AUDIENCE:</span> <span m="2727900">The</span> <span m="2727970">train</span>
  <span m="2728450">and test</span> <span m="2728660">distributions</span> <span m="2729760">were</span>
  <span m="2729910">drawn</span> <span m="2730340">from</span> <span m="2730660">the
  same-- or the</span> <span m="2731080">train and</span> <span m="2731420">tests</span>
  <span m="2731710">were</span> <span m="2731850">drawn</span> <span m="2732130">from
  the same</span> <span m="2732420">distribution.</span></p><p><span m="2733590">PROFESSOR:</span>
  <span m="2733690">So</span> <span m="2733790">in</span> <span m="2733910">the</span>
  <span m="2734000">way</span> <span m="2734180">that</span> <span m="2734300">we</span>
  <span m="2734360">did</span> <span m="2734480">our</span> <span m="2734570">evaluation</span>
  <span m="2735080">there,</span> <span m="2735920">we</span> <span m="2736070">said,</span>
  <span m="2736380">OK,</span> <span m="2739190">we're</span> <span m="2739340">going</span>
  <span m="2739640">to</span> <span m="2740750">set</span> <span m="2741110">it</span>
  <span m="2741230">up</span> <span m="2741380">such</span> <span m="2741650">that</span>
  <span m="2741790">on</span> <span m="2741890">January</span> <span m="2742430">1,</span>
  <span m="2742760">2009,</span> <span m="2743480">we're</span> <span m="2743570">predicting</span>
  <span m="2743990">what's</span> <span m="2744150">going</span> <span m="2744280">to</span>
  <span m="2744320">happen</span> <span m="2744710">in</span> <span m="2744800">the</span>
  <span m="2744860">following</span> <span m="2745520">three</span> <span m="2745820">years.</span>
  <span m="2747350">And</span> <span m="2747830">we</span> <span m="2748250">segmented</span>
  <span m="2748970">our</span> <span m="2749090">patient</span> <span m="2749480">population</span>
  <span m="2750140">into</span> <span m="2750380">train,</span> <span m="2750770">validate,</span>
  <span m="2751130">and</span> <span m="2751220">test,</span> <span m="2752580">but</span>
  <span m="2752660">at</span> <span m="2752780">all</span> <span m="2753050">times,</span>
  <span m="2753800">using</span> <span m="2754610">that</span> <span m="2754940">same</span>
  <span m="2755240">setup,</span> <span m="2755750">January</span> <span m="2756080">1</span>
  <span m="2756530">2009,</span> <span m="2757370">as</span> <span m="2757550">the</span>
  <span m="2757640">prediction</span> <span m="2758030">time.</span></p><p><span m="2760040">Now,</span>
  <span m="2760430">we</span> <span m="2760580">learned</span> <span m="2760910">this</span>
  <span m="2761120">model,</span> <span m="2762230">and</span> <span m="2762380">it's</span>
  <span m="2762530">now</span> <span m="2762830">2018.</span> <span m="2764570">We</span>
  <span m="2764660">want</span> <span m="2764840">to</span> <span m="2764930">apply</span>
  <span m="2765230">this</span> <span m="2765410">model</span> <span m="2765710">today.</span>
  <span m="2767000">And</span> <span m="2767540">I</span> <span m="2767720">computed</span>
  <span m="2768350">an</span> <span m="2768470">area</span> <span m="2768740">under</span>
  <span m="2768890">the</span> <span m="2768980">ROC</span> <span m="2769250">curve.</span>
  <span m="2769430">I</span> <span m="2769500">computed</span> <span m="2770030">positive</span>
  <span m="2770450">predictive</span> <span m="2770750">values</span> <span m="2771650">using</span>
  <span m="2771980">that</span> <span m="2772250">retrospective</span> <span m="2772790">data.</span>
  <span m="2773690">And</span> <span m="2773870">I</span> <span m="2774380">handed</span>
  <span m="2774710">those</span> <span m="2774980">off</span> <span m="2775310">to</span>
  <span m="2775670">my</span> <span m="2775940">partners.</span> <span m="2777650">And</span>
  <span m="2777770">they</span> <span m="2777890">might</span> <span m="2778100">hope</span>
  <span m="2778550">that</span> <span m="2778730">those</span> <span m="2778970">numbers</span>
  <span m="2779330">are</span> <span m="2779390">reflective</span> <span m="2780170">of</span>
  <span m="2780320">what</span> <span m="2780530">their</span> <span m="2780680">models</span>
  <span m="2781010">would</span> <span m="2781130">do</span> <span m="2781490">today.</span>
  <span m="2783390">But</span> <span m="2783410">because</span> <span m="2783770">of</span>
  <span m="2783860">these</span> <span m="2784040">issues</span> <span m="2784560">I</span>
  <span m="2784660">just</span> <span m="2784670">told</span> <span m="2785000">you</span>
  <span m="2785150">about--</span> <span m="2786090">for</span> <span m="2786190">example,</span>
  <span m="2786630">that</span> <span m="2786710">the</span> <span m="2787370">number</span>
  <span m="2787610">of</span> <span m="2787670">people</span> <span m="2787940">who</span>
  <span m="2788090">have</span> <span m="2788360">type 2</span> <span m="2788570">diabetes,</span>
  <span m="2788720">and even</span> <span m="2789020">the</span> <span m="2789110">definition</span>
  <span m="2789650">of</span> <span m="2789740">it</span> <span m="2789830">has</span>
  <span m="2790010">changed.</span></p><p><span m="2791480">Because</span> <span m="2791840">of</span>
  <span m="2791900">the</span> <span m="2791960">fact</span> <span m="2792290">that</span>
  <span m="2792530">the</span> <span m="2792650">laboratory--</span> <span m="2793190">ignore</span>
  <span m="2793550">this</span> <span m="2793700">part</span> <span m="2793880">over</span>
  <span m="2794000">here.</span> <span m="2794180">That's</span> <span m="2794330">just</span>
  <span m="2794450">a</span> <span m="2794480">fluke.</span> <span m="2794750">But</span>
  <span m="2795000">the</span> <span m="2795090">fact,</span> <span m="2795710">because</span>
  <span m="2796100">of</span> <span m="2796310">the</span> <span m="2796460">laboratory</span>
  <span m="2796940">tests</span> <span m="2797270">that</span> <span m="2797420">were</span>
  <span m="2797720">available</span> <span m="2798260">during</span> <span m="2798530">training</span>
  <span m="2798860">might</span> <span m="2798980">be</span> <span m="2799070">different</span>
  <span m="2799460">from</span> <span m="2799580">the</span> <span m="2799670">ones</span>
  <span m="2799910">that</span> <span m="2800000">are</span> <span m="2800030">available</span>
  <span m="2800390">now,</span> <span m="2801940">and</span> <span m="2802070">because</span>
  <span m="2802430">of</span> <span m="2802490">the</span> <span m="2802580">fact</span>
  <span m="2802940">that</span> <span m="2803180">we</span> <span m="2803750">have</span>
  <span m="2804080">only</span> <span m="2804410">ICD-10</span> <span m="2805190">data</span>
  <span m="2805520">now,</span> <span m="2805850">and not</span> <span m="2806020">ICD-9,</span>
  <span m="2807200">for</span> <span m="2807350">all</span> <span m="2807540">of</span>
  <span m="2807620">those</span> <span m="2807830">reasons,</span> <span m="2808520">our</span>
  <span m="2808640">predictive</span> <span m="2809030">performance</span> <span m="2809360">is</span>
  <span m="2809450">going</span> <span m="2809630">to</span> <span m="2809720">be</span>
  <span m="2809810">really</span> <span m="2810440">horrible</span> <span m="2810970">now,</span>
  <span m="2812510">Particularly</span> <span m="2812870">because</span> <span m="2813080">of
  this</span> <span m="2813230">last</span> <span m="2813500">issue</span> <span m="2813740">of</span>
  <span m="2813830">not</span> <span m="2813980">having</span> <span m="2814220">ICD-9s.</span>
  <span m="2815930">Our</span> <span m="2816020">predictive</span> <span m="2816350">model</span>
  <span m="2816530">is</span> <span m="2816590">going</span> <span m="2816740">to</span>
  <span m="2816830">work</span> <span m="2817040">horribly</span> <span m="2817580">now</span>
  <span m="2818480">if</span> <span m="2818630">it</span> <span m="2818690">was</span>
  <span m="2818810">trained</span> <span m="2819110">on</span> <span m="2819200">data</span>
  <span m="2819410">from</span> <span m="2819590">2008</span> <span m="2821080">or</span>
  <span m="2821210">2009.</span> <span m="2822170">And</span> <span m="2822320">so</span>
  <span m="2822680">we</span> <span m="2822980">would</span> <span m="2823130">have</span>
  <span m="2823250">never</span> <span m="2823670">ever</span> <span m="2823940">even</span>
  <span m="2824150">recognized</span> <span m="2825020">that</span> <span m="2825230">if</span>
  <span m="2825350">we</span> <span m="2825470">used</span> <span m="2825760">the</span>
  <span m="2825870">validation</span> <span m="2826310">set</span> <span m="2826560">up</span>
  <span m="2826640">that</span> <span m="2826790">we</span> <span m="2826910">had</span>
  <span m="2827120">done</span> <span m="2827330">there.</span></p><p><span m="2827840">So</span>
  <span m="2829130">I</span> <span m="2829280">wrote</span> <span m="2829460">that</span>
  <span m="2829580">paper</span> <span m="2830150">when</span> <span m="2830330">I</span>
  <span m="2830420">was</span> <span m="2830900">young</span> <span m="2831140">and</span>
  <span m="2831230">naive.</span></p><p><span m="2832107">[AUDIENCE CHUCKLING]</span></p><p><span
  m="2833480">I'm</span> <span m="2833630">a</span> <span m="2833660">little</span>
  <span m="2834080">bit</span> <span m="2834260">more</span> <span m="2834620">gray-haired</span>
  <span m="2835190">now.</span> <span m="2836540">And</span> <span m="2836690">so</span>
  <span m="2836960">in</span> <span m="2837080">our</span> <span m="2837170">more</span>
  <span m="2837290">recent</span> <span m="2837740">work--</span> <span m="2838070">for</span>
  <span m="2838160">example,</span> <span m="2838640">this</span> <span m="2838820">is</span>
  <span m="2838940">a</span> <span m="2838970">paper</span> <span m="2839330">which</span>
  <span m="2841280">we're</span> <span m="2841670">working</span> <span m="2841970">on</span>
  <span m="2842090">right</span> <span m="2842240">now,</span> <span m="2842510">done</span>
  <span m="2842690">by a</span> <span m="2842840">master's</span> <span m="2843230">student
  of</span> <span m="2843410">mine,</span> <span m="2843620">Helen</span> <span m="2843920">Zhou,</span>
  <span m="2844670">and</span> <span m="2844790">is</span> <span m="2844880">looking</span>
  <span m="2845120">at</span> <span m="2845180">predicting</span> <span m="2845540">antibiotic</span>
  <span m="2845960">resistance,</span> <span m="2847160">now</span> <span m="2847370">we're</span>
  <span m="2847550">a</span> <span m="2847580">little</span> <span m="2847820">bit</span>
  <span m="2848150">smarter</span> <span m="2848630">about</span> <span m="2848840">over</span>
  <span m="2849140">evaluation</span> <span m="2849620">setup.</span> <span m="2849950">And</span>
  <span m="2850040">we</span> <span m="2850220">decided</span> <span m="2850610">to</span>
  <span m="2850790">set</span> <span m="2851090">it</span> <span m="2851180">up</span>
  <span m="2851300">a</span> <span m="2851360">little</span> <span m="2851480">bit</span>
  <span m="2851570">differently.</span></p><p><span m="2852750">So</span> <span m="2852770">what</span>
  <span m="2852890">I'm</span> <span m="2852950">showing</span> <span m="2853220">you</span>
  <span m="2853310">now</span> <span m="2853520">is</span> <span m="2853700">the</span>
  <span m="2853790">way</span> <span m="2853940">that</span> <span m="2854060">we</span>
  <span m="2854150">chose,</span> <span m="2854750">trained,</span> <span m="2855260">validated</span>
  <span m="2855650">and</span> <span m="2855770">test</span> <span m="2856250">for</span>
  <span m="2856550">our</span> <span m="2856640">population.</span> <span m="2858960">So</span>
  <span m="2859370">we</span> <span m="2859850">segmented</span> <span m="2860570">our</span>
  <span m="2860690">data.</span> <span m="2861240">So</span> <span m="2861440">the</span>
  <span m="2861530">x-axis</span> <span m="2862100">here</span> <span m="2862400">is</span>
  <span m="2864320">time,</span> <span m="2865250">and</span> <span m="2865370">the</span>
  <span m="2865460">y-axis</span> <span m="2866120">here</span> <span m="2866390">are</span>
  <span m="2866570">people.</span> <span m="2867230">So</span> <span m="2867440">you</span>
  <span m="2867530">can</span> <span m="2867620">think</span> <span m="2867740">of</span>
  <span m="2867830">each</span> <span m="2868010">person</span> <span m="2868310">as</span>
  <span m="2868400">being</span> <span m="2868520">a</span> <span m="2868580">different</span>
  <span m="2868820">row.</span> <span m="2869900">And</span> <span m="2870020">you</span>
  <span m="2870110">can</span> <span m="2870200">imagine</span> <span m="2870350">that</span>
  <span m="2870470">we</span> <span m="2870560">randomly</span> <span m="2870980">sorted</span>
  <span m="2871340">the</span> <span m="2871440">rows.</span></p><p><span m="2874490">What</span>
  <span m="2874700">we</span> <span m="2874820">did</span> <span m="2875300">is</span>
  <span m="2875720">we</span> <span m="2875870">segmented</span> <span m="2876530">our</span>
  <span m="2876620">data</span> <span m="2876890">into</span> <span m="2877070">these</span>
  <span m="2877220">four</span> <span m="2877550">quadrants.</span> <span m="2879150">The</span>
  <span m="2879250">first</span> <span m="2879440">two</span> <span m="2879650">quadrants,</span>
  <span m="2880880">we</span> <span m="2881090">used</span> <span m="2881510">for</span>
  <span m="2882170">train</span> <span m="2882620">and</span> <span m="2882740">validate.</span>
  <span m="2883980">Notice,</span> <span m="2884450">by</span> <span m="2884630">the</span>
  <span m="2884720">way,</span> <span m="2884990">that</span> <span m="2885230">we</span>
  <span m="2885650">have</span> <span m="2887870">different</span> <span m="2888800">people</span>
  <span m="2889910">in</span> <span m="2890030">the</span> <span m="2890120">training</span>
  <span m="2890510">set</span> <span m="2890840">as</span> <span m="2891050">we</span>
  <span m="2891170">do</span> <span m="2891500">in</span> <span m="2891650">the</span>
  <span m="2891740">validate</span> <span m="2892250">set.</span> <span m="2892770">That's</span>
  <span m="2893030">important</span> <span m="2893450">for</span> <span m="2893600">another</span>
  <span m="2893840">quantity</span> <span m="2894140">which</span> <span m="2894290">I'll</span>
  <span m="2894350">talk</span> <span m="2894500">about</span> <span m="2894650">in</span>
  <span m="2894750">a</span> <span m="2894850">minute.</span> <span m="2896010">So</span>
  <span m="2896030">we</span> <span m="2896120">used</span> <span m="2896420">this</span>
  <span m="2896720">data</span> <span m="2896990">for</span> <span m="2897110">train</span>
  <span m="2897270">and</span> <span m="2897410">validate.</span> <span m="2898040">And</span>
  <span m="2898190">that's,</span> <span m="2898550">again,</span> <span m="2898820">very</span>
  <span m="2899060">similar</span> <span m="2899360">to</span> <span m="2899450">the</span>
  <span m="2899540">way</span> <span m="2899870">we</span> <span m="2900020">did</span>
  <span m="2900170">it</span> <span m="2900230">in</span> <span m="2900320">the</span>
  <span m="2900410">diabetes</span> <span m="2900950">paper.</span></p><p><span m="2902030">But</span>
  <span m="2902180">now,</span> <span m="2902840">for</span> <span m="2903020">testing,</span>
  <span m="2904040">we</span> <span m="2904190">use</span> <span m="2904430">this</span>
  <span m="2904620">future</span> <span m="2905090">data.</span> <span m="2906356">So</span>
  <span m="2906810">we</span> <span m="2906910">used</span> <span m="2907100">data</span>
  <span m="2907370">from</span> <span m="2907610">2014</span> <span m="2907925">to</span>
  <span m="2908240">2016.</span> <span m="2909590">And</span> <span m="2909680">one</span>
  <span m="2909830">can</span> <span m="2909920">imagine</span> <span m="2910220">two</span>
  <span m="2910370">different</span> <span m="2910610">quadrants.</span> <span m="2911120">You</span>
  <span m="2911240">might</span> <span m="2911390">be</span> <span m="2911480">interested</span>
  <span m="2911810">in</span> <span m="2911870">knowing,</span> <span m="2912710">for</span>
  <span m="2912890">the</span> <span m="2912980">same</span> <span m="2913430">patients</span>
  <span m="2914090">for</span> <span m="2914270">whom</span> <span m="2914450">you</span>
  <span m="2914510">made</span> <span m="2914690">predictions</span> <span m="2915260">on</span>
  <span m="2916940">during</span> <span m="2917210">training,</span> <span m="2919010">how</span>
  <span m="2919250">would</span> <span m="2919400">your</span> <span m="2919490">predictions</span>
  <span m="2919910">do</span> <span m="2920030">for</span> <span m="2920120">those</span>
  <span m="2920270">same</span> <span m="2920600">people</span> <span m="2921200">at</span>
  <span m="2921320">test</span> <span m="2921650">time</span> <span m="2924080">in</span>
  <span m="2924230">the</span> <span m="2924290">future</span> <span m="2924650">data.</span>
  <span m="2925010">And</span> <span m="2925130">that's</span> <span m="2925550">assuming</span>
  <span m="2925880">that</span> <span m="2925970">what</span> <span m="2926100">we're</span>
  <span m="2926270">predicting</span> <span m="2926660">is</span> <span m="2926720">something</span>
  <span m="2926960">that's</span> <span m="2927080">much</span> <span m="2927260">more</span>
  <span m="2927350">myopic</span> <span m="2928010">in</span> <span m="2928100">nature.</span>
  <span m="2928670">In</span> <span m="2928790">this</span> <span m="2928940">case</span>
  <span m="2929150">it</span> <span m="2929210">was</span> <span m="2929330">predicting,</span>
  <span m="2930620">are</span> <span m="2930740">they</span> <span m="2930830">going</span>
  <span m="2930980">to</span> <span m="2931070">be</span> <span m="2931160">resistant</span>
  <span m="2931730">to</span> <span m="2931850">some</span> <span m="2932030">antibiotic?</span></p><p><span
  m="2933800">But</span> <span m="2933950">you</span> <span m="2934010">can</span>
  <span m="2934100">also</span> <span m="2934310">look</span> <span m="2934460">at
  it</span> <span m="2934550">for</span> <span m="2934620">a</span> <span m="2934670">completely</span>
  <span m="2935000">different</span> <span m="2935240">set</span> <span m="2935390">of</span>
  <span m="2935450">patients,</span> <span m="2936320">for</span> <span m="2936410">patients</span>
  <span m="2936800">who</span> <span m="2936860">are</span> <span m="2936920">not</span>
  <span m="2937190">used</span> <span m="2937460">during</span> <span m="2937670">training</span>
  <span m="2938060">at</span> <span m="2938180">all.</span> <span m="2938660">And</span>
  <span m="2938780">suppose</span> <span m="2939140">that</span> <span m="2939260">this</span>
  <span m="2940610">2</span> <span m="2940880">bucket</span> <span m="2941150">isn't</span>
  <span m="2941360">used</span> <span m="2941600">at</span> <span m="2941690">all,</span>
  <span m="2942680">for</span> <span m="2942860">those</span> <span m="2943070">patients,</span>
  <span m="2943560">how</span> <span m="2943580">do</span> <span m="2943670">we</span>
  <span m="2943760">do,</span> <span m="2944060">again,</span> <span m="2944630">using</span>
  <span m="2944900">the</span> <span m="2944990">future</span> <span m="2945380">data</span>
  <span m="2945590">for</span> <span m="2945680">that.</span></p><p><span m="2946110">And</span>
  <span m="2946220">the</span> <span m="2946310">advantage</span> <span m="2946640">of</span>
  <span m="2946700">this</span> <span m="2946820">setup</span> <span m="2947330">is</span>
  <span m="2947480">that</span> <span m="2947600">it</span> <span m="2947660">can</span>
  <span m="2947810">really</span> <span m="2948080">help</span> <span m="2948320">you</span>
  <span m="2948410">assess</span> <span m="2949130">non-stationarity.</span> <span
  m="2950900">So</span> <span m="2951890">if</span> <span m="2952100">your</span>
  <span m="2952220">model</span> <span m="2952820">really</span> <span m="2953090">took</span>
  <span m="2953300">advantage</span> <span m="2954050">of</span> <span m="2954830">features</span>
  <span m="2955340">that</span> <span m="2955460">were</span> <span m="2955550">available</span>
  <span m="2955970">in</span> <span m="2956060">2007,</span> <span m="2956840">2008,</span>
  <span m="2957260">2009,</span> <span m="2957860">but</span> <span m="2957950">weren't</span>
  <span m="2958340">available</span> <span m="2958670">in</span> <span m="2958730">2014,</span>
  <span m="2959420">you</span> <span m="2959480">would</span> <span m="2959600">see</span>
  <span m="2959780">a</span> <span m="2959870">big</span> <span m="2960110">drop</span>
  <span m="2960410">in</span> <span m="2960500">your</span> <span m="2960590">performance.</span>
  <span m="2961130">Looking</span> <span m="2961420">at</span> <span m="2961490">the
  drop in</span> <span m="2961770">performance</span> <span m="2962180">from</span>
  <span m="2962330">your</span> <span m="2962450">validate</span> <span m="2962980">set</span>
  <span m="2963520">in</span> <span m="2963650">this</span> <span m="2963800">time</span>
  <span m="2964010">period,</span> <span m="2964550">to</span> <span m="2964730">your</span>
  <span m="2965120">test</span> <span m="2965460">set</span> <span m="2965720">from</span>
  <span m="2965900">that</span> <span m="2966020">time</span> <span m="2966230">period,</span>
  <span m="2966740">that</span> <span m="2966920">drop in</span> <span m="2967220">performance</span>
  <span m="2967760">will</span> <span m="2967940">be</span> <span m="2968390">uniquely</span>
  <span m="2969020">attributed</span> <span m="2969650">to</span> <span m="2970520">the</span>
  <span m="2970610">non-stationarity.</span> <span m="2971760">So</span> <span m="2971780">it's</span>
  <span m="2971870">a</span> <span m="2971900">good</span> <span m="2972050">way</span>
  <span m="2972140">to</span> <span m="2972230">diagnose</span> <span m="2972740">it.</span>
  <span m="2973335">Yep.</span></p><p><span m="2973690">AUDIENCE:</span> <span m="2973765">Just</span>
  <span m="2973840">some</span> <span m="2973915">clarification</span> <span m="2973990">on</span>
  <span m="2974395">non-stationarity--</span> <span m="2975680">is</span> <span m="2975980">it
  the</span> <span m="2976070">fact</span> <span m="2976370">that</span> <span m="2976820">certain</span>
  <span m="2977150">data</span> <span m="2977570">is</span> <span m="2977760">just</span>
  <span m="2978210">lost altogether,</span> <span m="2978570">or is it</span> <span
  m="2979060">the</span> <span m="2979180">fact</span> <span m="2979430">that</span>
  <span m="2979550">it's</span> <span m="2979926">just</span> <span m="2980680">encoded</span>
  <span m="2981160">differently,</span> <span m="2981240">and</span> <span m="2981703">so</span>
  <span m="2982166">then</span> <span m="2982629">it's difficult to get</span> <span
  m="2983092">that mapping</span> <span m="2983555">correct?</span></p><p><span m="2984020">PROFESSOR:</span>
  <span m="2984192">Both.</span> <span m="2984365">Both</span> <span m="2984710">of</span>
  <span m="2984770">these</span> <span m="2984890">happen.</span> <span m="2985790">So</span>
  <span m="2986270">I</span> <span m="2986870">have</span> <span m="2987020">a</span>
  <span m="2987080">big</span> <span m="2987230">research</span> <span m="2987530">program</span>
  <span m="2987800">now</span> <span m="2987980">which</span> <span m="2988130">is</span>
  <span m="2988280">asking</span> <span m="2989300">not</span> <span m="2989480">just</span>
  <span m="2989690">how--</span> <span m="2990210">so</span> <span m="2990550">this</span>
  <span m="2990730">is</span> <span m="2990790">how</span> <span m="2990910">you</span>
  <span m="2990970">can</span> <span m="2991090">evaluate</span> <span m="2991460">and</span>
  <span m="2991550">recognize</span> <span m="2991990">there's a</span> <span m="2992080">problem.</span>
  <span m="2992510">But</span> <span m="2992620">of</span> <span m="2992710">course</span>
  <span m="2992890">there's</span> <span m="2993010">a</span> <span m="2993040">really</span>
  <span m="2993190">interesting</span> <span m="2993520">research</span> <span m="2993910">question,</span>
  <span m="2994300">which</span> <span m="2994510">is,</span> <span m="2995590">how</span>
  <span m="2995800">can</span> <span m="2995920">you</span> <span m="2996010">make</span>
  <span m="2996160">use</span> <span m="2996490">of</span> <span m="2996600">the</span>
  <span m="2996690">non-stationarity.</span> <span m="2997450">Right,</span> <span
  m="2997630">so</span> <span m="2997840">for</span> <span m="2997960">example,</span>
  <span m="2998920">you</span> <span m="2999040">had</span> <span m="2999190">ICD-9/ICD-10</span>
  <span m="3000450">data.</span> <span m="3001870">You</span> <span m="3001970">don't</span>
  <span m="3001980">want</span> <span m="3002100">to</span> <span m="3002160">just</span>
  <span m="3002340">throw</span> <span m="3002640">away</span> <span m="3002880">the</span>
  <span m="3002970">ICD-9</span> <span m="3003570">data.</span> <span m="3005020">Is</span>
  <span m="3005100">there</span> <span m="3005180">a</span> <span m="3005220">way</span>
  <span m="3005340">to</span> <span m="3005430">use</span> <span m="3005640">it?</span></p><p><span
  m="3006640">So</span> <span m="3007140">the</span> <span m="3007290">naive</span>
  <span m="3007710">answer,</span> <span m="3008200">which</span> <span m="3008280">is</span>
  <span m="3008370">what</span> <span m="3008520">the</span> <span m="3008640">community</span>
  <span m="3009060">is</span> <span m="3009150">largely</span> <span m="3009510">using</span>
  <span m="3009750">today,</span> <span m="3010650">is</span> <span m="3011190">come</span>
  <span m="3011370">up</span> <span m="3011460">with</span> <span m="3011550">a</span>
  <span m="3011610">mapping.</span> <span m="3012990">Come</span> <span m="3013170">up</span>
  <span m="3013230">with</span> <span m="3013320">a</span> <span m="3013380">manual</span>
  <span m="3013710">mapping</span> <span m="3014040">from</span> <span m="3014190">ICD-9</span>
  <span m="3014760">to</span> <span m="3014850">ICD-10</span> <span m="3015700">so</span>
  <span m="3015750">that</span> <span m="3015870">you</span> <span m="3016020">can</span>
  <span m="3016410">sort</span> <span m="3016540">of</span> <span m="3016890">manually</span>
  <span m="3017430">transform</span> <span m="3017940">your</span> <span m="3018060">data</span>
  <span m="3018870">into</span> <span m="3019140">this</span> <span m="3019320">new</span>
  <span m="3019500">format</span> <span m="3019980">such</span> <span m="3020190">that</span>
  <span m="3020280">the</span> <span m="3020340">models</span> <span m="3020700">you</span>
  <span m="3020820">learn</span> <span m="3021120">from</span> <span m="3021390">this</span>
  <span m="3021540">older</span> <span m="3021810">time</span> <span m="3022320">is</span>
  <span m="3022590">useful</span> <span m="3022950">in</span> <span m="3023040">the</span>
  <span m="3023100">future</span> <span m="3023370">time.</span> <span m="3024300">That's</span>
  <span m="3024630">the</span> <span m="3025350">boring</span> <span m="3026010">and</span>
  <span m="3026610">simple</span> <span m="3026940">answer.</span></p><p><span m="3027650">But</span>
  <span m="3027930">I</span> <span m="3027990">think</span> <span m="3028170">we</span>
  <span m="3028260">could</span> <span m="3028380">do</span> <span m="3028470">much</span>
  <span m="3028620">better.</span> <span m="3029020">For</span> <span m="3029120">example,</span>
  <span m="3029440">we</span> <span m="3029540">can</span> <span m="3029550">learn</span>
  <span m="3029880">new</span> <span m="3030120">representations</span> <span m="3030930">of
  the</span> <span m="3031020">data.</span> <span m="3031260">We</span> <span m="3031350">can</span>
  <span m="3031500">learn</span> <span m="3031800">that</span> <span m="3031950">mapping</span>
  <span m="3032370">directly</span> <span m="3033780">in</span> <span m="3033960">order</span>
  <span m="3034200">to</span> <span m="3034830">optimize</span> <span m="3035520">for</span>
  <span m="3036030">your</span> <span m="3036710">sort</span> <span m="3036860">of</span>
  <span m="3036930">most</span> <span m="3037290">recent</span> <span m="3037680">performance.</span>
  <span m="3038640">And</span> <span m="3038790">there's</span> <span m="3039090">a</span>
  <span m="3039150">whole</span> <span m="3039300">bunch</span> <span m="3039510">more</span>
  <span m="3039690">that</span> <span m="3039780">we can</span> <span m="3039900">talk</span>
  <span m="3040050">about</span> <span m="3040170">later.</span> <span m="3040440">Yep.</span></p><p><span
  m="3041422">AUDIENCE:</span> <span m="3041667">[INAUDIBLE]</span> <span m="3042404">non-stationary</span>
  <span m="3043390">change,</span> <span m="3044040">this</span> <span m="3044660">will</span>
  <span m="3044920">[INAUDIBLE]</span> <span m="3046970">does</span> <span m="3047440">not</span>
  <span m="3047790">ensure</span> <span m="3048190">robustness</span> <span m="3049970">to</span>
  <span m="3050395">the future.</span></p><p><span m="3050820">PROFESSOR:</span> <span
  m="3051045">Correct.</span> <span m="3051970">So</span> <span m="3052320">this</span>
  <span m="3052500">allows</span> <span m="3052770">you</span> <span m="3052830">to</span>
  <span m="3052950">detect</span> <span m="3053340">that</span> <span m="3053510">a</span>
  <span m="3053600">non-stationarity</span> <span m="3054210">has</span> <span m="3054360">happened.</span>
  <span m="3055800">And</span> <span m="3055970">it</span> <span m="3056020">allows</span>
  <span m="3056340">you</span> <span m="3056430">to</span> <span m="3056550">say</span>
  <span m="3057390">that</span> <span m="3057930">your</span> <span m="3058050">model</span>
  <span m="3058500">is</span> <span m="3058710">going</span> <span m="3058950">to</span>
  <span m="3059070">generalize</span> <span m="3059670">to</span> <span m="3059820">2014-2016.</span>
  <span m="3061260">But</span> <span m="3061350">of</span> <span m="3061410">course,</span>
  <span m="3061690">that</span> <span m="3061790">doesn't</span> <span m="3061920">mean</span>
  <span m="3062070">that</span> <span m="3062160">your</span> <span m="3062220">model's</span>
  <span m="3062460">going to</span> <span m="3062610">generalize</span> <span m="3062970">to</span>
  <span m="3063060">2016-2018.</span></p><p><span m="3066600">And</span> <span m="3066720">so</span>
  <span m="3066870">how</span> <span m="3066990">do</span> <span m="3067080">you</span>
  <span m="3067140">do</span> <span m="3067260">that?</span> <span m="3067480">How</span>
  <span m="3067580">do</span> <span m="3067680">you</span> <span m="3067780">have</span>
  <span m="3067880">confidence</span> <span m="3068070">in</span> <span m="3068160">that?</span>
  <span m="3068310">Well,</span> <span m="3068550">that's</span> <span m="3068830">a</span>
  <span m="3068920">really</span> <span m="3069180">interesting</span> <span m="3069480">research</span>
  <span m="3069780">question.</span> <span m="3070200">We</span> <span m="3070380">don't</span>
  <span m="3070560">have</span> <span m="3070830">good</span> <span m="3071010">answers</span>
  <span m="3071310">to</span> <span m="3071400">that</span> <span m="3071520">today.</span></p><p><span
  m="3072610">From</span> <span m="3074910">a</span> <span m="3074970">practical</span>
  <span m="3075450">perspective,</span> <span m="3076210">the</span> <span m="3076230">best</span>
  <span m="3076530">I</span> <span m="3076590">can</span> <span m="3078000">offer</span>
  <span m="3078330">you</span> <span m="3078450">today</span> <span m="3079020">is,</span>
  <span m="3080410">build</span> <span m="3080810">in</span> <span m="3080940">these</span>
  <span m="3081090">checks</span> <span m="3081330">and</span> <span m="3081420">balances</span>
  <span m="3081870">all</span> <span m="3082050">the</span> <span m="3082140">time.</span>
  <span m="3082590">So</span> <span m="3082830">continuously</span> <span m="3083730">sort</span>
  <span m="3083940">of</span> <span m="3084570">evaluate</span> <span m="3085110">how</span>
  <span m="3085260">you're</span> <span m="3085380">doing</span> <span m="3085650">on</span>
  <span m="3085740">the</span> <span m="3085800">most</span> <span m="3086070">recent</span>
  <span m="3086370">data.</span> <span m="3086780">And</span> <span m="3086880">if</span>
  <span m="3086970">you</span> <span m="3087060">see</span> <span m="3087270">big</span>
  <span m="3087420">changes,</span> <span m="3088350">throw</span> <span m="3088590">a</span>
  <span m="3088620">red</span> <span m="3088770">flag.</span> <span m="3090150">Build</span>
  <span m="3090420">more</span> <span m="3090570">checks</span> <span m="3090840">and</span>
  <span m="3090930">balances</span> <span m="3091380">into</span> <span m="3091540">your</span>
  <span m="3091590">deployment</span> <span m="3092070">process.</span> <span m="3093510">If</span>
  <span m="3093630">you</span> <span m="3093750">see</span> <span m="3093900">a</span>
  <span m="3093960">bunch</span> <span m="3094170">of</span> <span m="3094230">patients</span>
  <span m="3094800">who</span> <span m="3095030">are</span> <span m="3095430">getting</span>
  <span m="3095790">predicted</span> <span m="3096180">probabilities</span> <span
  m="3096960">of</span> <span m="3097260">1,</span> <span m="3097710">and</span> <span
  m="3098160">in</span> <span m="3098250">the</span> <span m="3098310">past,</span>
  <span m="3098640">you'd</span> <span m="3098730">never</span> <span m="3099000">predicted</span>
  <span m="3099240">probability</span> <span m="3099570">1,</span> <span m="3100110">that</span>
  <span m="3100260">might</span> <span m="3100410">tell</span> <span m="3100590">you</span>
  <span m="3100680">something.</span></p><p><span m="3102170">Then</span> <span m="3102630">much</span>
  <span m="3102840">later</span> <span m="3103050">in</span> <span m="3103110">the</span>
  <span m="3103170">semester,</span> <span m="3103600">we'll</span> <span m="3103620">talk</span>
  <span m="3103830">about</span> <span m="3104040">robust</span> <span m="3104400">machine</span>
  <span m="3104670">learning</span> <span m="3104860">approaches,</span> <span m="3105180">for</span>
  <span m="3105270">example,</span> <span m="3105690">approaches</span> <span m="3106090">that</span>
  <span m="3106180">have</span> <span m="3106270">been</span> <span m="3106350">designed</span>
  <span m="3106860">to</span> <span m="3107070">be</span> <span m="3107280">robust</span>
  <span m="3107760">against</span> <span m="3108090">adversaries.</span> <span m="3109290">And</span>
  <span m="3109380">those</span> <span m="3109590">type</span> <span m="3109800">of</span>
  <span m="3109860">approaches</span> <span m="3110220">as</span> <span m="3110340">well</span>
  <span m="3110930">will</span> <span m="3111210">allow</span> <span m="3111450">you</span>
  <span m="3111510">to</span> <span m="3111600">be</span> <span m="3111690">much</span>
  <span m="3111930">more</span> <span m="3112050">robust</span> <span m="3112480">to</span>
  <span m="3112560">particular</span> <span m="3112980">types</span> <span m="3113370">of</span>
  <span m="3113460">data</span> <span m="3113620">set</span> <span m="3113850">shift,</span>
  <span m="3114450">of</span> <span m="3114570">which</span> <span m="3114750">non-stationarity</span>
  <span m="3115410">is</span> <span m="3115500">one</span> <span m="3115680">example.</span>
  <span m="3116400">But</span> <span m="3116580">it's</span> <span m="3117180">a</span>
  <span m="3117240">big,</span> <span m="3117570">open</span> <span m="3117870">research</span>
  <span m="3118200">field.</span> <span m="3118470">Yep.</span></p><p><span m="3118900">AUDIENCE:</span>
  <span m="3119115">So</span> <span m="3119330">just to make</span> <span m="3119760">sure
  I have</span> <span m="3120050">the understanding</span> <span m="3120340">correct,</span>
  <span m="3121610">theoretically,</span> <span m="3122090">if</span> <span m="3122220">you</span>
  <span m="3122280">could</span> <span m="3122400">map</span> <span m="3122790">everything</span>
  <span m="3123270">from</span> <span m="3123740">the old</span> <span m="3123970">data
  set</span> <span m="3124240">to the</span> <span m="3124670">new data</span> <span
  m="3125100">set, like the</span> <span m="3125530">encodings,</span> <span m="3127500">would</span>
  <span m="3127650">it</span> <span m="3127710">still</span> <span m="3127980">be</span>
  <span m="3128100">OK,</span> <span m="3128460">like</span> <span m="3128958">the
  results</span> <span m="3129456">you get</span> <span m="3129954">on the</span>
  <span m="3130452">future data</span> <span m="3130950">set?</span></p><p><span m="3132450">PROFESSOR:</span>
  <span m="3132585">If</span> <span m="3132720">you</span> <span m="3132870">could</span>
  <span m="3132990">do</span> <span m="3133140">a</span> <span m="3133200">perfect</span>
  <span m="3133650">mapping,</span> <span m="3134040">and</span> <span m="3134130">it's</span>
  <span m="3134280">one</span> <span m="3134550">to</span> <span m="3134670">one,</span>
  <span m="3134970">and</span> <span m="3135040">the</span> <span m="3135120">distributions</span>
  <span m="3135900">of</span> <span m="3135990">those</span> <span m="3136200">things</span>
  <span m="3136440">also</span> <span m="3136680">didn't</span> <span m="3136890">change,</span>
  <span m="3137430">then</span> <span m="3137880">yeah.</span> <span m="3138750">Really</span>
  <span m="3139080">what</span> <span m="3139230">you</span> <span m="3139320">need</span>
  <span m="3139440">to</span> <span m="3139500">assess</span> <span m="3139890">is,</span>
  <span m="3140100">is</span> <span m="3140370">there</span> <span m="3140770">data</span>
  <span m="3141080">set</span> <span m="3141240">shift?</span> <span m="3141660">Is</span>
  <span m="3141900">your</span> <span m="3142050">training</span> <span m="3142560">distribution,</span>
  <span m="3143290">after</span> <span m="3143520">mapping,</span> <span m="3143970">the</span>
  <span m="3144090">same</span> <span m="3144510">as</span> <span m="3144630">your</span>
  <span m="3144720">testing</span> <span m="3145170">distribution?</span> <span m="3146170">If</span>
  <span m="3146470">the answer is</span> <span m="3146760">yes,</span> <span m="3147090">you're</span>
  <span m="3147240">all</span> <span m="3147390">good.</span> <span m="3147730">If</span>
  <span m="3147830">you're</span> <span m="3147840">not,</span> <span m="3148110">you're</span>
  <span m="3148260">in</span> <span m="3148350">trouble.</span> <span m="3149160">Yep.</span></p><p><span
  m="3149610">AUDIENCE:</span> <span m="3149670">What</span> <span m="3149730">seems</span>
  <span m="3149790">to</span> <span m="3149850">be</span> <span m="3150350">the</span>
  <span m="3150470">test</span> <span m="3150810">set</span> <span m="3151200">of</span>
  <span m="3151380">traits</span> <span m="3151700">set here? </span> <span m="3151830">Or</span>
  <span m="3152010">what</span> <span m="3152510">[INAUDIBLE]?</span></p><p><span
  m="3155010">PROFESSOR:</span> <span m="3155160">So</span> <span m="3155500">1</span>
  <span m="3156180">is</span> <span m="3156360">using</span> <span m="3156690">data</span>
  <span m="3156930">only</span> <span m="3157170">from</span> <span m="3157290">2007-2013,</span>
  <span m="3158530">3</span> <span m="3158890">is</span> <span m="3159030">using</span>
  <span m="3159210">data</span> <span m="3159390">only</span> <span m="3159600">from</span>
  <span m="3159720">2014-2016.</span></p><p><span m="3160950">AUDIENCE:</span> <span
  m="3161165">But</span> <span m="3162243">in the case,</span> <span m="3162674">like,</span>
  <span m="3163536">the</span> <span m="3163970">output</span> <span m="3164130">we
  care about</span> <span m="3164611">happened</span> <span m="3165092">in, like,</span>
  <span m="3165573">2007-2013,</span> <span m="3166535">then</span> <span m="3167016">that</span>
  <span m="3167497">observation</span> <span m="3167978">would be</span> <span m="3168459">not--</span>
  <span m="3168940">it wouldn't</span> <span m="3169430">be useful. </span></p><p><span
  m="3169580">PROFESSOR:</span> <span m="3169815">Yeah,</span> <span m="3170050">so</span>
  <span m="3170190">for</span> <span m="3170340">the</span> <span m="3170430">diabetes</span>
  <span m="3171000">problem,</span> <span m="3171570">there's</span> <span m="3172190">also</span>
  <span m="3172400">just</span> <span m="3173010">inclusion/exclusion</span> <span
  m="3173880">criteria</span> <span m="3174090">that</span> <span m="3174270">you</span>
  <span m="3174420">have</span> <span m="3174540">to</span> <span m="3174630">deal</span>
  <span m="3174810">with.</span> <span m="3175310">For</span> <span m="3175470">what</span>
  <span m="3175590">I'm</span> <span m="3175680">showing</span> <span m="3175890">you</span>
  <span m="3176010">here,</span> <span m="3176340">I'm</span> <span m="3176430">talking</span>
  <span m="3176820">about</span> <span m="3176970">a</span> <span m="3177030">setting</span>
  <span m="3177450">where</span> <span m="3179580">you</span> <span m="3179730">might</span>
  <span m="3179880">be</span> <span m="3179970">making</span> <span m="3180210">multiple</span>
  <span m="3180510">predictions</span> <span m="3180840">for</span> <span m="3180900">patients</span>
  <span m="3181160">across</span> <span m="3181350">time.</span> <span m="3182230">So</span>
  <span m="3182310">it's</span> <span m="3182410">a</span> <span m="3182430">much</span>
  <span m="3182580">more</span> <span m="3182700">myopic</span> <span m="3183150">prediction</span>
  <span m="3183510">task.</span></p><p><span m="3184650">But</span> <span m="3184830">one</span>
  <span m="3184980">could</span> <span m="3185100">come</span> <span m="3185220">up</span>
  <span m="3185280">with</span> <span m="3185370">an</span> <span m="3185460">analogy</span>
  <span m="3185880">to</span> <span m="3186000">this</span> <span m="3186210">for</span>
  <span m="3186360">the</span> <span m="3186450">diabetes</span> <span m="3186840">setting.</span>
  <span m="3187720">Like,</span> <span m="3187950">for</span> <span m="3188010">example,</span>
  <span m="3188400">just</span> <span m="3189600">hold</span> <span m="3189960">out</span>
  <span m="3191310">half</span> <span m="3191580">of</span> <span m="3191640">the</span>
  <span m="3191730">patients</span> <span m="3193720">at</span> <span m="3194010">random.</span>
  <span m="3195000">And</span> <span m="3195150">then</span> <span m="3197130">for</span>
  <span m="3197370">your</span> <span m="3197490">training</span> <span m="3197850">set,</span>
  <span m="3198120">use</span> <span m="3198510">data</span> <span m="3199050">up</span>
  <span m="3199200">to</span> <span m="3199320">2009,</span> <span m="3201290">and</span>
  <span m="3201450">evaluate</span> <span m="3201810">on</span> <span m="3201930">data</span>
  <span m="3202110">only</span> <span m="3202320">up</span> <span m="3202410">to</span>
  <span m="3202470">2013.</span> <span m="3203760">And</span> <span m="3203910">for</span>
  <span m="3204060">your</span> <span m="3204180">test</span> <span m="3204540">set,</span>
  <span m="3205620">pretend</span> <span m="3206160">as</span> <span m="3206250">if</span>
  <span m="3206430">it</span> <span m="3206520">was</span> <span m="3207570">January</span>
  <span m="3208530">1,</span> <span m="3208890">2013,</span> <span m="3210610">and</span>
  <span m="3211380">look</span> <span m="3211590">at</span> <span m="3211710">performance</span>
  <span m="3212340">up</span> <span m="3212460">to</span> <span m="3212550">2017.</span>
  <span m="3215390">And</span> <span m="3215490">so</span> <span m="3215580">that</span>
  <span m="3215700">would</span> <span m="3215820">be--</span> <span m="3216600">you're</span>
  <span m="3216690">changing</span> <span m="3217140">your</span> <span m="3217230">prediction</span>
  <span m="3217620">time</span> <span m="3218370">to</span> <span m="3218520">use</span>
  <span m="3218670">more</span> <span m="3218820">recent</span> <span m="3219210">data.</span></p><p><span
  m="3223330">So</span> <span m="3223660">the</span> <span m="3223750">next</span>
  <span m="3224260">subtlety</span> <span m="3226750">is--</span> <span m="3227770">it's</span>
  <span m="3227950">a</span> <span m="3228010">name</span> <span m="3228250">that</span>
  <span m="3228370">I</span> <span m="3228430">put</span> <span m="3228580">on</span>
  <span m="3228670">to it.</span> <span m="3229060">This</span> <span m="3229210">isn't</span>
  <span m="3229410">a</span> <span m="3229450">standard</span> <span m="3229900">name.</span>
  <span m="3230220">This</span> <span m="3230330">is</span> <span m="3230410">what</span>
  <span m="3230530">I'm</span> <span m="3230650">calling</span> <span m="3231310">intervention-tainted</span>
  <span m="3232840">outcomes.</span> <span m="3236130">And</span> <span m="3236230">so</span>
  <span m="3236320">the</span> <span m="3236380">example</span> <span m="3236890">here</span>
  <span m="3237280">came</span> <span m="3237610">from</span> <span m="3237820">your</span>
  <span m="3237970">reading</span> <span m="3238330">for</span> <span m="3238480">today.</span>
  <span m="3241210">The</span> <span m="3241300">reading</span> <span m="3241570">was</span>
  <span m="3242380">this</span> <span m="3242560">paper</span> <span m="3242830">on</span>
  <span m="3243130">intelligible</span> <span m="3243670">models</span> <span m="3244000">for</span>
  <span m="3244090">health</span> <span m="3244360">care</span> <span m="3244630">predicting</span>
  <span m="3244990">pneumonia</span> <span m="3245320">risk</span> <span m="3245590">in</span>
  <span m="3245680">hospital</span> <span m="3245980">30-day</span> <span m="3246340">admissions</span>
  <span m="3246760">from</span> <span m="3246910">KDD</span> <span m="3247270">2015.</span></p><p><span
  m="3248350">So</span> <span m="3248530">in</span> <span m="3248650">that</span>
  <span m="3248770">paper,</span> <span m="3249100">they</span> <span m="3249220">give</span>
  <span m="3249370">an</span> <span m="3249460">example--</span> <span m="3250040">it's</span>
  <span m="3250210">a</span> <span m="3250240">very</span> <span m="3250480">old</span>
  <span m="3250750">example--</span> <span m="3252070">of</span> <span m="3252610">trying</span>
  <span m="3252910">to</span> <span m="3253000">use</span> <span m="3253150">a</span>
  <span m="3253180">predictive</span> <span m="3253540">model</span> <span m="3253840">to</span>
  <span m="3254350">understand</span> <span m="3255280">a</span> <span m="3255340">patient's</span>
  <span m="3255730">risk</span> <span m="3256000">of</span> <span m="3256090">mortality</span>
  <span m="3257920">when</span> <span m="3258250">they</span> <span m="3258370">come</span>
  <span m="3258670">into</span> <span m="3258910">the</span> <span m="3259000">hospital.</span>
  <span m="3261100">And</span> <span m="3261790">what</span> <span m="3262000">they</span>
  <span m="3262240">learned--</span> <span m="3262710">and</span> <span m="3263040">they</span>
  <span m="3263110">used</span> <span m="3263320">a</span> <span m="3263350">rule-based</span>
  <span m="3263920">learning</span> <span m="3264250">algorithm--</span> <span m="3264710">and</span>
  <span m="3264810">what</span> <span m="3264820">they</span> <span m="3264910">discovered</span>
  <span m="3265510">was</span> <span m="3266140">a</span> <span m="3266290">rule</span>
  <span m="3266740">that</span> <span m="3266920">said</span> <span m="3267310">if</span>
  <span m="3267490">the</span> <span m="3267610">patient</span> <span m="3267970">has</span>
  <span m="3268450">asthma,</span> <span m="3269740">then</span> <span m="3269980">they</span>
  <span m="3270160">have</span> <span m="3270400">low</span> <span m="3270910">risk</span>
  <span m="3271360">of</span> <span m="3272140">dying.</span> <span m="3273920">So</span>
  <span m="3273970">these</span> <span m="3274150">are</span> <span m="3274180">all</span>
  <span m="3274300">patients</span> <span m="3274600">who</span> <span m="3274660">have</span>
  <span m="3274780">pneumonia.</span> <span m="3275320">So</span> <span m="3275530">a</span>
  <span m="3275590">patient</span> <span m="3275860">who</span> <span m="3275950">comes</span>
  <span m="3276190">in</span> <span m="3276280">with</span> <span m="3276460">pneumonia</span>
  <span m="3276880">and</span> <span m="3277300">asthma</span> <span m="3278140">has</span>
  <span m="3278350">a</span> <span m="3278410">lower</span> <span m="3278830">risk</span>
  <span m="3279130">of</span> <span m="3279250">dying</span> <span m="3279640">than</span>
  <span m="3279760">a</span> <span m="3279790">patient</span> <span m="3280120">who</span>
  <span m="3280270">comes</span> <span m="3280690">in</span> <span m="3282580">with</span>
  <span m="3282820">pneumonia</span> <span m="3283210">and</span> <span m="3283360">does</span>
  <span m="3283540">not</span> <span m="3283810">have</span> <span m="3284020">a</span>
  <span m="3284050">history</span> <span m="3284380">of</span> <span m="3284470">asthma.</span>
  <span m="3285400">OK,</span> <span m="3285760">that's</span> <span m="3286000">what</span>
  <span m="3286120">this</span> <span m="3286270">rule</span> <span m="3286540">says.</span></p><p><span
  m="3287830">And</span> <span m="3288430">this</span> <span m="3288580">paper</span>
  <span m="3290260">argued</span> <span m="3290920">that</span> <span m="3291100">there's</span>
  <span m="3291220">something</span> <span m="3291550">wrong</span> <span m="3292090">with</span>
  <span m="3292360">that</span> <span m="3292540">learned</span> <span m="3292870">model.</span>
  <span m="3294440">Any</span> <span m="3294540">of</span> <span m="3294550">you</span>
  <span m="3294610">remember</span> <span m="3294940">what</span> <span m="3295030">that</span>
  <span m="3295150">was?</span> <span m="3296110">Someone</span> <span m="3296350">who</span>
  <span m="3296470">hasn't</span> <span m="3296710">talked</span> <span m="3296920">today,</span>
  <span m="3297520">please.</span> <span m="3298390">Yeah,</span> <span m="3298540">in</span>
  <span m="3298600">the</span> <span m="3298660">back.</span></p><p><span m="3299250">AUDIENCE:</span>
  <span m="3299337">It</span> <span m="3299424">was</span> <span m="3299511">that</span>
  <span m="3299600">those</span> <span m="3299950">with</span> <span m="3300340">asthma</span>
  <span m="3300710">had more</span> <span m="3301170">aggressive</span> <span m="3301460">treatment.</span>
  <span m="3302204">So</span> <span m="3302658">that means</span> <span m="3303112">that
  they</span> <span m="3303566">had a higher</span> <span m="3304020">chance of</span>
  <span m="3304474">survival.</span></p><p><span m="3304930">PROFESSOR:</span> <span
  m="3305170">Patients</span> <span m="3305410">with</span> <span m="3305650">asthma</span>
  <span m="3306040">had</span> <span m="3306190">more</span> <span m="3306460">aggressive</span>
  <span m="3306880">treatment.</span> <span m="3307540">In</span> <span m="3307630">particular,</span>
  <span m="3308320">they</span> <span m="3308500">might</span> <span m="3308710">have</span>
  <span m="3308800">been</span> <span m="3308950">admitted</span> <span m="3309310">to</span>
  <span m="3309430">the</span> <span m="3309490">intensive</span> <span m="3309910">care</span>
  <span m="3310180">unit</span> <span m="3310600">for</span> <span m="3311080">more</span>
  <span m="3311350">careful</span> <span m="3311950">vigilance.</span> <span m="3313090">And</span>
  <span m="3313210">as</span> <span m="3313330">a</span> <span m="3313360">result,</span>
  <span m="3313630">they</span> <span m="3313720">had</span> <span m="3313870">better</span>
  <span m="3314410">outcomes.</span> <span m="3314830">Yes,</span> <span m="3315040">that's</span>
  <span m="3315190">exactly</span> <span m="3315610">right.</span></p><p><span m="3317080">So</span>
  <span m="3318340">the</span> <span m="3318460">real</span> <span m="3319120">story</span>
  <span m="3319630">behind</span> <span m="3319990">this</span> <span m="3320170">is</span>
  <span m="3320290">that</span> <span m="3320560">risk</span> <span m="3320860">stratification,</span>
  <span m="3321370">as</span> <span m="3321460">we</span> <span m="3321550">talked</span>
  <span m="3321820">about</span> <span m="3322060">the last</span> <span m="3322300">couple</span>
  <span m="3322480">weeks,</span> <span m="3323140">it's</span> <span m="3323320">used</span>
  <span m="3323710">to</span> <span m="3323860">drive</span> <span m="3324160">interventions.</span>
  <span m="3325180">And</span> <span m="3325270">those</span> <span m="3325390">interventions,</span>
  <span m="3326290">if</span> <span m="3326470">they</span> <span m="3326590">happened</span>
  <span m="3327100">in</span> <span m="3327190">the</span> <span m="3327280">past</span>
  <span m="3327670">data,</span> <span m="3328360">would</span> <span m="3328540">change</span>
  <span m="3328930">the</span> <span m="3329050">outcomes.</span></p><p><span m="3330350">So</span>
  <span m="3331630">in</span> <span m="3331750">this</span> <span m="3331960">case,</span>
  <span m="3332870">you</span> <span m="3332890">might</span> <span m="3333070">imagine</span>
  <span m="3333550">using the</span> <span m="3334030">learned</span> <span m="3334360">predictive</span>
  <span m="3334750">model</span> <span m="3335140">to</span> <span m="3335260">say,</span>
  <span m="3335530">a</span> <span m="3335590">new</span> <span m="3335770">patient</span>
  <span m="3336130">comes</span> <span m="3336430">in,</span> <span m="3337270">this</span>
  <span m="3337420">new</span> <span m="3337540">patient</span> <span m="3337910">has</span>
  <span m="3338200">asthma,</span> <span m="3338620">and</span> <span m="3338710">so</span>
  <span m="3338770">we're</span> <span m="3338860">going</span> <span m="3338940">to</span>
  <span m="3339030">say</span> <span m="3339170">they're</span> <span m="3339280">low</span>
  <span m="3339490">risk.</span> <span m="3340010">And</span> <span m="3340110">if</span>
  <span m="3340210">we</span> <span m="3340310">took</span> <span m="3340450">a</span>
  <span m="3340510">naive</span> <span m="3340990">action</span> <span m="3341470">based</span>
  <span m="3341680">on</span> <span m="3341770">that</span> <span m="3341890">prediction,</span>
  <span m="3342340">we</span> <span m="3342460">might</span> <span m="3342670">say,</span>
  <span m="3342950">OK,</span> <span m="3343930">let's</span> <span m="3344140">send</span>
  <span m="3344320">them</span> <span m="3344470">home.</span> <span m="3344800">They're</span>
  <span m="3344950">at</span> <span m="3345010">low</span> <span m="3345230">risk</span>
  <span m="3345460">of</span> <span m="3345550">dying.</span> <span m="3346880">But</span>
  <span m="3346960">if</span> <span m="3347050">we</span> <span m="3347140">did</span>
  <span m="3347320">that,</span> <span m="3347600">we</span> <span m="3347700">could</span>
  <span m="3347740">be</span> <span m="3347890">killing</span> <span m="3348310">people.</span>
  <span m="3348700">Because</span> <span m="3349480">the</span> <span m="3349570">reason</span>
  <span m="3349960">why</span> <span m="3350230">they</span> <span m="3350380">were</span>
  <span m="3350530">low</span> <span m="3350710">risk</span> <span m="3351130">is</span>
  <span m="3351250">because</span> <span m="3351850">they</span> <span m="3352060">had</span>
  <span m="3352480">those</span> <span m="3352660">interventions</span> <span m="3353470">in</span>
  <span m="3353560">the</span> <span m="3353650">past.</span></p><p><span m="3356650">So</span>
  <span m="3357160">here's</span> <span m="3357490">what's</span> <span m="3357640">going</span>
  <span m="3357850">on</span> <span m="3357980">in that</span> <span m="3358090">picture.</span>
  <span m="3359800">You</span> <span m="3359920">have</span> <span m="3360100">your</span>
  <span m="3360220">data,</span> <span m="3361090">X.</span> <span m="3361960">And</span>
  <span m="3362050">you're</span> <span m="3362380">trying</span> <span m="3362680">to</span>
  <span m="3362770">make</span> <span m="3362920">a</span> <span m="3362980">prediction</span>
  <span m="3363310">at</span> <span m="3363370">some</span> <span m="3363550">point</span>
  <span m="3363730">in</span> <span m="3363790">time,</span> <span m="3364120">let's</span>
  <span m="3364240">say,</span> <span m="3364570">emergency</span> <span m="3364880">department</span>
  <span m="3365170">triage.</span> <span m="3366070">You</span> <span m="3366160">want</span>
  <span m="3366280">to</span> <span m="3366340">predict</span> <span m="3366580">some</span>
  <span m="3366790">outcome</span> <span m="3367180">Y,</span> <span m="3367630">let's</span>
  <span m="3367810">say,</span> <span m="3368380">whether</span> <span m="3368590">the</span>
  <span m="3368650">patient</span> <span m="3368920">dies</span> <span m="3369260">at</span>
  <span m="3369350">some</span> <span m="3369940">defined</span> <span m="3370300">point</span>
  <span m="3370480">in</span> <span m="3370570">the</span> <span m="3370630">future.</span></p><p><span
  m="3372710">Now,</span> <span m="3373060">the</span> <span m="3373150">challenge</span>
  <span m="3373630">is</span> <span m="3374140">that,</span> <span m="3374770">as</span>
  <span m="3375040">stated</span> <span m="3375790">in</span> <span m="3376090">the</span>
  <span m="3376390">machine</span> <span m="3376750">learning</span> <span m="3376960">tasks</span>
  <span m="3377320">that</span> <span m="3377440">you</span> <span m="3377530">saw</span>
  <span m="3377770">there,</span> <span m="3378820">all</span> <span m="3379030">you</span>
  <span m="3379180">had</span> <span m="3379330">access</span> <span m="3379750">to</span>
  <span m="3379940">was</span> <span m="3380260">X</span> <span m="3380800">and</span>
  <span m="3381070">Y,</span> <span m="3382320">the</span> <span m="3382420">covariance</span>
  <span m="3382705">of</span> <span m="3382990">the</span> <span m="3383080">features</span>
  <span m="3383770">and</span> <span m="3384040">the</span> <span m="3384220">outcome.</span>
  <span m="3385420">And</span> <span m="3385540">so</span> <span m="3386110">you're</span>
  <span m="3386260">predicting</span> <span m="3387010">Y</span> <span m="3387280">from</span>
  <span m="3387580">X,</span> <span m="3388150">but</span> <span m="3388360">you're</span>
  <span m="3388570">marginalizing</span> <span m="3389740">over</span> <span m="3390250">everything</span>
  <span m="3390670">that</span> <span m="3390790">happens</span> <span m="3391180">in</span>
  <span m="3391270">between,</span> <span m="3391820">in</span> <span m="3391920">this</span>
  <span m="3391960">case,</span> <span m="3392200">the</span> <span m="3392260">treatment.</span>
  <span m="3393490">So</span> <span m="3393790">the</span> <span m="3393910">good</span>
  <span m="3394720">outcomes,</span> <span m="3395510">people</span> <span m="3395890">surviving,</span>
  <span m="3396940">might</span> <span m="3397150">have</span> <span m="3397270">been</span>
  <span m="3397390">due</span> <span m="3397630">to</span> <span m="3397780">what's</span>
  <span m="3397990">going</span> <span m="3398170">on</span> <span m="3398290">in</span>
  <span m="3398380">between.</span> <span m="3398860">But</span> <span m="3399070">what's</span>
  <span m="3399220">going</span> <span m="3399370">on</span> <span m="3399460">in</span>
  <span m="3399520">between</span> <span m="3399790">is</span> <span m="3399880">not</span>
  <span m="3400030">even</span> <span m="3400240">observed</span> <span m="3400750">in</span>
  <span m="3400840">the</span> <span m="3400900">data</span> <span m="3401230">necessarily.</span></p><p><span
  m="3403780">So</span> <span m="3405100">how</span> <span m="3405340">do</span> <span
  m="3405400">we</span> <span m="3405550">address</span> <span m="3405880">this</span>
  <span m="3406030">problem?</span> <span m="3406520">Well,</span> <span m="3406720">the</span>
  <span m="3406820">first</span> <span m="3407050">thing</span> <span m="3407230">I</span>
  <span m="3407320">want</span> <span m="3407500">you</span> <span m="3407560">to</span>
  <span m="3407650">think</span> <span m="3407890">about</span> <span m="3408160">is,</span>
  <span m="3408610">can</span> <span m="3408790">we</span> <span m="3408880">even</span>
  <span m="3409090">recognize</span> <span m="3409780">that</span> <span m="3409870">this</span>
  <span m="3410020">is</span> <span m="3410140">a</span> <span m="3410200">problem?</span>
  <span m="3411030">And</span> <span m="3411130">that's</span> <span m="3411340">where</span>
  <span m="3411520">that</span> <span m="3411730">article</span> <span m="3412930">really</span>
  <span m="3413260">suggests</span> <span m="3413740">that</span> <span m="3413890">using</span>
  <span m="3414190">an</span> <span m="3414250">unintelligible</span> <span m="3415060">model,</span>
  <span m="3415360">a model</span> <span m="3415630">that</span> <span m="3415750">you</span>
  <span m="3415840">can</span> <span m="3415990">introspect</span> <span m="3416650">and</span>
  <span m="3416740">try</span> <span m="3416920">to</span> <span m="3417010">understand</span>
  <span m="3417550">a</span> <span m="3417610">little</span> <span m="3417820">bit,</span>
  <span m="3418510">is</span> <span m="3418660">actually</span> <span m="3418930">really</span>
  <span m="3419200">important</span> <span m="3420040">for</span> <span m="3420310">even</span>
  <span m="3420520">recognizing</span> <span m="3421270">that</span> <span m="3421420">weird</span>
  <span m="3421750">things</span> <span m="3421990">are</span> <span m="3422080">happening.</span>
  <span m="3424400">And</span> <span m="3424570">this</span> <span m="3424720">is</span>
  <span m="3424780">a</span> <span m="3424810">topic</span> <span m="3425230">which</span>
  <span m="3425590">we</span> <span m="3425770">will</span> <span m="3425860">talk</span>
  <span m="3426130">about</span> <span m="3426970">in</span> <span m="3427150">a</span>
  <span m="3427180">lecture</span> <span m="3427600">towards</span> <span m="3427870">the</span>
  <span m="3427930">end</span> <span m="3428020">of</span> <span m="3428080">the</span>
  <span m="3428170">semester</span> <span m="3428650">in</span> <span m="3428770">much</span>
  <span m="3428950">more--</span> <span m="3429070">Jack</span> <span m="3429300">will</span>
  <span m="3429400">talk</span> <span m="3429550">about</span> <span m="3429700">algorithms</span>
  <span m="3430240">for</span> <span m="3430450">interpreting</span> <span m="3431200">machine</span>
  <span m="3431470">learning</span> <span m="3431710">models.</span></p><p><span m="3433460">So</span>
  <span m="3433480">that's</span> <span m="3433720">important.</span> <span m="3434080">You've</span>
  <span m="3434150">got</span> <span m="3434230">to</span> <span m="3434300">recognize</span>
  <span m="3434680">what's</span> <span m="3434800">going</span> <span m="3435010">on.</span>
  <span m="3436090">But</span> <span m="3436780">what</span> <span m="3436880">do</span>
  <span m="3436920">you</span> <span m="3436990">do</span> <span m="3437200">about</span>
  <span m="3437440">it?</span> <span m="3437780">So</span> <span m="3438450">here</span>
  <span m="3438690">are</span> <span m="3438760">some</span> <span m="3438970">hacks.</span></p><p><span
  m="3440820">Hack</span> <span m="3441110">number</span> <span m="3441360">1--</span>
  <span m="3442190">modify</span> <span m="3442850">the</span> <span m="3442940">model.</span>
  <span m="3443390">This</span> <span m="3443570">is</span> <span m="3443690">the</span>
  <span m="3443780">solution</span> <span m="3444260">that</span> <span m="3444350">is</span>
  <span m="3444410">proposed</span> <span m="3444800">in</span> <span m="3444890">the</span>
  <span m="3444980">paper</span> <span m="3445280">you</span> <span m="3445370">read.</span>
  <span m="3446120">They</span> <span m="3446270">said,</span> <span m="3446510">OK,</span>
  <span m="3446990">if</span> <span m="3447170">it's</span> <span m="3447270">a</span>
  <span m="3447380">simple</span> <span m="3447770">rule-based</span> <span m="3449000">prediction</span>
  <span m="3449740">that</span> <span m="3450390">the</span> <span m="3450710">learning</span>
  <span m="3451010">algorithm</span> <span m="3451340">outputs</span> <span m="3451730">to</span>
  <span m="3451820">you,</span> <span m="3452360">you</span> <span m="3452480">could</span>
  <span m="3452600">see</span> <span m="3452960">the</span> <span m="3453080">rule</span>
  <span m="3453360">that</span> <span m="3453470">doesn't</span> <span m="3453740">make</span>
  <span m="3453920">sense,</span> <span m="3455180">you</span> <span m="3455330">could</span>
  <span m="3455450">use</span> <span m="3455660">your</span> <span m="3455780">clinical</span>
  <span m="3456410">insight</span> <span m="3456800">to</span> <span m="3456920">recognize</span>
  <span m="3457340">it</span> <span m="3457420">doesn't</span> <span m="3457520">make</span>
  <span m="3457660">sense.</span> <span m="3457850">You</span> <span m="3457910">might</span>
  <span m="3458030">even</span> <span m="3458210">be able to</span> <span m="3458370">explain</span>
  <span m="3458810">why</span> <span m="3458990">it</span> <span m="3459050">happened.</span>
  <span m="3459500">And</span> <span m="3459590">then</span> <span m="3459710">you</span>
  <span m="3459800">just</span> <span m="3459950">remove</span> <span m="3460370">that</span>
  <span m="3460550">rule.</span></p><p><span m="3461780">So</span> <span m="3463100">you</span>
  <span m="3463280">manually</span> <span m="3463910">modify</span> <span m="3464600">the</span>
  <span m="3464660">model</span> <span m="3466640">to</span> <span m="3466850">push</span>
  <span m="3467090">it</span> <span m="3467150">towards</span> <span m="3467360">something</span>
  <span m="3467570">that's</span> <span m="3467690">more</span> <span m="3467840">sensible.</span>
  <span m="3469216">All</span> <span m="3469620">right,</span> <span m="3469690">so</span>
  <span m="3469760">that's</span> <span m="3469970">what</span> <span m="3470090">was</span>
  <span m="3470180">suggested.</span> <span m="3470550">And</span> <span m="3470650">I</span>
  <span m="3470750">think</span> <span m="3470840">it's</span> <span m="3470930">nonsense.</span>
  <span m="3472020">I</span> <span m="3472130">don't</span> <span m="3472280">think</span>
  <span m="3472430">that's</span> <span m="3472610">ever</span> <span m="3472850">going</span>
  <span m="3472970">to</span> <span m="3473030">work</span> <span m="3474260">in</span>
  <span m="3474620">today's</span> <span m="3475040">world.</span> <span m="3476060">In</span>
  <span m="3476180">today's</span> <span m="3476480">world</span> <span m="3476690">of</span>
  <span m="3476780">high-dimensional</span> <span m="3477350">models,</span> <span
  m="3478940">there's</span> <span m="3479120">always</span> <span m="3479420">going</span>
  <span m="3479600">to</span> <span m="3479690">be</span> <span m="3479750">surrogates</span>
  <span m="3481220">which</span> <span m="3481490">are</span> <span m="3481550">somehow</span>
  <span m="3481940">picked</span> <span m="3482210">up</span> <span m="3482300">by</span>
  <span m="3482440">a</span> <span m="3482510">learning</span> <span m="3482810">algorithm</span>
  <span m="3483290">that</span> <span m="3483470">you</span> <span m="3483620">will</span>
  <span m="3483770">not</span> <span m="3484010">even</span> <span m="3484190">recognize.</span>
  <span m="3485510">And</span> <span m="3485660">it</span> <span m="3485720">will</span>
  <span m="3485840">be</span> <span m="3485990">really</span> <span m="3486500">hard</span>
  <span m="3486740">to</span> <span m="3486890">modify</span> <span m="3487450">it</span>
  <span m="3487580">in</span> <span m="3487670">the</span> <span m="3487760">way</span>
  <span m="3487910">that</span> <span m="3488030">you</span> <span m="3488150">want.</span></p><p><span
  m="3489260">Maybe</span> <span m="3489410">it's</span> <span m="3489530">impossible</span>
  <span m="3489980">using</span> <span m="3490220">the</span> <span m="3490280">simple</span>
  <span m="3490520">approach,</span> <span m="3490790">by</span> <span m="3490940">the</span>
  <span m="3491030">way.</span> <span m="3491540">Another</span> <span m="3491840">interesting</span>
  <span m="3492200">research</span> <span m="3492470">question--</span> <span m="3492920">how</span>
  <span m="3493100">do</span> <span m="3493190">you</span> <span m="3493280">actually</span>
  <span m="3493850">make</span> <span m="3494090">this</span> <span m="3494270">work</span>
  <span m="3494480">in a</span> <span m="3494570">high-dimensional</span> <span m="3495020">setting?</span></p><p><span
  m="3496820">But</span> <span m="3496910">for</span> <span m="3497030">now,</span>
  <span m="3497210">let's</span> <span m="3497360">say</span> <span m="3497510">we</span>
  <span m="3497600">don't</span> <span m="3497720">know</span> <span m="3497810">how</span>
  <span m="3497900">to</span> <span m="3498020">do</span> <span m="3498170">it</span>
  <span m="3498260">in a</span> <span m="3498460">high-dimensional</span> <span m="3498730">setting.</span>
  <span m="3499080">So</span> <span m="3499100">what</span> <span m="3499220">are</span>
  <span m="3499280">your</span> <span m="3499430">other</span> <span m="3499610">choices?</span>
  <span m="3500480">Hack</span> <span m="3500750">number</span> <span m="3500990">2</span>
  <span m="3502070">is</span> <span m="3502400">to</span> <span m="3502580">redefine</span>
  <span m="3503180">the</span> <span m="3503240">outcome</span> <span m="3503570">altogether,</span>
  <span m="3504080">to</span> <span m="3504230">change</span> <span m="3504770">what</span>
  <span m="3504980">you're</span> <span m="3505100">predicting.</span> <span m="3506180">So</span>
  <span m="3506360">for</span> <span m="3506450">example,</span> <span m="3507630">if</span>
  <span m="3507730">you</span> <span m="3507830">go</span> <span m="3507860">back</span>
  <span m="3508040">to</span> <span m="3508160">this</span> <span m="3508280">picture,</span>
  <span m="3509570">and</span> <span m="3509930">instead</span> <span m="3510320">of</span>
  <span m="3510440">trying</span> <span m="3510680">to</span> <span m="3510770">predict</span>
  <span m="3511040">Y,</span> <span m="3511490">death,</span> <span m="3512360">if</span>
  <span m="3512480">you</span> <span m="3512570">could</span> <span m="3512690">try</span>
  <span m="3512960">to</span> <span m="3513050">find</span> <span m="3513290">some</span>
  <span m="3513470">surrogate</span> <span m="3514100">for</span> <span m="3514220">the</span>
  <span m="3514310">thing</span> <span m="3514490">you</span> <span m="3514610">care</span>
  <span m="3514850">about,</span> <span m="3515150">which</span> <span m="3515330">is</span>
  <span m="3515450">pre-treatment,</span> <span m="3517410">and</span> <span m="3517520">you</span>
  <span m="3517580">predict</span> <span m="3517880">that</span> <span m="3518270">thing</span>
  <span m="3518600">instead,</span> <span m="3520160">then</span> <span m="3520880">you'll</span>
  <span m="3521090">be</span> <span m="3521210">back</span> <span m="3521480">in</span>
  <span m="3521570">business.</span></p><p><span m="3523070">And</span> <span m="3523190">so,</span>
  <span m="3523400">for</span> <span m="3523520">example,</span> <span m="3523950">in</span>
  <span m="3524000">one</span> <span m="3524120">of</span> <span m="3524180">the</span>
  <span m="3524270">optional</span> <span m="3524660">readings</span> <span m="3525240">for--</span>
  <span m="3526215">or</span> <span m="3526700">actually</span> <span m="3526970">I</span>
  <span m="3527060">think</span> <span m="3527210">in</span> <span m="3528140">the</span>
  <span m="3528230">second</span> <span m="3528680">required</span> <span m="3529040">reading</span>
  <span m="3529310">for</span> <span m="3529430">today's</span> <span m="3529910">class,</span>
  <span m="3530700">it</span> <span m="3530830">was</span> <span m="3530960">a</span>
  <span m="3530990">paper</span> <span m="3531380">about</span> <span m="3531740">risk</span>
  <span m="3532100">revocation</span> <span m="3532760">for</span> <span m="3533030">sepsis,</span>
  <span m="3533910">which</span> <span m="3533990">is</span> <span m="3534740">often</span>
  <span m="3535040">caused</span> <span m="3535400">by</span> <span m="3535700">infection.</span>
  <span m="3536850">And</span> <span m="3537410">what</span> <span m="3537560">they</span>
  <span m="3537680">show</span> <span m="3537950">in</span> <span m="3538040">that</span>
  <span m="3538160">article</span> <span m="3538640">is</span> <span m="3538790">that</span>
  <span m="3539360">there</span> <span m="3539600">are</span> <span m="3539690">laboratory</span>
  <span m="3540200">test</span> <span m="3540410">results,</span> <span m="3540800">such</span>
  <span m="3541010">as</span> <span m="3541130">lactate,</span> <span m="3541850">and</span>
  <span m="3541940">there</span> <span m="3542030">are</span> <span m="3542060">others,</span>
  <span m="3542840">which</span> <span m="3543080">can</span> <span m="3543290">give</span>
  <span m="3543530">you</span> <span m="3543980">a</span> <span m="3544040">hint</span>
  <span m="3544460">that</span> <span m="3545060">this</span> <span m="3545240">patient</span>
  <span m="3545630">might</span> <span m="3545840">be</span> <span m="3545990">on</span>
  <span m="3546110">a</span> <span m="3546170">path</span> <span m="3546500">to</span>
  <span m="3546620">clinical</span> <span m="3546950">deterioration.</span> <span
  m="3548960">And</span> <span m="3549080">that</span> <span m="3549500">test</span>
  <span m="3550220">might</span> <span m="3550460">precede</span> <span m="3551360">the</span>
  <span m="3551510">interventions</span> <span m="3552320">to</span> <span m="3552380">try</span>
  <span m="3552590">to</span> <span m="3552680">take</span> <span m="3552920">care</span>
  <span m="3553340">of</span> <span m="3553670">that</span> <span m="3553910">condition.</span>
  <span m="3555140">And</span> <span m="3555260">so</span> <span m="3555350">if</span>
  <span m="3555410">you</span> <span m="3556550">instead</span> <span m="3556790">change</span>
  <span m="3557150">your</span> <span m="3557240">outcome</span> <span m="3557720">to</span>
  <span m="3557810">be</span> <span m="3557960">predicting</span> <span m="3559040">that</span>
  <span m="3559220">surrogate,</span> <span m="3560600">then</span> <span m="3561080">you're</span>
  <span m="3561230">getting</span> <span m="3561530">around</span> <span m="3562070">this</span>
  <span m="3562220">problem</span> <span m="3562550">that</span> <span m="3562700">I</span>
  <span m="3562790">just</span> <span m="3563510">pointed</span> <span m="3563840">out.</span></p><p><span
  m="3566470">Now,</span> <span m="3566680">a</span> <span m="3566770">third</span>
  <span m="3567250">hack</span> <span m="3568330">is</span> <span m="3570160">from</span>
  <span m="3570430">one</span> <span m="3570550">of</span> <span m="3570610">the</span>
  <span m="3570700">optional</span> <span m="3571150">readings</span> <span m="3571450">from</span>
  <span m="3571570">today's</span> <span m="3571810">lecture,</span> <span m="3572170">this</span>
  <span m="3572320">paper</span> <span m="3572620">by</span> <span m="3572970">Suchi</span>
  <span m="3573170">Saria</span> <span m="3573480">and</span> <span m="3573580">her</span>
  <span m="3573670">students,</span> <span m="3574180">from</span> <span m="3574360"><i>Science</i></span>
  <span m="3574690"><i>Translational</i></span> <span m="3575080"><i>Medicine</i></span>
  <span m="3575380">2015.</span> <span m="3576080">It's</span> <span m="3576170">a</span>
  <span m="3576220">really</span> <span m="3576550">well-written</span> <span m="3576940">paper.</span>
  <span m="3577240">I</span> <span m="3577330">highly</span> <span m="3577510">recommend</span>
  <span m="3577780">reading</span> <span m="3578050">it.</span> <span m="3578960">In</span>
  <span m="3579010">that</span> <span m="3579190">paper,</span> <span m="3580000">they</span>
  <span m="3580150">suggest</span> <span m="3580810">formalizing</span> <span m="3581800">the</span>
  <span m="3581860">problem</span> <span m="3582370">as</span> <span m="3582550">one</span>
  <span m="3582700">of</span> <span m="3582760">censoring,</span> <span m="3583570">which</span>
  <span m="3583720">is</span> <span m="3583810">what</span> <span m="3583990">we'll</span>
  <span m="3584080">be</span> <span m="3584140">talking</span> <span m="3584380">about</span>
  <span m="3584560">for</span> <span m="3584710">the</span> <span m="3584830">very</span>
  <span m="3585100">last</span> <span m="3585400">third</span> <span m="3585670">of</span>
  <span m="3585760">today's</span> <span m="3586030">lecture.</span></p><p><span m="3587110">In</span>
  <span m="3587180">particular,</span> <span m="3587600">what</span> <span m="3587680">they</span>
  <span m="3587830">say</span> <span m="3588100">is</span> <span m="3590350">suppose</span>
  <span m="3590830">you</span> <span m="3590980">see</span> <span m="3591250">that</span>
  <span m="3591370">a</span> <span m="3591430">patient</span> <span m="3591730">is</span>
  <span m="3591880">treated</span> <span m="3592330">for</span> <span m="3592450">the</span>
  <span m="3592540">condition.</span> <span m="3593210">Let's</span> <span m="3593290">say</span>
  <span m="3593560">they're</span> <span m="3593710">treated</span> <span m="3594190">for</span>
  <span m="3594520">sepsis.</span> <span m="3596620">Then</span> <span m="3596800">if</span>
  <span m="3596890">the</span> <span m="3596950">patient</span> <span m="3597250">is</span>
  <span m="3597340">treated</span> <span m="3597760">for</span> <span m="3597820">that</span>
  <span m="3597940">condition,</span> <span m="3598810">then</span> <span m="3598960">we</span>
  <span m="3599080">don't</span> <span m="3599500">know</span> <span m="3599920">what</span>
  <span m="3600190">would</span> <span m="3600360">have</span> <span m="3600490">happened</span>
  <span m="3600850">to</span> <span m="3600970">them</span> <span m="3601120">had</span>
  <span m="3601300">they</span> <span m="3601390">not</span> <span m="3601600">been</span>
  <span m="3601720">treated.</span> <span m="3602570">So</span> <span m="3602620">we</span>
  <span m="3602740">don't</span> <span m="3602950">observe</span> <span m="3603640">the</span>
  <span m="3603730">outcome,</span> <span m="3604660">death</span> <span m="3605350">given</span>
  <span m="3605770">no</span> <span m="3605980">treatment.</span></p><p><span m="3607990">And</span>
  <span m="3608080">so</span> <span m="3608260">we're</span> <span m="3608350">going</span>
  <span m="3608500">to</span> <span m="3608560">treat</span> <span m="3608770">it</span>
  <span m="3608830">as</span> <span m="3608980">an</span> <span m="3609190">unknown</span>
  <span m="3609730">outcome.</span> <span m="3611070">And</span> <span m="3611410">for</span>
  <span m="3611530">patients</span> <span m="3612010">who</span> <span m="3612160">were</span>
  <span m="3612370">not</span> <span m="3612910">treated,</span> <span m="3613930">but</span>
  <span m="3614140">ended</span> <span m="3614380">up</span> <span m="3614500">dying</span>
  <span m="3614890">due</span> <span m="3615010">to</span> <span m="3615100">sepsis,</span>
  <span m="3616120">then</span> <span m="3616300">they're</span> <span m="3616450">not</span>
  <span m="3616690">censored.</span> <span m="3617530">And</span> <span m="3617890">what</span>
  <span m="3618040">I'll</span> <span m="3618130">show</span> <span m="3618310">you</span>
  <span m="3618430">in</span> <span m="3618520">the</span> <span m="3618700">later</span>
  <span m="3618940">part</span> <span m="3619090">of</span> <span m="3619150">the</span>
  <span m="3619270">class</span> <span m="3619670">is</span> <span m="3619840">how</span>
  <span m="3620020">to</span> <span m="3620140">learn</span> <span m="3620500">from</span>
  <span m="3620680">censored</span> <span m="3621040">data.</span> <span m="3621390">So</span>
  <span m="3621820">this</span> <span m="3622210">is</span> <span m="3622300">another</span>
  <span m="3622780">formalization</span> <span m="3623470">which</span> <span m="3623620">tries</span>
  <span m="3624250">to</span> <span m="3624460">address</span> <span m="3624820">this</span>
  <span m="3625000">problem</span> <span m="3625360">that</span> <span m="3625510">we</span>
  <span m="3625600">pointed</span> <span m="3625900">out.</span></p><p><span m="3627170">Now,</span>
  <span m="3627340">I</span> <span m="3627410">call</span> <span m="3627730">these</span>
  <span m="3627940">hacks</span> <span m="3628270">because,</span> <span m="3628870">really,</span>
  <span m="3629680">I</span> <span m="3629740">think</span> <span m="3629920">what</span>
  <span m="3630010">we</span> <span m="3630100">should</span> <span m="3630220">be</span>
  <span m="3630280">doing</span> <span m="3631210">is</span> <span m="3631330">formalizing</span>
  <span m="3631930">it</span> <span m="3632050">using</span> <span m="3632320">the</span>
  <span m="3632410">language</span> <span m="3632740">of</span> <span m="3632800">causality.</span>
  <span m="3635200">Once</span> <span m="3635620">you</span> <span m="3635740">do</span>
  <span m="3635920">this</span> <span m="3636070">introspection</span> <span m="3636670">and</span>
  <span m="3636760">you</span> <span m="3636820">realize</span> <span m="3637450">that</span>
  <span m="3637720">there</span> <span m="3637920">is</span> <span m="3638110">treatment,</span>
  <span m="3638930">in</span> <span m="3639030">fact,</span> <span m="3639290">you</span>
  <span m="3639390">should</span> <span m="3639490">be</span> <span m="3639670">rethinking</span>
  <span m="3640390">about</span> <span m="3640570">the</span> <span m="3640660">problem</span>
  <span m="3640990">as</span> <span m="3641140">one</span> <span m="3641350">of</span>
  <span m="3641560">now</span> <span m="3641800">having</span> <span m="3642070">three</span>
  <span m="3642460">quantities</span> <span m="3642735">of</span> <span m="3643010">interest.</span>
  <span m="3643870">There's</span> <span m="3644110">the</span> <span m="3644170">patient,</span>
  <span m="3644650">everything</span> <span m="3645010">you</span> <span m="3645070">know</span>
  <span m="3645220">about</span> <span m="3645460">them</span> <span m="3645760">at</span>
  <span m="3645910">triage.</span> <span m="3646360">That's</span> <span m="3646570">the</span>
  <span m="3646690">X-variable</span> <span m="3646930">I</span> <span m="3647260">showed</span>
  <span m="3647410">you</span> <span m="3647500">before.</span> <span m="3648430">There's</span>
  <span m="3648670">the</span> <span m="3648880">outcome,</span> <span m="3649390">let's</span>
  <span m="3649510">say,</span> <span m="3649750">Y.</span> <span m="3650440">And</span>
  <span m="3650560">then</span> <span m="3650710">there's</span> <span m="3650950">that</span>
  <span m="3651550">everything</span> <span m="3651940">that</span> <span m="3652030">happened</span>
  <span m="3652240">in</span> <span m="3652300">between,</span> <span m="3652660">in</span>
  <span m="3652720">particular</span> <span m="3653260">the</span> <span m="3653320">interventions</span>
  <span m="3654190">that</span> <span m="3654430">happened</span> <span m="3654740">in</span>
  <span m="3654850">between.</span> <span m="3655270">We'll</span> <span m="3655360">call</span>
  <span m="3655540">that</span> <span m="3655720">T,</span> <span m="3656170">for</span>
  <span m="3656380">treatment.</span></p><p><span m="3658120">And</span> <span m="3658750">the</span>
  <span m="3658930">question</span> <span m="3660060">that</span> <span m="3660250">one</span>
  <span m="3660460">would</span> <span m="3660610">like</span> <span m="3660850">to</span>
  <span m="3661030">ask</span> <span m="3661810">in</span> <span m="3661960">order</span>
  <span m="3662170">to</span> <span m="3662290">figure</span> <span m="3662530">out</span>
  <span m="3662650">how</span> <span m="3662770">to</span> <span m="3662860">optimally</span>
  <span m="3663640">care</span> <span m="3664030">for</span> <span m="3664180">the</span>
  <span m="3664270">patient</span> <span m="3664840">is</span> <span m="3665050">one</span>
  <span m="3665410">of,</span> <span m="3666280">will</span> <span m="3666790">admission</span>
  <span m="3667330">to</span> <span m="3667480">the</span> <span m="3667600">ICU,</span>
  <span m="3668450">which</span> <span m="3668530">is</span> <span m="3668650">the</span>
  <span m="3668770">intervention</span> <span m="3669370">that</span> <span m="3669460">we're</span>
  <span m="3669580">considering</span> <span m="3670060">here,</span> <span m="3670690">will</span>
  <span m="3670990">that</span> <span m="3671260">lower</span> <span m="3672040">the</span>
  <span m="3672190">likelihood</span> <span m="3672850">of</span> <span m="3672970">death</span>
  <span m="3673360">for</span> <span m="3673510">the</span> <span m="3673600">patient?</span>
  <span m="3675550">And</span> <span m="3675640">now</span> <span m="3675790">when</span>
  <span m="3675910">I</span> <span m="3676000">say</span> <span m="3676210">lower,</span>
  <span m="3676480">I</span> <span m="3676600">don't</span> <span m="3676780">mean</span>
  <span m="3677770">correlation,</span> <span m="3678610">I</span> <span m="3678730">mean</span>
  <span m="3678940">causation.</span> <span m="3679660">Will</span> <span m="3679990">it</span>
  <span m="3680170">actually</span> <span m="3680800">lower</span> <span m="3681310">the</span>
  <span m="3681400">patient's</span> <span m="3681760">risk</span> <span m="3682000">of</span>
  <span m="3682090">dying?</span> <span m="3683620">I</span> <span m="3683710">think</span>
  <span m="3683890">we</span> <span m="3684040">need</span> <span m="3684250">to</span>
  <span m="3684400">hit</span> <span m="3684670">these</span> <span m="3684880">questions</span>
  <span m="3685300">on</span> <span m="3685510">the</span> <span m="3685630">head</span>
  <span m="3685900">with</span> <span m="3686860">actually</span> <span m="3687340">thinking</span>
  <span m="3687670">about</span> <span m="3687820">causality</span> <span m="3688720">to</span>
  <span m="3688840">try</span> <span m="3688990">to</span> <span m="3689140">formalize</span>
  <span m="3689620">this</span> <span m="3689740">properly.</span> <span m="3690580">And</span>
  <span m="3690730">if</span> <span m="3690850">you</span> <span m="3690940">do</span>
  <span m="3691180">that,</span> <span m="3691930">this</span> <span m="3692140">will</span>
  <span m="3692230">be</span> <span m="3692350">a</span> <span m="3692380">solution</span>
  <span m="3692770">which</span> <span m="3693040">will</span> <span m="3693190">generalize</span>
  <span m="3693940">to</span> <span m="3694030">the</span> <span m="3694120">high-dimensional</span>
  <span m="3694690">settings</span> <span m="3695110">that</span> <span m="3695230">we</span>
  <span m="3695320">care</span> <span m="3695530">about in</span> <span m="3695780">machine</span>
  <span m="3696040">learning.</span></p><p><span m="3697450">And</span> <span m="3697600">this</span>
  <span m="3697750">will</span> <span m="3697840">be</span> <span m="3697960">a</span>
  <span m="3698020">topic</span> <span m="3699380">that</span> <span m="3699610">we'll</span>
  <span m="3699730">talk</span> <span m="3700060">really</span> <span m="3700280">in-depth</span>
  <span m="3700870">after</span> <span m="3701350">spring</span> <span m="3701620">break.</span>
  <span m="3701960">But</span> <span m="3702060">I</span> <span m="3702160">wanted</span>
  <span m="3702250">to</span> <span m="3702340">give</span> <span m="3702550">you</span>
  <span m="3702880">this</span> <span m="3703210">as</span> <span m="3703480">one</span>
  <span m="3703840">motivation</span> <span m="3704440">for</span> <span m="3704530">why</span>
  <span m="3704770">it's</span> <span m="3704860">so</span> <span m="3705010">important--</span>
  <span m="3705620">there</span> <span m="3705720">are</span> <span m="3705820">many</span>
  <span m="3705920">other</span> <span m="3705940">reasons--</span> <span m="3706530">to
  really</span> <span m="3706780">think</span> <span m="3707050">about</span> <span
  m="3707440">it</span> <span m="3707560">from</span> <span m="3707740">a</span> <span
  m="3707770">causal</span> <span m="3708100">perspective.</span></p><p><span m="3710700">OK,</span>
  <span m="3711850">so</span> <span m="3712250">subtlety</span> <span m="3712720">number</span>
  <span m="3712990">3--</span> <span m="3715570">there's</span> <span m="3715780">been</span>
  <span m="3715960">a</span> <span m="3716140">ton</span> <span m="3716440">of</span>
  <span m="3716560">hype</span> <span m="3716830">in</span> <span m="3716920">the</span>
  <span m="3716980">media</span> <span m="3717490">about</span> <span m="3717940">deep</span>
  <span m="3718210">learning</span> <span m="3718510">and</span> <span m="3718600">health</span>
  <span m="3718800">care.</span> <span m="3719590">A</span> <span m="3719680">lot</span>
  <span m="3719950">of</span> <span m="3720070">it</span> <span m="3720160">is</span>
  <span m="3720310">very</span> <span m="3720610">well</span> <span m="3720820">warranted.</span>
  <span m="3721570">For</span> <span m="3721690">example,</span> <span m="3722170">the</span>
  <span m="3722440">advances</span> <span m="3722860">we're</span> <span m="3722950">seeing</span>
  <span m="3723340">in</span> <span m="3723460">areas</span> <span m="3724180">ranging</span>
  <span m="3724600">from</span> <span m="3725590">radiology</span> <span m="3726400">and</span>
  <span m="3726480">pathology</span> <span m="3727390">to</span> <span m="3729100">interpretation</span>
  <span m="3730030">of</span> <span m="3730690">EKGs</span> <span m="3731650">are</span>
  <span m="3731890">all</span> <span m="3732280">really</span> <span m="3732970">being</span>
  <span m="3733270">transformed</span> <span m="3734170">by</span> <span m="3734380">deep</span>
  <span m="3734620">learning</span> <span m="3734890">algorithms.</span></p><p><span
  m="3736510">But</span> <span m="3736690">the</span> <span m="3736750">problems</span>
  <span m="3737140">I've</span> <span m="3737230">been</span> <span m="3737350">telling</span>
  <span m="3737680">you</span> <span m="3737770">about</span> <span m="3738040">for</span>
  <span m="3738190">the</span> <span m="3738250">last</span> <span m="3738460">couple</span>
  <span m="3738760">of</span> <span m="3738790">weeks,</span> <span m="3740110">of</span>
  <span m="3740200">doing</span> <span m="3740410">risk</span> <span m="3740590">stratification</span>
  <span m="3741460">on</span> <span m="3741790">electronic</span> <span m="3742210">health</span>
  <span m="3742420">record</span> <span m="3742660">data,</span> <span m="3743180">such</span>
  <span m="3743500">as</span> <span m="3744310">taxed </span> <span m="3744820">notes,</span>
  <span m="3745480">such</span> <span m="3745810">as</span> <span m="3746440">lab</span>
  <span m="3746710">test</span> <span m="3746920">results</span> <span m="3747520">and</span>
  <span m="3748630">vital</span> <span m="3748930">signs,</span> <span m="3750460">diagnosis</span>
  <span m="3751000">codes,</span> <span m="3751990">that's</span> <span m="3752230">a</span>
  <span m="3752260">different</span> <span m="3752530">story.</span> <span m="3753110">And</span>
  <span m="3753210">in</span> <span m="3753310">fact,</span> <span m="3753950">if</span>
  <span m="3754000">you</span> <span m="3754090">look</span> <span m="3754270">closely</span>
  <span m="3754990">at</span> <span m="3755110">all</span> <span m="3755280">of</span>
  <span m="3755350">the</span> <span m="3755440">papers,</span> <span m="3755860">all</span>
  <span m="3756140">the</span> <span m="3756220">papers</span> <span m="3756580">that
  have</span> <span m="3756670">been</span> <span m="3756790">published</span> <span
  m="3757360">in</span> <span m="3757480">the</span> <span m="3757570">last</span>
  <span m="3758740">few</span> <span m="3758980">years</span> <span m="3759440">that</span>
  <span m="3759510">have</span> <span m="3759580">been</span> <span m="3759670">trying</span>
  <span m="3760120">to</span> <span m="3760210">apply</span> <span m="3760520">the</span>
  <span m="3760630">gauntlet</span> <span m="3761140">of</span> <span m="3761230">deep</span>
  <span m="3761410">learning</span> <span m="3761680">algorithms</span> <span m="3762100">at</span>
  <span m="3762280">those</span> <span m="3762670">problems,</span> <span m="3763690">in</span>
  <span m="3763810">fact,</span> <span m="3764080">the</span> <span m="3764200">gains</span>
  <span m="3764590">are</span> <span m="3764830">very</span> <span m="3765280">small.</span></p><p><span
  m="3767240">And</span> <span m="3767260">so</span> <span m="3767470">what</span>
  <span m="3767650">I'm</span> <span m="3767770">showing</span> <span m="3767980">you</span>
  <span m="3768070">here</span> <span m="3768220">is</span> <span m="3768310">just</span>
  <span m="3768430">one</span> <span m="3768670">example</span> <span m="3769090">of</span>
  <span m="3769150">such</span> <span m="3769360">a</span> <span m="3769420">paper.</span>
  <span m="3770210">This</span> <span m="3770290">is</span> <span m="3770370">a</span>
  <span m="3770410">paper</span> <span m="3770740">that</span> <span m="3770890">received</span>
  <span m="3771220">a</span> <span m="3771250">lot</span> <span m="3771550">of</span>
  <span m="3771760">media</span> <span m="3772090">attention.</span> <span m="3772510">It's</span>
  <span m="3772630">a</span> <span m="3772690">Google</span> <span m="3773020">paper</span>
  <span m="3774190">called</span> <span m="3774460">&quot;Scalable</span> <span m="3774940">and</span>
  <span m="3775030">Accurate</span> <span m="3775330">Deep</span> <span m="3775600">Learning</span>
  <span m="3775870">with</span> <span m="3775990">Electronic</span> <span m="3776410">Health</span>
  <span m="3776590">Records.&quot;</span> <span m="3777310">And</span> <span m="3777580">if</span>
  <span m="3777730">you</span> <span m="3778240">go</span> <span m="3778480">across</span>
  <span m="3778810">the</span> <span m="3778910">United</span> <span m="3778960">States,</span>
  <span m="3779230">if</span> <span m="3779320">you</span> <span m="3779410">go</span>
  <span m="3779680">internationally,</span> <span m="3780370">you</span> <span m="3780430">talk</span>
  <span m="3780700">to</span> <span m="3780970">chief</span> <span m="3781300">medical</span>
  <span m="3781600">information</span> <span m="3781960">officers,</span> <span m="3782610">they're</span>
  <span m="3782800">all</span> <span m="3783010">going</span> <span m="3783130">to</span>
  <span m="3783190">be</span> <span m="3783250">telling</span> <span m="3783520">you</span>
  <span m="3783580">about</span> <span m="3783730">this</span> <span m="3783880">paper.</span>
  <span m="3784120">They've</span> <span m="3784300">all</span> <span m="3784420">read</span>
  <span m="3784570">it,</span> <span m="3784780">they've</span> <span m="3784960">all</span>
  <span m="3785050">heard</span> <span m="3785200">about</span> <span m="3785380">it,</span>
  <span m="3785470">and</span> <span m="3785590">they</span> <span m="3785680">all</span>
  <span m="3785770">want</span> <span m="3785920">to</span> <span m="3785980">use</span>
  <span m="3786160">it.</span></p><p><span m="3788440">But</span> <span m="3788530">what</span>
  <span m="3788650">is</span> <span m="3788740">this</span> <span m="3788890">actually</span>
  <span m="3789250">doing?</span> <span m="3789550">What's</span> <span m="3789670">going</span>
  <span m="3789820">on</span> <span m="3789880">behind</span> <span m="3790120">the</span>
  <span m="3790180">scenes?</span> <span m="3791030">Well,</span> <span m="3791590">this</span>
  <span m="3791830">paper</span> <span m="3793170">uses</span> <span m="3793500">the</span>
  <span m="3793600">same</span> <span m="3793900">sorts</span> <span m="3794230">of</span>
  <span m="3794290">data</span> <span m="3794600">we've</span> <span m="3794620">been</span>
  <span m="3794740">talking</span> <span m="3795070">about.</span> <span m="3795970">It</span>
  <span m="3796900">takes</span> <span m="3797150">vitals,</span> <span m="3797550">notes,</span>
  <span m="3797870">orders,</span> <span m="3798370">medications,</span> <span m="3799530">thinks</span>
  <span m="3799790">about</span> <span m="3799960">it as</span> <span m="3800080">a</span>
  <span m="3800160">timeline,</span> <span m="3801160">summarizes</span> <span m="3802060">it,</span>
  <span m="3802210">then</span> <span m="3802420">uses</span> <span m="3802700">a</span>
  <span m="3802860">recurrent</span> <span m="3803290">neural</span> <span m="3803390">network.</span>
  <span m="3803750">It</span> <span m="3803870">also</span> <span m="3803980">uses</span>
  <span m="3804400">attentional</span> <span m="3804940">architectures.</span> <span
  m="3805870">And</span> <span m="3805990">there's</span> <span m="3806130">some</span>
  <span m="3806260">pretty</span> <span m="3806500">smart</span> <span m="3806770">people</span>
  <span m="3807040">on</span> <span m="3807100">this</span> <span m="3807250">paper--</span>
  <span m="3808046">you know,</span> <span m="3808920">Greg</span> <span m="3809170">Corrado,</span>
  <span m="3809950">Jeff</span> <span m="3810250">Dean,</span> <span m="3810670">are</span>
  <span m="3810730">all</span> <span m="3811480">co-authors</span> <span m="3811990">of</span>
  <span m="3812050">this</span> <span m="3812170">paper.</span> <span m="3813190">They</span>
  <span m="3813310">know</span> <span m="3813430">what</span> <span m="3813550">they're</span>
  <span m="3813640">doing.</span></p><p><span m="3814345">All right, so</span> <span
  m="3814660">they</span> <span m="3814780">use</span> <span m="3815080">these</span>
  <span m="3815290">algorithms</span> <span m="3816040">to</span> <span m="3816220">predict</span>
  <span m="3816580">a</span> <span m="3816640">number</span> <span m="3816940">of</span>
  <span m="3817000">downstream</span> <span m="3817480">problems--</span> <span m="3818020">readmission</span>
  <span m="3818650">risk,</span> <span m="3819940">for</span> <span m="3820090">example,</span>
  <span m="3820480">30-day</span> <span m="3820780">readmission,</span> <span m="3821200">like</span>
  <span m="3821350">you</span> <span m="3821440">read</span> <span m="3821590">about</span>
  <span m="3821920">in</span> <span m="3822250">your</span> <span m="3822370">readings</span>
  <span m="3822700">for</span> <span m="3822820">this</span> <span m="3823000">week.</span>
  <span m="3824710">And</span> <span m="3826240">they</span> <span m="3826420">see</span>
  <span m="3826690">they</span> <span m="3826810">get</span> <span m="3826930">pretty</span>
  <span m="3827200">good</span> <span m="3827320">predictions.</span> <span m="3829150">But</span>
  <span m="3829390">if</span> <span m="3829570">you</span> <span m="3829750">go</span>
  <span m="3830080">to</span> <span m="3830380">the</span> <span m="3830550">supplementary</span>
  <span m="3831520">material,</span> <span m="3833530">which</span> <span m="3833740">is</span>
  <span m="3833860">a</span> <span m="3833920">bit</span> <span m="3834100">hard</span>
  <span m="3834310">to</span> <span m="3834400">find,</span> <span m="3834700">but</span>
  <span m="3834790">here's</span> <span m="3835090">the</span> <span m="3835180">link</span>
  <span m="3835420">for</span> <span m="3835600">all</span> <span m="3835720">of</span>
  <span m="3835810">you,</span> <span m="3835930">and I'll</span> <span m="3836020">post
  it</span> <span m="3836290">to</span> <span m="3836380">my</span> <span m="3836470">slides.</span>
  <span m="3838390">And</span> <span m="3838600">if</span> <span m="3838750">you</span>
  <span m="3838840">look</span> <span m="3839080">at</span> <span m="3839170">the</span>
  <span m="3839320">very</span> <span m="3839890">last</span> <span m="3840310">figure</span>
  <span m="3840790">in</span> <span m="3840870">that</span> <span m="3841030">supplementary</span>
  <span m="3841510">material,</span> <span m="3842590">you'll</span> <span m="3842740">see</span>
  <span m="3842890">something</span> <span m="3843190">interesting.</span></p><p><span
  m="3844670">So</span> <span m="3844720">here</span> <span m="3844970">are</span>
  <span m="3845020">those</span> <span m="3845620">three</span> <span m="3845830">different</span>
  <span m="3846100">tasks</span> <span m="3846490">that they</span> <span m="3846640">studied--</span>
  <span m="3847030">inpatient</span> <span m="3847390">mortality</span> <span m="3847810">prediction,</span>
  <span m="3848320">30-day</span> <span m="3848740">readmission,</span> <span m="3849490">length-of-stay</span>
  <span m="3850060">prediction.</span> <span m="3851720">The</span> <span m="3851740">first</span>
  <span m="3852130">line</span> <span m="3852400">each</span> <span m="3852550">of</span>
  <span m="3852610">these</span> <span m="3852730">buckets</span> <span m="3853240">is</span>
  <span m="3853840">what</span> <span m="3854050">your</span> <span m="3854230">deep</span>
  <span m="3854470">learning</span> <span m="3854740">algorithm</span> <span m="3855160">does.</span>
  <span m="3856330">Over</span> <span m="3856540">here,</span> <span m="3856900">they</span>
  <span m="3857050">have</span> <span m="3857170">two</span> <span m="3857290">different</span>
  <span m="3857530">hospitals.</span> <span m="3858230">I</span> <span m="3858330">think</span>
  <span m="3858370">it</span> <span m="3858460">might</span> <span m="3858580">have</span>
  <span m="3858670">been</span> <span m="3858790">University</span> <span m="3859030">of</span>
  <span m="3859090">Chicago</span> <span m="3859720">and</span> <span m="3859930">Stanford.</span>
  <span m="3861700">And</span> <span m="3862360">they're</span> <span m="3862600">showing</span>
  <span m="3863020">the</span> <span m="3863170">area</span> <span m="3863620">under</span>
  <span m="3863860">the</span> <span m="3863950">ROC</span> <span m="3864400">curve,</span>
  <span m="3864740">which we've</span> <span m="3864970">talked</span> <span m="3865240">about,</span>
  <span m="3866140">performance</span> <span m="3867130">for</span> <span m="3867370">each</span>
  <span m="3867550">of</span> <span m="3867640">these</span> <span m="3867820">tasks</span>
  <span m="3868300">for</span> <span m="3868480">their</span> <span m="3868600">best</span>
  <span m="3868840">models.</span> <span m="3870100">And</span> <span m="3870270">in</span>
  <span m="3870350">the</span> <span m="3870400">parentheses,</span> <span m="3870970">they</span>
  <span m="3871120">give</span> <span m="3871300">confidence</span> <span m="3871780">intervals--</span>
  <span m="3872330">let's</span> <span m="3872440">say</span> <span m="3872980">something</span>
  <span m="3873200">like</span> <span m="3873280">95%</span> <span m="3873850">confidence</span>
  <span m="3874150">intervals--</span> <span m="3874450">for</span> <span m="3874600">area</span>
  <span m="3874850">under the</span> <span m="3875090">ROC curve.</span></p><p><span
  m="3876640">Now,</span> <span m="3876880">the</span> <span m="3877000">second</span>
  <span m="3877630">line</span> <span m="3877900">that</span> <span m="3878020">you</span>
  <span m="3878140">see</span> <span m="3878560">is</span> <span m="3878710">called</span>
  <span m="3879880">full-feature</span> <span m="3880600">enhanced</span> <span m="3881020">baseline.</span>
  <span m="3882900">It's</span> <span m="3883060">using</span> <span m="3883330">the</span>
  <span m="3883390">same</span> <span m="3883810">data,</span> <span m="3884530">but</span>
  <span m="3884710">it's</span> <span m="3884890">using</span> <span m="3885520">something</span>
  <span m="3885940">very</span> <span m="3886300">close</span> <span m="3886930">to</span>
  <span m="3887200">the</span> <span m="3887320">feature</span> <span m="3887690">represetnation</span>
  <span m="3888190">that</span> <span m="3888310">you</span> <span m="3888400">saw</span>
  <span m="3888940">in</span> <span m="3889060">the</span> <span m="3889120">paper</span>
  <span m="3889450">by</span> <span m="3889660">Narges</span> <span m="3889990">Razavian,</span>
  <span m="3890550">so</span> <span m="3890620">that</span> <span m="3890740">paper</span>
  <span m="3891010">on</span> <span m="3891100">diabetes</span> <span m="3891580">prediction</span>
  <span m="3892030">that</span> <span m="3892120">I</span> <span m="3892180">told</span>
  <span m="3892360">you</span> <span m="3892420">about</span> <span m="3892850">and</span>
  <span m="3892950">we've</span> <span m="3892960">been</span> <span m="3893050">criticizing.</span>
  <span m="3894430">So</span> <span m="3894550">it's</span> <span m="3894640">using</span>
  <span m="3894910">that</span> <span m="3895240">L1-regularized</span> <span m="3896170">logistic</span>
  <span m="3896470">regression</span> <span m="3896860">with</span> <span m="3897310">a</span>
  <span m="3897640">smart</span> <span m="3898330">set</span> <span m="3898570">of</span>
  <span m="3898660">features.</span></p><p><span m="3900400">And</span> <span m="3900490">what</span>
  <span m="3900650">you</span> <span m="3900760">see</span> <span m="3902260">across</span>
  <span m="3902740">all</span> <span m="3903100">three</span> <span m="3903340">settings</span>
  <span m="3904210">is</span> <span m="3904390">that</span> <span m="3905050">the</span>
  <span m="3905140">results</span> <span m="3905620">are</span> <span m="3905710">not</span>
  <span m="3906010">physically</span> <span m="3906520">significantly</span> <span
  m="3907090">different.</span> <span m="3909460">So</span> <span m="3909850">let's</span>
  <span m="3909970">look</span> <span m="3910060">at</span> <span m="3910120">the</span>
  <span m="3910180">first</span> <span m="3910450">one,</span> <span m="3910720">hospital</span>
  <span m="3911200">A,</span> <span m="3912160">deep</span> <span m="3912400">learning,</span>
  <span m="3912700">0.95</span> <span m="3913460">AUC.</span> <span m="3914920">This</span>
  <span m="3915120">L1-regularized</span> <span m="3915660">logistic</span> <span
  m="3915790">regression,</span> <span m="3916180">0.93.</span> <span m="3918400">30-day</span>
  <span m="3918820">readmission,</span> <span m="3919360">0.77,</span> <span m="3920170">0.75,</span>
  <span m="3921010">0.86,</span> <span m="3921760">0.85.</span> <span m="3922570">And</span>
  <span m="3922660">the</span> <span m="3922720">confidence</span> <span m="3923110">intervals</span>
  <span m="3923320">are</span> <span m="3923380">all</span> <span m="3923530">overlapping.</span></p><p><span
  m="3926730">So</span> <span m="3928530">what's</span> <span m="3928770">going</span>
  <span m="3929190">on?</span> <span m="3931290">So</span> <span m="3931530">I</span>
  <span m="3931620">think</span> <span m="3931770">what</span> <span m="3931860">you're</span>
  <span m="3931980">seeing</span> <span m="3932190">here,</span> <span m="3932310">first</span>
  <span m="3932580">of</span> <span m="3932670">all,</span> <span m="3933030">is</span>
  <span m="3933900">a</span> <span m="3934020">recognition</span> <span m="3935070">by</span>
  <span m="3935220">the</span> <span m="3935310">machine</span> <span m="3935610">learning</span>
  <span m="3935880">community</span> <span m="3936390">that--</span> <span m="3937680">in</span>
  <span m="3937800">this</span> <span m="3937920">case,</span> <span m="3938130">a</span>
  <span m="3938190">late</span> <span m="3938490">recognition</span> <span m="3939260">that</span>
  <span m="3939450">simpler</span> <span m="3939750">approaches</span> <span m="3940110">tend</span>
  <span m="3940290">to</span> <span m="3940380">work</span> <span m="3940560">well</span>
  <span m="3940710">with</span> <span m="3940830">this</span> <span m="3940950">type</span>
  <span m="3941100">of</span> <span m="3941160">data.</span> <span m="3941940">I</span>
  <span m="3942030">don't</span> <span m="3942150">think</span> <span m="3942300">this</span>
  <span m="3942420">was</span> <span m="3942540">the</span> <span m="3942630">first</span>
  <span m="3942840">thing</span> <span m="3942960">that</span> <span m="3943050">they</span>
  <span m="3943140">tried.</span> <span m="3943740">They</span> <span m="3943890">tried</span>
  <span m="3944400">probably</span> <span m="3944700">the</span> <span m="3944790">deep</span>
  <span m="3944940">learning</span> <span m="3945210">algorithms</span> <span m="3945630">first.</span></p><p><span
  m="3949200">Second,</span> <span m="3949980">we're all</span> <span m="3950340">grasping</span>
  <span m="3950850">at</span> <span m="3950970">this,</span> <span m="3951150">and</span>
  <span m="3951270">we</span> <span m="3951360">all</span> <span m="3951510">want</span>
  <span m="3951720">to</span> <span m="3951780">come</span> <span m="3951960">up</span>
  <span m="3952020">with</span> <span m="3952110">these</span> <span m="3952260">better</span>
  <span m="3952470">algorithms,</span> <span m="3953910">but</span> <span m="3955200">so</span>
  <span m="3955590">far</span> <span m="3955980">we're</span> <span m="3956130">not</span>
  <span m="3956310">doing</span> <span m="3956640">that</span> <span m="3956850">well.</span>
  <span m="3957330">And</span> <span m="3957450">I'll</span> <span m="3957510">tell</span>
  <span m="3957780">you</span> <span m="3957900">more</span> <span m="3958050">about</span>
  <span m="3958200">that</span> <span m="3958320">in</span> <span m="3958380">just</span>
  <span m="3958560">a</span> <span m="3958590">second.</span> <span m="3960040">But</span>
  <span m="3960120">before</span> <span m="3960480">I</span> <span m="3960540">finish</span>
  <span m="3960870">with</span> <span m="3960960">the</span> <span m="3961060">slide,</span>
  <span m="3961260">I</span> <span m="3961320">want</span> <span m="3961440">to</span>
  <span m="3961500">give</span> <span m="3961620">you</span> <span m="3961710">a</span>
  <span m="3961770">punch</span> <span m="3962010">line</span> <span m="3962220">I</span>
  <span m="3962250">think</span> <span m="3962400">is</span> <span m="3962520">really</span>
  <span m="3962670">important.</span> <span m="3964290">You</span> <span m="3964410">might</span>
  <span m="3964620">come</span> <span m="3964830">home</span> <span m="3965010">from</span>
  <span m="3965160">this</span> <span m="3965280">and</span> <span m="3965400">say,</span>
  <span m="3965830">you</span> <span m="3965850">know</span> <span m="3965970">what,</span>
  <span m="3966580">it's</span> <span m="3966600">not</span> <span m="3966720">that</span>
  <span m="3966870">much</span> <span m="3967080">better,</span> <span m="3967260">but</span>
  <span m="3967350">it's</span> <span m="3967440">a</span> <span m="3967500">little</span>
  <span m="3967650">bit</span> <span m="3967770">better--</span> <span m="3968130">0.95</span>
  <span m="3968460">to</span> <span m="3968790">0.93.</span> <span m="3969900">Suppose</span>
  <span m="3970260">it was</span> <span m="3970440">tight</span> <span m="3970710">confidence</span>
  <span m="3970900">intervals,</span> <span m="3972030">there</span> <span m="3972150">might</span>
  <span m="3972300">be</span> <span m="3972360">a</span> <span m="3972420">few</span>
  <span m="3972600">patients</span> <span m="3972990">whose</span> <span m="3973110">lives</span>
  <span m="3973290">you</span> <span m="3973350">could</span> <span m="3973470">save</span>
  <span m="3973650">with</span> <span m="3973830">that.</span></p><p><span m="3975200">But</span>
  <span m="3975270">because</span> <span m="3975580">all</span> <span m="3975780">the</span>
  <span m="3975900">issues</span> <span m="3976170">I've</span> <span m="3976260">told</span>
  <span m="3976470">you</span> <span m="3976530">about</span> <span m="3976680">up</span>
  <span m="3976830">until</span> <span m="3977070">now,</span> <span m="3978120">of</span>
  <span m="3978300">non-stationary,</span> <span m="3979170">for</span> <span m="3979320">example,</span>
  <span m="3980790">those</span> <span m="3981300">gains</span> <span m="3981810">disappear.</span>
  <span m="3982440">In</span> <span m="3982560">many</span> <span m="3982770">cases,</span>
  <span m="3983070">they</span> <span m="3983160">even</span> <span m="3983430">reverse</span>
  <span m="3985170">when</span> <span m="3985350">you</span> <span m="3985470">actually</span>
  <span m="3985770">go</span> <span m="3985890">to</span> <span m="3985980">deploy</span>
  <span m="3986310">these</span> <span m="3986460">models</span> <span m="3987210">because</span>
  <span m="3987810">of</span> <span m="3987900">that</span> <span m="3988080">data</span>
  <span m="3988220">set</span> <span m="3988590">shift</span> <span m="3988850">for</span>
  <span m="3988910">non-stationarity.</span> <span m="3990000">It</span> <span m="3990120">so</span>
  <span m="3990360">happens</span> <span m="3990840">that</span> <span m="3990930">the</span>
  <span m="3991020">simpler</span> <span m="3991470">models</span> <span m="3991920">tend</span>
  <span m="3992130">to</span> <span m="3992250">generalize</span> <span m="3992760">better</span>
  <span m="3993510">when</span> <span m="3993720">your</span> <span m="3993870">data</span>
  <span m="3994170">changes</span> <span m="3994590">on</span> <span m="3994770">you.</span>
  <span m="3995590">And</span> <span m="3995780">this</span> <span m="3995980">is</span>
  <span m="3996060">nicely</span> <span m="3996330">explored</span> <span m="3996750">in</span>
  <span m="3996840">this</span> <span m="3996990">paper</span> <span m="3997920">from</span>
  <span m="3999030">Kenneth</span> <span m="3999310">Jung and</span> <span m="3999690">Nigam
  </span> <span m="4000020">Shah</span> <span m="4000695">in</span> <span m="4000950"><i>Journal</i></span>
  <span m="4001115"><i>of</i></span> <span m="4001280"><i>Biomedical</i></span> <span
  m="4001730"><i>Informatics,</i></span> <span m="4002180">2015.</span></p><p><span
  m="4004040">So</span> <span m="4004720">this</span> <span m="4004900">is</span>
  <span m="4005000">something</span> <span m="4005240">that</span> <span m="4005330">I</span>
  <span m="4005360">want</span> <span m="4005570">you</span> <span m="4005630">to</span>
  <span m="4005690">think</span> <span m="4005900">about.</span> <span m="4006420">Now</span>
  <span m="4007060">let's</span> <span m="4007280">try</span> <span m="4007400">to</span>
  <span m="4007490">answer</span> <span m="4007790">why.</span> <span m="4008540">Well,</span>
  <span m="4009530">the</span> <span m="4009670">areas</span> <span m="4009950">where</span>
  <span m="4010070">we've</span> <span m="4010220">been</span> <span m="4010340">seeing</span>
  <span m="4010610">recurrent</span> <span m="4010910">neural</span> <span m="4010960">networks</span>
  <span m="4011300">doing</span> <span m="4011570">really</span> <span m="4011870">well--</span>
  <span m="4012560">in,</span> <span m="4012680">for</span> <span m="4012770">example,</span>
  <span m="4013230">speech</span> <span m="4013400">recognition,</span> <span m="4014960">natural</span>
  <span m="4015200">language</span> <span m="4015470">processing,</span> <span m="4017000">are</span>
  <span m="4017180">areas</span> <span m="4017810">where,</span> <span m="4019340">often--</span>
  <span m="4020180">for</span> <span m="4020270">example,</span> <span m="4020590">you're</span>
  <span m="4020680">predicting</span> <span m="4021050">what</span> <span m="4021200">is</span>
  <span m="4021320">the</span> <span m="4021410">next</span> <span m="4021650">word</span>
  <span m="4021980">in</span> <span m="4022060">a</span> <span m="4022100">sequence</span>
  <span m="4022490">of</span> <span m="4022580">words,</span> <span m="4022880">the</span>
  <span m="4022940">previous</span> <span m="4023330">few</span> <span m="4023510">words</span>
  <span m="4023840">are</span> <span m="4023900">pretty</span> <span m="4024170">predictive.</span>
  <span m="4025760">Like,</span> <span m="4025970">what</span> <span m="4026180">is</span>
  <span m="4026330">the</span> <span m="4026420">next</span> <span m="4026870">[PAUSES]</span>
  <span m="4027230">that</span> <span m="4027380">I'm</span> <span m="4027470">going</span>
  <span m="4027590">to</span> <span m="4027680">say?</span> <span m="4028250">What</span>
  <span m="4028580">is it?</span></p><p><span m="4028780">AUDIENCE:</span> <span m="4028992">Word.</span></p><p><span
  m="4029630">PROFESSOR:</span> <span m="4029850">Word,</span> <span m="4030070">right,</span>
  <span m="4030270">and</span> <span m="4030350">you</span> <span m="4030470">knew</span>
  <span m="4030680">that,</span> <span m="4030980">right,</span> <span m="4031190">because</span>
  <span m="4031370">it was</span> <span m="4031760">pretty</span> <span m="4032030">obvious</span>
  <span m="4032450">to</span> <span m="4032540">predict</span> <span m="4032750">that.</span>
  <span m="4035310">And</span> <span m="4035330">so</span> <span m="4035660">the</span>
  <span m="4035780">models</span> <span m="4036230">that</span> <span m="4036350">are</span>
  <span m="4036440">good</span> <span m="4036680">at</span> <span m="4036740">predicting</span>
  <span m="4037100">for</span> <span m="4037220">that</span> <span m="4037370">type</span>
  <span m="4037580">of</span> <span m="4037640">data,</span> <span m="4037850">it</span>
  <span m="4037940">doesn't</span> <span m="4038210">mean</span> <span m="4038510">that</span>
  <span m="4038630">they</span> <span m="4038780">should</span> <span m="4038960">be</span>
  <span m="4039110">good</span> <span m="4039350">for</span> <span m="4039440">predicting</span>
  <span m="4039770">for</span> <span m="4039870">a</span> <span m="4039890">different</span>
  <span m="4040190">type</span> <span m="4040340">of</span> <span m="4040400">sequential</span>
  <span m="4040700">data.</span> <span m="4040940">Sequential</span> <span m="4041330">data</span>
  <span m="4041630">which,</span> <span m="4041870">by</span> <span m="4041990">the</span>
  <span m="4042050">way,</span> <span m="4042170">lives</span> <span m="4042380">in</span>
  <span m="4042440">many</span> <span m="4042590">different</span> <span m="4042800">time</span>
  <span m="4043160">scales.</span> <span m="4043850">Patients</span> <span m="4044330">who</span>
  <span m="4044630">are</span> <span m="4044960">hospitalized,</span> <span m="4045730">you</span>
  <span m="4045800">get</span> <span m="4045890">tons</span> <span m="4046130">of</span>
  <span m="4046190">data</span> <span m="4046370">for</span> <span m="4046490">them</span>
  <span m="4046580">at</span> <span m="4046640">a</span> <span m="4046730">time,</span>
  <span m="4047090">and</span> <span m="4047180">then</span> <span m="4047750">you</span>
  <span m="4047870">might</span> <span m="4048020">go</span> <span m="4048200">months</span>
  <span m="4048560">without</span> <span m="4048770">any</span> <span m="4048950">data</span>
  <span m="4049130">on</span> <span m="4049220">them.</span> <span m="4049790">Data</span>
  <span m="4050000">with</span> <span m="4050120">lots</span> <span m="4050330">of</span>
  <span m="4050420">missing</span> <span m="4050810">data.</span> <span m="4051440">Data</span>
  <span m="4051680">with</span> <span m="4052010">multivariate</span> <span m="4052610">observations</span>
  <span m="4053200">at</span> <span m="4053270">each</span> <span m="4053390">point</span>
  <span m="4053540">in</span> <span m="4053630">time,</span> <span m="4053960">not</span>
  <span m="4054170">just</span> <span m="4054440">a</span> <span m="4054500">single</span>
  <span m="4054920">word</span> <span m="4055310">at</span> <span m="4055430">that</span>
  <span m="4055550">point</span> <span m="4055730">in</span> <span m="4055820">time.</span></p><p><span
  m="4056150">All</span> <span m="4056510">right,</span> <span m="4056650">so</span>
  <span m="4056750">it's</span> <span m="4056870">a</span> <span m="4056930">different</span>
  <span m="4057260">setting.</span> <span m="4057800">And</span> <span m="4057980">we</span>
  <span m="4058130">shouldn't</span> <span m="4058310">expect</span> <span m="4058760">that</span>
  <span m="4059420">the</span> <span m="4059510">same</span> <span m="4059900">architectures</span>
  <span m="4060275">that</span> <span m="4060650">have</span> <span m="4060740">been</span>
  <span m="4060860">developed</span> <span m="4061310">for</span> <span m="4061550">other</span>
  <span m="4061760">problems</span> <span m="4062150">will</span> <span m="4062240">generalize</span>
  <span m="4062660">immediately</span> <span m="4063170">to</span> <span m="4063260">these</span>
  <span m="4063470">problems.</span></p><p><span m="4064910">Now,</span> <span m="4065060">I</span>
  <span m="4065150">do</span> <span m="4065390">conjecture</span> <span m="4065990">that</span>
  <span m="4066170">there</span> <span m="4066350">are</span> <span m="4066710">lots</span>
  <span m="4067130">of</span> <span m="4067250">nonlinear</span> <span m="4067790">attractions</span>
  <span m="4069080">where</span> <span m="4070250">deep</span> <span m="4070550">neural</span>
  <span m="4070750">networks</span> <span m="4071120">could</span> <span m="4071330">be</span>
  <span m="4071450">very</span> <span m="4071960">powerful</span> <span m="4072215">at</span>
  <span m="4072470">predicting</span> <span m="4072840">for.</span> <span m="4073220">But</span>
  <span m="4073370">I</span> <span m="4073430">think</span> <span m="4073610">they're</span>
  <span m="4073760">subtle.</span> <span m="4075020">And</span> <span m="4075530">I</span>
  <span m="4075650">don't</span> <span m="4076040">think</span> <span m="4076280">that</span>
  <span m="4076400">we</span> <span m="4076520">have</span> <span m="4076760">enough</span>
  <span m="4077000">data</span> <span m="4077360">currently</span> <span m="4078380">to</span>
  <span m="4078710">deal</span> <span m="4079190">with</span> <span m="4079730">the</span>
  <span m="4079820">fact</span> <span m="4080300">that</span> <span m="4081770">the</span>
  <span m="4081890">data</span> <span m="4082130">is</span> <span m="4082310">messy</span>
  <span m="4083270">and</span> <span m="4083440">that</span> <span m="4083900">the</span>
  <span m="4084110">non-linear</span> <span m="4084530">interactions</span> <span
  m="4084980">are</span> <span m="4085070">subtle.</span> <span m="4085940">We</span>
  <span m="4086030">just</span> <span m="4086180">can't</span> <span m="4086420">find</span>
  <span m="4086690">them</span> <span m="4086780">right</span> <span m="4086960">now.</span>
  <span m="4087470">But</span> <span m="4087650">this</span> <span m="4087800">shouldn't</span>
  <span m="4088220">mean</span> <span m="4088490">that</span> <span m="4088670">we're</span>
  <span m="4088790">not</span> <span m="4088970">going</span> <span m="4089090">to</span>
  <span m="4089150">find</span> <span m="4089420">them</span> <span m="4089690">a</span>
  <span m="4089750">few</span> <span m="4089960">years</span> <span m="4090200">from</span>
  <span m="4090320">now.</span> <span m="4090400">I</span> <span m="4090440">think</span>
  <span m="4090700">this</span> <span m="4091460">deservedly</span> <span m="4092120">is</span>
  <span m="4092360">a</span> <span m="4092420">very</span> <span m="4092810">interesting</span>
  <span m="4093170">research</span> <span m="4093590">direction</span> <span m="4093950">to</span>
  <span m="4094040">work</span> <span m="4094250">on.</span></p><p><span m="4095200">And</span>
  <span m="4095300">a</span> <span m="4095360">final</span> <span m="4095690">reason</span>
  <span m="4095930">to</span> <span m="4096020">point</span> <span m="4096290">out</span>
  <span m="4096439">is</span> <span m="4096560">that</span> <span m="4097010">the</span>
  <span m="4097130">features</span> <span m="4097760">that</span> <span m="4097850">are</span>
  <span m="4097939">going</span> <span m="4098140">into</span> <span m="4098270">these</span>
  <span m="4098450">types</span> <span m="4098660">of</span> <span m="4098720">models</span>
  <span m="4099290">are</span> <span m="4099380">actually</span> <span m="4099649">really</span>
  <span m="4100100">cleverly-chosen</span> <span m="4101120">features.</span> <span
  m="4102939">A</span> <span m="4103020">laboratory</span> <span m="4103609">test</span>
  <span m="4103819">result,</span> <span m="4104859">like</span> <span m="4105050">looking</span>
  <span m="4105410">at</span> <span m="4105500">your</span> <span m="4105680">A1C--</span>
  <span m="4106609">what</span> <span m="4106850">is</span> <span m="4107090">A1C?</span>
  <span m="4108200">So</span> <span m="4108490">it's</span> <span m="4110210">something</span>
  <span m="4110510">that</span> <span m="4110630">had</span> <span m="4110720">been</span>
  <span m="4110870">developed</span> <span m="4111470">over</span> <span m="4111680">decades</span>
  <span m="4112430">and</span> <span m="4112520">decades</span> <span m="4112939">of</span>
  <span m="4113000">research,</span> <span m="4113450">where</span> <span m="4113569">you</span>
  <span m="4113660">recognize</span> <span m="4114109">that</span> <span m="4114200">looking</span>
  <span m="4114439">at</span> <span m="4114500">a</span> <span m="4114560">particular</span>
  <span m="4114979">protein</span> <span m="4115550">is</span> <span m="4115670">actually</span>
  <span m="4115910">informative</span> <span m="4116479">as</span> <span m="4116529">something</span>
  <span m="4116740">about</span> <span m="4116880">a</span> <span m="4116990">patient's</span>
  <span m="4117260">health.</span></p><p><span m="4118550">So</span> <span m="4118790">the</span>
  <span m="4118880">features</span> <span m="4119510">that</span> <span m="4119630">we're</span>
  <span m="4119779">using</span> <span m="4120180">that</span> <span m="4120260">go</span>
  <span m="4120470">into</span> <span m="4120649">these</span> <span m="4120830">models</span>
  <span m="4121189">were</span> <span m="4121310">designed--</span> <span m="4122660">first,</span>
  <span m="4122960">they</span> <span m="4123050">were</span> <span m="4123109">designed</span>
  <span m="4123380">for</span> <span m="4123500">humans</span> <span m="4123800">to</span>
  <span m="4123920">look</span> <span m="4124100">at.</span> <span m="4125120">And</span>
  <span m="4125210">second,</span> <span m="4125450">they</span> <span m="4125510">were</span>
  <span m="4125569">designed</span> <span m="4125960">to</span> <span m="4126050">really</span>
  <span m="4126290">help</span> <span m="4126590">you</span> <span m="4126740">with</span>
  <span m="4126950">decision-making,</span> <span m="4127750">or</span> <span m="4127810">largely</span>
  <span m="4128180">independent</span> <span m="4128870">features</span> <span m="4129350">from</span>
  <span m="4129529">other</span> <span m="4129740">information</span> <span m="4130189">that</span>
  <span m="4130279">you</span> <span m="4130340">have</span> <span m="4130460">about</span>
  <span m="4130620">a</span> <span m="4130700">patient.</span> <span m="4131540">And</span>
  <span m="4131660">all</span> <span m="4131840">of</span> <span m="4131930">those</span>
  <span m="4132109">are</span> <span m="4132319">reasons,</span> <span m="4132830">really,</span>
  <span m="4133069">I</span> <span m="4133130">think</span> <span m="4133310">why</span>
  <span m="4133490">we're</span> <span m="4133609">observing</span> <span m="4134359">these</span>
  <span m="4134750">subtleties.</span></p><p><span m="4136160">OK,</span> <span m="4136319">so</span>
  <span m="4136430">for the</span> <span m="4136560">last</span> <span m="4136819">10</span>
  <span m="4137090">minutes</span> <span m="4137390">of</span> <span m="4137609">class--</span>
  <span m="4138729">I'm</span> <span m="4138930">going to</span> <span m="4139069">have</span>
  <span m="4139189">to</span> <span m="4139279">hold</span> <span m="4139510">questions,</span>
  <span m="4139850">because I</span> <span m="4139880">want</span> <span m="4140000">to</span>
  <span m="4140060">get</span> <span m="4140210">through</span> <span m="4140330">all</span>
  <span m="4140420">the</span> <span m="4140479">material.</span> <span m="4141510">But</span>
  <span m="4141859">please</span> <span m="4142100">post</span> <span m="4142279">them</span>
  <span m="4142370">to</span> <span m="4142439">Piazza.</span> <span m="4143145">For</span>
  <span m="4143540">the</span> <span m="4143790">last</span> <span m="4143990">10</span>
  <span m="4144109">minutes</span> <span m="4144290">of</span> <span m="4144350">class,</span>
  <span m="4144750">I</span> <span m="4144850">want</span> <span m="4144950">to</span>
  <span m="4145250">change</span> <span m="4145550">gears</span> <span m="4146450">a</span>
  <span m="4146510">little</span> <span m="4146630">bit,</span> <span m="4146720">and</span>
  <span m="4146810">talk</span> <span m="4146990">about</span> <span m="4147140">survival</span>
  <span m="4147660">modeling.</span></p><p><span m="4150350">So</span> <span m="4152810">often</span>
  <span m="4153109">we want</span> <span m="4153170">want</span> <span m="4153319">to</span>
  <span m="4153380">talk</span> <span m="4153500">about</span> <span m="4153620">predicting</span>
  <span m="4154100">time</span> <span m="4154490">to</span> <span m="4154640">some</span>
  <span m="4155090">event.</span> <span m="4156600">So</span> <span m="4156680">this</span>
  <span m="4156859">red</span> <span m="4157609">dot</span> <span m="4157939">here--</span>
  <span m="4158800">sorry,</span> <span m="4159109">this</span> <span m="4159260">black</span>
  <span m="4159770">line</span> <span m="4160130">here</span> <span m="4161300">is</span>
  <span m="4161479">what</span> <span m="4161630">I</span> <span m="4161689">mean</span>
  <span m="4161870">by</span> <span m="4162050">an</span> <span m="4162140">event.</span>
  <span m="4163740">That</span> <span m="4163819">event</span> <span m="4164149">might</span>
  <span m="4164359">be,</span> <span m="4164580">for</span> <span m="4164680">example,</span>
  <span m="4165600">a</span> <span m="4165700">patient</span> <span m="4165859">dying.</span>
  <span m="4166299">It</span> <span m="4166740">might</span> <span m="4166970">mean</span>
  <span m="4168170">a</span> <span m="4168229">married</span> <span m="4168500">couple</span>
  <span m="4168770">getting</span> <span m="4168979">divorced.</span> <span m="4169970">It</span>
  <span m="4170029">might</span> <span m="4170270">mean</span> <span m="4171080">the</span>
  <span m="4171260">day</span> <span m="4171520">that</span> <span m="4171680">what</span>
  <span m="4171870">you</span> <span m="4172010">graduate</span> <span m="4172460">from</span>
  <span m="4173270">MIT.</span> <span m="4175649">And</span> <span m="4176180">the</span>
  <span m="4176300">red</span> <span m="4176540">dot</span> <span m="4176930">here</span>
  <span m="4177710">denotes</span> <span m="4178100">censored</span> <span m="4178729">events.</span>
  <span m="4179330">So</span> <span m="4179660">for</span> <span m="4179870">whatever</span>
  <span m="4180319">reason,</span> <span m="4182270">we</span> <span m="4182450">don't</span>
  <span m="4182720">have</span> <span m="4182960">data</span> <span m="4183229">on</span>
  <span m="4183350">this</span> <span m="4183529">patient,</span> <span m="4184010">patient</span>
  <span m="4184370">S3,</span> <span m="4185240">after</span> <span m="4185569">time</span>
  <span m="4185810">step</span> <span m="4186069">4.</span> <span m="4187340">They</span>
  <span m="4187460">were</span> <span m="4187550">censored.</span></p><p><span m="4187920">So</span>
  <span m="4188569">we</span> <span m="4188720">do</span> <span m="4188960">know</span>
  <span m="4189770">that</span> <span m="4190490">the</span> <span m="4190580">event</span>
  <span m="4190910">didn't</span> <span m="4191270">occur</span> <span m="4191600">prior</span>
  <span m="4192260">to</span> <span m="4192410">time</span> <span m="4192859">step
  4.</span> <span m="4193670">But</span> <span m="4193850">we</span> <span m="4193970">don't</span>
  <span m="4194330">know</span> <span m="4194720">if</span> <span m="4194930">and</span>
  <span m="4195050">when</span> <span m="4195560">it's</span> <span m="4195740">going</span>
  <span m="4195950">to</span> <span m="4196040">occur</span> <span m="4196460">after</span>
  <span m="4196820">time</span> <span m="4197030">step</span> <span m="4197210">4,</span>
  <span m="4197510">because</span> <span m="4198470">we</span> <span m="4198590">have</span>
  <span m="4198740">missing</span> <span m="4199100">data</span> <span m="4199340">there.</span>
  <span m="4200015">OK,</span> <span m="4200420">so</span> <span m="4200510">this</span>
  <span m="4200660">is</span> <span m="4200750">what</span> <span m="4200870">I</span>
  <span m="4200930">mean</span> <span m="4201080">by</span> <span m="4201260">right-censored</span>
  <span m="4202280">data.</span></p><p><span m="4204170">So</span> <span m="4204620">you</span>
  <span m="4204770">might</span> <span m="4204950">ask,</span> <span m="4206120">why</span>
  <span m="4206330">not</span> <span m="4206510">just</span> <span m="4206720">use</span>
  <span m="4207050">classification--</span> <span m="4207980">like</span> <span m="4208160">binary</span>
  <span m="4208490">classification--</span> <span m="4209630">in</span> <span m="4209810">this</span>
  <span m="4209920">setting?</span> <span m="4211040">And</span> <span m="4211160">that's</span>
  <span m="4211310">exactly</span> <span m="4211610">what</span> <span m="4211700">we</span>
  <span m="4211760">did</span> <span m="4211880">earlier.</span> <span m="4212230">We</span>
  <span m="4212870">thought</span> <span m="4213290">about</span> <span m="4213890">formalizing</span>
  <span m="4215120">the</span> <span m="4215240">diabetes</span> <span m="4215840">risk</span>
  <span m="4216060">stratification</span> <span m="4216470">problem</span> <span m="4216860">as</span>
  <span m="4217130">looking</span> <span m="4217490">to</span> <span m="4217610">see</span>
  <span m="4217910">what</span> <span m="4218120">happens</span> <span m="4218750">years</span>
  <span m="4219130">1</span> <span m="4219500">to</span> <span m="4219680">3</span>
  <span m="4220400">after</span> <span m="4220940">the</span> <span m="4221060">time</span>
  <span m="4221300">of</span> <span m="4221360">prediction.</span> <span m="4222690">That</span>
  <span m="4222800">was</span> <span m="4222890">with</span> <span m="4223010">a</span>
  <span m="4223040">gap</span> <span m="4223370">of</span> <span m="4223490">one</span>
  <span m="4223820">year.</span></p><p><span m="4226180">And</span> <span m="4226390">there</span>
  <span m="4226510">a</span> <span m="4226550">couple</span> <span m="4226880">of</span>
  <span m="4226940">reasons</span> <span m="4227270">why</span> <span m="4227450">that's</span>
  <span m="4228170">perhaps</span> <span m="4228620">not</span> <span m="4228890">what</span>
  <span m="4229040">you</span> <span m="4229160">really</span> <span m="4229520">wanted</span>
  <span m="4229760">to</span> <span m="4229880">do.</span> <span m="4230720">First,</span>
  <span m="4231470">you</span> <span m="4231590">have</span> <span m="4231770">less</span>
  <span m="4232130">data</span> <span m="4233390">to</span> <span m="4233570">use</span>
  <span m="4233810">during</span> <span m="4234050">training.</span> <span m="4235490">Because</span>
  <span m="4236210">you've</span> <span m="4236390">suddenly</span> <span m="4236750">excluded</span>
  <span m="4237530">patients</span> <span m="4238670">for</span> <span m="4238940">whom--</span>
  <span m="4240920">or</span> <span m="4241540">to</span> <span m="4241700">differently--</span>
  <span m="4244370">if</span> <span m="4246950">you</span> <span m="4247070">have</span>
  <span m="4247400">patients</span> <span m="4248300">for</span> <span m="4248510">whom</span>
  <span m="4249080">they</span> <span m="4249260">were</span> <span m="4249440">censored</span>
  <span m="4250280">during</span> <span m="4250730">that</span> <span m="4250850">time</span>
  <span m="4251150">window,</span> <span m="4251570">you're</span> <span m="4251780">throwing</span>
  <span m="4252110">them</span> <span m="4252260">out.</span> <span m="4252570">So</span>
  <span m="4252620">you</span> <span m="4252710">have</span> <span m="4252860">fewer</span>
  <span m="4253190">data</span> <span m="4253400">points</span> <span m="4253700">there.</span>
  <span m="4254350">That</span> <span m="4254510">was</span> <span m="4254600">part</span>
  <span m="4254810">of</span> <span m="4254900">our</span> <span m="4255320">inclusion/exclusion</span>
  <span m="4256190">criteria.</span></p><p><span m="4258160">Also,</span> <span m="4259970">when</span>
  <span m="4260150">you</span> <span m="4260240">go</span> <span m="4260420">to</span>
  <span m="4260510">deploy</span> <span m="4260840">these</span> <span m="4260990">models,</span>
  <span m="4261740">your</span> <span m="4261860">model</span> <span m="4262130">might</span>
  <span m="4262310">say,</span> <span m="4263030">yes,</span> <span m="4263610">this</span>
  <span m="4263660">patient</span> <span m="4263960">is</span> <span m="4264200">going</span>
  <span m="4264320">to</span> <span m="4264380">develop</span> <span m="4265050">type</span>
  <span m="4265250">2</span> <span m="4265340">diabetes</span> <span m="4265700">between</span>
  <span m="4266000">one</span> <span m="4266180">and</span> <span m="4266270">three</span>
  <span m="4266450">years</span> <span m="4266660">from</span> <span m="4266780">now.</span>
  <span m="4267990">But</span> <span m="4268070">in</span> <span m="4268160">fact</span>
  <span m="4268460">what</span> <span m="4268610">happened</span> <span m="4268970">is</span>
  <span m="4269090">they</span> <span m="4269180">develop</span> <span m="4269450">type</span>
  <span m="4269660">2</span> <span m="4269720">diabetes</span> <span m="4270470">3.1</span>
  <span m="4271310">years</span> <span m="4271580">from</span> <span m="4271700">now.</span>
  <span m="4273240">So</span> <span m="4273500">your</span> <span m="4273710">model</span>
  <span m="4273980">would</span> <span m="4274070">count</span> <span m="4274340">this</span>
  <span m="4274520">as</span> <span m="4274670">a</span> <span m="4274730">negative.</span>
  <span m="4275750">Or</span> <span m="4276035">it</span> <span m="4276320">would</span>
  <span m="4276630">be</span> <span m="4276940">a</span> <span m="4277220">false</span>
  <span m="4277640">positive.</span> <span m="4279390">The</span> <span m="4279620">prediction</span>
  <span m="4279950">would</span> <span m="4280040">be</span> <span m="4280100">a</span>
  <span m="4280130">false</span> <span m="4280340">positive.</span> <span m="4281360">But</span>
  <span m="4281510">in</span> <span m="4281570">reality,</span> <span m="4282070">your</span>
  <span m="4282170">model</span> <span m="4282320">wasn't</span> <span m="4282620">actually</span>
  <span m="4282890">that</span> <span m="4283070">bad.</span> <span m="4283420">We</span>
  <span m="4283520">did</span> <span m="4283700">pretty</span> <span m="4284030">well.</span>
  <span m="4284450">We</span> <span m="4284570">didn't</span> <span m="4284930">quite</span>
  <span m="4285320">get</span> <span m="4285470">the</span> <span m="4285560">right</span>
  <span m="4285740">range,</span> <span m="4286130">but</span> <span m="4286250">they</span>
  <span m="4286370">did</span> <span m="4286640">get</span> <span m="4286940">diagnosed</span>
  <span m="4287330">diabetes</span> <span m="4288020">right</span> <span m="4288410">outside</span>
  <span m="4288680">that</span> <span m="4288800">time</span> <span m="4288980">window.</span></p><p><span
  m="4290170">And</span> <span m="4290330">so</span> <span m="4290690">your</span>
  <span m="4290960">measures</span> <span m="4291410">of</span> <span m="4291470">performance</span>
  <span m="4291950">are</span> <span m="4292040">going</span> <span m="4292160">to</span>
  <span m="4292220">be</span> <span m="4292340">pessimistic.</span> <span m="4294020">You</span>
  <span m="4294140">might</span> <span m="4294290">be</span> <span m="4294380">doing</span>
  <span m="4294740">better</span> <span m="4295100">than</span> <span m="4295250">you</span>
  <span m="4295340">thought.</span> <span m="4296660">Now,</span> <span m="4296870">you</span>
  <span m="4296960">can</span> <span m="4297110">try</span> <span m="4297290">to</span>
  <span m="4297410">address</span> <span m="4297830">these</span> <span m="4298010">two</span>
  <span m="4298160">challenges</span> <span m="4298580">in</span> <span m="4298640">many</span>
  <span m="4298820">ways.</span> <span m="4299180">You</span> <span m="4299270">can</span>
  <span m="4299390">imagine</span> <span m="4299720">a</span> <span m="4299780">multi-task</span>
  <span m="4300530">learning</span> <span m="4300860">framework</span> <span m="4301220">where
  you</span> <span m="4301340">try</span> <span m="4301490">to</span> <span m="4301580">predict</span>
  <span m="4302450">what's</span> <span m="4302660">going</span> <span m="4302780">to</span>
  <span m="4302840">happen</span> <span m="4303560">one</span> <span m="4303800">to</span>
  <span m="4303920">two</span> <span m="4304100">years</span> <span m="4304370">from</span>
  <span m="4304490">now,</span> <span m="4304650">what's</span> <span m="4304760">going
  to</span> <span m="4304870">happen</span> <span m="4305090">two</span> <span m="4305240">to</span>
  <span m="4305360">three</span> <span m="4305600">years</span> <span m="4305810">from</span>
  <span m="4305930">now,</span> <span m="4306150">three</span> <span m="4306290">to</span>
  <span m="4306380">four,</span> <span m="4306740">and</span> <span m="4306860">so</span>
  <span m="4307070">on.</span> <span m="4307320">Each</span> <span m="4307370">of</span>
  <span m="4307430">those</span> <span m="4307610">are</span> <span m="4307670">different</span>
  <span m="4308060">binary</span> <span m="4308450">classification</span> <span m="4308960">models.</span>
  <span m="4309680">You</span> <span m="4309770">might</span> <span m="4309920">try</span>
  <span m="4310100">to</span> <span m="4310220">tie</span> <span m="4310640">together</span>
  <span m="4311060">the</span> <span m="4311150">parameters</span> <span m="4311640">of</span>
  <span m="4311690">those</span> <span m="4311870">models</span> <span m="4312230">via
  a</span> <span m="4312330">multi-task</span> <span m="4312980">learning</span> <span
  m="4313280">formulation.</span> <span m="4314860">And</span> <span m="4315220">that</span>
  <span m="4315570">will</span> <span m="4315740">get</span> <span m="4315860">you</span>
  <span m="4315980">closer</span> <span m="4316320">to</span> <span m="4316370">what</span>
  <span m="4316490">you</span> <span m="4316610">care</span> <span m="4316820">about.</span></p><p><span
  m="4317480">But</span> <span m="4317660">what</span> <span m="4317780">I'll</span>
  <span m="4317870">tell</span> <span m="4318050">you</span> <span m="4318110">about</span>
  <span m="4318290">in</span> <span m="4318340">the</span> <span m="4318400">last</span>
  <span m="4318650">five</span> <span m="4318890">minutes</span> <span m="4319250">is</span>
  <span m="4319400">a</span> <span m="4319430">much</span> <span m="4319610">more</span>
  <span m="4319760">elegant</span> <span m="4320300">approach</span> <span m="4320660">to</span>
  <span m="4320750">trying</span> <span m="4320960">to</span> <span m="4321860">deal</span>
  <span m="4322010">with</span> <span m="4322130">that.</span> <span m="4322910">And</span>
  <span m="4323030">it's</span> <span m="4323180">akin</span> <span m="4323540">to</span>
  <span m="4323750">regression.</span> <span m="4324620">So</span> <span m="4325010">that</span>
  <span m="4325160">leads to</span> <span m="4325350">my</span> <span m="4325490">second</span>
  <span m="4325790">point--</span> <span m="4326730">why</span> <span m="4327020">not</span>
  <span m="4327170">just</span> <span m="4327380">treat</span> <span m="4327560">this</span>
  <span m="4327680">as</span> <span m="4327770">a</span> <span m="4327800">regression</span>
  <span m="4328250">problem?</span> <span m="4328970">Predict</span> <span m="4329630">time</span>
  <span m="4330200">to</span> <span m="4330360">event.</span> <span m="4330800">You</span>
  <span m="4330890">have</span> <span m="4331010">some</span> <span m="4331130">continuous</span>
  <span m="4331790">valued</span> <span m="4332210">outcome,</span> <span m="4333170">the</span>
  <span m="4333290">time</span> <span m="4333830">until</span> <span m="4334460">diagnosis</span>
  <span m="4334970">diabetes.</span> <span m="4335960">Just</span> <span m="4336140">try</span>
  <span m="4336320">to</span> <span m="4337310">minimize</span> <span m="4338300">mean</span>
  <span m="4338750">squared--</span> <span m="4339260">minimize</span> <span m="4339680">your</span>
  <span m="4339770">squared</span> <span m="4340100">error</span> <span m="4340730">trying</span>
  <span m="4340910">to</span> <span m="4341000">predict</span> <span m="4341250">that</span>
  <span m="4341570">continuous</span> <span m="4341990">value.</span></p><p><span
  m="4343610">Well,</span> <span m="4343850">the</span> <span m="4343940">first</span>
  <span m="4344930">challenge</span> <span m="4345410">to</span> <span m="4345470">think</span>
  <span m="4345650">about</span> <span m="4346190">is,</span> <span m="4346610">remember</span>
  <span m="4347030">where</span> <span m="4347150">that</span> <span m="4347300">mean</span>
  <span m="4347570">squared</span> <span m="4347750">error</span> <span m="4347880">loss</span>
  <span m="4348170">function</span> <span m="4348470">came</span> <span m="4348680">from.</span>
  <span m="4348890">It</span> <span m="4348980">came</span> <span m="4349280">from</span>
  <span m="4350270">thinking</span> <span m="4350750">about</span> <span m="4352240">your</span>
  <span m="4352970">data</span> <span m="4353630">as</span> <span m="4353900">coming</span>
  <span m="4354200">from</span> <span m="4354410">a</span> <span m="4354470">Gaussian</span>
  <span m="4354950">distribution.</span> <span m="4356330">And</span> <span m="4356360">if</span>
  <span m="4356420">you</span> <span m="4356660">do</span> <span m="4356840">maximum</span>
  <span m="4357160">likelihood</span> <span m="4357470">estimation</span> <span m="4357920">of</span>
  <span m="4358000">this</span> <span m="4358100">Gaussian</span> <span m="4358430">distribution,</span>
  <span m="4359190">it</span> <span m="4359290">turns</span> <span m="4359480">out</span>
  <span m="4359810">to</span> <span m="4360470">look</span> <span m="4360800">like</span>
  <span m="4361340">minimizing</span> <span m="4361940">a</span> <span m="4362150">squared</span>
  <span m="4362510">loss.</span></p><p><span m="4364250">So</span> <span m="4364520">it's</span>
  <span m="4364700">making</span> <span m="4365000">a</span> <span m="4365030">lot</span>
  <span m="4365150">of</span> <span m="4365210">assumptions</span> <span m="4365720">about</span>
  <span m="4365900">the</span> <span m="4365960">outcome.</span> <span m="4366350">For</span>
  <span m="4366500">one,</span> <span m="4366710">it's</span> <span m="4366830">making
  the</span> <span m="4367100">assumption</span> <span m="4367490">that</span> <span
  m="4367640">outcome</span> <span m="4368060">could</span> <span m="4368270">be</span>
  <span m="4368360">negative</span> <span m="4368750">or</span> <span m="4368810">positive.</span>
  <span m="4369190">A</span> <span m="4369230">Gaussian</span> <span m="4369560">distribution</span>
  <span m="4370310">doesn't</span> <span m="4370580">have</span> <span m="4370760">to</span>
  <span m="4370880">be</span> <span m="4371060">positive.</span> <span m="4371960">But</span>
  <span m="4372110">here</span> <span m="4372380">we</span> <span m="4372470">know</span>
  <span m="4372590">that</span> <span m="4372680">T</span> <span m="4372890">is</span>
  <span m="4373010">always</span> <span m="4373220">non-negative.</span> <span m="4374540">In</span>
  <span m="4374630">addition,</span> <span m="4375680">there</span> <span m="4375770">might</span>
  <span m="4375890">be</span> <span m="4375980">long</span> <span m="4376220">tails.</span>
  <span m="4376850">We</span> <span m="4376940">might</span> <span m="4377120">not</span>
  <span m="4377300">know</span> <span m="4377420">exactly</span> <span m="4377810">when
  the</span> <span m="4377930">patient's</span> <span m="4378260">going to</span>
  <span m="4378380">develop</span> <span m="4378620">diabetes,</span> <span m="4379010">but</span>
  <span m="4379100">we</span> <span m="4379190">know</span> <span m="4379340">it's</span>
  <span m="4379430">not</span> <span m="4379600">going</span> <span m="4379660">to</span>
  <span m="4379730">be</span> <span m="4379820">now.</span> <span m="4380110">It's
  going to be at</span> <span m="4380360">some</span> <span m="4380540">point</span>
  <span m="4380720">in</span> <span m="4380780">the</span> <span m="4380900">far</span>
  <span m="4381620">future.</span> <span m="4382640">And</span> <span m="4382790">that</span>
  <span m="4382970">may</span> <span m="4383120">also</span> <span m="4383330">look</span>
  <span m="4383480">very</span> <span m="4383660">non-Gaussian.</span> <span m="4384480">So</span>
  <span m="4384590">typical</span> <span m="4385360">regression</span> <span m="4385700">approaches</span>
  <span m="4386060">aren't</span> <span m="4386270">quite</span> <span m="4386480">what</span>
  <span m="4386600">you</span> <span m="4386660">want.</span></p><p><span m="4387290">But</span>
  <span m="4387440">there's</span> <span m="4387590">another</span> <span m="4388160">really</span>
  <span m="4388520">important</span> <span m="4388850">problem,</span> <span m="4389600">which
  is</span> <span m="4389750">that</span> <span m="4389870">if</span> <span m="4389960">you</span>
  <span m="4390050">naively</span> <span m="4390620">remove</span> <span m="4391100">those</span>
  <span m="4391280">censored</span> <span m="4391790">points--</span> <span m="4392220">like,</span>
  <span m="4392390">what</span> <span m="4392510">do</span> <span m="4392570">you</span>
  <span m="4392630">do</span> <span m="4392840">for</span> <span m="4393000">the</span>
  <span m="4393040">individuals</span> <span m="4393410">where</span> <span m="4393530">you</span>
  <span m="4393620">never</span> <span m="4394010">observe</span> <span m="4394520">the</span>
  <span m="4394610">time--</span> <span m="4395540">where</span> <span m="4395600">the</span>
  <span m="4395870">never</span> <span m="4396170">get</span> <span m="4396350">diabetes,</span>
  <span m="4396800">because</span> <span m="4397010">they</span> <span m="4397100">were</span>
  <span m="4397190">censored?</span> <span m="4398240">Well,</span> <span m="4398330">if</span>
  <span m="4398390">you</span> <span m="4398450">just</span> <span m="4398600">remove</span>
  <span m="4399050">those</span> <span m="4399290">from</span> <span m="4399440">your</span>
  <span m="4399530">learning</span> <span m="4399860">algorithm,</span> <span m="4400880">then</span>
  <span m="4401060">you're</span> <span m="4401180">biasing</span> <span m="4401870">your</span>
  <span m="4401960">results.</span></p><p><span m="4403560">So</span> <span m="4403640">for</span>
  <span m="4403760">example,</span> <span m="4405350">if</span> <span m="4405470">you</span>
  <span m="4405590">think</span> <span m="4405830">about</span> <span m="4406070">the</span>
  <span m="4406250">average</span> <span m="4407000">age</span> <span m="4407390">of</span>
  <span m="4407480">diabetes</span> <span m="4407990">onset,</span> <span m="4408680">if</span>
  <span m="4408830">you</span> <span m="4408920">only</span> <span m="4409250">look</span>
  <span m="4409490">at</span> <span m="4409580">people</span> <span m="4409820">who</span>
  <span m="4409970">actually</span> <span m="4410690">were</span> <span m="4410840">observed</span>
  <span m="4411200">to</span> <span m="4411290">get</span> <span m="4411440">diabetes,</span>
  <span m="4411980">it's</span> <span m="4412070">going</span> <span m="4412310">to</span>
  <span m="4412400">be</span> <span m="4412520">much</span> <span m="4413000">closer</span>
  <span m="4413510">to</span> <span m="4413660">now.</span> <span m="4414620">Because</span>
  <span m="4414890">obviously</span> <span m="4415280">the</span> <span m="4415400">people</span>
  <span m="4415700">who</span> <span m="4415820">were</span> <span m="4415940">censored</span>
  <span m="4416210">are</span> <span m="4416480">people</span> <span m="4416660">who</span>
  <span m="4416750">got</span> <span m="4416930">it</span> <span m="4416990">much</span>
  <span m="4417170">later</span> <span m="4417770">from</span> <span m="4417920">the</span>
  <span m="4417980">censoring</span> <span m="4418400">time.</span> <span m="4419920">So</span>
  <span m="4420020">that's</span> <span m="4420230">another</span> <span m="4420530">serious</span>
  <span m="4420950">problem.</span></p><p><span m="4422040">So</span> <span m="4422090">the</span>
  <span m="4422180">way</span> <span m="4422270">they</span> <span m="4422360">we're</span>
  <span m="4422420">trying</span> <span m="4422570">to</span> <span m="4422660">formalize</span>
  <span m="4423050">this</span> <span m="4423170">mathematically</span> <span m="4424490">is</span>
  <span m="4424640">as</span> <span m="4424760">follows.</span> <span m="4425340">Now</span>
  <span m="4425450">we</span> <span m="4425540">should</span> <span m="4425660">think</span>
  <span m="4425840">about</span> <span m="4426020">having</span> <span m="4426290">data</span>
  <span m="4427010">which</span> <span m="4427250">has,</span> <span m="4427800">again,</span>
  <span m="4427970">features</span> <span m="4428570">x,</span> <span m="4429800">outcome--</span>
  <span m="4431270">what</span> <span m="4431510">we</span> <span m="4431600">usually</span>
  <span m="4431840">call</span> <span m="4432080">Y</span> <span m="4432500">for</span>
  <span m="4432650">the</span> <span m="4432710">outcome</span> <span m="4433100">in</span>
  <span m="4433190">regression,</span> <span m="4433610">but</span> <span m="4433700">here</span>
  <span m="4433880">I'll</span> <span m="4433940">call</span> <span m="4434090">it</span>
  <span m="4434180">capital</span> <span m="4434570">T,</span> <span m="4434870">because</span>
  <span m="4435080">of</span> <span m="4435140">the</span> <span m="4435230">time</span>
  <span m="4435590">to</span> <span m="4435710">the</span> <span m="4435800">event.</span>
  <span m="4436850">And</span> <span m="4437120">now</span> <span m="4437420">we</span>
  <span m="4437510">have</span> <span m="4437630">an</span> <span m="4437690">additional</span>
  <span m="4438650">variable--</span> <span m="4439100">so it's</span> <span m="4439240">no</span>
  <span m="4439350">longer</span> <span m="4439580">a two-point,</span> <span m="4440840">now</span>
  <span m="4441020">it's a</span> <span m="4441230">triple--</span> <span m="4442220">b.</span>
  <span m="4442940">And</span> <span m="4443090">b</span> <span m="4443330">is</span>
  <span m="4443450">going</span> <span m="4443530">to</span> <span m="4443630">be</span>
  <span m="4443710">a</span> <span m="4443780">binary</span> <span m="4444200">variable,</span>
  <span m="4444660">which</span> <span m="4444710">is</span> <span m="4444750">saying,</span>
  <span m="4445610">was</span> <span m="4446000">this</span> <span m="4446090">individual</span>
  <span m="4446480">censored--</span> <span m="4447170">was</span> <span m="4447440">the</span>
  <span m="4447560">time,</span> <span m="4447950">t,</span> <span m="4448260">denoting</span>
  <span m="4448760">a</span> <span m="4448820">censoring</span> <span m="4449420">event,</span>
  <span m="4449780">or</span> <span m="4449840">was</span> <span m="4449990">it</span>
  <span m="4450080">denoting</span> <span m="4450590">the</span> <span m="4450710">actual</span>
  <span m="4451190">event</span> <span m="4451550">happening?</span> <span m="4452380">So</span>
  <span m="4452720">it's</span> <span m="4452840">distinguishing</span> <span m="4453470">between</span>
  <span m="4454220">the</span> <span m="4454400">red</span> <span m="4455030">and</span>
  <span m="4455210">the</span> <span m="4455330">black.</span> <span m="4455930">So</span>
  <span m="4456470">black</span> <span m="4457460">is</span> <span m="4458210">b equals</span>
  <span m="4458780">0.</span> <span m="4459500">Red</span> <span m="4459950">is</span>
  <span m="4460250">b</span> <span m="4460580">equals</span> <span m="4460820">1.</span></p><p><span
  m="4461940">OK,</span> <span m="4462860">so</span> <span m="4463430">now</span>
  <span m="4463730">we</span> <span m="4463820">can</span> <span m="4463970">talk</span>
  <span m="4464210">about</span> <span m="4464480">learning</span> <span m="4464870">a</span>
  <span m="4464930">density,</span> <span m="4466950">P</span> <span m="4467300">of</span>
  <span m="4467450">t,</span> <span m="4467880">which</span> <span m="4467960">I'll</span>
  <span m="4468350">also</span> <span m="4468590">call</span> <span m="4468890">f</span>
  <span m="4469070">of</span> <span m="4469190">t,</span> <span m="4469920">which</span>
  <span m="4469970">is</span> <span m="4470030">the</span> <span m="4470120">probability</span>
  <span m="4470840">of</span> <span m="4470930">death</span> <span m="4471250">at</span>
  <span m="4471410">time</span> <span m="4471800">t.</span> <span m="4474020">And</span>
  <span m="4474920">associated</span> <span m="4475340">with</span> <span m="4475490">any</span>
  <span m="4475670">density,</span> <span m="4476280">of</span> <span m="4476380">course,</span>
  <span m="4476660">is</span> <span m="4477140">the</span> <span m="4477260">cumulative</span>
  <span m="4477860">density</span> <span m="4478190">function,</span> <span m="4478650">which</span>
  <span m="4478670">is</span> <span m="4478760">the</span> <span m="4478850">integral</span>
  <span m="4479930">from</span> <span m="4480320">0</span> <span m="4480910">to</span>
  <span m="4481050">any</span> <span m="4481340">point</span> <span m="4481910">of</span>
  <span m="4482060">the</span> <span m="4482150">density.</span> <span m="4483260">Here</span>
  <span m="4483560">we'll</span> <span m="4483680">actually</span> <span m="4483920">look</span>
  <span m="4484100">at</span> <span m="4484190">1</span> <span m="4484550">minus</span>
  <span m="4484910">the</span> <span m="4485000">CDF,</span> <span m="4485720">what's</span>
  <span m="4485960">called</span> <span m="4486170">the</span> <span m="4486260">survival</span>
  <span m="4486800">function.</span> <span m="4487230">So</span> <span m="4487360">it's</span>
  <span m="4487430">looking</span> <span m="4487670">at</span> <span m="4487760">probability</span>
  <span m="4488930">of</span> <span m="4489380">T,</span> <span m="4490400">actual</span>
  <span m="4490910">time</span> <span m="4491210">of</span> <span m="4491300">the</span>
  <span m="4491360">event,</span> <span m="4491720">being</span> <span m="4491990">larger</span>
  <span m="4492470">than</span> <span m="4492650">some</span> <span m="4493130">quantity,</span>
  <span m="4493790">little</span> <span m="4494030">t.</span> <span m="4495320">And</span>
  <span m="4495410">that's,</span> <span m="4495690">of</span> <span m="4495790">course,</span>
  <span m="4495980">just</span> <span m="4496010">the</span> <span m="4496100">integral</span>
  <span m="4496490">of</span> <span m="4496580">the</span> <span m="4496670">density</span>
  <span m="4497180">from</span> <span m="4497390">little</span> <span m="4497600">t</span>
  <span m="4497840">to</span> <span m="4497960">infinity.</span></p><p><span m="4499266">All
  right,</span> <span m="4499650">so</span> <span m="4499670">this</span> <span m="4499820">is</span>
  <span m="4499880">the</span> <span m="4499970">survival</span> <span m="4500480">function.</span>
  <span m="4501170">It's</span> <span m="4501390">of</span> <span m="4501500">a</span>
  <span m="4501560">lot</span> <span m="4501710">of</span> <span m="4501800">interest.</span>
  <span m="4502250">You</span> <span m="4502340">want</span> <span m="4502460">to</span>
  <span m="4502520">know,</span> <span m="4502700">is</span> <span m="4502790">the</span>
  <span m="4502850">patient</span> <span m="4503120">going to</span> <span m="4503240">be</span>
  <span m="4503330">diagnosed</span> <span m="4503720">with</span> <span m="4503810">diabetes</span>
  <span m="4504770">two</span> <span m="4505100">or</span> <span m="4505190">more</span>
  <span m="4505430">years</span> <span m="4505730">from</span> <span m="4505850">now.</span></p><p><span
  m="4507330">So</span> <span m="4507470">pictorially,</span> <span m="4508220">what</span>
  <span m="4508430">you're</span> <span m="4508580">interested</span> <span m="4508910">in</span>
  <span m="4508970">is</span> <span m="4509030">something</span> <span m="4509300">like</span>
  <span m="4509450">this.</span> <span m="4509660">You want</span> <span m="4509770">to</span>
  <span m="4509870">estimate</span> <span m="4510350">these</span> <span m="4510680">conditional</span>
  <span m="4511370">distributions.</span> <span m="4512240">So</span> <span m="4512990">I</span>
  <span m="4513110">call it</span> <span m="4513350">conditional</span> <span m="4513890">because</span>
  <span m="4514160">you</span> <span m="4514250">want</span> <span m="4514370">to</span>
  <span m="4514430">condition</span> <span m="4515150">on</span> <span m="4515420">the</span>
  <span m="4515510">covariant</span> <span m="4516160">to</span> <span m="4516200">individual</span>
  <span m="4516560">x.</span> <span m="4518420">So</span> <span m="4518900">what</span>
  <span m="4519080">I'm</span> <span m="4519200">showing</span> <span m="4519410">you,</span>
  <span m="4519470">this</span> <span m="4519620">black</span> <span m="4520040">line,</span>
  <span m="4520580">is</span> <span m="4520820">your</span> <span m="4520960">density,</span>
  <span m="4522170">little</span> <span m="4522500">f</span> <span m="4522680">of</span>
  <span m="4522800">t.</span> <span m="4523670">And</span> <span m="4524000">this</span>
  <span m="4524360">white</span> <span m="4524960">area</span> <span m="4525410">here,</span>
  <span m="4526990">the</span> <span m="4527140">integral</span> <span m="4527950">from</span>
  <span m="4528160">little</span> <span m="4528430">t</span> <span m="4528760">to</span>
  <span m="4528880">infinity,</span> <span m="4529700">meaning</span> <span m="4530080">all</span>
  <span m="4530320">this</span> <span m="4530560">white</span> <span m="4530920">area,</span>
  <span m="4531430">is</span> <span m="4531700">capital</span> <span m="4532240">S</span>
  <span m="4532690">of</span> <span m="4532900">t.</span> <span m="4533380">It's</span>
  <span m="4533620">the</span> <span m="4534070">probability</span> <span m="4534940">of</span>
  <span m="4535120">surviving</span> <span m="4536410">longer</span> <span m="4537160">than</span>
  <span m="4537550">time</span> <span m="4537910">little</span> <span m="4538150">t.</span></p><p><span
  m="4539430">OK,</span> <span m="4540040">so</span> <span m="4540220">the</span>
  <span m="4540340">first</span> <span m="4540790">thing</span> <span m="4541000">you</span>
  <span m="4541120">might</span> <span m="4541360">do</span> <span m="4542260">is</span>
  <span m="4542410">say,</span> <span m="4543730">we</span> <span m="4543970">get</span>
  <span m="4544270">these</span> <span m="4544960">data,</span> <span m="4545380">these</span>
  <span m="4545590">tuples,</span> <span m="4546310">and</span> <span m="4546400">we</span>
  <span m="4546520">want</span> <span m="4546760">to</span> <span m="4546880">try</span>
  <span m="4547120">to</span> <span m="4547240">estimate</span> <span m="4547880">that</span>
  <span m="4548110">function,</span> <span m="4548660">little</span> <span m="4549060">f,</span>
  <span m="4549940">the</span> <span m="4550180">probability</span> <span m="4550900">of</span>
  <span m="4551020">death</span> <span m="4551290">at</span> <span m="4551380">some</span>
  <span m="4551560">time.</span> <span m="4552250">Or,</span> <span m="4552640">equivalently,</span>
  <span m="4553390">you</span> <span m="4553480">might</span> <span m="4553630">want</span>
  <span m="4553750">to</span> <span m="4553810">estimate</span> <span m="4554320">the</span>
  <span m="4554440">survival</span> <span m="4555160">time,</span> <span m="4555490">capital</span>
  <span m="4555880">S</span> <span m="4556060">of</span> <span m="4556150">t,</span>
  <span m="4556490">which</span> <span m="4556570">is</span> <span m="4556780">the</span>
  <span m="4557350">CDF</span> <span m="4557790">version.</span> <span m="4558220">And
  these</span> <span m="4558370">two</span> <span m="4558520">are</span> <span m="4558580">related</span>
  <span m="4558880">to</span> <span m="4559000">another</span> <span m="4559360">just</span>
  <span m="4559570">by</span> <span m="4559750">some</span> <span m="4560380">calculus.
  </span></p><p><span m="4562390">So</span> <span m="4563310">a</span> <span m="4563950">method</span>
  <span m="4564310">called</span> <span m="4564550">the</span> <span m="4564640">Kaplan-Meier</span>
  <span m="4565470">estimator</span> <span m="4566040">is</span> <span m="4566290">a</span>
  <span m="4566380">non-parametric</span> <span m="4567670">method</span> <span m="4568180">for</span>
  <span m="4568390">estimating</span> <span m="4568990">that</span> <span m="4569230">survival</span>
  <span m="4570280">probability,</span> <span m="4570820">capital S of</span> <span
  m="4571310">t.</span> <span m="4573070">So</span> <span m="4573190">this</span>
  <span m="4573370">is</span> <span m="4573520">the</span> <span m="4573610">probability</span>
  <span m="4574270">that an</span> <span m="4574390">individual</span> <span m="4574720">lives</span>
  <span m="4575290">more</span> <span m="4575590">than</span> <span m="4575770">some</span>
  <span m="4575980">time</span> <span m="4576250">period.</span></p><p><span m="4577150">So</span>
  <span m="4577330">first</span> <span m="4577660">I'll</span> <span m="4579190">explain</span>
  <span m="4579550">to you</span> <span m="4579730">this</span> <span m="4579940">plot,</span>
  <span m="4580300">then</span> <span m="4580420">I'll</span> <span m="4580510">tell</span>
  <span m="4580660">you</span> <span m="4580720">how</span> <span m="4580810">to</span>
  <span m="4580900">compute</span> <span m="4581230">it.</span> <span m="4582110">So</span>
  <span m="4582310">the</span> <span m="4582430">x-axis</span> <span m="4582940">of</span>
  <span m="4583000">this</span> <span m="4583150">plot</span> <span m="4583420">is</span>
  <span m="4583600">time.</span> <span m="4584860">The</span> <span m="4584980">y-axis</span>
  <span m="4585820">is</span> <span m="4586030">this</span> <span m="4586220">survival</span>
  <span m="4586750">property,</span> <span m="4587190">capital</span> <span m="4587590">S
  of</span> <span m="4587820">t.</span> <span m="4588130">It's</span> <span m="4588580">the</span>
  <span m="4588670">probability</span> <span m="4589120">that an</span> <span m="4589400">individual</span>
  <span m="4589650">lives</span> <span m="4590050">more</span> <span m="4590470">than</span>
  <span m="4590650">this</span> <span m="4591160">amount</span> <span m="4591370">of</span>
  <span m="4591460">time.</span> <span m="4592330">I</span> <span m="4592420">think</span>
  <span m="4592660">this</span> <span m="4592900">x-axis</span> <span m="4593350">is
  in</span> <span m="4593560">days,</span> <span m="4593980">so</span> <span m="4594220">500,</span>
  <span m="4594570">1,000,</span> <span m="4595270">1,500,</span> <span m="4595960">2,000.</span>
  <span m="4597490">This</span> <span m="4597670">figure,</span> <span m="4597910">by</span>
  <span m="4598000">the</span> <span m="4598090">way,</span> <span m="4598210">was</span>
  <span m="4598330">created</span> <span m="4598600">by</span> <span m="4598690">one</span>
  <span m="4598780">of</span> <span m="4598840">my</span> <span m="4598930">students</span>
  <span m="4599350">who's</span> <span m="4599440">studying</span> <span m="4600130">a</span>
  <span m="4600430">multiple</span> <span m="4600730">myeloma</span> <span m="4601060">data</span>
  <span m="4601250">set.</span></p><p><span m="4602800">So</span> <span m="4603100">you</span>
  <span m="4603220">could</span> <span m="4603340">then</span> <span m="4603580">ask,</span>
  <span m="4604730">well,</span> <span m="4606260">under</span> <span m="4606550">what</span>
  <span m="4606760">covariants </span> <span m="4607720">do</span> <span m="4607840">you</span>
  <span m="4607930">want</span> <span m="4608080">to</span> <span m="4608140">compute</span>
  <span m="4608500">this</span> <span m="4608640">survival?</span> <span m="4609680">So</span>
  <span m="4610210">here,</span> <span m="4610840">this</span> <span m="4611080">method</span>
  <span m="4611440">I'll</span> <span m="4611560">tell</span> <span m="4611740">you</span>
  <span m="4611800">about,</span> <span m="4612430">is</span> <span m="4613750">very</span>
  <span m="4614050">good</span> <span m="4614650">for</span> <span m="4614920">when</span>
  <span m="4615070">you</span> <span m="4615160">don't</span> <span m="4615370">have</span>
  <span m="4615520">any</span> <span m="4615670">features.</span> <span m="4616520">So</span>
  <span m="4616660">all</span> <span m="4616780">you</span> <span m="4616840">want</span>
  <span m="4616960">to</span> <span m="4617020">do</span> <span m="4617080">is</span>
  <span m="4617140">estimate</span> <span m="4617500">that</span> <span m="4617620">density</span>
  <span m="4617980">by</span> <span m="4618070">itself.</span> <span m="4618460">And</span>
  <span m="4618550">of</span> <span m="4618640">course</span> <span m="4619400">you</span>
  <span m="4619420">could</span> <span m="4619510">apply</span> <span m="4620200">a</span>
  <span m="4620740">method</span> <span m="4621970">for</span> <span m="4622150">multiple</span>
  <span m="4622480">populations.</span> <span m="4623240">So</span> <span m="4623340">what</span>
  <span m="4623440">I'm</span> <span m="4623540">showing</span> <span m="4623650">you</span>
  <span m="4623740">here</span> <span m="4623950">is</span> <span m="4624040">applying</span>
  <span m="4624400">it</span> <span m="4624490">for</span> <span m="4624670">two</span>
  <span m="4624820">different</span> <span m="4625060">populations.</span> <span m="4625720">Suppose</span>
  <span m="4626020">there's</span> <span m="4626170">just</span> <span m="4626290">a</span>
  <span m="4626350">single</span> <span m="4626680">binary</span> <span m="4627070">feature.</span>
  <span m="4628040">And</span> <span m="4628600">we're</span> <span m="4628720">going</span>
  <span m="4628900">to</span> <span m="4629020">apply</span> <span m="4629350">it</span>
  <span m="4629560">to</span> <span m="4629770">the</span> <span m="4629800">x</span>
  <span m="4630010">equals</span> <span m="4630250">0</span> <span m="4631030">and</span>
  <span m="4631180">to</span> <span m="4631240">x</span> <span m="4631450">equals</span>
  <span m="4631720">1.</span> <span m="4631875">That</span> <span m="4632030">gets</span>
  <span m="4632180">you</span> <span m="4632260">two</span> <span m="4632440">different</span>
  <span m="4632650">curves</span> <span m="4632980">out.</span> <span m="4633670">But</span>
  <span m="4634030">here</span> <span m="4634290">the</span> <span m="4634410">estimator</span>
  <span m="4634820">is</span> <span m="4634930">going</span> <span m="4635080">to</span>
  <span m="4635410">work</span> <span m="4635860">independently</span> <span m="4636460">for</span>
  <span m="4636640">each</span> <span m="4636790">of</span> <span m="4636850">the</span>
  <span m="4636910">two</span> <span m="4637060">populations.</span></p><p><span m="4639140">So</span>
  <span m="4639340">what</span> <span m="4639550">you</span> <span m="4639670">see</span>
  <span m="4639880">here</span> <span m="4640060">on</span> <span m="4640150">this</span>
  <span m="4640270">red</span> <span m="4640540">line</span> <span m="4640900">is</span>
  <span m="4641020">for</span> <span m="4641140">the</span> <span m="4641230">x</span>
  <span m="4641500">equals</span> <span m="4641740">0</span> <span m="4642010">population.</span>
  <span m="4642800">We</span> <span m="4642850">see</span> <span m="4643210">that,</span>
  <span m="4644030">at</span> <span m="4644140">time</span> <span m="4644580">0,</span>
  <span m="4645370">everyone</span> <span m="4645730">is</span> <span m="4645820">alive,</span>
  <span m="4646570">as</span> <span m="4646720">you</span> <span m="4646780">would</span>
  <span m="4646870">expect.</span> <span m="4648820">And</span> <span m="4649390">at</span>
  <span m="4649740">time</span> <span m="4650210">1,000,</span> <span m="4651920">roughly</span>
  <span m="4652730">60%</span> <span m="4654580">individuals</span> <span m="4655000">are</span>
  <span m="4655060">still</span> <span m="4655450">alive</span> <span m="4655860">for</span>
  <span m="4656020">time</span> <span m="4656320">1,000.</span> <span m="4657340">And</span>
  <span m="4657490">that</span> <span m="4657640">sort</span> <span m="4657820">of</span>
  <span m="4657910">stays</span> <span m="4658210">constant.</span></p><p><span m="4659480">Now</span>
  <span m="4659560">you</span> <span m="4659650">see</span> <span m="4659980">that,</span>
  <span m="4660340">for</span> <span m="4660550">the</span> <span m="4660670">other</span>
  <span m="4661150">subgroup,</span> <span m="4661495">the</span> <span m="4661840">x</span>
  <span m="4662050">equals 1</span> <span m="4662320">subgroup,</span> <span m="4664570">again,</span>
  <span m="4665010">time</span> <span m="4665260">step</span> <span m="4665470">0,</span>
  <span m="4665770">as</span> <span m="4665860">you</span> <span m="4665920">would</span>
  <span m="4666010">expect,</span> <span m="4666460">everyone</span> <span m="4666820">is</span>
  <span m="4666940">alive.</span> <span m="4667810">But</span> <span m="4668560">they</span>
  <span m="4668710">survive</span> <span m="4669220">much</span> <span m="4669460">longer.</span>
  <span m="4670180">At time</span> <span m="4670470">step</span> <span m="4670640">1,000,</span>
  <span m="4671200">over</span> <span m="4671410">75%</span> <span m="4672130">of</span>
  <span m="4672190">them</span> <span m="4672370">are</span> <span m="4672430">still</span>
  <span m="4672670">alive.</span> <span m="4673570">And</span> <span m="4673690">of</span>
  <span m="4673750">course</span> <span m="4674020">of</span> <span m="4674110">interest</span>
  <span m="4674470">here</span> <span m="4674650">is</span> <span m="4674740">also</span>
  <span m="4674920">confidence</span> <span m="4675370">balance.</span> <span m="4675760">I'm</span>
  <span m="4675850">not</span> <span m="4675940">going</span> <span m="4676060">to</span>
  <span m="4676120">tell</span> <span m="4676240">you</span> <span m="4676330">how</span>
  <span m="4676450">can</span> <span m="4676630">you</span> <span m="4676680">do</span>
  <span m="4676750">that,</span> <span m="4676900">but</span> <span m="4677020">it's</span>
  <span m="4677140">in</span> <span m="4677260">some of the</span> <span m="4677480">optional</span>
  <span m="4677800">readings.</span> <span m="4678820">And</span> <span m="4679330">by</span>
  <span m="4679450">the</span> <span m="4679540">way,</span> <span m="4679840">there</span>
  <span m="4679970">are</span> <span m="4680020">more</span> <span m="4680260">optional</span>
  <span m="4680560">readings</span> <span m="4680980">given</span> <span m="4681250">on</span>
  <span m="4681340">the</span> <span m="4681430">bottom</span> <span m="4681790">of</span>
  <span m="4681880">these</span> <span m="4682000">slides.</span></p><p><span m="4683820">And</span>
  <span m="4683980">so</span> <span m="4684100">you</span> <span m="4684220">see</span>
  <span m="4684400">that</span> <span m="4684550">there</span> <span m="4684670">is</span>
  <span m="4684740">a</span> <span m="4684760">statistically</span> <span m="4685630">significant</span>
  <span m="4686170">difference</span> <span m="4686770">between</span> <span m="4687610">x</span>
  <span m="4687880">equals 1 and</span> <span m="4688150">x</span> <span m="4688630">equals</span>
  <span m="4688870">0.</span> <span m="4689290">These</span> <span m="4689560">people</span>
  <span m="4689800">seem</span> <span m="4689980">to</span> <span m="4690100">be surviving</span>
  <span m="4690430">longer</span> <span m="4690790">than</span> <span m="4690940">these</span>
  <span m="4691120">people.</span> <span m="4691490">And</span> <span m="4691660">you</span>
  <span m="4691750">get</span> <span m="4691900">that</span> <span m="4692020">immediately</span>
  <span m="4692350">from</span> <span m="4692470">this</span> <span m="4692590">curve.</span></p><p><span
  m="4693530">So</span> <span m="4693580">how</span> <span m="4693670">do</span> <span
  m="4693760">we</span> <span m="4693850">compute</span> <span m="4694150">that?</span>
  <span m="4695240">Well,</span> <span m="4695680">we</span> <span m="4695800">take</span>
  <span m="4696010">those</span> <span m="4696220">observed</span> <span m="4696790">times,</span>
  <span m="4697630">those</span> <span m="4697870">capital</span> <span m="4698430">Ts,</span>
  <span m="4700840">and</span> <span m="4701470">here</span> <span m="4701830">I'm</span>
  <span m="4701920">going</span> <span m="4702130">to</span> <span m="4702220">call</span>
  <span m="4702520">them</span> <span m="4703020">just</span> <span m="4703970">y.</span>
  <span m="4704410">I'm</span> <span m="4704470">going</span> <span m="4704590">to</span>
  <span m="4704680">sort</span> <span m="4705190">them.</span> <span m="4705610">So</span>
  <span m="4705940">these</span> <span m="4706150">are</span> <span m="4706240">sorted</span>
  <span m="4706870">times.</span> <span m="4708280">And</span> <span m="4709900">I</span>
  <span m="4709990">don't</span> <span m="4710140">care</span> <span m="4710440">whether</span>
  <span m="4710650">they</span> <span m="4710740">were</span> <span m="4710830">censored</span>
  <span m="4711340">or</span> <span m="4711430">not</span> <span m="4711640">censored.</span></p><p><span
  m="4712680">So</span> <span m="4713050">y</span> <span m="4713470">is</span> <span
  m="4713560">just</span> <span m="4713710">all</span> <span m="4713920">of</span>
  <span m="4713980">the</span> <span m="4714070">times</span> <span m="4714520">for</span>
  <span m="4714640">all</span> <span m="4714760">of</span> <span m="4714850">the</span>
  <span m="4714910">patients,</span> <span m="4715840">whether</span> <span m="4716210">they</span>
  <span m="4716320">are</span> <span m="4716410">censored</span> <span m="4716800">or</span>
  <span m="4716860">not.</span> <span m="4718490">dK</span> <span m="4719170">I want</span>
  <span m="4719260">you</span> <span m="4719320">think</span> <span m="4719500">about</span>
  <span m="4719620">as</span> <span m="4719740">1.</span> <span m="4720310">It's</span>
  <span m="4720520">the</span> <span m="4720670">number</span> <span m="4720910">of</span>
  <span m="4720970">events</span> <span m="4721330">that</span> <span m="4721420">occurred</span>
  <span m="4722140">at</span> <span m="4722260">that</span> <span m="4722440">time.</span>
  <span m="4723310">So</span> <span m="4723430">if</span> <span m="4723580">everyone</span>
  <span m="4723910">had</span> <span m="4724060">a</span> <span m="4724090">unique</span>
  <span m="4724510">time</span> <span m="4724780">of</span> <span m="4724870">censoring</span>
  <span m="4725320">or</span> <span m="4725410">death,</span> <span m="4725740">then</span>
  <span m="4725920">dK</span> <span m="4726170">is</span> <span m="4726310">always</span>
  <span m="4726550">1.</span> <span m="4727510">K is</span> <span m="4727810">indexing</span>
  <span m="4728260">one</span> <span m="4728410">of</span> <span m="4728500">these</span>
  <span m="4728680">things.</span> <span m="4729910">n</span> <span m="4730120">of</span>
  <span m="4730270">K</span> <span m="4730960">is</span> <span m="4731110">the</span>
  <span m="4731200">number</span> <span m="4731500">of</span> <span m="4731590">individuals</span>
  <span m="4732430">alive</span> <span m="4733180">and</span> <span m="4733420">uncensored</span>
  <span m="4734320">by</span> <span m="4734680">the</span> <span m="4734800">K-th</span>
  <span m="4735250">time</span> <span m="4735610">point.</span></p><p><span m="4736930">Then</span>
  <span m="4737080">what</span> <span m="4737180">this</span> <span m="4737320">estimator</span>
  <span m="4737800">says</span> <span m="4738610">is</span> <span m="4738790">that</span>
  <span m="4739570">S</span> <span m="4740050">of</span> <span m="4740230">t--</span>
  <span m="4741160">so</span> <span m="4741310">the</span> <span m="4741380">estimator</span>
  <span m="4741820">at</span> <span m="4741970">any</span> <span m="4742180">point</span>
  <span m="4742450">in</span> <span m="4742540">time--</span> <span m="4743200">is</span>
  <span m="4743350">given</span> <span m="4743650">to</span> <span m="4743830">you</span>
  <span m="4743980">by</span> <span m="4744130">the</span> <span m="4744250">product</span>
  <span m="4745270">over</span> <span m="4746290">K</span> <span m="4747190">such</span>
  <span m="4747460">that</span> <span m="4747910">y</span> <span m="4748450">of</span>
  <span m="4748570">K</span> <span m="4748800">is</span> <span m="4748950">less than
  or</span> <span m="4749350">equal</span> <span m="4749560">to</span> <span m="4749680">t.</span>
  <span m="4750010">So</span> <span m="4750160">it's</span> <span m="4750280">going</span>
  <span m="4750730">over</span> <span m="4751240">the</span> <span m="4751420">observed</span>
  <span m="4751930">times</span> <span m="4752410">up</span> <span m="4752590">to</span>
  <span m="4753130">little</span> <span m="4753490">t,</span> <span m="4754570">of</span>
  <span m="4754720">1</span> <span m="4755110">minus</span> <span m="4755500">the</span>
  <span m="4755590">ratio</span> <span m="4756440">of</span> <span m="4756670">1</span>
  <span m="4757240">over--</span> <span m="4757810">so</span> <span m="4757930">I'm</span>
  <span m="4758020">thinking</span> <span m="4758240">about</span> <span m="4758350">dK</span>
  <span m="4758700">as</span> <span m="4758840">1--</span> <span m="4759430">1</span>
  <span m="4759820">over</span> <span m="4760240">the</span> <span m="4760360">number</span>
  <span m="4760570">of</span> <span m="4760630">people</span> <span m="4760900">who</span>
  <span m="4761020">are</span> <span m="4761080">alive</span> <span m="4761440">and</span>
  <span m="4761530">uncensored</span> <span m="4762070">by</span> <span m="4762220">that</span>
  <span m="4762370">time.</span> <span m="4763860">And</span> <span m="4763990">that</span>
  <span m="4764080">has</span> <span m="4764230">a</span> <span m="4764260">very</span>
  <span m="4764500">intuitive</span> <span m="4765310">definition.</span></p><p><span
  m="4766510">And</span> <span m="4767050">one</span> <span m="4767260">can</span>
  <span m="4767530">prove</span> <span m="4767980">that</span> <span m="4768130">this</span>
  <span m="4768310">estimator</span> <span m="4768850">gives</span> <span m="4769150">you</span>
  <span m="4769300">a</span> <span m="4769390">consistent</span> <span m="4770050">estimator</span>
  <span m="4770710">of</span> <span m="4771370">the</span> <span m="4771460">number</span>
  <span m="4771790">of</span> <span m="4771910">people</span> <span m="4772270">who</span>
  <span m="4772480">are</span> <span m="4772630">alive--</span> <span m="4774620">sorry,</span>
  <span m="4774760">the</span> <span m="4774850">number</span> <span m="4775180">of</span>
  <span m="4775510">survival</span> <span m="4775960">probability</span> <span m="4776910">at</span>
  <span m="4777040">any</span> <span m="4777210">one</span> <span m="4777370">point</span>
  <span m="4777610">in</span> <span m="4777700">time</span> <span m="4780260">for</span>
  <span m="4780580">censored</span> <span m="4781210">data.</span> <span m="4781690">And</span>
  <span m="4781810">that's</span> <span m="4781990">critical.</span> <span m="4782380">This</span>
  <span m="4782560">works</span> <span m="4782800">for</span> <span m="4782890">censored</span>
  <span m="4783190">data.</span> <span m="4785020">So</span> <span m="4786040">I'm</span>
  <span m="4786190">past</span> <span m="4786580">time</span> <span m="4786910">today.</span>
  <span m="4787340">So</span> <span m="4787570">I'll</span> <span m="4787750">finish</span>
  <span m="4788200">the</span> <span m="4788350">last</span> <span m="4788650">few</span>
  <span m="4788860">slides</span> <span m="4791020">on</span> <span m="4791140">Tuesday's</span>
  <span m="4791500">lecture.</span> <span m="4791860">So</span> <span m="4791980">that's</span>
  <span m="4792130">all</span> <span m="4792200">for</span> <span m="4792310">today.</span>
  <span m="4792520">Thanks.</span></p><p>&nbsp;</p>
type: course
uid: b923017e9d4756e7bd74deb4ab63c6fa

---
None