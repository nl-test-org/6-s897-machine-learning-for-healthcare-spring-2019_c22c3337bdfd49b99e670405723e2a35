---
about_this_resource_text: '<p>Prof. Sontag gives a recap of risk stratification and
  then explains physiological time-series. Two scenarios are examined: monitoring
  babies in neonatal ICUs and detecting atrial fibrillation.</p> <p>Speaker: David
  Sontag</p>             <p><a href="./resolveuid/2f322bbcdc5169c015f24a7ec3e76d4a">Lecture
  6: Physiological Time-Series slides (PDF - 1.5MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: lLhfDSOwWtU
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: Video-YouTube-Stream
  type: Video
  uid: e99af6dbe7b6db297035dd06847b09ce
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/lLhfDSOwWtU/default.jpg
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 8950202e516fc11fdb7ae374b34c7f8d
- id: 3Play-3PlayYouTubeid-MP4
  media_location: lLhfDSOwWtU
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: 1e544d0d5411e6af627e18085bab6697
- id: lLhfDSOwWtU.srt
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-6-physiological-time-series/lLhfDSOwWtU.srt
  title: 3play caption file
  type: null
  uid: f5529ea721381cfa5803d54b077b99bf
- id: lLhfDSOwWtU.pdf
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-6-physiological-time-series/lLhfDSOwWtU.pdf
  title: 3play pdf file
  type: null
  uid: 7287343c73f1afdce1dab0121331b7d5
- id: Caption-3Play YouTube id-SRT
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: d7a364fa9cc3f5c4454ffb8b86b828ff
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 3d23f96c976c3a4733afd37eb6898513
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec06_300k.mp4
  parent_uid: 44f500ad6f949b39c554882388e3e81e
  title: Video-Internet Archive-MP4
  type: Video
  uid: d72e25267bc329be324957da33050542
inline_embed_id: 56486643lecture6physiologicaltimeseries35813798
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-6-physiological-time-series
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-6-physiological-time-series
template_type: Tabbed
title: 'Lecture 6: Physiological Time-Series'
transcript: <p><span m="15580">DAVID SONTAG:</span> <span m="15745">So</span> <span
  m="15910">I'll</span> <span m="16030">begin</span> <span m="16300">today's</span>
  <span m="16700">lecture</span> <span m="16880">by</span> <span m="17080">giving</span>
  <span m="17500">a</span> <span m="18400">brief</span> <span m="18700">recap</span>
  <span m="19170">of</span> <span m="19270">risk</span> <span m="19450">stratification.</span>
  <span m="20860">We</span> <span m="20980">didn't</span> <span m="21160">get</span>
  <span m="21280">to</span> <span m="21370">finish</span> <span m="21640">talking</span>
  <span m="21960">survival</span> <span m="22330">modeling</span> <span m="22960">on</span>
  <span m="23590">Thursday,</span> <span m="24070">and</span> <span m="24160">so</span>
  <span m="24320">I'll</span> <span m="24370">go</span> <span m="24550">a</span> <span
  m="24610">little</span> <span m="24790">bit</span> <span m="24880">more</span> <span
  m="25090">into</span> <span m="25300">that,</span> <span m="25840">and</span> <span
  m="25960">I'll</span> <span m="26170">answer</span> <span m="26470">some</span>
  <span m="26620">of</span> <span m="26680">the</span> <span m="26740">questions</span>
  <span m="27190">that</span> <span m="27310">arose</span> <span m="27760">during</span>
  <span m="28300">our</span> <span m="28480">discussions</span> <span m="29170">and</span>
  <span m="29260">on</span> <span m="29380">Piazza</span> <span m="29640">since.</span>
  <span m="30810">And</span> <span m="31300">then</span> <span m="31390">the</span>
  <span m="31480">vast</span> <span m="31720">majority</span> <span m="32080">of</span>
  <span m="32170">today's</span> <span m="32409">lecture</span> <span m="32840">we'll</span>
  <span m="32860">be</span> <span m="32950">talking</span> <span m="33190">about</span>
  <span m="33310">a</span> <span m="33370">new</span> <span m="33490">topic--</span>
  <span m="35100">in</span> <span m="35260">particular,</span> <span m="35650">physiological</span>
  <span m="36190">time</span> <span m="36430">series</span> <span m="36670">modeling.</span>
  <span m="37600">I'll</span> <span m="37690">give</span> <span m="37930">two</span>
  <span m="38140">examples</span> <span m="39040">of</span> <span m="39310">physiological</span>
  <span m="39910">time</span> <span m="40170">series</span> <span m="40400">modeling--</span>
  <span m="40880">the</span> <span m="40980">first</span> <span m="41200">one</span>
  <span m="41500">coming</span> <span m="41830">from</span> <span m="42760">monitoring</span>
  <span m="43210">patients</span> <span m="43810">in</span> <span m="43960">intensive</span>
  <span m="44350">care</span> <span m="44560">units,</span> <span m="45370">and</span>
  <span m="45460">the</span> <span m="45520">second</span> <span m="45820">one</span>
  <span m="46300">asking</span> <span m="46660">a very</span> <span m="46840">different</span>
  <span m="47080">type</span> <span m="47200">of</span> <span m="47260">question--</span>
  <span m="47800">that</span> <span m="48190">of</span> <span m="48880">diagnosing</span>
  <span m="49660">patients'</span> <span m="50200">heart</span> <span m="50410">conditions</span>
  <span m="50950">using</span> <span m="52110">EKGs.</span></p><p><span m="53620">And</span>
  <span m="53980">both</span> <span m="54220">of</span> <span m="54280">these</span>
  <span m="54430">correspond</span> <span m="54910">to</span> <span m="55000">readings</span>
  <span m="55390">that</span> <span m="55510">you</span> <span m="55630">had</span>
  <span m="56020">for</span> <span m="56230">today's</span> <span m="56530">lecture,</span>
  <span m="57040">and</span> <span m="57160">we'll</span> <span m="57250">go</span>
  <span m="57370">into</span> <span m="57550">much</span> <span m="57730">more</span>
  <span m="57850">depth</span> <span m="58240">in</span> <span m="58330">these--</span>
  <span m="59200">of</span> <span m="59350">those</span> <span m="59620">papers</span>
  <span m="60010">today,</span> <span m="60370">and</span> <span m="60630">I'll</span>
  <span m="60760">provide</span> <span m="61000">much</span> <span m="61150">more</span>
  <span m="61240">color</span> <span m="61660">around</span> <span m="61900">them.</span>
  <span m="65379">So</span> <span m="65430">just</span> <span m="65580">to</span>
  <span m="65640">briefly</span> <span m="65940">remind</span> <span m="66270">you</span>
  <span m="66360">where</span> <span m="66480">we</span> <span m="66630">were</span>
  <span m="67050">on</span> <span m="67230">Thursday,</span> <span m="68130">we</span>
  <span m="68250">talked</span> <span m="68490">about</span> <span m="68670">how</span>
  <span m="68850">one</span> <span m="69060">could</span> <span m="69180">formalize</span>
  <span m="69820">risk</span> <span m="70000">stratification</span> <span m="70320">instead</span>
  <span m="70650">of</span> <span m="70710">as</span> <span m="70830">a</span> <span
  m="70890">classification</span> <span m="71670">problem</span> <span m="72100">of</span>
  <span m="72310">what would</span> <span m="72480">happen,</span> <span m="72840">let's</span>
  <span m="72990">say,</span> <span m="73320">in</span> <span m="73470">some</span>
  <span m="73680">predefined</span> <span m="74340">time</span> <span m="74700">period,</span>
  <span m="75570">rather</span> <span m="75780">thinking</span> <span m="76170">about</span>
  <span m="76890">risk</span> <span m="77100">stratification</span> <span m="77640">as</span>
  <span m="77940">a</span> <span m="78060">regression</span> <span m="78750">question,</span>
  <span m="79490">or</span> <span m="79600">regression</span> <span m="80040">task.</span></p><p><span
  m="81390">Given</span> <span m="82020">what</span> <span m="82200">you</span> <span
  m="82290">know</span> <span m="82410">about</span> <span m="82560">a</span> <span
  m="82590">patient</span> <span m="82890">at</span> <span m="82980">time</span> <span
  m="83310">zero,</span> <span m="83910">predicting</span> <span m="84780">time</span>
  <span m="85380">to</span> <span m="85620">event--</span> <span m="86380">so</span>
  <span m="86490">for</span> <span m="86580">example,</span> <span m="87090">here</span>
  <span m="87930">the</span> <span m="88080">event</span> <span m="88410">might</span>
  <span m="88680">be</span> <span m="88950">death,</span> <span m="89470">divorce,</span>
  <span m="89790">college</span> <span m="90060">graduation.</span> <span m="91150">And</span>
  <span m="91470">patient</span> <span m="91950">one--</span> <span m="93690">that</span>
  <span m="94020">event</span> <span m="94290">happened</span> <span m="94650">at</span>
  <span m="94720">time</span> <span m="94980">step</span> <span m="95250">nine.</span>
  <span m="95850">Patient</span> <span m="96180">two,</span> <span m="96390">that</span>
  <span m="96510">event</span> <span m="96720">happened</span> <span m="96960">at</span>
  <span m="97020">time</span> <span m="97290">step</span> <span m="97570">12.</span>
  <span m="98340">And</span> <span m="98580">for</span> <span m="98700">patient</span>
  <span m="99030">four,</span> <span m="100170">we</span> <span m="100290">don't</span>
  <span m="100440">know</span> <span m="100590">when</span> <span m="100740">that</span>
  <span m="100890">event</span> <span m="101190">happened,</span> <span m="102510">because</span>
  <span m="103170">it</span> <span m="103290">was</span> <span m="103440">censored.</span>
  <span m="105240">In</span> <span m="105340">particular,</span> <span m="106210">after</span>
  <span m="106600">time</span> <span m="106870">step</span> <span m="107110">seven,</span>
  <span m="107710">we</span> <span m="107830">no</span> <span m="108010">longer</span>
  <span m="108250">get</span> <span m="108370">to</span> <span m="108460">view</span>
  <span m="109300">any</span> <span m="109510">of</span> <span m="109570">the</span>
  <span m="109630">patients'</span> <span m="109990">data,</span> <span m="110340">and</span>
  <span m="110440">so</span> <span m="110560">we</span> <span m="110650">don't</span>
  <span m="110800">know</span> <span m="110950">when</span> <span m="111880">that</span>
  <span m="112000">red</span> <span m="112180">dot</span> <span m="112390">would</span>
  <span m="112510">be--</span> <span m="112960">sometime</span> <span m="113320">in</span>
  <span m="113380">the</span> <span m="113440">future</span> <span m="113770">or</span>
  <span m="113890">never.</span></p><p><span m="115360">So</span> <span m="115480">this</span>
  <span m="115630">is</span> <span m="115690">what</span> <span m="115840">we</span>
  <span m="115960">mean</span> <span m="116160">by</span> <span m="116250">right</span>
  <span m="116590">censor</span> <span m="116980">data,</span> <span m="117370">which</span>
  <span m="117550">is</span> <span m="117640">precisely</span> <span m="118180">what</span>
  <span m="118600">survival</span> <span m="119080">modeling</span> <span m="119500">is</span>
  <span m="119650">aiming</span> <span m="120040">to</span> <span m="120670">solve.</span>
  <span m="121780">Are</span> <span m="121840">there</span> <span m="121990">questions</span>
  <span m="122410">about</span> <span m="122560">this</span> <span m="122650">setup</span>
  <span m="122980">first?</span></p><p><span m="126358">AUDIENCE:</span> <span m="126597">You</span>
  <span m="126836">flipped</span> <span m="127314">the</span> <span m="127792">x</span>
  <span m="128270">on--</span></p><p><span m="128750">DAVID SONTAG:</span> <span m="128985">Yeah,</span>
  <span m="129220">I realized</span> <span m="129580">that.</span> <span m="129759">I</span>
  <span m="129820">flipped</span> <span m="130090">the</span> <span m="130220">x and</span>
  <span m="130550">the o</span> <span m="130960">in</span> <span m="131170">today's</span>
  <span m="131450">presentation,</span> <span m="131860">but that's</span> <span m="131980">not</span>
  <span m="132130">relevant.</span> <span m="134720">So</span> <span m="135450">f</span>
  <span m="135720">of</span> <span m="135980">t</span> <span m="136240">is</span>
  <span m="136720">the</span> <span m="136870">probability</span> <span m="137380">of</span>
  <span m="137470">death,</span> <span m="138370">or</span> <span m="138520">the</span>
  <span m="138640">event</span> <span m="138910">occurring</span> <span m="139360">at</span>
  <span m="139480">time</span> <span m="139750">step</span> <span m="139990">t.</span>
  <span m="140860">And</span> <span m="141160">although</span> <span m="141430">in</span>
  <span m="141490">this</span> <span m="141610">slide</span> <span m="142040">I'm</span>
  <span m="142140">showing</span> <span m="142330">it</span> <span m="142450">as</span>
  <span m="142630">an</span> <span m="142780">unconditional</span> <span m="143410">model,</span>
  <span m="143740">in</span> <span m="143830">general,</span> <span m="144300">you</span>
  <span m="144310">should</span> <span m="144430">think</span> <span m="144610">about</span>
  <span m="144760">this</span> <span m="144910">as</span> <span m="145000">a</span>
  <span m="145060">conditional</span> <span m="145600">density.</span> <span m="145875">So</span>
  <span m="146150">you</span> <span m="146230">might</span> <span m="146380">be</span>
  <span m="146470">conditioning</span> <span m="146950">on</span> <span m="147040">some</span>
  <span m="147220">covariates</span> <span m="147730">or</span> <span m="147790">features</span>
  <span m="148210">that</span> <span m="148300">you</span> <span m="148390">have for</span>
  <span m="148810">that</span> <span m="149110">patient</span> <span m="149710">at</span>
  <span m="150040">baseline.</span></p><p><span m="151810">And</span> <span m="153220">very</span>
  <span m="153550">important</span> <span m="153970">for</span> <span m="154090">survival</span>
  <span m="154420">modeling</span> <span m="154840">and</span> <span m="154940">for</span>
  <span m="154960">the</span> <span m="155050">next</span> <span m="155320">things</span>
  <span m="155590">I'll</span> <span m="155680">tell</span> <span m="155890">you</span>
  <span m="156520">are</span> <span m="156760">the</span> <span m="156910">survival</span>
  <span m="157360">function,</span> <span m="157615">to</span> <span m="158310">note
  it</span> <span m="158520">as</span> <span m="158710">capital</span> <span m="159100">S</span>
  <span m="159280">of</span> <span m="159400">t.</span> <span m="159790">And</span>
  <span m="159910">that's</span> <span m="160060">simply</span> <span m="160950">1</span>
  <span m="161290">minus</span> <span m="161860">the</span> <span m="162610">cumulative</span>
  <span m="163060">density</span> <span m="164140">function.</span> <span m="165170">So</span>
  <span m="165340">it's</span> <span m="165790">the</span> <span m="165880">probability</span>
  <span m="166720">that</span> <span m="167020">the</span> <span m="167170">event</span>
  <span m="167530">occurring,</span> <span m="168040">which</span> <span m="168160">is</span>
  <span m="168280">time--</span> <span m="169120">which</span> <span m="169270">is</span>
  <span m="169390">denoted</span> <span m="169750">here</span> <span m="169990">as</span>
  <span m="170170">capital</span> <span m="170590">T,</span> <span m="171640">occurs</span>
  <span m="172330">greater</span> <span m="172870">than</span> <span m="173530">some</span>
  <span m="173800">little</span> <span m="174070">t.</span> <span m="174430">So</span>
  <span m="174550">it's</span> <span m="174670">this</span> <span m="174910">function,</span>
  <span m="176360">which</span> <span m="176440">is</span> <span m="176500">simply</span>
  <span m="176770">given</span> <span m="176940">to</span> <span m="177010">you</span>
  <span m="177070">by</span> <span m="177190">the</span> <span m="177250">integral</span>
  <span m="177790">from</span> <span m="178000">0</span> <span m="178450">to</span>
  <span m="178540">infinity</span> <span m="179260">of</span> <span m="179590">the</span>
  <span m="179710">density.</span></p><p><span m="181370">So</span> <span m="181460">in</span>
  <span m="181550">pictures,</span> <span m="183170">this</span> <span m="183410">is</span>
  <span m="183560">the</span> <span m="183650">density.</span> <span m="184520">On</span>
  <span m="184670">the</span> <span m="184760">x-axis</span> <span m="185320">is</span>
  <span m="185420">time.</span> <span m="186230">The</span> <span m="186320">y-axis</span>
  <span m="186830">is</span> <span m="186920">the</span> <span m="187010">density</span>
  <span m="187460">function.</span> <span m="188040">And</span> <span m="188140">this</span>
  <span m="188210">black</span> <span m="188690">curve</span> <span m="189200">is</span>
  <span m="189380">what</span> <span m="189500">I'm</span> <span m="189610">denoting</span>
  <span m="189950">as</span> <span m="190100">f</span> <span m="190350">of</span>
  <span m="190460">t.</span> <span m="191660">And</span> <span m="192050">this</span>
  <span m="192560">white</span> <span m="193310">area</span> <span m="194240">is</span>
  <span m="195140">capital</span> <span m="195560">s of</span> <span m="195860">c,</span>
  <span m="196160">the</span> <span m="196320">survival</span> <span m="197360">probability,</span>
  <span m="198390">or</span> <span m="198530">survival</span> <span m="198830">function.</span>
  <span m="201250">Yes?</span></p><p><span m="201990">AUDIENCE:</span> <span m="202060">So</span>
  <span m="202130">I just</span> <span m="202340">want</span> <span m="202400">to</span>
  <span m="202460">be</span> <span m="202600">clear.</span> <span m="203090">So</span>
  <span m="203170">if</span> <span m="203290">you</span> <span m="203500">were</span>
  <span m="203650">to</span> <span m="203770">integrate</span> <span m="204160">the</span>
  <span m="204250">entire</span> <span m="204620">curve,</span> <span m="206446">[INAUDIBLE]</span>
  <span m="209460">by</span> <span m="209932">infinity</span> <span m="210404">you're
  going to be</span> <span m="210876">[INAUDIBLE].</span></p><p><span m="211820">DAVID
  SONTAG:</span> <span m="212070">In</span> <span m="212320">the</span> <span m="212410">way</span>
  <span m="212560">that</span> <span m="212920">I</span> <span m="213100">described</span>
  <span m="213490">it</span> <span m="213550">to</span> <span m="213820">here,</span>
  <span m="214330">yes,</span> <span m="215590">because</span> <span m="215800">we're</span>
  <span m="215890">talking</span> <span m="216310">about</span> <span m="216670">the</span>
  <span m="218560">time</span> <span m="218950">to</span> <span m="219130">event.</span>
  <span m="221050">But</span> <span m="222340">often</span> <span m="223390">we</span>
  <span m="223540">might</span> <span m="223690">be</span> <span m="223780">in</span>
  <span m="223840">scenarios</span> <span m="224200">where</span> <span m="224290">the</span>
  <span m="224350">event</span> <span m="224560">may</span> <span m="224680">never</span>
  <span m="224950">occur,</span> <span m="225710">and</span> <span m="225730">so</span>
  <span m="227860">that--</span> <span m="228310">you</span> <span m="228640">can</span>
  <span m="228760">formalize</span> <span m="229020">that</span> <span m="229150">in
  a</span> <span m="229180">couple</span> <span m="229360">of</span> <span m="229390">different</span>
  <span m="229600">ways.</span> <span m="229870">You</span> <span m="229930">could</span>
  <span m="230030">put</span> <span m="230120">that at</span> <span m="230230">point</span>
  <span m="230470">mass</span> <span m="230740">at</span> <span m="230860">s</span>
  <span m="230980">of</span> <span m="231130">infinity,</span> <span m="232060">or</span>
  <span m="232200">you</span> <span m="232270">could</span> <span m="232390">simply</span>
  <span m="232660">say</span> <span m="232870">that</span> <span m="232980">the</span>
  <span m="233050">integral</span> <span m="233560">from</span> <span m="233800">0</span>
  <span m="234190">to</span> <span m="234670">infinity</span> <span m="235270">is</span>
  <span m="235420">some</span> <span m="235980">quantity</span> <span m="236410">less</span>
  <span m="236650">than</span> <span m="236800">1.</span></p><p><span m="237730">And</span>
  <span m="237820">in</span> <span m="237910">the</span> <span m="237970">readings</span>
  <span m="238480">that</span> <span m="238630">I'm</span> <span m="239020">referencing</span>
  <span m="239440">in</span> <span m="239500">the</span> <span m="239560">very</span>
  <span m="239770">bottom of those</span> <span m="239980">slides--</span> <span m="240290">it</span>
  <span m="240440">shows</span> <span m="240760">you</span> <span m="240850">how</span>
  <span m="240970">you</span> <span m="241090">can</span> <span m="241330">very</span>
  <span m="241630">easily</span> <span m="241960">modify</span> <span m="242560">all</span>
  <span m="242700">of</span> <span m="242740">the</span> <span m="242860">frameworks</span>
  <span m="243310">I'm</span> <span m="243400">telling you</span> <span m="243640">about</span>
  <span m="243820">here</span> <span m="244420">to</span> <span m="244570">deal</span>
  <span m="244750">with</span> <span m="244900">that</span> <span m="245050">scenario</span>
  <span m="245500">where</span> <span m="245710">the</span> <span m="245770">event</span>
  <span m="245980">may</span> <span m="246100">never</span> <span m="246310">occur.</span>
  <span m="247120">But</span> <span m="247540">for</span> <span m="247960">the</span>
  <span m="248050">purposes</span> <span m="248440">of</span> <span m="249070">my</span>
  <span m="249310">presentation,</span> <span m="249820">you</span> <span m="249910">can</span>
  <span m="250030">assume</span> <span m="250390">that</span> <span m="250660">the</span>
  <span m="250750">event</span> <span m="251020">will</span> <span m="251110">always</span>
  <span m="251410">occur</span> <span m="251680">at</span> <span m="251860">some</span>
  <span m="252070">point.</span> <span m="253000">It's</span> <span m="253840">a</span>
  <span m="253870">very</span> <span m="254290">minor</span> <span m="254620">modification</span>
  <span m="255160">where</span> <span m="255250">you,</span> <span m="255310">in</span>
  <span m="255370">essence,</span> <span m="256300">divide</span> <span m="257350">the</span>
  <span m="257440">densities</span> <span m="258130">by</span> <span m="259600">a</span>
  <span m="259810">constant,</span> <span m="260660">which</span> <span m="260740">accounts</span>
  <span m="261089">for</span> <span m="261190">the</span> <span m="261279">fact</span>
  <span m="261700">that</span> <span m="261910">it</span> <span m="261970">wouldn't</span>
  <span m="262210">integrate</span> <span m="262510">to</span> <span m="262600">one</span>
  <span m="262780">otherwise.</span></p><p><span m="266170">Now,</span> <span m="267490">a</span>
  <span m="267580">key</span> <span m="267940">question</span> <span m="268420">that</span>
  <span m="268540">has</span> <span m="268780">to</span> <span m="268870">be</span>
  <span m="269320">solved</span> <span m="270100">when</span> <span m="270580">trying</span>
  <span m="270880">to</span> <span m="270970">use</span> <span m="271120">a</span>
  <span m="271180">parametric</span> <span m="272110">approach</span> <span m="272500">to</span>
  <span m="272620">survivor</span> <span m="272980">modeling</span> <span m="273400">is,</span>
  <span m="273520">what</span> <span m="273700">should</span> <span m="273880">that</span>
  <span m="274120">f</span> <span m="274330">of</span> <span m="274450">t</span> <span
  m="274690">look</span> <span m="274900">like?</span> <span m="275240">What</span>
  <span m="275260">should</span> <span m="275410">that</span> <span m="275530">density</span>
  <span m="276010">function</span> <span m="276340">look</span> <span m="276520">like?</span>
  <span m="278070">And</span> <span m="278925">what</span> <span m="279290">I'm</span>
  <span m="279610">showing</span> <span m="279820">you</span> <span m="279910">here</span>
  <span m="280420">is</span> <span m="280630">a</span> <span m="280690">table</span>
  <span m="281110">of</span> <span m="281170">some</span> <span m="281350">very</span>
  <span m="281560">commonly</span> <span m="282040">used</span> <span m="282250">density</span>
  <span m="282610">functions.</span> <span m="283990">What</span> <span m="284140">you</span>
  <span m="284230">see</span> <span m="284560">in</span> <span m="284650">these</span>
  <span m="284890">two</span> <span m="285100">columns--</span> <span m="286060">on</span>
  <span m="286450">the</span> <span m="286600">right</span> <span m="286840">hand</span>
  <span m="286990">column</span> <span m="287380">is</span> <span m="287470">the</span>
  <span m="287560">density</span> <span m="287890">function</span> <span m="288190">f</span>
  <span m="288370">of</span> <span m="288490">t</span> <span m="288670">itself.</span>
  <span m="289600">Lambda</span> <span m="290020">denotes</span> <span m="290400">some</span>
  <span m="290680">parameter</span> <span m="291280">of</span> <span m="291400">the</span>
  <span m="291490">model.</span> <span m="292180">t</span> <span m="292510">is</span>
  <span m="293080">the</span> <span m="293200">time.</span></p><p><span m="294520">And</span>
  <span m="294970">on</span> <span m="295120">this</span> <span m="295660">second</span>
  <span m="296080">middle</span> <span m="296350">column</span> <span m="296890">is</span>
  <span m="297010">the</span> <span m="297080">survival</span> <span m="297490">function.</span>
  <span m="297940">So</span> <span m="298060">this</span> <span m="298270">is</span>
  <span m="298780">obtained</span> <span m="299530">for</span> <span m="299770">these</span>
  <span m="300100">particular</span> <span m="300580">parametric</span> <span m="301030">forms</span>
  <span m="301510">by</span> <span m="302050">an</span> <span m="302500">analytical</span>
  <span m="303370">solution</span> <span m="304900">solving</span> <span m="305350">that</span>
  <span m="305470">integral</span> <span m="306250">from</span> <span m="306520">t</span>
  <span m="306790">to</span> <span m="307210">infinity.</span> <span m="308320">This</span>
  <span m="308500">is</span> <span m="308620">the</span> <span m="308740">analytic</span>
  <span m="309190">solution</span> <span m="309580">for</span> <span m="309730">that.</span>
  <span m="311090">And</span> <span m="311190">so</span> <span m="311320">these</span>
  <span m="311500">go</span> <span m="311610">by</span> <span m="311890">common</span>
  <span m="312190">names</span> <span m="312550">of</span> <span m="312640">exponential,</span>
  <span m="313600">weeble,</span> <span m="314190">log-normal,</span> <span m="315040">and</span>
  <span m="315130">so</span> <span m="315370">on.</span> <span m="315880">And</span>
  <span m="315970">critically,</span> <span m="316450">all</span> <span m="316630">of</span>
  <span m="316720">these</span> <span m="316960">have</span> <span m="317080">support</span>
  <span m="317560">only</span> <span m="317950">on</span> <span m="318130">the</span>
  <span m="318220">positive</span> <span m="319060">real</span> <span m="319300">numbers,</span>
  <span m="320200">because</span> <span m="320530">the</span> <span m="320590">event</span>
  <span m="320890">can</span> <span m="321010">ever</span> <span m="321220">occur</span>
  <span m="321430">at</span> <span m="321520">negative</span> <span m="321880">time.</span></p><p><span
  m="324690">Now,</span> <span m="326160">we</span> <span m="326550">live</span> <span
  m="326760">in</span> <span m="326880">a</span> <span m="326940">day</span> <span
  m="327180">and</span> <span m="327270">age</span> <span m="327630">where</span>
  <span m="327900">we</span> <span m="328020">no</span> <span m="328200">longer</span>
  <span m="328500">have</span> <span m="328710">to</span> <span m="328830">make</span>
  <span m="329910">standard</span> <span m="330900">parametric</span> <span m="331620">assumptions</span>
  <span m="332340">for</span> <span m="332970">densities.</span> <span m="333600">We</span>
  <span m="333750">could,</span> <span m="333970">for</span> <span m="333990">example,</span>
  <span m="335490">try</span> <span m="335700">to</span> <span m="335790">formalize</span>
  <span m="336420">the</span> <span m="336540">density</span> <span m="336990">as</span>
  <span m="337140">some</span> <span m="337680">output</span> <span m="338160">of</span>
  <span m="338400">some</span> <span m="338850">deep</span> <span m="339060">neural</span>
  <span m="339230">network.</span> <span m="341110">But</span> <span m="342500">if</span>
  <span m="342920">we</span> <span m="343100">don't</span> <span m="343370">use</span>
  <span m="343640">a</span> <span m="343700">parametric</span> <span m="344360">approach,</span>
  <span m="344880">so</span> <span m="345230">there</span> <span m="345350">are</span>
  <span m="345380">two</span> <span m="345590">ways</span> <span m="345800">to</span>
  <span m="345890">try</span> <span m="346010">to</span> <span m="346100">do</span>
  <span m="346220">that.</span> <span m="346500">One</span> <span m="346640">way</span>
  <span m="346760">to</span> <span m="346850">do</span> <span m="346970">that</span>
  <span m="347150">would</span> <span m="347270">be</span> <span m="347360">to</span>
  <span m="347450">say</span> <span m="347870">that</span> <span m="348290">we're</span>
  <span m="348470">going</span> <span m="348710">to</span> <span m="349070">model</span>
  <span m="349490">the</span> <span m="349580">post--</span> <span m="350120">the</span>
  <span m="350870">distribution,</span> <span m="351680">f</span> <span m="351890">of</span>
  <span m="351970">t,</span> <span m="352730">as</span> <span m="353030">one</span>
  <span m="353300">of</span> <span m="353450">these</span> <span m="353930">things,</span>
  <span m="355040">where</span> <span m="355700">lambda</span> <span m="356660">or</span>
  <span m="357230">whatever</span> <span m="357470">the</span> <span m="357560">parameters</span>
  <span m="357980">of</span> <span m="358050">distribution</span> <span m="358640">are</span>
  <span m="358730">given</span> <span m="359000">to</span> <span m="359210">by</span>
  <span m="359360">the</span> <span m="359510">output</span> <span m="360080">of,</span>
  <span m="360260">let's</span> <span m="360470">say,</span> <span m="361120">a</span>
  <span m="361220">deep</span> <span m="361390">neural</span> <span m="361530">network</span>
  <span m="361910">on</span> <span m="362630">the</span> <span m="362720">covariate</span>
  <span m="363260">x.</span> <span m="363890">So</span> <span m="363980">that</span>
  <span m="364100">would</span> <span m="364190">be</span> <span m="364280">one</span>
  <span m="364490">approach.</span></p><p><span m="365770">A</span> <span m="365870">very</span>
  <span m="365960">different</span> <span m="366260">approach</span> <span m="366530">would</span>
  <span m="366620">be</span> <span m="366830">a</span> <span m="366920">non-parametric</span>
  <span m="367790">distribution</span> <span m="368480">where</span> <span m="368630">you</span>
  <span m="368720">say,</span> <span m="369000">OK,</span> <span m="369980">I'm</span>
  <span m="370130">going</span> <span m="370340">to</span> <span m="370580">define</span>
  <span m="370970">f</span> <span m="371110">of</span> <span m="371190">t</span> <span
  m="371370">extremely</span> <span m="371690">flexibly,</span> <span m="372200">not</span>
  <span m="372950">as</span> <span m="373280">one</span> <span m="373490">of</span>
  <span m="373610">these</span> <span m="373910">forms.</span> <span m="375980">And</span>
  <span m="376160">there</span> <span m="376790">one</span> <span m="377000">runs</span>
  <span m="377180">into</span> <span m="377390">a</span> <span m="377420">slightly</span>
  <span m="377690">different</span> <span m="377930">challenge,</span> <span m="378500">because</span>
  <span m="378770">as</span> <span m="378890">I'll</span> <span m="378980">show</span>
  <span m="379160">you</span> <span m="379340">in the</span> <span m="379400">next</span>
  <span m="379610">slide,</span> <span m="380720">to</span> <span m="380900">do</span>
  <span m="381200">maximum</span> <span m="381620">likelihood</span> <span m="382010">estimation</span>
  <span m="382520">of</span> <span m="382580">these</span> <span m="382730">distributions</span>
  <span m="383420">from</span> <span m="383570">censor</span> <span m="384080">data,</span>
  <span m="384860">one</span> <span m="385160">needs</span> <span m="385550">to</span>
  <span m="385700">get--</span> <span m="386150">one</span> <span m="386390">needs</span>
  <span m="386600">to</span> <span m="386690">make</span> <span m="386870">use</span>
  <span m="387080">of</span> <span m="387140">this</span> <span m="387250">survival</span>
  <span m="387680">function,</span> <span m="388160">s</span> <span m="388310">of</span>
  <span m="388430">t.</span></p><p><span m="389820">And</span> <span m="389940">so</span>
  <span m="390210">if</span> <span m="390390">you're</span> <span m="390630">f</span>
  <span m="390940">if</span> <span m="391050">t</span> <span m="392070">is</span>
  <span m="392230">complex,</span> <span m="393060">and</span> <span m="393180">you</span>
  <span m="393270">don't</span> <span m="393540">have</span> <span m="393990">a</span>
  <span m="394110">nice</span> <span m="394500">analytic</span> <span m="395130">solution</span>
  <span m="395790">for</span> <span m="396090">s</span> <span m="396360">of</span>
  <span m="396480">t,</span> <span m="397560">then</span> <span m="397680">you're</span>
  <span m="397760">going</span> <span m="397860">to</span> <span m="397980">have</span>
  <span m="398160">to</span> <span m="398250">somehow</span> <span m="398610">use</span>
  <span m="398820">a</span> <span m="398910">numerical</span> <span m="399450">approximation</span>
  <span m="400080">of</span> <span m="400140">s</span> <span m="400280">of</span>
  <span m="400380">t</span> <span m="400530">during</span> <span m="400770">limiting.</span>
  <span m="401400">So</span> <span m="401550">it's</span> <span m="401670">definitely</span>
  <span m="402030">possible,</span> <span m="402630">but</span> <span m="402810">it's</span>
  <span m="402990">going</span> <span m="403200">to</span> <span m="403290">be</span>
  <span m="403350">a</span> <span m="403380">little</span> <span m="403500">bit</span>
  <span m="403620">more</span> <span m="403770">effort.</span> <span m="406730">So</span>
  <span m="406910">now</span> <span m="407270">here's</span> <span m="407540">where</span>
  <span m="407630">I'm</span> <span m="407750">going</span> <span m="407900">to</span>
  <span m="407990">get</span> <span m="408110">into</span> <span m="408350">maximum</span>
  <span m="408740">likelihood</span> <span m="409010">estimation</span> <span m="409580">of</span>
  <span m="409670">these</span> <span m="409850">distributions,</span> <span m="411530">and</span>
  <span m="411650">to</span> <span m="411740">define</span> <span m="412220">for</span>
  <span m="412400">you</span> <span m="412610">the</span> <span m="413000">likelihood</span>
  <span m="413540">function,</span> <span m="414350">I'm</span> <span m="414470">going</span>
  <span m="414590">to</span> <span m="414710">break</span> <span m="414950">it</span>
  <span m="415010">down</span> <span m="415280">into</span> <span m="415430">two</span>
  <span m="415640">different</span> <span m="416000">settings.</span> <span m="417150">The</span>
  <span m="417250">first</span> <span m="417440">setting</span> <span m="417920">is</span>
  <span m="418070">an</span> <span m="418160">observation</span> <span m="419300">which</span>
  <span m="419810">is</span> <span m="420200">uncensored,</span> <span m="420950">meaning</span>
  <span m="421460">we</span> <span m="421640">do</span> <span m="421910">observe</span>
  <span m="422360">when</span> <span m="422600">the</span> <span m="422720">event--</span>
  <span m="423530">death,</span> <span m="423860">for</span> <span m="423950">example--</span>
  <span m="424530">occurs.</span> <span m="425710">And</span> <span m="425810">in</span>
  <span m="425900">that</span> <span m="426050">case,</span> <span m="427260">the</span>
  <span m="427400">probability</span> <span m="428150">of</span> <span m="428300">the</span>
  <span m="428360">event--</span> <span m="428720">it's</span> <span m="428840">very</span>
  <span m="429020">simple.</span> <span m="429450">It's</span> <span m="429500">just</span>
  <span m="430130">probability</span> <span m="430770">of</span> <span m="431630">the</span>
  <span m="431750">event</span> <span m="431960">occurring</span> <span m="432230">at</span>
  <span m="432470">capital--</span> <span m="433345">at</span> <span m="433610">capital</span>
  <span m="433940">T,</span> <span m="434240">random</span> <span m="434480">variable</span>
  <span m="434720">T,</span> <span m="434930">equals</span> <span m="435230">a</span>
  <span m="435250">little</span> <span m="435440">t--</span> <span m="435620">is</span>
  <span m="435740">just</span> <span m="436480">f or t.</span> <span m="436770">Done.</span></p><p><span
  m="439600">However,</span> <span m="439840">what</span> <span m="440080">happens</span>
  <span m="440890">if,</span> <span m="441280">for</span> <span m="441520">this</span>
  <span m="441760">data</span> <span m="442060">point,</span> <span m="442870">you</span>
  <span m="442990">don't</span> <span m="443290">observe</span> <span m="443950">when</span>
  <span m="444130">the</span> <span m="444220">event</span> <span m="444460">occurred</span>
  <span m="444760">because</span> <span m="445030">of</span> <span m="445090">censoring?</span>
  <span m="446650">Well,</span> <span m="446740">of</span> <span m="446800">course,</span>
  <span m="447200">you</span> <span m="447220">could</span> <span m="447520">just</span>
  <span m="447820">throw</span> <span m="448150">away</span> <span m="449050">that</span>
  <span m="449230">data</span> <span m="449470">point,</span> <span m="450120">not</span>
  <span m="450450">use</span> <span m="450670">it</span> <span m="450740">in</span>
  <span m="450850">your</span> <span m="450970">estimation,</span> <span m="452080">but</span>
  <span m="452230">that's</span> <span m="452380">precisely</span> <span m="453010">what</span>
  <span m="453130">we</span> <span m="453250">mentioned</span> <span m="453820">at</span>
  <span m="453910">the</span> <span m="453970">very</span> <span m="454210">beginning</span>
  <span m="454930">of</span> <span m="455350">last</span> <span m="455680">week's</span>
  <span m="455890">lecture--</span> <span m="456310">was</span> <span m="456520">the</span>
  <span m="456640">goal</span> <span m="456910">of</span> <span m="457000">survival</span>
  <span m="457480">modeling</span> <span m="458710">to</span> <span m="458830">not</span>
  <span m="459070">do</span> <span m="459220">that,</span> <span m="459460">because</span>
  <span m="459700">if we</span> <span m="459850">did</span> <span m="460000">that,</span>
  <span m="460180">it would</span> <span m="460270">introduce</span> <span m="461050">bias</span>
  <span m="461710">into</span> <span m="462610">our</span> <span m="462730">estimation</span>
  <span m="463240">procedure.</span></p><p><span m="464440">So</span> <span m="464830">we</span>
  <span m="464980">would</span> <span m="465100">like</span> <span m="465430">to</span>
  <span m="465580">be</span> <span m="465670">able</span> <span m="465850">to</span>
  <span m="466000">use</span> <span m="466450">that</span> <span m="466630">observation</span>
  <span m="468110">that</span> <span m="468530">this</span> <span m="468880">data</span>
  <span m="469120">point</span> <span m="469270">was</span> <span m="469450">censored,</span>
  <span m="470770">but</span> <span m="471070">the</span> <span m="471220">only</span>
  <span m="471520">information</span> <span m="471940">we</span> <span m="472000">can</span>
  <span m="472180">get</span> <span m="472480">from</span> <span m="472660">that</span>
  <span m="472780">observation</span> <span m="473530">is</span> <span m="473710">that</span>
  <span m="473980">capital</span> <span m="474357">T,</span> <span m="475490">the</span>
  <span m="475650">event</span> <span m="475930">time,</span> <span m="477040">must</span>
  <span m="477280">have</span> <span m="477400">occurred</span> <span m="477790">some</span>
  <span m="478360">time</span> <span m="479170">larger</span> <span m="480490">than</span>
  <span m="481060">the</span> <span m="481210">observed--</span> <span m="481690">the</span>
  <span m="481930">time</span> <span m="482200">of</span> <span m="482290">censoring,</span>
  <span m="482890">which</span> <span m="483040">is</span> <span m="483160">little</span>
  <span m="483400">t</span> <span m="483700">here.</span> <span m="485410">So</span>
  <span m="486580">we</span> <span m="486760">don't</span> <span m="486970">know</span>
  <span m="487120">precisely</span> <span m="487600">when</span> <span m="487960">capital</span>
  <span m="488350">T</span> <span m="488590">was,</span> <span m="488860">but</span>
  <span m="489010">we</span> <span m="489130">know</span> <span m="489340">it's</span>
  <span m="489460">something</span> <span m="489940">larger</span> <span m="490630">than</span>
  <span m="491050">the</span> <span m="491380">observed</span> <span m="491860">centering</span>
  <span m="492280">time</span> <span m="492560">little of</span> <span m="492850">t.</span></p><p><span
  m="493660">And</span> <span m="493780">that,</span> <span m="494140">remember,</span>
  <span m="494560">is</span> <span m="494680">precisely</span> <span m="495460">what</span>
  <span m="495760">the</span> <span m="495970">survival</span> <span m="496780">function</span>
  <span m="497830">is</span> <span m="497950">capturing.</span> <span m="499000">So</span>
  <span m="499180">for</span> <span m="499300">a</span> <span m="499360">censored</span>
  <span m="499990">observation,</span> <span m="500560">we're</span> <span m="500680">going</span>
  <span m="500890">to</span> <span m="500980">use</span> <span m="501310">capital</span>
  <span m="501790">S</span> <span m="502030">of</span> <span m="502180">t</span> <span
  m="502810">within</span> <span m="503140">the</span> <span m="503440">likelihood.</span>
  <span m="504580">So</span> <span m="504670">now</span> <span m="504820">we</span>
  <span m="504910">can</span> <span m="505030">then</span> <span m="505150">combine</span>
  <span m="505510">these</span> <span m="505660">two</span> <span m="505840">for</span>
  <span m="506000">censored</span> <span m="506370">and</span> <span m="506470">uncensored</span>
  <span m="506920">data,</span> <span m="507670">and</span> <span m="507760">what</span>
  <span m="507850">we</span> <span m="507940">get</span> <span m="508120">is</span>
  <span m="508270">the</span> <span m="508360">following</span> <span m="509110">likelihood</span>
  <span m="509590">objective.</span></p><p><span m="510820">This</span> <span m="511000">is--</span>
  <span m="511090">I'm</span> <span m="511180">showing</span> <span m="511390">you</span>
  <span m="511480">here</span> <span m="511600">the</span> <span m="511720">log</span>
  <span m="512049">likelihood</span> <span m="512440">objective.</span> <span m="513880">Recall</span>
  <span m="514539">from</span> <span m="514870">last</span> <span m="515169">week</span>
  <span m="515480">that</span> <span m="516100">little</span> <span m="516400">b</span>
  <span m="516640">of</span> <span m="516789">i</span> <span m="517450">simply</span>
  <span m="517809">denotes</span> <span m="518320">is</span> <span m="518530">this</span>
  <span m="519159">observation</span> <span m="519730">censored</span> <span m="520179">or</span>
  <span m="520240">not?</span> <span m="520570">So</span> <span m="520809">if</span>
  <span m="521200">bi</span> <span m="521940">is</span> <span m="522150">1,</span>
  <span m="522510">it</span> <span m="522610">means</span> <span m="522880">the</span>
  <span m="522970">time</span> <span m="523240">that</span> <span m="523360">you're</span>
  <span m="523480">given</span> <span m="524290">is</span> <span m="524590">the</span>
  <span m="524710">time</span> <span m="525100">of</span> <span m="525250">the</span>
  <span m="525340">censoring</span> <span m="526360">event.</span> <span m="527200">And</span>
  <span m="527320">if</span> <span m="527440">bi is</span> <span m="527800">0,</span>
  <span m="528450">it</span> <span m="528550">means</span> <span m="528760">the</span>
  <span m="528820">time</span> <span m="529120">you're</span> <span m="529240">given</span>
  <span m="529540">is</span> <span m="529630">the</span> <span m="529690">time</span>
  <span m="529960">that</span> <span m="530050">the</span> <span m="530140">event</span>
  <span m="530440">occurs.</span> <span m="532010">So</span> <span m="532090">here
  what</span> <span m="532290">we're</span> <span m="532410">going</span> <span m="532540">to</span>
  <span m="532660">do</span> <span m="532970">is</span> <span m="533170">now sum</span>
  <span m="533470">over all</span> <span m="533980">of</span> <span m="534070">the</span>
  <span m="534160">data</span> <span m="534370">points</span> <span m="534760">in</span>
  <span m="534880">your</span> <span m="534940">data</span> <span m="535120">set</span>
  <span m="535420">from</span> <span m="535660">little</span> <span m="536140">i</span>
  <span m="536320">equals</span> <span m="536590">1</span> <span m="536860">to</span>
  <span m="537560">little</span> <span m="537790">n</span> <span m="538550">of</span>
  <span m="538950">bi</span> <span m="540070">times</span> <span m="540670">log</span>
  <span m="541210">of</span> <span m="541300">probability</span> <span m="542500">under</span>
  <span m="543070">the</span> <span m="543220">censored</span> <span m="543910">model</span>
  <span m="544810">plus</span> <span m="545320">1</span> <span m="545620">minus</span>
  <span m="545920">bi</span> <span m="546340">times</span> <span m="546610">log of</span>
  <span m="546910">probability</span> <span m="547240">under</span> <span m="547450">the</span>
  <span m="547570">uncensored</span> <span m="548050">model.</span> <span m="548410">And</span>
  <span m="548500">so</span> <span m="548650">this</span> <span m="548800">bi</span>
  <span m="549060">is</span> <span m="549130">just</span> <span m="549220">going</span>
  <span m="549340">to</span> <span m="549400">switch</span> <span m="549730">on</span>
  <span m="549970">which</span> <span m="550180">of</span> <span m="550240">these</span>
  <span m="550390">two</span> <span m="550510">you're</span> <span m="550630">going</span>
  <span m="550710">to</span> <span m="550810">use</span> <span m="551020">for</span>
  <span m="551110">that</span> <span m="551230">given</span> <span m="551440">data</span>
  <span m="551650">point.</span></p><p><span m="552760">So</span> <span m="553330">the</span>
  <span m="553420">learning</span> <span m="553690">objective</span> <span m="554320">for</span>
  <span m="554620">maximum</span> <span m="554920">likelihood</span> <span m="555130">estimation</span>
  <span m="555550">here</span> <span m="555700">is</span> <span m="555850">very</span>
  <span m="556390">similar</span> <span m="556780">to</span> <span m="556900">what</span>
  <span m="557020">you're</span> <span m="557140">used</span> <span m="557440">to</span>
  <span m="558070">in</span> <span m="558730">learning</span> <span m="559300">distributions</span>
  <span m="560500">with</span> <span m="560710">the</span> <span m="560830">big</span>
  <span m="561040">difference</span> <span m="561640">that,</span> <span m="561970">for</span>
  <span m="562300">censored</span> <span m="562630">data,</span> <span m="563110">we're</span>
  <span m="563290">going</span> <span m="563470">to</span> <span m="563560">use</span>
  <span m="563800">the</span> <span m="563950">survival</span> <span m="564730">function</span>
  <span m="565780">to</span> <span m="565930">estimate</span> <span m="566380">its</span>
  <span m="567700">probability.</span> <span m="569080">Are</span> <span m="569110">there</span>
  <span m="569200">any</span> <span m="569320">questions?</span> <span m="575150">And</span>
  <span m="575410">this,</span> <span m="575560">of</span> <span m="575650">course,</span>
  <span m="575980">could</span> <span m="576220">then</span> <span m="576490">be</span>
  <span m="577270">optimized</span> <span m="578050">via</span> <span m="578350">your</span>
  <span m="578470">favorite</span> <span m="578830">algorithm,</span> <span m="579760">whether</span>
  <span m="580030">it</span> <span m="580090">be</span> <span m="580750">stochastic</span>
  <span m="581260">gradient</span> <span m="581590">descent,</span> <span m="582400">or</span>
  <span m="582700">second</span> <span m="583060">order</span> <span m="583240">method,</span>
  <span m="583570">and</span> <span m="583690">so</span> <span m="583840">on.</span>
  <span m="584260">Yep?</span></p><p><span m="584420">AUDIENCE:</span> <span m="584611">I</span>
  <span m="584803">have a question</span> <span m="585186">about the</span> <span
  m="585570">a</span> <span m="585720">kind of</span> <span m="585850">side project.</span>
  <span m="586130">You mentioned</span> <span m="586603">that we could</span> <span
  m="587076">use</span> <span m="587549">[INAUDIBLE].</span></p><p><span m="588970">DAVID
  SONTAG:</span> <span m="589170">Yes.</span></p><p><span m="589370">AUDIENCE:</span>
  <span m="589510">And</span> <span m="589650">then combine it with</span> <span m="590093">the</span>
  <span m="590536">parametric</span> <span m="590980">approach.</span></p><p><span
  m="591310">DAVID SONTAG:</span> <span m="591520">Yes.</span></p><p><span m="591730">AUDIENCE:</span>
  <span m="591800">So</span> <span m="591870">is</span> <span m="591940">that</span>
  <span m="592020">true</span> <span m="592210">that</span> <span m="592390">we</span>
  <span m="592540">just</span> <span m="592930">still</span> <span m="593430">have
  the</span> <span m="593930">parametric</span> <span m="594430">assumption</span>
  <span m="594910">that</span> <span m="595060">we</span> <span m="595180">kind</span>
  <span m="595330">of</span> <span m="595390">map</span> <span m="595705">the input</span>
  <span m="596020">to the</span> <span m="596200">parameters?</span></p><p><span m="597250">DAVID
  SONTAG:</span> <span m="597325">Exactly.</span> <span m="598420">That's</span> <span
  m="598600">exactly</span> <span m="598930">right.</span> <span m="599260">So</span>
  <span m="600640">consider</span> <span m="601120">the</span> <span m="601210">following</span>
  <span m="601600">picture</span> <span m="603690">where</span> <span m="604260">for--</span>
  <span m="604980">this</span> <span m="605180">is</span> <span m="605280">time,</span>
  <span m="608020">t.</span> <span m="608500">And</span> <span m="608620">this</span>
  <span m="608830">is</span> <span m="609070">f</span> <span m="609400">of t.</span>
  <span m="611812">You</span> <span m="612310">can</span> <span m="612400">imagine</span>
  <span m="612670">for</span> <span m="612790">any</span> <span m="612940">one</span>
  <span m="613120">patient</span> <span m="613670">you</span> <span m="613770">might</span>
  <span m="613810">have</span> <span m="613960">a</span> <span m="614020">different</span>
  <span m="615400">function.</span> <span m="615910">You</span> <span m="615970">might--</span>
  <span m="616240">but</span> <span m="616420">they</span> <span m="616540">might</span>
  <span m="616690">all</span> <span m="616840">be</span> <span m="616960">of</span>
  <span m="617050">the</span> <span m="617140">same</span> <span m="617650">parametric</span>
  <span m="618160">form.</span> <span m="618490">So</span> <span m="618610">they</span>
  <span m="618670">might</span> <span m="618820">be</span> <span m="618970">like</span>
  <span m="620500">that,</span> <span m="620950">or</span> <span m="621040">maybe</span>
  <span m="621340">they're</span> <span m="621490">shifted</span> <span m="621910">a</span>
  <span m="621970">little</span> <span m="622120">bit.</span> <span m="625130">So</span>
  <span m="625510">you</span> <span m="625780">think</span> <span m="626020">about</span>
  <span m="626230">each</span> <span m="626500">of</span> <span m="626620">these</span>
  <span m="626830">three</span> <span m="627070">things</span> <span m="627490">as</span>
  <span m="627640">being</span> <span m="628840">from</span> <span m="629080">the</span>
  <span m="629170">same</span> <span m="629650">parametric</span> <span m="630220">family
  of</span> <span m="630490">distributions,</span> <span m="631060">but</span> <span
  m="631180">with</span> <span m="631300">different</span> <span m="631690">means.</span></p><p><span
  m="633310">And</span> <span m="633560">in</span> <span m="633670">this</span> <span
  m="633850">case,</span> <span m="634150">then</span> <span m="634360">the</span>
  <span m="634450">mean</span> <span m="635230">is</span> <span m="635380">given</span>
  <span m="635650">to</span> <span m="635770">as</span> <span m="635880">the</span>
  <span m="635950">output</span> <span m="636340">of</span> <span m="636490">the</span>
  <span m="636760">deep</span> <span m="636940">neural</span> <span m="637090">network.</span>
  <span m="637750">And</span> <span m="637840">so</span> <span m="637930">that</span>
  <span m="638050">would</span> <span m="638200">be</span> <span m="638890">the</span>
  <span m="639010">way it</span> <span m="639140">would</span> <span m="639250">be</span>
  <span m="639340">used,</span> <span m="639520">and</span> <span m="639610">then</span>
  <span m="639700">one</span> <span m="639850">could</span> <span m="640000">just</span>
  <span m="640180">back</span> <span m="640720">propagate</span> <span m="641100">in</span>
  <span m="641170">the</span> <span m="641230">usual</span> <span m="641500">way</span>
  <span m="641680">to</span> <span m="641800">do</span> <span m="641920">learning.</span>
  <span m="643106">Yep?</span></p><p><span m="644022">AUDIENCE:</span> <span m="644251">Can
  you repeat what</span> <span m="644480">b sub i is?</span></p><p><span m="645400">DAVID
  SONTAG:</span> <span m="645525">Excuse</span> <span m="645650">me?</span></p><p><span
  m="645780">AUDIENCE:</span> <span m="645930">Could</span> <span m="646080">you repeat</span>
  <span m="646380">what</span> <span m="646735">b sub i is?</span></p><p><span m="647500">DAVID
  SONTAG:</span> <span m="647605">b</span> <span m="647710">sub</span> <span m="647890">i</span>
  <span m="648310">is</span> <span m="648670">just</span> <span m="649000">an</span>
  <span m="649120">indicator</span> <span m="649720">whether</span> <span m="649990">the</span>
  <span m="650140">i-th</span> <span m="650470">data</span> <span m="650740">point</span>
  <span m="650950">was</span> <span m="651070">censored</span> <span m="651640">or</span>
  <span m="651730">not</span> <span m="651940">censored.</span> <span m="654510">Yes?</span></p><p><span
  m="655020">AUDIENCE:</span> <span m="655125">So</span> <span m="655230">[INAUDIBLE]</span>
  <span m="656070">equal</span> <span m="656640">it's</span> <span m="656960">more</span>
  <span m="657540">a</span> <span m="658050">probability</span> <span m="658530">density</span>
  <span m="659200">function</span> <span m="659610">[INAUDIBLE].</span></p><p><span
  m="660420">DAVID SONTAG:</span> <span m="660630">Cumulative</span> <span m="660840">density</span>
  <span m="661140">function.</span></p><p><span m="661880">AUDIENCE:</span> <span
  m="661940">Yeah,</span> <span m="663030">but</span> <span m="663230">[INAUDIBLE]</span>
  <span m="665115">probability.</span> <span m="665750">No,</span> <span m="666340">for</span>
  <span m="666570">the</span> <span m="666740">[INAUDIBLE]</span> <span m="667300">it's</span>
  <span m="668580">probability</span> <span m="668970">density</span> <span m="669390">function.</span></p><p><span
  m="670350">DAVID SONTAG</span> <span m="670515">Yes,</span> <span m="670680">so</span>
  <span m="671360">just</span> <span m="671610">to--</span></p><p><span m="671820">AUDIENCE:</span>
  <span m="671930">[INAUDIBLE]</span></p><p><span m="673200">DAVID SONTAG:</span>
  <span m="673305">Excuse</span> <span m="673410">me?</span></p><p><span m="675310">AUDIENCE:</span>
  <span m="675480">Will</span> <span m="675650">that</span> <span m="675810">be</span>
  <span m="675960">any</span> <span m="676170">problem</span> <span m="676530">to</span>
  <span m="676620">combine</span> <span m="677070">those</span> <span m="677280">two</span>
  <span m="677430">types</span> <span m="677680">there?</span></p><p><span m="678440">DAVID
  SONTAG:</span> <span m="678520">That's</span> <span m="678600">a</span> <span m="678630">very</span>
  <span m="678780">good</span> <span m="678870">question.</span> <span m="679360">So</span>
  <span m="680210">the</span> <span m="680280">observation</span> <span m="680850">was</span>
  <span m="681120">that</span> <span m="681330">you</span> <span m="681450">have</span>
  <span m="683590">two</span> <span m="683860">different</span> <span m="684160">types</span>
  <span m="684550">of</span> <span m="685240">probabilities</span> <span m="685780">used</span>
  <span m="685990">here.</span> <span m="687790">In</span> <span m="688060">this</span>
  <span m="688210">case,</span> <span m="688390">we're</span> <span m="688570">using</span>
  <span m="688640">something</span> <span m="688870">like</span> <span m="688990">the</span>
  <span m="689080">cumulative</span> <span m="689390">density,</span> <span m="691300">whereas</span>
  <span m="691690">here</span> <span m="692020">we're</span> <span m="692200">using</span>
  <span m="693130">the</span> <span m="693460">probability</span> <span m="693970">density</span>
  <span m="694330">function.</span> <span m="695380">The</span> <span m="695470">question</span>
  <span m="695770">was,</span> <span m="696130">are</span> <span m="696310">these</span>
  <span m="696550">two</span> <span m="696730">on</span> <span m="696820">different</span>
  <span m="697090">scales?</span> <span m="698890">Does it</span> <span m="699100">make</span>
  <span m="699250">sense</span> <span m="699640">to</span> <span m="699760">combine</span>
  <span m="700270">them</span> <span m="700540">in</span> <span m="700630">this</span>
  <span m="700810">type</span> <span m="701050">of</span> <span m="701140">linear</span>
  <span m="701440">fashion</span> <span m="701890">with</span> <span m="702010">the</span>
  <span m="702070">same</span> <span m="702280">weighting?</span> <span m="703360">And</span>
  <span m="703930">I</span> <span m="704140">think</span> <span m="704350">it</span>
  <span m="704410">does</span> <span m="704620">make</span> <span m="704770">sense.</span></p><p><span
  m="705490">So</span> <span m="707320">think</span> <span m="707620">about</span>
  <span m="713900">a</span> <span m="714030">setting</span> <span m="714630">where</span>
  <span m="715140">you</span> <span m="715320">have</span> <span m="715920">a</span>
  <span m="718690">very</span> <span m="718770">small</span> <span m="719100">time</span>
  <span m="719430">range.</span> <span m="720210">You're</span> <span m="720300">not</span>
  <span m="720450">exactly</span> <span m="720870">sure</span> <span m="721110">when</span>
  <span m="721320">this</span> <span m="721470">event</span> <span m="721710">occurs.</span>
  <span m="722400">It's</span> <span m="722570">something</span> <span m="722830">in</span>
  <span m="722890">this</span> <span m="723030">time</span> <span m="723240">range.</span>
  <span m="726690">In</span> <span m="727110">the</span> <span m="727170">setting</span>
  <span m="727830">of</span> <span m="729480">the</span> <span m="729600">censored</span>
  <span m="730080">data,</span> <span m="730440">where</span> <span m="730590">that</span>
  <span m="730710">time</span> <span m="730950">range</span> <span m="731160">could</span>
  <span m="731280">potentially</span> <span m="731610">be</span> <span m="731700">very</span>
  <span m="732000">large,</span> <span m="734180">your</span> <span m="735030">model</span>
  <span m="735630">is</span> <span m="736950">providing--</span> <span m="741150">your</span>
  <span m="741330">log</span> <span m="741870">probability</span> <span m="742560">is</span>
  <span m="743100">somehow</span> <span m="743400">going</span> <span m="743670">to</span>
  <span m="743790">be</span> <span m="744270">much</span> <span m="744540">more</span>
  <span m="744720">flat,</span> <span m="747840">because</span> <span m="748170">you're</span>
  <span m="748530">covering</span> <span m="748830">much</span> <span m="749010">more</span>
  <span m="749100">probability</span> <span m="749460">mass.</span></p><p><span m="752930">And</span>
  <span m="753330">so</span> <span m="753780">that</span> <span m="753930">observation,</span>
  <span m="754620">I</span> <span m="754680">think,</span> <span m="754830">intuitively</span>
  <span m="755400">is</span> <span m="755730">likely</span> <span m="756030">to</span>
  <span m="756120">have</span> <span m="756360">a</span> <span m="756450">much--</span>
  <span m="757200">a</span> <span m="757590">bit</span> <span m="757740">of</span>
  <span m="757800">a</span> <span m="757860">smaller</span> <span m="758400">effect</span>
  <span m="759180">on</span> <span m="759540">the</span> <span m="759660">overall</span>
  <span m="760020">learning</span> <span m="760350">algorithm.</span> <span m="761640">These</span>
  <span m="761850">observations--</span> <span m="762840">you</span> <span m="763200">know</span>
  <span m="763320">precisely</span> <span m="763830">where</span> <span m="763950">they</span>
  <span m="764130">are,</span> <span m="764590">and</span> <span m="764610">so</span>
  <span m="765330">as</span> <span m="765540">you</span> <span m="765660">deviate</span>
  <span m="766200">from</span> <span m="766440">that,</span> <span m="768040">you</span>
  <span m="768450">incur</span> <span m="769170">the</span> <span m="769260">corresponding</span>
  <span m="769920">log</span> <span m="771280">loss</span> <span m="771720">penalty.</span>
  <span m="773740">But</span> <span m="774850">I</span> <span m="774930">do</span>
  <span m="775110">think</span> <span m="775380">that</span> <span m="775590">it</span>
  <span m="775680">makes</span> <span m="775860">sense</span> <span m="776070">to</span>
  <span m="776130">have</span> <span m="776250">them in</span> <span m="776340">the</span>
  <span m="776430">same</span> <span m="776610">scale.</span> <span m="777210">If</span>
  <span m="777750">anyone</span> <span m="778050">in</span> <span m="778110">the</span>
  <span m="778170">room</span> <span m="778620">has</span> <span m="778890">done</span>
  <span m="779190">work</span> <span m="779400">with</span> <span m="779680">[INAUDIBLE]</span>
  <span m="780150">modeling and</span> <span m="780450">has</span> <span m="780600">a</span>
  <span m="780630">different</span> <span m="780900">answer</span> <span m="781110">to</span>
  <span m="781200">that,</span> <span m="781380">I'd</span> <span m="781500">love</span>
  <span m="781680">to</span> <span m="781770">hear</span> <span m="782010">it.</span>
  <span m="786450">Not</span> <span m="786690">today,</span> <span m="787020">but</span>
  <span m="787140">maybe</span> <span m="787380">someone</span> <span m="787680">in</span>
  <span m="789090">the</span> <span m="789240">future</span> <span m="789510">will</span>
  <span m="789750">answer</span> <span m="790050">this</span> <span m="790170">question</span>
  <span m="790470">differently.</span></p><p><span m="791260">I'm</span> <span m="791360">going</span>
  <span m="791460">to</span> <span m="791560">move</span> <span m="791660">on</span>
  <span m="791670">for</span> <span m="791790">now.</span> <span m="794250">So</span>
  <span m="795450">the</span> <span m="795570">remaining</span> <span m="795960">question</span>
  <span m="797310">that</span> <span m="797550">I</span> <span m="797610">want</span>
  <span m="797820">to</span> <span m="797880">talk</span> <span m="798030">about</span>
  <span m="798150">today</span> <span m="798480">is</span> <span m="798630">how</span>
  <span m="798840">one</span> <span m="799950">evaluates</span> <span m="800790">survival</span>
  <span m="801240">models.</span> <span m="802020">So</span> <span m="804870">we</span>
  <span m="804990">talked</span> <span m="805290">about</span> <span m="805590">binary</span>
  <span m="806010">classification</span> <span m="806550">a</span> <span m="806610">lot</span>
  <span m="807240">in</span> <span m="807570">the</span> <span m="807630">context</span>
  <span m="808200">of</span> <span m="808470">risk</span> <span m="808700">stratification</span>
  <span m="809090">in</span> <span m="809160">the</span> <span m="809220">beginning,</span>
  <span m="809550">and</span> <span m="809640">we</span> <span m="809850">talked</span>
  <span m="810120">about</span> <span m="810300">how</span> <span m="810600">area</span>
  <span m="810930">under</span> <span m="811110">the</span> <span m="811200">ROC</span>
  <span m="811590">curve</span> <span m="811830">is</span> <span m="811950">one</span>
  <span m="812220">measure</span> <span m="812760">of</span> <span m="813130">classification</span>
  <span m="813660">performance,</span> <span m="814900">but</span> <span m="814980">here</span>
  <span m="815430">we're</span> <span m="815610">doing</span> <span m="816270">more--</span>
  <span m="816630">something</span> <span m="816900">more</span> <span m="817080">akin</span>
  <span m="817350">to</span> <span m="817470">regression,</span> <span m="818010">not</span>
  <span m="818190">classification.</span></p><p><span m="820120">A</span> <span m="820180">standard</span>
  <span m="820600">measure</span> <span m="820900">that's</span> <span m="821140">used</span>
  <span m="821590">to</span> <span m="821920">measure</span> <span m="822190">performance</span>
  <span m="823180">is</span> <span m="823330">known</span> <span m="823540">as</span>
  <span m="823720">the</span> <span m="823900">C-statistic,</span> <span m="825040">or</span>
  <span m="825160">concordance</span> <span m="825760">index.</span> <span m="826240">Those</span>
  <span m="826420">are</span> <span m="826480">one</span> <span m="826630">in</span>
  <span m="826690">the</span> <span m="826780">same--</span> <span m="828130">and</span>
  <span m="828490">is</span> <span m="828640">defined</span> <span m="829090">as</span>
  <span m="829240">follows.</span> <span m="829630">And it</span> <span m="829700">has</span>
  <span m="829840">a</span> <span m="829900">very</span> <span m="830410">intuitive</span>
  <span m="830920">definition.</span> <span m="832050">It</span> <span m="832510">sums</span>
  <span m="833110">over</span> <span m="834190">pairs</span> <span m="834640">of</span>
  <span m="834760">data</span> <span m="835000">points</span> <span m="835300">that</span>
  <span m="835540">can</span> <span m="835990">be</span> <span m="836170">compared</span>
  <span m="836590">to</span> <span m="836710">one</span> <span m="836890">another,</span>
  <span m="839120">and it</span> <span m="839310">says,</span> <span m="839830">OK,</span>
  <span m="843510">what</span> <span m="843780">is</span> <span m="843990">the</span>
  <span m="844170">likelihood</span> <span m="844860">of</span> <span m="845100">the</span>
  <span m="845340">event</span> <span m="845740">happening</span> <span m="847650">for</span>
  <span m="847890">an</span> <span m="847980">event</span> <span m="848400">that</span>
  <span m="848550">occurs</span> <span m="849150">before</span> <span m="850440">an</span>
  <span m="850530">event--</span> <span m="851100">another</span> <span m="851430">event.</span>
  <span m="851820">And</span> <span m="851910">what</span> <span m="852030">you</span>
  <span m="852120">want</span> <span m="852480">is</span> <span m="852630">that</span>
  <span m="853440">the</span> <span m="853650">likelihood</span> <span m="854160">of</span>
  <span m="854250">the</span> <span m="854340">event</span> <span m="855010">that,</span>
  <span m="856020">on</span> <span m="856560">average,</span> <span m="856950">in</span>
  <span m="857060">essence,</span> <span m="857280">should</span> <span m="857460">occur</span>
  <span m="857700">later</span> <span m="858060">should</span> <span m="858270">be</span>
  <span m="858780">larger</span> <span m="859200">than</span> <span m="859350">the</span>
  <span m="859410">event</span> <span m="859740">that</span> <span m="860010">should</span>
  <span m="860190">occur</span> <span m="860460">earlier.</span></p><p><span m="861420">I'm</span>
  <span m="861450">going</span> <span m="861600">to</span> <span m="861660">first</span>
  <span m="862200">illustrate</span> <span m="862560">it</span> <span m="862650">with</span>
  <span m="862740">this</span> <span m="862890">picture,</span> <span m="863340">and</span>
  <span m="863430">then</span> <span m="863520">I'll</span> <span m="863760">work</span>
  <span m="864030">through</span> <span m="864240">the</span> <span m="864330">math.</span>
  <span m="864810">So</span> <span m="864990">here's</span> <span m="865260">the</span>
  <span m="865350">picture,</span> <span m="865770">and</span> <span m="865860">then</span>
  <span m="866250">we'll</span> <span m="866340">talk</span> <span m="866490">about</span>
  <span m="866640">the</span> <span m="866700">math.</span> <span m="868510">So</span>
  <span m="868670">what</span> <span m="868760">I'm</span> <span m="868850">showing</span>
  <span m="869150">you</span> <span m="869240">here</span> <span m="869810">are</span>
  <span m="871160">every</span> <span m="871430">single</span> <span m="871700">observation</span>
  <span m="871960">in</span> <span m="872220">your</span> <span m="872430">data</span>
  <span m="872680">set,</span> <span m="873080">and</span> <span m="873170">they're</span>
  <span m="873320">sorted</span> <span m="874130">by</span> <span m="875090">either</span>
  <span m="875720">the</span> <span m="876350">censoring</span> <span m="877040">time</span>
  <span m="877640">or</span> <span m="877880">the</span> <span m="878030">event</span>
  <span m="878420">time.</span> <span m="880900">So</span> <span m="881530">by</span>
  <span m="881890">black,</span> <span m="883040">I'm</span> <span m="883270">illustrating</span>
  <span m="883840">uncensored</span> <span m="884410">data</span> <span m="884650">points.</span>
  <span m="885130">And</span> <span m="885280">by</span> <span m="885430">red,</span>
  <span m="886140">I'm</span> <span m="886310">denoting</span> <span m="887260">censored</span>
  <span m="887820">data</span> <span m="888070">points.</span></p><p><span m="890010">Now,</span>
  <span m="891080">here</span> <span m="891380">we</span> <span m="891500">see</span>
  <span m="891830">that</span> <span m="892610">this</span> <span m="892940">data</span>
  <span m="893210">point--</span> <span m="894140">the</span> <span m="894380">event</span>
  <span m="894830">happened</span> <span m="895550">before</span> <span m="896870">this</span>
  <span m="897200">data</span> <span m="897440">point's</span> <span m="897770">censoring</span>
  <span m="898310">event.</span> <span m="898880">Now,</span> <span m="899060">since</span>
  <span m="899210">this</span> <span m="899320">data point</span> <span m="899580">was</span>
  <span m="899710">censored,</span> <span m="900260">it</span> <span m="900350">means</span>
  <span m="900530">it's</span> <span m="900860">true</span> <span m="901250">event</span>
  <span m="901610">time</span> <span m="902330">you</span> <span m="902420">could</span>
  <span m="902540">think</span> <span m="902720">about</span> <span m="902960">as</span>
  <span m="903030">sometime</span> <span m="903650">into</span> <span m="903830">the</span>
  <span m="903920">far</span> <span m="904190">future.</span> <span m="905700">So</span>
  <span m="905720">what</span> <span m="905870">we</span> <span m="905950">would</span>
  <span m="906080">want</span> <span m="906710">is</span> <span m="906950">that</span>
  <span m="908060">the</span> <span m="910100">model</span> <span m="911330">gives</span>
  <span m="911810">that</span> <span m="912050">the</span> <span m="912200">probability</span>
  <span m="912980">that</span> <span m="913400">this</span> <span m="914000">event</span>
  <span m="914720">happens</span> <span m="916610">by</span> <span m="917780">this</span>
  <span m="918260">time</span> <span m="920050">should</span> <span m="920530">be</span>
  <span m="921880">larger</span> <span m="923140">than</span> <span m="923260">the</span>
  <span m="923320">probability</span> <span m="924010">that</span> <span m="924340">this</span>
  <span m="924940">event</span> <span m="925300">happens</span> <span m="925990">by</span>
  <span m="926350">this</span> <span m="926740">time,</span> <span m="929190">because</span>
  <span m="929460">this</span> <span m="929610">actually</span> <span m="929970">occurred</span>
  <span m="930270">first.</span> <span m="931320">And</span> <span m="931440">these</span>
  <span m="931680">two</span> <span m="931800">are</span> <span m="931860">comparable</span>
  <span m="932330">together--</span> <span m="932790">to</span> <span m="932910">each</span>
  <span m="933030">other.</span></p><p><span m="934060">On</span> <span m="934160">the</span>
  <span m="934260">other</span> <span m="934360">hand,</span> <span m="934630">it</span>
  <span m="934730">wouldn't</span> <span m="935040">make</span> <span m="935250">sense</span>
  <span m="935550">to</span> <span m="935670">compare</span> <span m="936600">y2</span>
  <span m="937350">and</span> <span m="937470">y4,</span> <span m="938550">because</span>
  <span m="938850">both</span> <span m="939180">of</span> <span m="939270">these</span>
  <span m="939450">were</span> <span m="939570">censored</span> <span m="940410">data</span>
  <span m="940680">points, and</span> <span m="941120">we</span> <span m="941160">don't</span>
  <span m="941430">know</span> <span m="941610">precisely</span> <span m="942120">when</span>
  <span m="942450">they</span> <span m="942630">occurred.</span> <span m="943300">So</span>
  <span m="943380">for</span> <span m="943470">example,</span> <span m="943940">it</span>
  <span m="944040">could</span> <span m="944140">have</span> <span m="944330">very</span>
  <span m="944550">well</span> <span m="944670">happened</span> <span m="945090">that</span>
  <span m="945210">the</span> <span m="945300">event</span> <span m="945780">2</span>
  <span m="946500">happened</span> <span m="947280">after</span> <span m="947940">event</span>
  <span m="948300">4.</span> <span m="950280">So</span> <span m="950490">what</span>
  <span m="950640">I'm</span> <span m="950730">showing</span> <span m="951060">you</span>
  <span m="951150">here</span> <span m="951870">with</span> <span m="952080">each</span>
  <span m="952230">of</span> <span m="952290">these</span> <span m="952470">lines</span>
  <span m="953250">are</span> <span m="953370">the</span> <span m="953460">pairwise</span>
  <span m="953970">comparisons</span> <span m="954630">that</span> <span m="954750">are</span>
  <span m="954840">actually</span> <span m="955230">possible</span> <span m="955710">to</span>
  <span m="955830">make.</span> <span m="956700">You</span> <span m="956820">can</span>
  <span m="956940">make</span> <span m="957060">pairwise</span> <span m="957360">comparisons,</span>
  <span m="957840">of</span> <span m="957930">course,</span> <span m="958200">between</span>
  <span m="958470">any</span> <span m="958650">pair</span> <span m="958830">of</span>
  <span m="958920">events</span> <span m="959190">that</span> <span m="959310">actually</span>
  <span m="959610">did</span> <span m="959790">occur,</span> <span m="960730">and</span>
  <span m="960830">you</span> <span m="960930">can</span> <span m="961030">make</span>
  <span m="961130">pairwise</span> <span m="961350">comparisons</span> <span m="961860">between</span>
  <span m="962190">censored</span> <span m="962820">events</span> <span m="963330">and</span>
  <span m="963480">events</span> <span m="963810">that</span> <span m="963930">occurred</span>
  <span m="964590">before</span> <span m="965010">it.</span></p><p><span m="966690">Now,</span>
  <span m="966810">if</span> <span m="966900">you</span> <span m="966960">now</span>
  <span m="967110">look</span> <span m="967320">at</span> <span m="967410">this</span>
  <span m="967620">formula,</span> <span m="969350">the</span> <span m="969460">formula</span>
  <span m="970680">in</span> <span m="971080">this</span> <span m="971500">indicate--</span>
  <span m="972040">this</span> <span m="972220">is</span> <span m="972250">looking</span>
  <span m="972490">at</span> <span m="972610">an</span> <span m="972730">indicator</span>
  <span m="973870">of</span> <span m="974470">survival</span> <span m="975100">functions</span>
  <span m="975610">between</span> <span m="976060">pairs</span> <span m="976570">of</span>
  <span m="976660">data</span> <span m="976900">points,</span> <span m="977350">and</span>
  <span m="977470">which</span> <span m="977680">pairs</span> <span m="977950">of</span>
  <span m="978010">data</span> <span m="978220">points?</span> <span m="978580">It</span>
  <span m="978840">was</span> <span m="979030">precisely</span> <span m="979570">those</span>
  <span m="979780">pairs</span> <span m="980050">of</span> <span m="980140">data</span>
  <span m="980350">points,</span> <span m="981170">which</span> <span m="981280">I'm</span>
  <span m="981430">showing</span> <span m="982210">comparisons</span> <span m="983020">of</span>
  <span m="983200">with</span> <span m="983380">these</span> <span m="983530">blue</span>
  <span m="983710">lines</span> <span m="984040">here.</span></p><p><span m="984700">So</span>
  <span m="984790">we're</span> <span m="984880">going</span> <span m="984950">to</span>
  <span m="985040">sum</span> <span m="985600">over</span> <span m="986430">i</span>
  <span m="986880">such</span> <span m="987100">that</span> <span m="987350">bi is</span>
  <span m="987610">equal</span> <span m="987790">to</span> <span m="987880">0,</span>
  <span m="988210">and</span> <span m="988450">remember</span> <span m="988750">that</span>
  <span m="988900">means</span> <span m="989290">it</span> <span m="989500">is</span>
  <span m="989770">an</span> <span m="990430">uncensored</span> <span m="991600">data</span>
  <span m="991840">point.</span> <span m="992830">And</span> <span m="992950">then</span>
  <span m="993100">we</span> <span m="993220">look</span> <span m="993520">at--</span>
  <span m="995650">we</span> <span m="995950">look</span> <span m="996310">at</span>
  <span m="996670">yi</span> <span m="997630">compared</span> <span m="998020">to</span>
  <span m="998320">all</span> <span m="998770">other</span> <span m="999790">yj</span>
  <span m="1000510">that's</span> <span m="1000720">great--</span> <span m="1001050">that</span>
  <span m="1001200">has</span> <span m="1001350">a</span> <span m="1001410">value</span>
  <span m="1001650">greater</span> <span m="1001890">than--</span> <span m="1002100">both</span>
  <span m="1002340">censored</span> <span m="1002760">and</span> <span m="1003030">uncensored.</span>
  <span m="1005520">Now,</span> <span m="1006120">if</span> <span m="1006390">your</span>
  <span m="1006570">data</span> <span m="1006990">had</span> <span m="1007590">no</span>
  <span m="1009120">sensor</span> <span m="1009990">data</span> <span m="1010320">points</span>
  <span m="1010680">in</span> <span m="1010830">it,</span> <span m="1011860">then</span>
  <span m="1013020">you</span> <span m="1013140">can</span> <span m="1013290">verify</span>
  <span m="1013860">that,</span> <span m="1014010">in</span> <span m="1014130">fact,</span>
  <span m="1014520">this</span> <span m="1014850">corresponds--</span> <span m="1016390">so</span>
  <span m="1016510">there's</span> <span m="1016650">one</span> <span m="1016800">other</span>
  <span m="1016980">assumption</span> <span m="1017150">one</span> <span m="1017240">has</span>
  <span m="1017460">to</span> <span m="1017520">make,</span> <span m="1018310">which</span>
  <span m="1018420">is</span> <span m="1018660">that--</span> <span m="1019610">suppose</span>
  <span m="1020150">that</span> <span m="1021420">your</span> <span m="1021780">outcome</span>
  <span m="1022200">is</span> <span m="1022320">binary.</span> <span m="1023110">And</span>
  <span m="1023130">so</span> <span m="1023250">if</span> <span m="1023340">you</span>
  <span m="1023430">might</span> <span m="1023640">wonder</span> <span m="1024119">how</span>
  <span m="1024280">you</span> <span m="1024359">get</span> <span m="1024480">a</span>
  <span m="1024540">binary</span> <span m="1024810">outcome</span> <span m="1025109">from</span>
  <span m="1025260">this,</span> <span m="1025560">imagine</span> <span m="1026069">that</span>
  <span m="1027750">your</span> <span m="1028710">density</span> <span m="1029130">function</span>
  <span m="1029760">looked</span> <span m="1030000">a</span> <span m="1030060">little</span>
  <span m="1030240">bit</span> <span m="1030390">like</span> <span m="1030630">this,</span>
  <span m="1031470">where</span> <span m="1031950">it</span> <span m="1032040">could</span>
  <span m="1032190">occur</span> <span m="1032730">either</span> <span m="1033359">at</span>
  <span m="1033750">time</span> <span m="1036390">1</span> <span m="1037140">or</span>
  <span m="1037319">time</span> <span m="1037650">2.</span> <span m="1038490">So</span>
  <span m="1039720">something</span> <span m="1040050">like</span> <span m="1040890">that.</span></p><p><span
  m="1044130">So</span> <span m="1044550">if</span> <span m="1046440">the</span> <span
  m="1046540">event</span> <span m="1046829">can</span> <span m="1046950">occur</span>
  <span m="1047220">at</span> <span m="1047369">only</span> <span m="1047640">two</span>
  <span m="1047880">times,</span> <span m="1049300">not</span> <span m="1050190">a</span>
  <span m="1050250">whole</span> <span m="1050430">range</span> <span m="1050670">of</span>
  <span m="1050730">times,</span> <span m="1051060">then</span> <span m="1051410">this</span>
  <span m="1051770">is</span> <span m="1051980">analogous</span> <span m="1052560">to</span>
  <span m="1052960">a</span> <span m="1053940">binary</span> <span m="1054540">outcome.</span>
  <span m="1055570">And</span> <span m="1055590">so</span> <span m="1055830">if</span>
  <span m="1055980">you</span> <span m="1056070">have</span> <span m="1056220">a</span>
  <span m="1056280">binary</span> <span m="1056820">outcome</span> <span m="1057210">like</span>
  <span m="1057450">this</span> <span m="1058200">and</span> <span m="1058410">no</span>
  <span m="1058620">censoring,</span> <span m="1059310">then,</span> <span m="1059430">in</span>
  <span m="1059520">fact,</span> <span m="1059820">that</span> <span m="1060000">C-statistic</span>
  <span m="1060630">is</span> <span m="1060720">exactly</span> <span m="1061350">equal</span>
  <span m="1061710">to</span> <span m="1061830">the</span> <span m="1061920">area</span>
  <span m="1062280">under</span> <span m="1062460">the</span> <span m="1062520">ROC</span>
  <span m="1062970">curve.</span> <span m="1063210">So</span> <span m="1063530">that</span>
  <span m="1063690">just</span> <span m="1063840">connects</span> <span m="1064110">it</span>
  <span m="1064200">a</span> <span m="1064230">little</span> <span m="1064350">bit</span>
  <span m="1064470">back</span> <span m="1064590">to</span> <span m="1064770">things</span>
  <span m="1064930">we're</span> <span m="1065010">used</span> <span m="1065220">to.</span>
  <span m="1065400">Yep?</span></p><p><span m="1065850">AUDIENCE:</span> <span m="1066000">Just</span>
  <span m="1066150">to</span> <span m="1066300">make</span> <span m="1066450">sure</span>
  <span m="1066690">that</span> <span m="1067000">I</span> <span m="1067310">understand.</span>
  <span m="1067470">So</span> <span m="1067765">y1</span> <span m="1068060">is</span>
  <span m="1068440">going</span> <span m="1068580">to be</span> <span m="1068980">we
  observed</span> <span m="1069720">an</span> <span m="1070070">event,</span> <span
  m="1070370">and</span> <span m="1070680">y2</span> <span m="1070870">is</span> <span
  m="1070990">going</span> <span m="1071140">to</span> <span m="1071260">be</span>
  <span m="1071520">we know</span> <span m="1071720">that</span> <span m="1072100">no</span>
  <span m="1072400">event</span> <span m="1073090">occurred</span> <span m="1073920">until</span>
  <span m="1074280">that</span> <span m="1074410">day?</span></p><p><span m="1075210">DAVID
  SONTAG:</span> <span m="1075330">Every</span> <span m="1075450">dot</span> <span
  m="1075720">corresponds</span> <span m="1076140">to</span> <span m="1076230">one</span>
  <span m="1076680">event,</span> <span m="1078320">either</span> <span m="1078560">censored</span>
  <span m="1078920">or</span> <span m="1078980">not.</span></p><p><span m="1079370">AUDIENCE:</span>
  <span m="1079486">Thank</span> <span m="1079602">you.</span></p><p><span m="1080070">DAVID
  SONTAG:</span> <span m="1080080">And</span> <span m="1080090">they're</span> <span
  m="1080180">sorted.</span> <span m="1080930">In</span> <span m="1081050">this</span>
  <span m="1081230">figure,</span> <span m="1081560">they're</span> <span m="1081710">sorted</span>
  <span m="1082190">by</span> <span m="1083120">the</span> <span m="1083390">time</span>
  <span m="1084110">of</span> <span m="1084980">either</span> <span m="1085460">the</span>
  <span m="1085580">censoring</span> <span m="1086450">or</span> <span m="1087080">the</span>
  <span m="1087260">event</span> <span m="1087530">occurring.</span> <span m="1094420">So</span>
  <span m="1095670">I</span> <span m="1095760">talked</span> <span m="1096030">to--</span>
  <span m="1096570">when</span> <span m="1096810">I</span> <span m="1096870">talked</span>
  <span m="1097050">about</span> <span m="1097200">C-statistic,</span> <span m="1097360">it--</span>
  <span m="1098190">that's</span> <span m="1098430">one</span> <span m="1098820">way</span>
  <span m="1099030">to</span> <span m="1099120">measure</span> <span m="1099420">performance</span>
  <span m="1100380">of</span> <span m="1101130">your</span> <span m="1101250">survival</span>
  <span m="1101730">modeling,</span> <span m="1102810">but</span> <span m="1103080">you</span>
  <span m="1103140">might</span> <span m="1103320">remember</span> <span m="1103770">that</span>
  <span m="1103890">I--</span> <span m="1104140">that</span> <span m="1104520">when</span>
  <span m="1104640">we</span> <span m="1104700">talked</span> <span m="1104880">about</span>
  <span m="1104950">binary</span> <span m="1105300">classification,</span> <span m="1105780">we</span>
  <span m="1105870">said</span> <span m="1106080">how</span> <span m="1106350">area</span>
  <span m="1106600">under</span> <span m="1106710">there</span> <span m="1106820">ROC</span>
  <span m="1107100">curve</span> <span m="1107310">in</span> <span m="1107400">itself</span>
  <span m="1107700">is</span> <span m="1107790">very</span> <span m="1107940">limiting,</span>
  <span m="1108820">and so</span> <span m="1108990">we</span> <span m="1109080">should</span>
  <span m="1109200">think</span> <span m="1109380">through</span> <span m="1109590">other</span>
  <span m="1109890">performance</span> <span m="1110340">metrics</span> <span m="1110730">of</span>
  <span m="1110820">relevance.</span></p><p><span m="1111210">So</span> <span m="1111420">here</span>
  <span m="1111610">are</span> <span m="1111630">a</span> <span m="1111660">few</span>
  <span m="1111870">other</span> <span m="1112020">things</span> <span m="1112200">that</span>
  <span m="1112290">you</span> <span m="1112380">could</span> <span m="1112590">do.</span>
  <span m="1114060">One</span> <span m="1114270">thing</span> <span m="1114390">you</span>
  <span m="1114450">could</span> <span m="1114630">do</span> <span m="1114780">is</span>
  <span m="1114870">you</span> <span m="1114960">could</span> <span m="1115110">use</span>
  <span m="1115950">the</span> <span m="1116220">mean</span> <span m="1116570">squared</span>
  <span m="1117030">error.</span> <span m="1118330">So</span> <span m="1118860">again,</span>
  <span m="1119260">thinking</span> <span m="1119550">about</span> <span m="1119700">this</span>
  <span m="1119850">as</span> <span m="1119970">a</span> <span m="1120000">regression</span>
  <span m="1120540">problem.</span> <span m="1121410">But</span> <span m="1121590">of</span>
  <span m="1121650">course,</span> <span m="1121860">that</span> <span m="1121980">only</span>
  <span m="1122190">makes</span> <span m="1122400">sense</span> <span m="1123090">for</span>
  <span m="1124320">uncensored</span> <span m="1124920">data</span> <span m="1125130">points.</span>
  <span m="1125430">So</span> <span m="1126310">focus</span> <span m="1126710">just</span>
  <span m="1126930">in</span> <span m="1127050">the</span> <span m="1127110">uncensored</span>
  <span m="1127590">data</span> <span m="1127760">points,</span> <span m="1128040">look</span>
  <span m="1128130">to</span> <span m="1128220">see</span> <span m="1128370">how</span>
  <span m="1128580">well</span> <span m="1128730">we're</span> <span m="1128850">doing</span>
  <span m="1129060">at</span> <span m="1129120">predicting</span> <span m="1129480">when</span>
  <span m="1129630">the</span> <span m="1129690">event</span> <span m="1129900">occurs.</span></p><p><span
  m="1131410">The</span> <span m="1131510">second</span> <span m="1131670">thing</span>
  <span m="1131880">one</span> <span m="1132060">could</span> <span m="1132210">do,</span>
  <span m="1132450">since</span> <span m="1133560">you</span> <span m="1133710">have</span>
  <span m="1134880">the</span> <span m="1134970">ability</span> <span m="1135270">to</span>
  <span m="1136110">define</span> <span m="1136770">the</span> <span m="1137010">likelihood</span>
  <span m="1137670">of</span> <span m="1137850">an</span> <span m="1137940">observation,</span>
  <span m="1138490">censored</span> <span m="1138960">or</span> <span m="1139050">not</span>
  <span m="1139290">censored,</span> <span m="1140220">one</span> <span m="1140400">could</span>
  <span m="1140550">hold</span> <span m="1140880">out</span> <span m="1141210">data,</span>
  <span m="1142260">and</span> <span m="1142380">look</span> <span m="1142560">at</span>
  <span m="1142710">the</span> <span m="1142950">held-out</span> <span m="1143870">likelihood</span>
  <span m="1144220">or</span> <span m="1144330">log</span> <span m="1144570">likelihood</span>
  <span m="1145080">of</span> <span m="1145410">that</span> <span m="1145720">held-out</span>
  <span m="1145920">data.</span> <span m="1147170">And</span> <span m="1147630">the</span>
  <span m="1147730">third</span> <span m="1147830">thing</span> <span m="1148010">you</span>
  <span m="1148130">could</span> <span m="1148280">do</span> <span m="1148580">is</span>
  <span m="1148760">you</span> <span m="1148910">can--</span> <span m="1149210">after</span>
  <span m="1149690">learning</span> <span m="1150710">using</span> <span m="1151160">this</span>
  <span m="1151490">survival</span> <span m="1151940">modeling</span> <span m="1152270">framework,</span>
  <span m="1153320">one</span> <span m="1153530">could</span> <span m="1153770">then</span>
  <span m="1154220">turn</span> <span m="1154640">it</span> <span m="1154850">into</span>
  <span m="1155510">a</span> <span m="1155840">binary</span> <span m="1156620">classification</span>
  <span m="1157250">problem</span> <span m="1157940">by,</span> <span m="1158120">for</span>
  <span m="1158240">example,</span> <span m="1158690">artificially</span> <span m="1159380">choosing</span>
  <span m="1160010">time</span> <span m="1160370">ranges,</span> <span m="1160820">like</span>
  <span m="1161000">greater</span> <span m="1161450">than</span> <span m="1162410">three</span>
  <span m="1162680">months</span> <span m="1163250">is</span> <span m="1163580">1.</span>
  <span m="1164060">Less</span> <span m="1164270">than</span> <span m="1164420">three</span>
  <span m="1164600">months</span> <span m="1164880">is</span> <span m="1164960">0.</span></p><p><span
  m="1165830">That</span> <span m="1165950">would</span> <span m="1166040">be</span>
  <span m="1166130">one</span> <span m="1166310">crude</span> <span m="1166580">definition.</span>
  <span m="1167460">And</span> <span m="1167790">then</span> <span m="1167930">once</span>
  <span m="1168110">you've</span> <span m="1168230">done</span> <span m="1168380">a</span>
  <span m="1168410">reduction</span> <span m="1169010">to</span> <span m="1169160">a</span>
  <span m="1169190">binary</span> <span m="1169490">classification</span> <span m="1170090">problem,</span>
  <span m="1170360">you</span> <span m="1170420">could</span> <span m="1170600">use</span>
  <span m="1171500">all</span> <span m="1171840">of</span> <span m="1171920">the</span>
  <span m="1172130">existing</span> <span m="1172640">performance</span> <span m="1173060">metrics</span>
  <span m="1173400">they're</span> <span m="1173480">used</span> <span m="1173720">to</span>
  <span m="1173810">thinking</span> <span m="1174170">about</span> <span m="1174380">for</span>
  <span m="1174500">binary</span> <span m="1174770">classification</span> <span m="1175430">to</span>
  <span m="1175730">evaluate</span> <span m="1176210">the</span> <span m="1176300">performance</span>
  <span m="1176750">there--</span> <span m="1177020">things</span> <span m="1177260">like</span>
  <span m="1177740">positive</span> <span m="1178130">predictive</span> <span m="1178460">value,</span>
  <span m="1178760">for</span> <span m="1178880">example.</span> <span m="1180550">And</span>
  <span m="1180650">you</span> <span m="1180740">could,</span> <span m="1180830">of</span>
  <span m="1180920">course,</span> <span m="1181130">choose</span> <span m="1181370">different</span>
  <span m="1182000">reductions</span> <span m="1182990">and</span> <span m="1183110">get</span>
  <span m="1183260">different</span> <span m="1183590">performance</span> <span m="1183920">statistics</span>
  <span m="1184340">out.</span> <span m="1184970">So</span> <span m="1185090">this</span>
  <span m="1185210">is</span> <span m="1185270">just</span> <span m="1185450">a</span>
  <span m="1185510">small</span> <span m="1186020">subset</span> <span m="1186530">of</span>
  <span m="1187310">ways</span> <span m="1187700">to</span> <span m="1187790">try</span>
  <span m="1187970">to</span> <span m="1188060">evaluate</span> <span m="1188460">survivor</span>
  <span m="1188990">modeling,</span> <span m="1189710">but</span> <span m="1189860">it's</span>
  <span m="1189950">a</span> <span m="1190010">very,</span> <span m="1190560">very</span>
  <span m="1190760">rich</span> <span m="1191210">literature.</span> <span m="1192260">And</span>
  <span m="1192410">again,</span> <span m="1192620">on</span> <span m="1192710">the</span>
  <span m="1192770">bottom</span> <span m="1193040">of</span> <span m="1193100">these</span>
  <span m="1193190">slides,</span> <span m="1193520">I</span> <span m="1193610">pointed</span>
  <span m="1193940">you to</span> <span m="1194060">several</span> <span m="1194360">references</span>
  <span m="1194930">that</span> <span m="1195050">you</span> <span m="1195140">could</span>
  <span m="1195290">go</span> <span m="1195470">to to</span> <span m="1195800">learn</span>
  <span m="1196010">more.</span></p><p><span m="1197640">The</span> <span m="1197760">final</span>
  <span m="1198240">comment</span> <span m="1198630">I</span> <span m="1198720">wanted</span>
  <span m="1198900">to</span> <span m="1198990">make</span> <span m="1199710">is</span>
  <span m="1199830">that</span> <span m="1200010">I</span> <span m="1200130">only</span>
  <span m="1200340">told</span> <span m="1200610">you</span> <span m="1200670">about</span>
  <span m="1200910">one</span> <span m="1201540">estimator</span> <span m="1202470">in</span>
  <span m="1202620">today's</span> <span m="1203040">lecture,</span> <span m="1203610">and</span>
  <span m="1203700">that's</span> <span m="1203910">known</span> <span m="1204150">as</span>
  <span m="1204930">the</span> <span m="1205080">likelihood</span> <span m="1205590">based</span>
  <span m="1205830">estimator.</span> <span m="1207030">But</span> <span m="1207240">there</span>
  <span m="1207290">is</span> <span m="1207420">a</span> <span m="1207450">whole</span>
  <span m="1207750">other</span> <span m="1208470">estimation</span> <span m="1209070">approach</span>
  <span m="1209460">for</span> <span m="1209580">survival</span> <span m="1209910">modelings,</span>
  <span m="1210360">which</span> <span m="1210480">is</span> <span m="1210570">very</span>
  <span m="1210750">important</span> <span m="1211080">to</span> <span m="1211140">know</span>
  <span m="1211290">about,</span> <span m="1211890">that are</span> <span m="1212040">called</span>
  <span m="1212370">partial</span> <span m="1212940">likelihood</span> <span m="1213450">estimators.</span>
  <span m="1214390">And</span> <span m="1214490">for</span> <span m="1214530">those</span>
  <span m="1214740">of</span> <span m="1214800">you</span> <span m="1214920">who</span>
  <span m="1215010">have</span> <span m="1215130">heard</span> <span m="1215310">of</span>
  <span m="1215820">Cox</span> <span m="1216120">proportional</span> <span m="1216510">hazards</span>
  <span m="1216840">models--</span> <span m="1217170">and</span> <span m="1217260">I</span>
  <span m="1217320">know</span> <span m="1217440">they</span> <span m="1217530">were</span>
  <span m="1217620">discussed</span> <span m="1218070">in</span> <span m="1218160">Friday's</span>
  <span m="1218550">recitation--</span> <span m="1219750">that's</span> <span m="1219990">an</span>
  <span m="1220080">example</span> <span m="1220740">of</span> <span m="1220890">a</span>
  <span m="1220920">class</span> <span m="1221240">of</span> <span m="1221310">model</span>
  <span m="1221700">that's</span> <span m="1221970">commonly</span> <span m="1222990">used</span>
  <span m="1223470">within</span> <span m="1223770">this</span> <span m="1223920">partial</span>
  <span m="1224280">likelihood</span> <span m="1224810">estimator.</span></p><p><span
  m="1226210">Now,</span> <span m="1226470">at</span> <span m="1226590">a</span> <span
  m="1226620">very</span> <span m="1226860">intuitive</span> <span m="1227310">level,</span>
  <span m="1227550">what</span> <span m="1227700">this</span> <span m="1227820">partial</span>
  <span m="1228180">likelihood</span> <span m="1228540">estimator</span> <span m="1228960">is</span>
  <span m="1229110">doing</span> <span m="1229780">is</span> <span m="1230070">it's</span>
  <span m="1230400">working</span> <span m="1230880">with</span> <span m="1231300">something</span>
  <span m="1231600">like</span> <span m="1231750">the</span> <span m="1231840">C-statistic.</span>
  <span m="1233100">So</span> <span m="1234690">notice</span> <span m="1235140">how</span>
  <span m="1235320">the</span> <span m="1235470">C-statistic</span> <span m="1236910">only</span>
  <span m="1237240">looks</span> <span m="1237540">at</span> <span m="1237780">relative</span>
  <span m="1238890">orderings</span> <span m="1239610">of</span> <span m="1239760">events--</span>
  <span m="1240810">of</span> <span m="1240930">their</span> <span m="1241080">event</span>
  <span m="1241350">occurrences.</span> <span m="1244130">It</span> <span m="1244230">doesn't</span>
  <span m="1244390">care</span> <span m="1244660">about</span> <span m="1244870">exactly</span>
  <span m="1245350">when</span> <span m="1245830">the</span> <span m="1245980">event</span>
  <span m="1246310">occurred</span> <span m="1246790">or</span> <span m="1246880">not.</span></p><p><span
  m="1247330">In</span> <span m="1247420">some</span> <span m="1247600">sense,</span>
  <span m="1247980">there's</span> <span m="1250570">a</span> <span m="1250630">constant.</span>
  <span m="1252100">There's--</span> <span m="1252950">in</span> <span m="1253180">this</span>
  <span m="1253900">survival</span> <span m="1254440">function,</span> <span m="1255910">which</span>
  <span m="1256840">could</span> <span m="1257110">be</span> <span m="1257680">divided</span>
  <span m="1258100">out</span> <span m="1258280">from</span> <span m="1258460">both</span>
  <span m="1258730">sides</span> <span m="1259180">of</span> <span m="1259900">this</span>
  <span m="1260590">inequality,</span> <span m="1261400">and</span> <span m="1261520">it</span>
  <span m="1261610">wouldn't</span> <span m="1261820">affect</span> <span m="1262210">anything</span>
  <span m="1262600">about</span> <span m="1262780">the</span> <span m="1262870">statistic.</span>
  <span m="1265330">And</span> <span m="1265490">so</span> <span m="1265760">one</span>
  <span m="1265970">could</span> <span m="1266120">think</span> <span m="1266300">about</span>
  <span m="1266660">other</span> <span m="1266900">ways</span> <span m="1267200">of</span>
  <span m="1267290">learning</span> <span m="1267680">these</span> <span m="1267860">models</span>
  <span m="1268130">by</span> <span m="1268250">saying,</span> <span m="1268680">well,</span>
  <span m="1268800">we</span> <span m="1268850">want</span> <span m="1269030">to</span>
  <span m="1269150">learn</span> <span m="1269450">a</span> <span m="1269510">survival</span>
  <span m="1269990">function</span> <span m="1270530">such</span> <span m="1270770">that</span>
  <span m="1270890">it</span> <span m="1271070">gets</span> <span m="1271430">the</span>
  <span m="1271610">ordering</span> <span m="1272120">correct</span> <span m="1272510">between</span>
  <span m="1272810">data</span> <span m="1273050">points.</span></p><p><span m="1274620">Now,</span>
  <span m="1275000">such</span> <span m="1275280">a</span> <span m="1275340">survival</span>
  <span m="1275630">function</span> <span m="1275960">wouldn't</span> <span m="1276260">do</span>
  <span m="1276470">a</span> <span m="1276560">very</span> <span m="1276830">good</span>
  <span m="1276950">job.</span> <span m="1277760">There's</span> <span m="1278060">no</span>
  <span m="1278180">reason</span> <span m="1278410">it would</span> <span m="1278490">do</span>
  <span m="1278600">any</span> <span m="1279020">good</span> <span m="1279410">at</span>
  <span m="1280130">getting</span> <span m="1280400">the</span> <span m="1280490">precise</span>
  <span m="1281060">time</span> <span m="1281600">of</span> <span m="1281720">when</span>
  <span m="1282060">an</span> <span m="1282440">event</span> <span m="1282740">occurs,</span>
  <span m="1283700">but</span> <span m="1283880">if</span> <span m="1283940">your</span>
  <span m="1284060">goal</span> <span m="1284420">were</span> <span m="1284600">to</span>
  <span m="1284810">just</span> <span m="1286130">figure</span> <span m="1286550">out</span>
  <span m="1288980">what</span> <span m="1289280">is</span> <span m="1289400">the</span>
  <span m="1289550">sorted</span> <span m="1290120">order</span> <span m="1290480">of</span>
  <span m="1290570">patients</span> <span m="1291020">by</span> <span m="1291200">risk</span>
  <span m="1291710">so</span> <span m="1291830">that</span> <span m="1291950">you're</span>
  <span m="1292040">going</span> <span m="1292220">to</span> <span m="1292310">do</span>
  <span m="1292490">an</span> <span m="1292580">intervention</span> <span m="1293090">on</span>
  <span m="1293210">the</span> <span m="1293270">10</span> <span m="1293570">most</span>
  <span m="1293780">risky</span> <span m="1294110">people,</span> <span m="1295010">then</span>
  <span m="1295880">getting</span> <span m="1296270">that</span> <span m="1296480">order</span>
  <span m="1296860">incorrect</span> <span m="1297230">is</span> <span m="1297320">going</span>
  <span m="1297500">to</span> <span m="1297620">be</span> <span m="1297710">enough,</span>
  <span m="1298880">and</span> <span m="1298970">that's</span> <span m="1299090">precisely</span>
  <span m="1299480">the</span> <span m="1299570">intuition</span> <span m="1300050">used</span>
  <span m="1300290">behind</span> <span m="1300830">these</span> <span m="1301010">partial</span>
  <span m="1301370">likelihood</span> <span m="1301730">estimators--</span> <span
  m="1302190">so</span> <span m="1302340">they</span> <span m="1302450">focus</span>
  <span m="1302810">on</span> <span m="1302930">something</span> <span m="1303260">which</span>
  <span m="1303530">is</span> <span m="1304250">a</span> <span m="1304310">little</span>
  <span m="1304490">bit</span> <span m="1304610">less</span> <span m="1304940">than</span>
  <span m="1305060">the</span> <span m="1305150">original</span> <span m="1305510">goal,</span>
  <span m="1306350">but</span> <span m="1306560">in</span> <span m="1306680">doing</span>
  <span m="1307040">so,</span> <span m="1307370">they</span> <span m="1307490">can</span>
  <span m="1307640">have</span> <span m="1307790">much</span> <span m="1308000">better</span>
  <span m="1308240">statistical</span> <span m="1308840">complexity,</span> <span
  m="1309570">meaning</span> <span m="1309690">the</span> <span m="1309770">amount</span>
  <span m="1309950">of</span> <span m="1310040">data</span> <span m="1310370">they</span>
  <span m="1310520">need</span> <span m="1310700">in</span> <span m="1310790">order</span>
  <span m="1310880">to</span> <span m="1310970">fit</span> <span m="1311150">this</span>
  <span m="1311330">models</span> <span m="1311690">well.</span> <span m="1312780">And</span>
  <span m="1312880">again,</span> <span m="1313200">this</span> <span m="1313210">is</span>
  <span m="1313280">a</span> <span m="1313310">very</span> <span m="1313580">rich</span>
  <span m="1313880">topic.</span> <span m="1314390">All</span> <span m="1314530">I</span>
  <span m="1314630">wanted</span> <span m="1314840">to</span> <span m="1314930">do</span>
  <span m="1315050">is</span> <span m="1315140">give</span> <span m="1315290">you</span>
  <span m="1315350">a</span> <span m="1315380">pointer</span> <span m="1315770">to</span>
  <span m="1315980">it</span> <span m="1316100">so</span> <span m="1316220">that</span>
  <span m="1316370">you</span> <span m="1316460">can</span> <span m="1316610">go</span>
  <span m="1316790">read</span> <span m="1316970">more</span> <span m="1317150">about</span>
  <span m="1317330">it</span> <span m="1317460">if</span> <span m="1317510">this</span>
  <span m="1317660">is</span> <span m="1317720">something</span> <span m="1317940">of</span>
  <span m="1318010">interest</span> <span m="1318310">to you.</span></p><p><span m="1321910">So</span>
  <span m="1322540">now</span> <span m="1322780">moving</span> <span m="1323080">on</span>
  <span m="1323310">into</span> <span m="1323500">the</span> <span m="1323590">recap,</span>
  <span m="1326320">one</span> <span m="1326590">of</span> <span m="1326650">the</span>
  <span m="1327100">most</span> <span m="1327370">important</span> <span m="1327820">points</span>
  <span m="1328060">that</span> <span m="1328150">we</span> <span m="1328210">discussed</span>
  <span m="1328630">last</span> <span m="1328930">week</span> <span m="1329110">was</span>
  <span m="1329230">about</span> <span m="1329410">non-stationarity.</span> <span
  m="1330910">And</span> <span m="1331570">there</span> <span m="1331690">was</span>
  <span m="1331810">a</span> <span m="1331960">question</span> <span m="1332380">posted</span>
  <span m="1332710">to</span> <span m="1332800">Piazza,</span> <span m="1333250">which</span>
  <span m="1333400">was</span> <span m="1333520">really</span> <span m="1333670">interesting,</span>
  <span m="1334220">which</span> <span m="1334240">is</span> <span m="1334330">how</span>
  <span m="1334510">do</span> <span m="1334570">you</span> <span m="1334660">actually</span>
  <span m="1334990">deal</span> <span m="1335380">with</span> <span m="1335550">non-stationarity.</span>
  <span m="1335915">And</span> <span m="1336180">I</span> <span m="1336310">spoke</span>
  <span m="1336550">a</span> <span m="1336580">lot</span> <span m="1336820">about</span>
  <span m="1337420">it</span> <span m="1337510">existing,</span> <span m="1338080">and</span>
  <span m="1338170">I</span> <span m="1338260">talked</span> <span m="1338530">about</span>
  <span m="1338680">how</span> <span m="1338800">to</span> <span m="1338890">test</span>
  <span m="1339310">for</span> <span m="1339490">it,</span> <span m="1339700">but</span>
  <span m="1339800">I</span> <span m="1339900">didn't</span> <span m="1339910">say</span>
  <span m="1340060">what</span> <span m="1340210">to</span> <span m="1340300">do</span>
  <span m="1340630">if</span> <span m="1340720">you</span> <span m="1340840">have</span>
  <span m="1341050">it.</span></p><p><span m="1343776">So</span> <span m="1344200">I</span>
  <span m="1344260">thought</span> <span m="1344380">this</span> <span m="1344470">was</span>
  <span m="1344650">such</span> <span m="1344830">an</span> <span m="1344920">interesting</span>
  <span m="1345250">question</span> <span m="1345610">that</span> <span m="1345730">I</span>
  <span m="1345790">would</span> <span m="1345880">also</span> <span m="1346150">talk</span>
  <span m="1346480">about</span> <span m="1346660">it</span> <span m="1346720">a</span>
  <span m="1346780">bit</span> <span m="1346930">during</span> <span m="1347200">lecture.</span>
  <span m="1348190">So</span> <span m="1348580">the</span> <span m="1349150">short</span>
  <span m="1349480">answer</span> <span m="1349960">is,</span> <span m="1350510">if</span>
  <span m="1350560">you</span> <span m="1350740">have</span> <span m="1351100">to</span>
  <span m="1351760">have</span> <span m="1352000">a</span> <span m="1352030">solution</span>
  <span m="1352540">that</span> <span m="1352690">you</span> <span m="1352780">deploy</span>
  <span m="1353170">tomorrow,</span> <span m="1355380">then</span> <span m="1355920">here's</span>
  <span m="1356280">the</span> <span m="1356370">hack</span> <span m="1356700">that</span>
  <span m="1357090">sometimes</span> <span m="1357630">works.</span> <span m="1358710">You</span>
  <span m="1358800">take</span> <span m="1359010">your</span> <span m="1359100">most</span>
  <span m="1359370">recent</span> <span m="1359670">data,</span> <span m="1360030">like
  the</span> <span m="1360210">last</span> <span m="1360450">three</span> <span m="1360660">months'</span>
  <span m="1360900">data,</span> <span m="1361170">and</span> <span m="1361260">you</span>
  <span m="1361350">hope</span> <span m="1361650">that</span> <span m="1361950">there's</span>
  <span m="1362130">not</span> <span m="1362340">much</span> <span m="1362640">non-stationarity</span>
  <span m="1363360">within</span> <span m="1363570">last</span> <span m="1363750">three</span>
  <span m="1363930">months.</span> <span m="1365490">You</span> <span m="1365580">throw</span>
  <span m="1366120">out</span> <span m="1366300">all</span> <span m="1366420">the</span>
  <span m="1366510">historical</span> <span m="1367020">data,</span> <span m="1367800">and</span>
  <span m="1367890">you</span> <span m="1367950">just</span> <span m="1368100">train</span>
  <span m="1368400">using</span> <span m="1368580">the</span> <span m="1368640">most</span>
  <span m="1368820">recent</span> <span m="1369090">data.</span> <span m="1371410">So</span>
  <span m="1373490">a</span> <span m="1373550">bit</span> <span m="1373730">unsatisfying,</span>
  <span m="1374690">because</span> <span m="1375020">you</span> <span m="1375110">might</span>
  <span m="1375620">have</span> <span m="1375980">now</span> <span m="1376190">extremely</span>
  <span m="1376670">little</span> <span m="1376880">data</span> <span m="1377120">left</span>
  <span m="1377330">to</span> <span m="1377420">learn</span> <span m="1377660">with,</span>
  <span m="1377950">but</span> <span m="1378960">if</span> <span m="1379100">you</span>
  <span m="1379220">have</span> <span m="1379460">enough</span> <span m="1379610">volume,</span>
  <span m="1380370">it</span> <span m="1380660">might</span> <span m="1380840">be</span>
  <span m="1380930">good</span> <span m="1381050">enough.</span> <span m="1382920">But</span>
  <span m="1383150">the</span> <span m="1383270">real</span> <span m="1383570">interesting</span>
  <span m="1383960">question</span> <span m="1384260">from</span> <span m="1384380">a</span>
  <span m="1384410">research</span> <span m="1384710">perspective</span> <span m="1385100">is</span>
  <span m="1385220">how</span> <span m="1385430">could</span> <span m="1385580">you</span>
  <span m="1385700">optimally</span> <span m="1386180">use</span> <span m="1386460">that</span>
  <span m="1386630">historical</span> <span m="1387110">data.</span></p><p><span m="1387540">So</span>
  <span m="1388040">here</span> <span m="1388250">are</span> <span m="1388310">three</span>
  <span m="1388670">different</span> <span m="1388940">ways.</span> <span m="1390150">So</span>
  <span m="1390710">one</span> <span m="1390950">way</span> <span m="1391280">has</span>
  <span m="1391490">to</span> <span m="1391610">do</span> <span m="1391880">with</span>
  <span m="1392120">imputation.</span> <span m="1394420">Imagine</span> <span m="1394900">that</span>
  <span m="1395050">the</span> <span m="1395200">way</span> <span m="1395650">in</span>
  <span m="1395770">which</span> <span m="1396130">your</span> <span m="1396730">data</span>
  <span m="1397060">was</span> <span m="1397210">non-stationary</span> <span m="1397990">was</span>
  <span m="1398170">because</span> <span m="1398560">there</span> <span m="1398680">were,</span>
  <span m="1398960">let's</span> <span m="1399010">say,</span> <span m="1399130">parts</span>
  <span m="1399520">of</span> <span m="1399640">time</span> <span m="1400840">when</span>
  <span m="1401350">certain</span> <span m="1401980">features</span> <span m="1402370">were</span>
  <span m="1402460">just</span> <span m="1402670">unavailable.</span> <span m="1404110">I</span>
  <span m="1404350">gave</span> <span m="1404620">you</span> <span m="1404680">this</span>
  <span m="1404950">example</span> <span m="1405550">last</span> <span m="1405880">week</span>
  <span m="1406360">of</span> <span m="1406600">laboratory</span> <span m="1407140">test</span>
  <span m="1407410">results</span> <span m="1407710">across</span> <span m="1407980">time,</span>
  <span m="1408400">and</span> <span m="1408700">I</span> <span m="1408760">showed</span>
  <span m="1408940">you</span> <span m="1409030">how</span> <span m="1409150">there
  are</span> <span m="1409300">sometimes</span> <span m="1409660">these</span> <span
  m="1409780">really</span> <span m="1410020">big</span> <span m="1410200">blocks</span>
  <span m="1410620">of</span> <span m="1410710">time</span> <span m="1410950">where</span>
  <span m="1411070">no</span> <span m="1411310">lab</span> <span m="1411550">tests</span>
  <span m="1411850">are</span> <span m="1411880">available,</span> <span m="1412240">or</span>
  <span m="1412300">very</span> <span m="1412540">few</span> <span m="1412780">are</span>
  <span m="1412810">available.</span></p><p><span m="1414810">Well,</span> <span m="1415100">luckily</span>
  <span m="1415580">we</span> <span m="1415700">live</span> <span m="1415910">in</span>
  <span m="1415970">a</span> <span m="1416030">world</span> <span m="1416420">with</span>
  <span m="1416960">high</span> <span m="1417200">dimensional</span> <span m="1417620">data,</span>
  <span m="1417960">and</span> <span m="1418060">what</span> <span m="1418160">that</span>
  <span m="1418260">means</span> <span m="1418370">is</span> <span m="1418450">there's</span>
  <span m="1418580">often</span> <span m="1418850">a</span> <span m="1418910">lot</span>
  <span m="1419060">of</span> <span m="1419120">redundancy</span> <span m="1419720">in</span>
  <span m="1419810">the</span> <span m="1419870">data.</span> <span m="1420930">So</span>
  <span m="1421040">what</span> <span m="1421250">you</span> <span m="1421340">could</span>
  <span m="1421580">imagine</span> <span m="1421970">doing</span> <span m="1423080">is</span>
  <span m="1423740">imputing</span> <span m="1425390">features</span> <span m="1425840">that</span>
  <span m="1425930">you</span> <span m="1426050">observed</span> <span m="1426410">to</span>
  <span m="1426500">be</span> <span m="1426620">missing,</span> <span m="1428190">such</span>
  <span m="1428390">that</span> <span m="1428630">the</span> <span m="1428780">missingness</span>
  <span m="1429320">properties,</span> <span m="1429950">in</span> <span m="1430040">fact,</span>
  <span m="1430520">aren't</span> <span m="1430970">changing</span> <span m="1431510">as</span>
  <span m="1431630">much</span> <span m="1431870">across</span> <span m="1432170">time</span>
  <span m="1432440">after</span> <span m="1432710">imputation.</span> <span m="1434180">And
  if</span> <span m="1434300">you</span> <span m="1434360">do</span> <span m="1434450">that</span>
  <span m="1434580">as</span> <span m="1434650">a</span> <span m="1434710">pre-processing</span>
  <span m="1435230">step,</span> <span m="1436010">it</span> <span m="1436130">may</span>
  <span m="1436520">allow</span> <span m="1436820">you</span> <span m="1436910">to</span>
  <span m="1437000">make</span> <span m="1437180">use</span> <span m="1437450">of</span>
  <span m="1437570">much</span> <span m="1437810">more</span> <span m="1437960">of</span>
  <span m="1438050">the</span> <span m="1438110">historical</span> <span m="1438590">data.</span></p><p><span
  m="1440690">A</span> <span m="1441140">different</span> <span m="1441470">approach,</span>
  <span m="1441870">which</span> <span m="1441890">is</span> <span m="1442070">intimately</span>
  <span m="1442640">tied</span> <span m="1442970">to</span> <span m="1443090">that,</span>
  <span m="1443570">has</span> <span m="1443810">to</span> <span m="1443870">do</span>
  <span m="1443960">with</span> <span m="1444140">transforming</span> <span m="1445100">the</span>
  <span m="1445220">data.</span> <span m="1445490">Instead</span> <span m="1445700">of</span>
  <span m="1445820">imputing</span> <span m="1446480">it,</span> <span m="1446990">transforming</span>
  <span m="1447650">it</span> <span m="1447770">into</span> <span m="1448010">another</span>
  <span m="1448370">representation</span> <span m="1449090">altogether,</span> <span
  m="1450230">such</span> <span m="1450530">that</span> <span m="1450710">that</span>
  <span m="1450830">presentation</span> <span m="1451940">is</span> <span m="1452130">invariant</span>
  <span m="1453230">across</span> <span m="1453710">time.</span> <span m="1455150">And</span>
  <span m="1455390">here</span> <span m="1455630">I'm</span> <span m="1455720">giving</span>
  <span m="1455960">you</span> <span m="1456020">a</span> <span m="1456080">reference</span>
  <span m="1456560">to</span> <span m="1456650">this</span> <span m="1456800">paper</span>
  <span m="1457160">by</span> <span m="1457660">Ganin</span> <span m="1457890">et</span>
  <span m="1458060">al</span> <span m="1458330">from</span> <span m="1458750">the</span>
  <span m="1458870"><i>Journal</i></span> <span m="1459005"><i>of</i></span> <span
  m="1459140"><i>Machine</i></span> <span m="1459380"><i>Learning</i></span> <span
  m="1459620"><i>Research</i></span> <span m="1459920">2016,</span> <span m="1461090">which</span>
  <span m="1461240">talks</span> <span m="1461470">about</span> <span m="1461590">how</span>
  <span m="1461660">to</span> <span m="1461780">do</span> <span m="1461930">domain</span>
  <span m="1462500">and</span> <span m="1462650">variant</span> <span m="1463490">learning</span>
  <span m="1464120">of</span> <span m="1464270">neural</span> <span m="1464480">networks,</span>
  <span m="1464960">and that's</span> <span m="1465140">one</span> <span m="1465380">approach</span>
  <span m="1465680">to</span> <span m="1465770">do</span> <span m="1465920">so.</span>
  <span m="1466190">And</span> <span m="1466280">I</span> <span m="1466370">view</span>
  <span m="1466550">those</span> <span m="1466760">two</span> <span m="1466940">as</span>
  <span m="1467060">being</span> <span m="1467240">very</span> <span m="1467450">similar--</span>
  <span m="1467810">imputation</span> <span m="1468230">and</span> <span m="1468320">transformations.</span></p><p><span
  m="1470210">A</span> <span m="1470270">second</span> <span m="1470750">approach</span>
  <span m="1471590">is</span> <span m="1471740">to</span> <span m="1471860">re-weight</span>
  <span m="1472490">the</span> <span m="1472610">data</span> <span m="1472970">to</span>
  <span m="1473150">look</span> <span m="1473480">like</span> <span m="1473810">the</span>
  <span m="1473990">current</span> <span m="1474470">data.</span> <span m="1476230">So</span>
  <span m="1476520">imagine</span> <span m="1477000">that</span> <span m="1477120">you</span>
  <span m="1477240">go</span> <span m="1477420">back</span> <span m="1477720">in</span>
  <span m="1477810">time,</span> <span m="1478170">and you</span> <span m="1478290">say,</span>
  <span m="1478530">you</span> <span m="1478650">know</span> <span m="1478800">what?</span>
  <span m="1479670">I</span> <span m="1479780">ICD-10</span> <span m="1480300">codes,</span>
  <span m="1481260">for</span> <span m="1481410">some</span> <span m="1481650">very</span>
  <span m="1481950">weird</span> <span m="1482220">reason--</span> <span m="1483050">this</span>
  <span m="1483180">is</span> <span m="1483240">not</span> <span m="1483390">true,</span>
  <span m="1483540">by</span> <span m="1483630">the</span> <span m="1483690">way--</span>
  <span m="1484530">ICD-10</span> <span m="1484840">codes</span> <span m="1485850">in</span>
  <span m="1485970">this</span> <span m="1486120">untrue</span> <span m="1486510">world</span>
  <span m="1487260">happen</span> <span m="1487620">to</span> <span m="1487740">be</span>
  <span m="1487830">used</span> <span m="1488160">between</span> <span m="1488520">March</span>
  <span m="1489090">and</span> <span m="1489270">April</span> <span m="1489720">of</span>
  <span m="1489810">2003.</span> <span m="1491870">And</span> <span m="1491960">then</span>
  <span m="1492050">they</span> <span m="1492170">weren't</span> <span m="1492350">used</span>
  <span m="1492530">again</span> <span m="1492830">until</span> <span m="1494180">2015.</span></p><p><span
  m="1497190">So</span> <span m="1497440">instead</span> <span m="1497680">of</span>
  <span m="1497770">throwing</span> <span m="1498010">away</span> <span m="1498160">all</span>
  <span m="1498430">of</span> <span m="1498520">the</span> <span m="1498610">previous</span>
  <span m="1499000">data,</span> <span m="1499630">we're</span> <span m="1499720">going</span>
  <span m="1499830">to</span> <span m="1499900">recognize</span> <span m="1500620">that</span>
  <span m="1502390">those--</span> <span m="1502630">that</span> <span m="1502840">three</span>
  <span m="1503050">month</span> <span m="1503260">interval</span> <span m="1504030">10</span>
  <span m="1504280">years</span> <span m="1504550">ago</span> <span m="1504740">was</span>
  <span m="1504880">actually</span> <span m="1505690">drawn</span> <span m="1505990">from</span>
  <span m="1506140">a</span> <span m="1506160">very</span> <span m="1506410">similar</span>
  <span m="1506680">distribution</span> <span m="1507340">as</span> <span m="1507550">what</span>
  <span m="1507680">we're</span> <span m="1507770">going</span> <span m="1507820">to</span>
  <span m="1507880">be</span> <span m="1507940">testing</span> <span m="1508300">on</span>
  <span m="1508390">today.</span> <span m="1509200">So</span> <span m="1509290">we're</span>
  <span m="1509380">going</span> <span m="1509530">to</span> <span m="1509710">weight</span>
  <span m="1510250">those</span> <span m="1510610">data</span> <span m="1510880">points</span>
  <span m="1511210">up</span> <span m="1511480">very</span> <span m="1511810">much,</span>
  <span m="1512230">and</span> <span m="1512440">down</span> <span m="1512900">weight</span>
  <span m="1513370">the</span> <span m="1513520">data</span> <span m="1513760">points</span>
  <span m="1514090">that</span> <span m="1514210">are</span> <span m="1514330">less</span>
  <span m="1514870">like</span> <span m="1515200">the</span> <span m="1515320">ones</span>
  <span m="1515590">from</span> <span m="1515710">today.</span> <span m="1516760">That's
  the</span> <span m="1517000">intuition</span> <span m="1517480">behind</span> <span
  m="1517840">these</span> <span m="1518020">re-weighting</span> <span m="1518500">approaches,</span>
  <span m="1519790">and</span> <span m="1520330">we're</span> <span m="1520480">going</span>
  <span m="1520630">to</span> <span m="1520720">talk</span> <span m="1520900">much</span>
  <span m="1521260">more</span> <span m="1521560">about</span> <span m="1521830">that</span>
  <span m="1522010">in</span> <span m="1522100">the</span> <span m="1522160">context</span>
  <span m="1522640">of</span> <span m="1522730">causal</span> <span m="1523060">inference,</span>
  <span m="1523900">not</span> <span m="1524110">because</span> <span m="1524410">these</span>
  <span m="1524620">two</span> <span m="1525250">have</span> <span m="1525430">to</span>
  <span m="1525520">do with</span> <span m="1525640">each</span> <span m="1525790">other,</span>
  <span m="1526270">but</span> <span m="1526420">they</span> <span m="1526510">have--</span>
  <span m="1526750">they</span> <span m="1526870">end</span> <span m="1527020">up</span>
  <span m="1527140">using</span> <span m="1527410">a</span> <span m="1527440">very</span>
  <span m="1527680">similar</span> <span m="1527980">technique</span> <span m="1528370">for</span>
  <span m="1528460">how</span> <span m="1528550">to</span> <span m="1528670">deal</span>
  <span m="1528880">with</span> <span m="1529110">datas</span> <span m="1529310">that</span>
  <span m="1529600">shift,</span> <span m="1529890">or</span> <span m="1529960">covariate</span>
  <span m="1530260">shift.</span></p><p><span m="1532600">And</span> <span m="1532720">the</span>
  <span m="1532780">final</span> <span m="1533170">technique</span> <span m="1533860">that</span>
  <span m="1534040">I'll</span> <span m="1534130">mention</span> <span m="1534910">is</span>
  <span m="1535090">based</span> <span m="1535360">on</span> <span m="1535570">online</span>
  <span m="1536200">learning</span> <span m="1536530">algorithms.</span> <span m="1537710">So</span>
  <span m="1537730">the</span> <span m="1537790">idea</span> <span m="1538150">there</span>
  <span m="1539350">is</span> <span m="1539530">that</span> <span m="1542740">there</span>
  <span m="1542890">might</span> <span m="1543100">be</span> <span m="1543250">cut</span>
  <span m="1543550">points,</span> <span m="1544030">change</span> <span m="1544420">points</span>
  <span m="1544780">across</span> <span m="1545110">time.</span> <span m="1547760">So</span>
  <span m="1548380">maybe</span> <span m="1549310">the</span> <span m="1549430">data</span>
  <span m="1549730">looks</span> <span m="1550000">one</span> <span m="1550270">way</span>
  <span m="1550840">up</span> <span m="1551020">until</span> <span m="1551380">this</span>
  <span m="1551590">change</span> <span m="1551950">point,</span> <span m="1552490">and</span>
  <span m="1552610">then</span> <span m="1552730">suddenly</span> <span m="1553120">the</span>
  <span m="1553210">data</span> <span m="1553450">looks</span> <span m="1553660">really</span>
  <span m="1553900">different</span> <span m="1554440">until</span> <span m="1554740">this</span>
  <span m="1554980">change</span> <span m="1555310">point,</span> <span m="1555590">and</span>
  <span m="1555670">then</span> <span m="1555790">suddenly</span> <span m="1556020">the</span>
  <span m="1556090">data</span> <span m="1556330">looks</span> <span m="1556510">very</span>
  <span m="1556750">different</span> <span m="1558160">on</span> <span m="1558520">into</span>
  <span m="1558670">the</span> <span m="1558760">future.</span></p><p><span m="1559660">So</span>
  <span m="1559780">here</span> <span m="1559990">I'm</span> <span m="1560080">showing</span>
  <span m="1560290">you</span> <span m="1560350">there</span> <span m="1560500">are
  two</span> <span m="1560860">change</span> <span m="1561280">points</span> <span
  m="1561640">in</span> <span m="1561730">which</span> <span m="1561940">data</span>
  <span m="1562150">set</span> <span m="1562390">shift</span> <span m="1562840">happens.</span>
  <span m="1564610">What</span> <span m="1564760">these</span> <span m="1564940">online</span>
  <span m="1565330">learning</span> <span m="1565660">algorithms</span> <span m="1566140">do</span>
  <span m="1566350">is</span> <span m="1566470">they</span> <span m="1566560">say,</span>
  <span m="1566900">OK,</span> <span m="1567370">suppose</span> <span m="1567850">we</span>
  <span m="1567940">were</span> <span m="1568000">forced</span> <span m="1568450">to</span>
  <span m="1568540">make</span> <span m="1568690">predictions</span> <span m="1569350">throughout</span>
  <span m="1569800">this</span> <span m="1569980">time</span> <span m="1570220">period</span>
  <span m="1571030">using</span> <span m="1571360">only</span> <span m="1571750">the</span>
  <span m="1571840">historical</span> <span m="1572410">data</span> <span m="1572680">to</span>
  <span m="1572770">make</span> <span m="1572920">predictions</span> <span m="1573400">at</span>
  <span m="1573490">each</span> <span m="1573610">point</span> <span m="1573790">in</span>
  <span m="1573850">time.</span> <span m="1575200">Well,</span> <span m="1576160">if</span>
  <span m="1576670">we</span> <span m="1576910">could</span> <span m="1577090">somehow</span>
  <span m="1577660">recognize</span> <span m="1578650">that</span> <span m="1579580">there</span>
  <span m="1579760">might</span> <span m="1580090">be</span> <span m="1580270">these</span>
  <span m="1580480">shifts,</span> <span m="1581230">we</span> <span m="1581380">could</span>
  <span m="1581500">design</span> <span m="1581890">algorithms</span> <span m="1582490">that</span>
  <span m="1582580">are</span> <span m="1582670">going</span> <span m="1582880">to</span>
  <span m="1583060">be</span> <span m="1583240">robust</span> <span m="1584020">to</span>
  <span m="1584230">those</span> <span m="1584470">shifts.</span> <span m="1585910">And</span>
  <span m="1586030">then</span> <span m="1586180">one</span> <span m="1586360">could</span>
  <span m="1586480">try</span> <span m="1586630">to</span> <span m="1586750">analyze--</span>
  <span m="1587350">mathematically</span> <span m="1588040">analyze</span> <span m="1588430">those</span>
  <span m="1588850">algorithms</span> <span m="1589090">based</span> <span m="1589180">on
  the</span> <span m="1589240">amount</span> <span m="1589540">of</span> <span m="1589690">regret</span>
  <span m="1590350">they</span> <span m="1590530">would</span> <span m="1590650">have</span>
  <span m="1591460">to,</span> <span m="1591760">for</span> <span m="1591910">example,</span>
  <span m="1592390">an</span> <span m="1592510">algorithm</span> <span m="1592930">that</span>
  <span m="1593050">knew</span> <span m="1593260">exactly</span> <span m="1593770">when</span>
  <span m="1593920">those</span> <span m="1594070">changes</span> <span m="1594460">were.</span>
  <span m="1595270">And</span> <span m="1595360">of</span> <span m="1595420">course,</span>
  <span m="1595630">we</span> <span m="1595750">don't</span> <span m="1595990">know</span>
  <span m="1596260">precisely</span> <span m="1596770">when</span> <span m="1596890">those</span>
  <span m="1597010">changes</span> <span m="1597370">were.</span> <span m="1598970">And</span>
  <span m="1599110">so</span> <span m="1599290">there's</span> <span m="1599440">a</span>
  <span m="1599500">whole</span> <span m="1599800">field</span> <span m="1600100">of</span>
  <span m="1600190">algorithms</span> <span m="1601090">trying</span> <span m="1601330">to</span>
  <span m="1601420">do</span> <span m="1601510">that,</span> <span m="1601660">and</span>
  <span m="1601780">here</span> <span m="1601900">I'm</span> <span m="1601990">just</span>
  <span m="1602140">give</span> <span m="1602240">me</span> <span m="1602350">one</span>
  <span m="1602620">citation</span> <span m="1603160">for</span> <span m="1603760">a</span>
  <span m="1603830">recent</span> <span m="1604570">work.</span></p><p><span m="1607680">So</span>
  <span m="1608040">to</span> <span m="1608280">conclude</span> <span m="1608800">risk</span>
  <span m="1608880">stratification--</span> <span m="1609240">this</span> <span m="1609600">is</span>
  <span m="1609720">the</span> <span m="1609810">last</span> <span m="1610020">slide</span>
  <span m="1610290">here.</span> <span m="1611970">Maybe</span> <span m="1612180">ask</span>
  <span m="1612360">your</span> <span m="1612450">question</span> <span m="1612690">after</span>
  <span m="1612870">class.</span> <span m="1615080">We've</span> <span m="1615230">talked</span>
  <span m="1615410">about</span> <span m="1615560">two</span> <span m="1615830">approaches</span>
  <span m="1616490">for</span> <span m="1616910">formalizing</span> <span m="1617540">risk</span>
  <span m="1618140">stratification--</span> <span m="1618590">first</span> <span m="1618890">as</span>
  <span m="1619040">binary</span> <span m="1619310">classification.</span> <span m="1620000">Second</span>
  <span m="1620510">as</span> <span m="1621320">regression.</span> <span m="1622430">And</span>
  <span m="1622620">in</span> <span m="1622690">the</span> <span m="1622760">regression</span>
  <span m="1623960">framework,</span> <span m="1624770">one</span> <span m="1624950">has</span>
  <span m="1625130">to</span> <span m="1625250">think</span> <span m="1625550">about</span>
  <span m="1625790">censoring,</span> <span m="1626330">which</span> <span m="1626480">is</span>
  <span m="1626570">why</span> <span m="1626840">we</span> <span m="1626960">call</span>
  <span m="1627170">it</span> <span m="1627260">survival</span> <span m="1627710">modeling.</span></p><p><span
  m="1631090">Second,</span> <span m="1632920">in</span> <span m="1633370">our</span>
  <span m="1634180">examples,</span> <span m="1634960">and</span> <span m="1635080">again</span>
  <span m="1635620">in</span> <span m="1635890">your</span> <span m="1636220">homework</span>
  <span m="1636550">assignment</span> <span m="1636940">that's</span> <span m="1637180">coming</span>
  <span m="1637540">up</span> <span m="1638410">next</span> <span m="1638710">week,</span>
  <span m="1640990">we'll</span> <span m="1641200">see</span> <span m="1641770">that</span>
  <span m="1642640">often</span> <span m="1643360">the</span> <span m="1644170">variables,</span>
  <span m="1645010">the</span> <span m="1645070">features</span> <span m="1645700">that</span>
  <span m="1645970">are</span> <span m="1646240">most</span> <span m="1646540">predictive</span>
  <span m="1647110">make</span> <span m="1647350">a</span> <span m="1647410">lot</span>
  <span m="1647560">of</span> <span m="1647620">sense.</span> <span m="1649850">In</span>
  <span m="1649900">the</span> <span m="1650080">diabetes</span> <span m="1650650">case,</span>
  <span m="1651520">we</span> <span m="1651700">said--</span> <span m="1652480">we</span>
  <span m="1652630">saw</span> <span m="1652990">how</span> <span m="1654430">patients</span>
  <span m="1654850">having</span> <span m="1655510">comorbidities</span> <span m="1656170">of</span>
  <span m="1656260">diabetes,</span> <span m="1656740">like</span> <span m="1656920">hypertension,</span>
  <span m="1657790">or</span> <span m="1657880">patients</span> <span m="1658240">being</span>
  <span m="1658480">obese</span> <span m="1659080">were</span> <span m="1659260">very</span>
  <span m="1659530">predictive</span> <span m="1659950">of</span> <span m="1660010">patients</span>
  <span m="1660370">getting</span> <span m="1660700">diabetes.</span></p><p><span
  m="1662370">So</span> <span m="1662520">you</span> <span m="1662580">might</span>
  <span m="1662760">ask</span> <span m="1663120">yourself,</span> <span m="1664690">is</span>
  <span m="1664710">there</span> <span m="1664800">something</span> <span m="1665130">causal</span>
  <span m="1665550">there?</span> <span m="1666120">Are</span> <span m="1666240">those</span>
  <span m="1666480">features</span> <span m="1666930">that</span> <span m="1667050">are</span>
  <span m="1667110">very</span> <span m="1667350">predictive</span> <span m="1668220">in</span>
  <span m="1668340">fact</span> <span m="1668670">causing--</span> <span m="1669870">what's</span>
  <span m="1670140">causing</span> <span m="1670560">the</span> <span m="1670620">patient</span>
  <span m="1670950">to</span> <span m="1671070">develop</span> <span m="1671460">type</span>
  <span m="1671670">2</span> <span m="1671730">diabetes?</span> <span m="1672180">Like,</span>
  <span m="1672360">for</span> <span m="1672450">example,</span> <span m="1673120">obesity</span>
  <span m="1673560">causing</span> <span m="1674280">diabetes.</span> <span m="1675580">And</span>
  <span m="1675720">this</span> <span m="1675840">is</span> <span m="1675960">where</span>
  <span m="1676080">I</span> <span m="1676110">want</span> <span m="1676260">to</span>
  <span m="1676320">caution</span> <span m="1676800">you.</span> <span m="1678290">You</span>
  <span m="1678470">shouldn't</span> <span m="1679130">interpret</span> <span m="1679850">these</span>
  <span m="1680960">very</span> <span m="1681260">predictive</span> <span m="1681680">features</span>
  <span m="1682190">in</span> <span m="1682340">a</span> <span m="1682400">causal</span>
  <span m="1682760">fashion,</span> <span m="1684330">particularly</span> <span m="1684950">not</span>
  <span m="1685220">when</span> <span m="1685460">one</span> <span m="1686060">starts</span>
  <span m="1686390">to</span> <span m="1686450">work</span> <span m="1686660">with</span>
  <span m="1686780">high</span> <span m="1686960">dimensional</span> <span m="1687380">data,</span>
  <span m="1687650">as</span> <span m="1687770">we</span> <span m="1687890">do</span>
  <span m="1690160">in</span> <span m="1690380">this</span> <span m="1690530">course.</span></p><p><span
  m="1692680">The</span> <span m="1692800">reason</span> <span m="1693280">for</span>
  <span m="1693610">that</span> <span m="1693880">is</span> <span m="1694090">very</span>
  <span m="1694390">subtle,</span> <span m="1695290">and</span> <span m="1695440">we'll</span>
  <span m="1695560">talk</span> <span m="1695890">about</span> <span m="1696250">that</span>
  <span m="1696640">in</span> <span m="1696880">the</span> <span m="1697000">causal</span>
  <span m="1697330">inference</span> <span m="1697660">lectures,</span> <span m="1698200">but</span>
  <span m="1698470">I</span> <span m="1698560">just</span> <span m="1698710">wanted</span>
  <span m="1698950">to</span> <span m="1699100">give</span> <span m="1699370">you</span>
  <span m="1699580">a</span> <span m="1699700">pointer</span> <span m="1700180">now</span>
  <span m="1700540">that</span> <span m="1700690">you</span> <span m="1700780">shouldn't</span>
  <span m="1701170">think</span> <span m="1701380">about</span> <span m="1701560">it</span>
  <span m="1701620">in</span> <span m="1701680">that</span> <span m="1701860">way.</span>
  <span m="1702500">And</span> <span m="1702610">you'll</span> <span m="1703060">understand</span>
  <span m="1703540">why</span> <span m="1703900">in</span> <span m="1704020">just</span>
  <span m="1704260">a</span> <span m="1704290">few</span> <span m="1704500">weeks.</span>
  <span m="1706540">And</span> <span m="1706720">finally</span> <span m="1707050">we</span>
  <span m="1707140">talked</span> <span m="1707470">about</span> <span m="1708850">ways</span>
  <span m="1709270">of</span> <span m="1709360">dealing</span> <span m="1709750">with</span>
  <span m="1710170">missing</span> <span m="1710590">data.</span> <span m="1711820">I</span>
  <span m="1711940">gave</span> <span m="1712270">you</span> <span m="1712540">one</span>
  <span m="1712990">feature</span> <span m="1713470">representation</span> <span m="1715620">for</span>
  <span m="1715800">the</span> <span m="1715890">diabetes</span> <span m="1716460">case,</span>
  <span m="1717780">which</span> <span m="1718020">was</span> <span m="1718680">designed</span>
  <span m="1719430">to</span> <span m="1719560">deal</span> <span m="1719940">with</span>
  <span m="1720060">missing</span> <span m="1720300">data.</span> <span m="1720490">It</span>
  <span m="1720570">said,</span> <span m="1721170">was</span> <span m="1721440">there</span>
  <span m="1721650">any</span> <span m="1722040">diagnosis</span> <span m="1722790">code</span>
  <span m="1723480">250.01</span> <span m="1726890">in</span> <span m="1727080">the</span>
  <span m="1727200">last</span> <span m="1728040">three</span> <span m="1728460">months?</span>
  <span m="1729280">And</span> <span m="1729300">if</span> <span m="1729390">there</span>
  <span m="1729540">was,</span> <span m="1730020">you</span> <span m="1730140">have</span>
  <span m="1730320">a</span> <span m="1730380">1.</span> <span m="1730650">If</span>
  <span m="1730770">you</span> <span m="1730860">don't,</span> <span m="1731100">0.</span></p><p><span
  m="1731170">So</span> <span m="1731580">it's</span> <span m="1731700">designed</span>
  <span m="1732180">to</span> <span m="1732300">recognize</span> <span m="1732900">that</span>
  <span m="1733200">you</span> <span m="1733350">don't</span> <span m="1733470">have</span>
  <span m="1733710">information,</span> <span m="1734220">perhaps,</span> <span m="1734520">for</span>
  <span m="1734700">some</span> <span m="1734940">large</span> <span m="1735180">chunk</span>
  <span m="1735390">of</span> <span m="1735480">time</span> <span m="1735720">in</span>
  <span m="1735810">that</span> <span m="1735930">window.</span> <span m="1738100">But</span>
  <span m="1738790">that</span> <span m="1738970">missing</span> <span m="1739300">data</span>
  <span m="1739570">could</span> <span m="1739780">also</span> <span m="1740170">be</span>
  <span m="1740500">dangerous</span> <span m="1741520">if</span> <span m="1741790">that</span>
  <span m="1742000">missingness</span> <span m="1742540">itself</span> <span m="1743380">has</span>
  <span m="1743920">caused</span> <span m="1744430">you</span> <span m="1744520">to</span>
  <span m="1744610">non-stationarity,</span> <span m="1745690">which</span> <span
  m="1745900">is</span> <span m="1746050">then</span> <span m="1746260">going</span>
  <span m="1746530">to</span> <span m="1747220">result</span> <span m="1747790">in</span>
  <span m="1747940">your</span> <span m="1748300">test</span> <span m="1748600">distribution</span>
  <span m="1749050">looking</span> <span m="1749290">different</span> <span m="1749590">from</span>
  <span m="1749710">your</span> <span m="1749800">training</span> <span m="1750010">distribution.</span>
  <span m="1751490">And</span> <span m="1751590">that's</span> <span m="1751810">where</span>
  <span m="1752020">approaches</span> <span m="1752680">that</span> <span m="1753130">are</span>
  <span m="1753280">based</span> <span m="1753610">on</span> <span m="1753730">imputation</span>
  <span m="1754450">could</span> <span m="1754600">actually</span> <span m="1754840">be</span>
  <span m="1754930">very</span> <span m="1755170">valuable,</span> <span m="1756040">not</span>
  <span m="1756280">because</span> <span m="1756700">they</span> <span m="1757540">improve</span>
  <span m="1757840">your</span> <span m="1757960">predictive</span> <span m="1758320">accuracy</span>
  <span m="1758740">when</span> <span m="1758860">everything</span> <span m="1759220">goes</span>
  <span m="1759490">right,</span> <span m="1760240">but</span> <span m="1760390">because</span>
  <span m="1760810">they</span> <span m="1761020">might</span> <span m="1761260">improve</span>
  <span m="1761560">your</span> <span m="1761680">predictive</span> <span m="1762160">accuracy</span>
  <span m="1762700">when</span> <span m="1762820">things</span> <span m="1763090">go</span>
  <span m="1763240">wrong.</span></p><p><span m="1764840">And</span> <span m="1764890">so</span>
  <span m="1765010">one</span> <span m="1765190">of</span> <span m="1765280">your</span>
  <span m="1765400">readings</span> <span m="1765730">for</span> <span m="1765850">last</span>
  <span m="1766120">week's</span> <span m="1766360">lecture</span> <span m="1766690">was</span>
  <span m="1766870">actually</span> <span m="1767110">an</span> <span m="1767170">example</span>
  <span m="1767560">of</span> <span m="1767620">that,</span> <span m="1768340">where</span>
  <span m="1768520">they</span> <span m="1768640">used</span> <span m="1768970">a</span>
  <span m="1769030">Gaussian</span> <span m="1769510">process</span> <span m="1770080">model</span>
  <span m="1770800">to</span> <span m="1771010">impute</span> <span m="1771880">much</span>
  <span m="1772150">of</span> <span m="1772240">the</span> <span m="1772330">missing</span>
  <span m="1772780">data</span> <span m="1773460">in</span> <span m="1773590">a</span>
  <span m="1773630">patient's</span> <span m="1774190">continuous</span> <span m="1774700">vital</span>
  <span m="1775000">signs,</span> <span m="1775780">and</span> <span m="1775930">then</span>
  <span m="1776080">they</span> <span m="1776200">used</span> <span m="1776400">a</span>
  <span m="1776440">recurrent</span> <span m="1776860">neural</span> <span m="1777090">network</span>
  <span m="1777580">to</span> <span m="1777760">predict</span> <span m="1778210">based</span>
  <span m="1778630">on</span> <span m="1778960">that</span> <span m="1779410">imputed</span>
  <span m="1779860">data.</span> <span m="1781480">So</span> <span m="1781800">in</span>
  <span m="1781920">that</span> <span m="1782250">case,</span> <span m="1784650">there</span>
  <span m="1784890">are</span> <span m="1784950">really</span> <span m="1785190">two</span>
  <span m="1785490">things</span> <span m="1785760">going</span> <span m="1785940">on.</span>
  <span m="1786050">First</span> <span m="1786570">is</span> <span m="1786810">this</span>
  <span m="1786990">robustness</span> <span m="1787680">to</span> <span m="1787910">data</span>
  <span m="1788100">set</span> <span m="1788280">shift,</span> <span m="1788670">but</span>
  <span m="1788790">there's</span> <span m="1788940">a</span> <span m="1789000">second</span>
  <span m="1789390">thing,</span> <span m="1789600">which</span> <span m="1789720">is</span>
  <span m="1789810">going</span> <span m="1790050">on</span> <span m="1790170">as</span>
  <span m="1790290">well,</span> <span m="1790500">which</span> <span m="1790680">has</span>
  <span m="1790860">to</span> <span m="1790950">do</span> <span m="1791160">with</span>
  <span m="1791700">a</span> <span m="1791760">trade-off</span> <span m="1792300">between</span>
  <span m="1792600">the</span> <span m="1792660">amount</span> <span m="1792840">of</span>
  <span m="1792930">data</span> <span m="1793230">you</span> <span m="1793410">have</span>
  <span m="1794370">and</span> <span m="1795240">the</span> <span m="1796500">complexity</span>
  <span m="1797250">of</span> <span m="1797310">the</span> <span m="1797400">prediction</span>
  <span m="1797760">problem.</span> <span m="1798960">By</span> <span m="1799140">doing</span>
  <span m="1799320">imputations,</span> <span m="1799980">sometimes</span> <span m="1800400">you</span>
  <span m="1800520">make</span> <span m="1800850">your</span> <span m="1801000">problem</span>
  <span m="1801360">look</span> <span m="1801510">a</span> <span m="1801570">bit</span>
  <span m="1801750">simpler,</span> <span m="1802320">and</span> <span m="1802440">simpler</span>
  <span m="1802830">algorithms</span> <span m="1803340">might</span> <span m="1803520">succeed</span>
  <span m="1803970">where</span> <span m="1804660">otherwise</span> <span m="1805050">they</span>
  <span m="1805170">would</span> <span m="1805290">fail</span> <span m="1805620">because</span>
  <span m="1805890">not</span> <span m="1806070">having</span> <span m="1806310">enough</span>
  <span m="1806550">data.</span> <span m="1807910">And</span> <span m="1808010">that's</span>
  <span m="1808080">something</span> <span m="1808350">that</span> <span m="1808470">you</span>
  <span m="1808620">saw</span> <span m="1809040">in</span> <span m="1809160">that</span>
  <span m="1809370">last</span> <span m="1809700">week's</span> <span m="1809890">reading.</span></p><p><span
  m="1812150">So</span> <span m="1812540">I'm</span> <span m="1812660">done</span>
  <span m="1812840">with</span> <span m="1812970">risk</span> <span m="1813100">stratification.</span>
  <span m="1814730">I'll</span> <span m="1814850">take</span> <span m="1815210">a</span>
  <span m="1815750">one</span> <span m="1816050">minute</span> <span m="1816350">breather</span>
  <span m="1816680">for</span> <span m="1816830">everyone</span> <span m="1817100">in</span>
  <span m="1817190">the</span> <span m="1817250">room,</span> <span m="1818030">and</span>
  <span m="1818150">then</span> <span m="1818330">we'll</span> <span m="1819020">start</span>
  <span m="1819410">with</span> <span m="1820280">the</span> <span m="1820640">main</span>
  <span m="1820790">topic</span> <span m="1821110">of</span> <span m="1821200">this</span>
  <span m="1821380">lecture,</span> <span m="1821590">which</span> <span m="1821690">is</span>
  <span m="1822020">physiological</span> <span m="1822500">time-series</span> <span
  m="1822890">modeling.</span> <span m="1827870">Let's</span> <span m="1828200">say</span>
  <span m="1828440">started.</span></p><p><span m="1837450">So</span> <span m="1837530">here's</span>
  <span m="1837710">a</span> <span m="1837770">baby</span> <span m="1838010">that's</span>
  <span m="1838130">not</span> <span m="1838280">doing</span> <span m="1838490">very</span>
  <span m="1838670">well.</span> <span m="1842050">This</span> <span m="1842240">baby</span>
  <span m="1842540">is</span> <span m="1842770">in</span> <span m="1843120">the</span>
  <span m="1843190">intensive</span> <span m="1843550">care</span> <span m="1843790">unit.</span>
  <span m="1848050">Maybe</span> <span m="1848330">it was</span> <span m="1848490">a</span>
  <span m="1848620">premature</span> <span m="1849130">infant.</span> <span m="1851230">Maybe</span>
  <span m="1851530">it's</span> <span m="1851650">a</span> <span m="1851680">baby</span>
  <span m="1851890">who</span> <span m="1851980">has</span> <span m="1852190">some</span>
  <span m="1854620">chronic</span> <span m="1854920">disease,</span> <span m="1856360">and,</span>
  <span m="1857110">of</span> <span m="1857170">course,</span> <span m="1857440">parents</span>
  <span m="1857740">are</span> <span m="1857770">very</span> <span m="1857980">worried.</span>
  <span m="1859510">This</span> <span m="1859660">baby</span> <span m="1860020">is</span>
  <span m="1860170">getting</span> <span m="1860440">very</span> <span m="1860770">close</span>
  <span m="1861070">monitoring.</span> <span m="1862410">It's</span> <span m="1862600">connected</span>
  <span m="1863020">to</span> <span m="1863230">lots</span> <span m="1863500">of</span>
  <span m="1863590">different</span> <span m="1863830">probes.</span></p><p><span
  m="1867031">In</span> <span m="1867430">number</span> <span m="1867700">one</span>
  <span m="1867940">here,</span> <span m="1868210">it's</span> <span m="1868330">illustrating</span>
  <span m="1869020">a</span> <span m="1869350">three</span> <span m="1869650">probe--</span>
  <span m="1870160">three</span> <span m="1870400">lead</span> <span m="1871150">ECG,</span>
  <span m="1872300">which</span> <span m="1872350">we'll be</span> <span m="1872470">talking</span>
  <span m="1872630">about</span> <span m="1872830">much</span> <span m="1873010">more,</span>
  <span m="1873490">which</span> <span m="1873670">is</span> <span m="1873730">measuring</span>
  <span m="1874060">its</span> <span m="1874180">heart,</span> <span m="1874510">how</span>
  <span m="1874660">the</span> <span m="1875050">baby's</span> <span m="1875260">heart
  is</span> <span m="1875520">doing.</span> <span m="1877270">Over</span> <span m="1878010">here,</span>
  <span m="1878380">this</span> <span m="1878830">number</span> <span m="1879040">three</span>
  <span m="1880540">is</span> <span m="1880870">something</span> <span m="1881170">attached</span>
  <span m="1881410">to</span> <span m="1881470">the</span> <span m="1881560">baby's</span>
  <span m="1881920">foot,</span> <span m="1882500">which</span> <span m="1882580">is</span>
  <span m="1882700">measuring</span> <span m="1883440">its--</span> <span m="1884206">it's</span>
  <span m="1884590">a</span> <span m="1884650">pulse</span> <span m="1885310">oximeter,</span>
  <span m="1886090">which</span> <span m="1886240">is</span> <span m="1886300">measuring</span>
  <span m="1887050">the</span> <span m="1887140">baby's</span> <span m="1887500">oxygen</span>
  <span m="1887920">saturation,</span> <span m="1888370">the amount</span> <span m="1888550">of</span>
  <span m="1888610">oxygen</span> <span m="1889000">in</span> <span m="1889090">the</span>
  <span m="1889150">blood.</span> <span m="1892780">Number</span> <span m="1893140">four</span>
  <span m="1893770">is</span> <span m="1894700">a</span> <span m="1894760">probe</span>
  <span m="1895090">which</span> <span m="1895240">is</span> <span m="1895330">measuring</span>
  <span m="1895600">the</span> <span m="1895660">baby's</span> <span m="1895900">temperature</span>
  <span m="1896560">and</span> <span m="1896650">so</span> <span m="1896890">on.</span></p><p><span
  m="1897040">And</span> <span m="1897130">so</span> <span m="1897850">we're</span>
  <span m="1898120">really</span> <span m="1898480">taking</span> <span m="1899260">really</span>
  <span m="1899530">close</span> <span m="1899860">measurements</span> <span m="1900220">of</span>
  <span m="1900280">this</span> <span m="1900430">baby,</span> <span m="1900670">because</span>
  <span m="1900910">we</span> <span m="1901030">want</span> <span m="1901120">to</span>
  <span m="1901210">understand</span> <span m="1901960">how</span> <span m="1902160">is
  this</span> <span m="1902350">baby</span> <span m="1902590">doing.</span> <span
  m="1903400">We</span> <span m="1903520">recognize</span> <span m="1904060">that</span>
  <span m="1904150">there</span> <span m="1904240">might</span> <span m="1904480">be</span>
  <span m="1905320">really</span> <span m="1905740">sudden</span> <span m="1906310">changes</span>
  <span m="1907120">in</span> <span m="1907540">the</span> <span m="1907660">baby's</span>
  <span m="1908110">state</span> <span m="1908380">of</span> <span m="1908470">health</span>
  <span m="1908800">that</span> <span m="1908890">we</span> <span m="1909010">want</span>
  <span m="1909130">to be</span> <span m="1909220">able to</span> <span m="1909310">recognize</span>
  <span m="1910060">as</span> <span m="1910360">early</span> <span m="1910660">as</span>
  <span m="1910750">possible.</span> <span m="1912650">And</span> <span m="1913240">so</span>
  <span m="1914290">behind</span> <span m="1914680">the</span> <span m="1914770">scenes,</span>
  <span m="1915310">next</span> <span m="1915550">to</span> <span m="1915610">this</span>
  <span m="1915760">baby,</span> <span m="1916240">you'll,</span> <span m="1916390">of</span>
  <span m="1916510">course,</span> <span m="1916810">have</span> <span m="1917650">a</span>
  <span m="1917710">huge</span> <span m="1917950">number</span> <span m="1918100">of</span>
  <span m="1918160">monitors,</span> <span m="1918790">each</span> <span m="1918910">of</span>
  <span m="1918970">the</span> <span m="1919060">monitors</span> <span m="1919450">showing</span>
  <span m="1919720">the</span> <span m="1919810">readouts</span> <span m="1920200">from</span>
  <span m="1920320">each</span> <span m="1920440">of</span> <span m="1920500">these</span>
  <span m="1920620">different</span> <span m="1920860">signals.</span></p><p><span
  m="1923200">And</span> <span m="1923790">this</span> <span m="1923970">type</span>
  <span m="1924120">of</span> <span m="1924210">data</span> <span m="1924930">is</span>
  <span m="1925110">really</span> <span m="1925500">prevalent</span> <span m="1926440">in</span>
  <span m="1927330">intensive</span> <span m="1927660">care</span> <span m="1927870">units,</span>
  <span m="1928530">but</span> <span m="1928770">you'll</span> <span m="1928920">also</span>
  <span m="1929190">see</span> <span m="1929520">in</span> <span m="1929640">today's</span>
  <span m="1930000">lecture</span> <span m="1930600">how</span> <span m="1931320">some</span>
  <span m="1931620">aspects</span> <span m="1932010">of</span> <span m="1932070">this</span>
  <span m="1932220">data</span> <span m="1932490">are</span> <span m="1932580">now</span>
  <span m="1932760">starting</span> <span m="1933030">to</span> <span m="1933120">make</span>
  <span m="1933330">its</span> <span m="1933510">way</span> <span m="1933780">to</span>
  <span m="1934230">the</span> <span m="1934350">home,</span> <span m="1934590">as</span>
  <span m="1934740">well.</span> <span m="1935040">So</span> <span m="1935190">for</span>
  <span m="1935280">example,</span> <span m="1935910">EKGs</span> <span m="1937890">are</span>
  <span m="1938160">now</span> <span m="1938460">available</span> <span m="1939150">on</span>
  <span m="1939690">Apple</span> <span m="1940050">and</span> <span m="1940170">Samsung</span>
  <span m="1940590">watches</span> <span m="1942090">to</span> <span m="1942450">help</span>
  <span m="1942690">understand--</span> <span m="1944250">help</span> <span m="1944450">to</span>
  <span m="1944550">help</span> <span m="1944730">with</span> <span m="1944880">diagnosis</span>
  <span m="1945510">of</span> <span m="1945660">arrhythmias,</span> <span m="1947010">even</span>
  <span m="1947250">for</span> <span m="1947340">people</span> <span m="1947550">at</span>
  <span m="1947610">home.</span></p><p><span m="1949710">And</span> <span m="1949790">so</span>
  <span m="1950000">from</span> <span m="1950210">this</span> <span m="1950330">type</span>
  <span m="1950510">of</span> <span m="1950570">data,</span> <span m="1950750">there
  are a</span> <span m="1950870">number</span> <span m="1951110">of</span> <span m="1951830">really</span>
  <span m="1952070">important</span> <span m="1952340">use</span> <span m="1952520">cases</span>
  <span m="1952760">to</span> <span m="1952820">think</span> <span m="1953030">about.</span>
  <span m="1954210">The</span> <span m="1954310">first</span> <span m="1954500">one</span>
  <span m="1954710">is</span> <span m="1955190">to</span> <span m="1955310">recognize</span>
  <span m="1955760">that</span> <span m="1955880">often</span> <span m="1956120">we're</span>
  <span m="1956210">getting</span> <span m="1956420">really</span> <span m="1956630">noisy</span>
  <span m="1956960">data,</span> <span m="1958010">and</span> <span m="1958550">we</span>
  <span m="1958700">want</span> <span m="1958850">to</span> <span m="1958910">try</span>
  <span m="1959030">to</span> <span m="1959270">infer</span> <span m="1959840">the</span>
  <span m="1959960">true</span> <span m="1960320">signal.</span> <span m="1960710">So</span>
  <span m="1960830">imagine,</span> <span m="1961340">for</span> <span m="1961460">example,</span>
  <span m="1961740">the</span> <span m="1961850">temperature</span> <span m="1962240">probe.</span>
  <span m="1963170">The</span> <span m="1963290">baby's</span> <span m="1963530">true</span>
  <span m="1963710">temperature</span> <span m="1964130">might</span> <span m="1964340">be</span>
  <span m="1965540">98.5,</span> <span m="1967100">but</span> <span m="1967430">for</span>
  <span m="1967610">whatever</span> <span m="1967910">reason--</span> <span m="1968390">we'll</span>
  <span m="1968480">see</span> <span m="1968630">a</span> <span m="1968690">few</span>
  <span m="1968870">reasons</span> <span m="1969200">here</span> <span m="1969380">today--</span>
  <span m="1970640">maybe</span> <span m="1971090">you're</span> <span m="1971210">getting</span>
  <span m="1971380">an</span> <span m="1971420">observation</span> <span m="1971900">of</span>
  <span m="1972140">93.</span></p><p><span m="1973460">And</span> <span m="1973580">you</span>
  <span m="1973640">didn't</span> <span m="1973770">know.</span> <span m="1974030">Is</span>
  <span m="1974150">that</span> <span m="1974390">actually</span> <span m="1975170">the</span>
  <span m="1975260">true</span> <span m="1975560">baby</span> <span m="1975800">temperature?</span>
  <span m="1976190">In</span> <span m="1976280">which</span> <span m="1976430">case</span>
  <span m="1976700">we--</span> <span m="1977300">it</span> <span m="1977630">would</span>
  <span m="1977720">be</span> <span m="1977990">in</span> <span m="1978320">a</span>
  <span m="1978380">lot</span> <span m="1978470">of</span> <span m="1978530">trouble.</span>
  <span m="1979250">Or</span> <span m="1979460">is</span> <span m="1979610">that</span>
  <span m="1979820">an</span> <span m="1980040">anomalous</span> <span m="1980570">reading?</span>
  <span m="1981080">So</span> <span m="1981230">we</span> <span m="1981300">like</span>
  <span m="1981440">t be able to</span> <span m="1981530">distinguish</span> <span
  m="1982010">between</span> <span m="1982250">those</span> <span m="1982370">two</span>
  <span m="1982520">things.</span> <span m="1984440">And</span> <span m="1985580">in</span>
  <span m="1985730">other</span> <span m="1985970">cases,</span> <span m="1987200">we</span>
  <span m="1987950">are</span> <span m="1988070">interested</span> <span m="1988430">in</span>
  <span m="1988500">not</span> <span m="1988700">necessarily</span> <span m="1989090">fully</span>
  <span m="1989690">understanding</span> <span m="1990290">what's</span> <span m="1990440">going</span>
  <span m="1990570">on</span> <span m="1990770">with</span> <span m="1991100">the</span>
  <span m="1991310">baby</span> <span m="1991610">along</span> <span m="1991880">each</span>
  <span m="1992030">of</span> <span m="1992090">those</span> <span m="1992330">axes,</span>
  <span m="1992900">but</span> <span m="1993050">we</span> <span m="1993200">just</span>
  <span m="1993350">want</span> <span m="1993500">to</span> <span m="1993590">use</span>
  <span m="1994250">that</span> <span m="1994610">data</span> <span m="1995660">for</span>
  <span m="1995870">predictive</span> <span m="1996320">purposes,</span> <span m="1996920">for</span>
  <span m="1997100">risk</span> <span m="1997360">stratification,</span> <span m="1997880">for</span>
  <span m="1997970">example.</span></p><p><span m="1999940">And</span> <span m="2000040">so</span>
  <span m="2000140">the</span> <span m="2000240">type</span> <span m="2000330">of</span>
  <span m="2000390">machine</span> <span m="2000720">learning</span> <span m="2000960">approach</span>
  <span m="2001200">that</span> <span m="2001290">we'll</span> <span m="2001440">take</span>
  <span m="2001710">here</span> <span m="2003030">will</span> <span m="2003210">depend</span>
  <span m="2003780">on</span> <span m="2003990">the</span> <span m="2004050">following</span>
  <span m="2004470">three</span> <span m="2004680">factors.</span> <span m="2005520">First,</span>
  <span m="2006590">do</span> <span m="2006720">we</span> <span m="2006870">have</span>
  <span m="2007080">label</span> <span m="2007440">data</span> <span m="2007710">available?</span>
  <span m="2008350">For</span> <span m="2008370">example,</span> <span m="2008860">do</span>
  <span m="2008960">we</span> <span m="2009060">know</span> <span m="2009120">the</span>
  <span m="2009240">ground</span> <span m="2009630">truth</span> <span m="2010470">of</span>
  <span m="2011250">what</span> <span m="2011400">the</span> <span m="2011490">baby's</span>
  <span m="2011910">true</span> <span m="2012270">temperature</span> <span m="2012780">was,</span>
  <span m="2014130">at</span> <span m="2014250">least</span> <span m="2014460">for</span>
  <span m="2014610">a</span> <span m="2014640">few</span> <span m="2015000">of</span>
  <span m="2015120">the</span> <span m="2015210">babies</span> <span m="2015480">in</span>
  <span m="2015570">the</span> <span m="2015630">training</span> <span m="2015990">set?</span>
  <span m="2018630">Second.</span></p><p><span m="2019680">Do</span> <span m="2019800">we</span>
  <span m="2019920">have</span> <span m="2020370">a</span> <span m="2020430">good</span>
  <span m="2020700">mechanistic</span> <span m="2021870">or</span> <span m="2022020">statistical</span>
  <span m="2022500">model</span> <span m="2023310">of</span> <span m="2023490">how</span>
  <span m="2023820">this</span> <span m="2024030">data</span> <span m="2024270">might</span>
  <span m="2024450">evolve</span> <span m="2024780">across</span> <span m="2025080">time?</span>
  <span m="2026530">We</span> <span m="2026580">know</span> <span m="2026730">a</span>
  <span m="2026790">lot</span> <span m="2026970">about</span> <span m="2027120">hearts,</span>
  <span m="2027420">for</span> <span m="2027510">example.</span> <span m="2027780">Cardiology</span>
  <span m="2028200">is</span> <span m="2028320">one</span> <span m="2028410">of</span>
  <span m="2028470">those</span> <span m="2028650">fields</span> <span m="2029040">of</span>
  <span m="2029100">medicine</span> <span m="2029550">where</span> <span m="2029910">it's</span>
  <span m="2030120">really</span> <span m="2030510">well</span> <span m="2030630">studied.</span>
  <span m="2031500">There</span> <span m="2031610">are</span> <span m="2031650">good</span>
  <span m="2031830">simulators</span> <span m="2032730">of</span> <span m="2032970">hearts,</span>
  <span m="2033360">and</span> <span m="2033450">how</span> <span m="2033570">they</span>
  <span m="2033690">beat</span> <span m="2034020">across</span> <span m="2034380">time,</span>
  <span m="2034710">and</span> <span m="2034800">how</span> <span m="2034950">that</span>
  <span m="2035100">affects</span> <span m="2035490">the</span> <span m="2035710">electrical</span>
  <span m="2036240">stimulation</span> <span m="2038370">across</span> <span m="2038670">the</span>
  <span m="2038760">body.</span></p><p><span m="2041150">And</span> <span m="2041660">if</span>
  <span m="2041810">we</span> <span m="2041960">have</span> <span m="2042540">these</span>
  <span m="2042920">good</span> <span m="2043400">mechanistic</span> <span m="2043970">or</span>
  <span m="2044090">statistical</span> <span m="2044360">models,</span> <span m="2044750">that</span>
  <span m="2044840">can</span> <span m="2044990">often</span> <span m="2045770">allow</span>
  <span m="2046190">one</span> <span m="2046400">to</span> <span m="2046520">trade</span>
  <span m="2046850">off</span> <span m="2047480">not</span> <span m="2047690">having</span>
  <span m="2048020">much</span> <span m="2048260">label</span> <span m="2048530">data,</span>
  <span m="2048800">or</span> <span m="2048860">just</span> <span m="2049010">not</span>
  <span m="2049190">having</span> <span m="2049460">much</span> <span m="2049670">data</span>
  <span m="2049909">period.</span> <span m="2051540">And</span> <span m="2052080">it's</span>
  <span m="2052230">really</span> <span m="2052500">these</span> <span m="2052739">three</span>
  <span m="2052949">points</span> <span m="2053850">which</span> <span m="2054060">I</span>
  <span m="2054150">want</span> <span m="2054389">to</span> <span m="2054480">illustrate</span>
  <span m="2055110">the</span> <span m="2055170">extremes</span> <span m="2055920">of</span>
  <span m="2056040">in</span> <span m="2056130">today's</span> <span m="2056429">lecture--</span>
  <span m="2057210">what</span> <span m="2057400">do</span> <span m="2057449">you</span>
  <span m="2057540">do</span> <span m="2057690">when</span> <span m="2057840">you</span>
  <span m="2057929">don't</span> <span m="2058170">have</span> <span m="2058320">much</span>
  <span m="2058560">data,</span> <span m="2058830">and</span> <span m="2058889">what</span>
  <span m="2059040">you</span> <span m="2059130">do</span> <span m="2059489">when--</span>
  <span m="2059639">what you</span> <span m="2059730">can</span> <span m="2060000">do</span>
  <span m="2060150">when</span> <span m="2060239">you</span> <span m="2060330">have</span>
  <span m="2060420">a</span> <span m="2060480">ton</span> <span m="2060690">of</span>
  <span m="2060780">data.</span> <span m="2061395">And</span> <span m="2061710">I</span>
  <span m="2061800">think</span> <span m="2061949">it's</span> <span m="2062070">going</span>
  <span m="2062159">to</span> <span m="2062250">be</span> <span m="2062340">really</span>
  <span m="2062699">informative</span> <span m="2063389">for</span> <span m="2063780">us</span>
  <span m="2064110">as</span> <span m="2064260">we</span> <span m="2064380">go</span>
  <span m="2064530">out</span> <span m="2064679">into</span> <span m="2064860">the</span>
  <span m="2064920">world</span> <span m="2065190">and</span> <span m="2065280">will</span>
  <span m="2065550">have</span> <span m="2065730">to</span> <span m="2065820">tackle</span>
  <span m="2066179">each</span> <span m="2066300">of</span> <span m="2066360">those</span>
  <span m="2066510">two</span> <span m="2066630">settings.</span></p><p><span m="2070159">So</span>
  <span m="2070350">here's</span> <span m="2070560">an</span> <span m="2070620">example</span>
  <span m="2071100">of</span> <span m="2071760">two</span> <span m="2071940">different</span>
  <span m="2072750">babies</span> <span m="2073170">with</span> <span m="2073320">very</span>
  <span m="2073500">different</span> <span m="2073739">trajectories.</span> <span
  m="2075150">One</span> <span m="2075889">in</span> <span m="2076139">the</span>
  <span m="2076230">x-axis</span> <span m="2076710">here</span> <span m="2076889">is</span>
  <span m="2077010">time</span> <span m="2077760">in</span> <span m="2077940">seconds.</span>
  <span m="2078449">The</span> <span m="2078570">y-axis</span> <span m="2080370">here--</span>
  <span m="2081690">I</span> <span m="2081719">think</span> <span m="2081900">seconds,</span>
  <span m="2082219">maybe</span> <span m="2082409">minutes.</span> <span m="2082980">The</span>
  <span m="2083790">y-axis</span> <span m="2084270">here</span> <span m="2084570">is</span>
  <span m="2084840">beats</span> <span m="2085080">per</span> <span m="2085199">minute</span>
  <span m="2085530">of</span> <span m="2085620">the</span> <span m="2085679">baby's</span>
  <span m="2085920">heart</span> <span m="2086130">rate,</span> <span m="2086909">and</span>
  <span m="2087420">you</span> <span m="2087480">see</span> <span m="2087690">in</span>
  <span m="2087780">some</span> <span m="2087989">cases</span> <span m="2089310">it's</span>
  <span m="2090300">really</span> <span m="2090630">fluctuating</span> <span m="2091230">a</span>
  <span m="2091260">lot</span> <span m="2091530">up</span> <span m="2091679">and</span>
  <span m="2091800">down.</span> <span m="2092190">In</span> <span m="2092280">some</span>
  <span m="2092400">cases,</span> <span m="2092820">it's</span> <span m="2092880">sort</span>
  <span m="2093040">of</span> <span m="2093150">going</span> <span m="2093360">in</span>
  <span m="2093449">a</span> <span m="2093510">similar--</span> <span m="2093870">in</span>
  <span m="2094050">one</span> <span m="2094230">direction,</span> <span m="2094650">and</span>
  <span m="2094750">in</span> <span m="2094870">all</span> <span m="2095159">cases,</span>
  <span m="2096449">the</span> <span m="2097230">short</span> <span m="2097650">term</span>
  <span m="2098010">observations</span> <span m="2098700">are</span> <span m="2098790">very</span>
  <span m="2099090">different</span> <span m="2099420">from</span> <span m="2099570">the</span>
  <span m="2099660">long</span> <span m="2100260">range</span> <span m="2100740">trajectories.</span></p><p><span
  m="2104010">So</span> <span m="2104060">the</span> <span m="2104120">first</span>
  <span m="2104360">problem</span> <span m="2104570">that</span> <span m="2104660">I</span>
  <span m="2104750">want</span> <span m="2104930">us</span> <span m="2105020">to</span>
  <span m="2105110">think</span> <span m="2105380">about</span> <span m="2106130">is</span>
  <span m="2106340">one</span> <span m="2106640">of</span> <span m="2107510">trying</span>
  <span m="2107900">to</span> <span m="2109460">understand,</span> <span m="2110450">how</span>
  <span m="2110660">do</span> <span m="2110720">we</span> <span m="2110840">deconvolve</span>
  <span m="2111740">between</span> <span m="2112640">the</span> <span m="2112760">truth</span>
  <span m="2113390">of</span> <span m="2113450">what's</span> <span m="2113630">going</span>
  <span m="2113770">on</span> <span m="2113870">with,</span> <span m="2114380">for</span>
  <span m="2114500">example,</span> <span m="2114840">the</span> <span m="2114940">patient's</span>
  <span m="2115100">blood</span> <span m="2115280">pressure</span> <span m="2115680">or</span>
  <span m="2115790">oxygen</span> <span m="2116870">versus</span> <span m="2117800">interventions</span>
  <span m="2118730">that</span> <span m="2118820">are</span> <span m="2118910">happening</span>
  <span m="2119330">to</span> <span m="2119450">them?</span> <span m="2120390">So</span>
  <span m="2120440">on</span> <span m="2120530">the</span> <span m="2120620">bottom</span>
  <span m="2120950">here,</span> <span m="2121230">I'm</span> <span m="2121330">showing</span>
  <span m="2121580">examples</span> <span m="2122030">of</span> <span m="2122090">interventions.</span></p><p><span
  m="2124750">Here</span> <span m="2126230">in</span> <span m="2126400">this</span>
  <span m="2126580">oxygen</span> <span m="2127000">uptake,</span> <span m="2127490">we</span>
  <span m="2127590">notice</span> <span m="2127810">how</span> <span m="2128470">between</span>
  <span m="2129070">roughly</span> <span m="2129370">1,000</span> <span m="2129820">and
  2,000</span> <span m="2130270">seconds</span> <span m="2130660">suddenly</span>
  <span m="2131330">there's</span> <span m="2131440">no</span> <span m="2131590">signal</span>
  <span m="2131950">whatsoever.</span> <span m="2132255">And</span> <span m="2132560">that's</span>
  <span m="2132700">an</span> <span m="2132760">example</span> <span m="2133150">of</span>
  <span m="2133250">what's</span> <span m="2133300">called</span> <span m="2133480">dropout.</span>
  <span m="2136520">Over</span> <span m="2136760">here,</span> <span m="2137810">we</span>
  <span m="2137960">see</span> <span m="2138110">a</span> <span m="2138170">different</span>
  <span m="2138530">type</span> <span m="2138830">of--</span> <span m="2139650">the</span>
  <span m="2139760">effect</span> <span m="2140010">of</span> <span m="2140090">a</span>
  <span m="2140150">different</span> <span m="2140390">intervention,</span> <span
  m="2142430">which</span> <span m="2142610">is</span> <span m="2142730">due</span>
  <span m="2142970">to</span> <span m="2143330">a</span> <span m="2143420">probe</span>
  <span m="2143750">recalibration.</span> <span m="2144770">Now,</span> <span m="2145190">at</span>
  <span m="2145250">that</span> <span m="2145400">time,</span> <span m="2145790">there</span>
  <span m="2145910">was</span> <span m="2146330">a</span> <span m="2146390">drop</span>
  <span m="2146570">out</span> <span m="2146870">followed</span> <span m="2147290">by</span>
  <span m="2148010">a</span> <span m="2148100">sudden</span> <span m="2148430">change</span>
  <span m="2149180">in</span> <span m="2149300">the</span> <span m="2149390">values,</span>
  <span m="2150170">and</span> <span m="2150260">that's</span> <span m="2150470">really</span>
  <span m="2150710">happening</span> <span m="2151070">due to</span> <span m="2151190">a
  recalibration</span> <span m="2151920">step.</span> <span m="2152720">And in</span>
  <span m="2152840">both</span> <span m="2153050">of these</span> <span m="2153260">cases,</span>
  <span m="2155450">what's</span> <span m="2155710">going</span> <span m="2155830">on</span>
  <span m="2155920">with</span> <span m="2156190">the</span> <span m="2156550">individual</span>
  <span m="2157390">might</span> <span m="2157720">be</span> <span m="2157870">relatively</span>
  <span m="2158290">constant</span> <span m="2158680">across</span> <span m="2158950">time,</span>
  <span m="2159350">but</span> <span m="2159450">what's</span> <span m="2159490">being</span>
  <span m="2159670">observed</span> <span m="2160090">is</span> <span m="2160220">dramatically</span>
  <span m="2160750">affected</span> <span m="2161110">by</span> <span m="2161260">those</span>
  <span m="2161410">interventions.</span></p><p><span m="2164240">So</span> <span
  m="2164390">we</span> <span m="2164470">want</span> <span m="2164570">to</span>
  <span m="2164680">ask</span> <span m="2164820">the</span> <span m="2164900">question,</span>
  <span m="2165840">can</span> <span m="2165950">we</span> <span m="2166070">identify</span>
  <span m="2167000">those</span> <span m="2167300">artifactual</span> <span m="2167870">processes?</span>
  <span m="2168890">Can</span> <span m="2169070">we</span> <span m="2169160">identify</span>
  <span m="2169850">that</span> <span m="2170000">these</span> <span m="2170180">interventions</span>
  <span m="2170690">were</span> <span m="2170780">happening</span> <span m="2171080">at</span>
  <span m="2171170">those</span> <span m="2171350">points</span> <span m="2171620">in</span>
  <span m="2171740">time?</span> <span m="2175680">And</span> <span m="2176110">then,</span>
  <span m="2176560">if</span> <span m="2176740">we</span> <span m="2176830">could</span>
  <span m="2176980">identify</span> <span m="2177580">them,</span> <span m="2178000">then</span>
  <span m="2178180">we</span> <span m="2178270">could</span> <span m="2178360">potentially</span>
  <span m="2179140">subtract</span> <span m="2179950">their</span> <span m="2180190">effect</span>
  <span m="2180610">out.</span> <span m="2181120">So</span> <span m="2181900">we</span>
  <span m="2184150">could</span> <span m="2184660">impute</span> <span m="2185500">the</span>
  <span m="2185710">data,</span> <span m="2186160">which</span> <span m="2186370">we</span>
  <span m="2186490">know--</span> <span m="2186850">now</span> <span m="2187210">know</span>
  <span m="2187460">to</span> <span m="2187570">be</span> <span m="2187690">missing,</span>
  <span m="2188440">and</span> <span m="2188530">then</span> <span m="2188980">have</span>
  <span m="2189160">this</span> <span m="2189340">much</span> <span m="2189550">higher</span>
  <span m="2189910">quality</span> <span m="2190390">signal</span> <span m="2191050">used</span>
  <span m="2191530">for</span> <span m="2191710">some</span> <span m="2191920">downstream</span>
  <span m="2192400">predictive</span> <span m="2192790">purpose,</span> <span m="2193130">for</span>
  <span m="2193240">example.</span></p><p><span m="2194910">And</span> <span m="2195010">the</span>
  <span m="2195020">second</span> <span m="2195320">reason</span> <span m="2195590">why</span>
  <span m="2196220">this</span> <span m="2196400">can</span> <span m="2196520">be</span>
  <span m="2196610">really</span> <span m="2196790">important</span> <span m="2197510">is</span>
  <span m="2197960">to</span> <span m="2198110">tackle</span> <span m="2199040">this</span>
  <span m="2199190">problem</span> <span m="2199580">called</span> <span m="2199860">alarm</span>
  <span m="2200300">fatigue.</span> <span m="2203370">Alarm</span> <span m="2203640">fatigue</span>
  <span m="2204090">is</span> <span m="2204240">one</span> <span m="2204390">of</span>
  <span m="2204450">the</span> <span m="2204510">most</span> <span m="2204780">important</span>
  <span m="2205470">challenges</span> <span m="2206130">facing</span> <span m="2207030">medicine</span>
  <span m="2207450">today.</span> <span m="2208500">As</span> <span m="2208680">we</span>
  <span m="2208800">get</span> <span m="2209130">better</span> <span m="2209520">and</span>
  <span m="2209640">better</span> <span m="2210600">in</span> <span m="2211080">doing</span>
  <span m="2211440">risk</span> <span m="2211650">stratification,</span> <span m="2212370">as</span>
  <span m="2212490">we</span> <span m="2212610">come</span> <span m="2212820">up</span>
  <span m="2212910">with</span> <span m="2213120">more</span> <span m="2213630">and</span>
  <span m="2213720">more</span> <span m="2214950">diagnostic</span> <span m="2215760">tools</span>
  <span m="2216990">and</span> <span m="2217080">tests,</span> <span m="2218700">that</span>
  <span m="2219000">means</span> <span m="2219720">these</span> <span m="2219960">red</span>
  <span m="2220230">flags</span> <span m="2220710">are</span> <span m="2220770">being</span>
  <span m="2220980">raised</span> <span m="2221490">more</span> <span m="2221790">and</span>
  <span m="2221880">more</span> <span m="2222090">often.</span> <span m="2223690">And</span>
  <span m="2223850">each</span> <span m="2224090">one</span> <span m="2224240">of</span>
  <span m="2224360">these</span> <span m="2224990">has</span> <span m="2225530">some</span>
  <span m="2225770">associated</span> <span m="2226280">false</span> <span m="2226610">positive</span>
  <span m="2227240">rate</span> <span m="2228170">for</span> <span m="2228410">it.</span>
  <span m="2229800">And</span> <span m="2230510">so</span> <span m="2232010">the</span>
  <span m="2232130">more</span> <span m="2232400">tests</span> <span m="2232730">you</span>
  <span m="2232880">have--</span> <span m="2233510">suppose</span> <span m="2233870">the</span>
  <span m="2233930">false</span> <span m="2234170">positive</span> <span m="2234560">rate</span>
  <span m="2234800">is</span> <span m="2235250">kept</span> <span m="2235520">constant--</span>
  <span m="2236400">the</span> <span m="2236500">more</span> <span m="2236570">tests</span>
  <span m="2236870">you</span> <span m="2236990">have,</span> <span m="2237480">the</span>
  <span m="2237500">more</span> <span m="2237710">likely</span> <span m="2238160">it</span>
  <span m="2238280">is</span> <span m="2238520">that</span> <span m="2238850">the</span>
  <span m="2239000">union</span> <span m="2239450">of</span> <span m="2239630">all</span>
  <span m="2239850">of</span> <span m="2239900">those</span> <span m="2240140">is</span>
  <span m="2240260">going</span> <span m="2240500">to</span> <span m="2240620">be</span>
  <span m="2240770">some</span> <span m="2242480">error.</span></p><p><span m="2244568">And</span>
  <span m="2245000">so</span> <span m="2245180">when</span> <span m="2245390">you're</span>
  <span m="2245480">in an</span> <span m="2245570">intensive</span> <span m="2246050">care</span>
  <span m="2246320">unit,</span> <span m="2247540">there</span> <span m="2247700">are</span>
  <span m="2247730">alarms</span> <span m="2248150">going</span> <span m="2248300">off</span>
  <span m="2248480">all</span> <span m="2248570">the</span> <span m="2248660">time.</span>
  <span m="2249500">And</span> <span m="2249950">something</span> <span m="2250310">that</span>
  <span m="2250430">happens</span> <span m="2250850">is</span> <span m="2250940">that</span>
  <span m="2251060">nurses</span> <span m="2251450">end</span> <span m="2251570">up</span>
  <span m="2251630">starting</span> <span m="2251930">to</span> <span m="2252050">ignore</span>
  <span m="2252380">those</span> <span m="2252560">alarms,</span> <span m="2252980">because</span>
  <span m="2254180">so</span> <span m="2254540">often</span> <span m="2255110">those</span>
  <span m="2255320">alarms</span> <span m="2255710">are</span> <span m="2255980">false</span>
  <span m="2256430">positives,</span> <span m="2257480">are</span> <span m="2258200">due</span>
  <span m="2258500">to,</span> <span m="2258780">for</span> <span m="2258880">example,</span>
  <span m="2259160">artifacts</span> <span m="2259700">like</span> <span m="2259850">what</span>
  <span m="2259970">I'm</span> <span m="2260090">showing</span> <span m="2260360">you</span>
  <span m="2260480">here.</span></p><p><span m="2262120">And</span> <span m="2262220">so</span>
  <span m="2262320">if</span> <span m="2262430">we</span> <span m="2262580">had</span>
  <span m="2262730">techniques,</span> <span m="2263300">such</span> <span m="2263510">as</span>
  <span m="2263600">the</span> <span m="2263660">ones</span> <span m="2263870">we'll</span>
  <span m="2263960">talk</span> <span m="2264170">about</span> <span m="2264800">right</span>
  <span m="2265040">now,</span> <span m="2265850">which</span> <span m="2266060">could</span>
  <span m="2266210">recognize</span> <span m="2267320">when,</span> <span m="2267680">for</span>
  <span m="2267860">example,</span> <span m="2268430">the</span> <span m="2268520">sudden</span>
  <span m="2268940">drop</span> <span m="2269360">in</span> <span m="2269450">a</span>
  <span m="2269480">patient's</span> <span m="2269840">heart</span> <span m="2270140">rate</span>
  <span m="2270470">is</span> <span m="2270680">due</span> <span m="2271070">to</span>
  <span m="2272090">an</span> <span m="2272270">artifact</span> <span m="2272960">and</span>
  <span m="2273110">not</span> <span m="2273740">due</span> <span m="2273980">to</span>
  <span m="2274040">the</span> <span m="2274130">patient's</span> <span m="2274490">true</span>
  <span m="2274730">heart</span> <span m="2274940">rate</span> <span m="2275090">dropping--</span>
  <span m="2277070">if</span> <span m="2277160">we</span> <span m="2277220">had</span>
  <span m="2277310">enough</span> <span m="2277490">confidence</span> <span m="2278090">in</span>
  <span m="2278210">that--</span> <span m="2278500">in</span> <span m="2278630">distinguishing</span>
  <span m="2279290">those</span> <span m="2279440">two</span> <span m="2279560">things,</span>
  <span m="2279910">then</span> <span m="2279920">we</span> <span m="2280010">might</span>
  <span m="2280280">not</span> <span m="2280760">decide</span> <span m="2281120">to</span>
  <span m="2281240">raise</span> <span m="2281510">that</span> <span m="2281660">red</span>
  <span m="2281870">flag.</span> <span m="2283150">And</span> <span m="2283280">that</span>
  <span m="2283520">might</span> <span m="2284060">reduce</span> <span m="2284510">the</span>
  <span m="2284600">amount</span> <span m="2284900">of</span> <span m="2284990">false</span>
  <span m="2285320">alarms,</span> <span m="2286430">and</span> <span m="2286580">that</span>
  <span m="2286910">then</span> <span m="2287210">might</span> <span m="2287450">reduce</span>
  <span m="2287780">the</span> <span m="2287840">amount</span> <span m="2288080">of</span>
  <span m="2288200">alarm</span> <span m="2288590">fatigue.</span> <span m="2289150">And</span>
  <span m="2289280">that</span> <span m="2289460">could</span> <span m="2289610">have</span>
  <span m="2289790">a</span> <span m="2289850">very</span> <span m="2290390">big</span>
  <span m="2290570">impact</span> <span m="2291170">on</span> <span m="2291350">health</span>
  <span m="2291580">care.</span></p><p><span m="2295980">So</span> <span m="2296270">the</span>
  <span m="2296360">technique</span> <span m="2296780">which</span> <span m="2296900">we'll</span>
  <span m="2297140">talk</span> <span m="2297410">about</span> <span m="2297830">today</span>
  <span m="2299150">goes</span> <span m="2299420">by</span> <span m="2299510">the</span>
  <span m="2299600">name</span> <span m="2299960">of</span> <span m="2300230">switching</span>
  <span m="2300800">linear</span> <span m="2301130">dynamical</span> <span m="2301610">systems.</span>
  <span m="2304170">Who</span> <span m="2304410">here</span> <span m="2304680">has</span>
  <span m="2304800">seen</span> <span m="2305010">a</span> <span m="2305070">picture</span>
  <span m="2305460">like</span> <span m="2305640">this</span> <span m="2305820">on--</span>
  <span m="2306090">this</span> <span m="2306330">picture</span> <span m="2306600">on</span>
  <span m="2306690">the</span> <span m="2306750">bottom</span> <span m="2307050">before.</span>
  <span m="2309630">About</span> <span m="2310170">half</span> <span m="2310530">of</span>
  <span m="2310620">the</span> <span m="2310710">room.</span> <span m="2312240">So</span>
  <span m="2312450">for</span> <span m="2312570">the</span> <span m="2312630">other</span>
  <span m="2312840">half</span> <span m="2313080">of</span> <span m="2313140">the</span>
  <span m="2313230">room,</span> <span m="2313590">I'm</span> <span m="2313710">going</span>
  <span m="2313920">to</span> <span m="2314010">give</span> <span m="2314190">a</span>
  <span m="2314870">bit</span> <span m="2315090">of</span> <span m="2315180">a</span>
  <span m="2315360">recap</span> <span m="2316620">into</span> <span m="2317190">probabilistic</span>
  <span m="2317730">modeling.</span> <span m="2318960">All</span> <span m="2319230">of</span>
  <span m="2319320">you</span> <span m="2319890">are</span> <span m="2320040">now</span>
  <span m="2320280">familiar</span> <span m="2321930">with</span> <span m="2322560">general</span>
  <span m="2323010">probabilities.</span> <span m="2323830">So</span> <span m="2323880">you're</span>
  <span m="2324030">used</span> <span m="2324270">to</span> <span m="2324390">thinking</span>
  <span m="2324870">about,</span> <span m="2325390">for</span> <span m="2325440">example,</span>
  <span m="2328230">univariate</span> <span m="2329220">Gaussian</span> <span m="2329640">distributions.</span></p><p><span
  m="2331230">We</span> <span m="2331350">talked</span> <span m="2331680">about</span>
  <span m="2331920">how</span> <span m="2332070">one</span> <span m="2332550">could</span>
  <span m="2332730">model</span> <span m="2333060">survival,</span> <span m="2333970">which</span>
  <span m="2334050">was</span> <span m="2334230">an</span> <span m="2334320">example</span>
  <span m="2334860">of</span> <span m="2334950">such</span> <span m="2335250">a</span>
  <span m="2335640">distribution,</span> <span m="2337440">but</span> <span m="2337950">for</span>
  <span m="2338100">today's</span> <span m="2338430">lecture,</span> <span m="2338980">we're</span>
  <span m="2339000">going</span> <span m="2339180">to</span> <span m="2339270">be</span>
  <span m="2339330">thinking</span> <span m="2339720">now</span> <span m="2339900">about</span>
  <span m="2340080">multivariate</span> <span m="2340860">probability</span> <span
  m="2341130">distributions.</span> <span m="2341820">In</span> <span m="2341910">particular,</span>
  <span m="2342490">we'll</span> <span m="2342510">be</span> <span m="2342600">thinking</span>
  <span m="2343050">about</span> <span m="2343290">how</span> <span m="2344690">a</span>
  <span m="2344850">patient's</span> <span m="2345330">state--</span> <span m="2345870">let's</span>
  <span m="2346080">say</span> <span m="2346260">their</span> <span m="2346410">true</span>
  <span m="2346860">blood</span> <span m="2347160">pressure--</span> <span m="2348120">evolves</span>
  <span m="2348750">across</span> <span m="2349110">time.</span> <span m="2349990">And</span>
  <span m="2350090">so</span> <span m="2350130">now</span> <span m="2350370">we're</span>
  <span m="2350520">interested</span> <span m="2350940">in</span> <span m="2351060">not</span>
  <span m="2351360">just</span> <span m="2352830">the</span> <span m="2353400">random</span>
  <span m="2353730">variable</span> <span m="2354570">at</span> <span m="2354750">one</span>
  <span m="2354990">point</span> <span m="2355170">in</span> <span m="2355260">time,</span>
  <span m="2355560">but</span> <span m="2355710">that</span> <span m="2355900">same
  random</span> <span m="2356140">variable</span> <span m="2356740">at</span> <span
  m="2356840">the</span> <span m="2356940">second</span> <span m="2357120">point</span>
  <span m="2357290">in</span> <span m="2357330">time,</span> <span m="2357570">third</span>
  <span m="2357990">point</span> <span m="2358170">in</span> <span m="2358260">time,</span>
  <span m="2358500">fourth</span> <span m="2358830">point</span> <span m="2359010">in</span>
  <span m="2359120">time,</span> <span m="2359310">fifth</span> <span m="2359560">point
  in</span> <span m="2359790">time,</span> <span m="2360000">and</span> <span m="2360090">so</span>
  <span m="2360300">on.</span></p><p><span m="2361630">So</span> <span m="2361680">what</span>
  <span m="2361800">I'm</span> <span m="2361920">showing</span> <span m="2362220">you</span>
  <span m="2362340">here</span> <span m="2362640">is</span> <span m="2362790">known</span>
  <span m="2363030">as</span> <span m="2363150">a</span> <span m="2363210">graphical</span>
  <span m="2363660">model,</span> <span m="2364180">also</span> <span m="2364500">known</span>
  <span m="2364770">as</span> <span m="2364890">a</span> <span m="2364950">Bayesian</span>
  <span m="2365280">network.</span> <span m="2366270">And</span> <span m="2366390">it's</span>
  <span m="2366660">one</span> <span m="2366990">way</span> <span m="2367200">of</span>
  <span m="2367350">illustrating</span> <span m="2367950">a</span> <span m="2368010">multivariate</span>
  <span m="2368700">probability</span> <span m="2369050">distribution</span> <span
  m="2369600">that</span> <span m="2369720">has</span> <span m="2370020">particular</span>
  <span m="2370650">conditional</span> <span m="2371100">independence</span> <span
  m="2371460">properties.</span> <span m="2373490">Specifically,</span> <span m="2376050">in</span>
  <span m="2376200">this</span> <span m="2376440">model,</span> <span m="2379910">one</span>
  <span m="2380300">node</span> <span m="2380690">corresponds</span> <span m="2381170">to</span>
  <span m="2381260">one</span> <span m="2381470">random</span> <span m="2381710">variable.</span>
  <span m="2382260">So</span> <span m="2382310">this</span> <span m="2382490">is</span>
  <span m="2382610">describing</span> <span m="2383300">a</span> <span m="2383450">joint</span>
  <span m="2383810">distribution</span> <span m="2384740">on</span> <span m="2385670">x1</span>
  <span m="2386840">through</span> <span m="2387740">x6,</span> <span m="2390860">y1</span>
  <span m="2392240">through</span> <span m="2393110">y6.</span> <span m="2395170">So</span>
  <span m="2395380">it's</span> <span m="2395530">this</span> <span m="2395710">multivariate</span>
  <span m="2396210">distribution</span> <span m="2396700">on</span> <span m="2396940">12</span>
  <span m="2397510">random</span> <span m="2397840">variables.</span></p><p><span
  m="2400570">The</span> <span m="2400690">fact</span> <span m="2401050">that</span>
  <span m="2401260">this</span> <span m="2401530">is</span> <span m="2401770">shaded</span>
  <span m="2402400">in</span> <span m="2403180">simply</span> <span m="2403600">denotes</span>
  <span m="2404050">that,</span> <span m="2404380">at</span> <span m="2404590">test</span>
  <span m="2404980">time,</span> <span m="2405310">when</span> <span m="2405460">we</span>
  <span m="2405580">use</span> <span m="2405940">these</span> <span m="2406180">models,</span>
  <span m="2406540">typically</span> <span m="2407110">these</span> <span m="2407410">y</span>
  <span m="2407830">variables</span> <span m="2408280">are</span> <span m="2408370">observed.</span>
  <span m="2409780">Whereas</span> <span m="2410650">our</span> <span m="2410830">goal</span>
  <span m="2411160">is</span> <span m="2411310">usually</span> <span m="2411700">to</span>
  <span m="2411850">infer</span> <span m="2412600">the</span> <span m="2412750">x</span>
  <span m="2412990">variables.</span> <span m="2413410">Those</span> <span m="2413560">are</span>
  <span m="2413620">typically</span> <span m="2413980">unobserved,</span> <span m="2414700">meaning</span>
  <span m="2415030">that</span> <span m="2415270">our</span> <span m="2415390">typical</span>
  <span m="2416290">task</span> <span m="2416950">is</span> <span m="2417100">one</span>
  <span m="2417310">of</span> <span m="2417400">doing</span> <span m="2417640">posterior</span>
  <span m="2418310">inference</span> <span m="2419230">to</span> <span m="2419380">infer</span>
  <span m="2420340">the</span> <span m="2420520">x's</span> <span m="2421420">given</span>
  <span m="2422140">the</span> <span m="2422380">y's.</span></p><p><span m="2425470">Now,</span>
  <span m="2425710">associated</span> <span m="2426310">with</span> <span m="2426640">this</span>
  <span m="2427300">graph,</span> <span m="2428620">I</span> <span m="2428680">already</span>
  <span m="2428860">told</span> <span m="2429070">you</span> <span m="2429160">the</span>
  <span m="2429250">nodes</span> <span m="2429760">correspond</span> <span m="2430180">to</span>
  <span m="2430270">random</span> <span m="2430510">variables.</span> <span m="2431740">The</span>
  <span m="2431860">graph</span> <span m="2432370">tells</span> <span m="2432760">us</span>
  <span m="2432940">how</span> <span m="2433300">is</span> <span m="2433450">this</span>
  <span m="2433690">joint</span> <span m="2433990">distribution</span> <span m="2434620">factorized.</span>
  <span m="2436330">In</span> <span m="2436390">particular,</span> <span m="2438290">it's</span>
  <span m="2438310">going</span> <span m="2438490">to</span> <span m="2438550">be</span>
  <span m="2438640">factorized</span> <span m="2441130">in</span> <span m="2441250">the</span>
  <span m="2441310">following</span> <span m="2441730">way--</span> <span m="2442240">as</span>
  <span m="2442420">the</span> <span m="2442510">product</span> <span m="2443140">over</span>
  <span m="2443560">random</span> <span m="2443920">variables</span> <span m="2445210">of</span>
  <span m="2445570">the</span> <span m="2445690">probability</span> <span m="2446890">of</span>
  <span m="2447370">the</span> <span m="2447930">i-th</span> <span m="2448390">random</span>
  <span m="2448540">variable.</span> <span m="2449000">I'm</span> <span m="2449100">going</span>
  <span m="2449200">to</span> <span m="2449300">use</span> <span m="2449320">z</span>
  <span m="2449740">to</span> <span m="2449890">just</span> <span m="2450100">denote</span>
  <span m="2450280">a</span> <span m="2450340">random</span> <span m="2450550">variable.</span>
  <span m="2451840">Think</span> <span m="2452170">of</span> <span m="2452260">z</span>
  <span m="2452530">as</span> <span m="2452680">the</span> <span m="2452800">union</span>
  <span m="2453250">of</span> <span m="2453490">x</span> <span m="2453790">and</span>
  <span m="2453940">y.</span> <span m="2455680">zi</span> <span m="2457270">conditioned</span>
  <span m="2458170">on</span> <span m="2458470">the</span> <span m="2458740">parents--</span>
  <span m="2459610">the</span> <span m="2459760">values</span> <span m="2460360">of</span>
  <span m="2460510">the</span> <span m="2460630">parents</span> <span m="2461380">of</span>
  <span m="2461530">zi.</span></p><p><span m="2465820">So</span> <span m="2466030">I'm</span>
  <span m="2466120">going</span> <span m="2466300">to</span> <span m="2466420">assume</span>
  <span m="2466840">this</span> <span m="2467680">factorization,</span> <span m="2470080">and</span>
  <span m="2470530">in</span> <span m="2470650">particular</span> <span m="2471190">for</span>
  <span m="2471460">this</span> <span m="2472360">graphical</span> <span m="2472810">model,</span>
  <span m="2473560">which</span> <span m="2473800">goes</span> <span m="2474010">by</span>
  <span m="2474130">the</span> <span m="2474220">name</span> <span m="2474400">of</span>
  <span m="2474490">a</span> <span m="2474550">Markov</span> <span m="2475150">model,</span>
  <span m="2475870">it</span> <span m="2475960">has</span> <span m="2476140">a</span>
  <span m="2476200">very</span> <span m="2476440">specific</span> <span m="2476920">factorization.</span>
  <span m="2478810">And</span> <span m="2479020">we're</span> <span m="2479200">just</span>
  <span m="2479350">going</span> <span m="2479460">to</span> <span m="2479530">read</span>
  <span m="2479800">it</span> <span m="2479920">off</span> <span m="2480310">from</span>
  <span m="2480550">this</span> <span m="2480730">definition.</span> <span m="2482180">So</span>
  <span m="2482800">we're</span> <span m="2482910">going</span> <span m="2482990">to</span>
  <span m="2483100">go</span> <span m="2483250">in</span> <span m="2483370">order--</span>
  <span m="2483760">first</span> <span m="2484750">x1,</span> <span m="2485560">then</span>
  <span m="2485770">y1,</span> <span m="2486340">then</span> <span m="2486520">x2,</span>
  <span m="2487000">then</span> <span m="2487180">y2,</span> <span m="2487660">and</span>
  <span m="2487750">so</span> <span m="2487960">on,</span> <span m="2488300">which</span>
  <span m="2488410">is</span> <span m="2489040">going</span> <span m="2489370">based</span>
  <span m="2489730">on</span> <span m="2490420">a</span> <span m="2494080">root</span>
  <span m="2494650">to</span> <span m="2496030">children</span> <span m="2496630">transversal</span>
  <span m="2497065">of</span> <span m="2497500">this</span> <span m="2497650">graph.</span></p><p><span
  m="2499340">So</span> <span m="2499370">the</span> <span m="2499460">first</span>
  <span m="2499700">random</span> <span m="2499910">variable</span> <span m="2500540">is</span>
  <span m="2501800">x1.</span> <span m="2504410">Second</span> <span m="2504680">variable</span>
  <span m="2505250">is</span> <span m="2505630">y2,</span> <span m="2507140">and</span>
  <span m="2507830">what</span> <span m="2508070">are</span> <span m="2508160">the</span>
  <span m="2508280">parents</span> <span m="2508910">of</span> <span m="2509710">y--</span>
  <span m="2510230">sorry,</span> <span m="2510440">what</span> <span m="2510560">are</span>
  <span m="2510620">the</span> <span m="2510680">parents</span> <span m="2511010">of</span>
  <span m="2511130">y1.</span> <span m="2512000">Everyone</span> <span m="2512230">can</span>
  <span m="2512330">say</span> <span m="2512480">out</span> <span m="2512570">loud.</span></p><p><span
  m="2512840">AUDIENCE:</span> <span m="2513045">x1.</span></p><p><span m="2514070">DAVID
  SONTAG:</span> <span m="2514235">x1.</span> <span m="2515090">So</span> <span m="2515870">y1</span>
  <span m="2517700">in</span> <span m="2517940">this</span> <span m="2518390">factorization</span>
  <span m="2519050">is</span> <span m="2519140">only</span> <span m="2519380">going</span>
  <span m="2519500">to</span> <span m="2519590">depend</span> <span m="2519890">on</span>
  <span m="2520220">x1.</span> <span m="2521450">Next</span> <span m="2521750">we</span>
  <span m="2521870">have</span> <span m="2522050">x2.</span> <span m="2522740">What</span>
  <span m="2522890">are</span> <span m="2522950">the</span> <span m="2523040">parents</span>
  <span m="2523430">of</span> <span m="2523550">x2?</span> <span m="2523940">Everyone</span>
  <span m="2524210">say</span> <span m="2524330">out</span> <span m="2524450">loud?</span></p><p><span
  m="2525390">AUDIENCE:</span> <span m="2525635">x1.</span></p><p><span m="2526370">DAVID
  SONTAG:</span> <span m="2526512">x1.</span> <span m="2527840">Then</span> <span
  m="2528050">we</span> <span m="2528200">have</span> <span m="2529070">y2.</span>
  <span m="2529790">What</span> <span m="2529940">are</span> <span m="2529970">the</span>
  <span m="2530060">parents</span> <span m="2530630">of</span> <span m="2531140">y2.</span>
  <span m="2531710">Everyone</span> <span m="2531950">say</span> <span m="2532070">out</span>
  <span m="2532190">loud.</span></p><p><span m="2532550">AUDIENCE:</span> <span m="2532741">x2.</span></p><p><span
  m="2534080">DAVID SONTAG:</span> <span m="2534257">x2</span> <span m="2535400">and</span>
  <span m="2535640">so</span> <span m="2535940">on.</span> <span m="2536960">So</span>
  <span m="2537620">this</span> <span m="2537950">joint</span> <span m="2538280">distribution</span>
  <span m="2539780">is</span> <span m="2540680">going</span> <span m="2540920">to</span>
  <span m="2541010">have</span> <span m="2541430">a</span> <span m="2541490">particularly</span>
  <span m="2542210">simple</span> <span m="2542630">form,</span> <span m="2543410">which</span>
  <span m="2543560">is</span> <span m="2543680">given</span> <span m="2543920">to</span>
  <span m="2544100">by</span> <span m="2544220">this</span> <span m="2544400">factorization</span>
  <span m="2545030">shown</span> <span m="2545330">here.</span> <span m="2546280">And</span>
  <span m="2546380">this</span> <span m="2546530">factorization</span> <span m="2547160">corresponds</span>
  <span m="2547670">one</span> <span m="2547910">to</span> <span m="2548030">one</span>
  <span m="2548420">with</span> <span m="2548720">the</span> <span m="2548840">particular</span>
  <span m="2549350">graph</span> <span m="2550100">in</span> <span m="2550190">the</span>
  <span m="2550250">way</span> <span m="2550400">that</span> <span m="2550520">I</span>
  <span m="2550580">just</span> <span m="2550760">told</span> <span m="2550970">you.</span></p><p><span
  m="2552400">And</span> <span m="2552580">in</span> <span m="2552670">this</span>
  <span m="2552880">way,</span> <span m="2553300">we</span> <span m="2553450">can</span>
  <span m="2553570">define</span> <span m="2554350">a</span> <span m="2554470">very</span>
  <span m="2554830">complex</span> <span m="2555460">probability</span> <span m="2555760">distribution</span>
  <span m="2557020">by</span> <span m="2557350">a</span> <span m="2557410">number</span>
  <span m="2557830">of</span> <span m="2557920">much</span> <span m="2558220">simpler</span>
  <span m="2559000">conditional</span> <span m="2559600">probability</span> <span
  m="2559900">distributions.</span> <span m="2561220">For</span> <span m="2561370">example,</span>
  <span m="2562040">if</span> <span m="2562240">each</span> <span m="2562480">of</span>
  <span m="2562540">the</span> <span m="2562600">random</span> <span m="2562810">variables</span>
  <span m="2563230">were</span> <span m="2563500">binary,</span> <span m="2564740">then</span>
  <span m="2565240">to</span> <span m="2565390">describe</span> <span m="2566080">probability</span>
  <span m="2566560">of</span> <span m="2566650">y1</span> <span m="2567430">given</span>
  <span m="2567820">x1,</span> <span m="2568840">we</span> <span m="2568990">only</span>
  <span m="2569230">need</span> <span m="2569410">two</span> <span m="2569650">numbers.</span>
  <span m="2570250">For</span> <span m="2570490">each</span> <span m="2570640">value</span>
  <span m="2571030">of</span> <span m="2571120">x1,</span> <span m="2571720">either</span>
  <span m="2571990">0</span> <span m="2572270">or</span> <span m="2572320">1,</span>
  <span m="2572840">we</span> <span m="2572920">give</span> <span m="2573040">the</span>
  <span m="2573130">probability</span> <span m="2573520">of</span> <span m="2573580">y1</span>
  <span m="2573970">equals</span> <span m="2574300">1.</span> <span m="2575290">And</span>
  <span m="2575380">then,</span> <span m="2575470">of</span> <span m="2575560">course,</span>
  <span m="2575770">probably</span> <span m="2576070">y1</span> <span m="2576460">equals</span>
  <span m="2576700">0</span> <span m="2576955">is</span> <span m="2577210">just</span>
  <span m="2577360">1</span> <span m="2577540">minus</span> <span m="2577870">that.</span>
  <span m="2579530">So</span> <span m="2579650">we</span> <span m="2579740">can</span>
  <span m="2579890">describe</span> <span m="2580490">that</span> <span m="2580700">very</span>
  <span m="2580940">complicated</span> <span m="2581540">joint</span> <span m="2581750">distribution</span>
  <span m="2582290">by</span> <span m="2582890">a</span> <span m="2582950">number</span>
  <span m="2583250">of</span> <span m="2583340">much</span> <span m="2583580">smaller</span>
  <span m="2584330">distributions.</span></p><p><span m="2587200">Now,</span> <span
  m="2587280">the</span> <span m="2587370">reason</span> <span m="2587670">why</span>
  <span m="2587880">I'm</span> <span m="2588000">drawing</span> <span m="2588330">it</span>
  <span m="2588440">in</span> <span m="2588510">this</span> <span m="2588720">way</span>
  <span m="2590700">is</span> <span m="2591180">because</span> <span m="2591750">we're</span>
  <span m="2591960">making</span> <span m="2592290">some</span> <span m="2592470">really</span>
  <span m="2592860">strong</span> <span m="2593250">assumptions</span> <span m="2593940">about</span>
  <span m="2594270">the</span> <span m="2594390">temporal</span> <span m="2594990">dynamics</span>
  <span m="2596010">in</span> <span m="2596220">this</span> <span m="2596490">problem.</span>
  <span m="2598020">In</span> <span m="2598080">particular,</span> <span m="2599770">the</span>
  <span m="2599790">fact</span> <span m="2600300">that</span> <span m="2601350">x3</span>
  <span m="2602700">only</span> <span m="2603360">has</span> <span m="2603630">an</span>
  <span m="2603720">arrow</span> <span m="2604200">from</span> <span m="2604530">x2</span>
  <span m="2605250">and</span> <span m="2605340">not</span> <span m="2605640">from</span>
  <span m="2605880">x1</span> <span m="2607720">implies</span> <span m="2608610">that</span>
  <span m="2609360">x3</span> <span m="2610170">is</span> <span m="2610380">conditionally</span>
  <span m="2611010">independent</span> <span m="2611880">of</span> <span m="2612030">x1.</span>
  <span m="2612540">If</span> <span m="2612720">you</span> <span m="2612870">knew</span>
  <span m="2613170">x2's</span> <span m="2613740">value.</span> <span m="2614400">So
  in</span> <span m="2614610">some sense,</span> <span m="2615060">think</span> <span
  m="2615300">about</span> <span m="2615510">this</span> <span m="2615710">as</span>
  <span m="2617340">cutting.</span> <span m="2617970">If</span> <span m="2618030">you're</span>
  <span m="2618120">to</span> <span m="2618240">take</span> <span m="2618870">x2</span>
  <span m="2619440">out</span> <span m="2619680">of</span> <span m="2619770">the</span>
  <span m="2619860">model</span> <span m="2620700">and</span> <span m="2620790">remove</span>
  <span m="2621540">all</span> <span m="2621780">edges</span> <span m="2622350">incident</span>
  <span m="2622770">on</span> <span m="2622890">it,</span> <span m="2623040">then</span>
  <span m="2623220">x1</span> <span m="2623610">and</span> <span m="2623790">x3</span>
  <span m="2624030">are</span> <span m="2624120">now</span> <span m="2624570">separated</span>
  <span m="2625080">from</span> <span m="2625240">one</span> <span m="2625310">another.</span>
  <span m="2626490">They're</span> <span m="2626910">independent.</span> <span m="2628110">Now,</span>
  <span m="2628200">for</span> <span m="2628320">those</span> <span m="2628500">of</span>
  <span m="2628560">you</span> <span m="2628740">who</span> <span m="2629430">do</span>
  <span m="2629670">know</span> <span m="2630060">graphical</span> <span m="2630510">models,</span>
  <span m="2631740">you'll</span> <span m="2632160">recognize</span> <span m="2632760">that</span>
  <span m="2633240">that</span> <span m="2633480">type</span> <span m="2633810">of</span>
  <span m="2633900">independent</span> <span m="2634290">statement</span> <span m="2634590">that</span>
  <span m="2634710">I</span> <span m="2634770">made</span> <span m="2635010">is</span>
  <span m="2635100">only</span> <span m="2635280">true</span> <span m="2635520">for</span>
  <span m="2635650">Markov</span> <span m="2636060">models,</span> <span m="2636480">and</span>
  <span m="2636600">the</span> <span m="2636690">semantics</span> <span m="2637230">for</span>
  <span m="2637950">Bayesian</span> <span m="2638370">networks</span> <span m="2638730">are</span>
  <span m="2638820">a</span> <span m="2638850">little</span> <span m="2639000">bit</span>
  <span m="2639090">different.</span> <span m="2639730">But</span> <span m="2639810">actually</span>
  <span m="2640110">for</span> <span m="2640290">this</span> <span m="2640800">model,</span>
  <span m="2641370">it's--</span> <span m="2641730">they're</span> <span m="2641970">one</span>
  <span m="2642180">and</span> <span m="2642240">the</span> <span m="2642330">same.</span></p><p><span
  m="2645910">So</span> <span m="2646800">we're</span> <span m="2646920">going</span>
  <span m="2647100">to</span> <span m="2647160">make</span> <span m="2647310">the</span>
  <span m="2647400">following</span> <span m="2648060">assumptions</span> <span m="2648990">for</span>
  <span m="2649590">the</span> <span m="2649890">conditional</span> <span m="2650760">distributions</span>
  <span m="2651450">shown</span> <span m="2651750">here.</span> <span m="2652890">First,</span>
  <span m="2653190">we're</span> <span m="2653310">going</span> <span m="2653490">to</span>
  <span m="2653580">suppose</span> <span m="2654210">that</span> <span m="2654600">xt</span>
  <span m="2656160">is</span> <span m="2656310">given</span> <span m="2656640">to
  you</span> <span m="2656850">by</span> <span m="2657180">a</span> <span m="2657330">Gaussian</span>
  <span m="2657990">distribution.</span> <span m="2659490">Remember</span> <span m="2659790">xt--</span>
  <span m="2662760">t</span> <span m="2663090">is</span> <span m="2663150">denoting
  a time</span> <span m="2663360">step.</span> <span m="2663570">Let's</span> <span
  m="2663690">say</span> <span m="2663900">3--</span> <span m="2664840">it</span>
  <span m="2665240">only</span> <span m="2665580">depends</span> <span m="2666420">in</span>
  <span m="2666540">this</span> <span m="2666660">picture--</span> <span m="2667260">the</span>
  <span m="2667380">conditional</span> <span m="2667660">distribution</span> <span
  m="2667950">only</span> <span m="2668190">depends</span> <span m="2668520">on</span>
  <span m="2668610">the</span> <span m="2668670">previous</span> <span m="2669090">time</span>
  <span m="2669220">step's</span> <span m="2669510">value,</span> <span m="2669840">x2,</span>
  <span m="2670650">or</span> <span m="2670770">xt</span> <span m="2671070">minus</span>
  <span m="2671340">1.</span></p><p><span m="2672310">So</span> <span m="2672570">you'll</span>
  <span m="2672720">notice</span> <span m="2673140">how</span> <span m="2673800">I'm</span>
  <span m="2674040">going</span> <span m="2674150">to</span> <span m="2674250">say</span>
  <span m="2674490">here</span> <span m="2674850">xt</span> <span m="2675360">is</span>
  <span m="2675420">going</span> <span m="2675500">to</span> <span m="2675600">distribute</span>
  <span m="2675970">as</span> <span m="2676080">something,</span> <span m="2676620">but</span>
  <span m="2676740">the</span> <span m="2676860">only</span> <span m="2677190">random</span>
  <span m="2677400">variables</span> <span m="2677760">in</span> <span m="2677910">this</span>
  <span m="2678010">something</span> <span m="2678690">can</span> <span m="2678900">be</span>
  <span m="2679020">xt</span> <span m="2679380">minus 1,</span> <span m="2679680">according</span>
  <span m="2680580">to</span> <span m="2681270">these</span> <span m="2681450">assumptions.</span>
  <span m="2683160">In</span> <span m="2683250">particular,</span> <span m="2683680">we're</span>
  <span m="2683780">going</span> <span m="2683880">to</span> <span m="2683980">assume</span>
  <span m="2684180">that</span> <span m="2684360">it's</span> <span m="2684840">some</span>
  <span m="2685260">Gaussian</span> <span m="2686010">distribution,</span> <span m="2686790">whose</span>
  <span m="2687000">mean</span> <span m="2687600">is</span> <span m="2687930">some</span>
  <span m="2688230">linear</span> <span m="2688590">transformation</span> <span m="2689130">of</span>
  <span m="2689220">xt</span> <span m="2689490">minus</span> <span m="2689760">1,</span>
  <span m="2691020">and</span> <span m="2691230">which</span> <span m="2691440">has</span>
  <span m="2691590">a</span> <span m="2691650">fixed</span> <span m="2692160">covariance</span>
  <span m="2692760">matrix</span> <span m="2693580">q.</span> <span m="2695240">So</span>
  <span m="2696560">at</span> <span m="2696740">each</span> <span m="2697010">step</span>
  <span m="2697400">of</span> <span m="2697490">this</span> <span m="2697640">process,</span>
  <span m="2698690">the</span> <span m="2698810">next</span> <span m="2699380">random</span>
  <span m="2699740">variable</span> <span m="2700310">is</span> <span m="2700490">some</span>
  <span m="2700910">random</span> <span m="2701540">walk</span> <span m="2701930">from</span>
  <span m="2702140">the</span> <span m="2702230">previous</span> <span m="2702500">random</span>
  <span m="2702710">variable</span> <span m="2703700">where</span> <span m="2704030">you're</span>
  <span m="2704210">moving</span> <span m="2704840">according</span> <span m="2705170">to</span>
  <span m="2705320">some</span> <span m="2705620">Gaussian</span> <span m="2706010">distribution.</span></p><p><span
  m="2708150">In</span> <span m="2708260">a</span> <span m="2708320">very</span> <span
  m="2708470">similar</span> <span m="2708830">way,</span> <span m="2709080">we're</span>
  <span m="2709190">going</span> <span m="2709250">to</span> <span m="2709310">assume</span>
  <span m="2709700">that</span> <span m="2710090">yt</span> <span m="2711620">is</span>
  <span m="2713270">drawn</span> <span m="2715640">also</span> <span m="2716210">as</span>
  <span m="2716390">a</span> <span m="2716450">Gaussian</span> <span m="2716870">distribution,</span>
  <span m="2717410">but</span> <span m="2717530">now</span> <span m="2717710">depending</span>
  <span m="2718070">on</span> <span m="2718630">xt.</span> <span m="2720550">So</span>
  <span m="2720790">I</span> <span m="2720880">want</span> <span m="2721000">you</span>
  <span m="2721060">to</span> <span m="2721150">think</span> <span m="2721270">about</span>
  <span m="2721480">xt</span> <span m="2722320">as</span> <span m="2723250">the</span>
  <span m="2723370">true</span> <span m="2723730">state</span> <span m="2724120">of</span>
  <span m="2724180">the</span> <span m="2724270">patient.</span> <span m="2725410">It's</span>
  <span m="2726370">a</span> <span m="2726430">vector</span> <span m="2726970">that's</span>
  <span m="2727120">summarizing</span> <span m="2727900">their</span> <span m="2728260">blood</span>
  <span m="2728590">pressure,</span> <span m="2729800">their</span> <span m="2730180">oxygen</span>
  <span m="2730570">saturation,</span> <span m="2731200">a</span> <span m="2731260">whole</span>
  <span m="2731380">bunch</span> <span m="2731590">of</span> <span m="2731650">other</span>
  <span m="2731860">parameters,</span> <span m="2733150">or</span> <span m="2733240">maybe</span>
  <span m="2733510">even</span> <span m="2733690">just</span> <span m="2733840">one</span>
  <span m="2734020">of</span> <span m="2734140">those.</span> <span m="2735460">And</span>
  <span m="2735760">y1</span> <span m="2736720">are</span> <span m="2736870">the</span>
  <span m="2736990">observations</span> <span m="2737710">that</span> <span m="2737860">you</span>
  <span m="2737980">do</span> <span m="2738220">observe.</span> <span m="2739300">So</span>
  <span m="2739480">let's</span> <span m="2739630">say</span> <span m="2739780">x1</span>
  <span m="2740170">is</span> <span m="2740260">the</span> <span m="2740320">patient's</span>
  <span m="2740650">true</span> <span m="2740920">blood</span> <span m="2741160">pressure.</span>
  <span m="2741890">y1</span> <span m="2742420">is</span> <span m="2742540">the</span>
  <span m="2742720">observed</span> <span m="2743500">blood</span> <span m="2743680">pressure,</span>
  <span m="2743980">what</span> <span m="2744100">comes</span> <span m="2744400">from</span>
  <span m="2744580">your</span> <span m="2744670">monitor.</span></p><p><span m="2747010">So</span>
  <span m="2747160">then</span> <span m="2747730">a</span> <span m="2747820">reasonable</span>
  <span m="2748180">assumption</span> <span m="2748570">would</span> <span m="2748660">be</span>
  <span m="2748720">that,</span> <span m="2749410">well,</span> <span m="2750040">if</span>
  <span m="2750220">all</span> <span m="2750460">this</span> <span m="2750670">were</span>
  <span m="2750850">equal,</span> <span m="2752350">if</span> <span m="2752590">it</span>
  <span m="2752680">was</span> <span m="2752890">a</span> <span m="2752950">true</span>
  <span m="2753250">observation,</span> <span m="2753790">then</span> <span m="2753910">y1</span>
  <span m="2754240">should</span> <span m="2754330">be</span> <span m="2754420">very</span>
  <span m="2754600">close</span> <span m="2754870">to</span> <span m="2754960">x1.</span>
  <span m="2755750">So</span> <span m="2755770">you</span> <span m="2755830">might</span>
  <span m="2755980">assume</span> <span m="2756340">that</span> <span m="2756490">this</span>
  <span m="2757120">covariance</span> <span m="2757630">matrix</span> <span m="2758110">is--</span>
  <span m="2758680">the</span> <span m="2758800">covariance</span> <span m="2759410">is--</span>
  <span m="2759550">the</span> <span m="2759670">variance</span> <span m="2760030">is</span>
  <span m="2760120">very,</span> <span m="2760430">very</span> <span m="2760510">small.</span>
  <span m="2761460">y1</span> <span m="2761980">should</span> <span m="2762100">be</span>
  <span m="2762190">very</span> <span m="2762460">close</span> <span m="2762760">to</span>
  <span m="2762850">x1</span> <span m="2763510">if</span> <span m="2763930">it's</span>
  <span m="2764110">a</span> <span m="2764320">good</span> <span m="2764650">observation.</span>
  <span m="2767280">And of</span> <span m="2767400">course,</span> <span m="2768150">if</span>
  <span m="2768420">it's</span> <span m="2768660">a</span> <span m="2768750">noisy</span>
  <span m="2769320">observation--</span> <span m="2770100">like,</span> <span m="2770250">for</span>
  <span m="2770310">example,</span> <span m="2771130">if</span> <span m="2771930">the</span>
  <span m="2772380">probe</span> <span m="2772920">was</span> <span m="2773160">disconnected</span>
  <span m="2774180">from</span> <span m="2774480">the</span> <span m="2774570">baby,</span>
  <span m="2775680">then</span> <span m="2775860">y1</span> <span m="2776350">should</span>
  <span m="2776480">have</span> <span m="2776640">no</span> <span m="2776940">relationship</span>
  <span m="2777890">to</span> <span m="2778100">x1.</span> <span m="2779790">And</span>
  <span m="2780030">that</span> <span m="2780270">dependence</span> <span m="2781260">on</span>
  <span m="2781620">the</span> <span m="2781740">actual</span> <span m="2782250">state</span>
  <span m="2782580">of</span> <span m="2782670">the</span> <span m="2782760">world</span>
  <span m="2783460">I'm</span> <span m="2783600">denoting</span> <span m="2783990">here</span>
  <span m="2784320">by</span> <span m="2784500">these</span> <span m="2785170">superscripts,</span>
  <span m="2785810">s</span> <span m="2786000">of</span> <span m="2786150">t.</span>
  <span m="2786960">I'm</span> <span m="2787080">ignoring</span> <span m="2787500">that</span>
  <span m="2787650">right</span> <span m="2787860">now,</span> <span m="2788230">and</span>
  <span m="2788330">I'll</span> <span m="2788430">bring</span> <span m="2788580">that</span>
  <span m="2788730">in</span> <span m="2788910">in the</span> <span m="2789000">next</span>
  <span m="2789240">slide.</span></p><p><span m="2791910">Similarly,</span> <span
  m="2793410">the</span> <span m="2793500">relationship</span> <span m="2793980">between</span>
  <span m="2794370">x2</span> <span m="2795180">and</span> <span m="2795300">x1</span>
  <span m="2796230">should</span> <span m="2796440">be</span> <span m="2796560">one</span>
  <span m="2796890">which</span> <span m="2797130">captures</span> <span m="2797640">some</span>
  <span m="2797790">of</span> <span m="2797850">the</span> <span m="2797910">dynamics</span>
  <span m="2798510">that</span> <span m="2798630">I</span> <span m="2798690">showed</span>
  <span m="2799050">in</span> <span m="2799110">the</span> <span m="2799200">previous</span>
  <span m="2799620">slides,</span> <span m="2800925">where</span> <span m="2801360">I</span>
  <span m="2801670">showed</span> <span m="2801990">over</span> <span m="2802140">here</span>
  <span m="2802820">now</span> <span m="2802950">this</span> <span m="2803100">is</span>
  <span m="2803190">the</span> <span m="2803270">patient's</span> <span m="2804720">true</span>
  <span m="2805080">heart</span> <span m="2805350">rate</span> <span m="2805560">evolving</span>
  <span m="2806040">across</span> <span m="2806400">time,</span> <span m="2807000">let's</span>
  <span m="2807150">say.</span> <span m="2808080">Notice</span> <span m="2808530">how,</span>
  <span m="2810780">if</span> <span m="2810900">you</span> <span m="2810990">look</span>
  <span m="2811170">very</span> <span m="2811440">locally,</span> <span m="2811800">it</span>
  <span m="2812160">looks</span> <span m="2812400">like</span> <span m="2812550">there</span>
  <span m="2812730">are</span> <span m="2812790">some</span> <span m="2813060">very,</span>
  <span m="2814450">very</span> <span m="2814680">big</span> <span m="2814890">local</span>
  <span m="2815550">dynamics.</span> <span m="2816720">Whereas</span> <span m="2816960">if</span>
  <span m="2817050">you</span> <span m="2817110">look</span> <span m="2817320">more</span>
  <span m="2817530">globally,</span> <span m="2818790">again,</span> <span m="2819120">there's</span>
  <span m="2819240">some</span> <span m="2819480">smoothness,</span> <span m="2820260">but</span>
  <span m="2820410">there are</span> <span m="2820560">some--</span> <span m="2820980">again,</span>
  <span m="2821340">it</span> <span m="2821400">looks</span> <span m="2821580">like</span>
  <span m="2821700">some</span> <span m="2821880">random</span> <span m="2822240">changes</span>
  <span m="2822600">across</span> <span m="2822900">time.</span> <span m="2823590">And</span>
  <span m="2823710">so</span> <span m="2824520">those--</span> <span m="2827910">that</span>
  <span m="2828330">drift</span> <span m="2829350">has</span> <span m="2829650">to</span>
  <span m="2829740">somehow</span> <span m="2830070">be</span> <span m="2830190">summarized</span>
  <span m="2830910">in</span> <span m="2831030">this</span> <span m="2831240">model</span>
  <span m="2831630">by</span> <span m="2831930">that</span> <span m="2832530">A</span>
  <span m="2832770">random</span> <span m="2833040">variable.</span> <span m="2833550">And</span>
  <span m="2834270">I'll</span> <span m="2834360">get</span> <span m="2834540">into</span>
  <span m="2834720">more</span> <span m="2834840">detail</span> <span m="2835140">about</span>
  <span m="2835290">that</span> <span m="2835440">in</span> <span m="2835530">just</span>
  <span m="2835710">a</span> <span m="2835740">moment.</span></p><p><span m="2838750">So</span>
  <span m="2839580">what</span> <span m="2839760">I</span> <span m="2839820">just</span>
  <span m="2840000">showed</span> <span m="2840270">you</span> <span m="2840390">was</span>
  <span m="2840510">an</span> <span m="2840570">example</span> <span m="2840990">of</span>
  <span m="2841080">a</span> <span m="2841140">linear</span> <span m="2841530">dynamical</span>
  <span m="2842010">system,</span> <span m="2842940">but</span> <span m="2843270">it</span>
  <span m="2843360">was</span> <span m="2843660">assuming</span> <span m="2844290">that</span>
  <span m="2845160">there</span> <span m="2845310">were</span> <span m="2845430">none</span>
  <span m="2845670">of</span> <span m="2845880">these</span> <span m="2846480">events</span>
  <span m="2846870">happening,</span> <span m="2847170">none</span> <span m="2847290">of</span>
  <span m="2847350">these</span> <span m="2847500">artifacts</span> <span m="2847950">happening.</span>
  <span m="2850190">The</span> <span m="2850340">actual</span> <span m="2850730">model</span>
  <span m="2850940">that</span> <span m="2851030">we</span> <span m="2851150">were</span>
  <span m="2851300">going</span> <span m="2851540">to</span> <span m="2851630">want</span>
  <span m="2851810">to</span> <span m="2851900">be</span> <span m="2851990">able</span>
  <span m="2852110">to</span> <span m="2852200">use</span> <span m="2852650">then</span>
  <span m="2852920">is</span> <span m="2853040">going</span> <span m="2853220">to</span>
  <span m="2853310">also</span> <span m="2853610">incorporate</span> <span m="2854030">the</span>
  <span m="2854120">fact</span> <span m="2854330">that</span> <span m="2854420">there</span>
  <span m="2854510">might</span> <span m="2854650">be</span> <span m="2854750">artifacts.</span>
  <span m="2855320">And</span> <span m="2855440">to</span> <span m="2855530">model</span>
  <span m="2855830">that,</span> <span m="2856010">we</span> <span m="2856100">need
  to</span> <span m="2856220">introduce</span> <span m="2856640">additional</span>
  <span m="2857060">random</span> <span m="2857300">variables</span> <span m="2857780">corresponding</span>
  <span m="2858230">to</span> <span m="2858350">whether</span> <span m="2858590">those</span>
  <span m="2858770">artifacts</span> <span m="2859250">occurred</span> <span m="2859520">or</span>
  <span m="2859580">not.</span> <span m="2860250">And</span> <span m="2860560">so</span>
  <span m="2860660">that's</span> <span m="2860780">now</span> <span m="2860960">this</span>
  <span m="2861170">model.</span></p><p><span m="2862290">So</span> <span m="2862370">I'm</span>
  <span m="2862430">going</span> <span m="2862520">to</span> <span m="2862610">let</span>
  <span m="2862760">these</span> <span m="2863090">S's--</span> <span m="2865370">these</span>
  <span m="2865830">are</span> <span m="2866100">other</span> <span m="2866460">random</span>
  <span m="2866760">variables,</span> <span m="2867850">which</span> <span m="2867930">are</span>
  <span m="2867990">denoting</span> <span m="2868700">artifactual</span> <span m="2869490">events.</span>
  <span m="2871310">They</span> <span m="2871550">are</span> <span m="2871670">also</span>
  <span m="2872030">evolving</span> <span m="2872380">with</span> <span m="2872510">time.</span>
  <span m="2872970">For</span> <span m="2872990">example,</span> <span m="2873630">if</span>
  <span m="2873730">there's</span> <span m="2873800">artifactual</span> <span m="2874050">factual</span>
  <span m="2874520">event</span> <span m="2875420">at</span> <span m="2875660">three</span>
  <span m="2875960">seconds,</span> <span m="2876410">maybe</span> <span m="2876620">there's</span>
  <span m="2876770">also</span> <span m="2877130">an</span> <span m="2877220">artifactual</span>
  <span m="2877730">event at</span> <span m="2878020">four</span> <span m="2878270">seconds.</span>
  <span m="2878720">And we</span> <span m="2878860">like</span> <span m="2878990">to</span>
  <span m="2879110">model</span> <span m="2879380">the</span> <span m="2879440">relationship</span>
  <span m="2879830">between</span> <span m="2880160">those.</span> <span m="2880400">That's</span>
  <span m="2880550">why</span> <span m="2880640">you</span> <span m="2880730">have</span>
  <span m="2880850">these</span> <span m="2881060">arrows.</span></p><p><span m="2882600">And</span>
  <span m="2882720">then</span> <span m="2884820">the</span> <span m="2884970">way</span>
  <span m="2885210">that</span> <span m="2885390">we</span> <span m="2886170">interpret</span>
  <span m="2887070">the</span> <span m="2887250">observations</span> <span m="2888180">that</span>
  <span m="2888300">we</span> <span m="2888450">do</span> <span m="2888690">get</span>
  <span m="2889470">depends</span> <span m="2890220">on</span> <span m="2890490">both</span>
  <span m="2891450">the</span> <span m="2891570">true</span> <span m="2892020">value</span>
  <span m="2892620">of</span> <span m="2892740">what's</span> <span m="2892890">going</span>
  <span m="2893040">on</span> <span m="2893100">with</span> <span m="2893190">the</span>
  <span m="2893250">patient</span> <span m="2894340">and</span> <span m="2894780">whether</span>
  <span m="2895110">there</span> <span m="2895230">was</span> <span m="2895350">an</span>
  <span m="2895440">artifactual</span> <span m="2895980">event</span> <span m="2896310">or</span>
  <span m="2896400">not.</span> <span m="2897810">And</span> <span m="2897910">you'll</span>
  <span m="2897990">notice</span> <span m="2898380">that</span> <span m="2898500">there's</span>
  <span m="2898710">also</span> <span m="2899070">an</span> <span m="2899160">edge</span>
  <span m="2899460">going</span> <span m="2899730">from</span> <span m="2899850">the</span>
  <span m="2899910">artifactual</span> <span m="2900360">events</span> <span m="2900780">to</span>
  <span m="2900960">the</span> <span m="2901080">true</span> <span m="2901350">values</span>
  <span m="2902220">to</span> <span m="2902340">note</span> <span m="2902610">the</span>
  <span m="2902730">fact</span> <span m="2903270">that</span> <span m="2904830">those</span>
  <span m="2906450">interventions</span> <span m="2907260">might</span> <span m="2907440">actually</span>
  <span m="2907680">be</span> <span m="2907800">affecting</span> <span m="2908580">the</span>
  <span m="2908670">patient.</span> <span m="2909030">For</span> <span m="2909150">example,</span>
  <span m="2909670">if</span> <span m="2909690">you</span> <span m="2909810">give</span>
  <span m="2910050">them</span> <span m="2910200">a</span> <span m="2910260">medication</span>
  <span m="2911040">to</span> <span m="2911160">change</span> <span m="2911610">their</span>
  <span m="2911820">blood</span> <span m="2912060">pressure,</span> <span m="2912540">then</span>
  <span m="2913950">that</span> <span m="2915840">procedure</span> <span m="2916800">is</span>
  <span m="2916950">going</span> <span m="2917100">to</span> <span m="2917190">affect</span>
  <span m="2917880">the</span> <span m="2918000">next</span> <span m="2918390">time</span>
  <span m="2918690">step's</span> <span m="2918980">value</span> <span m="2919440">of</span>
  <span m="2919560">the</span> <span m="2919620">patient's</span> <span m="2919980">blood</span>
  <span m="2920130">pressure.</span></p><p><span m="2924360">So</span> <span m="2924620">when</span>
  <span m="2924800">one</span> <span m="2924920">wants</span> <span m="2925130">to</span>
  <span m="2925220">learn</span> <span m="2925580">this</span> <span m="2925820">model,</span>
  <span m="2928040">you</span> <span m="2928160">have</span> <span m="2928250">to</span>
  <span m="2928340">ask</span> <span m="2928550">yourself,</span> <span m="2928970">what</span>
  <span m="2929120">types</span> <span m="2929390">of</span> <span m="2929480">data</span>
  <span m="2929750">do</span> <span m="2929840">you</span> <span m="2929900">have</span>
  <span m="2930140">available?</span> <span m="2934370">Unfortunately,</span> <span
  m="2935630">it's</span> <span m="2936170">very</span> <span m="2936620">hard</span>
  <span m="2937250">to</span> <span m="2937430">get</span> <span m="2937670">data</span>
  <span m="2938390">on</span> <span m="2938870">both</span> <span m="2939230">the</span>
  <span m="2939350">ground</span> <span m="2939680">truth,</span> <span m="2940340">what's</span>
  <span m="2940520">going</span> <span m="2940700">on</span> <span m="2940820">with</span>
  <span m="2940940">the</span> <span m="2941000">patient,</span> <span m="2942210">and</span>
  <span m="2942980">whether</span> <span m="2943280">these</span> <span m="2943520">artifacts</span>
  <span m="2944180">truly</span> <span m="2944510">occurred</span> <span m="2944810">or</span>
  <span m="2944870">not.</span> <span m="2946530">Instead,</span> <span m="2946890">what</span>
  <span m="2947010">we</span> <span m="2947130">actually</span> <span m="2947520">have</span>
  <span m="2947910">are</span> <span m="2948000">just</span> <span m="2948240">these</span>
  <span m="2948390">observations.</span> <span m="2949530">We</span> <span m="2949650">get</span>
  <span m="2949770">these</span> <span m="2949950">very</span> <span m="2950160">noisy</span>
  <span m="2950520">blood</span> <span m="2950730">pressure</span> <span m="2951030">draws</span>
  <span m="2951330">across</span> <span m="2951630">time.</span></p><p><span m="2953450">So</span>
  <span m="2953470">what</span> <span m="2953590">this</span> <span m="2953770">paper</span>
  <span m="2954070">does</span> <span m="2954280">is</span> <span m="2954370">it</span>
  <span m="2954430">uses</span> <span m="2955090">a</span> <span m="2955540">maximum</span>
  <span m="2956050">likelihood</span> <span m="2956500">estimation</span> <span m="2957040">approach,</span>
  <span m="2958230">where it</span> <span m="2958360">recognizes</span> <span m="2958930">that</span>
  <span m="2959020">we're</span> <span m="2959200">going</span> <span m="2959440">to</span>
  <span m="2959530">be</span> <span m="2959620">learning</span> <span m="2959920">from</span>
  <span m="2960070">missing</span> <span m="2960550">data.</span> <span m="2960880">We're</span>
  <span m="2960970">going</span> <span m="2961090">to</span> <span m="2961180">explicitly</span>
  <span m="2961840">think</span> <span m="2962170">of</span> <span m="2962260">these</span>
  <span m="2962500">x's</span> <span m="2963070">and</span> <span m="2963350">the</span>
  <span m="2963450">s's</span> <span m="2963940">as</span> <span m="2964180">latent</span>
  <span m="2964720">variables.</span> <span m="2965875">And</span> <span m="2966370">we're</span>
  <span m="2966460">going</span> <span m="2966640">to</span> <span m="2966760">maximize</span>
  <span m="2967330">the</span> <span m="2967450">likelihood</span> <span m="2967990">of</span>
  <span m="2968080">the</span> <span m="2968170">whole</span> <span m="2968350">entire</span>
  <span m="2968660">model,</span> <span m="2969460">marginalizing</span> <span m="2970360">over</span>
  <span m="2970830">x</span> <span m="2971090">and</span> <span m="2971330">s.</span>
  <span m="2971820">So</span> <span m="2971920">just</span> <span m="2972130">maximizing</span>
  <span m="2972670">the</span> <span m="2972730">marginal</span> <span m="2973180">likelihood</span>
  <span m="2973690">over</span> <span m="2973960">the</span> <span m="2974080">y's.</span></p><p><span
  m="2977650">Now,</span> <span m="2977790">for</span> <span m="2977910">those</span>
  <span m="2978120">of</span> <span m="2978210">you</span> <span m="2978390">who have</span>
  <span m="2978690">studied</span> <span m="2979050">unsupervised</span> <span m="2979470">learning</span>
  <span m="2979740">before,</span> <span m="2980220">you</span> <span m="2980340">might</span>
  <span m="2980490">recognize</span> <span m="2981330">that</span> <span m="2981690">as</span>
  <span m="2982110">a</span> <span m="2982170">very</span> <span m="2982680">hard</span>
  <span m="2983340">learning</span> <span m="2983640">problem.</span> <span m="2984070">In</span>
  <span m="2984170">fact,</span> <span m="2984460">it's--</span> <span m="2984660">that</span>
  <span m="2984870">likelihood</span> <span m="2985740">is</span> <span m="2986190">non-convex.</span>
  <span m="2987780">And</span> <span m="2988980">one</span> <span m="2989190">could</span>
  <span m="2989310">imagine</span> <span m="2989730">all</span> <span m="2989880">sorts</span>
  <span m="2990120">of</span> <span m="2990240">a</span> <span m="2990630">heuristics</span>
  <span m="2990960">for</span> <span m="2991110">learning,</span> <span m="2991990">such</span>
  <span m="2992220">as</span> <span m="2992400">gradient</span> <span m="2992760">descent,</span>
  <span m="2993390">or,</span> <span m="2993750">as</span> <span m="2993900">this</span>
  <span m="2994050">paper</span> <span m="2994290">uses,</span> <span m="2995460">expectation</span>
  <span m="2996030">maximization,</span> <span m="2997260">and</span> <span m="2997650">because</span>
  <span m="2998010">of</span> <span m="2998070">that</span> <span m="2998220">non-convexity,</span>
  <span m="2999180">each</span> <span m="2999420">of</span> <span m="2999510">these</span>
  <span m="2999750">algorithms</span> <span m="3000320">typically</span> <span m="3000750">will</span>
  <span m="3000820">only</span> <span m="3001100">reach</span> <span m="3001430">a</span>
  <span m="3001610">local</span> <span m="3002060">maxima</span> <span m="3002530">of</span>
  <span m="3002600">the</span> <span m="3002690">likelihood.</span></p><p><span m="3004040">So</span>
  <span m="3004190">this</span> <span m="3004340">paper</span> <span m="3004580">uses</span>
  <span m="3005030">EM,</span> <span m="3006410">which</span> <span m="3006980">intuitively</span>
  <span m="3007940">iterates</span> <span m="3008420">between</span> <span m="3010190">inferring</span>
  <span m="3011270">those</span> <span m="3011600">missing</span> <span m="3011930">variables--</span>
  <span m="3012560">so</span> <span m="3012770">imputing</span> <span m="3013610">the</span>
  <span m="3013880">x's</span> <span m="3014420">and</span> <span m="3014510">the</span>
  <span m="3014610">s's</span> <span m="3015170">given</span> <span m="3015950">the</span>
  <span m="3016100">current</span> <span m="3016610">model,</span> <span m="3017210">and</span>
  <span m="3017360">doing</span> <span m="3017630">posterior</span> <span m="3018440">inference</span>
  <span m="3019130">to</span> <span m="3019280">infer</span> <span m="3019640">the</span>
  <span m="3019760">missing</span> <span m="3020300">variables</span> <span m="3020780">given</span>
  <span m="3021050">the</span> <span m="3021230">observed</span> <span m="3021650">variables,</span>
  <span m="3022430">using</span> <span m="3022760">the</span> <span m="3022850">current</span>
  <span m="3023270">model.</span> <span m="3024140">And</span> <span m="3024290">then,</span>
  <span m="3024890">once</span> <span m="3025130">you've</span> <span m="3025250">imputed</span>
  <span m="3025700">those</span> <span m="3025910">variables,</span> <span m="3027020">attempting</span>
  <span m="3027530">to</span> <span m="3027770">refit</span> <span m="3028340">the</span>
  <span m="3028460">model.</span> <span m="3028910">So</span> <span m="3029120">that's</span>
  <span m="3029330">called</span> <span m="3029520">the</span> <span m="3029600">m-step</span>
  <span m="3030020">for</span> <span m="3030140">maximization,</span> <span m="3030920">which</span>
  <span m="3031070">updates</span> <span m="3031400">the</span> <span m="3031490">model</span>
  <span m="3031730">and</span> <span m="3031820">just</span> <span m="3031970">iterates</span>
  <span m="3032300">between</span> <span m="3032570">those</span> <span m="3032720">two</span>
  <span m="3032900">things.</span> <span m="3033290">That's</span> <span m="3033500">one</span>
  <span m="3033770">learning</span> <span m="3034070">algorithm</span> <span m="3036440">which</span>
  <span m="3036590">is</span> <span m="3036680">guaranteed</span> <span m="3037130">to</span>
  <span m="3037250">reach</span> <span m="3037580">a</span> <span m="3038150">local</span>
  <span m="3038630">maxima</span> <span m="3039060">of</span> <span m="3039170">the</span>
  <span m="3039260">likelihood</span> <span m="3039650">under</span> <span m="3039830">some</span>
  <span m="3040760">regularity</span> <span m="3041210">assumptions.</span></p><p><span
  m="3042830">And</span> <span m="3042930">so</span> <span m="3043030">this</span>
  <span m="3043040">paper</span> <span m="3043310">uses</span> <span m="3043730">that</span>
  <span m="3043970">algorithm,</span> <span m="3044690">but</span> <span m="3044840">you</span>
  <span m="3044930">need</span> <span m="3045020">to</span> <span m="3045080">be</span>
  <span m="3045200">asking</span> <span m="3045560">yourself,</span> <span m="3046520">if</span>
  <span m="3046670">all</span> <span m="3046910">you</span> <span m="3047090">ever</span>
  <span m="3047330">observe</span> <span m="3048170">are</span> <span m="3048350">the</span>
  <span m="3048470">y's,</span> <span m="3050270">then</span> <span m="3052100">will</span>
  <span m="3052370">this</span> <span m="3052580">algorithm</span> <span m="3052970">ever</span>
  <span m="3053210">recover</span> <span m="3053660">anything</span> <span m="3054830">close</span>
  <span m="3055280">to</span> <span m="3055400">the</span> <span m="3055490">true</span>
  <span m="3055730">model?</span> <span m="3056600">For</span> <span m="3056690">example,</span>
  <span m="3057390">there</span> <span m="3057440">might</span> <span m="3057620">be</span>
  <span m="3057740">large</span> <span m="3058010">amounts</span> <span m="3058310">of</span>
  <span m="3058430">non-identifiability</span> <span m="3059630">here.</span> <span
  m="3060080">It</span> <span m="3060200">could</span> <span m="3060440">be</span>
  <span m="3060680">that</span> <span m="3063020">you</span> <span m="3063140">could</span>
  <span m="3063290">swap</span> <span m="3063920">the</span> <span m="3064040">meaning</span>
  <span m="3064490">of</span> <span m="3064610">the</span> <span m="3064700">s's,</span>
  <span m="3065450">and</span> <span m="3065810">you'd</span> <span m="3065990">get</span>
  <span m="3066770">a</span> <span m="3066860">similar</span> <span m="3067460">likelihood</span>
  <span m="3068000">on</span> <span m="3068120">the</span> <span m="3068220">y's.</span></p><p><span
  m="3070170">That's</span> <span m="3070530">where</span> <span m="3070770">bringing</span>
  <span m="3071190">in</span> <span m="3071340">domain</span> <span m="3071730">knowledge</span>
  <span m="3072090">becomes</span> <span m="3072450">critical.</span> <span m="3074010">So</span>
  <span m="3074190">this</span> <span m="3074370">is</span> <span m="3074520">going</span>
  <span m="3074700">to</span> <span m="3074790">be</span> <span m="3074850">an</span>
  <span m="3074910">example</span> <span m="3075600">where</span> <span m="3076290">we</span>
  <span m="3076440">have</span> <span m="3076740">no</span> <span m="3077190">label</span>
  <span m="3077670">data</span> <span m="3079740">or</span> <span m="3079860">very</span>
  <span m="3080250">little</span> <span m="3080550">label</span> <span m="3080850">data.</span>
  <span m="3083050">And</span> <span m="3083150">we're</span> <span m="3083240">going</span>
  <span m="3083390">to</span> <span m="3083480">do</span> <span m="3083660">unsupervised</span>
  <span m="3084440">learning</span> <span m="3084740">of</span> <span m="3084830">this</span>
  <span m="3084980">model,</span> <span m="3085310">but</span> <span m="3085460">we're</span>
  <span m="3085550">going</span> <span m="3085760">to</span> <span m="3085850">use</span>
  <span m="3086090">a</span> <span m="3086330">ton</span> <span m="3086690">of</span>
  <span m="3086840">domain</span> <span m="3087410">knowledge</span> <span m="3087890">in
  order</span> <span m="3088010">to</span> <span m="3088130">constrain</span> <span
  m="3088790">the</span> <span m="3088880">model</span> <span m="3089180">as</span>
  <span m="3089300">much</span> <span m="3089480">as</span> <span m="3089570">possible.</span></p><p><span
  m="3091050">So</span> <span m="3091130">what</span> <span m="3091360">is</span>
  <span m="3091460">that</span> <span m="3091610">domain</span> <span m="3091850">knowledge?</span>
  <span m="3093490">Well,</span> <span m="3093610">first</span> <span m="3094900">we're</span>
  <span m="3094990">going</span> <span m="3095260">to</span> <span m="3096710">use</span>
  <span m="3097100">the</span> <span m="3097250">fact</span> <span m="3097730">that</span>
  <span m="3097910">we</span> <span m="3098030">know</span> <span m="3099870">that</span>
  <span m="3101120">a</span> <span m="3101220">true</span> <span m="3102090">heart</span>
  <span m="3102450">rate</span> <span m="3104440">evolves</span> <span m="3105620">in</span>
  <span m="3106540">a</span> <span m="3106570">fashion</span> <span m="3107050">that</span>
  <span m="3107200">can</span> <span m="3107380">be</span> <span m="3107500">very</span>
  <span m="3107920">well</span> <span m="3108160">modeled</span> <span m="3108820">by</span>
  <span m="3110110">an</span> <span m="3110260">autoregressive</span> <span m="3111010">process.</span>
  <span m="3113530">So</span> <span m="3113740">the</span> <span m="3113830">autoregressive</span>
  <span m="3114430">process</span> <span m="3114820">that's</span> <span m="3114970">used</span>
  <span m="3115170">in</span> <span m="3115270">this</span> <span m="3115420">paper</span>
  <span m="3116260">is</span> <span m="3116410">used</span> <span m="3116680">to</span>
  <span m="3116800">model</span> <span m="3117100">the</span> <span m="3117220">normal</span>
  <span m="3117820">heart</span> <span m="3118030">rate</span> <span m="3118180">dynamics.</span>
  <span m="3118630">In</span> <span m="3118690">a</span> <span m="3118780">moment,</span>
  <span m="3119020">I'll</span> <span m="3119080">tell</span> <span m="3119260">you</span>
  <span m="3119380">how</span> <span m="3119470">to</span> <span m="3119560">model</span>
  <span m="3119890">the</span> <span m="3120040">abnormal</span> <span m="3120850">heart</span>
  <span m="3121060">rate</span> <span m="3121240">observations.</span></p><p><span
  m="3123370">And</span> <span m="3123760">intuitively--</span> <span m="3124330">I'll</span>
  <span m="3124450">first</span> <span m="3124780">go</span> <span m="3124870">over</span>
  <span m="3125080">the</span> <span m="3125140">intuition,</span> <span m="3125530">then</span>
  <span m="3125620">I'll</span> <span m="3125710">give</span> <span m="3125890">you</span>
  <span m="3126100">the</span> <span m="3126190">math.</span> <span m="3126850">Intuitively</span>
  <span m="3127390">what</span> <span m="3127510">it</span> <span m="3127570">does</span>
  <span m="3127780">is</span> <span m="3127870">it</span> <span m="3127960">recognizes</span>
  <span m="3128650">that</span> <span m="3128860">this</span> <span m="3129220">complicated</span>
  <span m="3129850">signal</span> <span m="3130210">can</span> <span m="3130630">be</span>
  <span m="3130780">decomposed</span> <span m="3131830">into</span> <span m="3132400">two</span>
  <span m="3132880">pieces.</span> <span m="3134060">The</span> <span m="3134160">first</span>
  <span m="3134350">piece</span> <span m="3134650">shown</span> <span m="3134950">here</span>
  <span m="3135310">is</span> <span m="3135430">called</span> <span m="3135640">a</span>
  <span m="3135700">baseline</span> <span m="3136270">signal,</span> <span m="3138020">and</span>
  <span m="3138440">that,</span> <span m="3139160">if</span> <span m="3139310">you</span>
  <span m="3139400">squint</span> <span m="3139880">your</span> <span m="3140060">eyes</span>
  <span m="3140315">and you sort</span> <span m="3140570">or</span> <span m="3140740">ignore</span>
  <span m="3141200">the</span> <span m="3141320">very</span> <span m="3141560">local</span>
  <span m="3141950">fluctuations,</span> <span m="3142700">this</span> <span m="3142910">is</span>
  <span m="3143000">what</span> <span m="3143150">you</span> <span m="3143270">get</span>
  <span m="3143450">out.</span></p><p><span m="3144860">And</span> <span m="3145010">then</span>
  <span m="3145340">you</span> <span m="3145460">can</span> <span m="3145610">look</span>
  <span m="3145760">at</span> <span m="3145850">the</span> <span m="3145940">residual</span>
  <span m="3147230">of</span> <span m="3147530">subtracting</span> <span m="3149180">this</span>
  <span m="3149600">signal,</span> <span m="3150770">subtracting</span> <span m="3151370">this</span>
  <span m="3151730">baseline</span> <span m="3152330">from</span> <span m="3152570">the</span>
  <span m="3152660">signal.</span> <span m="3153710">And</span> <span m="3153830">what</span>
  <span m="3153950">you</span> <span m="3154070">get</span> <span m="3154250">out</span>
  <span m="3154490">looks</span> <span m="3154730">like</span> <span m="3154970">this.</span>
  <span m="3156250">Notice</span> <span m="3156530">here</span> <span m="3157760">it's</span>
  <span m="3158270">around</span> <span m="3158870">0</span> <span m="3159330">mean.</span>
  <span m="3159770">So</span> <span m="3159890">it's a</span> <span m="3160010">0</span>
  <span m="3160370">mean</span> <span m="3160640">signal</span> <span m="3161090">with</span>
  <span m="3161270">some</span> <span m="3161510">random</span> <span m="3161780">fluctuations,</span>
  <span m="3162620">and</span> <span m="3162710">the</span> <span m="3162800">fluctuations</span>
  <span m="3163400">are</span> <span m="3163490">happening</span> <span m="3163910">here</span>
  <span m="3164210">at</span> <span m="3164300">a</span> <span m="3164330">much</span>
  <span m="3164630">faster</span> <span m="3165650">rate</span> <span m="3166370">than--</span>
  <span m="3167210">and</span> <span m="3167570">for</span> <span m="3167750">the</span>
  <span m="3167840">original</span> <span m="3168110">baseline.</span></p><p><span
  m="3169830">And</span> <span m="3169930">so</span> <span m="3171170">the</span>
  <span m="3171530">sum</span> <span m="3172340">of</span> <span m="3172670">bt</span>
  <span m="3173630">and</span> <span m="3174140">this</span> <span m="3174380">residual</span>
  <span m="3175610">is</span> <span m="3176330">a</span> <span m="3176390">very--</span>
  <span m="3176910">it</span> <span m="3177410">looks--</span> <span m="3178190">is</span>
  <span m="3178490">exactly</span> <span m="3178910">equal</span> <span m="3179120">to</span>
  <span m="3179210">the</span> <span m="3179300">true</span> <span m="3179480">heart</span>
  <span m="3179690">rate.</span> <span m="3180200">And</span> <span m="3180350">each</span>
  <span m="3180530">of</span> <span m="3180650">these</span> <span m="3180980">two</span>
  <span m="3181190">things</span> <span m="3181490">we</span> <span m="3181580">can</span>
  <span m="3181730">model</span> <span m="3182030">very</span> <span m="3182330">well.</span>
  <span m="3183290">This</span> <span m="3183620">we</span> <span m="3183740">can</span>
  <span m="3183860">model</span> <span m="3184220">by</span> <span m="3185120">a</span>
  <span m="3185210">random</span> <span m="3185720">walk</span> <span m="3186500">with--</span>
  <span m="3188210">which</span> <span m="3188390">goes</span> <span m="3188630">very</span>
  <span m="3188840">slowly,</span> <span m="3190370">and</span> <span m="3190580">this</span>
  <span m="3190850">we</span> <span m="3190970">can</span> <span m="3191090">model</span>
  <span m="3191420">by</span> <span m="3192240">a</span> <span m="3192560">random</span>
  <span m="3192890">walk</span> <span m="3193160">which</span> <span m="3193310">goes</span>
  <span m="3193520">very</span> <span m="3193700">quickly.</span> <span m="3195320">And</span>
  <span m="3195440">that</span> <span m="3195680">is</span> <span m="3195830">exactly</span>
  <span m="3196250">what</span> <span m="3196370">I'm</span> <span m="3196460">now</span>
  <span m="3196610">going</span> <span m="3196730">to</span> <span m="3196820">show</span>
  <span m="3197120">over</span> <span m="3197300">here</span> <span m="3197630">on</span>
  <span m="3197720">the</span> <span m="3197780">left</span> <span m="3197990">hand</span>
  <span m="3198140">side.</span></p><p><span m="3199180">bt,</span> <span m="3200900">this</span>
  <span m="3201170">baseline</span> <span m="3201770">signal,</span> <span m="3202550">we're</span>
  <span m="3202670">going</span> <span m="3202880">to</span> <span m="3202970">model</span>
  <span m="3203450">as</span> <span m="3203750">a</span> <span m="3203810">Gaussian</span>
  <span m="3204260">distribution,</span> <span m="3206300">which</span> <span m="3206540">is</span>
  <span m="3206630">parameterized</span> <span m="3207160">as</span> <span m="3207260">a</span>
  <span m="3207320">function</span> <span m="3207890">of</span> <span m="3208190">not</span>
  <span m="3208490">just</span> <span m="3208760">bt</span> <span m="3209240">minus
  1,</span> <span m="3209600">but</span> <span m="3209990">also</span> <span m="3210290">bt</span>
  <span m="3210680">minus</span> <span m="3210950">2,</span> <span m="3211220">and</span>
  <span m="3211310">bt</span> <span m="3211610">minus</span> <span m="3211970">3.</span>
  <span m="3212480">And</span> <span m="3212570">so</span> <span m="3212660">we're</span>
  <span m="3212750">going</span> <span m="3212930">to</span> <span m="3213230">be</span>
  <span m="3213350">taking</span> <span m="3213620">a</span> <span m="3213710">weighted</span>
  <span m="3214340">average</span> <span m="3214940">of</span> <span m="3215090">the</span>
  <span m="3215180">previous</span> <span m="3215570">few</span> <span m="3215750">time</span>
  <span m="3216010">steps,</span> <span m="3216890">where</span> <span m="3217520">we're</span>
  <span m="3217970">smoothing</span> <span m="3219080">out,</span> <span m="3219560">in</span>
  <span m="3219680">essence,</span> <span m="3220490">the</span> <span m="3220970">observation--</span>
  <span m="3221530">the</span> <span m="3221630">previous</span> <span m="3221990">few</span>
  <span m="3222200">observations.</span> <span m="3225220">If</span> <span m="3225270">you</span>
  <span m="3225360">were</span> <span m="3225450">to--</span> <span m="3227970">if</span>
  <span m="3228120">you're</span> <span m="3228690">being</span> <span m="3228960">a</span>
  <span m="3229020">keen</span> <span m="3229380">observer,</span> <span m="3230160">you'll</span>
  <span m="3230310">notice</span> <span m="3230850">that</span> <span m="3231570">this</span>
  <span m="3231750">is</span> <span m="3231900">no</span> <span m="3232140">longer</span>
  <span m="3232710">a</span> <span m="3232770">Markov</span> <span m="3233310">model.</span></p><p><span
  m="3244870">For</span> <span m="3244920">example,</span> <span m="3247500">if</span>
  <span m="3247650">this</span> <span m="3247860">p1</span> <span m="3248880">and</span>
  <span m="3249060">p2</span> <span m="3249870">are</span> <span m="3250080">equal</span>
  <span m="3250410">to</span> <span m="3250540">2,</span> <span m="3251460">this</span>
  <span m="3251670">then</span> <span m="3251850">corresponds</span> <span m="3252420">to</span>
  <span m="3252540">a</span> <span m="3252600">second</span> <span m="3253140">order</span>
  <span m="3253410">Markov</span> <span m="3253830">model,</span> <span m="3254790">because</span>
  <span m="3255840">each</span> <span m="3256440">random</span> <span m="3256710">variable</span>
  <span m="3257100">depends</span> <span m="3257610">on</span> <span m="3257760">the</span>
  <span m="3257850">previous</span> <span m="3258330">two</span> <span m="3258600">time</span>
  <span m="3258930">steps</span> <span m="3259560">of</span> <span m="3261700">the</span>
  <span m="3261810">Markov</span> <span m="3262110">chain.</span> <span m="3264530">And</span>
  <span m="3264650">so</span> <span m="3266360">after--</span> <span m="3266870">so</span>
  <span m="3266990">you</span> <span m="3267140">would</span> <span m="3267230">model</span>
  <span m="3267710">now</span> <span m="3268740">bt</span> <span m="3269990">by</span>
  <span m="3270620">this</span> <span m="3270980">process,</span> <span m="3271790">and</span>
  <span m="3273140">you</span> <span m="3273590">would</span> <span m="3273710">probably</span>
  <span m="3274010">be</span> <span m="3274280">averaging</span> <span m="3274880">over</span>
  <span m="3275180">a</span> <span m="3275240">large</span> <span m="3275600">number</span>
  <span m="3275810">of</span> <span m="3275870">previous</span> <span m="3276200">time</span>
  <span m="3276500">steps</span> <span m="3276920">to</span> <span m="3277100">get</span>
  <span m="3277310">this</span> <span m="3277430">smooth</span> <span m="3277910">property.</span>
  <span m="3279020">And</span> <span m="3279110">then</span> <span m="3279260">you'd</span>
  <span m="3279350">model</span> <span m="3280100">xt</span> <span m="3280670">minus</span>
  <span m="3281060">bt</span> <span m="3282470">by</span> <span m="3283220">this</span>
  <span m="3283940">autoregressive</span> <span m="3284480">process,</span> <span
  m="3285620">where</span> <span m="3286490">you</span> <span m="3286610">might,</span>
  <span m="3286790">for</span> <span m="3286940">example,</span> <span m="3287480">just</span>
  <span m="3287780">be</span> <span m="3287930">looking</span> <span m="3288380">at</span>
  <span m="3289340">just</span> <span m="3289580">the</span> <span m="3289640">previous</span>
  <span m="3289940">couple</span> <span m="3290210">of</span> <span m="3290300">time</span>
  <span m="3290600">steps.</span> <span m="3290930">And</span> <span m="3291020">you</span>
  <span m="3291080">recognize</span> <span m="3291500">that</span> <span m="3291590">you're</span>
  <span m="3291680">just</span> <span m="3291800">doing</span> <span m="3291980">much</span>
  <span m="3292160">more</span> <span m="3292310">random</span> <span m="3292730">fluctuations.</span></p><p><span
  m="3295600">And</span> <span m="3295730">then--</span> <span m="3296870">so</span>
  <span m="3296960">that's</span> <span m="3297170">how</span> <span m="3297410">one</span>
  <span m="3297740">would</span> <span m="3297950">now</span> <span m="3298130">model</span>
  <span m="3298730">normal</span> <span m="3299210">heart</span> <span m="3299480">rate</span>
  <span m="3299630">dynamics.</span> <span m="3300650">And</span> <span m="3300800">again,</span>
  <span m="3301820">it's</span> <span m="3302000">just--</span> <span m="3302900">this</span>
  <span m="3303230">is</span> <span m="3303380">an</span> <span m="3303500">example</span>
  <span m="3303830">of</span> <span m="3303890">a</span> <span m="3303950">statistical</span>
  <span m="3304400">model.</span> <span m="3304730">There</span> <span m="3304790">is</span>
  <span m="3304940">no</span> <span m="3305120">mechanistic</span> <span m="3305690">knowledge</span>
  <span m="3306110">of</span> <span m="3306200">hearts</span> <span m="3307100">being</span>
  <span m="3307280">used</span> <span m="3307580">here,</span> <span m="3308240">but</span>
  <span m="3308450">we</span> <span m="3308540">can</span> <span m="3308690">fit</span>
  <span m="3308930">the</span> <span m="3309020">data</span> <span m="3309470">of</span>
  <span m="3309650">normal</span> <span m="3310010">hearts</span> <span m="3310310">pretty</span>
  <span m="3310580">well</span> <span m="3311030">using</span> <span m="3311300">this.</span>
  <span m="3313710">But</span> <span m="3313860">the</span> <span m="3313920">next</span>
  <span m="3314190">question</span> <span m="3314580">and</span> <span m="3314670">the</span>
  <span m="3314760">most</span> <span m="3315240">interesting</span> <span m="3315690">one</span>
  <span m="3315960">is,</span> <span m="3316110">how</span> <span m="3316290">does</span>
  <span m="3316650">one</span> <span m="3316860">now</span> <span m="3317100">model</span>
  <span m="3317430">artifactual</span> <span m="3318120">events?</span> <span m="3320510">So</span>
  <span m="3320780">for</span> <span m="3320900">that,</span> <span m="3321140">that's</span>
  <span m="3321440">where</span> <span m="3321710">some</span> <span m="3323150">mechanistic</span>
  <span m="3323720">knowledge</span> <span m="3324080">comes</span> <span m="3324410">in.</span></p><p><span
  m="3326120">So</span> <span m="3326270">one</span> <span m="3326480">models</span>
  <span m="3326870">that</span> <span m="3327020">the</span> <span m="3327110">probe</span>
  <span m="3327540">dropouts</span> <span m="3330180">are</span> <span m="3330620">given</span>
  <span m="3331310">by</span> <span m="3332330">recognizing</span> <span m="3333140">that,</span>
  <span m="3333710">if</span> <span m="3334130">a</span> <span m="3334400">probe</span>
  <span m="3335120">is</span> <span m="3335570">removed</span> <span m="3336260">from</span>
  <span m="3336440">the</span> <span m="3336530">baby,</span> <span m="3337010">then</span>
  <span m="3337190">there</span> <span m="3337280">should</span> <span m="3337460">no</span>
  <span m="3337700">longer</span> <span m="3338360">be--</span> <span m="3339020">or</span>
  <span m="3339140">at</span> <span m="3339200">least</span> <span m="3339500">if</span>
  <span m="3339740">you--</span> <span m="3339860">after</span> <span m="3340370">a</span>
  <span m="3340400">small</span> <span m="3340670">amount</span> <span m="3340880">of</span>
  <span m="3340940">time,</span> <span m="3341270">there</span> <span m="3341360">should</span>
  <span m="3341510">no</span> <span m="3341630">longer</span> <span m="3341930">be</span>
  <span m="3342020">any</span> <span m="3342230">dependence</span> <span m="3342920">on</span>
  <span m="3343100">the</span> <span m="3343190">true</span> <span m="3343730">value</span>
  <span m="3344120">of</span> <span m="3344210">the</span> <span m="3344290">baby.</span>
  <span m="3344450">For</span> <span m="3344540">example,</span> <span m="3345230">the</span>
  <span m="3345350">blood</span> <span m="3345560">pressure,</span> <span m="3346980">once</span>
  <span m="3347120">the</span> <span m="3347240">blood</span> <span m="3347510">pressure</span>
  <span m="3347810">probe</span> <span m="3348080">is</span> <span m="3348170">removed,</span>
  <span m="3348650">is</span> <span m="3348770">no</span> <span m="3348980">longer</span>
  <span m="3349550">related</span> <span m="3349970">to</span> <span m="3350060">the</span>
  <span m="3350180">baby's</span> <span m="3350510">true</span> <span m="3350660">blood</span>
  <span m="3350870">pressure.</span></p><p><span m="3352910">But</span> <span m="3352960">there</span>
  <span m="3353080">might</span> <span m="3353290">be</span> <span m="3353440">some</span>
  <span m="3354010">delay</span> <span m="3354490">to</span> <span m="3354640">that</span>
  <span m="3355180">lack</span> <span m="3355510">of</span> <span m="3355600">dependence.</span>
  <span m="3357130">And</span> <span m="3357670">so--</span> <span m="3357950">and</span>
  <span m="3358060">that</span> <span m="3358210">is</span> <span m="3358330">going</span>
  <span m="3358480">to</span> <span m="3358570">be</span> <span m="3358630">encoded</span>
  <span m="3359050">in</span> <span m="3359110">some</span> <span m="3359320">domain</span>
  <span m="3359590">knowledge.</span> <span m="3359950">So</span> <span m="3360070">for</span>
  <span m="3360160">example,</span> <span m="3360440">in</span> <span m="3360520">the</span>
  <span m="3360580">temperature</span> <span m="3361060">probe,</span> <span m="3361840">when</span>
  <span m="3361990">you</span> <span m="3362110">remove</span> <span m="3362420">the</span>
  <span m="3362530">temperature</span> <span m="3362950">probe</span> <span m="3363250">from</span>
  <span m="3363460">the</span> <span m="3363550">baby,</span> <span m="3364480">it</span>
  <span m="3364570">starts</span> <span m="3364870">heating</span> <span m="3365170">up</span>
  <span m="3365320">again--</span> <span m="3365720">or</span> <span m="3365950">it</span>
  <span m="3366100">starts</span> <span m="3366340">cooling,</span> <span m="3367440">so</span>
  <span m="3367690">assuming</span> <span m="3368080">that</span> <span m="3368200">the</span>
  <span m="3368290">ambient</span> <span m="3368770">temperature</span> <span m="3369190">is</span>
  <span m="3369310">cooler</span> <span m="3369640">than</span> <span m="3369790">the</span>
  <span m="3369850">baby's</span> <span m="3370150">temperature.</span> <span m="3371280">So</span>
  <span m="3371380">you</span> <span m="3371480">take</span> <span m="3371560">it</span>
  <span m="3371650">off</span> <span m="3372040">the</span> <span m="3372160">baby.</span>
  <span m="3372790">It</span> <span m="3372880">starts</span> <span m="3373180">cooling</span>
  <span m="3373510">down.</span></p><p><span m="3374170">How</span> <span m="3374470">fast</span>
  <span m="3374860">does</span> <span m="3374950">it</span> <span m="3375010">cool</span>
  <span m="3375310">down?</span> <span m="3375730">Well,</span> <span m="3375880">you
  could</span> <span m="3376060">assume</span> <span m="3376390">that</span> <span
  m="3376510">it</span> <span m="3376600">cools</span> <span m="3376930">down</span>
  <span m="3377400">with</span> <span m="3377530">some</span> <span m="3377710">exponential</span>
  <span m="3378280">decay</span> <span m="3378760">from</span> <span m="3378940">the</span>
  <span m="3379030">baby's</span> <span m="3379300">temperature.</span> <span m="3380320">And</span>
  <span m="3380710">this is</span> <span m="3380850">something</span> <span m="3381190">that</span>
  <span m="3381670">is</span> <span m="3381790">very</span> <span m="3382000">reasonable,</span>
  <span m="3382750">and</span> <span m="3382840">you</span> <span m="3382930">could</span>
  <span m="3383050">imagine,</span> <span m="3384010">maybe</span> <span m="3384310">if</span>
  <span m="3384400">you</span> <span m="3384490">had</span> <span m="3384640">label</span>
  <span m="3384970">data</span> <span m="3385240">for</span> <span m="3385360">just</span>
  <span m="3385540">a</span> <span m="3385600">few</span> <span m="3386020">of</span>
  <span m="3386110">the</span> <span m="3386200">babies,</span> <span m="3386530">you</span>
  <span m="3386590">could</span> <span m="3386680">try</span> <span m="3386800">to</span>
  <span m="3386890">fit</span> <span m="3387220">the</span> <span m="3387310">parameters</span>
  <span m="3387760">of the</span> <span m="3387850">exponential</span> <span m="3388450">very</span>
  <span m="3388690">quickly.</span> <span m="3390840">And</span> <span m="3391060">in</span>
  <span m="3391150">this</span> <span m="3391300">way,</span> <span m="3391480">now,</span>
  <span m="3391630">we</span> <span m="3391780">parameterize</span> <span m="3392590">the</span>
  <span m="3392680">conditional</span> <span m="3393160">distribution</span> <span
  m="3394120">of</span> <span m="3394840">the</span> <span m="3394960">temperature</span>
  <span m="3395500">probe,</span> <span m="3396370">given</span> <span m="3397900">both</span>
  <span m="3398320">the</span> <span m="3398440">state</span> <span m="3399040">and</span>
  <span m="3399850">whether</span> <span m="3400330">the</span> <span m="3400420">artifact</span>
  <span m="3400900">occurred</span> <span m="3401230">or</span> <span m="3401290">not,</span>
  <span m="3402220">using</span> <span m="3402550">this</span> <span m="3402790">very</span>
  <span m="3403030">simple</span> <span m="3403480">exponential</span> <span m="3403990">decay.</span></p><p><span
  m="3405710">And</span> <span m="3405910">in</span> <span m="3406000">this</span>
  <span m="3406090">paper,</span> <span m="3406390">they</span> <span m="3406510">give</span>
  <span m="3406720">a</span> <span m="3406780">very</span> <span m="3407050">similar</span>
  <span m="3407560">type</span> <span m="3408040">of--</span> <span m="3410010">they</span>
  <span m="3410140">make</span> <span m="3410290">similar</span> <span m="3410650">types</span>
  <span m="3410890">of--</span> <span m="3411160">analogous</span> <span m="3411580">types</span>
  <span m="3411790">of</span> <span m="3411850">assumptions</span> <span m="3412420">for</span>
  <span m="3412540">all</span> <span m="3412690">of</span> <span m="3412750">the</span>
  <span m="3412840">other</span> <span m="3413050">artifactual</span> <span m="3413620">probes.</span>
  <span m="3414730">You</span> <span m="3414880">should</span> <span m="3415000">think</span>
  <span m="3415180">about</span> <span m="3415330">this</span> <span m="3415480">as</span>
  <span m="3415630">constraining</span> <span m="3416380">these</span> <span m="3416560">conditional</span>
  <span m="3417010">distributions</span> <span m="3417730">I</span> <span m="3417850">showed</span>
  <span m="3418060">you</span> <span m="3418150">here.</span> <span m="3418820">They're</span>
  <span m="3418960">no</span> <span m="3419110">longer</span> <span m="3419560">allowed</span>
  <span m="3419770">to</span> <span m="3419860">be</span> <span m="3419950">arbitrary</span>
  <span m="3420430">distributions,</span> <span m="3421090">and so</span> <span m="3421240">that,</span>
  <span m="3421570">when</span> <span m="3421840">one</span> <span m="3422140">does</span>
  <span m="3422470">now</span> <span m="3422710">expectation</span> <span m="3423310">maximization</span>
  <span m="3423910">to</span> <span m="3424000">try</span> <span m="3424150">to</span>
  <span m="3424240">maximize</span> <span m="3424660">the</span> <span m="3424750">marginal</span>
  <span m="3425080">likelihood</span> <span m="3425500">of</span> <span m="3425560">the</span>
  <span m="3425650">data,</span> <span m="3426580">you've</span> <span m="3426730">now</span>
  <span m="3426910">constrained</span> <span m="3427510">it</span> <span m="3427600">in</span>
  <span m="3427690">a</span> <span m="3427750">way</span> <span m="3427990">that</span>
  <span m="3428110">you</span> <span m="3428200">hopefully</span> <span m="3428530">are</span>
  <span m="3428610">moved</span> <span m="3428950">on</span> <span m="3429070">to</span>
  <span m="3429220">identifyability</span> <span m="3429830">of</span> <span m="3429870">the</span>
  <span m="3429940">learning</span> <span m="3430240">problem.</span> <span m="3431310">It</span>
  <span m="3431530">makes</span> <span m="3431830">all</span> <span m="3432130">of
  the</span> <span m="3432220">difference</span> <span m="3432550">in</span> <span
  m="3432610">learning</span> <span m="3433090">here.</span></p><p><span m="3438130">So</span>
  <span m="3438400">in</span> <span m="3439210">this</span> <span m="3439360">paper,</span>
  <span m="3439750">their</span> <span m="3439960">evaluation</span> <span m="3441730">did</span>
  <span m="3441940">a</span> <span m="3442000">little</span> <span m="3442300">bit</span>
  <span m="3442450">of</span> <span m="3442510">fine</span> <span m="3442840">tuning</span>
  <span m="3443200">for</span> <span m="3443320">each</span> <span m="3443470">baby.</span>
  <span m="3443830">In</span> <span m="3443920">particular,</span> <span m="3444520">they</span>
  <span m="3444670">assumed</span> <span m="3445180">that</span> <span m="3445330">the</span>
  <span m="3445420">first</span> <span m="3445810">30</span> <span m="3446140">minutes</span>
  <span m="3446650">near</span> <span m="3447340">the</span> <span m="3448030">start</span>
  <span m="3449200">consists</span> <span m="3449950">of</span> <span m="3450250">normal</span>
  <span m="3450670">dynamics</span> <span m="3451150">so</span> <span m="3451240">that's</span>
  <span m="3451480">there</span> <span m="3451630">are</span> <span m="3451690">no</span>
  <span m="3451900">artifacts.</span> <span m="3453190">That's,</span> <span m="3453460">of</span>
  <span m="3453610">course,</span> <span m="3453850">a</span> <span m="3453910">big</span>
  <span m="3454120">assumption,</span> <span m="3454750">but</span> <span m="3455140">they</span>
  <span m="3455290">use</span> <span m="3455530">that</span> <span m="3455680">to</span>
  <span m="3455800">try</span> <span m="3455950">to</span> <span m="3456070">fine</span>
  <span m="3456430">tune</span> <span m="3457030">the</span> <span m="3458140">dynamic</span>
  <span m="3458590">model</span> <span m="3459100">to</span> <span m="3459400">fine</span>
  <span m="3459640">tune it</span> <span m="3459820">for</span> <span m="3459970">each</span>
  <span m="3460120">baby</span> <span m="3460420">and</span> <span m="3461830">for</span>
  <span m="3462010">themselves.</span></p><p><span m="3463540">And</span> <span m="3463630">then</span>
  <span m="3463780">they</span> <span m="3463900">looked</span> <span m="3464230">at</span>
  <span m="3464500">the</span> <span m="3464590">ability</span> <span m="3465070">to</span>
  <span m="3465190">try</span> <span m="3465340">to</span> <span m="3465400">identify</span>
  <span m="3465940">artifactual</span> <span m="3466510">processes.</span> <span m="3467620">Now,</span>
  <span m="3468040">I</span> <span m="3468130">want</span> <span m="3468250">to</span>
  <span m="3468310">go</span> <span m="3468430">a</span> <span m="3468460">little</span>
  <span m="3468580">bit</span> <span m="3468700">slowly</span> <span m="3469060">through</span>
  <span m="3469200">this</span> <span m="3469330">plot,</span> <span m="3469690">because</span>
  <span m="3469930">it's</span> <span m="3470170">quite</span> <span m="3470380">interesting.</span>
  <span m="3472350">So</span> <span m="3472490">what</span> <span m="3472640">I'm</span>
  <span m="3472760">showing</span> <span m="3473120">you</span> <span m="3473240">here</span>
  <span m="3474290">is</span> <span m="3475040">a</span> <span m="3475580">ROC</span>
  <span m="3476030">curve</span> <span m="3477990">of</span> <span m="3478080">the</span>
  <span m="3478170">ability</span> <span m="3478560">to</span> <span m="3478770">predict</span>
  <span m="3479520">each</span> <span m="3479850">of</span> <span m="3480060">the</span>
  <span m="3480120">four</span> <span m="3480420">different</span> <span m="3480660">types</span>
  <span m="3480840">of</span> <span m="3480930">artifacts.</span> <span m="3481500">For</span>
  <span m="3481590">example,</span> <span m="3482500">at</span> <span m="3482520">any</span>
  <span m="3482700">one</span> <span m="3482880">point</span> <span m="3483030">in</span>
  <span m="3483150">time,</span> <span m="3483810">was</span> <span m="3484080">there</span>
  <span m="3484260">a</span> <span m="3484320">blood</span> <span m="3484650">sample</span>
  <span m="3485070">being</span> <span m="3485280">taken</span> <span m="3485610">or</span>
  <span m="3485670">not?</span> <span m="3485990">At</span> <span m="3486070">any</span>
  <span m="3486180">one</span> <span m="3486390">point</span> <span m="3486570">in</span>
  <span m="3486660">time,</span> <span m="3487440">was</span> <span m="3487710">there</span>
  <span m="3487890">a</span> <span m="3487920">core</span> <span m="3488220">temperature</span>
  <span m="3488940">disconnect</span> <span m="3489720">of</span> <span m="3490170">the</span>
  <span m="3490290">core</span> <span m="3490440">temperature</span> <span m="3490800">probe?</span></p><p><span
  m="3492320">And</span> <span m="3492510">to</span> <span m="3492630">evaluate</span>
  <span m="3493170">it,</span> <span m="3493260">they're</span> <span m="3493410">assuming</span>
  <span m="3493770">that</span> <span m="3493860">they</span> <span m="3493950">have</span>
  <span m="3494160">some</span> <span m="3494400">label</span> <span m="3494670">data</span>
  <span m="3494970">for</span> <span m="3495110">evaluation</span> <span m="3495720">purposes</span>
  <span m="3496170">only.</span> <span m="3498850">And</span> <span m="3498940">of</span>
  <span m="3499030">course,</span> <span m="3499330">you</span> <span m="3499420">want</span>
  <span m="3499660">to</span> <span m="3499810">be at</span> <span m="3499990">the</span>
  <span m="3500080">very</span> <span m="3500320">far</span> <span m="3500770">top</span>
  <span m="3501130">left</span> <span m="3501460">corner</span> <span m="3502110">up</span>
  <span m="3502230">here.</span> <span m="3503866">And</span> <span m="3504310">what</span>
  <span m="3504480">we're</span> <span m="3504600">showing</span> <span m="3504930">here</span>
  <span m="3505170">are</span> <span m="3505200">three</span> <span m="3505680">different</span>
  <span m="3506070">curves--</span> <span m="3507820">the</span> <span m="3508210">very</span>
  <span m="3508810">faint</span> <span m="3509740">dotted</span> <span m="3510160">line,</span>
  <span m="3511070">which</span> <span m="3511120">I'm</span> <span m="3511210">going</span>
  <span m="3511320">to</span> <span m="3511390">trace</span> <span m="3511750">out</span>
  <span m="3511960">with</span> <span m="3512110">my</span> <span m="3512260">cursor,</span>
  <span m="3513640">is</span> <span m="3513790">the</span> <span m="3513880">baseline.</span>
  <span m="3514780">Think</span> <span m="3514990">of</span> <span m="3515080">that</span>
  <span m="3515410">as</span> <span m="3516040">a</span> <span m="3517000">much</span>
  <span m="3517390">worse</span> <span m="3518080">algorithm.</span> <span m="3521750">Sorry.</span>
  <span m="3522140">That's</span> <span m="3522380">that</span> <span m="3522560">line</span>
  <span m="3522770">over</span> <span m="3522950">there.</span> <span m="3524650">Everyone</span>
  <span m="3524920">see</span> <span m="3525070">it?</span></p><p><span m="3529030">And</span>
  <span m="3529190">this</span> <span m="3529520">approach</span> <span m="3530270">are</span>
  <span m="3530420">the</span> <span m="3530510">other</span> <span m="3530750">two</span>
  <span m="3530930">lines.</span> <span m="3532110">Now,</span> <span m="3532190">what's</span>
  <span m="3532460">differentiating</span> <span m="3533450">those</span> <span m="3533720">other</span>
  <span m="3533990">two</span> <span m="3534260">lines</span> <span m="3534800">corresponds</span>
  <span m="3535400">to</span> <span m="3535550">the</span> <span m="3535640">particular</span>
  <span m="3536210">type</span> <span m="3536450">of</span> <span m="3536660">approximate</span>
  <span m="3537500">inference</span> <span m="3537940">algorithm</span> <span m="3538340">that's</span>
  <span m="3538580">used.</span> <span m="3540120">To</span> <span m="3540330">do</span>
  <span m="3540720">this</span> <span m="3542550">posterior</span> <span m="3543300">inference,</span>
  <span m="3544320">to</span> <span m="3544530">infer</span> <span m="3545640">the</span>
  <span m="3545730">true</span> <span m="3546120">value</span> <span m="3546420">of</span>
  <span m="3546510">the</span> <span m="3546570">x's</span> <span m="3547380">given</span>
  <span m="3547950">your</span> <span m="3548190">noisy</span> <span m="3548700">observations</span>
  <span m="3550290">in</span> <span m="3550410">the</span> <span m="3550470">model</span>
  <span m="3550860">given</span> <span m="3551160">here</span> <span m="3551820">is</span>
  <span m="3552000">actually</span> <span m="3552510">a</span> <span m="3552570">very</span>
  <span m="3553020">hard</span> <span m="3553800">inference</span> <span m="3554160">problem.</span>
  <span m="3555920">Mathematically,</span> <span m="3557430">I</span> <span m="3557670">think</span>
  <span m="3557880">one</span> <span m="3558030">can</span> <span m="3558150">show</span>
  <span m="3558330">that</span> <span m="3558510">it's</span> <span m="3558880">an
  NP-hard</span> <span m="3560340">computational</span> <span m="3560970">problem.</span></p><p><span
  m="3561940">And</span> <span m="3562080">so</span> <span m="3562170">they</span>
  <span m="3562260">have</span> <span m="3562410">to</span> <span m="3562500">approximate</span>
  <span m="3563130">it</span> <span m="3563190">in</span> <span m="3563280">some</span>
  <span m="3563460">way,</span> <span m="3563650">and they</span> <span m="3563730">use</span>
  <span m="3563880">two</span> <span m="3564090">different</span> <span m="3564330">approximations</span>
  <span m="3565140">here.</span> <span m="3566010">The</span> <span m="3566100">first</span>
  <span m="3566340">approximation</span> <span m="3566940">is</span> <span m="3567060">based</span>
  <span m="3567570">on</span> <span m="3568200">what</span> <span m="3568320">they're</span>
  <span m="3568400">calling</span> <span m="3568610">a</span> <span m="3568680">Gaussian</span>
  <span m="3569190">sum</span> <span m="3569460">approximation,</span> <span m="3571110">and</span>
  <span m="3571320">it's</span> <span m="3571530">a</span> <span m="3571590">deterministic</span>
  <span m="3572310">approximation.</span> <span m="3573420">The</span> <span m="3573510">second</span>
  <span m="3573840">approximation</span> <span m="3574380">is</span> <span m="3574470">based</span>
  <span m="3574710">on</span> <span m="3574800">a</span> <span m="3574830">Monte</span>
  <span m="3575130">Carlo</span> <span m="3575520">method.</span></p><p><span m="3577240">And</span>
  <span m="3577920">what</span> <span m="3578100">you</span> <span m="3578220">see</span>
  <span m="3578430">here</span> <span m="3578640">is</span> <span m="3578700">that</span>
  <span m="3578790">the</span> <span m="3578880">Gaussian</span> <span m="3579330">sum</span>
  <span m="3579540">approximation</span> <span m="3580290">is</span> <span m="3580440">actually</span>
  <span m="3580740">dramatically</span> <span m="3581340">better.</span> <span m="3581970">So</span>
  <span m="3582120">for</span> <span m="3582210">example,</span> <span m="3582570">in</span>
  <span m="3582630">this</span> <span m="3582750">blood</span> <span m="3582990">sample</span>
  <span m="3583290">one,</span> <span m="3583920">that</span> <span m="3584260">the</span>
  <span m="3584460">ROC</span> <span m="3584790">curve</span> <span m="3585240">looks</span>
  <span m="3585480">like</span> <span m="3585690">this</span> <span m="3586500">for</span>
  <span m="3588090">the</span> <span m="3588210">Gaussian</span> <span m="3588570">sum</span>
  <span m="3588750">approximation.</span> <span m="3589800">Whereas</span> <span m="3590010">for</span>
  <span m="3590100">the</span> <span m="3590190">Monte</span> <span m="3590430">Carlo</span>
  <span m="3590700">approximation,</span> <span m="3591390">it's</span> <span m="3592050">actually</span>
  <span m="3592350">significantly</span> <span m="3592950">lower.</span> <span m="3594510">And</span>
  <span m="3594630">this</span> <span m="3594780">is</span> <span m="3594840">just</span>
  <span m="3595020">to</span> <span m="3595080">point</span> <span m="3595320">out</span>
  <span m="3595470">that,</span> <span m="3596040">even</span> <span m="3596400">in</span>
  <span m="3597000">this</span> <span m="3597120">setting,</span> <span m="3597780">where</span>
  <span m="3600930">we</span> <span m="3601140">have</span> <span m="3602460">very</span>
  <span m="3602730">little</span> <span m="3602910">data,</span> <span m="3603660">we're</span>
  <span m="3603750">using</span> <span m="3603960">a</span> <span m="3603990">lot</span>
  <span m="3604170">of</span> <span m="3604260">domain</span> <span m="3604560">knowledge,</span>
  <span m="3605550">the</span> <span m="3605970">actual</span> <span m="3606300">details</span>
  <span m="3606780">of</span> <span m="3606870">how</span> <span m="3607050">one</span>
  <span m="3607320">does</span> <span m="3607830">the</span> <span m="3608220">math--</span>
  <span m="3608670">in</span> <span m="3608760">particular,</span> <span m="3609150">the</span>
  <span m="3609220">proximate</span> <span m="3609570">inference--</span> <span m="3610110">can</span>
  <span m="3610290">make</span> <span m="3610470">a</span> <span m="3610530">really</span>
  <span m="3610740">big</span> <span m="3610920">difference</span> <span m="3611460">in</span>
  <span m="3611610">the</span> <span m="3611700">performance</span> <span m="3612180">of</span>
  <span m="3612240">this</span> <span m="3612340">system.</span> <span m="3613770">And</span>
  <span m="3613830">so</span> <span m="3613950">it's</span> <span m="3614040">something</span>
  <span m="3614280">that</span> <span m="3614370">one</span> <span m="3614580">should</span>
  <span m="3614700">really</span> <span m="3614880">think</span> <span m="3615030">deeply</span>
  <span m="3615330">about,</span> <span m="3615570">as</span> <span m="3615690">well.</span></p><p><span
  m="3618666">I'm going to</span> <span m="3619130">skip</span> <span m="3620350">that</span>
  <span m="3620620">slide,</span> <span m="3620860">and</span> <span m="3620950">then</span>
  <span m="3621100">just</span> <span m="3621370">mention</span> <span m="3621700">very</span>
  <span m="3621880">briefly</span> <span m="3622150">this</span> <span m="3622360">one.</span>
  <span m="3623170">This</span> <span m="3623320">is</span> <span m="3623440">showing</span>
  <span m="3624190">an</span> <span m="3624310">inference</span> <span m="3625210">of</span>
  <span m="3627070">the</span> <span m="3627850">events.</span> <span m="3628640">So</span>
  <span m="3629380">here</span> <span m="3630710">I'm</span> <span m="3630850">showing</span>
  <span m="3631240">you</span> <span m="3631450">three</span> <span m="3632050">different</span>
  <span m="3632620">observations.</span> <span m="3634600">And</span> <span m="3635200">on</span>
  <span m="3635320">the</span> <span m="3635410">bottom</span> <span m="3635800">here,</span>
  <span m="3637420">I'm</span> <span m="3637450">showing</span> <span m="3637960">the</span>
  <span m="3638200">prediction</span> <span m="3639130">of</span> <span m="3639880">when</span>
  <span m="3640300">artifact--</span> <span m="3640870">two</span> <span m="3641050">different</span>
  <span m="3641300">artifactual</span> <span m="3641770">events</span> <span m="3642130">happened.</span>
  <span m="3643950">And</span> <span m="3644070">these</span> <span m="3644220">predictions</span>
  <span m="3644580">were</span> <span m="3644700">actually</span> <span m="3644910">quite</span>
  <span m="3645150">good,</span> <span m="3646020">using</span> <span m="3646290">this</span>
  <span m="3646410">model.</span></p><p><span m="3648180">So</span> <span m="3648420">I'm</span>
  <span m="3648540">done</span> <span m="3648720">with</span> <span m="3648840">that</span>
  <span m="3648960">first</span> <span m="3649230">example,</span> <span m="3650000">and--</span>
  <span m="3652210">and</span> <span m="3652940">the--</span> <span m="3653550">just</span>
  <span m="3653760">to</span> <span m="3653820">recap</span> <span m="3654300">the</span>
  <span m="3654750">important</span> <span m="3655170">points</span> <span m="3655380">of</span>
  <span m="3655440">that</span> <span m="3655560">example,</span> <span m="3656390">it</span>
  <span m="3656520">was</span> <span m="3657210">that</span> <span m="3658350">we</span>
  <span m="3658500">had</span> <span m="3658740">almost</span> <span m="3659160">no</span>
  <span m="3659370">label</span> <span m="3659670">data.</span> <span m="3661300">We're</span>
  <span m="3661450">tackling</span> <span m="3661990">this</span> <span m="3662140">problem</span>
  <span m="3663040">using</span> <span m="3663970">a</span> <span m="3664510">cleverly</span>
  <span m="3665080">chosen</span> <span m="3665470">statistical</span> <span m="3665890">model</span>
  <span m="3666250">with</span> <span m="3666460">some</span> <span m="3666790">domain</span>
  <span m="3667120">knowledge</span> <span m="3667480">built</span> <span m="3667840">in,</span>
  <span m="3668780">and</span> <span m="3668830">that</span> <span m="3669040">can</span>
  <span m="3669220">go</span> <span m="3669400">really</span> <span m="3669700">far.</span></p><p><span
  m="3672040">So</span> <span m="3672250">now</span> <span m="3672400">we'll</span>
  <span m="3672520">shift</span> <span m="3672760">gears</span> <span m="3673180">to</span>
  <span m="3673330">talk</span> <span m="3673570">about</span> <span m="3673900">a</span>
  <span m="3673960">different</span> <span m="3674290">type</span> <span m="3674500">of</span>
  <span m="3674560">problem</span> <span m="3674890">involving</span> <span m="3677050">physiological</span>
  <span m="3677710">data,</span> <span m="3678340">and</span> <span m="3678430">that's
  of</span> <span m="3678760">detecting</span> <span m="3679570">atrial</span> <span
  m="3679900">fibrillation.</span> <span m="3682570">So</span> <span m="3683310">what</span>
  <span m="3683430">I'm</span> <span m="3683520">showing</span> <span m="3683760">you</span>
  <span m="3683910">here</span> <span m="3684360">is</span> <span m="3684600">an</span>
  <span m="3684690">AliveCore</span> <span m="3685450">device.</span> <span m="3686280">I</span>
  <span m="3686610">own</span> <span m="3686760">one</span> <span m="3686910">of</span>
  <span m="3686970">these.</span> <span m="3687850">So</span> <span m="3687930">if</span>
  <span m="3688020">you</span> <span m="3688110">want</span> <span m="3688230">to</span>
  <span m="3688290">drop</span> <span m="3688530">by</span> <span m="3688590">my</span>
  <span m="3688950">E25</span> <span m="3689480">545</span> <span m="3690150">office,</span>
  <span m="3690540">you</span> <span m="3690660">can--</span> <span m="3690960">you</span>
  <span m="3691050">can</span> <span m="3691170">play</span> <span m="3691320">around</span>
  <span m="3691500">with</span> <span m="3691650">it.</span> <span m="3692860">And</span>
  <span m="3693120">if</span> <span m="3693210">you</span> <span m="3693270">attach</span>
  <span m="3693540">it</span> <span m="3693630">to</span> <span m="3693720">your</span>
  <span m="3693810">mobile</span> <span m="3694050">phone,</span> <span m="3695930">it'll</span>
  <span m="3696690">show</span> <span m="3697020">you</span> <span m="3698550">your</span>
  <span m="3701760">electric</span> <span m="3702330">conductance</span> <span m="3703050">through</span>
  <span m="3703200">your</span> <span m="3703380">heart</span> <span m="3703800">as</span>
  <span m="3704010">measured</span> <span m="3705240">through</span> <span m="3705780">your</span>
  <span m="3706110">two</span> <span m="3706350">fingers</span> <span m="3706710">touching</span>
  <span m="3706980">this</span> <span m="3707100">device</span> <span m="3707790">shown</span>
  <span m="3708060">over</span> <span m="3708240">here.</span> <span m="3708670">And</span>
  <span m="3708810">from</span> <span m="3709080">that,</span> <span m="3709470">one</span>
  <span m="3709650">can</span> <span m="3709770">try</span> <span m="3709890">to</span>
  <span m="3709980">detect</span> <span m="3710490">whether</span> <span m="3710670">the</span>
  <span m="3710730">patient</span> <span m="3711030">has</span> <span m="3711270">atrial</span>
  <span m="3711540">fibrillation.</span></p><p><span m="3712990">So</span> <span m="3713070">what</span>
  <span m="3713340">is</span> <span m="3713640">atrial</span> <span m="3713940">fibrillation?</span>
  <span m="3718630">Good</span> <span m="3718810">question.</span> <span m="3719200">It's</span>
  <span m="3719320">[INAUDIBLE].</span> <span m="3724240">So</span> <span m="3724600">this</span>
  <span m="3724810">is</span> <span m="3724960">from</span> <span m="3726310">the</span>
  <span m="3727030">American</span> <span m="3727540">Heart</span> <span m="3727780">Association.</span>
  <span m="3730270">They</span> <span m="3730390">defined</span> <span m="3730690">atrial</span>
  <span m="3730960">fibrillation</span> <span m="3731650">as</span> <span m="3732120">a</span>
  <span m="3732220">quivering</span> <span m="3733060">or</span> <span m="3733270">irregular</span>
  <span m="3733810">heartbeat,</span> <span m="3734780">also</span> <span m="3734980">known</span>
  <span m="3735190">as</span> <span m="3735340">arrhythmia.</span> <span m="3736450">And</span>
  <span m="3736960">one</span> <span m="3737140">of</span> <span m="3737200">the</span>
  <span m="3737260">big</span> <span m="3737440">challenges</span> <span m="3737950">is</span>
  <span m="3738010">that</span> <span m="3738130">it</span> <span m="3738220">could</span>
  <span m="3738370">lead</span> <span m="3738730">to</span> <span m="3739420">blood</span>
  <span m="3739660">clot,</span> <span m="3740080">stroke,</span> <span m="3740690">heart</span>
  <span m="3740770">failure,</span> <span m="3741040">and</span> <span m="3741130">so</span>
  <span m="3741280">on.</span></p><p><span m="3741530">So</span> <span m="3741810">here</span>
  <span m="3742050">is</span> <span m="3742270">how</span> <span m="3742420">a</span>
  <span m="3742480">patient</span> <span m="3742810">might</span> <span m="3742960">describe</span>
  <span m="3743980">having</span> <span m="3744460">atrial</span> <span m="3744760">fibrillation.</span>
  <span m="3746020">My</span> <span m="3746200">heart</span> <span m="3746500">flip-flops,</span>
  <span m="3747330">skips</span> <span m="3747700">beats,</span> <span m="3748180">feels</span>
  <span m="3748510">like</span> <span m="3748690">it's</span> <span m="3748810">banging</span>
  <span m="3749140">against</span> <span m="3749380">my</span> <span m="3749500">chest</span>
  <span m="3750100">wall,</span> <span m="3751150">particularly</span> <span m="3752020">when</span>
  <span m="3752260">I'm</span> <span m="3752380">carrying</span> <span m="3752800">stuff</span>
  <span m="3753070">up</span> <span m="3753160">my</span> <span m="3753340">stairs</span>
  <span m="3753790">or</span> <span m="3753850">bending</span> <span m="3754180">down.</span>
  <span m="3755920">Now</span> <span m="3756100">let's</span> <span m="3756250">try</span>
  <span m="3756370">to</span> <span m="3756460">look</span> <span m="3756610">at</span>
  <span m="3756700">a</span> <span m="3756760">picture</span> <span m="3757060">of</span>
  <span m="3757150">it.</span></p><p><span m="3768040">So</span> <span m="3772540">this</span>
  <span m="3772720">is</span> <span m="3772930">a</span> <span m="3773260">normal</span>
  <span m="3773740">heartbeat.</span> <span m="3775330">Hearts</span> <span m="3776820">move--</span>
  <span m="3777140">pumping</span> <span m="3778090">like</span> <span m="3778270">this.</span>
  <span m="3779860">And</span> <span m="3780730">if</span> <span m="3780850">you were</span>
  <span m="3780970">to</span> <span m="3781090">look</span> <span m="3781420">at</span>
  <span m="3781810">the</span> <span m="3782680">signal</span> <span m="3783130">output</span>
  <span m="3783430">of</span> <span m="3783520">the</span> <span m="3783570">EKG</span>
  <span m="3784150">of</span> <span m="3784240">a</span> <span m="3784270">normal</span>
  <span m="3784510">heartbeat,</span> <span m="3784810">it</span> <span m="3784870">would</span>
  <span m="3784960">look</span> <span m="3785140">like</span> <span m="3785320">this.</span>
  <span m="3785620">And</span> <span m="3785710">it's</span> <span m="3785890">roughly</span>
  <span m="3786250">corresponding</span> <span m="3786850">to</span> <span m="3787090">the</span>
  <span m="3787180">different--</span> <span m="3787735">the</span> <span m="3787990">signal</span>
  <span m="3788245">is</span> <span m="3788500">corresponding to</span> <span m="3788890">different</span>
  <span m="3789130">cycles</span> <span m="3789840">of</span> <span m="3790090">the</span>
  <span m="3790900">heartbeat.</span> <span m="3792420">Now</span> <span m="3792570">for</span>
  <span m="3792690">a</span> <span m="3792720">patient</span> <span m="3793120">who</span>
  <span m="3793350">has</span> <span m="3793750">atrial</span> <span m="3794070">fibrillation,</span>
  <span m="3795000">it</span> <span m="3795420">looks</span> <span m="3795630">more</span>
  <span m="3795810">like</span> <span m="3795960">this.</span></p><p><span m="3801650">So</span>
  <span m="3801860">much</span> <span m="3802160">more</span> <span m="3803540">obviously</span>
  <span m="3804050">abnormal,</span> <span m="3804500">at</span> <span m="3804590">least</span>
  <span m="3804770">in</span> <span m="3804830">this</span> <span m="3804950">figure.</span>
  <span m="3806160">And</span> <span m="3806210">if</span> <span m="3806270">you</span>
  <span m="3806330">look</span> <span m="3806510">at</span> <span m="3806570">the</span>
  <span m="3806660">corresponding</span> <span m="3807110">signal,</span> <span m="3807510">it</span>
  <span m="3807560">also</span> <span m="3807770">looks</span> <span m="3807980">very</span>
  <span m="3808160">different.</span> <span m="3810100">So</span> <span m="3810200">this</span>
  <span m="3810240">is</span> <span m="3810300">just</span> <span m="3810450">to</span>
  <span m="3810510">give</span> <span m="3810600">you</span> <span m="3810660">some</span>
  <span m="3810810">intuition</span> <span m="3811290">about</span> <span m="3811470">what</span>
  <span m="3811590">I</span> <span m="3811650">mean</span> <span m="3811890">by</span>
  <span m="3812190">atrial</span> <span m="3812490">fibrillation.</span></p><p><span
  m="3816990">So</span> <span m="3817370">what</span> <span m="3817520">we're</span>
  <span m="3817610">going</span> <span m="3817730">to</span> <span m="3817820">try</span>
  <span m="3817940">to</span> <span m="3818030">do</span> <span m="3818210">now</span>
  <span m="3818450">is</span> <span m="3818600">to</span> <span m="3818930">detect</span>
  <span m="3819410">it.</span> <span m="3819930">So</span> <span m="3820070">we're</span>
  <span m="3820190">going</span> <span m="3820400">to</span> <span m="3820910">take</span>
  <span m="3821360">data</span> <span m="3822350">like</span> <span m="3822620">that</span>
  <span m="3824090">and</span> <span m="3824420">try</span> <span m="3824570">to</span>
  <span m="3824690">classify</span> <span m="3825050">it</span> <span m="3825440">into
  a</span> <span m="3825660">number</span> <span m="3825890">of</span> <span m="3825950">different</span>
  <span m="3826370">categories.</span> <span m="3828580">Now</span> <span m="3829330">this</span>
  <span m="3829510">is</span> <span m="3829570">something</span> <span m="3829870">which</span>
  <span m="3830050">has</span> <span m="3830170">been</span> <span m="3830590">studied</span>
  <span m="3831100">for</span> <span m="3831340">decades,</span> <span m="3832630">and</span>
  <span m="3834640">last</span> <span m="3835090">year,</span> <span m="3835390">2017,</span>
  <span m="3836320">there</span> <span m="3836410">was</span> <span m="3836530">a</span>
  <span m="3836590">competition</span> <span m="3837430">run</span> <span m="3837700">by</span>
  <span m="3838330">Professor</span> <span m="3838900">Roger</span> <span m="3839230">Mark,</span>
  <span m="3840730">who</span> <span m="3841090">is</span> <span m="3841270">here</span>
  <span m="3841450">at</span> <span m="3841520">MIT,</span> <span m="3842530">which</span>
  <span m="3842710">is</span> <span m="3842800">trying</span> <span m="3842950">to</span>
  <span m="3843050">see,</span> <span m="3843380">well,</span> <span m="3843500">how</span>
  <span m="3843670">could--</span> <span m="3844390">how</span> <span m="3844570">good</span>
  <span m="3844840">are</span> <span m="3844930">we</span> <span m="3845170">at</span>
  <span m="3845440">trying</span> <span m="3845620">to</span> <span m="3845710">figure</span>
  <span m="3846010">out</span> <span m="3846460">which</span> <span m="3846670">patients</span>
  <span m="3847030">have</span> <span m="3847660">different</span> <span m="3847960">types</span>
  <span m="3848620">of</span> <span m="3848920">heart</span> <span m="3849190">rhythms</span>
  <span m="3849940">based</span> <span m="3850330">on</span> <span m="3850450">data</span>
  <span m="3850660">that</span> <span m="3850750">looks</span> <span m="3850900">like</span>
  <span m="3851020">this?</span></p><p><span m="3851780">So</span> <span m="3851800">this</span>
  <span m="3851980">is</span> <span m="3852070">a</span> <span m="3852130">normal</span>
  <span m="3852640">rhythm,</span> <span m="3853120">which</span> <span m="3853300">is</span>
  <span m="3853390">also</span> <span m="3853570">called</span> <span m="3853840">a</span>
  <span m="3854350">sinus</span> <span m="3855100">rhythm.</span> <span m="3856700">And</span>
  <span m="3857250">over</span> <span m="3857430">here</span> <span m="3857970">it's</span>
  <span m="3858360">atrial--</span> <span m="3858750">this</span> <span m="3858930">is</span>
  <span m="3859320">an</span> <span m="3859380">example</span> <span m="3859800">one</span>
  <span m="3860040">patient</span> <span m="3860370">who</span> <span m="3860460">has</span>
  <span m="3860610">atrial</span> <span m="3860910">fibrillation.</span> <span m="3862120">This</span>
  <span m="3862260">is</span> <span m="3862440">another</span> <span m="3863280">type</span>
  <span m="3863520">of</span> <span m="3863610">rhythm</span> <span m="3863880">that's</span>
  <span m="3864060">not</span> <span m="3864390">atrial</span> <span m="3864690">fibrillation,</span>
  <span m="3865200">but</span> <span m="3865320">is</span> <span m="3865440">abnormal.</span>
  <span m="3866590">And</span> <span m="3866690">this</span> <span m="3866730">is</span>
  <span m="3866820">a</span> <span m="3866910">noisy</span> <span m="3867390">recording--</span>
  <span m="3867880">for</span> <span m="3867990">example,</span> <span m="3868480">if</span>
  <span m="3868580">a</span> <span m="3868620">patient's--</span> <span m="3869670">doesn't</span>
  <span m="3870150">really</span> <span m="3870330">have</span> <span m="3870540">their</span>
  <span m="3870660">two</span> <span m="3870810">fingers</span> <span m="3871200">very</span>
  <span m="3871410">well</span> <span m="3872040">put</span> <span m="3872220">on
  to</span> <span m="3872430">the</span> <span m="3872490">two</span> <span m="3872670">leads</span>
  <span m="3873000">of</span> <span m="3873090">the</span> <span m="3873180">device.</span></p><p><span
  m="3875180">So</span> <span m="3876500">given</span> <span m="3878260">one</span>
  <span m="3878590">of</span> <span m="3878710">these</span> <span m="3879010">categories,</span>
  <span m="3879670">can</span> <span m="3879850">we</span> <span m="3880000">predict--</span>
  <span m="3881040">one</span> <span m="3881260">of</span> <span m="3881320">these</span>
  <span m="3881710">signals,</span> <span m="3882210">could</span> <span m="3882370">predict</span>
  <span m="3882760">which</span> <span m="3882910">category</span> <span m="3883330">it
  came</span> <span m="3883570">from?</span> <span m="3885470">So</span> <span m="3885490">if</span>
  <span m="3885580">you</span> <span m="3885640">looked</span> <span m="3885850">at</span>
  <span m="3886000">this,</span> <span m="3886370">you</span> <span m="3886470">might</span>
  <span m="3886510">recognize</span> <span m="3887230">that</span> <span m="3887800">they</span>
  <span m="3887950">look</span> <span m="3888130">a</span> <span m="3888160">bit</span>
  <span m="3888310">different.</span> <span m="3888970">So</span> <span m="3890020">could</span>
  <span m="3892120">some</span> <span m="3892300">of</span> <span m="3892390">you</span>
  <span m="3892540">guess</span> <span m="3892930">what</span> <span m="3893140">might</span>
  <span m="3893380">be</span> <span m="3893560">predictive</span> <span m="3894460">features</span>
  <span m="3895030">that</span> <span m="3895120">differentiate</span> <span m="3895780">one</span>
  <span m="3895990">of</span> <span m="3896110">these</span> <span m="3897880">signals</span>
  <span m="3898300">from</span> <span m="3898430">the</span> <span m="3898490">other?</span>
  <span m="3899440">In</span> <span m="3899530">the</span> <span m="3899590">back?</span></p><p><span
  m="3900760">AUDIENCE:</span> <span m="3900820">The</span> <span m="3900880">presence</span>
  <span m="3901300">and</span> <span m="3901520">absence</span> <span m="3901720">of
  one</span> <span m="3902080">of</span> <span m="3902440">the</span> <span m="3902800">peaks</span>
  <span m="3903280">the</span> <span m="3903460">QRS</span> <span m="3903880">complex</span>
  <span m="3904175">are</span> <span m="3904470">[INAUDIBLE].</span></p><p><span m="3907450">DAVID
  SONTAG:</span> <span m="3907495">So</span> <span m="3907540">speak</span> <span
  m="3907780">in</span> <span m="3907930">English</span> <span m="3908440">for</span>
  <span m="3909220">people</span> <span m="3909430">who</span> <span m="3909520">don't</span>
  <span m="3909640">know</span> <span m="3909700">what</span> <span m="3909790">these</span>
  <span m="3909910">terms</span> <span m="3910150">mean.</span></p><p><span m="3910750">AUDIENCE:</span>
  <span m="3910840">There</span> <span m="3910930">is</span> <span m="3911140">one</span>
  <span m="3911530">large</span> <span m="3911980">piece,</span> <span m="3912540">which
  can--</span> <span m="3912680">probably</span> <span m="3913240">we</span> <span
  m="3913500">can consider</span> <span m="3913610">one mV</span> <span m="3914510">and</span>
  <span m="3914970">there</span> <span m="3915150">is</span> <span m="3915310">another</span>
  <span m="3915580">peak,</span> <span m="3916730">which is</span> <span m="3917080">sort</span>
  <span m="3917350">of</span> <span m="3917480">like--</span> <span m="3918520">they</span>
  <span m="3918580">have</span> <span m="3918850">reverse</span> <span m="3919300">polarity</span>
  <span m="3919740">between</span> <span m="3919900">normal</span> <span m="3920060">rhythm</span>
  <span m="3920630">and</span> <span m="3921040">[INAUDIBLE].</span></p><p><span m="3921310">DAVID
  SONTAG:</span> <span m="3921475">Good.</span> <span m="3921880">So</span> <span
  m="3923170">are</span> <span m="3923260">you a</span> <span m="3923330">cardiologist?</span></p><p><span
  m="3923820">AUDIENCE:</span> <span m="3924042">No.</span></p><p><span m="3924710">DAVID
  SONTAG:</span> <span m="3924780">No,</span> <span m="3924850">OK.</span> <span m="3926440">So</span>
  <span m="3927280">what</span> <span m="3927610">the</span> <span m="3927700">student</span>
  <span m="3928000">suggested</span> <span m="3928400">is</span> <span m="3928610">one</span>
  <span m="3929050">could</span> <span m="3929200">look</span> <span m="3929440">for</span>
  <span m="3929770">sort</span> <span m="3929980">of</span> <span m="3930670">these</span>
  <span m="3930850">inversions</span> <span m="3931660">to</span> <span m="3932270">try</span>
  <span m="3932450">to</span> <span m="3932640">describe</span> <span m="3932920">it
  a</span> <span m="3932940">little bit</span> <span m="3933110">differently.</span>
  <span m="3934670">So</span> <span m="3937000">here</span> <span m="3939220">you're</span>
  <span m="3939530">suggesting</span> <span m="3939790">the</span> <span m="3939880">lack</span>
  <span m="3940270">of</span> <span m="3940360">those</span> <span m="3940510">inversions</span>
  <span m="3941290">is</span> <span m="3942190">predictive</span> <span m="3942650">of</span>
  <span m="3943030">an</span> <span m="3943120">abnormal</span> <span m="3943570">rhythm.</span>
  <span m="3945430">What</span> <span m="3945580">about</span> <span m="3945970">another</span>
  <span m="3946300">feature</span> <span m="3946660">that</span> <span m="3946780">could</span>
  <span m="3946900">be</span> <span m="3946990">predictive?</span> <span m="3947850">Yep?</span></p><p><span
  m="3948155">AUDIENCE:</span> <span m="3948307">The</span> <span m="3948460">spacing</span>
  <span m="3949060">between</span> <span m="3949430">the</span> <span m="3949500">peaks</span>
  <span m="3949840">is</span> <span m="3950180">more</span> <span m="3950460">irregular</span>
  <span m="3950740">with</span> <span m="3950960">the</span> <span m="3951316">AF.</span></p><p><span
  m="3952030">DAVID SONTAG:</span> <span m="3952180">The</span> <span m="3952330">spacing</span>
  <span m="3952990">between</span> <span m="3953380">beats</span> <span m="3953740">is</span>
  <span m="3953920">more</span> <span m="3954610">irregular</span> <span m="3955330">with</span>
  <span m="3955690">the</span> <span m="3956120">AF</span> <span m="3956540">rhythm.</span>
  <span m="3956860">So</span> <span m="3956980">you're</span> <span m="3957070">sort</span>
  <span m="3957310">of</span> <span m="3957400">looking</span> <span m="3957820">at</span>
  <span m="3957940">this.</span> <span m="3958270">You</span> <span m="3958360">see</span>
  <span m="3958510">how</span> <span m="3958780">here</span> <span m="3959170">this</span>
  <span m="3959380">spacing</span> <span m="3959890">is</span> <span m="3959980">very</span>
  <span m="3960160">different</span> <span m="3960400">from</span> <span m="3960550">this</span>
  <span m="3960750">spacing.</span> <span m="3961570">Whereas</span> <span m="3961900">in</span>
  <span m="3961960">the</span> <span m="3962050">normal</span> <span m="3962470">rhythm,</span>
  <span m="3962725">sort</span> <span m="3962980">of</span> <span m="3963100">the</span>
  <span m="3963190">spacing</span> <span m="3963580">looks</span> <span m="3963760">pretty</span>
  <span m="3964000">darn</span> <span m="3964840">regular.</span> <span m="3965690">All</span>
  <span m="3966120">right,</span> <span m="3966550">good.</span></p><p><span m="3967060">So</span>
  <span m="3968110">if</span> <span m="3968290">I</span> <span m="3968380">was</span>
  <span m="3968500">to</span> <span m="3968560">show</span> <span m="3968770">you</span>
  <span m="3969430">40</span> <span m="3969760">examples</span> <span m="3970300">of</span>
  <span m="3970390">these</span> <span m="3971050">and</span> <span m="3971230">then</span>
  <span m="3971530">ask</span> <span m="3971860">you</span> <span m="3971950">to</span>
  <span m="3972010">classify</span> <span m="3972400">some</span> <span m="3972490">new</span>
  <span m="3972640">ones,</span> <span m="3972940">how</span> <span m="3973090">well</span>
  <span m="3973240">do</span> <span m="3973300">you</span> <span m="3973360">think</span>
  <span m="3973510">you'll</span> <span m="3973550">be</span> <span m="3973620">able</span>
  <span m="3973750">to</span> <span m="3973840">do?</span> <span m="3975420">Pretty</span>
  <span m="3975570">well?</span> <span m="3980970">I</span> <span m="3981450">would</span>
  <span m="3981630">be</span> <span m="3981720">surprised</span> <span m="3982260">if</span>
  <span m="3982350">you</span> <span m="3982470">couldn't</span> <span m="3982740">do</span>
  <span m="3982920">reasonably</span> <span m="3983550">well</span> <span m="3983790">at</span>
  <span m="3983880">least</span> <span m="3984060">distinguishing</span> <span m="3984600">between</span>
  <span m="3984810">normal</span> <span m="3985170">rhythm</span> <span m="3985780">and</span>
  <span m="3986010">AF</span> <span m="3986250">rhythm,</span> <span m="3986940">because</span>
  <span m="3987210">there</span> <span m="3987330">seem</span> <span m="3987600">to</span>
  <span m="3987690">be</span> <span m="3987750">some</span> <span m="3987900">pretty</span>
  <span m="3988200">clear</span> <span m="3988620">signals</span> <span m="3989100">here.</span></p><p><span
  m="3990510">Of</span> <span m="3990600">course,</span> <span m="3990870">as</span>
  <span m="3991080">you</span> <span m="3991200">get</span> <span m="3991350">into</span>
  <span m="3991830">alternatives,</span> <span m="3992580">then the</span> <span m="3992710">story</span>
  <span m="3993030">gets</span> <span m="3993240">much</span> <span m="3993450">more</span>
  <span m="3993600">complex.</span> <span m="3995040">But</span> <span m="3995190">let</span>
  <span m="3995370">me</span> <span m="3995490">dig</span> <span m="3995730">in</span>
  <span m="3995820">a</span> <span m="3995850">little</span> <span m="3995970">bit</span>
  <span m="3996060">deeper</span> <span m="3996390">into</span> <span m="3996870">what</span>
  <span m="3997020">I</span> <span m="3997080">mean</span> <span m="3997230">by</span>
  <span m="3997350">this.</span> <span m="3997980">So</span> <span m="3998160">let's</span>
  <span m="3998310">define</span> <span m="3998700">some</span> <span m="3998820">of</span>
  <span m="3998880">these</span> <span m="3999000">terms.</span> <span m="3999600">Well,</span>
  <span m="4001070">cardiologists</span> <span m="4001790">have</span> <span m="4001910">studied</span>
  <span m="4002210">this</span> <span m="4002420">for</span> <span m="4003260">a</span>
  <span m="4003290">really</span> <span m="4003680">long</span> <span m="4003890">time,</span>
  <span m="4004430">and</span> <span m="4005270">they</span> <span m="4005570">have--</span>
  <span m="4005940">so</span> <span m="4005990">what</span> <span m="4006140">I'm</span>
  <span m="4006260">showing</span> <span m="4006530">you</span> <span m="4006650">here</span>
  <span m="4006980">is</span> <span m="4007520">one</span> <span m="4008030">heart</span>
  <span m="4008390">cycle.</span> <span m="4009380">And</span> <span m="4009710">they've--</span>
  <span m="4010250">you</span> <span m="4010490">can</span> <span m="4010880">put</span>
  <span m="4011120">names</span> <span m="4011720">to</span> <span m="4011930">each</span>
  <span m="4012200">of</span> <span m="4012350">the</span> <span m="4012500">peaks</span>
  <span m="4013010">that</span> <span m="4013130">you</span> <span m="4013220">would</span>
  <span m="4013340">see</span> <span m="4013700">in</span> <span m="4013820">a</span>
  <span m="4013880">regular</span> <span m="4014420">heart</span> <span m="4014720">cycle--</span>
  <span m="4015140">so</span> <span m="4015290">that--</span> <span m="4015440">for</span>
  <span m="4015500">example,</span> <span m="4015860">that</span> <span m="4016010">very</span>
  <span m="4016280">high</span> <span m="4016580">peak</span> <span m="4016940">is</span>
  <span m="4017060">known</span> <span m="4017330">as</span> <span m="4017510">the</span>
  <span m="4017690">R</span> <span m="4017930">peak.</span></p><p><span m="4019250">And</span>
  <span m="4020840">you</span> <span m="4020990">could</span> <span m="4021140">look</span>
  <span m="4021290">at,</span> <span m="4021410">for</span> <span m="4021500">example,</span>
  <span m="4021950">the</span> <span m="4022100">interval--</span> <span m="4023060">so</span>
  <span m="4023540">this</span> <span m="4023780">is</span> <span m="4025130">one</span>
  <span m="4026270">beat.</span> <span m="4026720">You</span> <span m="4026840">could</span>
  <span m="4026930">look</span> <span m="4027080">at</span> <span m="4027140">the</span>
  <span m="4027200">interval</span> <span m="4027710">between</span> <span m="4028310">the</span>
  <span m="4028670">R</span> <span m="4029000">peak</span> <span m="4029510">of</span>
  <span m="4029660">one</span> <span m="4029930">beat</span> <span m="4030320">and</span>
  <span m="4030470">the</span> <span m="4030710">R</span> <span m="4030980">peak</span>
  <span m="4031370">of</span> <span m="4031490">another</span> <span m="4031760">peak,</span>
  <span m="4032440">and</span> <span m="4032630">define</span> <span m="4033050">that</span>
  <span m="4033290">to</span> <span m="4033410">be</span> <span m="4033560">the</span>
  <span m="4034025">RR</span> <span m="4034490">interval.</span> <span m="4035440">In</span>
  <span m="4035720">a</span> <span m="4035780">similar</span> <span m="4036050">way,</span>
  <span m="4036380">one</span> <span m="4036590">could</span> <span m="4036740">take--</span>
  <span m="4038050">one</span> <span m="4038680">could</span> <span m="4038900">find</span>
  <span m="4039230">different</span> <span m="4039710">distinctive</span> <span m="4040340">elements</span>
  <span m="4041060">of</span> <span m="4041360">the</span> <span m="4041510">signal--</span>
  <span m="4042140">by</span> <span m="4042380">the way,</span> <span m="4042650">each--</span>
  <span m="4045680">each</span> <span m="4046130">time</span> <span m="4046570">step</span>
  <span m="4046760">corresponds</span> <span m="4047420">to</span> <span m="4047540">the</span>
  <span m="4047870">heart</span> <span m="4048110">being</span> <span m="4048290">in</span>
  <span m="4048380">a</span> <span m="4048410">different</span> <span m="4048650">position.</span>
  <span m="4050410">For</span> <span m="4050570">a</span> <span m="4050600">healthy</span>
  <span m="4050930">heart,</span> <span m="4051200">these</span> <span m="4051350">are</span>
  <span m="4051380">relatively</span> <span m="4051800">deterministic.</span> <span
  m="4053860">And</span> <span m="4054010">so</span> <span m="4054100">you</span>
  <span m="4054160">could</span> <span m="4054250">look</span> <span m="4054490">at</span>
  <span m="4054760">other</span> <span m="4055030">distances</span> <span m="4055750">and</span>
  <span m="4055990">derive</span> <span m="4056330">features</span> <span m="4056860">from</span>
  <span m="4056980">those</span> <span m="4057160">distances,</span> <span m="4057580">as</span>
  <span m="4057700">well,</span> <span m="4058010">just</span> <span m="4058060">like</span>
  <span m="4058180">we</span> <span m="4058240">were</span> <span m="4058330">talking</span>
  <span m="4058570">about,</span> <span m="4058750">both</span> <span m="4058960">within</span>
  <span m="4059620">a</span> <span m="4059710">beat</span> <span m="4060160">and</span>
  <span m="4060400">across</span> <span m="4060940">beats.</span> <span m="4062220">Yep?</span></p><p><span
  m="4062895">AUDIENCE:</span> <span m="4063142">So</span> <span m="4063390">what's</span>
  <span m="4063580">the</span> <span m="4063670">difference</span> <span m="4063910">between</span>
  <span m="4064230">a</span> <span m="4064270">segment</span> <span m="4064535">and
  an</span> <span m="4064800">interval</span> <span m="4065660">again?</span></p><p><span
  m="4069540">DAVID SONTAG:</span> <span m="4069635">I</span> <span m="4069730">don't</span>
  <span m="4069850">know what</span> <span m="4069950">the</span> <span m="4070010">difference</span>
  <span m="4070250">between</span> <span m="4070330">a</span> <span m="4070390">segment</span>
  <span m="4070730">and</span> <span m="4070790">an</span> <span m="4070880">interval</span>
  <span m="4071330">is.</span> <span m="4071420">Does</span> <span m="4071540">anyone</span>
  <span m="4071750">else</span> <span m="4071870">know?</span> <span m="4072070">I
  mean,</span> <span m="4072325">I guess</span> <span m="4072580">the</span> <span
  m="4072680">interval</span> <span m="4073100">is</span> <span m="4073190">between</span>
  <span m="4073610">probably</span> <span m="4073880">the</span> <span m="4074000">heads</span>
  <span m="4074270">of</span> <span m="4074360">peaks,</span> <span m="4074720">whereas</span>
  <span m="4074840">segments</span> <span m="4075290">might</span> <span m="4075440">refer</span>
  <span m="4075770">to</span> <span m="4076490">within</span> <span m="4077400">a</span>
  <span m="4077630">interval.</span> <span m="4079310">That's</span> <span m="4079460">my</span>
  <span m="4079610">guess.</span></p><p><span m="4079860">Does</span> <span m="4079920">someone</span>
  <span m="4080150">know</span> <span m="4080270">better?</span> <span m="4084190">For</span>
  <span m="4084730">the</span> <span m="4084820">purpose</span> <span m="4085090">of</span>
  <span m="4085150">today's</span> <span m="4085360">class,</span> <span m="4085630">that's
  a</span> <span m="4085780">good</span> <span m="4085930">enough</span> <span m="4086380">understanding.</span>
  <span m="4090940">The</span> <span m="4091000">point</span> <span m="4091240">is</span>
  <span m="4091360">this</span> <span m="4091510">is</span> <span m="4091600">well</span>
  <span m="4091840">understood.</span> <span m="4094060">One</span> <span m="4094300">could</span>
  <span m="4094450">derive</span> <span m="4094750">features</span> <span m="4095170">from</span>
  <span m="4095420">this.</span></p><p><span m="4096093">AUDIENCE:</span> <span m="4096314">By</span>
  <span m="4096536">us.</span></p><p><span m="4096979">DAVID SONTAG:</span> <span
  m="4097174">By</span> <span m="4097370">us.</span> <span m="4100180">So</span> <span
  m="4100600">what</span> <span m="4100770">would</span> <span m="4100899">a</span>
  <span m="4100930">traditional</span> <span m="4101439">approach</span> <span m="4101770">be</span>
  <span m="4101890">to</span> <span m="4101979">this</span> <span m="4102100">problem?</span>
  <span m="4103399">So</span> <span m="4103450">this</span> <span m="4103660">is--</span>
  <span m="4104020">I'm</span> <span m="4104200">pulling</span> <span m="4104439">this</span>
  <span m="4104560">figure</span> <span m="4104859">from</span> <span m="4105020">a</span>
  <span m="4105040">paper</span> <span m="4105310">from</span> <span m="4105430">2002.</span>
  <span m="4107050">What</span> <span m="4107260">it'll</span> <span m="4107410">do</span>
  <span m="4107680">is</span> <span m="4107859">it'll</span> <span m="4108380">take
  in</span> <span m="4108880">that</span> <span m="4109090">signal.</span> <span m="4110200">It'll</span>
  <span m="4110560">do</span> <span m="4110800">some</span> <span m="4111310">filtering</span>
  <span m="4112240">of</span> <span m="4112420">it.</span> <span m="4112960">Then</span>
  <span m="4113170">it'll</span> <span m="4113380">run</span> <span m="4113770">a</span>
  <span m="4113890">peak</span> <span m="4114399">detection</span> <span m="4114970">logic,</span>
  <span m="4115609">which</span> <span m="4115750">will</span> <span m="4116319">find</span>
  <span m="4117100">these</span> <span m="4117430">peaks,</span> <span m="4118420">and</span>
  <span m="4118540">then</span> <span m="4118689">it'll</span> <span m="4118840">measure</span>
  <span m="4119260">intervals</span> <span m="4119950">between</span> <span m="4120580">these</span>
  <span m="4120850">peaks</span> <span m="4121270">and</span> <span m="4121359">within</span>
  <span m="4122950">a</span> <span m="4123010">beat.</span> <span m="4123939">And</span>
  <span m="4124600">it'll</span> <span m="4124840">take</span> <span m="4125260">those</span>
  <span m="4127390">computations</span> <span m="4128069">or</span> <span m="4128140">make</span>
  <span m="4128290">some</span> <span m="4128439">decision</span> <span m="4128890">based</span>
  <span m="4129160">on</span> <span m="4129279">it.</span> <span m="4129760">So</span>
  <span m="4129880">that's</span> <span m="4130050">a</span> <span m="4130120">traditional</span>
  <span m="4130750">algorithm,</span> <span m="4131590">and</span> <span m="4131710">they</span>
  <span m="4131830">work</span> <span m="4132100">pretty</span> <span m="4132399">reasonably.</span></p><p><span
  m="4134310">And</span> <span m="4134439">so</span> <span m="4135010">what</span>
  <span m="4135130">do</span> <span m="4135220">I</span> <span m="4135310">mean</span>
  <span m="4135520">by</span> <span m="4135609">signal</span> <span m="4135910">processing?</span>
  <span m="4136560">Well,</span> <span m="4137020">this</span> <span m="4137229">is</span>
  <span m="4137350">an</span> <span m="4137439">example</span> <span m="4137840">of</span>
  <span m="4137890">that.</span> <span m="4138790">I</span> <span m="4139300">encourage</span>
  <span m="4139779">any</span> <span m="4139899">of</span> <span m="4139990">you</span>
  <span m="4140140">to</span> <span m="4140260">go</span> <span m="4140470">home</span>
  <span m="4140740">today</span> <span m="4141069">and</span> <span m="4141189">try</span>
  <span m="4141340">to</span> <span m="4141460">code</span> <span m="4141729">up</span>
  <span m="4141880">a</span> <span m="4141939">peaked</span> <span m="4142300">finding</span>
  <span m="4142689">algorithm.</span> <span m="4143140">It's</span> <span m="4143350">not</span>
  <span m="4143620">that</span> <span m="4143859">hard,</span> <span m="4144910">at</span>
  <span m="4144970">least</span> <span m="4145120">not</span> <span m="4145240">to</span>
  <span m="4145330">get</span> <span m="4145450">an</span> <span m="4145680">OK</span>
  <span m="4146029">one.</span> <span m="4146819">You</span> <span m="4146979">might</span>
  <span m="4147550">imagine</span> <span m="4147939">keeping</span> <span m="4148359">a</span>
  <span m="4148420">running</span> <span m="4150640">tab</span> <span m="4151149">of</span>
  <span m="4151720">what's</span> <span m="4151960">the</span> <span m="4152080">highest</span>
  <span m="4152500">signal</span> <span m="4152890">you've</span> <span m="4153069">seen</span>
  <span m="4153310">so</span> <span m="4153430">far.</span> <span m="4154300">Then</span>
  <span m="4154479">you</span> <span m="4154540">look</span> <span m="4154660">to</span>
  <span m="4154750">see</span> <span m="4154840">what</span> <span m="4154960">is</span>
  <span m="4155020">the</span> <span m="4155109">first</span> <span m="4155350">time</span>
  <span m="4155560">it</span> <span m="4155680">drops,</span> <span m="4156019">and</span>
  <span m="4156359">the</span> <span m="4156430">second</span> <span m="4156720">time--</span>
  <span m="4156880">and the</span> <span m="4156939">next</span> <span m="4157120">time</span>
  <span m="4157300">it</span> <span m="4157390">goes</span> <span m="4157660">up</span>
  <span m="4157840">larger</span> <span m="4158260">than,</span> <span m="4158540">let's</span>
  <span m="4158590">say,</span> <span m="4159470">the</span> <span m="4159569">previous--</span>
  <span m="4162100">suppose</span> <span m="4162430">that</span> <span m="4162550">one</span>
  <span m="4162700">of--</span> <span m="4162939">you</span> <span m="4163000">want</span>
  <span m="4163120">to</span> <span m="4163180">look</span> <span m="4163300">for</span>
  <span m="4164200">when</span> <span m="4164470">the</span> <span m="4164590">drop</span>
  <span m="4165160">is--</span> <span m="4165609">the</span> <span m="4165700">maximum</span>
  <span m="4166240">value--</span> <span m="4166689">recent</span> <span m="4167100">maximum</span>
  <span m="4167439">value</span> <span m="4167740">divided</span> <span m="4168069">by</span>
  <span m="4168220">2.</span> <span m="4168790">And</span> <span m="4168910">then</span>
  <span m="4169090">you--</span> <span m="4169870">then</span> <span m="4170050">you</span>
  <span m="4170140">reset.</span> <span m="4171279">And</span> <span m="4171399">you</span>
  <span m="4171460">can</span> <span m="4171550">imagine</span> <span m="4171819">in</span>
  <span m="4171880">this</span> <span m="4172029">way</span> <span m="4172649">very</span>
  <span m="4172930">quickly</span> <span m="4173260">coding</span> <span m="4173620">up</span>
  <span m="4173800">a</span> <span m="4173950">peak</span> <span m="4174189">finding</span>
  <span m="4174670">algorithm.</span></p><p><span m="4177830">And</span> <span m="4178060">so</span>
  <span m="4178540">this</span> <span m="4178779">is</span> <span m="4178840">just,</span>
  <span m="4178960">again,</span> <span m="4179140">to</span> <span m="4179229">give</span>
  <span m="4179319">you</span> <span m="4179380">some</span> <span m="4179529">intuition</span>
  <span m="4180160">behind</span> <span m="4180609">what</span> <span m="4181000">a</span>
  <span m="4181060">traditional</span> <span m="4181479">approach</span> <span m="4181779">would</span>
  <span m="4181899">be.</span> <span m="4183130">And</span> <span m="4183220">then</span>
  <span m="4184450">you</span> <span m="4184600">can</span> <span m="4184720">very</span>
  <span m="4184960">quickly</span> <span m="4185260">see</span> <span m="4185500">that</span>
  <span m="4185784">that--</span> <span m="4186790">once</span> <span m="4187000">you</span>
  <span m="4187090">start</span> <span m="4187300">to</span> <span m="4187390">look</span>
  <span m="4187540">at</span> <span m="4187600">some</span> <span m="4187750">intervals</span>
  <span m="4188350">between</span> <span m="4188890">peaks,</span> <span m="4189729">that</span>
  <span m="4190090">alone</span> <span m="4190510">is</span> <span m="4190870">often</span>
  <span m="4191290">good</span> <span m="4191470">enough</span> <span m="4192310">for</span>
  <span m="4192460">predicting</span> <span m="4192880">whether</span> <span m="4193060">a</span>
  <span m="4193090">patient</span> <span m="4193390">has</span> <span m="4194020">atrial</span>
  <span m="4194320">fibrillation.</span> <span m="4195050">So</span> <span m="4195610">this</span>
  <span m="4195850">is</span> <span m="4196180">a</span> <span m="4196420">figure</span>
  <span m="4196910">taken</span> <span m="4197140">from</span> <span m="4197290">paper</span>
  <span m="4197530">in</span> <span m="4197590">2001</span> <span m="4198940">showing</span>
  <span m="4199300">a</span> <span m="4199360">single</span> <span m="4199720">patient's</span>
  <span m="4200350">time</span> <span m="4200770">series.</span> <span m="4201310">So</span>
  <span m="4201940">the</span> <span m="4202060">x-axis</span> <span m="4202750">is</span>
  <span m="4203050">for</span> <span m="4203230">that</span> <span m="4203680">single</span>
  <span m="4204010">patient,</span> <span m="4204940">their</span> <span m="4205570">heart</span>
  <span m="4205810">beats</span> <span m="4206170">across</span> <span m="4206500">time.</span>
  <span m="4207250">The</span> <span m="4207370">y-axis</span> <span m="4207940">is</span>
  <span m="4208030">just</span> <span m="4208330">showing</span> <span m="4208630">the</span>
  <span m="4208780">RR</span> <span m="4209350">interval</span> <span m="4209830">between</span>
  <span m="4210310">the</span> <span m="4210400">previous</span> <span m="4211480">beat</span>
  <span m="4211840">and</span> <span m="4211990">the</span> <span m="4212080">current</span>
  <span m="4212500">beat.</span></p><p><span m="4214300">And</span> <span m="4214540">down</span>
  <span m="4214900">here</span> <span m="4215040">in</span> <span m="4215110">the</span>
  <span m="4215170">bottom</span> <span m="4216490">is</span> <span m="4217090">the</span>
  <span m="4217210">ground</span> <span m="4217570">truth</span> <span m="4218080">of</span>
  <span m="4218200">whether</span> <span m="4218650">the</span> <span m="4219160">patient</span>
  <span m="4219580">is</span> <span m="4219700">assessed</span> <span m="4220240">to</span>
  <span m="4220480">have--</span> <span m="4220990">to</span> <span m="4221140">be</span>
  <span m="4221440">in--</span> <span m="4222850">to</span> <span m="4222940">have</span>
  <span m="4223090">a</span> <span m="4223150">normal</span> <span m="4224710">rhythm</span>
  <span m="4225250">or</span> <span m="4225550">atrial</span> <span m="4225970">fibrillation,</span>
  <span m="4227650">which</span> <span m="4227890">is</span> <span m="4228070">noted</span>
  <span m="4228490">as</span> <span m="4228910">this</span> <span m="4229330">higher</span>
  <span m="4229870">value</span> <span m="4230260">here.</span> <span m="4230630">So</span>
  <span m="4230710">these</span> <span m="4231070">are</span> <span m="4231670">AF</span>
  <span m="4232690">rhythms.</span> <span m="4233830">This</span> <span m="4234010">is</span>
  <span m="4234130">normal.</span> <span m="4234710">This</span> <span m="4234790">is</span>
  <span m="4234940">AF</span> <span m="4235270">again.</span></p><p><span m="4236800">And</span>
  <span m="4237190">what</span> <span m="4237340">you</span> <span m="4237430">can</span>
  <span m="4237580">see</span> <span m="4237880">is</span> <span m="4238120">that</span>
  <span m="4238810">the</span> <span m="4239170">RR</span> <span m="4239770">interval</span>
  <span m="4240340">actually</span> <span m="4240670">gets</span> <span m="4240910">you</span>
  <span m="4241000">pretty</span> <span m="4241240">far.</span> <span m="4241640">You
  notice</span> <span m="4241810">how</span> <span m="4241960">it's</span> <span m="4242170">pretty</span>
  <span m="4242890">high</span> <span m="4243370">up</span> <span m="4243550">here.</span>
  <span m="4244210">Suddenly</span> <span m="4244780">it</span> <span m="4244840">drops.</span>
  <span m="4246130">The</span> <span m="4246350">RR</span> <span m="4246800">interval</span>
  <span m="4247120">drops</span> <span m="4247480">for</span> <span m="4247600">a</span>
  <span m="4247630">while,</span> <span m="4247930">and</span> <span m="4248020">that's</span>
  <span m="4248350">when</span> <span m="4248650">the</span> <span m="4248740">patient</span>
  <span m="4249010">has</span> <span m="4249460">AF.</span> <span m="4250450">Then</span>
  <span m="4250630">it</span> <span m="4250690">goes</span> <span m="4250930">up</span>
  <span m="4251080">again.</span> <span m="4251860">Then</span> <span m="4252010">it</span>
  <span m="4252130">drops</span> <span m="4252580">again,</span> <span m="4253300">and</span>
  <span m="4253390">so</span> <span m="4253570">on.</span> <span m="4254800">And</span>
  <span m="4255040">so</span> <span m="4255190">it's not</span> <span m="4255310">deterministic,</span>
  <span m="4256240">the</span> <span m="4256300">relationship,</span> <span m="4256780">but</span>
  <span m="4256900">there's</span> <span m="4257050">definitely</span> <span m="4257440">a</span>
  <span m="4257500">lot</span> <span m="4257710">of</span> <span m="4257800">signal</span>
  <span m="4258160">just</span> <span m="4258370">from</span> <span m="4258520">that.</span></p><p><span
  m="4259540">So</span> <span m="4259660">you</span> <span m="4259720">might</span>
  <span m="4259900">say,</span> <span m="4260080">OK,</span> <span m="4260290">well,</span>
  <span m="4260410">what's</span> <span m="4260560">the</span> <span m="4260650">next</span>
  <span m="4260950">thing</span> <span m="4261130">we</span> <span m="4261250">could</span>
  <span m="4261370">do</span> <span m="4261490">to</span> <span m="4261580">try</span>
  <span m="4261730">to</span> <span m="4261820">clean</span> <span m="4262030">up</span>
  <span m="4262090">the</span> <span m="4262180">signal</span> <span m="4262480">a</span>
  <span m="4262510">little</span> <span m="4262720">bit</span> <span m="4262840">more?</span>
  <span m="4263130">So</span> <span m="4264190">flash</span> <span m="4264560">backwards</span>
  <span m="4265240">from</span> <span m="4265360">2001</span> <span m="4265990">to</span>
  <span m="4266600">1970</span> <span m="4268510">here</span> <span m="4268750">at</span>
  <span m="4268840">MIT,</span> <span m="4270130">studied</span> <span m="4270520">by--</span>
  <span m="4271210">actually,</span> <span m="4272320">no,</span> <span m="4272410">this</span>
  <span m="4272530">is</span> <span m="4272590">not</span> <span m="4272770">MIT.</span>
  <span m="4273760">This</span> <span m="4273880">is</span> <span m="4273940">somewhere</span>
  <span m="4274150">else,</span> <span m="4274460">sorry.</span> <span m="4276070">But</span>
  <span m="4276220">still</span> <span m="4276440">1970--</span> <span m="4278560">where</span>
  <span m="4278890">they</span> <span m="4279430">used</span> <span m="4279850">a</span>
  <span m="4280420">Markov</span> <span m="4281110">model</span> <span m="4281530">very</span>
  <span m="4281800">similar</span> <span m="4282070">to</span> <span m="4282190">the</span>
  <span m="4282250">Markov</span> <span m="4282640">models</span> <span m="4282940">we</span>
  <span m="4283010">were</span> <span m="4283090">just</span> <span m="4283270">talking</span>
  <span m="4283570">about</span> <span m="4283690">in</span> <span m="4283750">the</span>
  <span m="4283810">previous</span> <span m="4284140">example</span> <span m="4285070">to</span>
  <span m="4285640">model</span> <span m="4286270">what</span> <span m="4287230">a</span>
  <span m="4287530">sequence</span> <span m="4288220">of</span> <span m="4288850">normal</span>
  <span m="4289880">RR</span> <span m="4290410">intervals</span> <span m="4290890">looks</span>
  <span m="4291130">like</span> <span m="4291400">versus</span> <span m="4291700">what</span>
  <span m="4291820">a</span> <span m="4291880">sequence</span> <span m="4292450">of</span>
  <span m="4293320">abnormal,</span> <span m="4294310">for</span> <span m="4294430">example,</span>
  <span m="4294820">AF</span> <span m="4295460">RR</span> <span m="4296030">intervals</span>
  <span m="4296470">looks</span> <span m="4296710">like.</span></p><p><span m="4297370">And</span>
  <span m="4297540">in</span> <span m="4297580">that</span> <span m="4297790">way,</span>
  <span m="4298120">one</span> <span m="4298390">can</span> <span m="4298870">recognize</span>
  <span m="4299590">that,</span> <span m="4300640">for</span> <span m="4300850">any</span>
  <span m="4301120">one</span> <span m="4301420">observation</span> <span m="4302050">of</span>
  <span m="4302140">an</span> <span m="4302260">RR</span> <span m="4302470">interval</span>
  <span m="4302980">might</span> <span m="4303790">not</span> <span m="4304030">by</span>
  <span m="4304210">itself</span> <span m="4304600">be</span> <span m="4304690">perfectly</span>
  <span m="4305080">predictive,</span> <span m="4305540">but</span> <span m="4305650">if</span>
  <span m="4305740">you</span> <span m="4305800">look</span> <span m="4305950">at</span>
  <span m="4306010">sort</span> <span m="4306130">of</span> <span m="4306190">a</span>
  <span m="4306220">sequence</span> <span m="4306670">of</span> <span m="4306790">them</span>
  <span m="4307480">for</span> <span m="4307780">a</span> <span m="4307900">patient</span>
  <span m="4308260">with</span> <span m="4309280">atrial</span> <span m="4309550">fibrillation,</span>
  <span m="4310480">there</span> <span m="4310750">is</span> <span m="4310900">some</span>
  <span m="4311380">common</span> <span m="4312070">pattern</span> <span m="4312610">to</span>
  <span m="4312850">it.</span> <span m="4313420">And</span> <span m="4313570">you</span>
  <span m="4313770">can--</span> <span m="4313920">one</span> <span m="4314050">can</span>
  <span m="4314170">detect</span> <span m="4314425">it</span> <span m="4314680">by</span>
  <span m="4314800">just</span> <span m="4314950">looking</span> <span m="4315190">at</span>
  <span m="4315280">likelihood</span> <span m="4316090">of</span> <span m="4317200">that</span>
  <span m="4317380">sequence</span> <span m="4317860">under</span> <span m="4318130">each</span>
  <span m="4318340">of</span> <span m="4318400">these</span> <span m="4318550">two</span>
  <span m="4318730">different</span> <span m="4319030">models,</span> <span m="4319450">normal</span>
  <span m="4319720">and</span> <span m="4319810">abnormal.</span> <span m="4321230">And</span>
  <span m="4321280">that</span> <span m="4321520">did</span> <span m="4321730">pretty</span>
  <span m="4321970">well--</span> <span m="4322240">even</span> <span m="4322480">better</span>
  <span m="4322840">than</span> <span m="4323710">the</span> <span m="4323770">previous</span>
  <span m="4324070">approaches</span> <span m="4324720">for--</span> <span m="4325310">for</span>
  <span m="4325600">predicting</span> <span m="4325990">atrial</span> <span m="4326290">fibrillation.</span></p><p><span
  m="4328370">This</span> <span m="4328520">is</span> <span m="4328580">the</span>
  <span m="4328640">paper</span> <span m="4328880">I</span> <span m="4328940">wanted</span>
  <span m="4329120">to</span> <span m="4329180">say</span> <span m="4329360">from</span>
  <span m="4331200">MIT.</span> <span m="4331790">Now</span> <span m="4332030">1991,</span>
  <span m="4333620">this</span> <span m="4333800">is</span> <span m="4334040">also</span>
  <span m="4334280">from</span> <span m="4334460">Roger</span> <span m="4334700">Mark's</span>
  <span m="4334970">group.</span> <span m="4335880">Now</span> <span m="4336440">this</span>
  <span m="4336650">is</span> <span m="4336860">a neural</span> <span m="4337070">network</span>
  <span m="4337610">based</span> <span m="4337820">approach,</span> <span m="4338360">where</span>
  <span m="4338930">it</span> <span m="4339080">says,</span> <span m="4339480">OK,</span>
  <span m="4339900">we're</span> <span m="4339920">going</span> <span m="4340070">to</span>
  <span m="4340190">take</span> <span m="4340490">a</span> <span m="4340550">bunch</span>
  <span m="4340790">of</span> <span m="4340880">these</span> <span m="4341120">things.</span>
  <span m="4342120">We're</span> <span m="4342230">going</span> <span m="4342340">to</span>
  <span m="4342410">derive</span> <span m="4342740">a</span> <span m="4342770">bunch</span>
  <span m="4342950">of</span> <span m="4343010">these</span> <span m="4343160">intervals,</span>
  <span m="4344150">and then</span> <span m="4344240">we're</span> <span m="4344330">going</span>
  <span m="4344450">to</span> <span m="4344510">throw</span> <span m="4344780">that</span>
  <span m="4344960">through</span> <span m="4345170">a</span> <span m="4345230">black</span>
  <span m="4345530">box</span> <span m="4345890">supervised</span> <span m="4346430">machine</span>
  <span m="4346700">learning</span> <span m="4347000">algorithm</span> <span m="4347390">to</span>
  <span m="4347480">predict</span> <span m="4347780">whether</span> <span m="4347920">a</span>
  <span m="4347960">patient</span> <span m="4348260">has</span> <span m="4348530">AF</span>
  <span m="4348830">or</span> <span m="4348920">not.</span></p><p><span m="4350240">So</span>
  <span m="4350840">these</span> <span m="4351220">are</span> <span m="4351420">very--</span>
  <span m="4352220">first</span> <span m="4352490">of</span> <span m="4352580">all,</span>
  <span m="4353390">there are</span> <span m="4353720">some</span> <span m="4353870">simple</span>
  <span m="4354200">approaches</span> <span m="4354650">here</span> <span m="4354890">that</span>
  <span m="4355040">work</span> <span m="4355310">reasonably</span> <span m="4355730">well.</span>
  <span m="4356540">Using</span> <span m="4356870">neural</span> <span m="4357070">networks</span>
  <span m="4357500">in</span> <span m="4357620">this</span> <span m="4357770">domain</span>
  <span m="4358430">is</span> <span m="4358610">not</span> <span m="4359120">a</span>
  <span m="4359180">new</span> <span m="4359450">thing,</span> <span m="4362280">but</span>
  <span m="4362540">where</span> <span m="4362870">are</span> <span m="4363080">we</span>
  <span m="4363290">as</span> <span m="4363500">a</span> <span m="4363560">field?</span>
  <span m="4364140">So</span> <span m="4364850">as</span> <span m="4365000">I</span>
  <span m="4365060">mentioned,</span> <span m="4365390">there</span> <span m="4365480">was</span>
  <span m="4365600">this</span> <span m="4365690">competition</span> <span m="4366170">last</span>
  <span m="4366470">year,</span> <span m="4366920">and</span> <span m="4367370">what</span>
  <span m="4367520">I'm</span> <span m="4367610">showing</span> <span m="4367940">you</span>
  <span m="4368060">here--</span> <span m="4368330">the</span> <span m="4368450">citation</span>
  <span m="4368960">is</span> <span m="4369080">from</span> <span m="4369230">one</span>
  <span m="4369380">of</span> <span m="4369470">the</span> <span m="4369560">winning</span>
  <span m="4369830">approaches.</span></p><p><span m="4370470">And</span> <span m="4370570">this</span>
  <span m="4370580">winning</span> <span m="4370820">approach</span> <span m="4371180">really</span>
  <span m="4371420">brings</span> <span m="4371750">the</span> <span m="4371870">two</span>
  <span m="4372260">paradigms</span> <span m="4372830">together.</span> <span m="4373910">It</span>
  <span m="4374630">extracts</span> <span m="4375380">a</span> <span m="4375410">large</span>
  <span m="4375710">number</span> <span m="4375890">of</span> <span m="4375980">expert</span>
  <span m="4376400">derived</span> <span m="4376670">features--</span> <span m="4377600">so</span>
  <span m="4377960">shown</span> <span m="4379040">here.</span> <span m="4379810">And</span>
  <span m="4379910">these</span> <span m="4380030">are</span> <span m="4380090">exactly</span>
  <span m="4380450">the</span> <span m="4380510">types</span> <span m="4380750">of</span>
  <span m="4380810">things</span> <span m="4381050">you</span> <span m="4381140">might</span>
  <span m="4381290">think,</span> <span m="4381800">like</span> <span m="4383240">proportion,</span>
  <span m="4385100">median</span> <span m="4385790">RR</span> <span m="4386390">interval</span>
  <span m="4387020">of</span> <span m="4387200">regular</span> <span m="4387620">rhythms,</span>
  <span m="4389090">max</span> <span m="4389710">RR</span> <span m="4390260">irregularity</span>
  <span m="4390950">measure.</span> <span m="4391550">And</span> <span m="4391650">there's</span>
  <span m="4391760">just</span> <span m="4391910">a</span> <span m="4391970">whole</span>
  <span m="4392360">range</span> <span m="4392780">of</span> <span m="4392870">different</span>
  <span m="4393200">things</span> <span m="4393500">that</span> <span m="4393590">you</span>
  <span m="4393680">can</span> <span m="4393770">imagine</span> <span m="4394130">manually</span>
  <span m="4394610">deriving</span> <span m="4395030">from</span> <span m="4395210">the</span>
  <span m="4395300">data.</span> <span m="4396160">And</span> <span m="4396290">you</span>
  <span m="4396380">throw</span> <span m="4396800">all</span> <span m="4396980">of</span>
  <span m="4397070">these</span> <span m="4397250">features</span> <span m="4397910">into</span>
  <span m="4398690">a</span> <span m="4400220">machine</span> <span m="4400550">learning</span>
  <span m="4400820">algorithm,</span> <span m="4401840">maybe a</span> <span m="4402140">random</span>
  <span m="4402410">forest,</span> <span m="4402860">maybe</span> <span m="4403140">a
  neural</span> <span m="4403190">network,</span> <span m="4403610">doesn't</span>
  <span m="4403850">matter.</span> <span m="4405040">And</span> <span m="4405260">what</span>
  <span m="4405410">you</span> <span m="4405530">get</span> <span m="4405710">out</span>
  <span m="4405890">is</span> <span m="4406010">a</span> <span m="4406040">slightly</span>
  <span m="4406430">better</span> <span m="4406730">algorithm</span> <span m="4407180">than</span>
  <span m="4407370">what if</span> <span m="4407480">you</span> <span m="4407600">had</span>
  <span m="4407720">just</span> <span m="4408260">come</span> <span m="4408470">up</span>
  <span m="4408530">with</span> <span m="4408650">a</span> <span m="4408680">simple</span>
  <span m="4408980">rule</span> <span m="4409250">on</span> <span m="4409340">your</span>
  <span m="4409460">own.</span> <span m="4410510">That</span> <span m="4410990">was</span>
  <span m="4411140">the</span> <span m="4411230">winning</span> <span m="4411440">algorithm</span>
  <span m="4411800">then.</span></p><p><span m="4413470">And</span> <span m="4413940">in</span>
  <span m="4414090">the</span> <span m="4414150">summary</span> <span m="4414630">paper,</span>
  <span m="4415450">they</span> <span m="4415620">conjectured</span> <span m="4416310">that,</span>
  <span m="4416490">well,</span> <span m="4416610">maybe</span> <span m="4416970">it's</span>
  <span m="4417240">the</span> <span m="4417360">case</span> <span m="4417780">that</span>
  <span m="4418890">they</span> <span m="4419130">were--</span> <span m="4419460">they'd</span>
  <span m="4419640">expected</span> <span m="4420090">that</span> <span m="4420210">convolutional</span>
  <span m="4420690">neural</span> <span m="4420850">networks</span> <span m="4421440">would</span>
  <span m="4421620">win.</span> <span m="4422550">And</span> <span m="4422670">they</span>
  <span m="4422760">were</span> <span m="4422880">surprised</span> <span m="4423420">that</span>
  <span m="4423660">none</span> <span m="4424020">of</span> <span m="4424140">the</span>
  <span m="4424230">winning</span> <span m="4424470">solutions</span> <span m="4424860">involved</span>
  <span m="4425190">convolution</span> <span m="4425710">neural</span> <span m="4425850">networks.</span>
  <span m="4427070">And</span> <span m="4427170">they</span> <span m="4427260">conjectured</span>
  <span m="4427710">that</span> <span m="4427830">may</span> <span m="4428030">be</span>
  <span m="4428160">the</span> <span m="4428250">reason</span> <span m="4428550">why</span>
  <span m="4428790">is</span> <span m="4428880">because</span> <span m="4430020">maybe</span>
  <span m="4430380">with</span> <span m="4430590">these</span> <span m="4430820">8,000</span>
  <span m="4431460">patients</span> <span m="4431880">that</span> <span m="4431970">they</span>
  <span m="4432060">had</span> <span m="4432170">[INAUDIBLE]</span> <span m="4432490">that</span>
  <span m="4432630">just</span> <span m="4432780">wasn't</span> <span m="4433110">enough</span>
  <span m="4433410">to</span> <span m="4433530">give</span> <span m="4433650">the</span>
  <span m="4433740">more</span> <span m="4433890">complex</span> <span m="4434340">models</span>
  <span m="4434880">advantage.</span></p><p><span m="4436590">So</span> <span m="4436890">flip</span>
  <span m="4437130">forward</span> <span m="4437610">now</span> <span m="4438030">to</span>
  <span m="4438480">this</span> <span m="4438750">year</span> <span m="4439800">and</span>
  <span m="4439950">the</span> <span m="4440040">article</span> <span m="4440370">that</span>
  <span m="4440490">you</span> <span m="4440610">read</span> <span m="4441060">in</span>
  <span m="4441660">your</span> <span m="4441780">readings</span> <span m="4443790">in</span>
  <span m="4444060"><i>Nature</i></span> <span m="4444330"><i>Medicine,</i></span>
  <span m="4445840">where</span> <span m="4445920">the</span> <span m="4446010">Stanford</span>
  <span m="4446520">group</span> <span m="4446760">now</span> <span m="4447030">showed</span>
  <span m="4447420">how</span> <span m="4447750">a</span> <span m="4447870">convolutional</span>
  <span m="4448610">neural</span> <span m="4448760">network</span> <span m="4449400">approach,</span>
  <span m="4450330">which</span> <span m="4450540">is,</span> <span m="4452040">in</span>
  <span m="4452130">many</span> <span m="4452370">ways,</span> <span m="4452580">extremely</span>
  <span m="4453150">naive--</span> <span m="4453570">all</span> <span m="4453690">it</span>
  <span m="4453750">does</span> <span m="4453960">is</span> <span m="4454050">it</span>
  <span m="4454110">takes</span> <span m="4454470">the</span> <span m="4454590">sequence</span>
  <span m="4455610">data</span> <span m="4456030">in.</span> <span m="4457870">It</span>
  <span m="4458130">makes</span> <span m="4458490">no</span> <span m="4458730">attempt</span>
  <span m="4459120">at</span> <span m="4459210">trying</span> <span m="4459480">to</span>
  <span m="4459570">understand</span> <span m="4460200">the</span> <span m="4460290">underlying</span>
  <span m="4460710">physiology,</span> <span m="4461820">and</span> <span m="4461940">just</span>
  <span m="4462090">predicts</span> <span m="4462840">from</span> <span m="4463110">that--</span>
  <span m="4463800">can</span> <span m="4464040">do</span> <span m="4464190">really,</span>
  <span m="4464710">really</span> <span m="4464910">well.</span></p><p><span m="4466180">And</span>
  <span m="4466200">so</span> <span m="4466320">there</span> <span m="4466410">are</span>
  <span m="4466440">couple</span> <span m="4466620">of</span> <span m="4466710">differences</span>
  <span m="4467230">that</span> <span m="4467290">I</span> <span m="4467340">want</span>
  <span m="4467490">to</span> <span m="4467550">emphasize</span> <span m="4468180">to</span>
  <span m="4468330">the</span> <span m="4468390">previous</span> <span m="4468750">work.</span>
  <span m="4469590">First,</span> <span m="4469980">the</span> <span m="4470100">censor</span>
  <span m="4470610">is</span> <span m="4470730">different.</span> <span m="4471360">Whereas</span>
  <span m="4471750">the</span> <span m="4471840">previous</span> <span m="4472260">work</span>
  <span m="4472590">used</span> <span m="4473070">this</span> <span m="4473280">alive</span>
  <span m="4473730">core</span> <span m="4474120">censor,</span> <span m="4475580">in</span>
  <span m="4475710">this</span> <span m="4476250">paper</span> <span m="4476580">from</span>
  <span m="4476760">Stanford,</span> <span m="4477300">they're</span> <span m="4477420">using</span>
  <span m="4478320">a</span> <span m="4478410">different</span> <span m="4478800">censor</span>
  <span m="4479190">called</span> <span m="4479430">the</span> <span m="4479520">Zio</span>
  <span m="4479850">patch,</span> <span m="4480660">which</span> <span m="4480870">is</span>
  <span m="4481050">attached</span> <span m="4481500">to</span> <span m="4481740">the</span>
  <span m="4481860">human</span> <span m="4482160">body</span> <span m="4483030">and</span>
  <span m="4483480">conceivably</span> <span m="4484110">much</span> <span m="4484380">less</span>
  <span m="4484560">noisy.</span> <span m="4485580">So</span> <span m="4485670">that's</span>
  <span m="4485880">one</span> <span m="4486090">big</span> <span m="4486240">difference.</span></p><p><span
  m="4488050">The</span> <span m="4488150">second</span> <span m="4488340">big</span>
  <span m="4488490">difference</span> <span m="4488820">is</span> <span m="4488910">that</span>
  <span m="4489000">there's</span> <span m="4489180">dramatically</span> <span m="4489810">more</span>
  <span m="4489990">data.</span> <span m="4490770">Instead</span> <span m="4491010">of</span>
  <span m="4491100">8,000</span> <span m="4491640">patients</span> <span m="4491940">to</span>
  <span m="4492030">train</span> <span m="4492270">from,</span> <span m="4492510">now</span>
  <span m="4492690">they</span> <span m="4492810">have</span> <span m="4493050">over</span>
  <span m="4493260">90,000</span> <span m="4494250">records</span> <span m="4494790">from</span>
  <span m="4495000">50,000</span> <span m="4495600">different</span> <span m="4495870">patients</span>
  <span m="4496290">to</span> <span m="4496380">train</span> <span m="4496620">from.</span>
  <span m="4498060">The</span> <span m="4498150">third</span> <span m="4498510">major</span>
  <span m="4498810">difference</span> <span m="4499100">is</span> <span m="4499260">that</span>
  <span m="4499380">now,</span> <span m="4499740">rather</span> <span m="4500010">than</span>
  <span m="4500160">just</span> <span m="4500370">trying</span> <span m="4500550">to</span>
  <span m="4500640">classify</span> <span m="4501300">into</span> <span m="4501510">four</span>
  <span m="4501870">categories--</span> <span m="4502740">normal,</span> <span m="4503820">abnormal,</span>
  <span m="4504930">other,</span> <span m="4505560">or</span> <span m="4505740">noisy--</span>
  <span m="4506730">now</span> <span m="4507060">we're</span> <span m="4507150">going</span>
  <span m="4507330">to</span> <span m="4507420">try</span> <span m="4507540">to</span>
  <span m="4507630">classify</span> <span m="4508140">into</span> <span m="4508320">14</span>
  <span m="4509010">different</span> <span m="4509310">categories.</span> <span m="4509880">We're,</span>
  <span m="4510060">in</span> <span m="4510200">essence,</span> <span m="4510450">breaking</span>
  <span m="4511020">apart</span> <span m="4511450">that</span> <span m="4511710">other</span>
  <span m="4512040">class</span> <span m="4512850">into</span> <span m="4513090">much</span>
  <span m="4513540">finer</span> <span m="4513990">grain</span> <span m="4514320">detail</span>
  <span m="4514920">of</span> <span m="4515010">different</span> <span m="4515340">types</span>
  <span m="4515610">of</span> <span m="4515730">abnormal</span> <span m="4516210">rhythms.</span></p><p><span
  m="4517780">And</span> <span m="4517830">so</span> <span m="4518130">here</span>
  <span m="4518430">are</span> <span m="4518490">some</span> <span m="4518730">of</span>
  <span m="4518790">those</span> <span m="4518970">other</span> <span m="4519210">abnormal</span>
  <span m="4519570">rhythms,</span> <span m="4520110">things</span> <span m="4520500">like</span>
  <span m="4521130">complete</span> <span m="4521610">heart</span> <span m="4521910">block,</span>
  <span m="4528140">and</span> <span m="4528290">a</span> <span m="4528350">bunch</span>
  <span m="4528500">of</span> <span m="4528560">other</span> <span m="4528680">names</span>
  <span m="4528960">I</span> <span m="4529040">can't</span> <span m="4529250">pronounce.</span>
  <span m="4531650">And</span> <span m="4532520">from</span> <span m="4532760">each</span>
  <span m="4532970">one</span> <span m="4533150">of</span> <span m="4533270">these,</span>
  <span m="4533510">they</span> <span m="4533600">gathered</span> <span m="4533990">a</span>
  <span m="4534020">lot</span> <span m="4534170">of</span> <span m="4534260">data.</span>
  <span m="4534560">And</span> <span m="4534650">that</span> <span m="4534740">actually</span>
  <span m="4534980">did--</span> <span m="4535430">so</span> <span m="4535610">it's</span>
  <span m="4535820">not</span> <span m="4536000">described</span> <span m="4536420">in</span>
  <span m="4536480">the</span> <span m="4536540">paper,</span> <span m="4536870">but</span>
  <span m="4536990">I've</span> <span m="4537170">talked</span> <span m="4537440">to</span>
  <span m="4537530">the</span> <span m="4537620">authors,</span> <span m="4537980">and</span>
  <span m="4538070">they</span> <span m="4538160">did--</span> <span m="4538370">they</span>
  <span m="4538490">gathered</span> <span m="4538760">this</span> <span m="4538910">data</span>
  <span m="4539140">in</span> <span m="4539210">a</span> <span m="4539240">very</span>
  <span m="4539450">interesting</span> <span m="4539780">way.</span></p><p><span m="4540690">So</span>
  <span m="4540720">they</span> <span m="4540950">sort of--</span> <span m="4541250">they</span>
  <span m="4541340">did</span> <span m="4541490">their</span> <span m="4541640">training</span>
  <span m="4542060">iteratively.</span> <span m="4542720">They</span> <span m="4542840">looked</span>
  <span m="4543020">to</span> <span m="4543140">see</span> <span m="4543410">where</span>
  <span m="4543590">their</span> <span m="4543770">errors</span> <span m="4544190">were,</span>
  <span m="4544460">and</span> <span m="4544550">then</span> <span m="4544670">they</span>
  <span m="4544760">went</span> <span m="4544970">and</span> <span m="4545060">gathered</span>
  <span m="4545390">more</span> <span m="4545660">data</span> <span m="4545960">from</span>
  <span m="4546110">patients</span> <span m="4546560">with</span> <span m="4546740">that</span>
  <span m="4546920">subcategory.</span> <span m="4548180">So</span> <span m="4549440">many</span>
  <span m="4549890">of</span> <span m="4550010">these</span> <span m="4550400">other</span>
  <span m="4551090">categories</span> <span m="4551930">are</span> <span m="4552590">very</span>
  <span m="4553190">under--</span> <span m="4553520">might</span> <span m="4553680">be</span>
  <span m="4553880">underrepresented</span> <span m="4554630">in</span> <span m="4554720">the</span>
  <span m="4554780">general</span> <span m="4555020">population,</span> <span m="4555620">but</span>
  <span m="4555710">they</span> <span m="4555830">actually</span> <span m="4556100">gather</span>
  <span m="4556460">a</span> <span m="4556520">lot</span> <span m="4556730">of</span>
  <span m="4556790">patients</span> <span m="4557240">of</span> <span m="4557360">that</span>
  <span m="4557480">type</span> <span m="4557810">in</span> <span m="4557930">their</span>
  <span m="4558020">data</span> <span m="4558220">set</span> <span m="4558440">for</span>
  <span m="4558590">training</span> <span m="4558860">purposes.</span> <span m="4560520">And</span>
  <span m="4560540">so</span> <span m="4561230">I</span> <span m="4561290">think</span>
  <span m="4561470">those</span> <span m="4561770">three</span> <span m="4562070">things</span>
  <span m="4562460">ended</span> <span m="4562640">up</span> <span m="4562700">making</span>
  <span m="4562970">a</span> <span m="4563030">very</span> <span m="4563240">big</span>
  <span m="4563420">difference.</span></p><p><span m="4565320">So</span> <span m="4565430">what</span>
  <span m="4565640">is</span> <span m="4565880">their</span> <span m="4566090">convolutional</span>
  <span m="4566640">network?</span> <span m="4567050">Well,</span> <span m="4568100">first</span>
  <span m="4568430">of</span> <span m="4568520">all,</span> <span m="4568730">it's</span>
  <span m="4568940">a</span> <span m="4569090">1-D</span> <span m="4570020">signal.</span>
  <span m="4570750">So</span> <span m="4570830">it's</span> <span m="4570950">a</span>
  <span m="4570980">little</span> <span m="4571160">bit</span> <span m="4571250">different</span>
  <span m="4571550">from</span> <span m="4571670">the</span> <span m="4571730">con
  nets</span> <span m="4572180">you</span> <span m="4572240">typically</span> <span
  m="4572600">see</span> <span m="4572750">in</span> <span m="4572840">computer</span>
  <span m="4573110">vision,</span> <span m="4573380">and</span> <span m="4573470">I'll</span>
  <span m="4573560">show</span> <span m="4573770">you</span> <span m="4574070">an</span>
  <span m="4574220">illustration</span> <span m="4574640">of</span> <span m="4574700">that</span>
  <span m="4574790">in</span> <span m="4574850">the</span> <span m="4574910">next</span>
  <span m="4575120">slide.</span> <span m="4576080">It's</span> <span m="4576200">a</span>
  <span m="4576230">very</span> <span m="4576470">deep</span> <span m="4576920">model.</span>
  <span m="4577430">So it's</span> <span m="4577650">34</span> <span m="4578420">layers.</span></p><p><span
  m="4580100">So</span> <span m="4580640">the</span> <span m="4580790">input</span>
  <span m="4581120">comes</span> <span m="4581390">in</span> <span m="4581510">on</span>
  <span m="4581570">the</span> <span m="4581630">very</span> <span m="4581750">top</span>
  <span m="4582050">in</span> <span m="4582140">this</span> <span m="4582260">picture.</span>
  <span m="4583010">It's</span> <span m="4583160">passed</span> <span m="4583550">through</span>
  <span m="4583790">a</span> <span m="4583820">number</span> <span m="4584180">of</span>
  <span m="4586340">layers.</span> <span m="4586730">Each</span> <span m="4586910">layer</span>
  <span m="4587180">consists</span> <span m="4587900">of</span> <span m="4588530">convolution</span>
  <span m="4589790">followed</span> <span m="4590210">by</span> <span m="4590780">rectified</span>
  <span m="4591260">linear</span> <span m="4591530">units,</span> <span m="4592190">and</span>
  <span m="4592670">there</span> <span m="4592940">is</span> <span m="4593180">sub</span>
  <span m="4593600">sampling</span> <span m="4594260">at</span> <span m="4594350">every</span>
  <span m="4594650">other</span> <span m="4594860">layer</span> <span m="4595280">so</span>
  <span m="4595520">that</span> <span m="4595670">you</span> <span m="4595790">go</span>
  <span m="4596060">from</span> <span m="4596630">a</span> <span m="4596690">very</span>
  <span m="4596990">wide</span> <span m="4597500">signal--</span> <span m="4598010">so
  a</span> <span m="4598280">very</span> <span m="4598510">long--</span> <span m="4599780">I</span>
  <span m="4599870">can't</span> <span m="4600030">remember</span> <span m="4600200">how</span>
  <span m="4600440">long--</span> <span m="4600770">1</span> <span m="4601040">second</span>
  <span m="4601580">long</span> <span m="4601820">signal</span> <span m="4602890">summarized</span>
  <span m="4603500">down</span> <span m="4603830">into</span> <span m="4605150">sort
  of</span> <span m="4605460">much--</span> <span m="4605720">just</span> <span m="4606050">many</span>
  <span m="4606380">smaller</span> <span m="4606740">number</span> <span m="4606920">of</span>
  <span m="4607010">dimensions,</span> <span m="4607610">which</span> <span m="4607790">you</span>
  <span m="4607910">then</span> <span m="4608090">have</span> <span m="4608220">a</span>
  <span m="4608270">sort</span> <span m="4608450">of</span> <span m="4608510">fully</span>
  <span m="4608750">connected</span> <span m="4609080">layer</span> <span m="4609290">at
  the</span> <span m="4609380">bottom</span> <span m="4609680">to</span> <span m="4609830">do</span>
  <span m="4610010">for</span> <span m="4610130">your</span> <span m="4610250">predictions.</span>
  <span m="4612770">And</span> <span m="4612950">then</span> <span m="4613130">they</span>
  <span m="4613280">also</span> <span m="4613520">have</span> <span m="4613670">these</span>
  <span m="4613940">shortcut</span> <span m="4614630">connections,</span> <span m="4615590">which</span>
  <span m="4615830">allow</span> <span m="4616130">you</span> <span m="4616220">to</span>
  <span m="4616310">pass</span> <span m="4616730">information</span> <span m="4617390">from</span>
  <span m="4617810">earlier</span> <span m="4618320">layers</span> <span m="4618770">down</span>
  <span m="4619100">to</span> <span m="4619190">the</span> <span m="4619280">very</span>
  <span m="4619520">end</span> <span m="4619850">of</span> <span m="4619940">the</span>
  <span m="4620030">network,</span> <span m="4620630">or</span> <span m="4620850">even</span>
  <span m="4621140">into</span> <span m="4621440">intermediate</span> <span m="4621950">layers.</span>
  <span m="4622710">And</span> <span m="4622810">for</span> <span m="4622910">those</span>
  <span m="4622970">of</span> <span m="4623060">you</span> <span m="4623150">who</span>
  <span m="4623270">are</span> <span m="4623330">familiar</span> <span m="4623720">with</span>
  <span m="4623870">residual</span> <span m="4624380">networks,</span> <span m="4624770">it's</span>
  <span m="4624890">the</span> <span m="4624980">same</span> <span m="4625250">idea.</span></p><p><span
  m="4626850">So</span> <span m="4626870">what</span> <span m="4627020">is</span>
  <span m="4627200">a</span> <span m="4627260">1D</span> <span m="4627530">convolution?</span>
  <span m="4628340">Well,</span> <span m="4628430">it</span> <span m="4628490">looks</span>
  <span m="4628670">a</span> <span m="4628700">little</span> <span m="4628850">bit</span>
  <span m="4628970">like</span> <span m="4629120">this.</span> <span m="4630270">So</span>
  <span m="4632090">this</span> <span m="4632270">is</span> <span m="4632360">the</span>
  <span m="4632450">signal.</span> <span m="4632960">I'm</span> <span m="4633110">going</span>
  <span m="4633350">to</span> <span m="4633500">just</span> <span m="4633710">approximate</span>
  <span m="4634090">it</span> <span m="4634340">by</span> <span m="4634490">a</span>
  <span m="4634520">bunch</span> <span m="4634670">of</span> <span m="4634760">1's</span>
  <span m="4635000">and</span> <span m="4635090">0's.</span> <span m="4635570">I'll</span>
  <span m="4635660">say</span> <span m="4635900">this</span> <span m="4636050">is</span>
  <span m="4636170">a</span> <span m="4636230">1.</span> <span m="4636560">This</span>
  <span m="4636740">is</span> <span m="4636830">a</span> <span m="4636900">0.</span>
  <span m="4637360">This is a</span> <span m="4637770">1,</span> <span m="4638180">1,</span>
  <span m="4638360">so on.</span></p><p><span m="4641620">A</span> <span m="4641980">convolutional</span>
  <span m="4642590">network</span> <span m="4642910">has</span> <span m="4643210">a</span>
  <span m="4643330">filter</span> <span m="4643990">associated</span> <span m="4644410">with</span>
  <span m="4644590">it.</span> <span m="4645280">That</span> <span m="4645460">filter</span>
  <span m="4646060">is</span> <span m="4646240">then</span> <span m="4646450">applied</span>
  <span m="4646810">in</span> <span m="4646900">a</span> <span m="4646960">1D</span>
  <span m="4647680">model.</span> <span m="4648070">It's</span> <span m="4648220">applied</span>
  <span m="4648670">in</span> <span m="4648820">a</span> <span m="4648880">linear</span>
  <span m="4649240">fashion.</span> <span m="4649630">It's</span> <span m="4649750">just</span>
  <span m="4649880">taken</span> <span m="4650050">a</span> <span m="4650170">dot</span>
  <span m="4650470">product</span> <span m="4650890">with</span> <span m="4650950">the</span>
  <span m="4651040">filter's</span> <span m="4651640">values,</span> <span m="4652240">with</span>
  <span m="4652570">the</span> <span m="4652690">values</span> <span m="4653140">of</span>
  <span m="4653230">the</span> <span m="4653320">signal</span> <span m="4653770">at</span>
  <span m="4653860">each</span> <span m="4653980">point</span> <span m="4654160">in</span>
  <span m="4654250">time.</span></p><p><span m="4655150">So</span> <span m="4655580">it</span>
  <span m="4655680">looks</span> <span m="4655870">a</span> <span m="4655900">little</span>
  <span m="4656050">bit</span> <span m="4656140">like</span> <span m="4656320">this,</span>
  <span m="4658130">and</span> <span m="4658400">this</span> <span m="4658580">is</span>
  <span m="4658640">what</span> <span m="4658760">you</span> <span m="4658850">get</span>
  <span m="4659000">out.</span> <span m="4659450">So</span> <span m="4659600">this</span>
  <span m="4659810">is</span> <span m="4660440">the</span> <span m="4660620">convolution</span>
  <span m="4661250">of</span> <span m="4661340">a</span> <span m="4661400">single</span>
  <span m="4661850">filter</span> <span m="4662330">with</span> <span m="4662600">the</span>
  <span m="4662780">whole</span> <span m="4663260">signal.</span> <span m="4664760">And</span>
  <span m="4665210">the</span> <span m="4665330">computation</span> <span m="4665940">I</span>
  <span m="4666040">did</span> <span m="4666050">there--</span> <span m="4666290">so</span>
  <span m="4666440">for</span> <span m="4666530">example,</span> <span m="4667140">this</span>
  <span m="4667250">first</span> <span m="4667550">number</span> <span m="4668210">came</span>
  <span m="4668510">from</span> <span m="4668660">taking</span> <span m="4668930">the</span>
  <span m="4669020">dot</span> <span m="4669320">product</span> <span m="4669860">of</span>
  <span m="4670100">the</span> <span m="4670220">first</span> <span m="4670610">three</span>
  <span m="4670850">numbers--</span> <span m="4671360">1,</span> <span m="4671700">0,</span>
  <span m="4672040">1--</span> <span m="4672620">with</span> <span m="4672800">the</span>
  <span m="4672890">filter.</span> <span m="4673370">So</span> <span m="4673580">it's</span>
  <span m="4674870">1</span> <span m="4675290">times</span> <span m="4675680">2</span>
  <span m="4676430">plus</span> <span m="4676820">3</span> <span m="4677120">times</span>
  <span m="4677420">0</span> <span m="4677810">plus</span> <span m="4678080">1</span>
  <span m="4678410">times</span> <span m="4678740">1,</span> <span m="4679280">which</span>
  <span m="4679610">is</span> <span m="4680090">3.</span></p><p><span m="4681780">And</span>
  <span m="4681800">so</span> <span m="4681920">each</span> <span m="4682100">of</span>
  <span m="4682190">the</span> <span m="4682280">subsequent</span> <span m="4682700">numbers</span>
  <span m="4683090">was</span> <span m="4683200">computed</span> <span m="4683500">in</span>
  <span m="4683570">the</span> <span m="4683630">same</span> <span m="4683870">way.</span>
  <span m="4684900">And</span> <span m="4686450">I</span> <span m="4686780">usually</span>
  <span m="4687260">have</span> <span m="4687590">you</span> <span m="4687770">figure</span>
  <span m="4688070">out</span> <span m="4688220">what</span> <span m="4688370">this</span>
  <span m="4688520">last</span> <span m="4688760">one</span> <span m="4688910">is,</span>
  <span m="4689060">but</span> <span m="4689150">I'll</span> <span m="4689210">leave</span>
  <span m="4689390">that</span> <span m="4689510">for</span> <span m="4689630">you</span>
  <span m="4689690">to</span> <span m="4689780">do</span> <span m="4689930">at</span>
  <span m="4690050">home.</span> <span m="4692440">And</span> <span m="4692570">that's</span>
  <span m="4692750">what</span> <span m="4692870">a</span> <span m="4692930">1D</span>
  <span m="4693140">convolution</span> <span m="4693860">is.</span> <span m="4694190">And</span>
  <span m="4694400">so</span> <span m="4694580">they</span> <span m="4694700">have--</span>
  <span m="4694880">they</span> <span m="4695030">do</span> <span m="4695210">this</span>
  <span m="4695390">for</span> <span m="4695540">lots</span> <span m="4695810">of</span>
  <span m="4695900">different</span> <span m="4696200">filters.</span> <span m="4696680">Each</span>
  <span m="4696860">of</span> <span m="4696920">those</span> <span m="4697130">filters</span>
  <span m="4697760">might</span> <span m="4697940">be</span> <span m="4698090">of</span>
  <span m="4698150">varying</span> <span m="4698630">lengths,</span> <span m="4699200">and</span>
  <span m="4699290">each</span> <span m="4699470">of</span> <span m="4699560">those</span>
  <span m="4699890">will</span> <span m="4700010">detect</span> <span m="4700460">different</span>
  <span m="4700790">types</span> <span m="4701030">of</span> <span m="4701120">signal</span>
  <span m="4701480">patterns.</span></p><p><span m="4703040">And</span> <span m="4703190">in</span>
  <span m="4703280">this</span> <span m="4703460">way,</span> <span m="4703700">after</span>
  <span m="4704300">having</span> <span m="4704630">many</span> <span m="4704900">layers</span>
  <span m="4705380">of</span> <span m="4705470">these,</span> <span m="4705800">one</span>
  <span m="4706130">can,</span> <span m="4707120">in</span> <span m="4707240">an</span>
  <span m="4707390">automatic</span> <span m="4707870">fashion,</span> <span m="4708320">extract</span>
  <span m="4708770">many</span> <span m="4709010">of</span> <span m="4709100">the</span>
  <span m="4709190">same</span> <span m="4709430">types</span> <span m="4709790">of</span>
  <span m="4709880">signals</span> <span m="4710300">used</span> <span m="4710600">in</span>
  <span m="4710660">that</span> <span m="4710780">earlier</span> <span m="4711080">work,</span>
  <span m="4711320">but</span> <span m="4711440">also</span> <span m="4711680">be</span>
  <span m="4711800">much</span> <span m="4711980">more</span> <span m="4712100">flexible</span>
  <span m="4712490">to</span> <span m="4712550">detect</span> <span m="4712820">some</span>
  <span m="4712970">new</span> <span m="4713090">ones,</span> <span m="4713300">as</span>
  <span m="4713420">well.</span> <span m="4714420">Hold</span> <span m="4714620">your</span>
  <span m="4714710">question,</span> <span m="4715110">because</span> <span m="4715280">I</span>
  <span m="4715340">need</span> <span m="4715520">to</span> <span m="4715620">wrap</span>
  <span m="4715850">up.</span></p><p><span m="4717120">So</span> <span m="4717690">in</span>
  <span m="4717780">the</span> <span m="4717870">paper</span> <span m="4718110">that</span>
  <span m="4718230">you</span> <span m="4718320">read,</span> <span m="4718560">they</span>
  <span m="4718710">talked</span> <span m="4719040">about</span> <span m="4719730">how</span>
  <span m="4720060">they</span> <span m="4720210">evaluated</span> <span m="4720660">this.</span>
  <span m="4721950">And</span> <span m="4722600">so</span> <span m="4722700">I'm</span>
  <span m="4722790">not</span> <span m="4722940">going</span> <span m="4723060">to</span>
  <span m="4723120">go</span> <span m="4723210">into</span> <span m="4723390">much</span>
  <span m="4723570">depth</span> <span m="4723800">in</span> <span m="4723870">it</span>
  <span m="4723960">now.</span> <span m="4724110">I</span> <span m="4724170">just</span>
  <span m="4724290">want</span> <span m="4724410">to</span> <span m="4724470">point</span>
  <span m="4724800">out</span> <span m="4725430">two</span> <span m="4725670">different</span>
  <span m="4725970">metrics</span> <span m="4726330">that</span> <span m="4726420">they</span>
  <span m="4726540">used.</span></p><p><span m="4727320">So</span> <span m="4727620">the</span>
  <span m="4727740">first</span> <span m="4728040">metric</span> <span m="4728340">they</span>
  <span m="4728460">used</span> <span m="4728760">was</span> <span m="4728910">what</span>
  <span m="4729060">they</span> <span m="4729180">called</span> <span m="4729690">a</span>
  <span m="4730200">sequential</span> <span m="4731490">error</span> <span m="4731730">metric.</span>
  <span m="4732690">What</span> <span m="4732900">that</span> <span m="4733110">looked</span>
  <span m="4733410">at</span> <span m="4733620">is</span> <span m="4734190">you</span>
  <span m="4734310">had</span> <span m="4734460">this</span> <span m="4734640">very</span>
  <span m="4735030">long</span> <span m="4735390">sequence</span> <span m="4735990">for</span>
  <span m="4736170">each</span> <span m="4736350">patient,</span> <span m="4737400">and</span>
  <span m="4738300">they</span> <span m="4738570">labeled</span> <span m="4739890">different</span>
  <span m="4740340">one</span> <span m="4740670">second</span> <span m="4741150">intervals</span>
  <span m="4741630">of</span> <span m="4741690">that</span> <span m="4741870">sequence</span>
  <span m="4742350">into</span> <span m="4742650">abnormal,</span> <span m="4743310">normal,</span>
  <span m="4743880">and</span> <span m="4744000">so</span> <span m="4744240">on.</span>
  <span m="4745690">So</span> <span m="4745840">you</span> <span m="4745930">could</span>
  <span m="4746080">ask,</span> <span m="4746530">how</span> <span m="4746770">good</span>
  <span m="4746980">are</span> <span m="4747040">we</span> <span m="4747220">at</span>
  <span m="4747340">labeling</span> <span m="4747850">each</span> <span m="4748090">of</span>
  <span m="4748150">the</span> <span m="4748240">different</span> <span m="4748480">points</span>
  <span m="4748780">along</span> <span m="4748990">the</span> <span m="4749080">sequence?</span>
  <span m="4749600">And</span> <span m="4749700">that's</span> <span m="4749800">the</span>
  <span m="4749860">sequence</span> <span m="4750320">metric.</span></p><p><span m="4751720">The</span>
  <span m="4751840">different--</span> <span m="4752260">the</span> <span m="4752380">second</span>
  <span m="4752680">metric</span> <span m="4753070">is</span> <span m="4753520">the</span>
  <span m="4753640">set</span> <span m="4754090">metric,</span> <span m="4754510">and</span>
  <span m="4754600">that</span> <span m="4754750">looks</span> <span m="4755050">at,</span>
  <span m="4755740">if</span> <span m="4755890">the</span> <span m="4755980">patient</span>
  <span m="4756340">has</span> <span m="4756520">something</span> <span m="4756850">that's</span>
  <span m="4757030">abnormal</span> <span m="4757570">anywhere,</span> <span m="4758320">did</span>
  <span m="4758530">you</span> <span m="4758590">detect</span> <span m="4759040">it?</span>
  <span m="4759730">So</span> <span m="4759850">that's,</span> <span m="4760120">in</span>
  <span m="4760210">essence,</span> <span m="4760550">taking</span> <span m="4760760">an</span>
  <span m="4761020">or</span> <span m="4761650">of</span> <span m="4762040">each</span>
  <span m="4762220">of</span> <span m="4762280">those</span> <span m="4762460">1</span>
  <span m="4762670">second</span> <span m="4762970">intervals,</span> <span m="4763510">and</span>
  <span m="4763600">then</span> <span m="4763690">looking</span> <span m="4763930">across</span>
  <span m="4764290">patients.</span> <span m="4765310">And</span> <span m="4765760">from</span>
  <span m="4766000">a</span> <span m="4766030">clinical</span> <span m="4766390">diagnostic</span>
  <span m="4766930">perspective,</span> <span m="4767410">the</span> <span m="4767500">set</span>
  <span m="4768010">metric</span> <span m="4768400">might</span> <span m="4768610">be</span>
  <span m="4768730">most</span> <span m="4769000">useful,</span> <span m="4769400">but</span>
  <span m="4769420">then</span> <span m="4769510">when</span> <span m="4769630">you</span>
  <span m="4769720">want</span> <span m="4769840">to</span> <span m="4769960">introspect</span>
  <span m="4770590">and</span> <span m="4770680">understand</span> <span m="4771340">where</span>
  <span m="4771880">is</span> <span m="4772000">that</span> <span m="4772150">happening,</span>
  <span m="4772730">then</span> <span m="4772780">the</span> <span m="4772870">sequential</span>
  <span m="4773830">metric</span> <span m="4774250">is</span> <span m="4774370">important.</span></p><p><span
  m="4775600">And</span> <span m="4775960">the</span> <span m="4776050">key</span>
  <span m="4776290">take</span> <span m="4776560">home</span> <span m="4776650">message</span>
  <span m="4776980">from</span> <span m="4777130">the</span> <span m="4777220">paper</span>
  <span m="4778030">is</span> <span m="4778180">that,</span> <span m="4778300">if</span>
  <span m="4778390">you</span> <span m="4778480">compared</span> <span m="4778900">the</span>
  <span m="4778990">model's</span> <span m="4779320">predictions--</span> <span m="4780020">this</span>
  <span m="4780130">is,</span> <span m="4780850">I</span> <span m="4781030">think,</span>
  <span m="4781240">using</span> <span m="4782320">an</span> <span m="4782470">f1</span>
  <span m="4782980">metric--</span> <span m="4784990">to</span> <span m="4785650">what</span>
  <span m="4785830">you</span> <span m="4785910">would</span> <span m="4786040">get</span>
  <span m="4786250">from</span> <span m="4787630">a</span> <span m="4787840">panel</span>
  <span m="4788410">of</span> <span m="4788560">cardiologists,</span> <span m="4789790">these</span>
  <span m="4790030">models</span> <span m="4790570">are</span> <span m="4790720">doing</span>
  <span m="4791500">as</span> <span m="4791800">well,</span> <span m="4792010">if</span>
  <span m="4792100">not</span> <span m="4792310">better</span> <span m="4792790">than</span>
  <span m="4793030">these</span> <span m="4793210">panels</span> <span m="4793510">of</span>
  <span m="4793600">cardiologists.</span> <span m="4794500">So</span> <span m="4794620">this</span>
  <span m="4794800">is</span> <span m="4794920">extremely</span> <span m="4795580">exciting.</span>
  <span m="4796930">This</span> <span m="4797140">is</span> <span m="4797230">technology--</span>
  <span m="4797950">or</span> <span m="4798040">variance</span> <span m="4798480">of</span>
  <span m="4798550">this</span> <span m="4798700">is</span> <span m="4798790">technology</span>
  <span m="4799330">that</span> <span m="4799450">you're</span> <span m="4799600">going</span>
  <span m="4799930">to</span> <span m="4800050">see</span> <span m="4800530">deployed</span>
  <span m="4801160">now.</span> <span m="4802240">So</span> <span m="4802480">for</span>
  <span m="4802690">those</span> <span m="4802930">of</span> <span m="4802990">you</span>
  <span m="4803110">who</span> <span m="4803200">have</span> <span m="4803290">purchased</span>
  <span m="4803740">these</span> <span m="4803980">Apple</span> <span m="4804250">watches,</span>
  <span m="4804760">these</span> <span m="4804910">Samsung</span> <span m="4805300">watches,</span>
  <span m="4806200">I</span> <span m="4806260">don't</span> <span m="4806410">know</span>
  <span m="4806500">exactly</span> <span m="4807010">what</span> <span m="4807130">they're</span>
  <span m="4807220">using,</span> <span m="4807550">but</span> <span m="4807660">I</span>
  <span m="4807700">wouldn't</span> <span m="4807880">be</span> <span m="4807970">surprised</span>
  <span m="4808300">if</span> <span m="4808390">they're</span> <span m="4808480">using</span>
  <span m="4808750">techniques</span> <span m="4809520">similar</span> <span m="4809740">to</span>
  <span m="4809860">this.</span> <span m="4810580">And</span> <span m="4810700">you're</span>
  <span m="4810790">going</span> <span m="4810850">to</span> <span m="4810910">see</span>
  <span m="4811060">much</span> <span m="4811360">more</span> <span m="4811570">of</span>
  <span m="4811660">that</span> <span m="4811780">in</span> <span m="4811870">the</span>
  <span m="4811930">future.</span></p><p><span m="4812390">So</span> <span m="4812490">this</span>
  <span m="4812530">is</span> <span m="4812620">going</span> <span m="4812800">to</span>
  <span m="4812860">be</span> <span m="4812980">really</span> <span m="4813130">the</span>
  <span m="4813220">first</span> <span m="4813520">example</span> <span m="4814030">in</span>
  <span m="4814120">this</span> <span m="4814300">course</span> <span m="4814590">so</span>
  <span m="4814720">far</span> <span m="4814960">of</span> <span m="4815050">something</span>
  <span m="4815350">that's</span> <span m="4815530">really</span> <span m="4815830">been</span>
  <span m="4816190">deployed.</span> <span m="4818280">And</span> <span m="4818410">so</span>
  <span m="4818650">in</span> <span m="4818740">summary,</span> <span m="4819710">we're</span>
  <span m="4819940">very</span> <span m="4820330">often</span> <span m="4820660">in</span>
  <span m="4820750">the</span> <span m="4820810">realm</span> <span m="4821140">of</span>
  <span m="4821230">not</span> <span m="4821410">enough</span> <span m="4821680">data.</span>
  <span m="4822450">And</span> <span m="4822760">in</span> <span m="4822880">this</span>
  <span m="4823150">lecture</span> <span m="4823450">today,</span> <span m="4823720">we</span>
  <span m="4823840">gave</span> <span m="4824050">two</span> <span m="4824290">examples</span>
  <span m="4824860">how</span> <span m="4825220">you</span> <span m="4825340">can</span>
  <span m="4825460">deal</span> <span m="4825640">with</span> <span m="4825790">that.</span>
  <span m="4826030">First,</span> <span m="4826960">you</span> <span m="4827140">can</span>
  <span m="4828280">try</span> <span m="4828670">to</span> <span m="4828910">use</span>
  <span m="4829450">mechanistic</span> <span m="4830440">and</span> <span m="4830800">statistical</span>
  <span m="4831340">models</span> <span m="4832600">to</span> <span m="4832780">try</span>
  <span m="4833140">to</span> <span m="4837190">work</span> <span m="4837610">in</span>
  <span m="4837700">settings</span> <span m="4838050">where</span> <span m="4838150">you
  don't have</span> <span m="4838270">much</span> <span m="4838450">data.</span> <span
  m="4839590">And</span> <span m="4840350">in</span> <span m="4840730">other</span>
  <span m="4841000">extremes,</span> <span m="4841640">you</span> <span m="4841720">do</span>
  <span m="4841900">have</span> <span m="4842020">a</span> <span m="4842050">lot</span>
  <span m="4842170">of</span> <span m="4842230">data,</span> <span m="4842680">and</span>
  <span m="4842800">you</span> <span m="4842890">can</span> <span m="4843040">try</span>
  <span m="4843190">to</span> <span m="4843280">ignore</span> <span m="4843610">that,</span>
  <span m="4843760">and</span> <span m="4843850">just</span> <span m="4844000">use</span>
  <span m="4844160">these</span> <span m="4844300">black box</span> <span m="4844730">approaches.</span>
  <span m="4845050">That's</span> <span m="4845230">all</span> <span m="4845290">for</span>
  <span m="4845380">today.</span></p>
type: course
uid: 44f500ad6f949b39c554882388e3e81e

---
None