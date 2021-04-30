---
about_this_resource_text: '<p>Prof. Szolovits gives a deep dive into clinical data,
  the types of data, and how the data can be standardized. MIMIC-III data is used
  to illustrate these points. He discusses the difficulties of medicine harmonization
  and interoperability.</p> <p>Speaker: Peter Szolovits</p>             <p><a href="./resolveuid/32c1f4a77bf991ff7a40497d7fdc1e51">Lecture
  3: Deep Dive into Clinical Data slides (PDF - 2.1MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: 0UFwGJe6ubg
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: Video-YouTube-Stream
  type: Video
  uid: cdf77349c820ee3d942fd2f10cb5dcdb
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/0UFwGJe6ubg/default.jpg
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 5a3edc565bd55ae22b48a87ff398e118
- id: 3Play-3PlayYouTubeid-MP4
  media_location: 0UFwGJe6ubg
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: e6fdb48abd355df5cb11373192f499e7
- id: 0UFwGJe6ubg.srt
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-3-deep-dive-into-clinical-data/0UFwGJe6ubg.srt
  title: 3play caption file
  type: null
  uid: 378140d884730566301416ba551fd938
- id: 0UFwGJe6ubg.pdf
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-3-deep-dive-into-clinical-data/0UFwGJe6ubg.pdf
  title: 3play pdf file
  type: null
  uid: 862928e03615b009d43d86a6316d8113
- id: Caption-3Play YouTube id-SRT
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 806d8fd8a172879b3c8f7d9f64a41d2f
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 5593256e60d96d0b75ae34c560c3938a
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec03_300k.mp4
  parent_uid: 6418339f00fd3ae0b9d063f65ba1df17
  title: Video-Internet Archive-MP4
  type: Video
  uid: 7d865c872e5af5c0d96cdecdb6155e60
inline_embed_id: 41379135lecture3deepdiveintoclinicaldata70171169
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-3-deep-dive-into-clinical-data
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-3-deep-dive-into-clinical-data
template_type: Tabbed
title: 'Lecture 3: Deep Dive Into Clinical Data'
transcript: <p><span m="16170">PETER SZOLOVITS:</span> <span m="16274">So</span> <span
  m="16379">last</span> <span m="16680">time</span> <span m="16890">we</span> <span
  m="17010">talked</span> <span m="17400">about</span> <span m="17670">what</span>
  <span m="17910">medicine</span> <span m="18420">does,</span> <span m="19560">and</span>
  <span m="19920">today</span> <span m="20430">I</span> <span m="20580">want</span>
  <span m="20760">to</span> <span m="20820">take</span> <span m="21240">a</span> <span
  m="21300">deep</span> <span m="21600">dive</span> <span m="21990">into</span> <span
  m="22290">medical</span> <span m="22740">data.</span> <span m="24330">And</span>
  <span m="24510">I'm</span> <span m="24660">going</span> <span m="24900">to</span>
  <span m="25050">use</span> <span m="25620">as</span> <span m="25860">examples</span>
  <span m="27520">a</span> <span m="27620">lot</span> <span m="27720">of</span> <span
  m="27780">stuff</span> <span m="28110">from</span> <span m="28350">the</span> <span
  m="28440">MIMIC</span> <span m="28800">database,</span> <span m="29500">which</span>
  <span m="29610">is</span> <span m="29760">one</span> <span m="29970">of</span> <span
  m="30060">the</span> <span m="30180">databases</span> <span m="31470">that</span>
  <span m="31710">we're</span> <span m="31830">going</span> <span m="32070">to</span>
  <span m="32189">be</span> <span m="32340">using</span> <span m="32880">in</span>
  <span m="33030">this</span> <span m="33240">class.</span> <span m="34180">Some</span>
  <span m="34350">of</span> <span m="34470">you</span> <span m="34620">are</span>
  <span m="34710">probably</span> <span m="35160">familiar</span> <span m="35640">with</span>
  <span m="35910">it,</span> <span m="36480">and</span> <span m="36660">some</span>
  <span m="36930">of</span> <span m="37050">you</span> <span m="37200">are</span>
  <span m="37290">not.</span></p><p><span m="38670">And</span> <span m="38880">there</span>
  <span m="39090">are,</span> <span m="39450">I</span> <span m="39600">hope,</span>
  <span m="39900">some</span> <span m="40140">takeaway</span> <span m="40710">lessons</span>
  <span m="41280">from</span> <span m="41730">this</span> <span m="42030">discussion.</span>
  <span m="43600">So</span> <span m="43740">for</span> <span m="43950">example,</span>
  <span m="45850">a</span> <span m="45950">few</span> <span m="46080">years</span>
  <span m="46380">ago,</span> <span m="46890">when</span> <span m="48450">MIMIC-III</span>
  <span m="49770">was</span> <span m="50430">about</span> <span m="50760">to</span>
  <span m="50910">be</span> <span m="51090">released,</span> <span m="51630">I</span>
  <span m="51750">was</span> <span m="51960">playing</span> <span m="52350">with</span>
  <span m="52530">the</span> <span m="52650">data,</span> <span m="53790">and</span>
  <span m="54060">I</span> <span m="54270">looked</span> <span m="54750">at</span>
  <span m="55080">the</span> <span m="55860">distribution</span> <span m="56760">of</span>
  <span m="56880">heart</span> <span m="57180">rates</span> <span m="58440">in</span>
  <span m="58620">the</span> <span m="58740">CareVue</span> <span m="59310">part</span>
  <span m="59610">of</span> <span m="59730">the</span> <span m="59850">database.</span></p><p><span
  m="60660">So</span> <span m="60870">MIMIC,</span> <span m="61260">for</span> <span
  m="61470">those</span> <span m="61740">of</span> <span m="61860">you</span> <span
  m="62070">who</span> <span m="62170">don't</span> <span m="62400">know,</span> <span
  m="63690">has</span> <span m="64860">intensive</span> <span m="65400">care</span>
  <span m="65700">data</span> <span m="66120">from</span> <span m="66750">about</span>
  <span m="67320">60-something</span> <span m="68310">thousand</span> <span m="70410">admissions</span>
  <span m="71100">to</span> <span m="71280">intensive</span> <span m="71790">care</span>
  <span m="72030">units</span> <span m="72510">at</span> <span m="72660">the</span>
  <span m="72780">Beth</span> <span m="73020">Israel</span> <span m="73380">Deaconess</span>
  <span m="73860">Medical</span> <span m="74250">Center</span> <span m="76050">over</span>
  <span m="76410">a</span> <span m="76470">period</span> <span m="76890">of</span>
  <span m="77010">about</span> <span m="77370">12</span> <span m="77670">years.</span>
  <span m="78720">And</span> <span m="79230">one</span> <span m="79500">of</span>
  <span m="79650">the</span> <span m="80670">technical</span> <span m="81240">difficulties</span>
  <span m="81960">that</span> <span m="82170">we</span> <span m="82320">encountered</span>
  <span m="82860">is</span> <span m="83040">that</span> <span m="83190">in</span>
  <span m="83310">the</span> <span m="83400">middle</span> <span m="83670">of</span>
  <span m="83790">that</span> <span m="84000">time</span> <span m="84300">period.</span>
  <span m="85440">The</span> <span m="85560">hospitals</span> <span m="86120">shifted</span>
  <span m="86760">from</span> <span m="87090">one</span> <span m="87330">information</span>
  <span m="88050">system</span> <span m="89040">that</span> <span m="89220">they</span>
  <span m="89400">used</span> <span m="89760">in</span> <span m="89850">their</span>
  <span m="90030">intensive</span> <span m="90510">care</span> <span m="90780">unit</span>
  <span m="91110">to</span> <span m="91350">another.</span> <span m="92190">CareVue</span>
  <span m="92700">is</span> <span m="92850">the</span> <span m="92970">old</span>
  <span m="93240">one.</span> <span m="93480">MetaVision</span> <span m="94050">is</span>
  <span m="94230">the</span> <span m="94350">new</span> <span m="94530">one.</span>
  <span m="95310">And</span> <span m="95460">of</span> <span m="95550">course,</span>
  <span m="95980">they're</span> <span m="96030">not</span> <span m="96240">exactly</span>
  <span m="96750">compatible.</span> <span m="97420">So</span> <span m="98400">we'll</span>
  <span m="98580">see</span> <span m="98790">some</span> <span m="99030">examples</span>
  <span m="99600">of</span> <span m="99720">that.</span></p><p><span m="100510">So</span>
  <span m="100590">this</span> <span m="100860">is</span> <span m="101010">the</span>
  <span m="101190">old</span> <span m="101400">data.</span> <span m="101980">So</span>
  <span m="102150">this</span> <span m="102420">is</span> <span m="102570">from</span>
  <span m="103050">CareVue.</span> <span m="104100">And</span> <span m="104520">you</span>
  <span m="104670">look</span> <span m="104910">at</span> <span m="105000">that</span>
  <span m="105330">and</span> <span m="105450">say,</span> <span m="105850">well,</span>
  <span m="105960">heart</span> <span m="106290">rates</span> <span m="106650">range</span>
  <span m="107040">from</span> <span m="107900">40</span> <span m="108660">to</span>
  <span m="108870">200</span> <span m="109590">roughly,</span> <span m="111670">which</span>
  <span m="111870">is</span> <span m="112030">OK.</span> <span m="113250">But</span>
  <span m="113550">then</span> <span m="113850">there's</span> <span m="114210">this</span>
  <span m="114480">funny</span> <span m="114810">thing.</span> <span m="115380">There</span>
  <span m="115530">are</span> <span m="115620">two</span> <span m="115920">peaks.</span>
  <span m="117900">So</span> <span m="118890">where,</span> <span m="119340">if</span>
  <span m="119580">ever,</span> <span m="119970">do</span> <span m="120120">you</span>
  <span m="120300">see</span> <span m="120690">two</span> <span m="120960">peaks</span>
  <span m="122070">in</span> <span m="123600">physiological</span> <span m="124530">data?</span>
  <span m="128090">Not</span> <span m="128330">typical.</span> <span m="130380">And</span>
  <span m="130430">so</span> <span m="130699">my</span> <span m="131300">initial</span>
  <span m="131750">reaction</span> <span m="133070">was--</span></p><p><span m="134043">[LAUGHTER]</span></p><p>&nbsp;</p><p><span
  m="138480">So</span> <span m="139230">then</span> <span m="139380">I</span> <span
  m="139520">looked</span> <span m="139820">a</span> <span m="140310">little</span>
  <span m="140630">closer,</span> <span m="141170">and</span> <span m="141320">I</span>
  <span m="141440">said,</span> <span m="141710">hmm,</span> <span m="143330">what</span>
  <span m="143570">do</span> <span m="143630">the</span> <span m="143750">heart</span>
  <span m="144050">rates</span> <span m="144380">look</span> <span m="144650">like</span>
  <span m="145040">from</span> <span m="145370">these</span> <span m="145610">two</span>
  <span m="145790">systems?</span> <span m="147450">And</span> <span m="147620">if</span>
  <span m="147740">you</span> <span m="147890">look</span> <span m="148100">in</span>
  <span m="148490">CareVue,</span> <span m="148860">you</span> <span m="148910">see</span>
  <span m="149120">the</span> <span m="149240">picture</span> <span m="149660">that</span>
  <span m="149840">I</span> <span m="149960">just</span> <span m="150140">showed</span>
  <span m="150440">you.</span> <span m="150620">And</span> <span m="150740">if</span>
  <span m="150860">you</span> <span m="150980">look</span> <span m="151220">in</span>
  <span m="151340">MetaVision,</span> <span m="152640">you</span> <span m="152690">see</span>
  <span m="152960">this</span> <span m="153200">other</span> <span m="153440">picture,</span>
  <span m="153890">which</span> <span m="154160">looks</span> <span m="154490">more</span>
  <span m="154790">like</span> <span m="155060">what</span> <span m="155300">you</span>
  <span m="155390">would</span> <span m="155870">normally</span> <span m="156320">expect.</span></p><p><span
  m="158610">And</span> <span m="158660">so</span> <span m="158840">I'm</span> <span
  m="159020">sitting</span> <span m="159320">there</span> <span m="159500">scratching</span>
  <span m="160040">my</span> <span m="160250">head</span> <span m="160550">going,</span>
  <span m="160940">OK,</span> <span m="161270">there</span> <span m="161420">must</span>
  <span m="161660">be</span> <span m="161810">some</span> <span m="162110">difference</span>
  <span m="163310">between</span> <span m="163820">these.</span> <span m="164790">It's</span>
  <span m="164930">not</span> <span m="165800">that</span> <span m="166640">simultaneous</span>
  <span m="167690">with</span> <span m="167930">the</span> <span m="168020">switchover</span>
  <span m="168740">of</span> <span m="168890">the</span> <span m="168980">hospital</span>
  <span m="170000">from</span> <span m="170270">one</span> <span m="170480">information</span>
  <span m="171110">system</span> <span m="171560">to</span> <span m="171740">another.</span>
  <span m="173060">Physiology</span> <span m="173900">of</span> <span m="174050">people</span>
  <span m="174470">changed,</span> <span m="175130">and</span> <span m="175280">all</span>
  <span m="175430">of</span> <span m="175550">a</span> <span m="175610">sudden</span>
  <span m="176390">some</span> <span m="176690">subset</span> <span m="177200">of</span>
  <span m="177290">people</span> <span m="178580">started</span> <span m="179060">having</span>
  <span m="179450">faster</span> <span m="179990">heart</span> <span m="180230">rates.</span>
  <span m="181950">Right?</span> <span m="182930">But</span> <span m="183110">if</span>
  <span m="183260">you</span> <span m="183350">think</span> <span m="183620">about</span>
  <span m="183920">that</span> <span m="184190">what</span> <span m="184490">subset</span>
  <span m="185000">of</span> <span m="185090">people</span> <span m="185510">have</span>
  <span m="185750">faster</span> <span m="186260">heart</span> <span m="186530">rates?</span></p><p><span
  m="188420">AUDIENCE:</span> <span m="188665">Athletes.</span></p><p><span m="188910">PETER
  SZOLOVITS:</span> <span m="189155">Hmm?</span></p><p><span m="190380">AUDIENCE:</span>
  <span m="190625">Babies?</span></p><p><span m="193320">AUDIENCE:</span> <span m="193483">If</span>
  <span m="193646">you're</span> <span m="193810">in a</span> <span m="194300">stress
  test.</span></p><p><span m="195280">PETER SZOLOVITS:</span> <span m="195525">Unh-hmm.</span></p><p><span
  m="197260">AUDIENCE:</span> <span m="197320">Is</span> <span m="197380">it</span>
  <span m="197440">children?</span></p><p><span m="198252">PETER SZOLOVITS:</span>
  <span m="198456">Yeah,</span> <span m="198660">kids.</span> <span m="201490">So</span>
  <span m="201730">I</span> <span m="201840">said,</span> <span m="202120">hmm,</span>
  <span m="202660">interesting.</span> <span m="203590">So</span> <span m="203830">anyway,</span>
  <span m="204160">if</span> <span m="204310">you</span> <span m="204430">look</span>
  <span m="204640">at</span> <span m="204730">the</span> <span m="204850">statistics,</span>
  <span m="206300">you</span> <span m="206380">see</span> <span m="206620">that</span>
  <span m="206830">the</span> <span m="206950">mean</span> <span m="207220">heart</span>
  <span m="207550">rate</span> <span m="207850">in</span> <span m="208360">CareVue</span>
  <span m="208690">is</span> <span m="208870">108,</span> <span m="209820">and</span>
  <span m="209990">the</span> <span m="210180">mean</span> <span m="211400">heart</span>
  <span m="211900">rate</span> <span m="212140">in</span> <span m="212460">MetaVision</span>
  <span m="213160">is</span> <span m="213400">87.</span> <span m="215050">But</span>
  <span m="215320">of</span> <span m="215410">course,</span> <span m="217210">means</span>
  <span m="218110">are</span> <span m="218230">not</span> <span m="218500">that</span>
  <span m="218710">meaningful</span> <span m="219310">when</span> <span m="219490">you</span>
  <span m="219610">look</span> <span m="219910">at</span> <span m="221200">these</span>
  <span m="221440">bimodal</span> <span m="221980">distributions.</span></p><p><span
  m="223480">So</span> <span m="223660">then</span> <span m="223840">I</span> <span
  m="223960">said,</span> <span m="224300">well,</span> <span m="224480">what</span>
  <span m="224590">if</span> <span m="224710">we</span> <span m="224830">just</span>
  <span m="225070">look</span> <span m="225350">at</span> <span m="225700">adults?</span>
  <span m="226540">So</span> <span m="227800">we</span> <span m="227980">look</span>
  <span m="228190">at</span> <span m="228310">people</span> <span m="228730">from</span>
  <span m="229720">age</span> <span m="230590">greater</span> <span m="231010">than</span>
  <span m="231220">1</span> <span m="232570">up</span> <span m="232780">to</span>
  <span m="233170">age</span> <span m="233470">90.</span> <span m="234230">And</span>
  <span m="234430">I'll</span> <span m="234700">say</span> <span m="234970">a</span>
  <span m="235000">word</span> <span m="235270">about</span> <span m="235540">that</span>
  <span m="235780">in</span> <span m="235900">a</span> <span m="235960">minute.</span>
  <span m="236940">And</span> <span m="237130">I</span> <span m="237250">look</span>
  <span m="237490">at</span> <span m="237580">those</span> <span m="237820">two</span>
  <span m="238000">distributions.</span> <span m="238840">They</span> <span m="238990">look</span>
  <span m="239200">pretty</span> <span m="239470">close.</span> <span m="240100">They</span>
  <span m="240220">look</span> <span m="240400">pretty</span> <span m="240670">similar.</span>
  <span m="242120">So</span> <span m="242230">that</span> <span m="242470">means</span>
  <span m="242860">that</span> <span m="243850">the</span> <span m="244780">number</span>
  <span m="245290">of</span> <span m="245440">patients</span> <span m="246160">of</span>
  <span m="246340">different</span> <span m="246790">ages</span> <span m="247330">in</span>
  <span m="247510">the</span> <span m="247630">adult</span> <span m="248020">group</span>
  <span m="249010">is</span> <span m="249160">similar</span> <span m="249700">in</span>
  <span m="249850">the</span> <span m="249940">two</span> <span m="250150">data</span>
  <span m="250490">sets.</span></p><p><span m="252220">But</span> <span m="252460">if</span>
  <span m="252610">I</span> <span m="252820">don't</span> <span m="253240">exclude</span>
  <span m="254590">the</span> <span m="255040">very</span> <span m="255370">young</span>
  <span m="255760">or</span> <span m="255910">the</span> <span m="256029">very</span>
  <span m="256360">old,</span> <span m="257290">then</span> <span m="257529">I</span>
  <span m="257649">see</span> <span m="257920">this</span> <span m="258160">funny</span>
  <span m="258490">distribution</span> <span m="260200">where</span> <span m="260470">I</span>
  <span m="260589">have</span> <span m="260860">suppressed</span> <span m="261470">ages</span>
  <span m="261850">greater</span> <span m="262210">than</span> <span m="262360">90</span>
  <span m="262840">but</span> <span m="263080">not</span> <span m="263440">the</span>
  <span m="263560">young.</span> <span m="264700">And</span> <span m="264880">what</span>
  <span m="265120">you</span> <span m="265240">see</span> <span m="265540">is</span>
  <span m="265720">that</span> <span m="265900">in</span> <span m="266390">CareVue</span>
  <span m="266640">there's</span> <span m="266890">this</span> <span m="267100">giant</span>
  <span m="267490">spike</span> <span m="268240">at</span> <span m="268420">age</span>
  <span m="268600">0.</span></p><p><span m="272440">So</span> <span m="272650">what</span>
  <span m="272860">happened</span> <span m="273940">at</span> <span m="274120">the</span>
  <span m="274210">hospital</span> <span m="275380">is</span> <span m="275620">that</span>
  <span m="275920">under</span> <span m="276220">the</span> <span m="276400">old</span>
  <span m="276640">system</span> <span m="277570">it</span> <span m="277750">was</span>
  <span m="277960">also</span> <span m="278380">being</span> <span m="278710">used</span>
  <span m="279220">in</span> <span m="279460">the</span> <span m="279580">NICU,</span>
  <span m="280510">the</span> <span m="280720">Neonatal</span> <span m="281320">Intensive</span>
  <span m="281860">Care</span> <span m="282100">Unit.</span> <span m="283110">And</span>
  <span m="283240">the</span> <span m="283330">new</span> <span m="283540">system</span>
  <span m="283960">was</span> <span m="284170">not</span> <span m="284440">being</span>
  <span m="284710">used</span> <span m="285170">in</span> <span m="285190">the</span>
  <span m="285340">NICU.</span> <span m="286750">And</span> <span m="286960">therefore,</span>
  <span m="287830">they</span> <span m="288100">didn't</span> <span m="288280">capture</span>
  <span m="288820">data</span> <span m="289240">about</span> <span m="289510">babies.</span></p><p><span
  m="292090">And</span> <span m="292270">in</span> <span m="292390">fact,</span> <span
  m="292880">if</span> <span m="292930">you</span> <span m="293080">look</span> <span
  m="294010">at</span> <span m="295900">age</span> <span m="296260">versus</span>
  <span m="296770">heart</span> <span m="297100">rate</span> <span m="298000">of</span>
  <span m="298210">the</span> <span m="298360">entire</span> <span m="298780">population,</span>
  <span m="300340">you</span> <span m="300520">see</span> <span m="300970">two</span>
  <span m="301240">very</span> <span m="301540">peculiar</span> <span m="302170">things.</span>
  <span m="303200">So</span> <span m="303760">here</span> <span m="304030">are</span>
  <span m="304150">the</span> <span m="304330">adults</span> <span m="304930">that</span>
  <span m="305140">we've</span> <span m="305350">been</span> <span m="305500">talking</span>
  <span m="305950">about,</span> <span m="307120">and</span> <span m="307270">here</span>
  <span m="307510">are</span> <span m="307570">the</span> <span m="307720">babies.</span>
  <span m="308290">And</span> <span m="308410">sure</span> <span m="308680">enough,</span>
  <span m="308980">they</span> <span m="309160">have</span> <span m="309370">higher</span>
  <span m="309670">heart</span> <span m="309970">rates.</span> <span m="311080">And</span>
  <span m="311230">then</span> <span m="311440">here</span> <span m="311690">are</span>
  <span m="311770">these</span> <span m="312040">300-year-old</span> <span m="313000">people.</span></p><p><span
  m="313892">[LAUGHTER]</span></p><p><span m="315040">You go,</span> <span m="315280">wow,</span>
  <span m="316400">I</span> <span m="316570">don't</span> <span m="316810">think</span>
  <span m="317080">I'm</span> <span m="317210">going</span> <span m="317320">to</span>
  <span m="317410">have</span> <span m="317650">a</span> <span m="317710">heart</span>
  <span m="318010">rate</span> <span m="318310">when</span> <span m="318460">I'm</span>
  <span m="318610">300</span> <span m="319180">years</span> <span m="319520">old.</span>
  <span m="321000">So</span> <span m="321700">who</span> <span m="322030">are</span>
  <span m="322210">those</span> <span m="322540">people?</span> <span m="326230">Anybody</span>
  <span m="326680">have</span> <span m="326890">a</span> <span m="326950">clue?</span>
  <span m="328960">Yeah?</span></p><p><span m="329612">AUDIENCE:</span> <span m="329833">Entry</span>
  <span m="330054">errors.</span></p><p><span m="330940">PETER SZOLOVITS:</span> <span
  m="331135">Sorry?</span></p><p><span m="331330">AUDIENCE:</span> <span m="331550">Entry</span>
  <span m="332210">errors?</span></p><p><span m="334410">PETER SZOLOVITS:</span> <span
  m="334560">There</span> <span m="334710">are</span> <span m="334750">too</span>
  <span m="334990">many</span> <span m="335290">of</span> <span m="335440">them.</span>
  <span m="335940">Yeah,</span> <span m="336280">entry</span> <span m="336700">errors</span>
  <span m="337090">is</span> <span m="337240">always</span> <span m="337600">a</span>
  <span m="337660">possibility,</span> <span m="338890">but</span> <span m="339130">there's</span>
  <span m="339370">quite</span> <span m="339640">a</span> <span m="339700">few</span>
  <span m="340000">data</span> <span m="340300">points</span> <span m="340750">there.</span>
  <span m="341470">Yeah?</span></p><p><span m="342176">AUDIENCE:</span> <span m="342409">[INAUDIBLE]</span></p><p><span
  m="345910">PETER SZOLOVITS:</span> <span m="346067">Close.</span> <span m="346540">It's</span>
  <span m="346750">not</span> <span m="346990">quite</span> <span m="347290">missing</span>
  <span m="347650">data.</span> <span m="348460">So</span> <span m="348670">HIPAA,</span>
  <span m="349180">the</span> <span m="349570">Health</span> <span m="349870">Insurance</span>
  <span m="350380">Portability</span> <span m="351160">and</span> <span m="351310">Accountability</span>
  <span m="352150">Act,</span> <span m="352990">defines</span> <span m="353710">a</span>
  <span m="353800">set</span> <span m="354070">of</span> <span m="354190">criteria</span>
  <span m="355570">about</span> <span m="355960">protecting</span> <span m="356620">personal</span>
  <span m="357160">health</span> <span m="357460">information.</span> <span m="358850">And</span>
  <span m="359170">one</span> <span m="359440">of</span> <span m="359560">the</span>
  <span m="359680">things</span> <span m="360070">you</span> <span m="360130">are</span>
  <span m="360220">not</span> <span m="360460">allowed</span> <span m="360790">to</span>
  <span m="360970">do</span> <span m="361540">is</span> <span m="361780">to</span>
  <span m="361900">specify</span> <span m="362650">the</span> <span m="362830">age</span>
  <span m="363220">of</span> <span m="363340">somebody</span> <span m="364270">who</span>
  <span m="364450">is</span> <span m="364600">90</span> <span m="364930">years</span>
  <span m="365260">old</span> <span m="365560">or</span> <span m="365770">older.</span>
  <span m="367600">And</span> <span m="367750">the</span> <span m="367810">reason</span>
  <span m="368200">is</span> <span m="368410">because</span> <span m="368680">the</span>
  <span m="368800">number</span> <span m="369220">of</span> <span m="369400">97-year-olds</span>
  <span m="371200">is</span> <span m="371380">pretty</span> <span m="371650">small.</span></p><p><span
  m="372800">And</span> <span m="372880">so</span> <span m="373120">if</span> <span
  m="373300">I</span> <span m="373420">tell</span> <span m="373720">you</span> <span
  m="373930">that</span> <span m="374170">Willy</span> <span m="374530">is</span>
  <span m="374680">97</span> <span m="375370">years</span> <span m="375670">old,</span>
  <span m="376420">then</span> <span m="376690">you're</span> <span m="376810">going</span>
  <span m="377000">to</span> <span m="377050">be</span> <span m="377230">able</span>
  <span m="377380">to</span> <span m="377500">pick</span> <span m="377800">him</span>
  <span m="377950">out</span> <span m="378100">of</span> <span m="378220">a</span>
  <span m="378280">population</span> <span m="379120">relatively</span> <span m="379750">easily,</span>
  <span m="380710">and</span> <span m="380860">so</span> <span m="381070">it's</span>
  <span m="381280">prohibited</span> <span m="382000">to</span> <span m="382180">say</span>
  <span m="382480">that.</span> <span m="384640">So</span> <span m="384970">as</span>
  <span m="385210">a</span> <span m="385270">result,</span> <span m="385960">everybody</span>
  <span m="386560">who's</span> <span m="386770">90</span> <span m="387160">or</span>
  <span m="387310">older</span> <span m="388150">gets</span> <span m="388510">labeled</span>
  <span m="389050">as</span> <span m="389230">being</span> <span m="389500">300</span>
  <span m="390130">years</span> <span m="390400">old</span> <span m="391000">in</span>
  <span m="391150">the</span> <span m="391240">database.</span></p><p><span m="392350">It's</span>
  <span m="392550">an</span> <span m="392680">artifact.</span> <span m="394840">It's</span>
  <span m="395080">like</span> <span m="395770">back</span> <span m="398156">in</span>
  <span m="398500">my</span> <span m="398710">youth,</span> <span m="399280">I</span>
  <span m="399460">worked</span> <span m="399850">as</span> <span m="400030">a</span>
  <span m="400090">computer</span> <span m="400570">programmer</span> <span m="401770">at</span>
  <span m="401980">a</span> <span m="402040">health</span> <span m="402310">sciences</span>
  <span m="402850">computing</span> <span m="403360">facility</span> <span m="403990">at</span>
  <span m="404140">UCLA.</span> <span m="405370">And</span> <span m="405550">we</span>
  <span m="405700">used</span> <span m="405910">to</span> <span m="406000">have</span>
  <span m="406180">a</span> <span m="406240">convention</span> <span m="408130">that</span>
  <span m="408370">missing</span> <span m="408790">data</span> <span m="409150">was</span>
  <span m="409390">represented</span> <span m="410080">by</span> <span m="410320">99999.</span>
  <span m="413272">And</span> <span m="413770">of</span> <span m="413860">course,</span>
  <span m="414190">if</span> <span m="414310">you</span> <span m="414520">average</span>
  <span m="415030">that</span> <span m="415340">into</span> <span m="416590">a</span>
  <span m="416650">real</span> <span m="416950">data</span> <span m="417290">set,</span>
  <span m="417640">you</span> <span m="417760">get</span> <span m="418000">garbage,</span>
  <span m="419530">which</span> <span m="419830">people</span> <span m="420190">did</span>
  <span m="420430">regularly.</span> <span m="421720">So</span> <span m="421950">there</span>
  <span m="422450">are</span> <span m="422530">problems</span> <span m="423040">with</span>
  <span m="423280">this,</span> <span m="423580">and</span> <span m="423700">we're</span>
  <span m="423850">running</span> <span m="424210">into</span> <span m="424450">one</span>
  <span m="424630">of</span> <span m="424690">those.</span></p><p><span m="425530">If</span>
  <span m="425680">you</span> <span m="425830">look</span> <span m="426100">at</span>
  <span m="426190">just</span> <span m="426940">the</span> <span m="427170">adults,</span>
  <span m="430120">the</span> <span m="430300">two</span> <span m="430510">systems</span>
  <span m="431050">actually</span> <span m="431530">look</span> <span m="431740">very</span>
  <span m="432010">similar.</span> <span m="432620">So</span> <span m="432760">the</span>
  <span m="433420">blue</span> <span m="433690">and</span> <span m="433780">red</span>
  <span m="434050">dots,</span> <span m="434560">or</span> <span m="434710">the</span>
  <span m="434860">two</span> <span m="435070">systems,</span> <span m="436150">and</span>
  <span m="436360">I've</span> <span m="436570">drawn</span> <span m="437560">the</span>
  <span m="437740">trend</span> <span m="438100">lines</span> <span m="438520">between</span>
  <span m="438970">them,</span> <span m="439180">and</span> <span m="439300">you</span>
  <span m="439390">can</span> <span m="439570">see</span> <span m="439780">that</span>
  <span m="439990">they're</span> <span m="440140">very</span> <span m="440380">similar.</span>
  <span m="441680">So</span> <span m="441970">it</span> <span m="442150">looks</span>
  <span m="442420">like</span> <span m="442720">as</span> <span m="442900">you</span>
  <span m="443020">get</span> <span m="443200">older,</span> <span m="443720">your</span>
  <span m="443830">heart</span> <span m="444130">rate</span> <span m="444400">declines</span>
  <span m="445210">very</span> <span m="445480">slightly.</span> <span m="447130">But</span>
  <span m="447370">it</span> <span m="447460">does</span> <span m="447700">so</span>
  <span m="448120">equally</span> <span m="448570">in</span> <span m="448690">the</span>
  <span m="448810">two</span> <span m="449430">data</span> <span m="449740">sets.</span>
  <span m="450110">Yeah?</span></p><p><span m="450390">AUDIENCE:</span> <span m="450463">On</span>
  <span m="450536">the</span> <span m="450610">previous slide,</span> <span m="451530">beyond</span>
  <span m="451940">300,</span> <span m="452330">it</span> <span m="452720">looks like</span>
  <span m="453110">they're</span> <span m="453770">older</span> <span m="454040">than</span>
  <span m="454466">300?</span></p><p><span m="455320">PETER SZOLOVITS:</span> <span
  m="455440">Well</span> <span m="455560">that's</span> <span m="455830">because</span>
  <span m="456340">the</span> <span m="456760">ages</span> <span m="457240">there</span>
  <span m="457600">are</span> <span m="457780">computed</span> <span m="458530">at</span>
  <span m="458800">the</span> <span m="458950">time</span> <span m="459310">that</span>
  <span m="459520">the</span> <span m="459610">heart</span> <span m="459940">rate</span>
  <span m="460210">is</span> <span m="460390">measured.</span> <span m="461120">And</span>
  <span m="461200">so</span> <span m="461710">if</span> <span m="461950">you</span>
  <span m="462220">are</span> <span m="462790">300</span> <span m="463390">years</span>
  <span m="463690">old</span> <span m="463960">when</span> <span m="464170">you're</span>
  <span m="464350">admitted</span> <span m="464740">to</span> <span m="464890">the</span>
  <span m="465010">hospital,</span> <span m="466060">if</span> <span m="466270">you</span>
  <span m="466420">stay</span> <span m="466750">in</span> <span m="466840">the</span>
  <span m="466930">hospital</span> <span m="467470">for</span> <span m="467710">six</span>
  <span m="468040">months,</span> <span m="468910">then</span> <span m="469180">you're</span>
  <span m="469390">300</span> <span m="469780">and</span> <span m="470170">1/2</span>
  <span m="470560">years</span> <span m="470830">old</span> <span m="471220">by</span>
  <span m="471360">the</span> <span m="471490">time</span> <span m="471910">of</span>
  <span m="472050">that</span> <span m="472260">measurement.</span> <span m="472595">[LAUGHS]</span>
  <span m="473320">So</span> <span m="473500">that's</span> <span m="473770">why</span>
  <span m="474010">there</span> <span m="474190">are</span> <span m="474460">data</span>
  <span m="474730">points</span> <span m="475150">to</span> <span m="475330">the</span>
  <span m="475450">right</span> <span m="475960">of</span> <span m="476830">300.</span>
  <span m="478000">Yeah,</span> <span m="478720">good</span> <span m="478930">catch.</span></p><p><span
  m="481240">OK,</span> <span m="481690">and</span> <span m="481840">then</span> <span
  m="482020">this</span> <span m="482230">is</span> <span m="482380">what</span> <span
  m="482560">the</span> <span m="482650">babies</span> <span m="483070">look</span>
  <span m="483280">like.</span> <span m="483580">And</span> <span m="483670">of</span>
  <span m="483790">course,</span> <span m="484190">they</span> <span m="484240">do</span>
  <span m="484450">have</span> <span m="484660">higher</span> <span m="484960">heart</span>
  <span m="485200">rates.</span> <span m="486730">And</span> <span m="486970">here</span>
  <span m="487360">here</span> <span m="487600">are</span> <span m="487660">the</span>
  <span m="487840">oldsters.</span> <span m="488500">So</span> <span m="488920">actually,</span>
  <span m="489430">there</span> <span m="489670">are</span> <span m="490750">people</span>
  <span m="491230">out</span> <span m="491440">to</span> <span m="491900">310</span>
  <span m="492700">years</span> <span m="493600">old</span> <span m="494560">because</span>
  <span m="495100">maybe</span> <span m="495550">they</span> <span m="495790">were</span>
  <span m="496030">discharged</span> <span m="496690">from the</span> <span m="496900">hospital.</span>
  <span m="498430">And</span> <span m="498700">then</span> <span m="498940">at</span>
  <span m="499090">age</span> <span m="499300">100,</span> <span m="499810">they</span>
  <span m="500020">came</span> <span m="500320">back.</span> <span m="501410">You</span>
  <span m="501480">know,</span> <span m="501790">maybe</span> <span m="502090">they</span>
  <span m="502240">were</span> <span m="502390">90</span> <span m="502720">years</span>
  <span m="503050">old</span> <span m="503320">at</span> <span m="503440">the</span>
  <span m="503560">time</span> <span m="503890">they</span> <span m="504040">were</span>
  <span m="504700">initially</span> <span m="505180">admitted</span> <span m="505600">10</span>
  <span m="505870">years</span> <span m="506110">later.</span> <span m="506540">They</span>
  <span m="506620">came</span> <span m="506860">back,</span> <span m="507550">and</span>
  <span m="507730">we</span> <span m="507880">recorded</span> <span m="508420">more</span>
  <span m="508630">data</span> <span m="508990">about</span> <span m="509320">them,</span>
  <span m="509650">and</span> <span m="509755">so</span> <span m="509860">this</span>
  <span m="510100">is</span> <span m="510250">all</span> <span m="510400">relative</span>
  <span m="511550">to</span> <span m="511780">that</span> <span m="512020">300.</span></p><p><span
  m="513600">OK,</span> <span m="513940">so</span> <span m="514150">that's</span>
  <span m="514419">just</span> <span m="514659">one</span> <span m="514900">example.</span>
  <span m="515679">And</span> <span m="516100">the</span> <span m="516280">lesson</span>
  <span m="516760">there</span> <span m="517690">is</span> <span m="517990">be</span>
  <span m="518169">careful</span> <span m="518799">when</span> <span m="519010">you</span>
  <span m="519130">look</span> <span m="519370">at</span> <span m="519490">data</span>
  <span m="519909">because</span> <span m="520480">it</span> <span m="520630">can</span>
  <span m="520990">really</span> <span m="521320">easily</span> <span m="521770">fool</span>
  <span m="522070">you</span> <span m="522950">'cause</span> <span m="523480">there</span>
  <span m="523630">are</span> <span m="523720">all</span> <span m="523929">kinds</span>
  <span m="524320">of</span> <span m="524380">funny</span> <span m="524770">things</span>
  <span m="525220">about</span> <span m="525550">the</span> <span m="525640">way</span>
  <span m="525850">it's</span> <span m="526030">collected,</span> <span m="527200">about</span>
  <span m="527740">these</span> <span m="528210">artifactual</span> <span m="528940">things</span>
  <span m="529360">like</span> <span m="529630">300-year-old</span> <span m="530560">patients</span>
  <span m="531610">and</span> <span m="531760">so</span> <span m="532030">on.</span></p><p><span
  m="534370">So</span> <span m="534610">here's</span> <span m="534880">a</span> <span
  m="534940">catalog</span> <span m="535840">of</span> <span m="536020">the</span>
  <span m="536170">types</span> <span m="536590">of</span> <span m="536710">data</span>
  <span m="537100">that</span> <span m="537280">are</span> <span m="537430">available</span>
  <span m="538000">to</span> <span m="538210">us.</span> <span m="539330">So</span>
  <span m="539470">we</span> <span m="539620">have</span> <span m="540480">the</span>
  <span m="540670">typical</span> <span m="541240">kind</span> <span m="541540">of</span>
  <span m="541810">electronic</span> <span m="542410">health</span> <span m="542680">record</span>
  <span m="543040">data</span> <span m="543400">from</span> <span m="543670">hospitals--</span>
  <span m="545110">demographics,</span> <span m="546580">age,</span> <span m="546890">sex,</span>
  <span m="547090">socioeconomic</span> <span m="547960">status,</span> <span m="549010">insurance</span>
  <span m="549520">type,</span> <span m="549820">language,</span> <span m="550370">religion,</span>
  <span m="550720">living</span> <span m="551050">situation,</span> <span m="551740">family</span>
  <span m="552160">structure,</span> <span m="552670">location,</span> <span m="553390">work,</span>
  <span m="554240">et</span> <span m="554290">cetera.</span></p><p><span m="555700">We</span>
  <span m="555880">have</span> <span m="555970">vital</span> <span m="556360">signs--</span>
  <span m="557020">your</span> <span m="557230">weight,</span> <span m="557620">your</span>
  <span m="557770">height,</span> <span m="558190">your</span> <span m="558340">pulse,</span>
  <span m="558860">respiration</span> <span m="559570">rate,</span> <span m="559840">body</span>
  <span m="560170">temperature,</span> <span m="561370">et</span> <span m="561390">cetera.</span>
  <span m="562430">So</span> <span m="562540">these</span> <span m="562810">are</span>
  <span m="562930">typically</span> <span m="563500">the</span> <span m="563650">things</span>
  <span m="564070">that</span> <span m="564760">if</span> <span m="564940">you</span>
  <span m="565360">ever</span> <span m="565600">go</span> <span m="565750">to</span>
  <span m="565870">a</span> <span m="565960">doctor's</span> <span m="566500">office,</span>
  <span m="567040">or</span> <span m="567490">you</span> <span m="567640">go</span>
  <span m="567850">into</span> <span m="568150">a</span> <span m="568210">hospital,</span>
  <span m="569170">the</span> <span m="569500">nurse</span> <span m="569860">will</span>
  <span m="570040">take</span> <span m="570340">you</span> <span m="570520">aside</span>
  <span m="570970">and</span> <span m="571480">weigh</span> <span m="571780">you</span>
  <span m="572020">and</span> <span m="572140">measure</span> <span m="572500">your</span>
  <span m="572710">height</span> <span m="573130">and</span> <span m="574210">check</span>
  <span m="574510">your</span> <span m="574660">blood</span> <span m="574930">pressure</span>
  <span m="575500">and</span> <span m="576790">take</span> <span m="577090">your</span>
  <span m="577240">temperature</span> <span m="577930">and</span> <span m="578050">stuff</span>
  <span m="578380">like</span> <span m="578590">that.</span> <span m="578890">These</span>
  <span m="579160">are</span> <span m="579610">standard</span> <span m="580090">vital</span>
  <span m="580420">signs,</span> <span m="580930">and</span> <span m="581050">so</span>
  <span m="581230">we</span> <span m="581380">have</span> <span m="581980">lots</span>
  <span m="582310">of</span> <span m="582430">those</span> <span m="582730">recorded.</span></p><p><span
  m="584380">Medications--</span> <span m="585880">prescription</span> <span m="586570">medications,</span>
  <span m="587920">over-the-counter</span> <span m="588670">drugs,</span> <span m="589300">illegal</span>
  <span m="589810">drugs</span> <span m="590420">if</span> <span m="590470">you're</span>
  <span m="590620">willing</span> <span m="590950">not</span> <span m="591190">to</span>
  <span m="591310">lie</span> <span m="591700">to</span> <span m="591850">your</span>
  <span m="592240">health</span> <span m="592340">care</span> <span m="592660">provider,</span>
  <span m="594130">alcohol.</span> <span m="596050">Again,</span> <span m="596650">one</span>
  <span m="596950">of</span> <span m="597010">my</span> <span m="597220">earliest</span>
  <span m="597730">days,</span> <span m="598720">I</span> <span m="598870">was</span>
  <span m="599110">hanging</span> <span m="599440">out</span> <span m="599680">with</span>
  <span m="599920">a</span> <span m="599950">cardiologist</span> <span m="600940">at</span>
  <span m="602230">Tufts</span> <span m="602590">Medical</span> <span m="603010">Center,</span>
  <span m="603580">and</span> <span m="604330">we</span> <span m="604570">see</span>
  <span m="604840">this</span> <span m="605260">elderly</span> <span m="605740">lady</span>
  <span m="606700">who</span> <span m="608380">looks</span> <span m="608710">kind</span>
  <span m="608980">of</span> <span m="609040">terrible.</span> <span m="611140">And</span>
  <span m="611350">we're</span> <span m="611560">talking</span> <span m="612040">to</span>
  <span m="612250">her--</span> <span m="613060">well,</span> <span m="613360">the</span>
  <span m="613540">doctor</span> <span m="613990">is</span> <span m="614140">talking</span>
  <span m="614530">to</span> <span m="614710">her.</span> <span m="614860">I'm</span>
  <span m="615040">trying</span> <span m="615370">to</span> <span m="615520">stay</span>
  <span m="615820">out</span> <span m="615970">of</span> <span m="616030">the</span>
  <span m="616150">way.</span></p><p><span m="618300">And</span> <span m="618610">he</span>
  <span m="618730">says,</span> <span m="620560">so</span> <span m="622330">do</span>
  <span m="622510">you</span> <span m="622600">drink</span> <span m="622930">alcohol?</span>
  <span m="624430">And</span> <span m="624610">she</span> <span m="624760">says,</span>
  <span m="625160">oh,</span> <span m="625210">no,</span> <span m="625460">never</span>
  <span m="625780">touch</span> <span m="626080">the</span> <span m="626170">stuff.</span>
  <span m="627760">And</span> <span m="627940">then</span> <span m="628150">we</span>
  <span m="628300">talk</span> <span m="628600">some</span> <span m="628780">more,</span>
  <span m="629260">and</span> <span m="629630">we go</span> <span m="629780">out</span>
  <span m="630740">of</span> <span m="630860">the</span> <span m="630950">patient's</span>
  <span m="631490">room.</span> <span m="632440">And</span> <span m="634880">the</span>
  <span m="634970">doctor</span> <span m="635360">turns</span> <span m="635750">to</span>
  <span m="635870">me</span> <span m="636290">out</span> <span m="636500">of</span>
  <span m="636680">earshot</span> <span m="637160">of</span> <span m="637280">the</span>
  <span m="637400">patient</span> <span m="638360">and</span> <span m="638540">says,</span>
  <span m="638970">oh,</span> <span m="639020">she's</span> <span m="639380">a</span>
  <span m="639440">chronic</span> <span m="639860">drunk.</span></p><p><span m="641540">I</span>
  <span m="641630">said,</span> <span m="641990">well,</span> <span m="642120">how</span>
  <span m="642170">do</span> <span m="642230">you</span> <span m="642350">know?</span>
  <span m="643400">And</span> <span m="643550">he</span> <span m="643640">says,</span>
  <span m="643910">well,</span> <span m="644630">from</span> <span m="644900">lab</span>
  <span m="645200">tests,</span> <span m="645710">from</span> <span m="645950">the</span>
  <span m="646100">appearance</span> <span m="646640">of</span> <span m="646760">her</span>
  <span m="646880">skin,</span> <span m="647390">from</span> <span m="647690">her</span>
  <span m="647810">general</span> <span m="648290">demeanor,</span> <span m="649760">from</span>
  <span m="650660">various</span> <span m="651620">sort</span> <span m="651860">of</span>
  <span m="652100">ineffable</span> <span m="652670">factors.</span> <span m="653750">And</span>
  <span m="653900">so</span> <span m="654080">patients</span> <span m="654620">lie.</span>
  <span m="657200">They</span> <span m="657500">really</span> <span m="657770">do</span>
  <span m="658160">because</span> <span m="658610">they</span> <span m="658730">don't</span>
  <span m="658850">want</span> <span m="659000">to</span> <span m="659060">tell</span>
  <span m="659270">you</span> <span m="659390">things.</span></p><p><span m="662910">Medications,</span>
  <span m="663710">by</span> <span m="663920">the</span> <span m="664010">way,</span>
  <span m="664190">is</span> <span m="664340">a</span> <span m="664400">big</span>
  <span m="664670">deal.</span> <span m="665250">So</span> <span m="665720">there</span>
  <span m="665980">is</span> <span m="666200">this</span> <span m="666380">whole</span>
  <span m="666650">field</span> <span m="667130">called</span> <span m="667460">med</span>
  <span m="667805">red,</span> <span m="668660">medication</span> <span m="669350">reconciliation,</span>
  <span m="671820">which</span> <span m="672080">is</span> <span m="672290">the</span>
  <span m="672740">hospitals</span> <span m="673460">or</span> <span m="673610">the</span>
  <span m="673730">doctors'</span> <span m="674240">offices</span> <span m="674840">attempt</span>
  <span m="675770">to</span> <span m="675920">figure</span> <span m="676310">out</span>
  <span m="676580">what</span> <span m="676790">medications</span> <span m="677600">you're</span>
  <span m="677720">actually</span> <span m="678140">taking.</span> <span m="679440">So</span>
  <span m="679700">I'm</span> <span m="679970">a</span> <span m="680060">member</span>
  <span m="680420">of</span> <span m="680510">the</span> <span m="680660">MIT</span>
  <span m="681140">health</span> <span m="681440">plan,</span> <span m="681800">and</span>
  <span m="681950">if</span> <span m="682130">I</span> <span m="682280">sign</span>
  <span m="682670">into</span> <span m="683030">my</span> <span m="683480">health</span>
  <span m="683750">plan</span> <span m="684050">account,</span> <span m="685070">it</span>
  <span m="685220">tells</span> <span m="685670">me</span> <span m="685910">that</span>
  <span m="686360">I'm</span> <span m="686600">taking</span> <span m="687890">some</span>
  <span m="688220">pills</span> <span m="688880">that</span> <span m="689120">I</span>
  <span m="689270">got</span> <span m="690080">12</span> <span m="690350">years</span>
  <span m="690710">ago</span> <span m="692030">as</span> <span m="692300">part</span>
  <span m="692660">of</span> <span m="692870">a</span> <span m="693290">laboratory</span>
  <span m="694070">test,</span> <span m="696320">where</span> <span m="696980">I</span>
  <span m="697100">took</span> <span m="697370">two</span> <span m="697580">pills</span>
  <span m="698570">which</span> <span m="698870">were</span> <span m="699050">supposed</span>
  <span m="699500">to</span> <span m="699620">have</span> <span m="699800">some</span>
  <span m="700070">physiological</span> <span m="700910">effect,</span> <span m="701390">and</span>
  <span m="701510">then</span> <span m="701660">they</span> <span m="701810">measured</span>
  <span m="702200">that.</span> <span m="703070">And</span> <span m="703280">I've</span>
  <span m="703460">never</span> <span m="703820">gotten</span> <span m="704240">another</span>
  <span m="704600">pill</span> <span m="704990">and</span> <span m="705110">never</span>
  <span m="705410">taken</span> <span m="705830">one</span> <span m="706220">since</span>
  <span m="706610">then,</span> <span m="707360">nor</span> <span m="707600">would</span>
  <span m="707780">it</span> <span m="707900">be</span> <span m="708110">particularly</span>
  <span m="708860">good</span> <span m="709070">for</span> <span m="709340">me.</span>
  <span m="710270">But</span> <span m="710510">it's</span> <span m="710630">still</span>
  <span m="710930">on</span> <span m="711050">my</span> <span m="711230">record,</span>
  <span m="712100">and</span> <span m="712370">there's</span> <span m="712670">no</span>
  <span m="713090">notice</span> <span m="713720">of</span> <span m="713870">it</span>
  <span m="714050">ever</span> <span m="714320">having</span> <span m="714650">been</span>
  <span m="714830">discontinued.</span> <span m="716720">And</span> <span m="716840">that's</span>
  <span m="717080">a</span> <span m="717110">real</span> <span m="717380">problem</span>
  <span m="717950">because</span> <span m="718730">if</span> <span m="718940">you're</span>
  <span m="719090">taking</span> <span m="719480">care</span> <span m="719720">of</span>
  <span m="719810">a</span> <span m="719870">patient,</span> <span m="720830">you'd</span>
  <span m="721040">like</span> <span m="721250">to</span> <span m="721400">understand</span>
  <span m="722030">what</span> <span m="722270">drugs</span> <span m="722600">they're</span>
  <span m="722780">actually</span> <span m="723200">taking,</span> <span m="724030">and</span>
  <span m="724910">it's</span> <span m="725060">hard</span> <span m="725270">to</span>
  <span m="725420">know.</span></p><p><span m="727760">Then</span> <span m="728000">lab</span>
  <span m="728300">tests--</span> <span m="728870">so</span> <span m="729110">this</span>
  <span m="729380">is</span> <span m="730010">the</span> <span m="730130">things</span>
  <span m="730490">that</span> <span m="731030">you</span> <span m="731720">imagine</span>
  <span m="732950">that</span> <span m="733340">we</span> <span m="733520">do</span>
  <span m="733730">a</span> <span m="733790">lot</span> <span m="734060">of,</span>
  <span m="734810">and</span> <span m="734990">these</span> <span m="735180">are</span>
  <span m="735410">components</span> <span m="736160">of</span> <span m="736310">the</span>
  <span m="736460">blood</span> <span m="736850">and</span> <span m="736970">the</span>
  <span m="737090">urine</span> <span m="737510">mainly,</span> <span m="738530">but</span>
  <span m="738770">also</span> <span m="739210">of</span> <span m="739310">the</span>
  <span m="739460">stool,</span> <span m="739880">saliva,</span> <span m="740450">spinal</span>
  <span m="740960">fluid,</span> <span m="742400">fluid</span> <span m="742880">taken</span>
  <span m="743300">off</span> <span m="743540">the</span> <span m="743690">belly,</span>
  <span m="744530">joint</span> <span m="744950">fluid,</span> <span m="745940">bone</span>
  <span m="746240">marrow,</span> <span m="747590">stuff</span> <span m="748010">coming</span>
  <span m="748400">out</span> <span m="748580">of</span> <span m="748700">your</span>
  <span m="748880">lungs.</span> <span m="750030">It's</span> <span m="750350">anything</span>
  <span m="751970">and</span> <span m="752120">any</span> <span m="752390">place</span>
  <span m="752810">where</span> <span m="753290">you</span> <span m="753470">can</span>
  <span m="753680">produce</span> <span m="754730">some</span> <span m="755480">specimen,</span>
  <span m="756590">they</span> <span m="756800">can</span> <span m="756980">send</span>
  <span m="757340">it</span> <span m="757400">to</span> <span m="757640">a</span>
  <span m="757700">lab</span> <span m="758030">and</span> <span m="758150">measure</span>
  <span m="758510">things</span> <span m="758870">in</span> <span m="758990">it,</span>
  <span m="759380">and</span> <span m="759530">they</span> <span m="759650">measure</span>
  <span m="759980">lots</span> <span m="760310">and</span> <span m="760400">lots</span>
  <span m="760670">of</span> <span m="760790">different</span> <span m="761120">kinds</span>
  <span m="761480">of</span> <span m="761570">things.</span> <span m="762600">And</span>
  <span m="762620">these</span> <span m="762830">are</span> <span m="762950">often</span>
  <span m="763280">useful.</span></p><p><span m="764660">Pathology,</span> <span m="765920">qualitative</span>
  <span m="766610">and</span> <span m="766700">quantitative</span> <span m="767390">examination</span>
  <span m="768740">of</span> <span m="768890">any</span> <span m="769175">body</span>
  <span m="769460">tissue,</span> <span m="769910">for</span> <span m="770120">example,</span>
  <span m="770600">biopsy</span> <span m="771200">samples</span> <span m="771830">or</span>
  <span m="771980">surgical</span> <span m="772520">scraps.</span> <span m="775340">You</span>
  <span m="775490">know,</span> <span m="775640">if</span> <span m="776120">they</span>
  <span m="776270">do</span> <span m="776450">an</span> <span m="776570">operation,</span>
  <span m="777290">they</span> <span m="777470">cut</span> <span m="777740">something</span>
  <span m="778190">out</span> <span m="778370">of</span> <span m="778550">you,</span>
  <span m="779150">that</span> <span m="779390">typically</span> <span m="779960">winds</span>
  <span m="780320">up</span> <span m="780530">on</span> <span m="780680">a</span>
  <span m="780740">pathologist's</span> <span m="781490">bench,</span> <span m="781765">who</span>
  <span m="782040">then</span> <span m="782300">tries</span> <span m="782630">to</span>
  <span m="782750">figure</span> <span m="783110">out</span> <span m="783740">what</span>
  <span m="783950">its</span> <span m="784100">characteristics</span> <span m="785000">are</span>
  <span m="785230">and</span> <span m="785330">that's,</span> <span m="785600">again,</span>
  <span m="785960">useful</span> <span m="786380">information.</span></p><p><span
  m="789590">Microbiology--</span> <span m="792140">ever</span> <span m="792380">since</span>
  <span m="792710">Pasteur,</span> <span m="793310">we</span> <span m="793490">know</span>
  <span m="793760">that</span> <span m="793940">organisms</span> <span m="794630">cause</span>
  <span m="794990">disease.</span> <span m="796580">And</span> <span m="797330">so</span>
  <span m="798690">we're</span> <span m="799100">quite</span> <span m="799400">interested</span>
  <span m="799970">in</span> <span m="800060">knowing</span> <span m="800480">what</span>
  <span m="800690">organisms</span> <span m="801950">are</span> <span m="802100">growing</span>
  <span m="802670">inside</span> <span m="803120">your</span> <span m="803270">body.</span>
  <span m="806480">And</span> <span m="806690">typically,</span> <span m="807530">testing</span>
  <span m="808100">is</span> <span m="808250">not</span> <span m="808490">only</span>
  <span m="808730">to</span> <span m="808940">identify</span> <span m="809570">the</span>
  <span m="809690">organism</span> <span m="810770">but</span> <span m="810980">also</span>
  <span m="811310">to</span> <span m="811490">figure</span> <span m="811820">out</span>
  <span m="812030">which</span> <span m="812270">antibiotics</span> <span m="813140">it's</span>
  <span m="813290">sensitive</span> <span m="813860">to</span> <span m="814610">and</span>
  <span m="814790">insensitive</span> <span m="815540">to.</span></p><p><span m="816260">And</span>
  <span m="816440">so</span> <span m="816650">you'll</span> <span m="816860">see</span>
  <span m="817190">things</span> <span m="817610">like</span> <span m="818600">reports</span>
  <span m="819290">of</span> <span m="819830">sensitivity</span> <span m="820580">testing</span>
  <span m="821900">at</span> <span m="822140">various</span> <span m="822620">dilutions.</span>
  <span m="824270">In</span> <span m="824420">other</span> <span m="824600">words,</span>
  <span m="825480">they</span> <span m="825590">try</span> <span m="825890">to</span>
  <span m="826160">give</span> <span m="826460">a</span> <span m="826520">strong</span>
  <span m="826970">dose</span> <span m="827300">of</span> <span m="827420">an</span>
  <span m="827540">antibiotic</span> <span m="828670">a</span> <span m="828800">week</span>
  <span m="828930">weaker</span> <span m="829190">dose</span> <span m="829610">a</span>
  <span m="829670">week</span> <span m="829870">or</span> <span m="830030">dose</span>
  <span m="830360">a</span> <span m="830420">weaker</span> <span m="830750">dose</span>
  <span m="831080">a</span> <span m="831140">week</span> <span m="831290">or</span>
  <span m="831470">dose</span> <span m="832250">to</span> <span m="832430">see</span>
  <span m="832760">which</span> <span m="833030">is</span> <span m="833210">the</span>
  <span m="833360">minimum</span> <span m="833840">level</span> <span m="834440">of</span>
  <span m="834590">dosing</span> <span m="835550">that's</span> <span m="835820">enough</span>
  <span m="836120">to</span> <span m="836240">kill</span> <span m="836540">the</span>
  <span m="836810">bacteria.</span></p><p><span m="838220">There's</span> <span m="838430">a</span>
  <span m="838490">comma</span> <span m="838880">missing</span> <span m="839300">there,</span>
  <span m="839540">but</span> <span m="840080">input,</span> <span m="840470">output</span>
  <span m="840860">of</span> <span m="840950">fluids</span> <span m="841580">is</span>
  <span m="841790">another</span> <span m="842150">important</span> <span m="842690">thing</span>
  <span m="843980">because</span> <span m="845180">people,</span> <span m="845810">especially</span>
  <span m="846380">in</span> <span m="846500">the</span> <span m="846560">hospital,</span>
  <span m="848060">often</span> <span m="848510">get</span> <span m="848900">either</span>
  <span m="849200">dehydrated</span> <span m="850100">or</span> <span m="850610">over</span>
  <span m="850940">hydrated.</span> <span m="851990">And</span> <span m="852140">neither</span>
  <span m="852500">of</span> <span m="852620">those</span> <span m="852950">is</span>
  <span m="853070">good</span> <span m="853280">for</span> <span m="853580">you,</span>
  <span m="853790">and</span> <span m="853940">so</span> <span m="854180">trying</span>
  <span m="854480">to</span> <span m="854600">keep</span> <span m="854900">track</span>
  <span m="855740">of</span> <span m="855920">what's</span> <span m="856190">going</span>
  <span m="856490">into</span> <span m="856760">you</span> <span m="856940">and</span>
  <span m="857060">what's</span> <span m="857270">coming</span> <span m="857630">out</span>
  <span m="857810">of</span> <span m="857930">you</span> <span m="858110">is</span>
  <span m="858260">important.</span></p><p><span m="860990">Then</span> <span m="861230">there</span>
  <span m="861350">are</span> <span m="861440">tons</span> <span m="861830">of</span>
  <span m="861950">notes.</span> <span m="862740">So</span> <span m="864380">an</span>
  <span m="864500">important</span> <span m="865070">one</span> <span m="865340">that</span>
  <span m="865580">we're</span> <span m="865730">going</span> <span m="865850">to</span>
  <span m="865910">look</span> <span m="866150">at</span> <span m="866330">in</span>
  <span m="866420">this</span> <span m="866630">class</span> <span m="866960">is</span>
  <span m="867180">discharge</span> <span m="867610">summaries.</span> <span m="868700">So</span>
  <span m="868940">these</span> <span m="869290">are</span> <span m="869430">the</span>
  <span m="869570">typically</span> <span m="870200">long</span> <span m="870650">notes</span>
  <span m="871640">that</span> <span m="871880">are</span> <span m="871970">written</span>
  <span m="872450">at</span> <span m="872690">the</span> <span m="872840">end</span>
  <span m="873050">of</span> <span m="873140">a</span> <span m="873200">hospitalization.</span>
  <span m="875390">So</span> <span m="875570">this</span> <span m="875840">is</span>
  <span m="875990">a</span> <span m="876050">summary</span> <span m="877220">of</span>
  <span m="878000">why</span> <span m="878330">you</span> <span m="878480">came</span>
  <span m="878870">in,</span> <span m="879620">what</span> <span m="879890">they</span>
  <span m="880070">did</span> <span m="880340">to</span> <span m="880670">you,</span>
  <span m="881570">the</span> <span m="882050">main</span> <span m="882770">things</span>
  <span m="883160">they</span> <span m="883340">discovered</span> <span m="883940">about</span>
  <span m="884330">you,</span> <span m="885410">and</span> <span m="885680">then</span>
  <span m="885920">plans</span> <span m="886490">for</span> <span m="886730">what</span>
  <span m="886970">to</span> <span m="887090">do</span> <span m="887360">after</span>
  <span m="887660">your</span> <span m="887830">discharge.</span> <span m="888470">Where</span>
  <span m="888710">are</span> <span m="888740">you</span> <span m="888890">going</span>
  <span m="889010">to</span> <span m="889100">go?</span> <span m="890340">What</span>
  <span m="890510">drugs</span> <span m="890870">are</span> <span m="890990">you</span>
  <span m="891080">going</span> <span m="891200">to</span> <span m="891260">be</span>
  <span m="891410">taking?</span> <span m="892250">When</span> <span m="892490">are</span>
  <span m="892610">you</span> <span m="892730">supposed</span> <span m="893060">to</span>
  <span m="893150">come</span> <span m="893390">back</span> <span m="893660">for</span>
  <span m="893840">follow</span> <span m="894260">up,</span> <span m="894540">et</span>
  <span m="894700">cetera.</span> <span m="895650">I'll</span> <span m="895670">show</span>
  <span m="895940">you</span> <span m="896180">an</span> <span m="896510">excruciatingly</span>
  <span m="897590">long</span> <span m="897950">one</span> <span m="898100">of</span>
  <span m="898220">those</span> <span m="898850">later</span> <span m="899240">in</span>
  <span m="899360">the</span> <span m="899900">lecture</span> <span m="900260">today.</span></p><p><span
  m="901650">But</span> <span m="901820">we</span> <span m="901970">also</span> <span
  m="902300">have</span> <span m="902510">notes</span> <span m="902900">from</span>
  <span m="903170">attendings</span> <span m="903740">and/or</span> <span m="904010">residents,</span>
  <span m="904760">nurses,</span> <span m="905810">various</span> <span m="906200">specialties,</span>
  <span m="907580">consultants.</span> <span m="908990">The</span> <span m="909140">referring</span>
  <span m="909650">physician--</span> <span m="910220">if</span> <span m="910340">somebody</span>
  <span m="910760">sends</span> <span m="911210">you</span> <span m="911390">to</span>
  <span m="911570">the</span> <span m="911690">hospital,</span> <span m="912890">that</span>
  <span m="913130">doctor</span> <span m="913640">will</span> <span m="913850">usually</span>
  <span m="914360">write</span> <span m="914630">a</span> <span m="914690">note</span>
  <span m="915110">saying</span> <span m="915780">this</span> <span m="915980">is</span>
  <span m="916130">what</span> <span m="916310">I'm</span> <span m="916490">interested</span>
  <span m="917000">in.</span> <span m="917310">Here's</span> <span m="917510">why</span>
  <span m="917810">I'm</span> <span m="918320">sending</span> <span m="918740">in</span>
  <span m="918890">the</span> <span m="918980">patient.</span> <span m="920110">There</span>
  <span m="920360">are</span> <span m="920420">letters</span> <span m="920870">back</span>
  <span m="921260">to</span> <span m="921530">the</span> <span m="921680">referring</span>
  <span m="922220">physician</span> <span m="922850">saying,</span> <span m="923370">OK,</span>
  <span m="924090">this</span> <span m="924260">is</span> <span m="924410">what</span>
  <span m="924620">we</span> <span m="924770">found</span> <span m="925160">out.</span>
  <span m="925460">Here's</span> <span m="925760">the</span> <span m="925910">answer</span>
  <span m="926660">to</span> <span m="926780">the</span> <span m="926900">question</span>
  <span m="927350">you</span> <span m="927440">were</span> <span m="927620">asking.</span>
  <span m="928810">There</span> <span m="928935">are</span> <span m="929060">emergency</span>
  <span m="929650">department</span> <span m="930310">notes.</span> <span m="930820">So</span>
  <span m="930970">that's</span> <span m="931240">often</span> <span m="931600">the</span>
  <span m="931690">first</span> <span m="932080">contact</span> <span m="933130">between</span>
  <span m="933730">the</span> <span m="933850">patient</span> <span m="934450">and</span>
  <span m="934630">the</span> <span m="934690">health</span> <span m="934830">care</span>
  <span m="935140">system.</span> <span m="936410">So</span> <span m="936490">these</span>
  <span m="936730">are</span> <span m="936880">all</span> <span m="937090">important.</span></p><p><span
  m="938620">And</span> <span m="938800">then</span> <span m="940690">there's</span>
  <span m="941020">tons</span> <span m="941380">and</span> <span m="941500">tons</span>
  <span m="941890">of</span> <span m="942010">billing</span> <span m="942370">data.</span>
  <span m="943300">So</span> <span m="943510">remember</span> <span m="944590">the</span>
  <span m="945130">EHR</span> <span m="945640">systems</span> <span m="946780">were</span>
  <span m="948010">initially</span> <span m="948610">designed</span> <span m="949240">by</span>
  <span m="949660">accountants.</span> <span m="951550">And</span> <span m="951760">they</span>
  <span m="951910">were</span> <span m="952060">designed</span> <span m="952570">for</span>
  <span m="952780">the</span> <span m="952900">purpose</span> <span m="953350">of</span>
  <span m="953440">billing.</span> <span m="954520">And</span> <span m="954730">so</span>
  <span m="955000">we</span> <span m="955180">capture</span> <span m="955750">a</span>
  <span m="955840">lot</span> <span m="956110">of</span> <span m="956230">data</span>
  <span m="957190">about</span> <span m="957550">formalized</span> <span m="958390">ways</span>
  <span m="958810">of</span> <span m="958960">describing</span> <span m="960190">the</span>
  <span m="960310">condition</span> <span m="960820">of</span> <span m="960940">the</span>
  <span m="961060">patient</span> <span m="961730">and</span> <span m="961780">what</span>
  <span m="961990">was</span> <span m="962200">done</span> <span m="962440">to</span>
  <span m="962560">the</span> <span m="962680">patient</span> <span m="964060">in</span>
  <span m="964270">order</span> <span m="964540">to</span> <span m="965050">submit</span>
  <span m="965500">the</span> <span m="965620">right</span> <span m="965890">bills.</span></p><p><span
  m="967720">You</span> <span m="968860">obviously</span> <span m="969460">want</span>
  <span m="969650">to</span> <span m="969730">bill</span> <span m="970030">through</span>
  <span m="970300">it</span> <span m="970570">as</span> <span m="970720">much</span>
  <span m="970990">as</span> <span m="971140">possible.</span> <span m="972320">But</span>
  <span m="972520">you</span> <span m="972610">have</span> <span m="972790">to</span>
  <span m="972910">be</span> <span m="973060">able</span> <span m="973270">to</span>
  <span m="973420">justify</span> <span m="974020">the</span> <span m="974140">bills</span>
  <span m="974500">that</span> <span m="974740">you</span> <span m="974830">submit</span>
  <span m="975850">because</span> <span m="976630">insurance</span> <span m="977170">companies</span>
  <span m="977830">and</span> <span m="978040">Medicare</span> <span m="978610">and</span>
  <span m="979150">Medicaid</span> <span m="980800">don't</span> <span m="981100">have</span>
  <span m="981280">a</span> <span m="981340">good</span> <span m="981520">sense</span>
  <span m="981850">of</span> <span m="981940">humor.</span> <span m="983112">And</span>
  <span m="983500">if</span> <span m="983710">you</span> <span m="983830">submit</span>
  <span m="984340">bills</span> <span m="984760">for</span> <span m="984940">things</span>
  <span m="985270">that</span> <span m="985510">you</span> <span m="985630">can't</span>
  <span m="985900">justify,</span> <span m="987040">then</span> <span m="987220">you</span>
  <span m="987340">get</span> <span m="987520">penalized.</span></p><p><span m="991690">And</span>
  <span m="991870">then</span> <span m="992050">there</span> <span m="992230">are</span>
  <span m="992410">administrative</span> <span m="993250">data</span> <span m="993610">like,</span>
  <span m="994240">which</span> <span m="994510">service</span> <span m="995080">are</span>
  <span m="995200">you</span> <span m="995440">on?</span> <span m="996100">So</span>
  <span m="996310">this</span> <span m="996670">this</span> <span m="996970">is</span>
  <span m="997540">occasionally</span> <span m="998260">a</span> <span m="998320">confusing</span>
  <span m="999010">thing.</span> <span m="1000300">You</span> <span m="1000540">can</span>
  <span m="1000750">go</span> <span m="1000960">into</span> <span m="1001200">the</span>
  <span m="1001320">hospital</span> <span m="1002070">and</span> <span m="1002400">have</span>
  <span m="1002640">heart</span> <span m="1002910">problems,</span> <span m="1003990">but</span>
  <span m="1004200">it</span> <span m="1004290">turns</span> <span m="1004650">out</span>
  <span m="1004890">that</span> <span m="1005130">the</span> <span m="1005490">heart</span>
  <span m="1005910">intensive</span> <span m="1006480">care</span> <span m="1006750">unit,</span>
  <span m="1007050">the</span> <span m="1007170">cardiac</span> <span m="1007710">intensive</span>
  <span m="1008190">care</span> <span m="1008460">unit,</span> <span m="1009210">is</span>
  <span m="1009390">full</span> <span m="1009690">up</span> <span m="1010080">with</span>
  <span m="1010260">patients.</span> <span m="1011400">But</span> <span m="1011640">there's</span>
  <span m="1011910">an</span> <span m="1012000">extra</span> <span m="1012390">bed</span>
  <span m="1012900">in</span> <span m="1013140">the</span> <span m="1013830">pulmonary</span>
  <span m="1014490">intensive</span> <span m="1015030">care</span> <span m="1015270">unit,</span>
  <span m="1016110">and</span> <span m="1016260">so</span> <span m="1016470">they</span>
  <span m="1016650">stick</span> <span m="1017010">you</span> <span m="1017190">in</span>
  <span m="1017310">that</span> <span m="1017760">unit,</span> <span m="1018790">but</span>
  <span m="1018960">you're</span> <span m="1019140">still</span> <span m="1019500">on</span>
  <span m="1019680">the</span> <span m="1019770">cardiology</span> <span m="1020550">service.</span>
  <span m="1021300">And</span> <span m="1021450">so</span> <span m="1021690">there</span>
  <span m="1021930">are</span> <span m="1021990">these</span> <span m="1022740">sort</span>
  <span m="1022950">of</span> <span m="1023100">mixture</span> <span m="1023730">kinds</span>
  <span m="1024089">of</span> <span m="1024210">cases</span> <span m="1024780">that</span>
  <span m="1025020">you</span> <span m="1025140">still</span> <span m="1025410">have</span>
  <span m="1025560">to</span> <span m="1025680">take</span> <span m="1025890">care</span>
  <span m="1026190">of.</span> <span m="1026700">Transfers</span> <span m="1027450">are</span>
  <span m="1027690">when</span> <span m="1027930">you</span> <span m="1028020">get</span>
  <span m="1028200">transferred</span> <span m="1028829">from</span> <span m="1029099">one</span>
  <span m="1029310">place</span> <span m="1029579">to</span> <span m="1029760">another</span>
  <span m="1030119">in</span> <span m="1030270">the</span> <span m="1030359">hospital.</span></p><p><span
  m="1033119">Imaging</span> <span m="1033569">data--</span> <span m="1034599">so</span>
  <span m="1035280">I'm</span> <span m="1035400">not</span> <span m="1035550">going</span>
  <span m="1035700">to</span> <span m="1035790">talk</span> <span m="1036060">about</span>
  <span m="1036329">that</span> <span m="1036569">much</span> <span m="1036930">today,</span>
  <span m="1037890">but</span> <span m="1038130">there</span> <span m="1038339">are</span>
  <span m="1038460">X-rays,</span> <span m="1039030">ultrasound,</span> <span m="1040829">CT,</span>
  <span m="1041460">MRI,</span> <span m="1042030">PET</span> <span m="1042329">scans,</span>
  <span m="1043410">retinal</span> <span m="1043950">scans,</span> <span m="1044670">endoscopy,</span>
  <span m="1045660">photographs</span> <span m="1046650">of</span> <span m="1047040">your</span>
  <span m="1047190">skin</span> <span m="1047760">and</span> <span m="1047849">stuff</span>
  <span m="1048180">like</span> <span m="1048390">that.</span> <span m="1048790">So</span>
  <span m="1048900">this</span> <span m="1049140">is</span> <span m="1049710">all</span>
  <span m="1049960">imaging</span> <span m="1050430">data,</span> <span m="1051270">and</span>
  <span m="1051450">there's</span> <span m="1051750">been</span> <span m="1051930">a</span>
  <span m="1051990">tremendous</span> <span m="1052590">amount</span> <span m="1052830">of</span>
  <span m="1052950">progress</span> <span m="1053550">recently</span> <span m="1054660">in</span>
  <span m="1054840">applying</span> <span m="1055290">machine</span> <span m="1055650">learning</span>
  <span m="1055980">techniques</span> <span m="1056610">to</span> <span m="1056730">try</span>
  <span m="1056970">to</span> <span m="1057120">interpret</span> <span m="1058080">the</span>
  <span m="1058200">contents</span> <span m="1058800">of</span> <span m="1058950">these</span>
  <span m="1059190">data.</span> <span m="1059590">So</span> <span m="1059700">these</span>
  <span m="1059970">are</span> <span m="1060090">also</span> <span m="1060390">very</span>
  <span m="1060690">important.</span></p><p><span m="1062590">And</span> <span m="1062670">then</span>
  <span m="1063720">there's</span> <span m="1064050">the</span> <span m="1064170">whole</span>
  <span m="1064410">quantified</span> <span m="1065100">self</span> <span m="1065520">movement.</span>
  <span m="1067170">I</span> <span m="1067200">mean,</span> <span m="1067440">how</span>
  <span m="1067620">many</span> <span m="1067860">of</span> <span m="1067980">you</span>
  <span m="1068100">where</span> <span m="1068430">an</span> <span m="1069420">activity</span>
  <span m="1069930">tracker?</span> <span m="1072900">Only</span> <span m="1073170">about</span>
  <span m="1073470">1/3?</span> <span m="1074520">I'm</span> <span m="1074850">surprised</span>
  <span m="1075450">at</span> <span m="1075790">a</span> <span m="1075870">place</span>
  <span m="1076170">like</span> <span m="1076410">MIT.</span></p><p><span m="1076980">[LAUGHTER]</span></p><p><span
  m="1078900">So</span> <span m="1079290">you</span> <span m="1079440">know,</span>
  <span m="1079620">we</span> <span m="1079800">measure</span> <span m="1081090">steps</span>
  <span m="1081630">and</span> <span m="1081750">elevation</span> <span m="1082320">change</span>
  <span m="1082740">and</span> <span m="1082860">workouts.</span> <span m="1083590">And</span>
  <span m="1084150">you</span> <span m="1084270">can</span> <span m="1084450">record</span>
  <span m="1084900">vital</span> <span m="1085260">signs</span> <span m="1086340">and</span>
  <span m="1087450">diet</span> <span m="1088140">and</span> <span m="1088710">your</span>
  <span m="1088950">blood</span> <span m="1089250">sugar,</span> <span m="1089970">especially</span>
  <span m="1090600">if</span> <span m="1090720">you're</span> <span m="1090870">diabetic;</span>
  <span m="1092040">allergies,</span> <span m="1093360">allergic</span> <span m="1095100">incidents.</span>
  <span m="1096710">There's</span> <span m="1097230">all</span> <span m="1097440">this</span>
  <span m="1097650">mindfulness,</span> <span m="1098670">mood,</span> <span m="1099030">sleep,</span>
  <span m="1099450">pain,</span> <span m="1100380">sexual</span> <span m="1100980">activity.</span></p><p><span
  m="1102180">And</span> <span m="1102360">then</span> <span m="1102720">people</span>
  <span m="1103110">have</span> <span m="1103320">developed</span> <span m="1103830">this</span>
  <span m="1104040">idea</span> <span m="1104520">of</span> <span m="1104680">N</span>
  <span m="1104850">of</span> <span m="1105000">1</span> <span m="1105210">experiments.</span>
  <span m="1107340">For</span> <span m="1107580">example,</span> <span m="1108060">I</span>
  <span m="1108180">had</span> <span m="1108390">a</span> <span m="1108450">student</span>
  <span m="1109230">some</span> <span m="1109500">years</span> <span m="1109800">ago</span>
  <span m="1110550">who</span> <span m="1110880">suffered</span> <span m="1111330">from</span>
  <span m="1111600">psoriasis.</span> <span m="1113490">It's</span> <span m="1113730">a</span>
  <span m="1114570">grody</span> <span m="1114930">condition</span> <span m="1115500">of</span>
  <span m="1115620">the</span> <span m="1115740">skin.</span> <span m="1116730">And</span>
  <span m="1116880">the</span> <span m="1116970">problem</span> <span m="1117390">is</span>
  <span m="1117600">there</span> <span m="1117690">are</span> <span m="1117750">no</span>
  <span m="1117990">good</span> <span m="1118200">cures</span> <span m="1118650">for</span>
  <span m="1118950">it.</span> <span m="1119160">And</span> <span m="1119310">so</span>
  <span m="1119730">people</span> <span m="1120150">who</span> <span m="1120240">suffer</span>
  <span m="1120660">from</span> <span m="1120900">psoriasis</span> <span m="1122130">try</span>
  <span m="1122520">all</span> <span m="1122700">kinds</span> <span m="1123060">of</span>
  <span m="1123180">things.</span> <span m="1123750">You</span> <span m="1123900">know,</span>
  <span m="1124090">they</span> <span m="1124440">stop</span> <span m="1124830">eating</span>
  <span m="1125130">nonce</span> <span m="1125490">for</span> <span m="1125700">a</span>
  <span m="1125760">while,</span> <span m="1126210">or</span> <span m="1126360">they</span>
  <span m="1127320">douse</span> <span m="1127710">themselves</span> <span m="1128340">with</span>
  <span m="1128550">vinegar.</span> <span m="1129120">Or</span> <span m="1129330">they</span>
  <span m="1129540">do</span> <span m="1130770">whatever</span> <span m="1131190">crazy</span>
  <span m="1131640">thing</span> <span m="1131880">comes</span> <span m="1132210">to</span>
  <span m="1132300">mind.</span> <span m="1134040">And</span> <span m="1134520">we</span>
  <span m="1134730">don't</span> <span m="1135030">have</span> <span m="1135270">a</span>
  <span m="1135330">good</span> <span m="1135570">theory</span> <span m="1136050">for</span>
  <span m="1136290">how</span> <span m="1136440">to</span> <span m="1136560">treat</span>
  <span m="1136830">this</span> <span m="1137070">disease.</span></p><p><span m="1137970">But</span>
  <span m="1138210">on</span> <span m="1138300">the</span> <span m="1138420">other</span>
  <span m="1138630">hand,</span> <span m="1139000">some</span> <span m="1139170">things</span>
  <span m="1139530">work</span> <span m="1139800">for</span> <span m="1139950">some</span>
  <span m="1140190">people.</span> <span m="1141280">And</span> <span m="1141330">so</span>
  <span m="1141570">there's</span> <span m="1141810">a</span> <span m="1141870">whole</span>
  <span m="1142350">methodology</span> <span m="1143220">that</span> <span m="1143460">has</span>
  <span m="1143610">been</span> <span m="1143790">developed</span> <span m="1144270">that</span>
  <span m="1144450">says,</span> <span m="1144780">when</span> <span m="1144990">you</span>
  <span m="1145110">try</span> <span m="1145440">these</span> <span m="1145710">things,</span>
  <span m="1146820">act</span> <span m="1147060">like</span> <span m="1147330">a</span>
  <span m="1147360">scientist.</span> <span m="1148770">Have</span> <span m="1149040">hypotheses.</span>
  <span m="1150360">Take</span> <span m="1150600">good</span> <span m="1150840">notes.</span>
  <span m="1151320">Collect</span> <span m="1151710">good</span> <span m="1151950">data.</span>
  <span m="1154380">Be</span> <span m="1154710">cognizant</span> <span m="1155520">of</span>
  <span m="1155670">things</span> <span m="1156000">like</span> <span m="1156300">onset</span>
  <span m="1156750">periods,</span> <span m="1157800">where</span> <span m="1158040">you</span>
  <span m="1158160">know</span> <span m="1158310">you</span> <span m="1158460">may</span>
  <span m="1158640">have</span> <span m="1158850">to</span> <span m="1159000">drip</span>
  <span m="1159450">vinegar</span> <span m="1159930">on</span> <span m="1160050">yourself</span>
  <span m="1160530">for</span> <span m="1160770">a</span> <span m="1160830">week</span>
  <span m="1161190">before</span> <span m="1161610">you</span> <span m="1161730">see</span>
  <span m="1162000">any</span> <span m="1162240">effect.</span> <span m="1163270">So</span>
  <span m="1163410">if</span> <span m="1163540">that</span> <span m="1163620">doesn't</span>
  <span m="1163950">do</span> <span m="1164130">a</span> <span m="1164250">thing</span>
  <span m="1164580">after</span> <span m="1164910">one</span> <span m="1165180">day,</span>
  <span m="1165510">don't</span> <span m="1165780">stop.</span> <span m="1166890">And</span>
  <span m="1167190">furthermore,</span> <span m="1168060">if</span> <span m="1168270">you</span>
  <span m="1168390">stop</span> <span m="1169380">then</span> <span m="1169710">don't</span>
  <span m="1170010">start</span> <span m="1170430">something</span> <span m="1170910">new</span>
  <span m="1171510">immediately</span> <span m="1172260">because</span> <span m="1174030">you</span>
  <span m="1174990">will</span> <span m="1175260">then</span> <span m="1175470">be</span>
  <span m="1175620">confused</span> <span m="1176340">about</span> <span m="1177120">whether</span>
  <span m="1177480">this</span> <span m="1177780">is</span> <span m="1177930">the</span>
  <span m="1178110">effect</span> <span m="1178530">of</span> <span m="1178650">the</span>
  <span m="1178770">thing</span> <span m="1179010">you</span> <span m="1179130">were</span>
  <span m="1179550">on</span> <span m="1179760">before</span> <span m="1180330">or</span>
  <span m="1180480">the</span> <span m="1180660">new</span> <span m="1180870">thing</span>
  <span m="1181110">that</span> <span m="1181320">you're</span> <span m="1181440">trying.</span>
  <span m="1182250">So</span> <span m="1182430">there's</span> <span m="1182670">all</span>
  <span m="1182790">sorts</span> <span m="1183150">of</span> <span m="1183300">ideas</span>
  <span m="1183750">like</span> <span m="1183990">that.</span></p><p><span m="1186480">So</span>
  <span m="1186660">this</span> <span m="1186930">is</span> <span m="1187110">a</span>
  <span m="1187170">slide</span> <span m="1187680">from</span> <span m="1188010">our</span>
  <span m="1188250">paper</span> <span m="1188790">on</span> <span m="1189270">MIMIC-III.</span>
  <span m="1190740">And</span> <span m="1191040">it</span> <span m="1191250">gives</span>
  <span m="1191610">you</span> <span m="1192090">a</span> <span m="1192180">kind</span>
  <span m="1192510">of</span> <span m="1192720">overview</span> <span m="1193650">of</span>
  <span m="1194070">what's</span> <span m="1194370">going</span> <span m="1194730">on</span>
  <span m="1194910">with</span> <span m="1195090">the</span> <span m="1195180">patient.</span>
  <span m="1196390">So</span> <span m="1196530">if</span> <span m="1196650">you</span>
  <span m="1196770">look</span> <span m="1196980">at</span> <span m="1197130">this--</span>
  <span m="1199210">I'm</span> <span m="1199310">going</span> <span m="1199320">to</span>
  <span m="1199410">point</span> <span m="1199770">with</span> <span m="1199950">my</span>
  <span m="1200160">hands--</span> <span m="1201570">at</span> <span m="1201780">the</span>
  <span m="1201900">top</span> <span m="1202620">is</span> <span m="1202830">something</span>
  <span m="1203250">very</span> <span m="1203550">important.</span> <span m="1204150">This</span>
  <span m="1204390">patient</span> <span m="1204840">starts</span> <span m="1205350">off</span>
  <span m="1206130">at</span> <span m="1206280">full</span> <span m="1206580">code.</span>
  <span m="1207640">That</span> <span m="1207750">means</span> <span m="1208140">that</span>
  <span m="1208350">if</span> <span m="1208770">something</span> <span m="1209220">bad</span>
  <span m="1209520">happens</span> <span m="1210030">to</span> <span m="1210240">him,</span>
  <span m="1211390">he</span> <span m="1211500">wants</span> <span m="1212130">everything</span>
  <span m="1212640">to</span> <span m="1212790">be</span> <span m="1212970">done</span>
  <span m="1213240">to</span> <span m="1213420">try</span> <span m="1213660">to</span>
  <span m="1213750">save</span> <span m="1214080">him.</span> <span m="1215340">And</span>
  <span m="1215580">he</span> <span m="1215730">winds</span> <span m="1216120">up</span>
  <span m="1216330">in</span> <span m="1216480">comfort</span> <span m="1216990">measures</span>
  <span m="1217470">only,</span> <span m="1218560">which</span> <span m="1218760">means</span>
  <span m="1219120">that</span> <span m="1219360">if</span> <span m="1219480">something</span>
  <span m="1219900">bad</span> <span m="1220170">happens</span> <span m="1220680">to</span>
  <span m="1220830">him,</span> <span m="1221110">he</span> <span m="1221210">wants</span>
  <span m="1221400">to</span> <span m="1221550">die--</span> <span m="1223350">or</span>
  <span m="1223560">his</span> <span m="1223770">family</span> <span m="1224190">does</span>
  <span m="1224580">if</span> <span m="1225210">he's</span> <span m="1225510">unconscious.</span></p><p><span
  m="1228360">So</span> <span m="1228880">what</span> <span m="1229030">else</span>
  <span m="1229270">do</span> <span m="1229390">we</span> <span m="1229540">know</span>
  <span m="1229810">about</span> <span m="1230080">this</span> <span m="1230290">guy?</span>
  <span m="1230560">Well</span> <span m="1231430">GCS</span> <span m="1232220">is</span>
  <span m="1232420">the</span> <span m="1232540">Glasgow</span> <span m="1233170">Coma</span>
  <span m="1233590">Score.</span> <span m="1234730">And</span> <span m="1235060">it's</span>
  <span m="1235360">a</span> <span m="1235420">way</span> <span m="1235660">of</span>
  <span m="1235810">quantifying</span> <span m="1237250">people's</span> <span m="1237730">level</span>
  <span m="1238090">of</span> <span m="1238240">consciousness.</span> <span m="1239620">And</span>
  <span m="1239830">you</span> <span m="1239980">see</span> <span m="1240310">that</span>
  <span m="1242380">at</span> <span m="1242560">the</span> <span m="1242680">beginning</span>
  <span m="1243310">this</span> <span m="1243550">patient</span> <span m="1244090">is</span>
  <span m="1244270">oriented,</span> <span m="1245720">and</span> <span m="1245800">then</span>
  <span m="1246010">gets</span> <span m="1246280">confused.</span> <span m="1247120">And</span>
  <span m="1247720">finally,</span> <span m="1248230">is</span> <span m="1248470">only</span>
  <span m="1248770">making</span> <span m="1249220">incomprehensible</span> <span
  m="1250240">words</span> <span m="1251410">or</span> <span m="1251980">sounds.</span>
  <span m="1253980">Motor,</span> <span m="1254900">he's</span> <span m="1255160">able</span>
  <span m="1255460">to</span> <span m="1255640">obey</span> <span m="1256000">commands.</span>
  <span m="1257590">Eventually,</span> <span m="1258760">he's</span> <span m="1259360">only</span>
  <span m="1259720">able</span> <span m="1260080">to</span> <span m="1260890">flex</span>
  <span m="1261610">when</span> <span m="1261880">you</span> <span m="1262090">stimulate</span>
  <span m="1262720">his</span> <span m="1262870">muscles.</span> <span m="1263560">So</span>
  <span m="1263860">he's</span> <span m="1264010">no</span> <span m="1264220">longer</span>
  <span m="1265060">conscious.</span></p><p><span m="1266970">Eye</span> <span m="1267450">movements--</span>
  <span m="1269090">he's</span> <span m="1269350">able</span> <span m="1269650">to</span>
  <span m="1269800">follow</span> <span m="1270190">you</span> <span m="1270340">spontaneously.</span>
  <span m="1271900">He's</span> <span m="1272140">able</span> <span m="1272410">to</span>
  <span m="1272530">orient</span> <span m="1272950">to</span> <span m="1273100">speech.</span>
  <span m="1274000">And</span> <span m="1274180">eventually</span> <span m="1274720">orientation</span>
  <span m="1275740">at</span> <span m="1275860">all.</span> <span m="1276200">So</span>
  <span m="1276280">this</span> <span m="1276520">is</span> <span m="1277060">clearly</span>
  <span m="1277420">somebody</span> <span m="1277930">who's</span> <span m="1278170">going</span>
  <span m="1278440">downhill</span> <span m="1279610">quickly</span> <span m="1280700">and,</span>
  <span m="1280750">in</span> <span m="1280870">fact,</span> <span m="1281200">dies</span>
  <span m="1281770">at</span> <span m="1281920">the</span> <span m="1282070">end</span>
  <span m="1282280">of</span> <span m="1282710">this</span> <span m="1283000">episode.</span></p><p><span
  m="1285160">Now,</span> <span m="1285910">we</span> <span m="1286090">then</span>
  <span m="1286330">look</span> <span m="1286630">at</span> <span m="1286780">labs</span>
  <span m="1287620">so</span> <span m="1287860">we</span> <span m="1288010">can</span>
  <span m="1288220">see</span> <span m="1289450">what</span> <span m="1289690">is</span>
  <span m="1289840">their</span> <span m="1290020">level</span> <span m="1290350">of</span>
  <span m="1290470">platelets</span> <span m="1291190">at</span> <span m="1291460">about</span>
  <span m="1291790">the</span> <span m="1291940">time</span> <span m="1292240">that</span>
  <span m="1292420">they're</span> <span m="1292600">measured,</span> <span m="1293560">their</span>
  <span m="1293740">creatinine</span> <span m="1294460">level,</span> <span m="1295000">their</span>
  <span m="1295210">white</span> <span m="1295480">blood</span> <span m="1295750">cell</span>
  <span m="1296050">count,</span> <span m="1297040">the</span> <span m="1297310">neutrophils</span>
  <span m="1297940">percentage,</span> <span m="1298670">et</span> <span m="1298970">cetera.</span>
  <span m="1300220">And</span> <span m="1300580">there's</span> <span m="1300820">not</span>
  <span m="1301090">every</span> <span m="1301450">possible</span> <span m="1302950">data</span>
  <span m="1303250">point</span> <span m="1303640">on</span> <span m="1303820">the</span>
  <span m="1303910">slide.</span> <span m="1304450">This</span> <span m="1304660">is</span>
  <span m="1304810">just</span> <span m="1305080">illustrative.</span></p><p><span
  m="1307150">The</span> <span m="1307240">next</span> <span m="1307510">section</span>
  <span m="1307960">is</span> <span m="1308140">medications.</span> <span m="1309590">So</span>
  <span m="1309670">the</span> <span m="1309790">person</span> <span m="1310240">is</span>
  <span m="1310390">on</span> <span m="1310570">morphine.</span> <span m="1311920">They're</span>
  <span m="1312100">on</span> <span m="1312280">Vancomycin,</span> <span m="1313220">which</span>
  <span m="1313360">is</span> <span m="1313480">an</span> <span m="1313600">antibiotic.</span>
  <span m="1315330">Piperacillin--</span> <span m="1316330">I</span> <span m="1316420">don't</span>
  <span m="1316600">know</span> <span m="1316780">what</span> <span m="1316960">that</span>
  <span m="1317170">is.</span> <span m="1317440">Does</span> <span m="1317710">somebody</span>
  <span m="1318170">know?</span></p><p><span m="1318842">AUDIENCE:</span> <span m="1319083">Antibiotic.</span></p><p><span
  m="1320288">PETER SZOLOVITS:</span> <span m="1320529">It's</span> <span m="1320770">what?</span></p><p><span
  m="1321463">AUDIENCE:</span> <span m="1321689">It's</span> <span m="1321916">antibiotic.</span></p><p><span
  m="1322822">PETER SZOLOVITS:</span> <span m="1323048">OK.</span> <span m="1325090">Sodium</span>
  <span m="1325570">chloride</span> <span m="1326080">9%,</span> <span m="1326830">So</span>
  <span m="1327010">that's</span> <span m="1327310">just</span> <span m="1327520">keeping</span>
  <span m="1327910">him</span> <span m="1328030">hydrated.</span> <span m="1329210">Amiodarone</span>
  <span m="1330460">and</span> <span m="1330610">dextrose.</span> <span m="1331310">So</span>
  <span m="1331510">dextrose</span> <span m="1332140">is</span> <span m="1332830">giving</span>
  <span m="1333160">him</span> <span m="1333280">some</span> <span m="1333550">energy.</span></p><p><span
  m="1334480">And</span> <span m="1334630">then</span> <span m="1334870">these</span>
  <span m="1335260">are</span> <span m="1335530">the</span> <span m="1335680">various</span>
  <span m="1336190">measurements.</span> <span m="1338030">So</span> <span m="1338170">you</span>
  <span m="1338320">see</span> <span m="1338560">the</span> <span m="1338680">heart</span>
  <span m="1339010">rate,</span> <span m="1339410">for</span> <span m="1339520">example,</span>
  <span m="1340730">is</span> <span m="1341080">up</span> <span m="1341260">pretty</span>
  <span m="1341590">high</span> <span m="1342010">and</span> <span m="1342190">is</span>
  <span m="1342370">going</span> <span m="1342790">up</span> <span m="1343140">near</span>
  <span m="1343340">the</span> <span m="1343540">end.</span> <span m="1344290">The</span>
  <span m="1344470">oxygen</span> <span m="1345040">saturation</span> <span m="1346360">starts</span>
  <span m="1346930">off</span> <span m="1347200">pretty</span> <span m="1347500">good.</span>
  <span m="1348310">But</span> <span m="1348580">here</span> <span m="1349240">we're</span>
  <span m="1349510">down</span> <span m="1349870">to</span> <span m="1350690">60%</span>
  <span m="1352030">or</span> <span m="1352150">50%</span> <span m="1353540">O2</span>
  <span m="1353890">sat,</span> <span m="1354340">which</span> <span m="1354580">is</span>
  <span m="1354700">supposed</span> <span m="1355060">to</span> <span m="1355150">be</span>
  <span m="1355330">above</span> <span m="1355720">about</span> <span m="1356140">92</span>
  <span m="1357640">in</span> <span m="1357880">order</span> <span m="1358150">to</span>
  <span m="1358330">be</span> <span m="1358450">considered</span> <span m="1359050">reasonable.</span>
  <span m="1360100">So</span> <span m="1360610">again,</span> <span m="1361000">this</span>
  <span m="1361210">is</span> <span m="1361360">a</span> <span m="1361390">very</span>
  <span m="1361630">consistent</span> <span m="1362260">picture</span> <span m="1362770">of</span>
  <span m="1362920">things</span> <span m="1363250">going</span> <span m="1363610">very</span>
  <span m="1363880">badly</span> <span m="1364330">wrong</span> <span m="1365140">for</span>
  <span m="1365320">this</span> <span m="1365530">particular</span> <span m="1366070">patient.</span>
  <span m="1368300">So</span> <span m="1368380">this</span> <span m="1368650">is</span>
  <span m="1368800">all</span> <span m="1369360">the</span> <span m="1369940">data</span>
  <span m="1370330">in</span> <span m="1370510">the</span> <span m="1370630">database.</span></p><p><span
  m="1372080">Now,</span> <span m="1372370">if</span> <span m="1372550">you</span>
  <span m="1372670">want</span> <span m="1372850">to</span> <span m="1372910">try</span>
  <span m="1373150">to</span> <span m="1373270">analyze</span> <span m="1373750">some</span>
  <span m="1373990">of</span> <span m="1374110">this</span> <span m="1374260">stuff,</span>
  <span m="1374680">you</span> <span m="1374800">can</span> <span m="1374980">say,</span>
  <span m="1375350">well,</span> <span m="1377300">let's</span> <span m="1377500">look</span>
  <span m="1377950">at</span> <span m="1378760">the</span> <span m="1378970">ages</span>
  <span m="1379450">at</span> <span m="1379600">the</span> <span m="1379720">time</span>
  <span m="1380110">of</span> <span m="1380230">the</span> <span m="1380350">last</span>
  <span m="1380740">lab</span> <span m="1381040">measurement</span> <span m="1381880">in</span>
  <span m="1382060">the</span> <span m="1382150">database.</span> <span m="1383360">So</span>
  <span m="1383440">we</span> <span m="1383560">have</span> <span m="1383740">the</span>
  <span m="1383860">times</span> <span m="1384370">of</span> <span m="1384490">all</span>
  <span m="1384640">the</span> <span m="1384730">lab</span> <span m="1385030">measurements.</span></p><p><span
  m="1386330">So</span> <span m="1386410">we</span> <span m="1386530">can</span> <span
  m="1386740">see</span> <span m="1387760">that</span> <span m="1388240">many</span>
  <span m="1388690">of</span> <span m="1388840">the</span> <span m="1389020">ICU</span>
  <span m="1389560">population</span> <span m="1391000">are</span> <span m="1391150">fairly</span>
  <span m="1391600">old.</span> <span m="1393580">There's</span> <span m="1394630">a</span>
  <span m="1395140">relatively</span> <span m="1395830">small</span> <span m="1396250">number</span>
  <span m="1396640">of</span> <span m="1396790">young</span> <span m="1397030">people</span>
  <span m="1398120">and</span> <span m="1398200">then</span> <span m="1398380">a</span>
  <span m="1398470">growing</span> <span m="1398860">number</span> <span m="1399280">of</span>
  <span m="1399400">older</span> <span m="1399730">people</span> <span m="1400510">in</span>
  <span m="1400690">both</span> <span m="1402070">females</span> <span m="1402610">and</span>
  <span m="1402730">males.</span> <span m="1404140">If</span> <span m="1404440">we</span>
  <span m="1404530">look</span> <span m="1404950">at</span> <span m="1406950">age</span>
  <span m="1407230">at</span> <span m="1407350">admission</span> <span m="1407890">by</span>
  <span m="1408130">gender--</span> <span m="1409430">so</span> <span m="1409540">this</span>
  <span m="1409810">is</span> <span m="1409960">age at</span> <span m="1410380">admission</span>
  <span m="1410950">not</span> <span m="1411250">age</span> <span m="1411550">at</span>
  <span m="1411670">the</span> <span m="1411820">time</span> <span m="1412150">the</span>
  <span m="1412240">last</span> <span m="1412630">lab</span> <span m="1412870">measurement</span>
  <span m="1413440">was</span> <span m="1413650">done--</span> <span m="1415060">it's
  a</span> <span m="1415300">pretty</span> <span m="1415570">similar</span> <span
  m="1416470">curve.</span> <span m="1417160">So</span> <span m="1417430">we</span>
  <span m="1417580">see</span> <span m="1417880">that</span> <span m="1418920">females</span>
  <span m="1420160">were</span> <span m="1420490">64.21</span> <span m="1422800">at</span>
  <span m="1422950">time</span> <span m="1423250">of</span> <span m="1423400">last</span>
  <span m="1425110">lab</span> <span m="1425380">measurement;</span> <span m="1425970">63.5</span>
  <span m="1427990">at</span> <span m="1428170">the</span> <span m="1428290">time</span>
  <span m="1428620">of</span> <span m="1428770">admission.</span></p><p><span m="1431470">So</span>
  <span m="1431740">we</span> <span m="1431920">can</span> <span m="1432130">look</span>
  <span m="1432370">at</span> <span m="1432460">demographics,</span> <span m="1433840">and</span>
  <span m="1434140">demographics</span> <span m="1435010">typically</span> <span m="1435580">includes</span>
  <span m="1436810">these</span> <span m="1437170">kinds</span> <span m="1437590">of</span>
  <span m="1437710">factors,</span> <span m="1438550">which</span> <span m="1438790">I've</span>
  <span m="1438890">mentioned</span> <span m="1439300">before.</span> <span m="1440560">And</span>
  <span m="1440710">again,</span> <span m="1441040">if</span> <span m="1441190">we're</span>
  <span m="1441340">interested</span> <span m="1441880">in</span> <span m="1442000">the</span>
  <span m="1442090">relationship</span> <span m="1442900">between</span> <span m="1443410">this</span>
  <span m="1444260">and,</span> <span m="1444340">for</span> <span m="1444520">example,</span>
  <span m="1444970">the</span> <span m="1445120">age</span> <span m="1445390">distribution,</span>
  <span m="1446960">we</span> <span m="1447040">see</span> <span m="1447340">that</span>
  <span m="1449020">if</span> <span m="1449230">you</span> <span m="1449410">look</span>
  <span m="1449710">at</span> <span m="1449980">the</span> <span m="1450130">different</span>
  <span m="1451150">admission</span> <span m="1451660">types--</span> <span m="1452860">so</span>
  <span m="1453100">you</span> <span m="1453250">can</span> <span m="1453460">be</span>
  <span m="1454030">either</span> <span m="1454600">admitted</span> <span m="1456520">for</span>
  <span m="1456820">an</span> <span m="1456910">emergency</span> <span m="1458260">for</span>
  <span m="1458710">some</span> <span m="1459040">urgent</span> <span m="1459430">care</span>
  <span m="1460330">or</span> <span m="1460580">electively.</span> <span m="1462670">And</span>
  <span m="1463030">it</span> <span m="1463150">doesn't</span> <span m="1463510">seem</span>
  <span m="1463810">to</span> <span m="1463960">make</span> <span m="1464230">a</span>
  <span m="1464290">whole</span> <span m="1464470">lot</span> <span m="1464710">of</span>
  <span m="1464830">difference,</span> <span m="1465850">at</span> <span m="1466000">least</span>
  <span m="1466360">in</span> <span m="1466480">the</span> <span m="1466570">means</span>
  <span m="1467170">of</span> <span m="1467440">the</span> <span m="1467710">population</span>
  <span m="1469300">age</span> <span m="1469630">distribution.</span></p><p><span
  m="1471260">On</span> <span m="1471280">the</span> <span m="1471400">other</span>
  <span m="1471640">hand,</span> <span m="1472370">if</span> <span m="1472450">you</span>
  <span m="1472630">look</span> <span m="1473020">at</span> <span m="1473440">insurance</span>
  <span m="1474040">type</span> <span m="1475390">and,</span> <span m="1475570">say,</span>
  <span m="1476740">who's</span> <span m="1477010">paying</span> <span m="1477340">the</span>
  <span m="1477430">bills,</span> <span m="1478320">there</span> <span m="1478720">is</span>
  <span m="1478930">a</span> <span m="1479020">big</span> <span m="1479290">difference</span>
  <span m="1480040">in</span> <span m="1480220">the</span> <span m="1480340">age</span>
  <span m="1480610">distributions.</span> <span m="1482190">Now,</span> <span m="1484240">why</span>
  <span m="1484570">do</span> <span m="1484660">you</span> <span m="1484810">think</span>
  <span m="1485170">that</span> <span m="1485770">private</span> <span m="1486250">insurance</span>
  <span m="1487390">drops</span> <span m="1487900">way</span> <span m="1488200">off</span>
  <span m="1488710">at</span> <span m="1488890">about</span> <span m="1489220">65?</span></p><p><span
  m="1491331">AUDIENCE:</span> <span m="1491550">Isn't</span> <span m="1491770">insurance</span>
  <span m="1492800">always</span> <span m="1492970">covered</span> <span m="1493330">for</span>
  <span m="1493550">everyone</span> <span m="1494000">by the state health?</span></p><p><span
  m="1496120">PETER SZOLOVITS:</span> <span m="1496225">It's</span> <span m="1496330">because</span>
  <span m="1496690">of</span> <span m="1496780">Medicare.</span> <span m="1497860">So</span>
  <span m="1498100">Medicare</span> <span m="1498640">covers</span> <span m="1499180">people</span>
  <span m="1499630">who</span> <span m="1499750">are</span> <span m="1499810">65</span>
  <span m="1500500">years</span> <span m="1500740">old.</span> <span m="1502450">There's</span>
  <span m="1502600">a</span> <span m="1502660">terrible</span> <span m="1503110">story</span>
  <span m="1503560">I</span> <span m="1503680">have</span> <span m="1503830">to</span>
  <span m="1503980">tell</span> <span m="1504220">you.</span> <span m="1504370">I</span>
  <span m="1504460">was</span> <span m="1504640">talking</span> <span m="1505000">to</span>
  <span m="1505120">somebody</span> <span m="1505600">at</span> <span m="1505720">an</span>
  <span m="1505840">insurance</span> <span m="1506350">company</span> <span m="1507270">who's</span>
  <span m="1507430">a</span> <span m="1507490">bit</span> <span m="1507670">cynical,</span>
  <span m="1508270">and</span> <span m="1508390">he</span> <span m="1508510">said</span>
  <span m="1509800">suppose</span> <span m="1510370">that</span> <span m="1510610">you</span>
  <span m="1510730">see</span> <span m="1511030">a</span> <span m="1511090">63-year-old</span>
  <span m="1512050">patient</span> <span m="1513070">who's</span> <span m="1513280">developing</span>
  <span m="1513880">type</span> <span m="1514150">2</span> <span m="1514330">diabetes,</span>
  <span m="1515020">what</span> <span m="1515230">should</span> <span m="1515470">you</span>
  <span m="1515560">do</span> <span m="1515740">for</span> <span m="1515980">him?</span></p><p><span
  m="1519210">Well,</span> <span m="1519900">there</span> <span m="1520075">are</span>
  <span m="1520250">standard</span> <span m="1520700">things</span> <span m="1521060">you</span>
  <span m="1521180">should</span> <span m="1521390">do</span> <span m="1521600">for</span>
  <span m="1521810">somebody</span> <span m="1522260">developing</span> <span m="1523130">type</span>
  <span m="1523370">2</span> <span m="1523520">diabetes,</span> <span m="1525200">like</span>
  <span m="1525470">get</span> <span m="1525710">him</span> <span m="1525800">to</span>
  <span m="1525920">eat</span> <span m="1526130">better,</span> <span m="1526550">get</span>
  <span m="1526730">him</span> <span m="1526850">to</span> <span m="1526970">lose</span>
  <span m="1527270">weight,</span> <span m="1527600">get</span> <span m="1527810">him</span>
  <span m="1527930">to</span> <span m="1528050">exercise</span> <span m="1528740">more,</span>
  <span m="1529040">et</span> <span m="1529130">cetera,</span> <span m="1529650">et</span>
  <span m="1529750">cetera.</span> <span m="1531000">But</span> <span m="1531140">his</span>
  <span m="1531350">cynical</span> <span m="1531830">answer</span> <span m="1532220">was</span>
  <span m="1532490">absolutely</span> <span m="1533120">nothing.</span></p><p><span
  m="1536790">Why?</span> <span m="1537180">Well</span> <span m="1537450">it's</span>
  <span m="1537600">very</span> <span m="1537810">cheap</span> <span m="1538140">to</span>
  <span m="1538290">do</span> <span m="1538470">nothing.</span> <span m="1540330">Most</span>
  <span m="1540660">people</span> <span m="1541020">who</span> <span m="1541170">develop</span>
  <span m="1541590">type</span> <span m="1541890">2</span> <span m="1542070">diabetes</span>
  <span m="1542760">don't</span> <span m="1543060">get</span> <span m="1543270">real</span>
  <span m="1543570">sick</span> <span m="1543960">in</span> <span m="1544080">the</span>
  <span m="1544170">next</span> <span m="1544470">two</span> <span m="1544650">years.</span>
  <span m="1546670">And</span> <span m="1546750">by</span> <span m="1546960">the</span>
  <span m="1547050">time</span> <span m="1547590">this</span> <span m="1547800">patient</span>
  <span m="1548280">is</span> <span m="1548370">65,</span> <span m="1549630">he'll</span>
  <span m="1549810">be</span> <span m="1549960">the</span> <span m="1550080">government's</span>
  <span m="1550620">responsibility,</span> <span m="1551670">not</span> <span m="1551940">the</span>
  <span m="1552060">insurance</span> <span m="1552600">company's.</span> <span m="1555440">Nice.</span></p><p><span
  m="1557154">AUDIENCE:</span> <span m="1557378">Yeah.</span></p><p><span m="1561180">PETER
  SZOLOVITS:</span> <span m="1561315">So</span> <span m="1561450">of</span> <span
  m="1561570">course</span> <span m="1562110">a</span> <span m="1562170">lot</span>
  <span m="1562410">of</span> <span m="1562530">the</span> <span m="1562680">elderly</span>
  <span m="1563190">are</span> <span m="1563340">insured</span> <span m="1563820">by</span>
  <span m="1564000">Medicare</span> <span m="1564510">or</span> <span m="1564630">Medicaid,</span>
  <span m="1566310">not</span> <span m="1566580">that</span> <span m="1566790">surprising.</span>
  <span m="1567840">Self-pay</span> <span m="1568650">is</span> <span m="1568890">a</span>
  <span m="1568980">pretty</span> <span m="1569250">small</span> <span m="1569640">number</span>
  <span m="1570810">because</span> <span m="1571260">it's</span> <span m="1571500">insanely</span>
  <span m="1572130">expensive</span> <span m="1572790">to</span> <span m="1572940">pay</span>
  <span m="1573180">for</span> <span m="1573390">your</span> <span m="1573570">own</span>
  <span m="1573780">health</span> <span m="1574030">care.</span></p><p><span m="1576810">What</span>
  <span m="1576990">about</span> <span m="1577260">where</span> <span m="1577440">you</span>
  <span m="1577590">came</span> <span m="1577890">from?</span> <span m="1581580">Were</span>
  <span m="1581980">you</span> <span m="1582150">referred</span> <span m="1583890">from</span>
  <span m="1584190">a</span> <span m="1584250">clinic,</span> <span m="1584850">or</span>
  <span m="1585090">were</span> <span m="1585330">you</span> <span m="1585510">an</span>
  <span m="1585630">emergency</span> <span m="1586260">room</span> <span m="1586530">admit?</span>
  <span m="1587070">Or</span> <span m="1587280">were</span> <span m="1587580">you</span>
  <span m="1588330">referred</span> <span m="1588810">from</span> <span m="1589080">an</span>
  <span m="1589170">HMO</span> <span m="1590010">or</span> <span m="1591210">et</span>
  <span m="1591350">cetera?</span> <span m="1592530">And</span> <span m="1593640">other</span>
  <span m="1593970">than</span> <span m="1595170">a</span> <span m="1595350">transfer</span>
  <span m="1595860">from</span> <span m="1596160">a</span> <span m="1596190">skilled</span>
  <span m="1596580">nursing</span> <span m="1597000">facility</span> <span m="1598170">or</span>
  <span m="1598410">transfer</span> <span m="1599040">within</span> <span m="1599520">the</span>
  <span m="1599640">facility,</span> <span m="1600780">within</span> <span m="1601140">the</span>
  <span m="1601230">hospital,</span> <span m="1602490">it</span> <span m="1602610">doesn't</span>
  <span m="1602910">make</span> <span m="1603120">much</span> <span m="1603390">difference.</span>
  <span m="1604200">The</span> <span m="1604790">averages</span> <span m="1605440">there</span>
  <span m="1605820">and</span> <span m="1605895">the</span> <span m="1605970">distributions</span>
  <span m="1607350">look</span> <span m="1607620">moderately</span> <span m="1608310">similar.</span></p><p><span
  m="1610290">If</span> <span m="1610500">you're</span> <span m="1610950">coming</span>
  <span m="1611310">from</span> <span m="1611580">a</span> <span m="1611640">skilled</span>
  <span m="1612000">nursing</span> <span m="1612390">facility,</span> <span m="1613440">if</span>
  <span m="1613590">you</span> <span m="1613830">are</span> <span m="1614100">in</span>
  <span m="1614340">a</span> <span m="1614400">skilled</span> <span m="1614790">nursing</span>
  <span m="1615210">facility,</span> <span m="1616290">you're</span> <span m="1616470">probably</span>
  <span m="1617040">old</span> <span m="1618390">because</span> <span m="1618630">younger</span>
  <span m="1618930">people</span> <span m="1619320">don't</span> <span m="1619680">typically</span>
  <span m="1620600">need</span> <span m="1620880">skilled</span> <span m="1621240">nursing</span>
  <span m="1621660">care.</span> <span m="1622560">And</span> <span m="1622740">I'm</span>
  <span m="1622920">not</span> <span m="1623100">sure</span> <span m="1623370">why</span>
  <span m="1624120">transfers</span> <span m="1624840">within</span> <span m="1625200">the</span>
  <span m="1625320">facility</span> <span m="1626490">are</span> <span m="1628230">significantly</span>
  <span m="1629100">younger</span> <span m="1629490">ages,</span> <span m="1630120">but</span>
  <span m="1630540">that's</span> <span m="1630780">true</span> <span m="1632040">from</span>
  <span m="1632310">the</span> <span m="1632400">MIMIC</span> <span m="1632730">data.</span></p><p><span
  m="1635610">What</span> <span m="1635790">about</span> <span m="1636060">age</span>
  <span m="1636560">at</span> <span m="1636820">admission</span> <span m="1637440">by</span>
  <span m="1637710">language?</span> <span m="1638730">So</span> <span m="1639000">some</span>
  <span m="1639270">people</span> <span m="1639630">speak</span> <span m="1640020">English.</span>
  <span m="1640950">Some</span> <span m="1641670">people</span> <span m="1642060">speak</span>
  <span m="1642450">not</span> <span m="1642720">available.</span> <span m="1645180">Some</span>
  <span m="1645450">people</span> <span m="1645840">speak</span> <span m="1646230">Spanish,</span>
  <span m="1646860">et</span> <span m="1646940">cetera.</span> <span m="1648490">So</span>
  <span m="1648610">it</span> <span m="1648660">turns</span> <span m="1648990">out</span>
  <span m="1649140">the</span> <span m="1649260">Russians</span> <span m="1650370">are</span>
  <span m="1650550">the</span> <span m="1650700">oldest.</span> <span m="1653610">And</span>
  <span m="1654030">that</span> <span m="1654270">may</span> <span m="1654510">have</span>
  <span m="1654720">to</span> <span m="1654840">do</span> <span m="1655050">with</span>
  <span m="1655260">immigration</span> <span m="1655920">patterns,</span> <span m="1656550">or</span>
  <span m="1657150">I</span> <span m="1657240">don't</span> <span m="1657390">know</span>
  <span m="1657570">exactly</span> <span m="1658140">why.</span> <span m="1661040">But</span>
  <span m="1661480">that's</span> <span m="1663190">what</span> <span m="1663450">the</span>
  <span m="1663570">data</span> <span m="1663870">show.</span></p><p><span m="1665700">If</span>
  <span m="1665940">you</span> <span m="1666060">do</span> <span m="1666240">it</span>
  <span m="1666330">by</span> <span m="1666570">ethnicity,</span> <span m="1668310">it</span>
  <span m="1668460">turns</span> <span m="1668850">out</span> <span m="1669120">that</span>
  <span m="1670800">African-Americans,</span> <span m="1672690">on</span> <span m="1672900">the</span>
  <span m="1672990">whole,</span> <span m="1673590">are</span> <span m="1673950">somewhat</span>
  <span m="1674460">younger</span> <span m="1674880">than</span> <span m="1675090">whites.</span>
  <span m="1676080">And</span> <span m="1676320">Hispanics</span> <span m="1677130">are</span>
  <span m="1677280">somewhat</span> <span m="1677730">younger</span> <span m="1678150">yet.</span>
  <span m="1681300">So</span> <span m="1681570">that</span> <span m="1681780">means</span>
  <span m="1682140">that</span> <span m="1682950">those</span> <span m="1683980">subpopulations</span>
  <span m="1685860">apparently</span> <span m="1686520">need</span> <span m="1687150">intensive</span>
  <span m="1687720">care</span> <span m="1688590">earlier</span> <span m="1689100">in</span>
  <span m="1689220">life</span> <span m="1689670">than</span> <span m="1690690">whites.</span>
  <span m="1691680">So</span> <span m="1691860">this</span> <span m="1692130">is</span>
  <span m="1692970">a</span> <span m="1693030">topic</span> <span m="1693510">that's</span>
  <span m="1693750">very</span> <span m="1694410">hot</span> <span m="1694800">right</span>
  <span m="1695100">now,</span> <span m="1695670">discussions</span> <span m="1696450">about</span>
  <span m="1696960">how</span> <span m="1697710">bias</span> <span m="1698160">might</span>
  <span m="1698460">play</span> <span m="1698790">into</span> <span m="1699620">health</span>
  <span m="1699890">care.</span> <span m="1700250">Yeah?</span></p><p><span m="1700864">AUDIENCE:</span>
  <span m="1701025">What</span> <span m="1701186">does</span> <span m="1701348">unable</span>
  <span m="1701832">to obtain</span> <span m="1702316">mean?</span></p><p><span m="1703770">PETER
  SZOLOVITS:</span> <span m="1703815">It</span> <span m="1703860">just</span> <span
  m="1704130">means</span> <span m="1704490">that</span> <span m="1705000">somebody</span>
  <span m="1705690">refused</span> <span m="1706200">to</span> <span m="1706320">say</span>
  <span m="1706680">what</span> <span m="1706920">their</span> <span m="1707100">ethnicity</span>
  <span m="1707670">was.</span></p><p><span m="1708000">AUDIENCE:</span> <span m="1708192">When</span>
  <span m="1708385">they were asked</span> <span m="1708770">this?</span></p><p><span
  m="1709540">PETER SZOLOVITS:</span> <span m="1709625">Yeah.</span> <span m="1710910">I</span>
  <span m="1711240">think.</span> <span m="1711750">I'm</span> <span m="1711870">not</span>
  <span m="1712080">positive.</span></p><p><span m="1714150">AUDIENCE:</span> <span
  m="1714200">So</span> <span m="1714510">just</span> <span m="1714810">to</span>
  <span m="1714990">confirm.</span> <span m="1716610">This</span> <span m="1716820">also</span>
  <span m="1717060">represents</span> <span m="1717750">Boston's</span> <span m="1718820">population</span>
  <span m="1719160">dynamics</span> <span m="1719602">too,</span> <span m="1720044">right?</span></p><p><span
  m="1720930">PETER SZOLOVITS:</span> <span m="1721065">It's</span> <span m="1721200">the</span>
  <span m="1721320">catchment</span> <span m="1721860">basin</span> <span m="1722430">of</span>
  <span m="1722670">the</span> <span m="1722790">Beth</span> <span m="1723060">Israel</span>
  <span m="1723450">Deaconess</span> <span m="1723550">Hospital,</span> <span m="1724530">which</span>
  <span m="1724800">is</span> <span m="1725460">Boston</span> <span m="1726030">clearly.</span>
  <span m="1727020">But</span> <span m="1727320">there</span> <span m="1727530">are--</span>
  <span m="1729030">it</span> <span m="1729150">turns</span> <span m="1729510">out</span>
  <span m="1729720">that</span> <span m="1730950">a</span> <span m="1731010">lot</span>
  <span m="1731220">of</span> <span m="1731340">North</span> <span m="1731640">Shore</span>
  <span m="1731940">people</span> <span m="1732390">go</span> <span m="1732600">to</span>
  <span m="1732690">Mass</span> <span m="1732790">General,</span> <span m="1734020">and</span>
  <span m="1734610">so</span> <span m="1734820">different</span> <span m="1735210">hospitals</span>
  <span m="1735900">have</span> <span m="1736140">different</span> <span m="1736500">catchment</span>
  <span m="1736980">basins.</span></p><p><span m="1737730">AUDIENCE:</span> <span
  m="1737835">Does</span> <span m="1737940">it</span> <span m="1738090">have</span>
  <span m="1738360">anything</span> <span m="1738660">to</span> <span m="1738780">do</span>
  <span m="1738910">with</span> <span m="1739030">like,</span> <span m="1739380">is</span>
  <span m="1739530">this</span> <span m="1739680">just</span> <span m="1739870">the</span>
  <span m="1740020">ICU?</span> <span m="1740640">Or</span> <span m="1740820">is</span>
  <span m="1740970">this</span> <span m="1741930">everybody</span> <span m="1742245">who</span>
  <span m="1742560">goes</span> <span m="1742860">to</span> <span m="1743160">the</span>
  <span m="1743250">hospital</span> <span m="1743640">or the</span> <span m="1744033">ER?</span></p><p><span
  m="1744820">PETER SZOLOVITS:</span> <span m="1744980">These</span> <span m="1745140">are</span>
  <span m="1745260">all</span> <span m="1745530">people</span> <span m="1746040">who</span>
  <span m="1746400">at</span> <span m="1746610">some</span> <span m="1746910">point</span>
  <span m="1747270">were</span> <span m="1747480">in</span> <span m="1747630">the</span>
  <span m="1747780">ICU.</span> <span m="1750040">So</span> <span m="1750150">these</span>
  <span m="1750420">are</span> <span m="1750540">the</span> <span m="1750690">sicker</span>
  <span m="1751140">patients.</span> <span m="1752580">Yeah?</span></p><p><span m="1753690">AUDIENCE:</span>
  <span m="1753832">So just want</span> <span m="1754970">to double-check</span> <span
  m="1756090">there's a</span> <span m="1756150">higher</span> <span m="1756510">proportion</span>
  <span m="1756840">of</span> <span m="1757210">black,</span> <span m="1757691">African
  American people</span> <span m="1758172">in</span> <span m="1758653">the population</span>
  <span m="1759134">here as well</span> <span m="1760096">because</span> <span m="1760577">the</span>
  <span m="1761058">red is</span> <span m="1761539">higher than</span> <span m="1762020">the
  others?</span></p><p><span m="1763950">PETER SZOLOVITS:</span> <span m="1764175">No,</span>
  <span m="1764400">actually--</span> <span m="1766230">I</span> <span m="1766290">don't</span>
  <span m="1766500">remember</span> <span m="1766950">if</span> <span m="1767130">I</span>
  <span m="1767220">have</span> <span m="1767430">that</span> <span m="1767640">graph--</span>
  <span m="1767970">I</span> <span m="1768090">think</span> <span m="1768300">this</span>
  <span m="1768540">is</span> <span m="1768690">cumulative.</span></p><p><span m="1769883">AUDIENCE:</span>
  <span m="1770020">Oh,</span> <span m="1770157">OK.</span></p><p><span m="1771570">PETER
  SZOLOVITS:</span> <span m="1771705">So</span> <span m="1773130">most</span> <span
  m="1774030">people</span> <span m="1774570">are</span> <span m="1775530">white</span>
  <span m="1778010">for</span> <span m="1778260">whatever</span> <span m="1778980">definition</span>
  <span m="1779670">of</span> <span m="1779790">white</span> <span m="1780510">we're</span>
  <span m="1780690">using.</span> <span m="1781680">And</span> <span m="1781860">I</span>
  <span m="1781950">think</span> <span m="1782220">it's</span> <span m="1782400">only</span>
  <span m="1782700">the</span> <span m="1783090">increment</span> <span m="1783660">that</span>
  <span m="1783870">you</span> <span m="1784020">see</span> <span m="1784260">on</span>
  <span m="1784410">top.</span></p><p><span m="1789570">All</span> <span m="1789630">right,</span>
  <span m="1789840">how</span> <span m="1789960">about</span> <span m="1790200">marital</span>
  <span m="1790620">status?</span> <span m="1793490">Well,</span> <span m="1793730">according</span>
  <span m="1794150">to</span> <span m="1794300">this,</span> <span m="1794660">it's</span>
  <span m="1794840">bad</span> <span m="1795140">to</span> <span m="1795320">be</span>
  <span m="1795470">single.</span> <span m="1803280">So</span> <span m="1803640">I</span>
  <span m="1803970">could</span> <span m="1804180">sort</span> <span m="1804480">of</span>
  <span m="1804540">see</span> <span m="1804780">that</span> <span m="1804990">for</span>
  <span m="1805170">hospitalization.</span> <span m="1806130">I'm</span> <span m="1806250">not</span>
  <span m="1806430">sure</span> <span m="1806670">why</span> <span m="1807000">it's</span>
  <span m="1807240">true</span> <span m="1807480">for</span> <span m="1807690">the</span>
  <span m="1807840">ICU</span> <span m="1809580">because</span> <span m="1810900">if</span>
  <span m="1811110">you</span> <span m="1811200">don't</span> <span m="1811410">have</span>
  <span m="1811590">anybody</span> <span m="1812220">at</span> <span m="1812370">home</span>
  <span m="1813180">to</span> <span m="1813330">take</span> <span m="1813570">care</span>
  <span m="1813870">of</span> <span m="1813990">you</span> <span m="1814120">when</span>
  <span m="1814320">you</span> <span m="1814440">get</span> <span m="1814650">sick,</span>
  <span m="1815450">it</span> <span m="1815550">seems</span> <span m="1816150">reasonable</span>
  <span m="1816780">that</span> <span m="1816990">you'd</span> <span m="1817110">be</span>
  <span m="1817260">more</span> <span m="1817470">likely</span> <span m="1817860">to</span>
  <span m="1817980">wind</span> <span m="1818280">up</span> <span m="1818430">in</span>
  <span m="1818550">the</span> <span m="1818610">hospital.</span> <span m="1819150">But</span>
  <span m="1819300">I</span> <span m="1819390">don't</span> <span m="1819510">know</span>
  <span m="1819660">why</span> <span m="1819870">you'd</span> <span m="1820050">wind</span>
  <span m="1820290">up</span> <span m="1820470">in</span> <span m="1820590">intensive</span>
  <span m="1821070">care.</span> <span m="1821480">Yeah?</span></p><p><span m="1822080">AUDIENCE:</span>
  <span m="1822180">Isn't</span> <span m="1822280">it</span> <span m="1822390">possible</span>
  <span m="1822840">that</span> <span m="1823320">those</span> <span m="1823540">are</span>
  <span m="1823760">also</span> <span m="1824790">single</span> <span m="1825170">people</span>
  <span m="1825430">are</span> <span m="1825940">probably</span> <span m="1826470">younger</span>
  <span m="1826860">than</span> <span m="1827272">married</span> <span m="1827684">people,</span>
  <span m="1828510">and</span> <span m="1828900">those</span> <span m="1829040">are</span>
  <span m="1829230">probably</span> <span m="1829470">younger</span> <span m="1829840">than--</span></p><p><span
  m="1830130">PETER SZOLOVITS:</span> <span m="1830295">Yes,</span> <span m="1830460">yeah.</span></p><p><span
  m="1830790">AUDIENCE:</span> <span m="1830870">[INAUDIBLE]</span> <span m="1830950">people.</span></p><p><span
  m="1831450">PETER SZOLOVITS:</span> <span m="1831530">Yeah,</span> <span m="1831610">that's</span>
  <span m="1831690">probably</span> <span m="1832020">also</span> <span m="1832480">right.</span></p><p><span
  m="1839330">So</span> <span m="1840260">here's</span> <span m="1840530">an</span>
  <span m="1840650">interesting</span> <span m="1841130">question,</span> <span m="1841610">a</span>
  <span m="1841670">little</span> <span m="1841880">bit</span> <span m="1842090">related</span>
  <span m="1842600">to</span> <span m="1842750">something</span> <span m="1843170">you'll</span>
  <span m="1843380">see</span> <span m="1843650">on</span> <span m="1844130">the</span>
  <span m="1844250">next</span> <span m="1844580">problem</span> <span m="1845000">set.</span>
  <span m="1846800">So</span> <span m="1847040">could</span> <span m="1847400">we</span>
  <span m="1847610">predict</span> <span m="1848420">in-hospital</span> <span m="1849170">mortality</span>
  <span m="1850520">from</span> <span m="1850880">just</span> <span m="1851150">these</span>
  <span m="1851360">demographic</span> <span m="1852020">features?</span> <span m="1856100">So</span>
  <span m="1856370">I'm</span> <span m="1856550">using</span> <span m="1856940">a</span>
  <span m="1857030">tool</span> <span m="1857720">in</span> <span m="1859280">language</span>
  <span m="1859730">called</span> <span m="1860120">R.</span> <span m="1860990">This</span>
  <span m="1861290">is</span> <span m="1861455">a</span> <span m="1861620">general</span>
  <span m="1862040">linear</span> <span m="1862460">model,</span> <span m="1862940">and</span>
  <span m="1863060">I've</span> <span m="1863180">set</span> <span m="1863450">it</span>
  <span m="1863570">up</span> <span m="1863720">to</span> <span m="1863840">do</span>
  <span m="1864140">basically</span> <span m="1864710">logistic</span> <span m="1865220">regression.</span>
  <span m="1866540">And</span> <span m="1866960">it</span> <span m="1867140">says</span>
  <span m="1867770">I'm</span> <span m="1867980">predicting</span> <span m="1868670">whether</span>
  <span m="1869000">you</span> <span m="1869180">die</span> <span m="1869480">in</span>
  <span m="1869600">the</span> <span m="1869690">hospital</span> <span m="1871400">based</span>
  <span m="1871910">on</span> <span m="1872390">these</span> <span m="1874850">demographic</span>
  <span m="1875600">factors.</span></p><p><span m="1876920">And</span> <span m="1877160">it</span>
  <span m="1877220">turns</span> <span m="1877580">out</span> <span m="1877850">that</span>
  <span m="1878360">the</span> <span m="1878810">only</span> <span m="1879110">ones</span>
  <span m="1879500">that</span> <span m="1879710">are</span> <span m="1880490">highly</span>
  <span m="1880850">significant</span> <span m="1882170">are</span> <span m="1882350">age.</span>
  <span m="1883940">So</span> <span m="1884120">that's</span> <span m="1884360">not</span>
  <span m="1884570">surprising,</span> <span m="1885860">that</span> <span m="1886610">older</span>
  <span m="1886910">people</span> <span m="1887300">are</span> <span m="1887390">more</span>
  <span m="1887630">likely</span> <span m="1888050">to</span> <span m="1888230">die</span>
  <span m="1888530">than</span> <span m="1888740">younger</span> <span m="1889040">people.</span>
  <span m="1889940">It's</span> <span m="1890090">generally</span> <span m="1890540">true.</span>
  <span m="1892100">And</span> <span m="1892940">if</span> <span m="1893180">I'm</span>
  <span m="1893540">unable</span> <span m="1894080">to</span> <span m="1894710">obtain</span>
  <span m="1895160">your</span> <span m="1895340">ethnicity,</span> <span m="1896210">or</span>
  <span m="1896480">I</span> <span m="1896630">don't</span> <span m="1896960">know</span>
  <span m="1897170">your</span> <span m="1897380">ethnicity,</span> <span m="1898940">then</span>
  <span m="1899180">you're</span> <span m="1899300">more</span> <span m="1899540">likely</span>
  <span m="1899930">to</span> <span m="1900050">die.</span> <span m="1902540">I</span>
  <span m="1902710">have</span> <span m="1902840">no</span> <span m="1903170">clue</span>
  <span m="1904280">why</span> <span m="1904520">that</span> <span m="1904760">might</span>
  <span m="1905000">be</span> <span m="1905180">the</span> <span m="1905270">case.</span></p><p><span
  m="1906980">And</span> <span m="1907220">other</span> <span m="1907520">things</span>
  <span m="1907970">are</span> <span m="1908450">not</span> <span m="1908750">as</span>
  <span m="1908900">significant.</span> <span m="1909810">So</span> <span m="1909980">if</span>
  <span m="1910130">you</span> <span m="1910220">speak</span> <span m="1910550">Spanish</span>
  <span m="1911060">or</span> <span m="1911180">English,</span> <span m="1912170">you're</span>
  <span m="1912350">slightly</span> <span m="1912890">less</span> <span m="1913220">likely</span>
  <span m="1913700">to</span> <span m="1913850">die.</span> <span m="1914180">You</span>
  <span m="1914330">see</span> <span m="1914600">a</span> <span m="1914690">negative</span>
  <span m="1915170">contribution</span> <span m="1916040">here.</span> <span m="1916970">And</span>
  <span m="1917180">if</span> <span m="1918050">you</span> <span m="1918200">speak</span>
  <span m="1918560">Russian,</span> <span m="1919070">you're</span> <span m="1919250">slightly</span>
  <span m="1919790">less</span> <span m="1920060">likely</span> <span m="1920480">to</span>
  <span m="1920630">die.</span> <span m="1921560">But</span> <span m="1921770">it's</span>
  <span m="1922370">significant</span> <span m="1923210">not</span> <span m="1923540">at</span>
  <span m="1923660">the</span> <span m="1923810">p</span> <span m="1924200">equal</span>
  <span m="1924380">0.05</span> <span m="1925190">level,</span> <span m="1926030">but</span>
  <span m="1926240">it</span> <span m="1926360">is</span> <span m="1926570">at</span>
  <span m="1926690">the</span> <span m="1926930">p equal</span> <span m="1927410">0.06</span>
  <span m="1928220">level.</span> <span m="1930170">And</span> <span m="1930650">marriage</span>
  <span m="1931220">doesn't</span> <span m="1931610">seem</span> <span m="1931940">to</span>
  <span m="1932090">make</span> <span m="1932360">much</span> <span m="1932630">difference</span>
  <span m="1933260">in</span> <span m="1934280">predicting</span> <span m="1934880">whether</span>
  <span m="1935180">you're</span> <span m="1935330">going</span> <span m="1935480">to</span>
  <span m="1935570">die</span> <span m="1935840">or</span> <span m="1935960">not.</span></p><p><span
  m="1937190">Now,</span> <span m="1937340">remember,</span> <span m="1937820">this</span>
  <span m="1938060">is</span> <span m="1938250">ICU</span> <span m="1938780">patients.</span>
  <span m="1940770">And</span> <span m="1940940">we're</span> <span m="1941150">looking</span>
  <span m="1941540">at</span> <span m="1941690">in-hospital</span> <span m="1942380">mortality.</span></p><p><span
  m="1944570">AUDIENCE:</span> <span m="1944695">For</span> <span m="1944820">ethnicity,</span>
  <span m="1946430">can</span> <span m="1946580">they learn</span> <span m="1946850">that</span>
  <span m="1947030">at</span> <span m="1947150">any</span> <span m="1947360">point</span>
  <span m="1947570">in this</span> <span m="1947870">study,</span> <span m="1948190">or</span>
  <span m="1948320">just</span> <span m="1948520">right</span> <span m="1948700">at</span>
  <span m="1948770">the</span> <span m="1948860">beginning?</span> <span m="1949450">Or</span>
  <span m="1950060">do</span> <span m="1950270">you</span> <span m="1950390">know?</span>
  <span m="1950630">Because</span> <span m="1950975">I don't know.</span></p><p><span
  m="1951320">PROFESSOR:</span> <span m="1951365">I</span> <span m="1951410">don't</span>
  <span m="1951590">know.</span></p><p><span m="1952340">AUDIENCE:</span> <span m="1952460">Because</span>
  <span m="1952730">it</span> <span m="1952820">could</span> <span m="1953000">be</span>
  <span m="1953180">that</span> <span m="1954170">unable</span> <span m="1954470">to</span>
  <span m="1954860">obtain</span> <span m="1955180">means</span> <span m="1955370">that</span>
  <span m="1955520">they</span> <span m="1955640">died</span> <span m="1955940">before</span>
  <span m="1956210">we</span> <span m="1956330">can</span> <span m="1956450">ask</span>
  <span m="1956660">them.</span></p><p><span m="1957880">PROFESSOR:</span> <span m="1958020">No,</span>
  <span m="1958160">because</span> <span m="1958820">there</span> <span m="1959330">wouldn't</span>
  <span m="1959630">be</span> <span m="1959810">that</span> <span m="1960050">many</span>
  <span m="1960320">of</span> <span m="1960440">those</span> <span m="1960710">people,</span>
  <span m="1961160">I</span> <span m="1961250">think.</span> <span m="1964040">There
  are</span> <span m="1964250">not</span> <span m="1964460">that</span> <span m="1964670">many</span>
  <span m="1964910">people</span> <span m="1965750">who</span> <span m="1965930">don't</span>
  <span m="1966260">live</span> <span m="1966500">past</span> <span m="1967290">the</span>
  <span m="1968390">intake</span> <span m="1968840">interview.</span> <span m="1971300">And</span>
  <span m="1971450">they</span> <span m="1971600">do</span> <span m="1971810">ask</span>
  <span m="1972080">them.</span></p><p><span m="1975350">AUDIENCE:</span> <span m="1975465">[INAUDIBLE]</span></p><p><span
  m="1978420">PROFESSOR:</span> <span m="1978645">Yeah,</span> <span m="1978870">that</span>
  <span m="1979470">would</span> <span m="1979650">be</span> <span m="1979800">an</span>
  <span m="1979890">example.</span> <span m="1980560">But</span> <span m="1980640">I</span>
  <span m="1980730">don't</span> <span m="1980910">think</span> <span m="1981150">you'd</span>
  <span m="1981360">see</span> <span m="1981630">enough</span> <span m="1982020">such</span>
  <span m="1982350">people</span> <span m="1983820">to</span> <span m="1985170">show</span>
  <span m="1985500">up</span> <span m="1985860">statistically.</span></p><p><span
  m="1988800">OK.</span> <span m="1991410">Well,</span> <span m="1992910">so</span>
  <span m="1993240">I've</span> <span m="1993450">already</span> <span m="1993780">mentioned</span>
  <span m="1994380">that</span> <span m="1994620">there</span> <span m="1994720">is</span>
  <span m="1994920">this</span> <span m="1995100">problem</span> <span m="1996390">of</span>
  <span m="1996570">having</span> <span m="1996930">moved</span> <span m="1997380">from</span>
  <span m="1997740">CareVue</span> <span m="1997970">view</span> <span m="1998180">to</span>
  <span m="1998280">MetaVision</span> <span m="1999090">just</span> <span m="1999450">in</span>
  <span m="1999600">the</span> <span m="1999660">MIMIC</span> <span m="1999990">database.</span>
  <span m="2001590">But</span> <span m="2001670">of</span> <span m="2001790">course,</span>
  <span m="2002090">this</span> <span m="2002330">is</span> <span m="2002480">a</span>
  <span m="2002540">much</span> <span m="2002780">bigger</span> <span m="2003080">problem</span>
  <span m="2003890">around</span> <span m="2004250">the</span> <span m="2004340">country</span>
  <span m="2004790">and</span> <span m="2004940">around</span> <span m="2005240">the</span>
  <span m="2005330">world,</span> <span m="2005720">because</span> <span m="2006650">every</span>
  <span m="2006890">hospital</span> <span m="2007400">has</span> <span m="2007670">its</span>
  <span m="2007850">own</span> <span m="2008030">way</span> <span m="2008210">of</span>
  <span m="2008360">keeping</span> <span m="2008720">records.</span> <span m="2009890">And</span>
  <span m="2010100">wouldn't</span> <span m="2010430">it</span> <span m="2010580">be</span>
  <span m="2010730">nice</span> <span m="2011360">if</span> <span m="2011630">we</span>
  <span m="2011840">had</span> <span m="2012320">standards?</span></p><p><span m="2014180">And</span>
  <span m="2014360">of</span> <span m="2014480">course,</span> <span m="2014900">there's</span>
  <span m="2015170">this</span> <span m="2015380">funny</span> <span m="2015860">phrase,</span>
  <span m="2016310">the</span> <span m="2016430">wonderful</span> <span m="2016880">thing</span>
  <span m="2017120">about</span> <span m="2017360">standards</span> <span m="2018470">is</span>
  <span m="2018650">that</span> <span m="2018800">there's</span> <span m="2018980">so</span>
  <span m="2019160">many</span> <span m="2019430">to</span> <span m="2019580">choose</span>
  <span m="2019910">from.</span> <span m="2021530">So</span> <span m="2021770">for</span>
  <span m="2021980">example,</span> <span m="2022560">if</span> <span m="2022610">you</span>
  <span m="2022730">look</span> <span m="2022970">at</span> <span m="2023090">prescriptions</span>
  <span m="2024170">in</span> <span m="2024350">the</span> <span m="2024440">MIMIC</span>
  <span m="2024770">database,</span> <span m="2026390">here</span> <span m="2026690">are</span>
  <span m="2026870">two</span> <span m="2027140">particular</span> <span m="2028340">prescriptions</span>
  <span m="2029280">for</span> <span m="2029510">subject</span> <span m="2029990">number</span>
  <span m="2030390">57139</span> <span m="2033050">admitted</span> <span m="2033800">on</span>
  <span m="2034250">admission</span> <span m="2034830">ID</span> <span m="2035960">155470.</span>
  <span m="2038690">And</span> <span m="2038930">so</span> <span m="2039310">they</span>
  <span m="2039830">have</span> <span m="2040010">the</span> <span m="2040130">same</span>
  <span m="2040430">start</span> <span m="2040850">date</span> <span m="2041150">but</span>
  <span m="2041360">different</span> <span m="2041780">end</span> <span m="2041990">dates.</span>
  <span m="2043310">One</span> <span m="2043670">is</span> <span m="2044030">a</span>
  <span m="2044120">prescription</span> <span m="2044870">for</span> <span m="2045860">Tylenol,</span>
  <span m="2046730">acetaminophen,</span> <span m="2048199">and</span> <span m="2048380">the</span>
  <span m="2048530">other</span> <span m="2048889">is</span> <span m="2049100">for</span>
  <span m="2049340">clobetasol</span> <span m="2049820">propionate</span> <span m="2050719">0.05%</span>
  <span m="2052580">cream.</span> <span m="2053469">That's</span> <span m="2053810">a</span>
  <span m="2054080">skin</span> <span m="2054920">lotion</span> <span m="2055670">thing</span>
  <span m="2056000">for--</span> <span m="2056960">I</span> <span m="2057050">think</span>
  <span m="2057260">it's</span> <span m="2057440">a</span> <span m="2057500">steroid</span>
  <span m="2058730">skin</span> <span m="2059120">cream.</span></p><p><span m="2060530">So</span>
  <span m="2061010">if</span> <span m="2061190">you</span> <span m="2061340">look</span>
  <span m="2061790">in</span> <span m="2061969">the</span> <span m="2062210">BI's</span>
  <span m="2062630">database,</span> <span m="2063710">they</span> <span m="2064040">have</span>
  <span m="2064340">their</span> <span m="2064610">own</span> <span m="2064940">private</span>
  <span m="2065480">formulary</span> <span m="2066170">code</span> <span m="2067340">where</span>
  <span m="2067880">this</span> <span m="2068270">thing</span> <span m="2068690">is</span>
  <span m="2069500">acet325</span> <span m="2071870">and</span> <span m="2072110">this</span>
  <span m="2072380">thing</span> <span m="2072679">is</span> <span m="2072889">clob.05C30,</span>
  <span m="2076940">right?</span> <span m="2078380">And</span> <span m="2078530">if</span>
  <span m="2078679">you</span> <span m="2078800">look,</span> <span m="2079360">there</span>
  <span m="2079739">there's</span> <span m="2079940">also</span> <span m="2080300">something</span>
  <span m="2080750">called</span> <span m="2081070">a</span> <span m="2081330">GSN,</span>
  <span m="2082739">which</span> <span m="2082940">is</span> <span m="2083060">some</span>
  <span m="2083690">commercial</span> <span m="2085070">coding</span> <span m="2085520">system</span>
  <span m="2086030">for</span> <span m="2086270">drugs.</span> <span m="2087590">Maybe</span>
  <span m="2087980">having</span> <span m="2088340">to</span> <span m="2088520">do</span>
  <span m="2088730">with</span> <span m="2089030">who</span> <span m="2089750">their</span>
  <span m="2089960">drug</span> <span m="2090260">supplier</span> <span m="2090920">is</span>
  <span m="2091219">at</span> <span m="2091400">the</span> <span m="2091489">hospital.</span>
  <span m="2093090">And</span> <span m="2093320">these</span> <span m="2093620">have</span>
  <span m="2093830">different</span> <span m="2094190">codes.</span></p><p><span m="2095310">There's</span>
  <span m="2095659">the</span> <span m="2095780">National</span> <span m="2095880">Drug</span>
  <span m="2096350">Code,</span> <span m="2097100">which</span> <span m="2097340">is</span>
  <span m="2097520">an</span> <span m="2097670">FDA</span> <span m="2098300">assigned</span>
  <span m="2100730">nine</span> <span m="2101090">digit</span> <span m="2101480">code</span>
  <span m="2102380">that</span> <span m="2102620">specifies</span> <span m="2103490">who</span>
  <span m="2103610">made</span> <span m="2103940">the</span> <span m="2104090">drug,</span>
  <span m="2105320">what</span> <span m="2105590">form</span> <span m="2106010">it's</span>
  <span m="2106280">in,</span> <span m="2106730">and</span> <span m="2107630">what's</span>
  <span m="2107990">its</span> <span m="2108110">strength.</span> <span m="2109670">And</span>
  <span m="2109850">so</span> <span m="2110060">you</span> <span m="2110180">get</span>
  <span m="2110450">these.</span> <span m="2111650">Then</span> <span m="2111950">there's</span>
  <span m="2112310">a</span> <span m="2112850">human</span> <span m="2113510">readable</span>
  <span m="2114110">description</span> <span m="2114890">that</span> <span m="2115100">says</span>
  <span m="2116360">Tylenol</span> <span m="2116990">comes</span> <span m="2117410">in</span>
  <span m="2117610">325</span> <span m="2118610">milligram</span> <span m="2119120">tablets.</span>
  <span m="2120450">And</span> <span m="2120590">the</span> <span m="2120730">clobetasol</span>
  <span m="2121670">comes</span> <span m="2122060">in</span> <span m="2122180">30</span>
  <span m="2122510">gram</span> <span m="2122840">tubes.</span> <span m="2124640">And</span>
  <span m="2125060">the</span> <span m="2125750">dose</span> <span m="2126500">is</span>
  <span m="2126680">supposed</span> <span m="2127160">to</span> <span m="2127310">be</span>
  <span m="2127910">325</span> <span m="2128870">to</span> <span m="2129020">650,</span>
  <span m="2130310">i.e.</span> <span m="2130790">one</span> <span m="2131030">to</span>
  <span m="2131210">two</span> <span m="2131930">tablets</span> <span m="2133190">measured</span>
  <span m="2133640">in</span> <span m="2133730">milligrams.</span> <span m="2134510">The</span>
  <span m="2134660">dose</span> <span m="2135080">here</span> <span m="2135830">is</span>
  <span m="2136100">one</span> <span m="2136640">application,</span> <span m="2138570">whatever</span>
  <span m="2138830">that</span> <span m="2139070">is.</span></p><p><span m="2140270">I</span>
  <span m="2140360">don't</span> <span m="2140510">know</span> <span m="2140690">what</span>
  <span m="2140900">the</span> <span m="2141020">0.01</span> <span m="2141710">means.</span>
  <span m="2142640">And</span> <span m="2142820">this</span> <span m="2143060">is</span>
  <span m="2143240">a</span> <span m="2143300">tablet</span> <span m="2143910">and</span>
  <span m="2144050">that's</span> <span m="2144320">a</span> <span m="2144380">tube.</span>
  <span m="2145370">And</span> <span m="2145700">this</span> <span m="2146000">is</span>
  <span m="2146150">taken</span> <span m="2146600">orally.</span> <span m="2147260">That's</span>
  <span m="2147830">administered</span> <span m="2148610">on</span> <span m="2148760">the</span>
  <span m="2148850">skin,</span> <span m="2150350">right?</span> <span m="2151970">So</span>
  <span m="2152960">this</span> <span m="2153200">is</span> <span m="2153350">a</span>
  <span m="2153410">local</span> <span m="2153830">database.</span></p><p><span m="2155230">AUDIENCE:</span>
  <span m="2155355">For</span> <span m="2155480">a</span> <span m="2155550">doctor,</span>
  <span m="2156320">they just</span> <span m="2156625">[INAUDIBLE]</span></p><p><span
  m="2160490">PROFESSOR:</span> <span m="2160580">At</span> <span m="2160670">most</span>
  <span m="2161090">hospitals,</span> <span m="2161810">that's</span> <span m="2162110">true</span>
  <span m="2162410">now.</span> <span m="2163250">It</span> <span m="2163400">wasn't</span>
  <span m="2163790">true</span> <span m="2164120">when</span> <span m="2164420">the</span>
  <span m="2164510">MIMIC</span> <span m="2164840">database</span> <span m="2165350">started</span>
  <span m="2165800">being</span> <span m="2166880">collected.</span> <span m="2168170">And</span>
  <span m="2169160">the</span> <span m="2169600">BI</span> <span m="2169940">was</span>
  <span m="2170210">relatively</span> <span m="2170870">late</span> <span m="2171860">in</span>
  <span m="2172040">moving</span> <span m="2172430">to</span> <span m="2172580">that</span>
  <span m="2172940">compared</span> <span m="2173390">to</span> <span m="2173570">some</span>
  <span m="2173840">of</span> <span m="2173930">the</span> <span m="2174020">other</span>
  <span m="2174230">hospitals</span> <span m="2174860">in</span> <span m="2174980">the</span>
  <span m="2175040">Boston</span> <span m="2175490">area.</span> <span m="2176510">Each</span>
  <span m="2176750">hospital</span> <span m="2177230">has</span> <span m="2177470">its</span>
  <span m="2177680">own</span> <span m="2178910">digitorata</span> <span m="2179720">for</span>
  <span m="2179960">what</span> <span m="2180200">it</span> <span m="2180320">thinks</span>
  <span m="2180650">is</span> <span m="2180800">most</span> <span m="2181100">important.</span>
  <span m="2183100">And</span> <span m="2183320">I</span> <span m="2183410">think</span>
  <span m="2183650">the</span> <span m="2183770">BI</span> <span m="2184160">just</span>
  <span m="2184400">didn't</span> <span m="2185960">prioritize</span> <span m="2186770">it</span>
  <span m="2187040">as</span> <span m="2187250">much</span> <span m="2187550">as</span>
  <span m="2187670">some</span> <span m="2187910">of</span> <span m="2187970">the</span>
  <span m="2188090">other</span> <span m="2188270">hospitals.</span></p><p><span m="2191180">OK,</span>
  <span m="2191870">so</span> <span m="2192110">then</span> <span m="2192320">I</span>
  <span m="2192440">said,</span> <span m="2192680">well,</span> <span m="2193250">if</span>
  <span m="2193430">you</span> <span m="2193580">look</span> <span m="2193790">at</span>
  <span m="2193910">prescriptions,</span> <span m="2196950">how</span> <span m="2197180">often</span>
  <span m="2197540">are</span> <span m="2197690">they</span> <span m="2197870">given?</span>
  <span m="2198260">So</span> <span m="2198500">remember,</span> <span m="2198950">we</span>
  <span m="2199100">have</span> <span m="2199280">about</span> <span m="2199610">60,000</span>
  <span m="2200660">ICU</span> <span m="2201200">stays.</span> <span m="2202310">And</span>
  <span m="2202520">so</span> <span m="2202940">iso-osmotic</span> <span m="2203900">dextrose</span>
  <span m="2205160">was</span> <span m="2205400">given</span> <span m="2205920">87,000</span>
  <span m="2206930">times</span> <span m="2209810">to</span> <span m="2209940">various</span>
  <span m="2210390">people.</span> <span m="2211200">Sodium</span> <span m="2211680">chloride</span>
  <span m="2212250">0.9</span> <span m="2212880">percent</span> <span m="2213390">flush.</span>
  <span m="2214090">Do</span> <span m="2214170">you</span> <span m="2214230">know</span>
  <span m="2214380">what</span> <span m="2214530">that</span> <span m="2214770">is?</span>
  <span m="2216960">Have</span> <span m="2217080">you</span> <span m="2217200">ever</span>
  <span m="2217410">had</span> <span m="2217590">an</span> <span m="2217710">IV?</span>
  <span m="2219360">So</span> <span m="2220110">periodically,</span> <span m="2220950">the</span>
  <span m="2221070">nurse</span> <span m="2221400">comes</span> <span m="2221760">by</span>
  <span m="2222000">and</span> <span m="2222120">squirts</span> <span m="2222720">a</span>
  <span m="2222750">little</span> <span m="2222990">bit</span> <span m="2223200">of</span>
  <span m="2223290">stuff</span> <span m="2223970">in</span> <span m="2224160">the</span>
  <span m="2224310">IV</span> <span m="2224670">to</span> <span m="2224850">make</span>
  <span m="2225060">sure</span> <span m="2225300">that</span> <span m="2225510">it</span>
  <span m="2225630">hasn't</span> <span m="2225960">clogged</span> <span m="2226410">up.</span>
  <span m="2227130">That's</span> <span m="2227400">what</span> <span m="2227550">that</span>
  <span m="2227790">is.</span></p><p><span m="2229920">Insulin,</span> <span m="2232030">SW.</span>
  <span m="2232950">I</span> <span m="2233070">don't</span> <span m="2233190">know.</span>
  <span m="2233420">Salt</span> <span m="2233640">water?</span> <span m="2234480">I</span>
  <span m="2234580">don't</span> <span m="2234600">know</span> <span m="2234760">what</span>
  <span m="2235140">SW is.</span> <span m="2236730">Magnesium</span> <span m="2237360">sulfate,</span>
  <span m="2238410">dextrose</span> <span m="2239040">five</span> <span m="2239400">in</span>
  <span m="2239520">water.</span> <span m="2240670">Furosimide</span> <span m="2241470">is</span>
  <span m="2241620">a</span> <span m="2241650">diuretic.</span> <span m="2242340">Potassium</span>
  <span m="2243000">chloride</span> <span m="2244050">replenishes</span> <span m="2244800">potassium</span>
  <span m="2246030">that</span> <span m="2246180">people</span> <span m="2246570">are</span>
  <span m="2246660">often</span> <span m="2247440">low</span> <span m="2247740">on.</span>
  <span m="2249330">And</span> <span m="2249510">then</span> <span m="2249750">you</span>
  <span m="2249900">go,</span> <span m="2250770">so</span> <span m="2251010">why</span>
  <span m="2251400">is</span> <span m="2251610">there</span> <span m="2252420">this</span>
  <span m="2252790">D5W</span> <span m="2253920">and</span> <span m="2254070">that</span>
  <span m="2254430">D5W?</span> <span m="2256590">And</span> <span m="2256740">that's</span>
  <span m="2256980">probably</span> <span m="2257400">some</span> <span m="2257730">data</span>
  <span m="2258630">in</span> <span m="2258810">the</span> <span m="2258900">system,</span>
  <span m="2260200">OK?</span> <span m="2262080">One</span> <span m="2262320">of</span>
  <span m="2262470">them</span> <span m="2262710">has</span> <span m="2263910">an</span>
  <span m="2264030">NDC</span> <span m="2264600">code</span> <span m="2264930">associated</span>
  <span m="2265710">with</span> <span m="2265950">it</span> <span m="2266130">and</span>
  <span m="2266220">the</span> <span m="2266310">other</span> <span m="2266490">one</span>
  <span m="2266730">doesn't</span> <span m="2267810">but</span> <span m="2268020">probably</span>
  <span m="2268560">should.</span> <span m="2269680">Yeah.</span></p><p><span m="2270377">AUDIENCE:</span>
  <span m="2270620">I was actually</span> <span m="2270864">going to ask,</span> <span
  m="2271351">does</span> <span m="2271840">yours</span> <span m="2272070">mean</span>
  <span m="2272490">that</span> <span m="2272890">they're standard</span> <span m="2273290">across</span>
  <span m="2273690">hospitals</span> <span m="2274155">or just that</span> <span m="2274620">we
  don't</span> <span m="2275085">have</span> <span m="2275550">the data?</span></p><p><span
  m="2277410">PROFESSOR:</span> <span m="2277552">The</span> <span m="2277980">NDC</span>
  <span m="2278580">code</span> <span m="2279570">should</span> <span m="2279930">be</span>
  <span m="2280110">standard</span> <span m="2280710">across</span> <span m="2281310">the</span>
  <span m="2281430">country,</span> <span m="2282300">because</span> <span m="2282720">those</span>
  <span m="2283020">are</span> <span m="2283140">FDA</span> <span m="2283650">assigned</span>
  <span m="2284070">codes.</span> <span m="2285120">But</span> <span m="2285390">not</span>
  <span m="2285600">every</span> <span m="2285840">hospital</span> <span m="2286320">uses</span>
  <span m="2286800">them,</span> <span m="2288100">OK?</span> <span m="2288810">And</span>
  <span m="2288990">for</span> <span m="2289200">the</span> <span m="2289320">ones</span>
  <span m="2289620">that</span> <span m="2289830">say</span> <span m="2290100">zero,</span>
  <span m="2290730">I'm</span> <span m="2290880">not</span> <span m="2291120">sure</span>
  <span m="2291450">why</span> <span m="2292230">they're</span> <span m="2292500">not</span>
  <span m="2292770">associated</span> <span m="2293490">with</span> <span m="2293700">a</span>
  <span m="2293760">code</span> <span m="2294210">in</span> <span m="2294360">this</span>
  <span m="2294960">hospital's</span> <span m="2296220">database.</span></p><p><span
  m="2298220">OK,</span> <span m="2301980">next</span> <span m="2302310">most</span>
  <span m="2302580">common,</span> <span m="2303190">you</span> <span m="2303270">see</span>
  <span m="2303990">normal</span> <span m="2304380">saline,</span> <span m="2306990">0.9</span>
  <span m="2307620">percent</span> <span m="2308100">sodium</span> <span m="2308550">chloride.</span>
  <span m="2309570">So</span> <span m="2309660">that</span> <span m="2309810">was</span>
  <span m="2309990">the</span> <span m="2310080">same</span> <span m="2310410">stuff</span>
  <span m="2310800">as</span> <span m="2310980">the</span> <span m="2311100">flush</span>
  <span m="2311460">solution</span> <span m="2312570">but</span> <span m="2312810">this</span>
  <span m="2313020">time</span> <span m="2313290">not</span> <span m="2313530">being</span>
  <span m="2313800">used</span> <span m="2314130">for</span> <span m="2314310">flush.</span>
  <span m="2315450">Metoprolol</span> <span m="2316280">is</span> <span m="2316470">a</span>
  <span m="2316560">beta</span> <span m="2316860">blocker.</span> <span m="2318270">Here's</span>
  <span m="2318570">another</span> <span m="2319020">insulin</span> <span m="2319650">this</span>
  <span m="2319890">time</span> <span m="2320130">with</span> <span m="2320400">an</span>
  <span m="2320520">NDC</span> <span m="2321060">code,</span> <span m="2322480">et</span>
  <span m="2322780">cetera.</span></p><p><span m="2323760">I</span> <span m="2324060">love</span>
  <span m="2324510">bag</span> <span m="2325080">and</span> <span m="2325320">vial,</span>
  <span m="2326418">OK?</span> <span m="2328410">So</span> <span m="2329250">these</span>
  <span m="2329460">are</span> <span m="2329580">not</span> <span m="2329820">exactly</span>
  <span m="2330330">medications.</span> <span m="2331680">A</span> <span m="2331740">bag</span>
  <span m="2332280">is</span> <span m="2333030">literally</span> <span m="2333690">like</span>
  <span m="2333990">a</span> <span m="2334350">baggy</span> <span m="2335370">that</span>
  <span m="2335910">they</span> <span m="2336120">put</span> <span m="2336360">something</span>
  <span m="2336870">into,</span> <span m="2337760">and</span> <span m="2337980">a</span>
  <span m="2338040">vial</span> <span m="2338520">is</span> <span m="2338700">literally</span>
  <span m="2339210">something</span> <span m="2339690">that</span> <span m="2339870">they</span>
  <span m="2340080">put</span> <span m="2340500">pills</span> <span m="2340890">in.</span>
  <span m="2341700">And</span> <span m="2342000">why</span> <span m="2342330">is</span>
  <span m="2342480">that</span> <span m="2342720">in</span> <span m="2342840">the</span>
  <span m="2342930">database?</span> <span m="2343590">Because</span> <span m="2344010">they</span>
  <span m="2344160">get</span> <span m="2344410">to charge</span> <span m="2344850">for</span>
  <span m="2345120">it,</span> <span m="2346004">OK?</span> <span m="2346830">And</span>
  <span m="2347280">I</span> <span m="2347400">don't</span> <span m="2347550">know</span>
  <span m="2347700">what</span> <span m="2347880">the</span> <span m="2348000">charge
  is,</span> <span m="2348710">but</span> <span m="2348930">it</span> <span m="2348990">wouldn't</span>
  <span m="2349260">surprise</span> <span m="2349830">me</span> <span m="2350010">if</span>
  <span m="2350160">you're</span> <span m="2350280">paying</span> <span m="2351030">$5</span>
  <span m="2351750">for</span> <span m="2351930">a</span> <span m="2351990">plastic</span>
  <span m="2352530">bag</span> <span m="2353430">to</span> <span m="2353580">put</span>
  <span m="2353790">something</span> <span m="2354270">in.</span></p><p><span m="2355870">OK,</span>
  <span m="2356850">so</span> <span m="2357180">if</span> <span m="2357390">we</span>
  <span m="2357510">say,</span> <span m="2357850">well,</span> <span m="2359410">how</span>
  <span m="2359550">many</span> <span m="2359820">pharmacy</span> <span m="2360390">orders</span>
  <span m="2360780">are</span> <span m="2360960">there</span> <span m="2361170">per</span>
  <span m="2361410">admission</span> <span m="2362190">at</span> <span m="2362370">this</span>
  <span m="2362580">hospital,</span> <span m="2363690">and</span> <span m="2363870">the</span>
  <span m="2364020">answer</span> <span m="2364470">is</span> <span m="2365220">a</span>
  <span m="2365310">lot.</span> <span m="2366390">So</span> <span m="2366840">if</span>
  <span m="2367020">you</span> <span m="2367170">look</span> <span m="2367440">at--</span>
  <span m="2368190">it's</span> <span m="2368370">a</span> <span m="2368430">very</span>
  <span m="2368700">long</span> <span m="2369060">tailed</span> <span m="2369450">distribution,</span>
  <span m="2370380">goes</span> <span m="2370680">out</span> <span m="2370860">to</span>
  <span m="2371040">about</span> <span m="2371340">2,500.</span> <span m="2372930">But</span>
  <span m="2373200">you</span> <span m="2373320">see,</span> <span m="2374130">if</span>
  <span m="2374370">I</span> <span m="2374520">blow</span> <span m="2374910">up</span>
  <span m="2375330">just</span> <span m="2375690">the</span> <span m="2376080">numbers</span>
  <span m="2376590">up</span> <span m="2376770">to</span> <span m="2376980">about</span>
  <span m="2377340">200,</span> <span m="2378980">there's</span> <span m="2379590">a</span>
  <span m="2379680">very</span> <span m="2380040">large</span> <span m="2380460">number</span>
  <span m="2381000">of</span> <span m="2381210">people</span> <span m="2381690">with</span>
  <span m="2382470">two</span> <span m="2385350">prescriptions</span> <span m="2387000">filled,</span>
  <span m="2387990">and</span> <span m="2388170">then</span> <span m="2388470">a</span>
  <span m="2388530">fairly</span> <span m="2389820">declining</span> <span m="2390540">number</span>
  <span m="2390960">with</span> <span m="2391650">more.</span> <span m="2392610">And</span>
  <span m="2392760">then</span> <span m="2392940">it's</span> <span m="2393120">a</span>
  <span m="2393180">very</span> <span m="2393480">long</span> <span m="2393780">tail.</span>
  <span m="2394240">So</span> <span m="2394380">can</span> <span m="2394590">you</span>
  <span m="2394710">imagine</span> <span m="2395940">2,500</span> <span m="2396930">things</span>
  <span m="2397780">prescribed</span> <span m="2398400">for</span> <span m="2398670">you</span>
  <span m="2398820">during</span> <span m="2399240">a</span> <span m="2400050">hospital</span>
  <span m="2400560">stay?</span></p><p><span m="2403110">Well,</span> <span m="2403860">a</span>
  <span m="2403920">little</span> <span m="2404160">more</span> <span m="2404430">about</span>
  <span m="2405220">standards,</span> <span m="2405840">so</span> <span m="2406230">NDC</span>
  <span m="2407040">is</span> <span m="2407280">probably</span> <span m="2407700">the</span>
  <span m="2407850">best</span> <span m="2408210">of</span> <span m="2408300">the</span>
  <span m="2408420">coding</span> <span m="2408810">systems.</span> <span m="2410490">And</span>
  <span m="2410760">it's</span> <span m="2411030">developed</span> <span m="2411480">by</span>
  <span m="2411690">the</span> <span m="2411840">FDA.</span> <span m="2413380">The</span>
  <span m="2413430">picture</span> <span m="2413880">up</span> <span m="2414090">on</span>
  <span m="2414240">the</span> <span m="2414330">top</span> <span m="2414660">right</span>
  <span m="2415050">shows</span> <span m="2416460">that</span> <span m="2416760">the</span>
  <span m="2416880">first</span> <span m="2417240">four</span> <span m="2417480">digits</span>
  <span m="2418110">are</span> <span m="2418980">the</span> <span m="2419670">so-called</span>
  <span m="2420210">labeler.</span> <span m="2420870">That's</span> <span m="2421260">usually</span>
  <span m="2421800">the</span> <span m="2421950">person</span> <span m="2422400">who</span>
  <span m="2422550">produced</span> <span m="2423060">the</span> <span m="2423180">drugs,</span>
  <span m="2423660">or</span> <span m="2423810">at</span> <span m="2423930">least</span>
  <span m="2424170">the</span> <span m="2424260">person</span> <span m="2424710">who</span>
  <span m="2424800">distributes</span> <span m="2425490">them.</span> <span m="2426870">The</span>
  <span m="2427380">second</span> <span m="2428010">four</span> <span m="2428400">digit</span>
  <span m="2428820">number</span> <span m="2429450">is</span> <span m="2430590">the</span>
  <span m="2430800">form</span> <span m="2431340">of</span> <span m="2431520">the</span>
  <span m="2431640">drug,</span> <span m="2432490">so</span> <span m="2432630">whether</span>
  <span m="2432960">it's</span> <span m="2433170">capsules,</span> <span m="2433800">or</span>
  <span m="2433920">tablets,</span> <span m="2434610">or</span> <span m="2435510">liquid,</span>
  <span m="2436080">or</span> <span m="2436380">whatever</span> <span m="2437910">and</span>
  <span m="2438150">the</span> <span m="2438240">dose.</span> <span m="2439330">And</span>
  <span m="2439410">then</span> <span m="2439740">the</span> <span m="2441660">last</span>
  <span m="2441990">two</span> <span m="2442170">digits</span> <span m="2442710">are</span>
  <span m="2442920">a</span> <span m="2442980">package</span> <span m="2443490">code</span>
  <span m="2444330">which</span> <span m="2444630">translates</span> <span m="2445380">into</span>
  <span m="2445710">the</span> <span m="2445860">total</span> <span m="2446220">number</span>
  <span m="2446580">of</span> <span m="2446700">doses</span> <span m="2447390">that</span>
  <span m="2447570">are</span> <span m="2447720">in</span> <span m="2447870">a</span>
  <span m="2447930">package,</span> <span m="2449310">right?</span></p><p><span m="2449580">So</span>
  <span m="2449760">this</span> <span m="2450000">is</span> <span m="2450150">a</span>
  <span m="2450210">godsend.</span> <span m="2451440">And</span> <span m="2451680">all</span>
  <span m="2451950">of</span> <span m="2452100">the</span> <span m="2452220">robotic</span>
  <span m="2452790">pharmacies</span> <span m="2453630">and</span> <span m="2453750">so</span>
  <span m="2453990">on</span> <span m="2454170">rely</span> <span m="2454770">on</span>
  <span m="2455580">using</span> <span m="2456060">this</span> <span m="2456270">kind</span>
  <span m="2456540">of</span> <span m="2456630">information</span> <span m="2457810">nowadays.</span>
  <span m="2460500">Unfortunately,</span> <span m="2461460">they</span> <span m="2461670">ran</span>
  <span m="2462060">out</span> <span m="2462390">of</span> <span m="2463320">four</span>
  <span m="2463620">digit</span> <span m="2463980">numbers,</span> <span m="2465180">and</span>
  <span m="2465390">so</span> <span m="2465780">there's</span> <span m="2466140">now</span>
  <span m="2466650">a--</span> <span m="2467670">they</span> <span m="2467940">added</span>
  <span m="2468330">an</span> <span m="2468480">extra</span> <span m="2468840">digit,</span>
  <span m="2470130">but</span> <span m="2470430">they</span> <span m="2470610">didn't</span>
  <span m="2470880">do</span> <span m="2471060">it</span> <span m="2471180">systematically,</span>
  <span m="2472150">and</span> <span m="2472290">so</span> <span m="2472530">sometimes</span>
  <span m="2473100">they</span> <span m="2473280">added</span> <span m="2474120">an</span>
  <span m="2474240">extra</span> <span m="2474570">digit</span> <span m="2474930">to</span>
  <span m="2475080">the</span> <span m="2475230">labeler</span> <span m="2475620">and</span>
  <span m="2475920">sometimes</span> <span m="2476520">to</span> <span m="2476670">the</span>
  <span m="2476760">product</span> <span m="2477150">code.</span> <span m="2478180">And</span>
  <span m="2478260">so</span> <span m="2478500">there</span> <span m="2478630">is</span>
  <span m="2478770">a</span> <span m="2478860">nightmare</span> <span m="2479550">of</span>
  <span m="2479700">translations</span> <span m="2480720">between</span> <span m="2481680">the</span>
  <span m="2481860">old</span> <span m="2482100">codes</span> <span m="2482580">and</span>
  <span m="2482730">the</span> <span m="2482820">new</span> <span m="2483030">codes.</span>
  <span m="2483600">And</span> <span m="2483750">you</span> <span m="2483870">have</span>
  <span m="2484050">to</span> <span m="2484170">have</span> <span m="2484380">a</span>
  <span m="2484410">code</span> <span m="2484710">dictionary</span> <span m="2485400">in</span>
  <span m="2485520">order</span> <span m="2485790">to</span> <span m="2486420">do</span>
  <span m="2486600">it</span> <span m="2486690">properly</span> <span m="2487320">and</span>
  <span m="2487440">so</span> <span m="2487680">on.</span></p><p><span m="2488700">OK,</span>
  <span m="2489060">well,</span> <span m="2489780">if</span> <span m="2489930">that</span>
  <span m="2490170">weren't</span> <span m="2490440">good</span> <span m="2490650">enough,</span>
  <span m="2491730">the</span> <span m="2492540">International</span> <span m="2493260">Council</span>
  <span m="2493830">for</span> <span m="2494040">the</span> <span m="2494130">Harmonization</span>
  <span m="2495510">of</span> <span m="2495660">Technical</span> <span m="2496230">requirements</span>
  <span m="2497010">for</span> <span m="2497190">Pharmaceuticals</span> <span m="2498180">for</span>
  <span m="2498390">Human</span> <span m="2498810">Use</span> <span m="2499860">developed</span>
  <span m="2500490">another</span> <span m="2500850">coding</span> <span m="2501270">system</span>
  <span m="2501750">called</span> <span m="2502060">MedDRA,</span> <span m="2502560">which</span>
  <span m="2502800">is</span> <span m="2502950">also</span> <span m="2503310">used</span>
  <span m="2503820">in</span> <span m="2503970">various</span> <span m="2504390">places.</span>
  <span m="2505930">And</span> <span m="2506070">this</span> <span m="2506310">is</span>
  <span m="2506460">an</span> <span m="2506580">international</span> <span m="2507420">standard,</span>
  <span m="2508980">which</span> <span m="2509280">is,</span> <span m="2509430">of</span>
  <span m="2509550">course,</span> <span m="2509880">incompatible</span> <span m="2510720">with</span>
  <span m="2511130">the</span> <span m="2511430">NDC.</span></p><p><span m="2516830">CPT</span>
  <span m="2518100">is</span> <span m="2518400">the</span> <span m="2519630">Common</span>
  <span m="2520050">Procedural</span> <span m="2520860">Terminology,</span> <span
  m="2521850">which</span> <span m="2522090">we'll</span> <span m="2522270">talk</span>
  <span m="2522540">about</span> <span m="2522840">in</span> <span m="2522950">a</span>
  <span m="2522990">little</span> <span m="2523200">bit.</span> <span m="2524040">And</span>
  <span m="2524430">they</span> <span m="2524760">have</span> <span m="2525060">a</span>
  <span m="2525120">subrange</span> <span m="2525870">of</span> <span m="2526020">their</span>
  <span m="2526230">codes</span> <span m="2526860">which</span> <span m="2527310">also</span>
  <span m="2527730">correspond</span> <span m="2528930">to</span> <span m="2529080">medication</span>
  <span m="2529770">administration.</span> <span m="2531400">And</span> <span m="2531450">so</span>
  <span m="2531630">this</span> <span m="2531870">is</span> <span m="2532020">yet</span>
  <span m="2532260">another</span> <span m="2532620">way</span> <span m="2532860">of</span>
  <span m="2532980">coding</span> <span m="2533850">giving</span> <span m="2534210">medicines.</span>
  <span m="2535980">And</span> <span m="2536160">then</span> <span m="2536940">the</span>
  <span m="2539100">HCPCS</span> <span m="2541920">is</span> <span m="2542220">yet</span>
  <span m="2542490">another</span> <span m="2542910">set</span> <span m="2543180">of</span>
  <span m="2543300">codes</span> <span m="2544320">for</span> <span m="2544710">specifying</span>
  <span m="2545550">what</span> <span m="2545760">medicines</span> <span m="2546360">you've</span>
  <span m="2546510">given</span> <span m="2546870">to</span> <span m="2547020">somebody.</span></p><p><span
  m="2549210">And</span> <span m="2549420">then</span> <span m="2551340">I</span>
  <span m="2551490">had</span> <span m="2551700">mentioned</span> <span m="2552210">this</span>
  <span m="2552480">GSN</span> <span m="2553200">number,</span> <span m="2553680">which</span>
  <span m="2553980">apparently</span> <span m="2554820">the</span> <span m="2555120">Beth</span>
  <span m="2555420">Israel</span> <span m="2555840">uses.</span> <span m="2556890">This</span>
  <span m="2557160">as</span> <span m="2557340">a</span> <span m="2557400">commercial</span>
  <span m="2558000">coding</span> <span m="2558450">system</span> <span m="2559350">from</span>
  <span m="2559620">a</span> <span m="2559680">company</span> <span m="2560130">called</span>
  <span m="2560400">First</span> <span m="2560720">Databank</span> <span m="2562170">that</span>
  <span m="2562440">is</span> <span m="2562650">in</span> <span m="2562770">the</span>
  <span m="2562860">business</span> <span m="2563400">of</span> <span m="2563550">trying</span>
  <span m="2563910">to</span> <span m="2564060">produce</span> <span m="2564480">standards.</span>
  <span m="2566310">But</span> <span m="2566850">in</span> <span m="2567000">this</span>
  <span m="2567210">case,</span> <span m="2567570">they're</span> <span m="2567780">producing</span>
  <span m="2568380">ones</span> <span m="2568740">that</span> <span m="2568950">are</span>
  <span m="2569070">pretty</span> <span m="2569400">redundant</span> <span m="2570570">with</span>
  <span m="2570840">other</span> <span m="2571140">existing</span> <span m="2571620">standards.</span>
  <span m="2572280">But</span> <span m="2572460">nevertheless,</span> <span m="2573630">for</span>
  <span m="2573870">historical</span> <span m="2574560">reasons,</span> <span m="2575160">or</span>
  <span m="2575340">for</span> <span m="2575580">whatever</span> <span m="2576000">reasons,</span>
  <span m="2576540">people</span> <span m="2576900">are</span> <span m="2577020">using</span>
  <span m="2577410">these.</span></p><p><span m="2578900">OK,</span> <span m="2579930">enough</span>
  <span m="2580350">of</span> <span m="2580440">drugs.</span> <span m="2581400">So</span>
  <span m="2581580">what</span> <span m="2581820">procedures</span> <span m="2582510">were</span>
  <span m="2582690">done</span> <span m="2582960">to</span> <span m="2583170">a</span>
  <span m="2583230">patient?</span> <span m="2584950">If</span> <span m="2585000">you</span>
  <span m="2585120">look</span> <span m="2585360">in</span> <span m="2585510">MIMIC,</span>
  <span m="2586480">there</span> <span m="2586670">are</span> <span m="2586740">three</span>
  <span m="2587040">tables.</span> <span m="2587880">There's</span> <span m="2588480">procedures</span>
  <span m="2589200">ICD,</span> <span m="2590550">which</span> <span m="2590820">has</span>
  <span m="2591330">ICD-9</span> <span m="2592170">codes</span> <span m="2592710">for</span>
  <span m="2593340">about</span> <span m="2593850">a</span> <span m="2593940">quarter</span>
  <span m="2594300">million</span> <span m="2594690">procedures.</span> <span m="2596550">There's</span>
  <span m="2596810">CPT</span> <span m="2597600">events,</span> <span m="2598200">which</span>
  <span m="2598470">has</span> <span m="2598740">about</span> <span m="2599010">half</span>
  <span m="2599310">a</span> <span m="2599370">million,</span> <span m="2600290">600,000</span>
  <span m="2602940">events</span> <span m="2603540">that</span> <span m="2603750">are</span>
  <span m="2603900">coded</span> <span m="2604890">in</span> <span m="2605070">the</span>
  <span m="2605190">CPT</span> <span m="2605910">terminology.</span> <span m="2607740">And</span>
  <span m="2607920">then</span> <span m="2608950">MetaVision,</span> <span m="2609810">the</span>
  <span m="2609960">newer</span> <span m="2610470">of</span> <span m="2610620">the</span>
  <span m="2610740">two</span> <span m="2610980">systems,</span> <span m="2612090">has</span>
  <span m="2612630">about</span> <span m="2612960">a</span> <span m="2613020">quarter</span>
  <span m="2613410">million</span> <span m="2613830">procedure</span> <span m="2614520">events</span>
  <span m="2615420">that</span> <span m="2615660">are</span> <span m="2615750">coded</span>
  <span m="2616230">in</span> <span m="2616350">that</span> <span m="2616590">system.</span></p><p><span
  m="2617770">So</span> <span m="2617850">some</span> <span m="2618120">examples,</span>
  <span m="2619550">here's</span> <span m="2620880">the</span> <span m="2621030">most</span>
  <span m="2621330">common</span> <span m="2621930">ICD-9</span> <span m="2622710">procedure</span>
  <span m="2623280">codes.</span> <span m="2624300">So</span> <span m="2624750">ICD-9</span>
  <span m="2625500">code</span> <span m="2625810">3893</span> <span m="2628320">of</span>
  <span m="2628560">which</span> <span m="2628860">there</span> <span m="2629070">are</span>
  <span m="2629190">14,000</span> <span m="2630210">instances</span> <span m="2632700">is</span>
  <span m="2633000">venous</span> <span m="2633390">catheterization,</span> <span
  m="2634950">not</span> <span m="2635250">elsewhere</span> <span m="2635730">classified.</span>
  <span m="2637410">So</span> <span m="2637620">what's</span> <span m="2637890">venous</span>
  <span m="2638250">catheterization?</span> <span m="2640710">It's</span> <span m="2640890">when</span>
  <span m="2641070">somebody</span> <span m="2641460">sticks</span> <span m="2641880">an</span>
  <span m="2642000">IV</span> <span m="2642360">in</span> <span m="2642480">your</span>
  <span m="2642630">vein,</span> <span m="2643415">OK?</span></p><p><span m="2645540">Very</span>
  <span m="2645870">common.</span> <span m="2646500">You</span> <span m="2646620">show</span>
  <span m="2646920">up</span> <span m="2647100">at</span> <span m="2647190">a</span>
  <span m="2647220">hospital.</span> <span m="2648270">Before</span> <span m="2648660">they</span>
  <span m="2648840">ask</span> <span m="2649140">you</span> <span m="2649260">your</span>
  <span m="2649410">name,</span> <span m="2649770">they</span> <span m="2649920">stick</span>
  <span m="2650250">an</span> <span m="2650370">IV</span> <span m="2650730">in</span>
  <span m="2650880">your</span> <span m="2651090">arm.</span> <span m="2653800">That's</span>
  <span m="2654060">a</span> <span m="2654120">billable</span> <span m="2654600">event,</span>
  <span m="2654960">too.</span> <span m="2656910">Then</span> <span m="2657780">insertion</span>
  <span m="2658440">of</span> <span m="2658810">an</span> <span m="2659140">endotracheal</span>
  <span m="2660270">tube,</span> <span m="2661440">you</span> <span m="2661560">know,</span>
  <span m="2661740">if</span> <span m="2661860">you're</span> <span m="2662010">having</span>
  <span m="2662340">any</span> <span m="2662670">problems</span> <span m="2663210">like</span>
  <span m="2663480">that,</span> <span m="2663780">they</span> <span m="2664770">stick</span>
  <span m="2665100">something</span> <span m="2665490">down</span> <span m="2665700">your</span>
  <span m="2665850">throat.</span> <span m="2666860">Ventral</span> <span m="2667320">infusion</span>
  <span m="2667860">of</span> <span m="2667980">concentrated</span> <span m="2668790">nutritional</span>
  <span m="2669450">substances,</span> <span m="2670750">so</span> <span m="2670860">if</span>
  <span m="2670950">you're</span> <span m="2671070">not</span> <span m="2671310">able</span>
  <span m="2671580">to</span> <span m="2671760">eat,</span> <span m="2672570">then</span>
  <span m="2672810">they</span> <span m="2672990">feed</span> <span m="2673380">you</span>
  <span m="2673650">through</span> <span m="2674620">a</span> <span m="2674790">stomach</span>
  <span m="2675220">tube,</span> <span m="2675905">OK?</span> <span m="2676290">So</span>
  <span m="2676500">that's</span> <span m="2677040">what</span> <span m="2677310">that</span>
  <span m="2677550">is.</span></p><p><span m="2679620">Continuous</span> <span m="2680370">invasive</span>
  <span m="2680940">mechanical</span> <span m="2681570">ventilation</span> <span m="2682800">for</span>
  <span m="2683010">less</span> <span m="2683310">than</span> <span m="2683490">96</span>
  <span m="2684180">consecutive</span> <span m="2684870">hours,</span> <span m="2685740">so</span>
  <span m="2685950">this</span> <span m="2686250">is</span> <span m="2686400">being</span>
  <span m="2686700">put</span> <span m="2687090">on</span> <span m="2688660">a</span>
  <span m="2688710">ventilator</span> <span m="2689550">that's</span> <span m="2689910">breathing</span>
  <span m="2690330">for</span> <span m="2690600">you,</span> <span m="2691450">et</span>
  <span m="2691470">cetera.</span> <span m="2692080">So</span> <span m="2692190">you</span>
  <span m="2692370">see</span> <span m="2692640">that</span> <span m="2692980">there</span>
  <span m="2693130">is</span> <span m="2693330">a</span> <span m="2693960">very</span>
  <span m="2694230">long</span> <span m="2694500">tail</span> <span m="2694920">of</span>
  <span m="2695040">these.</span> <span m="2696070">So</span> <span m="2696180">those</span>
  <span m="2696450">are</span> <span m="2696540">the</span> <span m="2696720">ICD-9</span>
  <span m="2697470">codes.</span></p><p><span m="2698490">Now,</span> <span m="2698670">CPT</span>
  <span m="2699540">has</span> <span m="2699840">its</span> <span m="2700050">own</span>
  <span m="2700230">procedure</span> <span m="2700830">codes</span> <span m="2702450">that</span>
  <span m="2702720">go</span> <span m="2702960">into</span> <span m="2703240">a</span>
  <span m="2703260">tremendous</span> <span m="2703890">amount</span> <span m="2704160">of</span>
  <span m="2704280">detail.</span> <span m="2705880">So</span> <span m="2706050">for</span>
  <span m="2706230">example,</span> <span m="2706810">this</span> <span m="2706950">is</span>
  <span m="2707130">the</span> <span m="2707250">medicine</span> <span m="2707760">subsection,</span>
  <span m="2709050">and</span> <span m="2709260">it</span> <span m="2709380">shows</span>
  <span m="2709800">you</span> <span m="2710220">the</span> <span m="2710400">kinds</span>
  <span m="2710970">of</span> <span m="2711750">drugs</span> <span m="2712200">that</span>
  <span m="2712470">you're</span> <span m="2712620">being</span> <span m="2713160">administered</span>
  <span m="2714660">that</span> <span m="2715410">are</span> <span m="2715560">involved</span>
  <span m="2716160">in</span> <span m="2717120">dialysis,</span> <span m="2718110">or</span>
  <span m="2719040">psychiatry,</span> <span m="2719940">or</span> <span m="2720330">vaccines,</span>
  <span m="2721110">or</span> <span m="2721260">whatever.</span> <span m="2722730">And</span>
  <span m="2723080">then</span> <span m="2723300">here</span> <span m="2723610">are</span>
  <span m="2723720">the</span> <span m="2723870">surgical</span> <span m="2724770">and</span>
  <span m="2724960">the</span> <span m="2725070">radiological</span> <span m="2726480">codes.</span>
  <span m="2727530">And</span> <span m="2727710">there's</span> <span m="2728010">tons</span>
  <span m="2728370">and</span> <span m="2728520">tons</span> <span m="2728850">of</span>
  <span m="2728970">detail</span> <span m="2729450">on</span> <span m="2729600">these.</span>
  <span m="2729810">Yeah.</span></p><p><span m="2730470">AUDIENCE:</span> <span m="2730575">So</span>
  <span m="2730680">how</span> <span m="2730920">can</span> <span m="2731070">they
  put</span> <span m="2731540">these</span> <span m="2731760">codes</span> <span m="2732130">as</span>
  <span m="2732510">1,000</span> <span m="2733230">to</span> <span m="2733380">1,022?</span>
  <span m="2734760">This</span> <span m="2735030">is</span> <span m="2735360">really</span>
  <span m="2735720">annoying</span> <span m="2736250">for</span> <span m="2736530">anyone--</span></p><p><span
  m="2736800">PROFESSOR:</span> <span m="2736905">No,</span> <span m="2737010">these</span>
  <span m="2737250">are</span> <span m="2737370">categories.</span> <span m="2738790">So</span>
  <span m="2739090">if</span> <span m="2739290">you</span> <span m="2739440">drill</span>
  <span m="2739770">down,</span> <span m="2740510">there's</span> <span m="2744210">a</span>
  <span m="2744270">fanout</span> <span m="2744840">of</span> <span m="2744960">that</span>
  <span m="2745170">tree</span> <span m="2745650">and</span> <span m="2745980">you</span>
  <span m="2746160">get</span> <span m="2746400">down</span> <span m="2746700">to</span>
  <span m="2746850">individual</span> <span m="2747480">codes.</span> <span m="2749300">Just</span>
  <span m="2749670">as</span> <span m="2750210">a</span> <span m="2750300">nasty</span>
  <span m="2750840">surprise,</span> <span m="2752190">CPT</span> <span m="2752910">is</span>
  <span m="2753120">owned</span> <span m="2753510">by</span> <span m="2753780">the</span>
  <span m="2753930">American</span> <span m="2754410">College</span> <span m="2754860">of</span>
  <span m="2754950">Physicians,</span> <span m="2756260">and</span> <span m="2758030">they</span>
  <span m="2758760">could</span> <span m="2759000">sue</span> <span m="2759300">me</span>
  <span m="2759600">if</span> <span m="2759810">I</span> <span m="2759960">showed</span>
  <span m="2760380">you</span> <span m="2760560">the</span> <span m="2760890">actual</span>
  <span m="2761370">codes</span> <span m="2762450">because</span> <span m="2762960">they're</span>
  <span m="2763180">copyrighted.</span> <span m="2766950">And</span> <span m="2767040">you</span>
  <span m="2767160">have</span> <span m="2767280">to</span> <span m="2767400">pay</span>
  <span m="2767670">them</span> <span m="2768150">if</span> <span m="2768870">you</span>
  <span m="2769020">use</span> <span m="2769290">those</span> <span m="2769560">codes.</span>
  <span m="2770550">It's</span> <span m="2770730">crazy.</span></p><p><span m="2773730">OK,</span>
  <span m="2774600">so</span> <span m="2775290">if</span> <span m="2775470">you</span>
  <span m="2775620">look</span> <span m="2775860">at</span> <span m="2775980">the</span>
  <span m="2776130">number</span> <span m="2776850">of</span> <span m="2777240">all
  of</span> <span m="2777630">these</span> <span m="2777930">codes</span> <span m="2778440">per</span>
  <span m="2778770">admission,</span> <span m="2779940">you</span> <span m="2780090">see</span>
  <span m="2780360">a</span> <span m="2780720">distribution</span> <span m="2781500">like</span>
  <span m="2781800">this.</span> <span m="2782760">Or</span> <span m="2783090">if</span>
  <span m="2783270">I</span> <span m="2783390">separate</span> <span m="2783990">them</span>
  <span m="2784170">out,</span> <span m="2784470">you</span> <span m="2784620">see</span>
  <span m="2784860">that</span> <span m="2785520">there</span> <span m="2785670">are</span>
  <span m="2785700">more</span> <span m="2786000">ICD-9</span> <span m="2786810">codes</span>
  <span m="2787620">and</span> <span m="2787830">fewer</span> <span m="2788550">of</span>
  <span m="2788700">the</span> <span m="2788820">CPT</span> <span m="2789540">and</span>
  <span m="2789720">the</span> <span m="2790710">codes</span> <span m="2791130">that</span>
  <span m="2791280">are</span> <span m="2791640">in</span> <span m="2791820">MetaVision.</span>
  <span m="2793050">But</span> <span m="2793260">they</span> <span m="2793470">look</span>
  <span m="2794040">somewhat</span> <span m="2794520">similar</span> <span m="2795060">in</span>
  <span m="2795180">their</span> <span m="2795330">distributions.</span></p><p><span
  m="2797650">OK,</span> <span m="2798270">lab</span> <span m="2798540">measurements.</span>
  <span m="2799930">So</span> <span m="2800070">you</span> <span m="2800190">send</span>
  <span m="2800550">off</span> <span m="2801300">a</span> <span m="2801360">sputum</span>
  <span m="2801810">sample,</span> <span m="2802380">blood,</span> <span m="2802960">urine,</span>
  <span m="2803760">piece</span> <span m="2804090">of</span> <span m="2804210">your</span>
  <span m="2804390">brain,</span> <span m="2805170">something.</span> <span m="2806460">They</span>
  <span m="2806670">stick</span> <span m="2807090">it</span> <span m="2807180">in</span>
  <span m="2807570">some</span> <span m="2807870">goo</span> <span m="2808260">and</span>
  <span m="2808640">measure</span> <span m="2809000">something</span> <span m="2809450">about</span>
  <span m="2809780">it.</span> <span m="2810420">So</span> <span m="2810500">what</span>
  <span m="2810680">is</span> <span m="2810830">it</span> <span m="2810950">that</span>
  <span m="2811130">they're</span> <span m="2811310">measuring?</span></p><p><span
  m="2812330">Well,</span> <span m="2812780">it</span> <span m="2812900">turns</span>
  <span m="2813260">out</span> <span m="2813530">that</span> <span m="2814880">hematocrit</span>
  <span m="2815840">is</span> <span m="2816050">the</span> <span m="2816170">most</span>
  <span m="2816470">common</span> <span m="2816860">measurement.</span> <span m="2817460">So</span>
  <span m="2817670">this</span> <span m="2817940">is</span> <span m="2818540">how</span>
  <span m="2818660">much</span> <span m="2819830">hemoglobin</span> <span m="2820550">is</span>
  <span m="2820730">in</span> <span m="2820850">your</span> <span m="2821030">blood,</span>
  <span m="2822480">or</span> <span m="2822670">what</span> <span m="2822920">fraction</span>
  <span m="2823730">in</span> <span m="2823910">your</span> <span m="2824060">blood,</span>
  <span m="2824960">and</span> <span m="2825290">is</span> <span m="2825500">very</span>
  <span m="2825770">important</span> <span m="2826370">for</span> <span m="2826730">sick</span>
  <span m="2827030">people.</span> <span m="2828750">And</span> <span m="2829250">the</span>
  <span m="2829400">second</span> <span m="2829820">most</span> <span m="2830270">important</span>
  <span m="2830950">is</span> <span m="2831110">potassium,</span> <span m="2831890">then</span>
  <span m="2831980">sodium</span> <span m="2832490">creatinine,</span> <span m="2833060">chloride,</span>
  <span m="2834300">urea</span> <span m="2834680">nitrogen,</span> <span m="2835340">bicarbonate,</span>
  <span m="2836150">et</span> <span m="2836420">cetera.</span> <span m="2836770">So</span>
  <span m="2837020">this</span> <span m="2837250">is</span> <span m="2837410">a</span>
  <span m="2837470">long,</span> <span m="2837860">long</span> <span m="2838160">list</span>
  <span m="2838700">of</span> <span m="2838850">different</span> <span m="2839210">things</span>
  <span m="2839600">that</span> <span m="2839750">can</span> <span m="2839990">be</span>
  <span m="2840140">measured,</span> <span m="2841070">and</span> <span m="2841190">all</span>
  <span m="2841370">the</span> <span m="2841490">stuff</span> <span m="2841850">is</span>
  <span m="2842030">in</span> <span m="2842120">the</span> <span m="2842240">database.</span></p><p><span
  m="2843990">So</span> <span m="2844100">for</span> <span m="2844310">example,</span>
  <span m="2845340">here's</span> <span m="2845600">patient</span> <span m="2846240">number</span>
  <span m="2846530">two</span> <span m="2847580">in</span> <span m="2847820">the</span>
  <span m="2848030">database.</span> <span m="2849770">And</span> <span m="2852701">on</span>
  <span m="2853160">July</span> <span m="2853550">17</span> <span m="2854300">of</span>
  <span m="2854420">2138,</span> <span m="2857420">this</span> <span m="2857690">is</span>
  <span m="2857840">part</span> <span m="2858110">of</span> <span m="2858230">the</span>
  <span m="2858380">deidentification</span> <span m="2859490">process</span> <span
  m="2860120">to</span> <span m="2860660">make</span> <span m="2860960">it</span>
  <span m="2861050">difficult</span> <span m="2861590">to</span> <span m="2861740">figure</span>
  <span m="2862130">out</span> <span m="2862730">who</span> <span m="2862880">the</span>
  <span m="2863000">patient</span> <span m="2863480">actually</span> <span m="2863990">is.</span>
  <span m="2865070">This</span> <span m="2865370">person</span> <span m="2866480">got</span>
  <span m="2868670">a</span> <span m="2868760">test</span> <span m="2869210">for</span>
  <span m="2871160">their</span> <span m="2871400">blood</span> <span m="2872450">and</span>
  <span m="2874190">they</span> <span m="2874400">reported</span> <span m="2875060">atypical</span>
  <span m="2875780">lymphocytes.</span></p><p><span m="2877670">So</span> <span m="2877850">there</span>
  <span m="2877990">are</span> <span m="2878030">a</span> <span m="2878090">couple</span>
  <span m="2878420">of</span> <span m="2878540">interesting</span> <span m="2879050">things</span>
  <span m="2879410">to</span> <span m="2879560">note</span> <span m="2879830">here.</span>
  <span m="2881940">One</span> <span m="2882170">is</span> <span m="2883040">that</span>
  <span m="2884060">some</span> <span m="2884420">things</span> <span m="2884810">have</span>
  <span m="2885050">a</span> <span m="2885110">value</span> <span m="2885710">and</span>
  <span m="2885860">others</span> <span m="2886220">don't.</span> <span m="2887130">So</span>
  <span m="2887270">this</span> <span m="2887480">is</span> <span m="2887660">a</span>
  <span m="2887720">qualitative</span> <span m="2888440">measure,</span> <span m="2889100">so</span>
  <span m="2889340">there's</span> <span m="2889580">no</span> <span m="2889760">value</span>
  <span m="2890210">associated</span> <span m="2890930">with</span> <span m="2891140">it.</span>
  <span m="2891800">Just</span> <span m="2892070">the</span> <span m="2892190">fact</span>
  <span m="2892850">of</span> <span m="2893030">the</span> <span m="2893150">label</span>
  <span m="2893840">tells</span> <span m="2894200">you</span> <span m="2894320">what</span>
  <span m="2894530">the</span> <span m="2894650">result</span> <span m="2895100">of</span>
  <span m="2895250">the</span> <span m="2895370">test</span> <span m="2895700">was.</span>
  <span m="2896930">The</span> <span m="2897050">other</span> <span m="2897290">thing</span>
  <span m="2897500">that's</span> <span m="2897710">interesting</span> <span m="2898760">is</span>
  <span m="2898970">this</span> <span m="2899180">last</span> <span m="2899540">column,</span>
  <span m="2900120">which</span> <span m="2900290">is</span> <span m="2900440">LOINK,</span>
  <span m="2901160">and</span> <span m="2901310">I'll</span> <span m="2901430">say</span>
  <span m="2901700">a</span> <span m="2901760">word</span> <span m="2902030">about</span>
  <span m="2902360">that</span> <span m="2902780">in</span> <span m="2902900">a</span>
  <span m="2902960">minute--</span> <span m="2905390">actually</span> <span m="2905810">right</span>
  <span m="2906110">now.</span></p><p><span m="2908030">So</span> <span m="2908270">LOINK</span>
  <span m="2908720">is</span> <span m="2908990">the</span> <span m="2909140">Logical</span>
  <span m="2909830">Observation</span> <span m="2910670">Identifiers</span> <span
  m="2911660">Names</span> <span m="2912140">and</span> <span m="2912320">Codes.</span>
  <span m="2913730">It</span> <span m="2913880">was</span> <span m="2914120">developed</span>
  <span m="2914630">by</span> <span m="2915110">our</span> <span m="2915260">colleagues</span>
  <span m="2915950">at</span> <span m="2916220">Regenstrief</span> <span m="2916970">Clinic</span>
  <span m="2917450">in</span> <span m="2917630">Indiana</span> <span m="2919320">about</span>
  <span m="2920000">15</span> <span m="2920480">years</span> <span m="2920810">ago,</span>
  <span m="2921360">maybe</span> <span m="2921560">20</span> <span m="2921890">years</span>
  <span m="2922190">ago</span> <span m="2922430">at</span> <span m="2922550">this</span>
  <span m="2922730">point.</span> <span m="2924110">And</span> <span m="2924590">the</span>
  <span m="2924830">attempt</span> <span m="2925310">was</span> <span m="2925640">to</span>
  <span m="2925790">say</span> <span m="2926720">every</span> <span m="2927080">different</span>
  <span m="2927530">type</span> <span m="2927890">of</span> <span m="2928040">laboratory</span>
  <span m="2928700">test</span> <span m="2929210">ought</span> <span m="2929390">to</span>
  <span m="2929480">have</span> <span m="2929780">a</span> <span m="2929840">unique</span>
  <span m="2930260">name,</span> <span m="2931890">and</span> <span m="2932030">they</span>
  <span m="2932240">ought</span> <span m="2932420">to</span> <span m="2932480">be</span>
  <span m="2932660">hierarchical</span> <span m="2933680">so</span> <span m="2933980">that</span>
  <span m="2934400">if</span> <span m="2934610">you</span> <span m="2934760">have,</span>
  <span m="2935000">for</span> <span m="2935270">example,</span> <span m="2936200">three</span>
  <span m="2936500">different</span> <span m="2936920">ways</span> <span m="2937220">of</span>
  <span m="2937340">measuring</span> <span m="2937880">serum</span> <span m="2938240">potassium,</span>
  <span m="2939590">that</span> <span m="2939860">they're</span> <span m="2940070">related</span>
  <span m="2940580">to</span> <span m="2940790">each</span> <span m="2941000">other</span>
  <span m="2941390">but</span> <span m="2941700">that</span> <span m="2941910">they're</span>
  <span m="2942500">distinct</span> <span m="2942950">from</span> <span m="2943220">each</span>
  <span m="2943400">other,</span> <span m="2943700">because</span> <span m="2944570">there</span>
  <span m="2944750">may</span> <span m="2944930">be</span> <span m="2945080">circumstances</span>
  <span m="2946130">under</span> <span m="2946400">which</span> <span m="2946760">the</span>
  <span m="2947210">errors</span> <span m="2947600">that</span> <span m="2947810">you</span>
  <span m="2947930">get</span> <span m="2948170">from</span> <span m="2948470">one</span>
  <span m="2948680">measurement</span> <span m="2949640">versus</span> <span m="2950120">another</span>
  <span m="2950600">are</span> <span m="2950750">different.</span></p><p><span m="2953310">And</span>
  <span m="2953360">so</span> <span m="2953960">this</span> <span m="2954470">is</span>
  <span m="2955220">the</span> <span m="2955340">standard</span> <span m="2955970">way.</span>
  <span m="2956450">If</span> <span m="2956630">you</span> <span m="2956810">send</span>
  <span m="2957200">off</span> <span m="2957470">your</span> <span m="2957650">blood</span>
  <span m="2957920">sample</span> <span m="2958400">to</span> <span m="2958610">a</span>
  <span m="2958670">lab,</span> <span m="2959630">they</span> <span m="2959900">send</span>
  <span m="2960260">back</span> <span m="2960740">a</span> <span m="2960830">string</span>
  <span m="2961310">like</span> <span m="2961610">this</span> <span m="2962480">to</span>
  <span m="2962690">the</span> <span m="2962810">hospital</span> <span m="2963440">or</span>
  <span m="2963590">to</span> <span m="2963770">your</span> <span m="2963920">doctor's</span>
  <span m="2964430">office</span> <span m="2965420">that</span> <span m="2965690">says,</span>
  <span m="2967220">it's</span> <span m="2967460">coded</span> <span m="2968000">in</span>
  <span m="2968150">this</span> <span m="2968450">OBX</span> <span m="2969170">coding</span>
  <span m="2969620">system,</span> <span m="2970250">and</span> <span m="2970980">here</span>
  <span m="2971290">is</span> <span m="2971570">the</span> <span m="2972710">LOINK</span>
  <span m="2973070">code,</span> <span m="2973770">and</span> <span m="2974360">this</span>
  <span m="2974720">is</span> <span m="2975020">the</span> <span m="2975410">SNOMED</span>
  <span m="2976040">interpretation.</span> <span m="2978050">And</span> <span m="2978290">so</span>
  <span m="2978530">this</span> <span m="2978740">string</span> <span m="2979760">is</span>
  <span m="2980030">the</span> <span m="2980150">way</span> <span m="2980390">that</span>
  <span m="2980660">your</span> <span m="2981040">hospital's</span> <span m="2981600">EHR</span>
  <span m="2982430">or</span> <span m="2982640">your</span> <span m="2982820">doctor's</span>
  <span m="2983330">office</span> <span m="2983660">system</span> <span m="2984560">figures</span>
  <span m="2985010">out</span> <span m="2985190">what</span> <span m="2985400">the</span>
  <span m="2985520">result</span> <span m="2985970">of</span> <span m="2986060">the</span>
  <span m="2986210">test</span> <span m="2986540">was.</span></p><p><span m="2987740">HL7</span>
  <span m="2988580">is</span> <span m="2988790">this</span> <span m="2989210">30-something</span>
  <span m="2990440">year</span> <span m="2990680">old</span> <span m="2990950">organization</span>
  <span m="2992300">that</span> <span m="2992480">has</span> <span m="2992690">been</span>
  <span m="2992870">working</span> <span m="2993320">on</span> <span m="2993470">standardizing</span>
  <span m="2994370">stuff</span> <span m="2994670">like</span> <span m="2994880">this.</span>
  <span m="2995660">And</span> <span m="2995840">LOINK</span> <span m="2996250">is</span>
  <span m="2996440">part</span> <span m="2996740">of</span> <span m="2997880">their</span>
  <span m="2998090">standardization.</span> <span m="3000260">So</span> <span m="3000430">if</span>
  <span m="3000580">you</span> <span m="3000700">look</span> <span m="3000910">at</span>
  <span m="3001030">these,</span> <span m="3001360">you</span> <span m="3001480">say,</span>
  <span m="3001720">well,</span> <span m="3002470">again,</span> <span m="3002830">how</span>
  <span m="3003010">many</span> <span m="3003280">tests</span> <span m="3003880">per</span>
  <span m="3004180">admission?</span> <span m="3005500">Again,</span> <span m="3005830">a</span>
  <span m="3005890">huge,</span> <span m="3006400">long</span> <span m="3006730">tail</span>
  <span m="3007630">up</span> <span m="3007780">to</span> <span m="3007990">about</span>
  <span m="3008320">15,000</span> <span m="3009400">for</span> <span m="3009670">a</span>
  <span m="3009730">very</span> <span m="3010000">small</span> <span m="3010330">number</span>
  <span m="3011170">of</span> <span m="3011320">patients.</span></p><p><span m="3014150">If</span>
  <span m="3014230">you</span> <span m="3014380">look</span> <span m="3014800">at</span>
  <span m="3015700">lab</span> <span m="3016000">tests</span> <span m="3016360">per</span>
  <span m="3016600">admission,</span> <span m="3018100">you</span> <span m="3018370">can</span>
  <span m="3020110">do</span> <span m="3020350">a</span> <span m="3020410">log</span>
  <span m="3020710">transform</span> <span m="3021490">and</span> <span m="3021610">get</span>
  <span m="3021850">something</span> <span m="3022270">that</span> <span m="3022450">looks</span>
  <span m="3022750">like</span> <span m="3022990">a</span> <span m="3023050">more</span>
  <span m="3023290">reasonable</span> <span m="3023830">distribution.</span> <span
  m="3025120">By</span> <span m="3025330">the</span> <span m="3025420">way,</span>
  <span m="3025570">that's</span> <span m="3025780">a</span> <span m="3025840">very</span>
  <span m="3026080">generic</span> <span m="3026620">lesson</span> <span m="3027260">when</span>
  <span m="3027550">we're</span> <span m="3027940">going</span> <span m="3028240">to</span>
  <span m="3028390">do</span> <span m="3028570">analyses</span> <span m="3029290">of</span>
  <span m="3029410">these</span> <span m="3029650">data,</span> <span m="3030580">is</span>
  <span m="3030790">that,</span> <span m="3031000">often,</span> <span m="3031480">doing
  a</span> <span m="3031840">transform</span> <span m="3032680">of</span> <span m="3032800">some</span>
  <span m="3033070">sort,</span> <span m="3033550">like</span> <span m="3033850">in</span>
  <span m="3034000">this</span> <span m="3034180">case,</span> <span m="3034520">a</span>
  <span m="3034570">log,</span> <span m="3035890">takes</span> <span m="3036280">some</span>
  <span m="3036580">funny</span> <span m="3036940">looking</span> <span m="3037300">distribution</span>
  <span m="3038110">and</span> <span m="3038230">turns</span> <span m="3038590">it</span>
  <span m="3038710">into</span> <span m="3038950">something</span> <span m="3039400">that</span>
  <span m="3039610">looks</span> <span m="3040270">plausibly</span> <span m="3040990">normal,</span>
  <span m="3041680">which</span> <span m="3041950">is</span> <span m="3042460">better</span>
  <span m="3042790">for</span> <span m="3043060">a</span> <span m="3043120">lot</span>
  <span m="3043360">of</span> <span m="3043480">the</span> <span m="3043600">techniques</span>
  <span m="3044110">we</span> <span m="3044200">use.</span> <span m="3044490">Yeah.</span></p><p><span
  m="3045560">AUDIENCE:</span> <span m="3045777">[INAUDIBLE]</span> <span m="3049900">means</span>
  <span m="3050110">the</span> <span m="3050200">same</span> <span m="3050540">thing?</span>
  <span m="3050630">Like, for instance--</span></p><p><span m="3051070">PROFESSOR:</span>
  <span m="3051250">Yes.</span></p><p><span m="3051760">AUDIENCE:</span> <span m="3051825">--hematocrit</span>
  <span m="3052850">[INAUDIBLE]</span></p><p><span m="3053950">PROFESSOR:</span> <span
  m="3054130">Yes</span></p><p><span m="3054310">AUDIENCE:</span> <span m="3054520">--same?</span></p><p><span
  m="3055150">PROFESSOR:</span> <span m="3055300">Yes</span></p><p><span m="3055450">AUDIENCE:</span>
  <span m="3055640">Always</span> <span m="3056210">same?</span></p><p><span m="3056590">PROFESSOR:</span>
  <span m="3056725">Yes,</span> <span m="3057130">that's</span> <span m="3057430">the</span>
  <span m="3057550">whole</span> <span m="3057790">idea</span> <span m="3058210">of</span>
  <span m="3058360">creating</span> <span m="3058900">the</span> <span m="3058990">standard.</span>
  <span m="3060520">And</span> <span m="3060670">that</span> <span m="3060850">has</span>
  <span m="3061120">been</span> <span m="3061360">pretty</span> <span m="3061630">successful,</span>
  <span m="3062740">pretty</span> <span m="3062980">successfully</span> <span m="3063700">adopted.</span></p><p><span
  m="3066160">OK,</span> <span m="3067370">chart</span> <span m="3067720">events.</span>
  <span m="3068130">So</span> <span m="3068320">these</span> <span m="3068620">are</span>
  <span m="3068740">the</span> <span m="3068860">things</span> <span m="3069280">that</span>
  <span m="3069490">nurses</span> <span m="3070000">typically</span> <span m="3070540">enter</span>
  <span m="3071140">at</span> <span m="3071350">the</span> <span m="3071470">bedside.</span>
  <span m="3073220">And</span> <span m="3073330">so</span> <span m="3074260">there</span>
  <span m="3074560">are</span> <span m="3074830">5.1,</span> <span m="3076030">5.2</span>
  <span m="3076780">million</span> <span m="3077230">heart</span> <span m="3077560">rates</span>
  <span m="3078370">measured</span> <span m="3078910">in</span> <span m="3079060">the</span>
  <span m="3079120">MIMIC</span> <span m="3079420">database.</span> <span m="3080940">And</span>
  <span m="3082460">calprevslig</span> <span m="3084150">is</span> <span m="3084790">an</span>
  <span m="3084910">artifact.</span> <span m="3086080">It</span> <span m="3086230">exists</span>
  <span m="3086770">in</span> <span m="3086920">every</span> <span m="3087190">record.</span>
  <span m="3088430">And</span> <span m="3088870">it's</span> <span m="3089080">some</span>
  <span m="3089470">calibration</span> <span m="3090790">something</span> <span m="3091210">or</span>
  <span m="3091330">other</span> <span m="3091600">that</span> <span m="3091750">doesn't</span>
  <span m="3092080">mean</span> <span m="3092320">anything.</span> <span m="3093130">I've</span>
  <span m="3093250">never</span> <span m="3093550">been</span> <span m="3093700">able</span>
  <span m="3093940">to</span> <span m="3094000">figure</span> <span m="3094360">out</span>
  <span m="3094510">exactly</span> <span m="3095020">what</span> <span m="3095200">it</span>
  <span m="3095290">is.</span></p><p><span m="3096090">SPO2</span> <span m="3097330">is</span>
  <span m="3097600">the</span> <span m="3097870">partial</span> <span m="3098320">pressure</span>
  <span m="3098770">of</span> <span m="3098920">oxygen</span> <span m="3099970">in</span>
  <span m="3100120">your</span> <span m="3100300">blood.</span> <span m="3101160">If</span>
  <span m="3101250">you</span> <span m="3101390">use</span> <span m="3101620">a</span>
  <span m="3101680">pulse</span> <span m="3102070">oximeter,</span> <span m="3102730">that's</span>
  <span m="3103105">what that's</span> <span m="3103480">measuring.</span> <span m="3104770">Respiratory</span>
  <span m="3105520">rate,</span> <span m="3105820">heart</span> <span m="3106120">rhythm,</span>
  <span m="3106930">ectopy</span> <span m="3107260">type,</span> <span m="3107470">dot,</span>
  <span m="3107710">dot,</span> <span m="3107950">dot.</span></p><p><span m="3109050">Now,</span>
  <span m="3109590">you</span> <span m="3109800">might</span> <span m="3110100">be</span>
  <span m="3110220">troubled</span> <span m="3110760">by</span> <span m="3110970">the</span>
  <span m="3111090">fact</span> <span m="3111510">that</span> <span m="3111690">here
  is</span> <span m="3112020">heart</span> <span m="3112290">rate</span> <span m="3112560">again,</span>
  <span m="3115140">right?</span> <span m="3115830">But</span> <span m="3116040">I've</span>
  <span m="3116220">already</span> <span m="3116520">shown</span> <span m="3116880">you</span>
  <span m="3117030">this,</span> <span m="3117540">that</span> <span m="3118500">heart</span>
  <span m="3118830">rate</span> <span m="3119280">in</span> <span m="3120360">CareVue</span>
  <span m="3121200">and</span> <span m="3121380">heart</span> <span m="3121710">rate</span>
  <span m="3122070">in</span> <span m="3122280">MetaVision</span> <span m="3123510">were</span>
  <span m="3123730">coded</span> <span m="3124740">under</span> <span m="3125130">different</span>
  <span m="3125610">codes</span> <span m="3126870">in</span> <span m="3127110">the</span>
  <span m="3127230">joint</span> <span m="3127620">system</span> <span m="3128340">that</span>
  <span m="3128580">we</span> <span m="3128760">created</span> <span m="3129330">out</span>
  <span m="3129480">of</span> <span m="3129600">those</span> <span m="3129870">two</span>
  <span m="3130020">databases.</span> <span m="3131940">And</span> <span m="3132120">so</span>
  <span m="3133200">you</span> <span m="3133410">have</span> <span m="3133620">to</span>
  <span m="3133740">take</span> <span m="3134010">care</span> <span m="3134430">of</span>
  <span m="3135600">figuring</span> <span m="3136170">out</span> <span m="3136470">what's</span>
  <span m="3136830">what</span> <span m="3137580">if</span> <span m="3137790">you're</span>
  <span m="3138120">trying</span> <span m="3138450">to</span> <span m="3138570">analyze</span>
  <span m="3139080">this</span> <span m="3139290">data.</span> <span m="3140160">Not</span>
  <span m="3140370">only</span> <span m="3140640">do</span> <span m="3140790">we</span>
  <span m="3140910">have</span> <span m="3141120">that</span> <span m="3141330">problem</span>
  <span m="3141960">of</span> <span m="3142350">different</span> <span m="3142830">age</span>
  <span m="3143160">distributions</span> <span m="3144570">across</span> <span m="3144990">the</span>
  <span m="3145170">two</span> <span m="3145440">different</span> <span m="3145770">data</span>
  <span m="3146140">sets,</span> <span m="3147040">but</span> <span m="3147180">we</span>
  <span m="3147300">also</span> <span m="3147660">just</span> <span m="3147930">have</span>
  <span m="3148110">the</span> <span m="3148200">mechanical</span> <span m="3148860">problem</span>
  <span m="3149820">that</span> <span m="3150030">there</span> <span m="3150210">will</span>
  <span m="3150420">be</span> <span m="3150600">things</span> <span m="3151020">with</span>
  <span m="3151200">the</span> <span m="3151320">same</span> <span m="3151650">label</span>
  <span m="3152700">that</span> <span m="3152940">may</span> <span m="3153210">or</span>
  <span m="3153330">may</span> <span m="3153540">not</span> <span m="3153900">represent</span>
  <span m="3154500">the</span> <span m="3154620">same</span> <span m="3154920">measurement</span>
  <span m="3155670">at</span> <span m="3156210">different</span> <span m="3156570">times</span>
  <span m="3157380">in</span> <span m="3157500">the</span> <span m="3157590">system.</span></p><p><span
  m="3159300">OK,</span> <span m="3163570">this</span> <span m="3163810">is</span>
  <span m="3164020">the</span> <span m="3164350">number</span> <span m="3164770">of</span>
  <span m="3164890">chart</span> <span m="3165250">entries</span> <span m="3165730">per</span>
  <span m="3166000">admission,</span> <span m="3166570">again,</span> <span m="3166870">on</span>
  <span m="3167020">a</span> <span m="3167050">log</span> <span m="3167380">scale.</span>
  <span m="3167960">So</span> <span m="3168340">you</span> <span m="3168490">see</span>
  <span m="3168760">that</span> <span m="3169000">there</span> <span m="3169240">are</span>
  <span m="3169390">about</span> <span m="3169750">10</span> <span m="3170020">to</span>
  <span m="3170170">the</span> <span m="3170410">3.5</span> <span m="3173380">chart</span>
  <span m="3173740">entries</span> <span m="3174220">per</span> <span m="3174460">admission,</span>
  <span m="3175030">so</span> <span m="3175570">thousands</span> <span m="3177600">of</span>
  <span m="3179660">admissions,</span> <span m="3180380">of</span> <span m="3180760">chart</span>
  <span m="3181300">events</span> <span m="3181720">per</span> <span m="3181930">admission.</span>
  <span m="3183520">We</span> <span m="3183700">also</span> <span m="3184030">track</span>
  <span m="3184450">outputs.</span> <span m="3186160">So</span> <span m="3187270">Foley</span>
  <span m="3187660">catheter</span> <span m="3189340">allows</span> <span m="3190150">your</span>
  <span m="3190390">bladder</span> <span m="3190810">to</span> <span m="3190990">drain</span>
  <span m="3191650">without</span> <span m="3192070">your</span> <span m="3192250">having</span>
  <span m="3192580">consciously</span> <span m="3193300">to</span> <span m="3193420">go</span>
  <span m="3193600">to</span> <span m="3193690">the</span> <span m="3193780">bathroom,</span>
  <span m="3194930">so</span> <span m="3195040">they</span> <span m="3195220">collect</span>
  <span m="3195700">that</span> <span m="3195910">information.</span> <span m="3196720">There</span>
  <span m="3196930">are</span> <span m="3197110">1.9</span> <span m="3197950">million</span>
  <span m="3198880">recordings</span> <span m="3199750">of</span> <span m="3199960">how</span>
  <span m="3200110">much</span> <span m="3200380">fluid</span> <span m="3200800">came</span>
  <span m="3201130">out</span> <span m="3201310">of</span> <span m="3201430">your</span>
  <span m="3201580">bladder.</span></p><p><span m="3204790">Chest</span> <span m="3205180">tubes</span>
  <span m="3205720">will</span> <span m="3205990">drain</span> <span m="3206830">stuff</span>
  <span m="3207280">out</span> <span m="3207430">of</span> <span m="3207580">your</span>
  <span m="3207730">chest</span> <span m="3208210">if</span> <span m="3208360">you</span>
  <span m="3208510">have</span> <span m="3208870">congestion.</span> <span m="3210070">Urine</span>
  <span m="3210550">is</span> <span m="3210760">if</span> <span m="3210940">you</span>
  <span m="3211630">pee</span> <span m="3212050">regularly,</span> <span m="3212770">stool</span>
  <span m="3213250">out,</span> <span m="3214390">et</span> <span m="3214660">cetera.</span>
  <span m="3215620">And</span> <span m="3216700">again,</span> <span m="3217030">I'm</span>
  <span m="3217180">not</span> <span m="3217390">sure</span> <span m="3217630">I</span>
  <span m="3217780">understand</span> <span m="3218350">what</span> <span m="3218560">the</span>
  <span m="3218680">difference</span> <span m="3219090">is</span> <span m="3219370">between</span>
  <span m="3221980">urine</span> <span m="3222420">out</span> <span m="3222580">Foley</span>
  <span m="3223360">versus</span> <span m="3223960">Foley.</span> <span m="3225220">They</span>
  <span m="3225400">may</span> <span m="3225640">be</span> <span m="3225790">the</span>
  <span m="3225940">same</span> <span m="3226270">thing</span> <span m="3227050">but</span>
  <span m="3227320">one</span> <span m="3227650">from</span> <span m="3228040">CareVue</span>
  <span m="3228640">and</span> <span m="3228760">one</span> <span m="3228970">from</span>
  <span m="3229210">MetaVision,</span> <span m="3230740">so</span> <span m="3230860">again,</span>
  <span m="3231250">typical</span> <span m="3231880">kinds</span> <span m="3232270">of</span>
  <span m="3232390">problems.</span></p><p><span m="3233990">If</span> <span m="3234100">you</span>
  <span m="3234250">look</span> <span m="3234520">at</span> <span m="3234700">the</span>
  <span m="3235390">number</span> <span m="3235810">of</span> <span m="3235990">output</span>
  <span m="3236470">events</span> <span m="3237010">per</span> <span m="3238090">admission,</span>
  <span m="3239560">you're</span> <span m="3239800">seeing</span> <span m="3240250">on</span>
  <span m="3240490">the</span> <span m="3240610">order</span> <span m="3241000">of</span>
  <span m="3241350">100,</span> <span m="3243100">roughly.</span> <span m="3247960">Well,</span>
  <span m="3248200">if</span> <span m="3248320">you're</span> <span m="3248440">tracking</span>
  <span m="3248920">outputs,</span> <span m="3249520">you</span> <span m="3249640">should</span>
  <span m="3249850">also</span> <span m="3250210">track</span> <span m="3250570">inputs,</span>
  <span m="3251900">and</span> <span m="3251980">so</span> <span m="3252250">they</span>
  <span m="3252430">do.</span> <span m="3253480">And</span> <span m="3253720">so</span>
  <span m="3254920">D5W</span> <span m="3255970">is</span> <span m="3256150">this</span>
  <span m="3256390">dextrose</span> <span m="3256990">in</span> <span m="3257110">water,</span>
  <span m="3259060">0.9</span> <span m="3259630">percent</span> <span m="3260110">normal</span>
  <span m="3260470">saline.</span> <span m="3261750">Propofol</span> <span m="3262450">is</span>
  <span m="3262600">an</span> <span m="3262720">anesthetic.</span> <span m="3264010">Insulin,</span>
  <span m="3264610">heparin,</span> <span m="3266350">blood</span> <span m="3266650">thinner,</span>
  <span m="3267640">et</span> <span m="3267920">cetera.</span> <span m="3268300">Fentanyl</span>
  <span m="3268910">is,</span> <span m="3269470">I</span> <span m="3269590">think,</span>
  <span m="3270820">an</span> <span m="3270970">opioid,</span> <span m="3271690">if</span>
  <span m="3271840">I</span> <span m="3271960">remember</span> <span m="3272350">right.</span></p><p><span
  m="3273190">So</span> <span m="3273400">these</span> <span m="3273670">are</span>
  <span m="3274030">various</span> <span m="3274510">things</span> <span m="3274900">that</span>
  <span m="3275050">are</span> <span m="3275170">given</span> <span m="3275530">to</span>
  <span m="3275680">people.</span> <span m="3277090">And</span> <span m="3277540">they</span>
  <span m="3278680">affect</span> <span m="3279070">the</span> <span m="3279190">volume</span>
  <span m="3280030">of</span> <span m="3280210">the</span> <span m="3280330">person.</span>
  <span m="3281020">So</span> <span m="3281260">this</span> <span m="3281500">is</span>
  <span m="3282040">an</span> <span m="3282160">attempt</span> <span m="3282490">to</span>
  <span m="3282640">keep</span> <span m="3282940">the</span> <span m="3283060">person</span>
  <span m="3283480">in</span> <span m="3283630">balance</span> <span m="3284170">and</span>
  <span m="3284290">keep</span> <span m="3284530">track</span> <span m="3284860">of</span>
  <span m="3285010">that.</span> <span m="3286600">MetaVision</span> <span m="3287260">inputs</span>
  <span m="3288340">are</span> <span m="3288550">classified</span> <span m="3289360">somewhat</span>
  <span m="3289840">differently</span> <span m="3290920">but</span> <span m="3291190">they</span>
  <span m="3291340">have</span> <span m="3291550">similar</span> <span m="3292330">kinds</span>
  <span m="3292690">of</span> <span m="3292840">data.</span> <span m="3293770">And</span>
  <span m="3293950">if</span> <span m="3294100">you</span> <span m="3294220">combine</span>
  <span m="3294790">them,</span> <span m="3295030">you</span> <span m="3295210">get,</span>
  <span m="3295670">again,</span> <span m="3296190">a</span> <span m="3296200">distribution</span>
  <span m="3297310">on</span> <span m="3297490">a</span> <span m="3297550">log</span>
  <span m="3297880">scale</span> <span m="3299350">that</span> <span m="3299560">shows</span>
  <span m="3300040">that</span> <span m="3300250">there</span> <span m="3300490">are</span>
  <span m="3300730">on</span> <span m="3300940">the</span> <span m="3301060">order</span>
  <span m="3301420">of</span> <span m="3301780">10</span> <span m="3302050">to</span>
  <span m="3302230">the</span> <span m="3302350">fifth</span> <span m="3302950">input</span>
  <span m="3303370">events,</span> <span m="3305140">so</span> <span m="3305320">quite</span>
  <span m="3305590">a</span> <span m="3305650">few</span> <span m="3307000">input</span>
  <span m="3307360">events,</span> <span m="3308230">because</span> <span m="3308680">this</span>
  <span m="3308920">is</span> <span m="3309130">recorded</span> <span m="3309670">periodically.</span></p><p><span
  m="3311780">Now,</span> <span m="3312310">the</span> <span m="3312460">paper</span>
  <span m="3312880">that</span> <span m="3313090">I--</span> <span m="3313740">yeah.</span></p><p><span
  m="3313940">AUDIENCE:</span> <span m="3314179">What's the input</span> <span m="3314896">again?</span>
  <span m="3315374">Is that when</span> <span m="3315852">you come to the</span> <span
  m="3316330">hospital and get</span> <span m="3316808">admitted</span> <span m="3317286">or--</span></p><p><span
  m="3317770">PROFESSOR:</span> <span m="3317855">No,</span> <span m="3318190">no,</span>
  <span m="3318560">no.</span> <span m="3318950">It's</span> <span m="3319660">an</span>
  <span m="3319810">input</span> <span m="3320170">into</span> <span m="3320470">you.</span>
  <span m="3321460">So</span> <span m="3321700">it's</span> <span m="3321850">like</span>
  <span m="3322120">you</span> <span m="3322240">drink</span> <span m="3322510">a</span>
  <span m="3322570">glass</span> <span m="3322960">of</span> <span m="3323020">water,</span>
  <span m="3323570">the</span> <span m="3323860">nurse</span> <span m="3324250">is</span>
  <span m="3324310">supposed</span> <span m="3324760">to</span> <span m="3324880">record</span>
  <span m="3325330">it.</span> <span m="3326020">Although,</span> <span m="3326230">she</span>
  <span m="3326380">doesn't</span> <span m="3326770">always</span> <span m="3327220">because</span>
  <span m="3327400">she</span> <span m="3327580">may</span> <span m="3327760">not</span>
  <span m="3327970">notice</span> <span m="3328390">it.</span> <span m="3329570">But</span>
  <span m="3329740">if</span> <span m="3329920">they</span> <span m="3330100">hang</span>
  <span m="3330400">an</span> <span m="3330520">IV</span> <span m="3330880">bag</span>
  <span m="3331300">and</span> <span m="3331480">pour</span> <span m="3331840">a</span>
  <span m="3331990">liter</span> <span m="3332380">of</span> <span m="3332500">liquid</span>
  <span m="3332890">into</span> <span m="3333160">you,</span> <span m="3333820">they</span>
  <span m="3334030">do</span> <span m="3334210">record</span> <span m="3334690">that,</span>
  <span m="3336270">OK?</span></p><p><span m="3338050">All</span> <span m="3338110">right,</span>
  <span m="3339100">so</span> <span m="3339580">I</span> <span m="3339700">had</span>
  <span m="3339910">you</span> <span m="3340030">read</span> <span m="3340300">this</span>
  <span m="3340510">interesting</span> <span m="3341020">paper</span> <span m="3342850">and</span>
  <span m="3346680">a</span> <span m="3346780">discussion</span> <span m="3347440">prior</span>
  <span m="3347890">to</span> <span m="3348070">that</span> <span m="3348280">paper,</span>
  <span m="3348790">because</span> <span m="3349630">one</span> <span m="3349870">of</span>
  <span m="3349930">the</span> <span m="3350140">authors</span> <span m="3351070">is</span>
  <span m="3351460">a</span> <span m="3351520">former</span> <span m="3351910">student</span>
  <span m="3352300">of</span> <span m="3352420">mine.</span> <span m="3352810">And</span>
  <span m="3352960">I</span> <span m="3353080">know</span> <span m="3353860">one</span>
  <span m="3354100">of</span> <span m="3354190">the</span> <span m="3354310">other</span>
  <span m="3354550">guys</span> <span m="3354880">pretty</span> <span m="3355150">well.</span>
  <span m="3356200">And</span> <span m="3357400">the</span> <span m="3357760">former</span>
  <span m="3358180">student,</span> <span m="3358600">Zak</span> <span m="3358880">Kohane,</span>
  <span m="3360100">came</span> <span m="3360400">back</span> <span m="3361150">some</span>
  <span m="3361450">years</span> <span m="3361750">ago</span> <span m="3362080">from</span>
  <span m="3362410">a</span> <span m="3362470">conference</span> <span m="3363040">in</span>
  <span m="3363160">California</span> <span m="3365050">and</span> <span m="3365230">was</span>
  <span m="3365470">explaining</span> <span m="3366010">to</span> <span m="3366160">me</span>
  <span m="3366370">that</span> <span m="3366550">he</span> <span m="3366700">ran</span>
  <span m="3367000">into</span> <span m="3367270">a</span> <span m="3367360">venture</span>
  <span m="3367690">capitalist</span> <span m="3369040">who</span> <span m="3369340">discovered</span>
  <span m="3370090">that</span> <span m="3370300">there</span> <span m="3370430">is</span>
  <span m="3370780">an</span> <span m="3370930">interesting</span> <span m="3371470">physiological</span>
  <span m="3372370">variation</span> <span m="3373750">in</span> <span m="3374170">the</span>
  <span m="3375730">abnormality</span> <span m="3376840">of</span> <span m="3377170">lab</span>
  <span m="3377470">tests</span> <span m="3378100">that</span> <span m="3378280">are</span>
  <span m="3378400">done</span> <span m="3378640">at</span> <span m="3378790">night.</span>
  <span m="3380110">And</span> <span m="3380320">he</span> <span m="3380470">suspected</span>
  <span m="3381220">that</span> <span m="3381430">there</span> <span m="3381590">was</span>
  <span m="3381730">a</span> <span m="3381790">diurnal</span> <span m="3382360">variation</span>
  <span m="3383690">that</span> <span m="3383950">lab</span> <span m="3384220">tests</span>
  <span m="3384630">actually</span> <span m="3385090">become</span> <span m="3385570">more</span>
  <span m="3385840">abnormal</span> <span m="3386710">at</span> <span m="3386890">night</span>
  <span m="3387250">than</span> <span m="3387460">they</span> <span m="3387640">do</span>
  <span m="3387910">during</span> <span m="3388240">the</span> <span m="3388360">day.</span></p><p><span
  m="3389800">And</span> <span m="3390010">Zak,</span> <span m="3390460">who</span>
  <span m="3390850">is</span> <span m="3391150">not</span> <span m="3391390">only</span>
  <span m="3391660">a</span> <span m="3391810">computer</span> <span m="3392260">science</span>
  <span m="3392680">PhD</span> <span m="3393250">but</span> <span m="3393400">also</span>
  <span m="3393760">a</span> <span m="3393820">practicing</span> <span m="3394450">doctor,</span>
  <span m="3395350">turns</span> <span m="3395710">to him</span> <span m="3395890">and
  says,</span> <span m="3396670">you're</span> <span m="3396880">an</span> <span m="3397000">idiot,</span>
  <span m="3398400">right?</span> <span m="3399430">Who</span> <span m="3399730">has</span>
  <span m="3400120">their</span> <span m="3401620">blood</span> <span m="3401950">drawn</span>
  <span m="3402520">at</span> <span m="3402700">3</span> <span m="3402970">o'clock</span>
  <span m="3403390">in</span> <span m="3403510">the</span> <span m="3403600">morning.</span>
  <span m="3405670">It's</span> <span m="3405880">typically</span> <span m="3406480">not</span>
  <span m="3406810">healthy</span> <span m="3407200">people,</span> <span m="3409120">right?</span>
  <span m="3410650">So</span> <span m="3411160">this</span> <span m="3411460">is</span>
  <span m="3411640">another</span> <span m="3412180">of</span> <span m="3412330">these</span>
  <span m="3412630">nice</span> <span m="3412990">confounding</span> <span m="3413710">stories</span>
  <span m="3414910">where,</span> <span m="3416620">if</span> <span m="3416920">you</span>
  <span m="3417760">have</span> <span m="3418030">a</span> <span m="3418090">test</span>
  <span m="3418510">done</span> <span m="3418960">in</span> <span m="3419140">the</span>
  <span m="3419230">middle</span> <span m="3419500">of</span> <span m="3419620">the</span>
  <span m="3419710">night,</span> <span m="3420040">it</span> <span m="3420160">probably</span>
  <span m="3420670">indicates</span> <span m="3421240">that</span> <span m="3421450">you're</span>
  <span m="3421570">sicker.</span></p><p><span m="3423290">So</span> <span m="3423970">he</span>
  <span m="3424180">and</span> <span m="3424330">Griffin</span> <span m="3424780">recruited</span>
  <span m="3425410">their</span> <span m="3425620">third</span> <span m="3425950">author</span>
  <span m="3426340">and</span> <span m="3426490">went</span> <span m="3426700">off</span>
  <span m="3427420">and</span> <span m="3427600">did</span> <span m="3427840">a</span>
  <span m="3427960">very</span> <span m="3428320">large</span> <span m="3428620">scale</span>
  <span m="3429010">study</span> <span m="3429460">of</span> <span m="3429610">this</span>
  <span m="3429790">question,</span> <span m="3430300">which</span> <span m="3430540">is</span>
  <span m="3430690">what</span> <span m="3430930">the</span> <span m="3431050">paper</span>
  <span m="3431440">that</span> <span m="3431740">I</span> <span m="3431890">asked</span>
  <span m="3432130">you</span> <span m="3432220">to</span> <span m="3432310">read</span>
  <span m="3433270">reports</span> <span m="3433840">on.</span> <span m="3434860">And</span>
  <span m="3435310">so</span> <span m="3436210">I</span> <span m="3436720">said,</span>
  <span m="3436990">well,</span> <span m="3437380">I</span> <span m="3437470">wonder</span>
  <span m="3437800">if</span> <span m="3437950">I</span> <span m="3438070">could</span>
  <span m="3438280">reproduce</span> <span m="3438940">that</span> <span m="3439210">study</span>
  <span m="3439930">in</span> <span m="3440110">the</span> <span m="3440230">MIMIC</span>
  <span m="3440590">database.</span> <span m="3442210">And</span> <span m="3442570">the</span>
  <span m="3442810">answer,</span> <span m="3443200">just</span> <span m="3443530">in</span>
  <span m="3443620">case</span> <span m="3443950">you</span> <span m="3444070">get</span>
  <span m="3444280">your</span> <span m="3444400">hopes</span> <span m="3444760">up,</span>
  <span m="3444970">was</span> <span m="3445210">no,</span> <span m="3448360">in</span>
  <span m="3448510">large</span> <span m="3448840">part</span> <span m="3449170">because</span>
  <span m="3449530">we</span> <span m="3449680">just</span> <span m="3449860">don't</span>
  <span m="3450070">have</span> <span m="3450280">the</span> <span m="3450370">right</span>
  <span m="3450580">kind</span> <span m="3450850">of</span> <span m="3450940">data.</span>
  <span m="3451390">So</span> <span m="3451510">there</span> <span m="3451690">are</span>
  <span m="3452110">not</span> <span m="3452380">that</span> <span m="3452590">many</span>
  <span m="3453370">white</span> <span m="3453610">blood</span> <span m="3453910">counts</span>
  <span m="3454420">that</span> <span m="3454700">were</span> <span m="3454900">measured</span>
  <span m="3455440">in</span> <span m="3455620">the</span> <span m="3455710">MIMIC</span>
  <span m="3456040">database,</span> <span m="3456610">for</span> <span m="3456820">example.</span></p><p><span
  m="3458510">But</span> <span m="3459280">if</span> <span m="3459490">you</span>
  <span m="3459670">look</span> <span m="3460090">at</span> <span m="3461350">the--</span>
  <span m="3461860">this</span> <span m="3462130">is</span> <span m="3462280">MIMIC</span>
  <span m="3462640">data.</span> <span m="3463660">And</span> <span m="3463840">if</span>
  <span m="3463990">you</span> <span m="3464110">say,</span> <span m="3465020">what's</span>
  <span m="3465250">the</span> <span m="3465370">fraction</span> <span m="3466270">of</span>
  <span m="3466510">abnormal</span> <span m="3467230">white</span> <span m="3467500">blood</span>
  <span m="3467800">count</span> <span m="3468130">values</span> <span m="3468700">by</span>
  <span m="3469000">hour--</span> <span m="3469480">so</span> <span m="3469690">this</span>
  <span m="3469930">is</span> <span m="3470080">midnight</span> <span m="3471160">to</span>
  <span m="3471310">midnight.</span> <span m="3473290">And</span> <span m="3473890">each</span>
  <span m="3474160">hour,</span> <span m="3475360">there's</span> <span m="3475600">some</span>
  <span m="3475960">fraction</span> <span m="3476710">of</span> <span m="3476920">these</span>
  <span m="3477190">test</span> <span m="3477520">results</span> <span m="3478000">that</span>
  <span m="3478150">are</span> <span m="3478270">abnormal.</span> <span m="3479380">And</span>
  <span m="3479560">sure</span> <span m="3479860">enough,</span> <span m="3480220">what</span>
  <span m="3480430">you</span> <span m="3480550">see</span> <span m="3480850">is</span>
  <span m="3481060">that,</span> <span m="3481240">at</span> <span m="3481360">5</span>
  <span m="3481630">o'clock</span> <span m="3482050">in</span> <span m="3482140">the</span>
  <span m="3482230">morning,</span> <span m="3483055">a</span> <span m="3483400">much</span>
  <span m="3483700">higher</span> <span m="3484030">fraction</span> <span m="3484570">of</span>
  <span m="3484720">them</span> <span m="3484930">is</span> <span m="3485110">abnormal</span>
  <span m="3486260">than</span> <span m="3486630">at</span> <span m="3487000">3</span>
  <span m="3487280">o'clock</span> <span m="3487720">in</span> <span m="3487810">the</span>
  <span m="3487930">afternoon,</span> <span m="3488926">OK,</span> <span m="3489800">which</span>
  <span m="3491020">is</span> <span m="3491200">consistent</span> <span m="3491980">with</span>
  <span m="3492520">Zak's</span> <span m="3493840">peremptory</span> <span m="3495640">comment</span>
  <span m="3496210">about</span> <span m="3496510">the</span> <span m="3496630">guy</span>
  <span m="3496870">being</span> <span m="3497170">an</span> <span m="3497290">idiot.</span></p><p><span
  m="3500590">So</span> <span m="3500860">once</span> <span m="3501190">again,</span>
  <span m="3501760">I</span> <span m="3501910">said,</span> <span m="3502310">well,</span>
  <span m="3502670">can</span> <span m="3502810">we</span> <span m="3502960">build</span>
  <span m="3503290">a</span> <span m="3503350">really</span> <span m="3503620">simple</span>
  <span m="3504040">model</span> <span m="3505030">that</span> <span m="3505300">predicts</span>
  <span m="3506500">who's</span> <span m="3506800">going</span> <span m="3506980">to</span>
  <span m="3507070">die</span> <span m="3507430">in</span> <span m="3507550">the</span>
  <span m="3507640">hospital</span> <span m="3508370">in</span> <span m="3508390">this</span>
  <span m="3508600">case?</span> <span m="3509570">That's</span> <span m="3509770">the</span>
  <span m="3509890">easiest</span> <span m="3510400">one</span> <span m="3510610">to</span>
  <span m="3510760">predict</span> <span m="3511210">because</span> <span m="3511570">I</span>
  <span m="3511720">have</span> <span m="3511960">that</span> <span m="3512170">data.</span>
  <span m="3513590">We</span> <span m="3514060">could</span> <span m="3514390">get</span>
  <span m="3514930">three-year</span> <span m="3515410">survival</span> <span m="3516040">data,</span>
  <span m="3516590">which</span> <span m="3516760">is</span> <span m="3516880">what</span>
  <span m="3517090">they</span> <span m="3517240">were</span> <span m="3517390">looking</span>
  <span m="3517780">at.</span> <span m="3518810">But</span> <span m="3518920">it's</span>
  <span m="3519070">harder</span> <span m="3519550">and</span> <span m="3519700">it</span>
  <span m="3519820">runs</span> <span m="3520120">into</span> <span m="3520360">censoring</span>
  <span m="3520960">problems</span> <span m="3521590">of</span> <span m="3522160">what</span>
  <span m="3522370">happens</span> <span m="3522940">if</span> <span m="3523090">the</span>
  <span m="3523180">person</span> <span m="3523630">was</span> <span m="3523840">hospitalized</span>
  <span m="3524620">less</span> <span m="3524920">than</span> <span m="3525100">three</span>
  <span m="3525370">years</span> <span m="3525760">before</span> <span m="3526690">the</span>
  <span m="3526870">end</span> <span m="3527050">of</span> <span m="3527170">our</span>
  <span m="3527290">data</span> <span m="3527560">collection</span> <span m="3528100">period</span>
  <span m="3528710">and</span> <span m="3528760">so</span> <span m="3529000">on.</span>
  <span m="3529660">And</span> <span m="3529780">so</span> <span m="3529990">I</span>
  <span m="3530110">avoided</span> <span m="3530560">that.</span></p><p><span m="3531520">But</span>
  <span m="3531760">what</span> <span m="3531940">this</span> <span m="3532210">is</span>
  <span m="3532300">showing</span> <span m="3532750">you</span> <span m="3534100">is,</span>
  <span m="3534460">for</span> <span m="3534970">each</span> <span m="3535270">of</span>
  <span m="3535480">the</span> <span m="3536230">hours,</span> <span m="3536590">zero</span>
  <span m="3537130">to</span> <span m="3537380">24,</span> <span m="3539800">what</span>
  <span m="3540070">is</span> <span m="3540310">the</span> <span m="3542710">number</span>
  <span m="3543550">of</span> <span m="3545530">measurements?</span> <span m="3547850">And</span>
  <span m="3548180">for</span> <span m="3548900">each</span> <span m="3549170">of</span>
  <span m="3549320">those</span> <span m="3549680">hours,</span> <span m="3551280">what</span>
  <span m="3551390">is</span> <span m="3551510">the</span> <span m="3551630">fraction</span>
  <span m="3552230">of</span> <span m="3552350">those</span> <span m="3552620">measurements</span>
  <span m="3553310">that's</span> <span m="3553580">abnormal,</span> <span m="3555870">OK?</span>
  <span m="3556820">So</span> <span m="3557000">I</span> <span m="3557090">said,</span>
  <span m="3557460">well,</span> <span m="3558030">let's</span> <span m="3558230">just</span>
  <span m="3558440">throw</span> <span m="3558680">it</span> <span m="3558800">into</span>
  <span m="3559070">a</span> <span m="3559130">logistic</span> <span m="3559640">regression</span>
  <span m="3560120">model.</span> <span m="3561020">And</span> <span m="3561140">what</span>
  <span m="3561350">comes</span> <span m="3561680">out</span> <span m="3561920">is</span>
  <span m="3562010">something</span> <span m="3562430">really</span> <span m="3562730">weird,</span>
  <span m="3563420">which</span> <span m="3563750">is</span> <span m="3563930">that</span>
  <span m="3564770">a</span> <span m="3564860">few</span> <span m="3565280">particular</span>
  <span m="3566030">hours</span> <span m="3566570">are</span> <span m="3566690">significant,</span>
  <span m="3567620">but</span> <span m="3567860">most</span> <span m="3568190">of</span>
  <span m="3568340">them</span> <span m="3568550">are</span> <span m="3568670">not.</span></p><p><span
  m="3569990">And</span> <span m="3570110">that</span> <span m="3570320">looks</span>
  <span m="3570590">like</span> <span m="3570830">noise</span> <span m="3571250">to</span>
  <span m="3571370">me,</span> <span m="3572950">right?</span> <span m="3573770">Because</span>
  <span m="3575000">you</span> <span m="3575120">wouldn't</span> <span m="3575450">expect</span>
  <span m="3577460">that,</span> <span m="3578570">at</span> <span m="3579550">8</span>
  <span m="3579720">o'clock</span> <span m="3580160">in</span> <span m="3580250">the</span>
  <span m="3580340">morning,</span> <span m="3582520">the</span> <span m="3582740">fact</span>
  <span m="3583130">that</span> <span m="3583370">you</span> <span m="3583520">had</span>
  <span m="3583910">something</span> <span m="3584420">measured</span> <span m="3585410">matters.</span>
  <span m="3586580">But</span> <span m="3586850">at</span> <span m="3586970">9</span>
  <span m="3587230">o'clock</span> <span m="3587660">in</span> <span m="3587750">the</span>
  <span m="3587840">morning,</span> <span m="3588260">it</span> <span m="3588350">doesn't.</span>
  <span m="3589970">That</span> <span m="3590120">doesn't</span> <span m="3590450">seem</span>
  <span m="3590750">sensible.</span> <span m="3592490">So</span> <span m="3592700">I</span>
  <span m="3592820">don't</span> <span m="3593000">think</span> <span m="3593210">there's</span>
  <span m="3593510">enough</span> <span m="3593780">signal</span> <span m="3594170">here.</span></p><p><span
  m="3595910">And</span> <span m="3596090">in</span> <span m="3596180">fact,</span>
  <span m="3597080">when</span> <span m="3597290">I</span> <span m="3597440">looked</span>
  <span m="3597860">at</span> <span m="3600050">the</span> <span m="3600230">number</span>
  <span m="3600620">of</span> <span m="3600770">white</span> <span m="3600980">blood</span>
  <span m="3601220">count</span> <span m="3601520">measurements</span> <span m="3602180">at</span>
  <span m="3602300">night</span> <span m="3603170">and</span> <span m="3603380">related</span>
  <span m="3603830">to</span> <span m="3604010">mortality--</span> <span m="3604790">so</span>
  <span m="3605090">false</span> <span m="3606140">means</span> <span m="3606470">people</span>
  <span m="3606860">lived</span> <span m="3607330">and</span> <span m="3607460">true</span>
  <span m="3607700">means</span> <span m="3608060">they</span> <span m="3608240">died.</span>
  <span m="3609200">But</span> <span m="3609500">you</span> <span m="3609620">see</span>
  <span m="3609890">that</span> <span m="3610070">there's</span> <span m="3610340">not</span>
  <span m="3610610">a</span> <span m="3610670">whole</span> <span m="3610880">lot</span>
  <span m="3611150">of</span> <span m="3611240">difference</span> <span m="3611810">between</span>
  <span m="3612230">the</span> <span m="3612350">distributions.</span> <span m="3613730">But</span>
  <span m="3613970">you</span> <span m="3614090">also</span> <span m="3614420">see</span>
  <span m="3614660">that</span> <span m="3614870">the</span> <span m="3614960">number</span>
  <span m="3615290">of</span> <span m="3615410">white</span> <span m="3615650">blood</span>
  <span m="3615890">counts</span> <span m="3616310">is</span> <span m="3616460">relatively</span>
  <span m="3617060">small</span> <span m="3617990">in</span> <span m="3618110">this</span>
  <span m="3618320">database.</span> <span m="3618920">And</span> <span m="3619040">so</span>
  <span m="3619400">I</span> <span m="3619550">think</span> <span m="3619760">we</span>
  <span m="3619910">just</span> <span m="3620150">don't</span> <span m="3620360">have</span>
  <span m="3620570">enough</span> <span m="3620840">data</span> <span m="3623000">to</span>
  <span m="3623180">do</span> <span m="3623390">it.</span></p><p><span m="3624360">On</span>
  <span m="3624380">the</span> <span m="3624500">other</span> <span m="3624680">hand,</span>
  <span m="3625050">if</span> <span m="3625100">you</span> <span m="3625250">look</span>
  <span m="3625520">at</span> <span m="3625640">a</span> <span m="3625730">panel</span>
  <span m="3626270">of</span> <span m="3626510">different</span> <span m="3626930">drugs,</span>
  <span m="3628070">you</span> <span m="3628220">look</span> <span m="3628460">at</span>
  <span m="3628580">mean</span> <span m="3628880">values</span> <span m="3629570">of</span>
  <span m="3629810">blood</span> <span m="3630050">urea</span> <span m="3630380">nitrogen</span>
  <span m="3631040">or</span> <span m="3631160">calcium</span> <span m="3631730">chloride,</span>
  <span m="3632390">CO2,</span> <span m="3633090">et</span> <span m="3633390">cetera,</span>
  <span m="3634130">you</span> <span m="3634280">see</span> <span m="3634490">that</span>
  <span m="3634700">there</span> <span m="3634910">is</span> <span m="3635120">variation</span>
  <span m="3636590">across</span> <span m="3637070">time.</span> <span m="3638280">So</span>
  <span m="3639050">there</span> <span m="3639320">is</span> <span m="3639500">some</span>
  <span m="3640250">sort</span> <span m="3640520">of</span> <span m="3641090">variance</span>
  <span m="3641900">that's</span> <span m="3642320">either</span> <span m="3642710">caused</span>
  <span m="3643220">by</span> <span m="3644060">the</span> <span m="3644210">diurnal</span>
  <span m="3644780">physiology</span> <span m="3645830">of</span> <span m="3646070">the</span>
  <span m="3646190">human</span> <span m="3646520">body</span> <span m="3647060">or</span>
  <span m="3647300">by</span> <span m="3647630">the</span> <span m="3648110">routine</span>
  <span m="3648530">practice</span> <span m="3649610">of</span> <span m="3649760">medicine,</span>
  <span m="3650300">about</span> <span m="3650630">when</span> <span m="3650870">people</span>
  <span m="3651260">choose</span> <span m="3651590">to</span> <span m="3651740">take</span>
  <span m="3652010">lab</span> <span m="3652250">measurements.</span> <span m="3655190">And</span>
  <span m="3655490">in</span> <span m="3655640">fact,</span> <span m="3656280">if</span>
  <span m="3656390">you</span> <span m="3657230">look</span> <span m="3657650">at</span>
  <span m="3658100">the</span> <span m="3658820">fraction</span> <span m="3659810">of</span>
  <span m="3660560">high</span> <span m="3660890">end</span> <span m="3661070">low</span>
  <span m="3661340">lab</span> <span m="3661670">values,</span> <span m="3662630">they</span>
  <span m="3662840">do</span> <span m="3663080">vary</span> <span m="3663440">by</span>
  <span m="3663680">hour.</span> <span m="3664580">And</span> <span m="3664820">in</span>
  <span m="3664910">particular,</span> <span m="3665850">if</span> <span m="3665930">you</span>
  <span m="3666080">look</span> <span m="3666320">at</span> <span m="3666470">white</span>
  <span m="3666740">blood</span> <span m="3667010">counts,</span> <span m="3667970">you</span>
  <span m="3668130">see</span> <span m="3668480">that</span> <span m="3668810">the</span>
  <span m="3669830">fraction</span> <span m="3670700">of</span> <span m="3670970">high</span>
  <span m="3671300">values</span> <span m="3673400">goes</span> <span m="3673820">up</span>
  <span m="3674150">at</span> <span m="3674330">night</span> <span m="3675200">and</span>
  <span m="3675470">the</span> <span m="3675590">fraction</span> <span m="3676160">of</span>
  <span m="3676310">low</span> <span m="3676520">values</span> <span m="3677060">goes</span>
  <span m="3677360">down</span> <span m="3677660">at</span> <span m="3677780">night,</span>
  <span m="3678860">right,</span> <span m="3679250">which</span> <span m="3679460">is</span>
  <span m="3679580">consistent</span> <span m="3680270">with</span> <span m="3680450">what</span>
  <span m="3680660">they</span> <span m="3680810">saw</span> <span m="3681650">as</span>
  <span m="3681830">well.</span></p><p><span m="3683410">There</span> <span m="3683770">is</span>
  <span m="3683960">another</span> <span m="3684320">way</span> <span m="3684500">to</span>
  <span m="3684590">measure</span> <span m="3685040">it,</span> <span m="3685250">which</span>
  <span m="3685550">is,</span> <span m="3687650">instead</span> <span m="3688160">of</span>
  <span m="3688280">using</span> <span m="3688760">normal</span> <span m="3689180">ranges,</span>
  <span m="3690230">the</span> <span m="3690380">lab</span> <span m="3690770">actually</span>
  <span m="3691310">gives</span> <span m="3691640">you</span> <span m="3691790">a</span>
  <span m="3691880">call</span> <span m="3692660">that</span> <span m="3692900">says,</span>
  <span m="3693680">is</span> <span m="3693860">this</span> <span m="3694100">value</span>
  <span m="3694640">normal,</span> <span m="3695110">low,</span> <span m="3695390">or</span>
  <span m="3695510">high?</span> <span m="3696530">And</span> <span m="3696770">we</span>
  <span m="3696920">can</span> <span m="3697130">use</span> <span m="3697430">that.</span>
  <span m="3698630">That's</span> <span m="3699020">a</span> <span m="3699050">little</span>
  <span m="3699320">bit</span> <span m="3699530">more</span> <span m="3699770">subtle</span>
  <span m="3700250">because</span> <span m="3701150">it</span> <span m="3701240">depends</span>
  <span m="3701750">on</span> <span m="3702230">calibration</span> <span m="3702980">of</span>
  <span m="3703100">the</span> <span m="3703250">equipment</span> <span m="3704300">and</span>
  <span m="3704480">is</span> <span m="3704660">updated</span> <span m="3705200">as</span>
  <span m="3705410">the</span> <span m="3705530">calibration</span> <span m="3706280">changes.</span>
  <span m="3707220">So</span> <span m="3707330">that's</span> <span m="3707630">probably</span>
  <span m="3708050">a</span> <span m="3708110">little</span> <span m="3708320">bit</span>
  <span m="3708500">more</span> <span m="3708710">accurate.</span> <span m="3709610">But</span>
  <span m="3709850">you</span> <span m="3709970">see</span> <span m="3710180">essentially</span>
  <span m="3710780">the</span> <span m="3710900">same</span> <span m="3711170">phenomenon</span>
  <span m="3711800">here.</span></p><p><span m="3713330">But</span> <span m="3713780">if</span>
  <span m="3713990">you</span> <span m="3714140">look</span> <span m="3714530">at</span>
  <span m="3716720">the</span> <span m="3716900">distributions</span> <span m="3718010">of</span>
  <span m="3718850">when</span> <span m="3719780">measurements</span> <span m="3720500">are</span>
  <span m="3720620">done</span> <span m="3720980">that</span> <span m="3721130">turn</span>
  <span m="3721460">out</span> <span m="3721640">to</span> <span m="3721760">be</span>
  <span m="3721910">normal</span> <span m="3722450">versus</span> <span m="3722990">when</span>
  <span m="3723200">they</span> <span m="3723380">turn</span> <span m="3723650">out</span>
  <span m="3723800">to</span> <span m="3723920">be</span> <span m="3724100">abnormal,</span>
  <span m="3725310">there</span> <span m="3725680">is</span> <span m="3725900">a</span>
  <span m="3725960">lot</span> <span m="3726230">of</span> <span m="3726320">similarity</span>
  <span m="3727070">between</span> <span m="3727520">the</span> <span m="3727640">normal</span>
  <span m="3728090">and</span> <span m="3728210">the</span> <span m="3728360">abnormal</span>
  <span m="3729410">curves</span> <span m="3730070">of</span> <span m="3730250">when</span>
  <span m="3730460">those</span> <span m="3730730">measurements</span> <span m="3731330">are</span>
  <span m="3731420">taken.</span> <span m="3732590">So</span> <span m="3733640">we're</span>
  <span m="3733790">not</span> <span m="3734030">seeing</span> <span m="3734390">that.</span></p><p><span
  m="3735770">OK,</span> <span m="3736610">let</span> <span m="3736760">me</span>
  <span m="3736880">race</span> <span m="3737180">through</span> <span m="3737420">to</span>
  <span m="3737570">the</span> <span m="3737750">end.</span> <span m="3738950">This</span>
  <span m="3739280">is</span> <span m="3739460">my</span> <span m="3739700">heartbeat</span>
  <span m="3740330">from</span> <span m="3740630">my</span> <span m="3740810">watch.</span>
  <span m="3743240">You</span> <span m="3743420">can</span> <span m="3743600">actually</span>
  <span m="3744140">download</span> <span m="3744830">the</span> <span m="3744980">stuff</span>
  <span m="3745520">and</span> <span m="3746180">put</span> <span m="3746390">it</span>
  <span m="3746510">in</span> <span m="3746630">your</span> <span m="3746810">favorite</span>
  <span m="3747530">analysis</span> <span m="3748190">engine</span> <span m="3748760">and</span>
  <span m="3749780">take</span> <span m="3750080">a</span> <span m="3750110">look.</span>
  <span m="3750540">So</span> <span m="3750650">here</span> <span m="3750920">I</span>
  <span m="3751070">was</span> <span m="3751280">running</span> <span m="3751640">across</span>
  <span m="3752090">the</span> <span m="3752180">Harvard</span> <span m="3752600">bridge.</span>
  <span m="3753650">And</span> <span m="3753950">if</span> <span m="3754160">you</span>
  <span m="3754280">look</span> <span m="3754520">at</span> <span m="3754670">my</span>
  <span m="3754880">heart</span> <span m="3755150">rate</span> <span m="3755390">variability</span>
  <span m="3756230">over</span> <span m="3756530">the</span> <span m="3756710">30</span>
  <span m="3757070">seconds</span> <span m="3757670">or</span> <span m="3757790">so,</span>
  <span m="3758690">you</span> <span m="3758840">see</span> <span m="3759140">that</span>
  <span m="3759350">the</span> <span m="3759590">interbeat</span> <span m="3760400">interval</span>
  <span m="3761390">ranges</span> <span m="3761960">from</span> <span m="3762260">about</span>
  <span m="3762560">550</span> <span m="3763580">to</span> <span m="3763760">about</span>
  <span m="3766930">600</span> <span m="3767240">and</span> <span m="3767990">whatever</span>
  <span m="3768770">20</span> <span m="3769160">milliseconds.</span></p><p><span m="3770900">And</span>
  <span m="3771110">so</span> <span m="3771320">you</span> <span m="3771470">could</span>
  <span m="3771680">calculate</span> <span m="3772340">my</span> <span m="3772520">heart</span>
  <span m="3772820">rate</span> <span m="3773030">variability,</span> <span m="3773970">which</span>
  <span m="3774110">is</span> <span m="3774290">thought</span> <span m="3774560">to</span>
  <span m="3774710">be</span> <span m="3775520">an</span> <span m="3775640">indicator</span>
  <span m="3776330">of</span> <span m="3776780">heart</span> <span m="3777050">health</span>
  <span m="3777500">and</span> <span m="3777620">so</span> <span m="3777860">on.</span>
  <span m="3778610">You</span> <span m="3778760">can</span> <span m="3778970">calculate</span>
  <span m="3779690">that</span> <span m="3779870">I</span> <span m="3779990">was</span>
  <span m="3780230">running</span> <span m="3780650">at</span> <span m="3780740">a</span>
  <span m="3780830">pace</span> <span m="3781220">of</span> <span m="3781370">about</span>
  <span m="3781610">100--</span> <span m="3782930">my</span> <span m="3783170">heart</span>
  <span m="3783470">was</span> <span m="3783680">beating</span> <span m="3784100">at</span>
  <span m="3784220">a</span> <span m="3784250">pace</span> <span m="3784580">of</span>
  <span m="3784730">about</span> <span m="3784970">100</span> <span m="3785360">beats</span>
  <span m="3785660">per</span> <span m="3785840">minute.</span> <span m="3787320">So</span>
  <span m="3787820">you</span> <span m="3787940">know</span> <span m="3788090">there's</span>
  <span m="3788360">all</span> <span m="3788510">sorts</span> <span m="3788870">of</span>
  <span m="3788990">information</span> <span m="3789620">like</span> <span m="3789860">that</span>
  <span m="3790040">available.</span></p><p><span m="3791570">Now,</span> <span m="3793280">as</span>
  <span m="3793460">I</span> <span m="3793580">said,</span> <span m="3793820">I'm</span>
  <span m="3793970">not</span> <span m="3794120">going</span> <span m="3794240">to</span>
  <span m="3794360">get</span> <span m="3794540">into</span> <span m="3794810">this</span>
  <span m="3795080">today,</span> <span m="3795530">but</span> <span m="3797690">this</span>
  <span m="3797960">was</span> <span m="3798170">a</span> <span m="3798230">very</span>
  <span m="3798500">successful</span> <span m="3799250">recently</span> <span m="3799850">published</span>
  <span m="3800330">paper</span> <span m="3801350">where</span> <span m="3801590">they're</span>
  <span m="3801830">able</span> <span m="3802190">to</span> <span m="3802370">take</span>
  <span m="3802670">a</span> <span m="3802730">look</span> <span m="3803150">at</span>
  <span m="3804800">images</span> <span m="3805520">of</span> <span m="3805760">the
  lung.</span> <span m="3806460">So</span> <span m="3806810">this</span> <span m="3807110">is</span>
  <span m="3807290">a</span> <span m="3807380">transverse</span> <span m="3807950">scan</span>
  <span m="3808800">of</span> <span m="3809900">the</span> <span m="3810020">lung.</span>
  <span m="3811370">And</span> <span m="3811850">they</span> <span m="3812090">have</span>
  <span m="3812360">a</span> <span m="3812510">deep</span> <span m="3812810">learning</span>
  <span m="3813410">machine</span> <span m="3814100">that</span> <span m="3814310">is</span>
  <span m="3814460">able</span> <span m="3814760">to</span> <span m="3814940">identify</span>
  <span m="3816170">these</span> <span m="3816500">two</span> <span m="3816710">yellow</span>
  <span m="3817070">marked</span> <span m="3817460">things</span> <span m="3817880">as</span>
  <span m="3818030">pulmonary</span> <span m="3818650">emboli</span> <span m="3819800">as</span>
  <span m="3820070">opposed</span> <span m="3820520">to</span> <span m="3820670">these</span>
  <span m="3821000">other</span> <span m="3821300">things</span> <span m="3821810">that</span>
  <span m="3822020">are</span> <span m="3822170">just</span> <span m="3822470">random</span>
  <span m="3822890">flecks</span> <span m="3823880">in</span> <span m="3824030">the</span>
  <span m="3824150">tissue.</span> <span m="3825270">And</span> <span m="3825350">I</span>
  <span m="3825500">can't</span> <span m="3825830">do</span> <span m="3826010">that</span>
  <span m="3826280">by</span> <span m="3826550">eyeball.</span> <span m="3827820">Maybe</span>
  <span m="3828380">a</span> <span m="3828470">good</span> <span m="3828680">radiologist</span>
  <span m="3829550">might</span> <span m="3829790">be</span> <span m="3829970">able</span>
  <span m="3830240">to,</span> <span m="3831230">but</span> <span m="3831500">this</span>
  <span m="3831800">is</span> <span m="3831980">claimed</span> <span m="3832670">in</span>
  <span m="3832850">the</span> <span m="3832940">paper</span> <span m="3833390">to</span>
  <span m="3833600">outperform</span> <span m="3835340">decent</span> <span m="3835790">radiologists</span>
  <span m="3837010">already.</span></p><p><span m="3838070">This</span> <span m="3838340">was</span>
  <span m="3838520">one</span> <span m="3838760">of</span> <span m="3838910">the</span>
  <span m="3839090">articles</span> <span m="3839690">that</span> <span m="3839930">led</span>
  <span m="3840200">Geoff</span> <span m="3840530">Hinton</span> <span m="3841430">to</span>
  <span m="3841610">make</span> <span m="3841880">this</span> <span m="3842120">rather</span>
  <span m="3842450">stupid</span> <span m="3842900">pronouncement</span> <span m="3843710">that</span>
  <span m="3843920">said,</span> <span m="3845450">tell</span> <span m="3845720">your</span>
  <span m="3845900">children</span> <span m="3846500">not</span> <span m="3846720">to</span>
  <span m="3846810">become</span> <span m="3847260">radiologists</span> <span m="3848130">because</span>
  <span m="3848550">the</span> <span m="3848670">profession</span> <span m="3849360">will</span>
  <span m="3849570">be</span> <span m="3850200">over</span> <span m="3850800">by</span>
  <span m="3851100">the</span> <span m="3851250">time</span> <span m="3851520">they</span>
  <span m="3851850">get</span> <span m="3852060">fully</span> <span m="3852390">trained,</span>
  <span m="3853530">which</span> <span m="3853830">I</span> <span m="3853920">don't</span>
  <span m="3854160">believe.</span> <span m="3855060">They</span> <span m="3855240">may</span>
  <span m="3855420">do</span> <span m="3855600">different</span> <span m="3855990">things,</span>
  <span m="3856520">but</span> <span m="3857280">they</span> <span m="3857430">won't</span>
  <span m="3857640">go</span> <span m="3857820">away.</span></p><p><span m="3860670">This</span>
  <span m="3861000">was</span> <span m="3861840">a</span> <span m="3861930">slide</span>
  <span m="3862290">from</span> <span m="3862530">Ron</span> <span m="3862800">Kikinis</span>
  <span m="3864210">at</span> <span m="3864450">the</span> <span m="3864540">Brigham,</span>
  <span m="3865170">and</span> <span m="3865470">they're</span> <span m="3865650">using</span>
  <span m="3866700">automated</span> <span m="3867180">techniques</span> <span m="3867960">of</span>
  <span m="3869340">analyzing</span> <span m="3869940">white</span> <span m="3870240">matter</span>
  <span m="3870810">in</span> <span m="3871020">order</span> <span m="3871380">to</span>
  <span m="3871830">identify</span> <span m="3873030">lupus</span> <span m="3873450">lesions.</span>
  <span m="3873810">So</span> <span m="3874170">lupus</span> <span m="3874680">is</span>
  <span m="3874860">a</span> <span m="3874920">bad</span> <span m="3875220">disease</span>
  <span m="3875820">that</span> <span m="3877350">shows</span> <span m="3877800">up</span>
  <span m="3878490">in</span> <span m="3878760">these</span> <span m="3879870">magnetic</span>
  <span m="3880410">resonance</span> <span m="3880980">images</span> <span m="3882300">in</span>
  <span m="3882510">certain</span> <span m="3882930">ways.</span></p><p><span m="3884880">The</span>
  <span m="3885030">last</span> <span m="3885300">thing</span> <span m="3885510">I</span>
  <span m="3885600">want</span> <span m="3885750">to</span> <span m="3885840">talk</span>
  <span m="3886110">about</span> <span m="3886380">today</span> <span m="3886710">is</span>
  <span m="3886860">notes.</span> <span m="3888210">So</span> <span m="3890340">my</span>
  <span m="3890610">students</span> <span m="3891140">did</span> <span m="3891330">a</span>
  <span m="3891360">little</span> <span m="3891660">exercise</span> <span m="3892920">last</span>
  <span m="3893220">semester</span> <span m="3894420">where</span> <span m="3895860">we</span>
  <span m="3896070">tried</span> <span m="3896390">to</span> <span m="3896550">see</span>
  <span m="3897840">how</span> <span m="3898140">good</span> <span m="3898490">is</span>
  <span m="3898770">the</span> <span m="3899190">average</span> <span m="3899700">ape,</span>
  <span m="3900450">namely</span> <span m="3901320">member</span> <span m="3901740">of</span>
  <span m="3901860">my</span> <span m="3902040">research</span> <span m="3902520">group,</span>
  <span m="3903750">at</span> <span m="3903990">predicting</span> <span m="3904560">mortality?</span>
  <span m="3907390">And</span> <span m="3907470">so</span> <span m="3907710">we</span>
  <span m="3907890">took</span> <span m="3908160">a</span> <span m="3908220">bunch</span>
  <span m="3908520">of</span> <span m="3908640">cases</span> <span m="3909240">from</span>
  <span m="3909540">the</span> <span m="3909630">MIMIC</span> <span m="3910070">data</span>
  <span m="3910330">set,</span> <span m="3911130">blinded</span> <span m="3911790">to</span>
  <span m="3911970">the</span> <span m="3912570">question</span> <span m="3913080">of</span>
  <span m="3913230">whether</span> <span m="3913530">the</span> <span m="3913650">person</span>
  <span m="3914100">lived</span> <span m="3914400">or</span> <span m="3914490">died.</span>
  <span m="3915390">We</span> <span m="3915600">gave</span> <span m="3915840">the</span>
  <span m="3915960">data</span> <span m="3916290">to</span> <span m="3916470">people</span>
  <span m="3916920">in</span> <span m="3917100">a</span> <span m="3917190">kind</span>
  <span m="3917460">of</span> <span m="3917520">visualization</span> <span m="3918450">tool,</span>
  <span m="3918780">sort</span> <span m="3919050">of</span> <span m="3919170">like</span>
  <span m="3919410">the</span> <span m="3919500">one</span> <span m="3919710">that</span>
  <span m="3920220">I</span> <span m="3920340">showed</span> <span m="3920670">you</span>
  <span m="3920790">earlier,</span> <span m="3921630">that</span> <span m="3921840">summarizes</span>
  <span m="3922980">the</span> <span m="3923100">case,</span> <span m="3924220">and</span>
  <span m="3924600">then</span> <span m="3924990">also</span> <span m="3925470">gave</span>
  <span m="3925770">people</span> <span m="3926160">access</span> <span m="3926610">to</span>
  <span m="3926760">the</span> <span m="3926910">notes,</span> <span m="3927570">the</span>
  <span m="3927840">deidentified</span> <span m="3928470">notes</span> <span m="3929370">about</span>
  <span m="3929730">those</span> <span m="3929970">cases,</span> <span m="3930930">to</span>
  <span m="3931080">see</span> <span m="3931380">whether</span> <span m="3931740">people</span>
  <span m="3932130">could</span> <span m="3932340">predict,</span> <span m="3933390">better</span>
  <span m="3933780">than</span> <span m="3934170">a</span> <span m="3934230">coin</span>
  <span m="3934560">flip,</span> <span m="3935790">whether</span> <span m="3936270">somebody</span>
  <span m="3936750">was</span> <span m="3936960">going</span> <span m="3937230">to</span>
  <span m="3937320">live</span> <span m="3937560">or</span> <span m="3937650">die.</span></p><p><span
  m="3939150">And</span> <span m="3939300">the</span> <span m="3939450">answer</span>
  <span m="3939840">is</span> <span m="3940410">yes,</span> <span m="3940890">slightly</span>
  <span m="3941460">better,</span> <span m="3942170">OK?</span> <span m="3942870">Not</span>
  <span m="3943350">immensely</span> <span m="3943920">better</span> <span m="3944670">but</span>
  <span m="3944880">slightly</span> <span m="3945360">better.</span> <span m="3946170">And</span>
  <span m="3946320">furthermore,</span> <span m="3947190">it</span> <span m="3947370">looks</span>
  <span m="3947730">like,</span> <span m="3948660">by</span> <span m="3948960">giving</span>
  <span m="3949320">them</span> <span m="3949470">feedback,</span> <span m="3950380">so</span>
  <span m="3950580">as</span> <span m="3950790">they're</span> <span m="3951480">looking</span>
  <span m="3951840">at</span> <span m="3951960">these</span> <span m="3952200">cases</span>
  <span m="3952890">and</span> <span m="3953040">trying</span> <span m="3953340">to</span>
  <span m="3953460">make</span> <span m="3953700">the</span> <span m="3953820">prediction,</span>
  <span m="3954960">they</span> <span m="3955140">make</span> <span m="3955380">a</span>
  <span m="3955440">prediction,</span> <span m="3955950">you</span> <span m="3956070">tell</span>
  <span m="3956250">them</span> <span m="3956370">if</span> <span m="3956490">they</span>
  <span m="3956640">were</span> <span m="3956790">right</span> <span m="3957030">or</span>
  <span m="3957120">wrong,</span> <span m="3958710">we</span> <span m="3958920">learn.</span>
  <span m="3960000">And</span> <span m="3960150">so</span> <span m="3960360">we</span>
  <span m="3960480">get</span> <span m="3960720">slightly</span> <span m="3961260">better</span>
  <span m="3962370">than</span> <span m="3962610">slightly</span> <span m="3963180">better</span>
  <span m="3963480">than</span> <span m="3963720">random,</span> <span m="3965380">right?</span>
  <span m="3965950">It's</span> <span m="3966060">kind</span> <span m="3966300">of</span>
  <span m="3966390">interesting.</span></p><p><span m="3967940">OK,</span> <span m="3968820">so</span>
  <span m="3969510">one</span> <span m="3969750">of</span> <span m="3969870">the</span>
  <span m="3969960">things</span> <span m="3970320">I</span> <span m="3970410">discovered</span>
  <span m="3971250">is</span> <span m="3971460">that,</span> <span m="3971820">at</span>
  <span m="3971970">least</span> <span m="3972270">when</span> <span m="3972450">I</span>
  <span m="3972570">was</span> <span m="3973080">playing</span> <span m="3973440">the</span>
  <span m="3973530">monkey</span> <span m="3973950">in</span> <span m="3974070">this</span>
  <span m="3974430">exercise,</span> <span m="3976050">I</span> <span m="3976200">found</span>
  <span m="3976590">the</span> <span m="3976710">notes</span> <span m="3977160">to</span>
  <span m="3977280">be</span> <span m="3977490">immensely</span> <span m="3978000">useful,</span>
  <span m="3979350">much</span> <span m="3979620">more</span> <span m="3979890">useful</span>
  <span m="3980490">than</span> <span m="3980730">the</span> <span m="3980850">trend</span>
  <span m="3981180">lines</span> <span m="3982140">of</span> <span m="3982350">laboratory</span>
  <span m="3982980">data.</span> <span m="3984660">Partly,</span> <span m="3985140">it's</span>
  <span m="3985350">because</span> <span m="3985560">I'm</span> <span m="3985710">used</span>
  <span m="3985950">to</span> <span m="3986070">reading</span> <span m="3986490">English.</span>
  <span m="3987390">I'm</span> <span m="3987540">not</span> <span m="3987750">so</span>
  <span m="3987930">used</span> <span m="3988200">to</span> <span m="3988320">reading</span>
  <span m="3989610">graphs</span> <span m="3990060">of</span> <span m="3990180">laboratory</span>
  <span m="3990810">data.</span> <span m="3991950">But</span> <span m="3992190">part</span>
  <span m="3992460">of</span> <span m="3992580">it</span> <span m="3992700">is</span>
  <span m="3992910">that</span> <span m="3993090">there</span> <span m="3993200">is</span>
  <span m="3993680">a</span> <span m="3993750">level</span> <span m="3994110">of</span>
  <span m="3994230">human</span> <span m="3994590">understanding</span> <span m="3995430">that</span>
  <span m="3995610">is</span> <span m="3995790">transmitted</span> <span m="3997110">in</span>
  <span m="3997410">the</span> <span m="3997710">nursing</span> <span m="3998190">notes</span>
  <span m="3998670">and</span> <span m="3998800">in</span> <span m="3998940">the</span>
  <span m="3999060">discharge</span> <span m="3999540">summaries</span> <span m="4000080">and</span>
  <span m="4000200">so</span> <span m="4000440">on</span> <span m="4001100">that</span>
  <span m="4001400">you</span> <span m="4001520">don't</span> <span m="4001790">get</span>
  <span m="4002120">from</span> <span m="4002420">just</span> <span m="4002690">looking</span>
  <span m="4003080">at</span> <span m="4003230">raw</span> <span m="4003440">data.</span></p><p><span
  m="4004340">And</span> <span m="4004490">so</span> <span m="4005000">there</span>
  <span m="4005330">is</span> <span m="4005540">very</span> <span m="4005810">much</span>
  <span m="4006110">the</span> <span m="4006260">sense,</span> <span m="4007010">which</span>
  <span m="4007310">we're</span> <span m="4007460">going</span> <span m="4007610">to</span>
  <span m="4007670">talk</span> <span m="4007970">about</span> <span m="4008270">in</span>
  <span m="4008420">a</span> <span m="4008450">couple</span> <span m="4008780">of</span>
  <span m="4008870">weeks,</span> <span m="4009800">of</span> <span m="4010280">how</span>
  <span m="4010760">can</span> <span m="4011060">we</span> <span m="4011930">take</span>
  <span m="4012260">advantage</span> <span m="4013370">of</span> <span m="4013520">that</span>
  <span m="4013730">information,</span> <span m="4014930">extract it,</span> <span
  m="4015800">and</span> <span m="4016010">use</span> <span m="4016370">it</span>
  <span m="4016490">in</span> <span m="4016610">the</span> <span m="4016730">kinds</span>
  <span m="4017030">of</span> <span m="4017150">modeling</span> <span m="4017600">that</span>
  <span m="4017780">we</span> <span m="4017930">want</span> <span m="4018110">to</span>
  <span m="4018170">do?</span> <span m="4019140">So</span> <span m="4019250">in</span>
  <span m="4019370">MIMIC,</span> <span m="4019920">if</span> <span m="4020030">you</span>
  <span m="4020180">look,</span> <span m="4020840">we</span> <span m="4021050">have</span>
  <span m="4021710">nursing</span> <span m="4022130">notes,</span> <span m="4022580">and</span>
  <span m="4022700">radiology</span> <span m="4023390">reports,</span> <span m="4024080">and</span>
  <span m="4024290">more</span> <span m="4024560">nursing</span> <span m="4025040">notes,</span>
  <span m="4026030">and</span> <span m="4026390">electrocardiogram</span> <span m="4027470">reports,</span>
  <span m="4028160">and</span> <span m="4028490">doctor's</span> <span m="4029000">notes,</span>
  <span m="4029420">and</span> <span m="4029540">discharge</span> <span m="4030020">summaries,</span>
  <span m="4030600">and</span> <span m="4031760">echocardiograms,</span> <span m="4032990">respiratory,</span>
  <span m="4033770">et</span> <span m="4034070">cetera.</span> <span m="4036170">And</span>
  <span m="4036350">if</span> <span m="4036500">you</span> <span m="4036650">look</span>
  <span m="4036920">at</span> <span m="4037100">the</span> <span m="4037820">distribution</span>
  <span m="4038630">of</span> <span m="4039110">the</span> <span m="4039230">lengths</span>
  <span m="4039830">of</span> <span m="4040040">these,</span> <span m="4041501">these</span>
  <span m="4041990">are,</span> <span m="4042110">unfortunately,</span> <span m="4042950">not</span>
  <span m="4043220">on</span> <span m="4043340">the</span> <span m="4043460">same</span>
  <span m="4043760">scale.</span></p><p><span m="4044780">But</span> <span m="4045020">the</span>
  <span m="4045140">discharge</span> <span m="4045680">summary</span> <span m="4046220">is</span>
  <span m="4046400">the</span> <span m="4046520">thing</span> <span m="4046790">that's</span>
  <span m="4047030">written</span> <span m="4047630">at</span> <span m="4047810">the</span>
  <span m="4047960">time</span> <span m="4048260">you</span> <span m="4048410">leave</span>
  <span m="4048680">the</span> <span m="4048770">hospital.</span> <span m="4050010">So</span>
  <span m="4050090">this</span> <span m="4050330">is</span> <span m="4050420">sort</span>
  <span m="4050690">of</span> <span m="4050780">the</span> <span m="4050930">summary</span>
  <span m="4051560">of</span> <span m="4051740">everything</span> <span m="4052190">that</span>
  <span m="4052340">happened</span> <span m="4052700">to</span> <span m="4052850">you</span>
  <span m="4053270">during</span> <span m="4053570">your</span> <span m="4053690">hospitalization.</span>
  <span m="4055310">And</span> <span m="4055490">it's</span> <span m="4055670">long.</span>
  <span m="4056330">So,</span> <span m="4056960">you</span> <span m="4057030">know,</span>
  <span m="4057320">it</span> <span m="4057380">goes</span> <span m="4057710">up</span>
  <span m="4057890">to</span> <span m="4058130">like</span> <span m="4058400">30,000</span>
  <span m="4059480">characters.</span> <span m="4061190">You</span> <span m="4061490">know,</span>
  <span m="4063650">it's</span> <span m="4063860">a</span> <span m="4063890">short</span>
  <span m="4064220">story,</span> <span m="4065260">not</span> <span m="4065840">so</span>
  <span m="4066020">short</span> <span m="4066390">short</span> <span m="4066710">story.</span></p><p><span
  m="4068240">Nursing</span> <span m="4068750">notes</span> <span m="4069110">tend</span>
  <span m="4069350">to</span> <span m="4069470">be</span> <span m="4069650">shorter.</span>
  <span m="4070580">They</span> <span m="4070730">run</span> <span m="4070970">up</span>
  <span m="4071120">to</span> <span m="4071270">about</span> <span m="4071570">3,000</span>
  <span m="4072290">characters.</span> <span m="4073490">This</span> <span m="4073760">other</span>
  <span m="4074030">set</span> <span m="4074300">of</span> <span m="4074420">nursing</span>
  <span m="4074840">notes,</span> <span m="4075320">which</span> <span m="4075500">I</span>
  <span m="4075590">think</span> <span m="4076100">comes</span> <span m="4076430">from</span>
  <span m="4076640">the</span> <span m="4076760">other</span> <span m="4077000">system,</span>
  <span m="4077960">is</span> <span m="4078110">a</span> <span m="4078140">little</span>
  <span m="4078380">bit</span> <span m="4078590">longer.</span> <span m="4079040">It</span>
  <span m="4079100">goes</span> <span m="4079370">up</span> <span m="4079520">to</span>
  <span m="4079670">about</span> <span m="4079990">5,000.</span></p><p><span m="4081560">Doctor's</span>
  <span m="4082130">notes</span> <span m="4082580">are</span> <span m="4082700">a</span>
  <span m="4082730">little</span> <span m="4082970">bit</span> <span m="4083180">longer</span>
  <span m="4083600">yet.</span> <span m="4083930">They</span> <span m="4084110">go</span>
  <span m="4084320">up</span> <span m="4084440">to</span> <span m="4084620">about</span>
  <span m="4084920">10,000,</span> <span m="4085160">15,000</span> <span m="4086480">characters,</span>
  <span m="4087320">typically.</span> <span m="4089030">And</span> <span m="4089360">there</span>
  <span m="4089600">are</span> <span m="4089660">various</span> <span m="4090140">other</span>
  <span m="4090410">kinds</span> <span m="4090740">of</span> <span m="4090860">notes.</span>
  <span m="4091760">So</span> <span m="4091970">I</span> <span m="4092060">just</span>
  <span m="4092270">wanted</span> <span m="4092510">to</span> <span m="4092660">show</span>
  <span m="4092930">you</span> <span m="4093110">a</span> <span m="4093170">few</span>
  <span m="4093470">of</span> <span m="4093590">these.</span></p><p><span m="4094470">Here's</span>
  <span m="4094640">a</span> <span m="4094730">brief</span> <span m="4095090">nursing</span>
  <span m="4095570">note.</span> <span m="4096080">So</span> <span m="4096290">this</span>
  <span m="4096560">is</span> <span m="4096710">a</span> <span m="4096770">patient</span>
  <span m="4097760">who</span> <span m="4097910">is</span> <span m="4098060">hypotensive</span>
  <span m="4098899">but</span> <span m="4099109">not</span> <span m="4099350">in</span>
  <span m="4099500">shock.</span> <span m="4100939">Patient</span> <span m="4101450">remains</span>
  <span m="4102080">on</span> <span m="4102350">this</span> <span m="4102620">drug</span>
  <span m="4102950">drip</span> <span m="4103399">at</span> <span m="4103670">0.75</span>
  <span m="4105410">micrograms</span> <span m="4106189">per</span> <span m="4106399">kilogram</span>
  <span m="4107000">per</span> <span m="4107180">minute,</span> <span m="4107930">no</span>
  <span m="4108170">titration</span> <span m="4108859">needed</span> <span m="4109220">at</span>
  <span m="4109370">this</span> <span m="4109609">time.</span> <span m="4110479">Their</span>
  <span m="4110660">blood</span> <span m="4110899">pressure</span> <span m="4111319">is</span>
  <span m="4111410">stable</span> <span m="4111950">at</span> <span m="4112100">more</span>
  <span m="4112310">than</span> <span m="4112490">100.</span> <span m="4112810">Their</span>
  <span m="4113130">mean</span> <span m="4113430">arterial</span> <span m="4113960">pressure</span>
  <span m="4114380">is</span> <span m="4114580">65,</span> <span m="4115640">greater</span>
  <span m="4115939">than</span> <span m="4116120">65.</span> <span m="4118130">Wean</span>
  <span m="4118520">them</span> <span m="4118790">from</span> <span m="4119120">this</span>
  <span m="4119359">drug</span> <span m="4119750">presumably</span> <span m="4120560">if</span>
  <span m="4121160">it's</span> <span m="4121340">tolerated.</span></p><p><span m="4122660">A</span>
  <span m="4123229">wound</span> <span m="4123649">infection,</span> <span m="4125240">so</span>
  <span m="4125620">anterior</span> <span m="4126380">groin</span> <span m="4126770">area</span>
  <span m="4127220">open</span> <span m="4127640">and</span> <span m="4127910">oozing</span>
  <span m="4128960">moderate</span> <span m="4129680">amounts</span> <span m="4130160">of</span>
  <span m="4130250">thin,</span> <span m="4131120">pink-tinged</span> <span m="4132050">serous</span>
  <span m="4132560">fluid.</span> <span m="4133479">Patient's</span> <span m="4134000">stooling</span>
  <span m="4134569">with</span> <span m="4134750">small</span> <span m="4135109">amounts</span>
  <span m="4135439">of</span> <span m="4135500">stool</span> <span m="4136040">on</span>
  <span m="4137000">something</span> <span m="4137660">and</span> <span m="4137870">dangerously</span>
  <span m="4138590">close</span> <span m="4138950">to</span> <span m="4139069">the</span>
  <span m="4139250">open</span> <span m="4139580">wound,</span> <span m="4140300">et</span>
  <span m="4140490">cetera.</span> <span m="4141170">So</span> <span m="4141229">this</span>
  <span m="4141500">is</span> <span m="4141560">sort</span> <span m="4141830">of</span>
  <span m="4141979">the</span> <span m="4142130">nurse's</span> <span m="4143210">snapshot.</span>
  <span m="4144200">She</span> <span m="4144410">just</span> <span m="4144680">went</span>
  <span m="4144920">in,</span> <span m="4145520">saw</span> <span m="4145819">the</span>
  <span m="4145939">patient--</span> <span m="4147010">by</span> <span m="4147160">the</span>
  <span m="4147220">way,</span> <span m="4147399">I</span> <span m="4147490">say</span>
  <span m="4147760">she,</span> <span m="4148015">but</span> <span m="4149950">probably</span>
  <span m="4150399">a</span> <span m="4150729">vast</span> <span m="4151120">majority</span>
  <span m="4151660">of</span> <span m="4151779">nurses</span> <span m="4152470">in</span>
  <span m="4152800">Boston</span> <span m="4153279">area</span> <span m="4153520">hospitals</span>
  <span m="4154540">really</span> <span m="4154840">are</span> <span m="4154990">women,</span>
  <span m="4155500">but</span> <span m="4155740">there</span> <span m="4155920">are</span>
  <span m="4156069">some</span> <span m="4156340">male</span> <span m="4156580">nurses--</span>
  <span m="4159189">and</span> <span m="4159640">will</span> <span m="4159910">record</span>
  <span m="4160779">sort</span> <span m="4161050">of</span> <span m="4161170">a</span>
  <span m="4161229">snapshot</span> <span m="4161890">of</span> <span m="4162010">what's</span>
  <span m="4162250">going</span> <span m="4162550">on</span> <span m="4162700">with</span>
  <span m="4162880">the</span> <span m="4162970">patient.</span></p><p><span m="4164149">What</span>
  <span m="4164229">are</span> <span m="4164350">the</span> <span m="4164470">concerns?</span>
  <span m="4165729">In</span> <span m="4165880">principle,</span> <span m="4166660">this</span>
  <span m="4166930">is</span> <span m="4167080">going</span> <span m="4167350">to</span>
  <span m="4167500">be</span> <span m="4167649">useful</span> <span m="4168220">not</span>
  <span m="4168490">only</span> <span m="4168970">as</span> <span m="4169300">a</span>
  <span m="4169600">part</span> <span m="4169930">of</span> <span m="4170020">the</span>
  <span m="4170140">medical</span> <span m="4170529">record,</span> <span m="4171500">but</span>
  <span m="4171609">also</span> <span m="4171970">when</span> <span m="4172210">this</span>
  <span m="4172420">nurse</span> <span m="4172720">goes</span> <span m="4173020">off</span>
  <span m="4173260">shift</span> <span m="4174160">and</span> <span m="4174370">the</span>
  <span m="4174490">next</span> <span m="4174790">nurse</span> <span m="4175090">comes</span>
  <span m="4175420">on</span> <span m="4175630">shift.</span> <span m="4176470">Then</span>
  <span m="4176770">this</span> <span m="4177010">is</span> <span m="4177160">a</span>
  <span m="4177220">recording</span> <span m="4177880">of</span> <span m="4178060">what</span>
  <span m="4178270">the</span> <span m="4178359">state</span> <span m="4178720">of</span>
  <span m="4178840">the</span> <span m="4178930">patient</span> <span m="4179380">was</span>
  <span m="4179680">the</span> <span m="4179800">last</span> <span m="4180040">time</span>
  <span m="4180310">they</span> <span m="4180460">were</span> <span m="4180580">seen</span>
  <span m="4180880">by</span> <span m="4181810">the</span> <span m="4181960">nurse.</span>
  <span m="4183130">In</span> <span m="4183370">reality,</span> <span m="4184029">the</span>
  <span m="4184210">nurses</span> <span m="4184660">tend</span> <span m="4184899">to</span>
  <span m="4185080">tell</span> <span m="4185350">each</span> <span m="4185560">other</span>
  <span m="4185800">verbally</span> <span m="4186939">rather</span> <span m="4187359">than</span>
  <span m="4187689">relying</span> <span m="4188229">on</span> <span m="4188380">the</span>
  <span m="4188460">written</span> <span m="4188740">version.</span></p><p><span m="4190750">I</span>
  <span m="4191080">remember</span> <span m="4191500">one</span> <span m="4191740">time</span>
  <span m="4192010">talking</span> <span m="4192460">to</span> <span m="4192700">a</span>
  <span m="4192760">nurse</span> <span m="4193240">in</span> <span m="4193420">an</span>
  <span m="4193540">intensive</span> <span m="4194080">care</span> <span m="4194350">unit</span>
  <span m="4194740">in</span> <span m="4195370">another</span> <span m="4195700">part</span>
  <span m="4195970">of</span> <span m="4196030">the</span> <span m="4196120">country,</span>
  <span m="4196570">and</span> <span m="4196690">I</span> <span m="4196810">said,</span>
  <span m="4197080">so</span> <span m="4197680">whoever</span> <span m="4198160">reads</span>
  <span m="4198610">your</span> <span m="4198760">notes,</span> <span m="4199960">and</span>
  <span m="4200140">she</span> <span m="4200350">says,</span> <span m="4203320">quality</span>
  <span m="4203830">assurance</span> <span m="4204370">officers,</span> <span m="4206110">so</span>
  <span m="4206350">the</span> <span m="4206770">hospital</span> <span m="4207340">has</span>
  <span m="4208060">people</span> <span m="4208450">responsible</span> <span m="4209200">for</span>
  <span m="4209410">trying</span> <span m="4209740">to</span> <span m="4209920">assess</span>
  <span m="4210310">the</span> <span m="4210400">quality</span> <span m="4210850">of</span>
  <span m="4210970">care</span> <span m="4211210">they're</span> <span m="4211420">giving,</span>
  <span m="4212740">and</span> <span m="4212980">lawyers</span> <span m="4213580">when</span>
  <span m="4213790">there's</span> <span m="4214030">a</span> <span m="4214090">lawsuit.</span>
  <span m="4215890">And</span> <span m="4216070">she</span> <span m="4216280">was</span>
  <span m="4216520">very</span> <span m="4216790">happy</span> <span m="4217240">because</span>
  <span m="4217660">she</span> <span m="4217930">had</span> <span m="4218080">saved</span>
  <span m="4218500">the</span> <span m="4218620">hospital</span> <span m="4219190">10</span>
  <span m="4219460">million</span> <span m="4219850">dollars</span> <span m="4220900">by</span>
  <span m="4221170">having</span> <span m="4221560">carefully</span> <span m="4222160">recorded</span>
  <span m="4222910">that</span> <span m="4223150">some</span> <span m="4223780">procedure</span>
  <span m="4224410">had</span> <span m="4224620">been</span> <span m="4224920">done</span>
  <span m="4225190">to</span> <span m="4225430">a</span> <span m="4225490">patient</span>
  <span m="4226510">who</span> <span m="4226660">then</span> <span m="4226900">had</span>
  <span m="4227110">a</span> <span m="4227170">bad</span> <span m="4227470">outcome</span>
  <span m="4228080">and</span> <span m="4228100">was</span> <span m="4228250">suing</span>
  <span m="4228670">the</span> <span m="4228760">hospital</span> <span m="4229780">for</span>
  <span m="4230560">their</span> <span m="4230830">neglect</span> <span m="4231430">in</span>
  <span m="4231550">not</span> <span m="4231790">having</span> <span m="4232120">done</span>
  <span m="4232390">this.</span> <span m="4233050">But</span> <span m="4233290">because</span>
  <span m="4233740">it</span> <span m="4233860">was</span> <span m="4234130">in</span>
  <span m="4234250">the</span> <span m="4234370">note,</span> <span m="4235210">that</span>
  <span m="4235390">was</span> <span m="4235600">proof</span> <span m="4235990">that</span>
  <span m="4236170">it</span> <span m="4236290">actually</span> <span m="4236740">had</span>
  <span m="4236920">been</span> <span m="4237130">done,</span> <span m="4237670">and</span>
  <span m="4238030">therefore</span> <span m="4238510">the</span> <span m="4238600">hospital</span>
  <span m="4239770">wasn't</span> <span m="4240160">liable.</span> <span m="4243310">But</span>
  <span m="4243550">there</span> <span m="4243650">is</span> <span m="4243760">a</span>
  <span m="4243820">lot</span> <span m="4244060">of</span> <span m="4244150">information</span>
  <span m="4244840">in</span> <span m="4244960">here.</span></p><p><span m="4245950">Now,</span>
  <span m="4246450">I'm</span> <span m="4246580">going</span> <span m="4246700">to</span>
  <span m="4246790">show</span> <span m="4247090">you</span> <span m="4247750">many</span>
  <span m="4248080">pages</span> <span m="4248830">of</span> <span m="4249010">a</span>
  <span m="4249070">typical</span> <span m="4249610">discharge</span> <span m="4250090">summary.</span>
  <span m="4251020">So</span> <span m="4251200">this</span> <span m="4251440">is</span>
  <span m="4251530">somebody</span> <span m="4252010">on</span> <span m="4252160">the</span>
  <span m="4252250">surgery</span> <span m="4252760">service</span> <span m="4254800">who</span>
  <span m="4255040">came</span> <span m="4255400">in</span> <span m="4255610">complaining</span>
  <span m="4256270">of</span> <span m="4257110">leg</span> <span m="4257410">pain,</span>
  <span m="4259160">redness,</span> <span m="4259750">and</span> <span m="4259930">swelling</span>
  <span m="4260560">secondary</span> <span m="4261220">to</span> <span m="4261400">infection</span>
  <span m="4262630">of</span> <span m="4262900">the</span> <span m="4263950">left</span>
  <span m="4264370">femoral</span> <span m="4265720">popliteal</span> <span m="4266500">bypass.</span>
  <span m="4267610">So</span> <span m="4267820">she</span> <span m="4268030">had</span>
  <span m="4268270">surgery--</span> <span m="4269980">I</span> <span m="4270040">think</span>
  <span m="4270280">she.</span> <span m="4270700">Yeah,</span> <span m="4270940">female.</span>
  <span m="4271810">She</span> <span m="4272020">had</span> <span m="4272230">surgery</span>
  <span m="4272980">which</span> <span m="4273460">didn't</span> <span m="4273820">heal</span>
  <span m="4274090">well,</span> <span m="4275320">so</span> <span m="4276370">major</span>
  <span m="4276730">surgical</span> <span m="4277330">or</span> <span m="4277420">invasive</span>
  <span m="4277900">procedure,</span> <span m="4278920">incision</span> <span m="4279430">and</span>
  <span m="4279550">drainage</span> <span m="4280090">and</span> <span m="4280210">pulse</span>
  <span m="4280570">irrigation</span> <span m="4281200">of</span> <span m="4281350">the</span>
  <span m="4281440">left</span> <span m="4281770">groin,</span> <span m="4282670">and</span>
  <span m="4282850">left</span> <span m="4283210">above-knee</span> <span m="4284260">popliteal</span>
  <span m="4285590">site</span> <span m="4286420">incisions</span> <span m="4287230">with</span>
  <span m="4288130">exploration</span> <span m="4289150">of</span> <span m="4289360">bypass</span>
  <span m="4289960">graft,</span> <span m="4291280">and</span> <span m="4291670">excision</span>
  <span m="4292300">of</span> <span m="4292420">the</span> <span m="4292630">entire</span>
  <span m="4293110">left</span> <span m="4293410">common</span> <span m="4293830">femoral</span>
  <span m="4294370">artery</span> <span m="4294850">to</span> <span m="4295630">above-knee</span>
  <span m="4296320">blah, blah,</span> <span m="4296670">blah, blah</span> <span m="4297000">blah,</span>
  <span m="4297110">blah.</span> <span m="4297460">So</span> <span m="4297670">this</span>
  <span m="4297880">is</span> <span m="4298000">what</span> <span m="4298180">they</span>
  <span m="4298360">did.</span></p><p><span m="4300010">History</span> <span m="4300430">of</span>
  <span m="4300550">the</span> <span m="4300640">present</span> <span m="4301060">illness--</span>
  <span m="4301910">she's</span> <span m="4302200">a</span> <span m="4302260">45-year-old</span>
  <span m="4303220">woman</span> <span m="4303580">who</span> <span m="4303730">underwent</span>
  <span m="4304280">the</span> <span m="4304360">left</span> <span m="4304690">femoral,</span>
  <span m="4305560">a.k.a.</span> <span m="4307130">doctor</span> <span m="4307840">something</span>
  <span m="4308350">or</span> <span m="4308440">other</span> <span m="4309220">with</span>
  <span m="4309670">PTFE,</span> <span m="4310750">whatever</span> <span m="4311170">that</span>
  <span m="4311410">is,</span> <span m="4311680">over</span> <span m="4312040">a</span>
  <span m="4312070">month</span> <span m="4312400">ago</span> <span m="4313540">on</span>
  <span m="4313810">a</span> <span m="4313840">certain</span> <span m="4314290">date.</span>
  <span m="4315130">By</span> <span m="4315310">the</span> <span m="4315400">way,</span>
  <span m="4315610">these</span> <span m="4316090">bracketed</span> <span m="4316630">asterisked</span>
  <span m="4317350">things</span> <span m="4317800">are</span> <span m="4317950">where</span>
  <span m="4318160">we've</span> <span m="4318550">taken</span> <span m="4318970">out</span>
  <span m="4319660">identifying</span> <span m="4320500">information</span> <span
  m="4321340">from</span> <span m="4321610">the</span> <span m="4321700">record.</span>
  <span m="4324310">She</span> <span m="4324550">had</span> <span m="4324670">been</span>
  <span m="4324850">doing</span> <span m="4325120">well</span> <span m="4325300">post-operatively</span>
  <span m="4326320">and</span> <span m="4326410">was</span> <span m="4326560">seen</span>
  <span m="4326890">in</span> <span m="4327010">the</span> <span m="4327100">clinic</span>
  <span m="4327460">six</span> <span m="4327730">days</span> <span m="4327940">prior</span>
  <span m="4328270">to</span> <span m="4328390">presentation.</span> <span m="4329780">At</span>
  <span m="4329800">this</span> <span m="4330040">time,</span> <span m="4330310">she</span>
  <span m="4330520">acutely</span> <span m="4330970">developed</span> <span m="4331420">nausea,</span>
  <span m="4331810">vomiting,</span> <span m="4332320">fevers,</span> <span m="4332770">and</span>
  <span m="4332890">progressive</span> <span m="4333460">redness,</span> <span m="4334460">swelling,</span>
  <span m="4334970">pain</span> <span m="4335200">of</span> <span m="4335350">her</span>
  <span m="4335470">left</span> <span m="4335770">thigh,</span> <span m="4336130">et</span>
  <span m="4336190">cetera,</span> <span m="4337093">OK?</span> <span m="4337940">So</span>
  <span m="4338020">that's</span> <span m="4338290">just</span> <span m="4338530">page</span>
  <span m="4338860">one</span> <span m="4339190">of</span> <span m="4339310">many</span>
  <span m="4339610">pages.</span> <span m="4341170">Yeah.</span></p><p><span m="4341320">AUDIENCE:</span>
  <span m="4341437">Just</span> <span m="4341554">a</span> <span m="4341673">question.</span>
  <span m="4342026">Is</span> <span m="4342380">this</span> <span m="4342530">completely</span>
  <span m="4343302">[INAUDIBLE]</span> <span m="4343690">information</span> <span
  m="4344320">[INAUDIBLE]</span> <span m="4347950">patient's</span> <span m="4348430">name</span>
  <span m="4348720">or</span> <span m="4348830">date?</span></p><p><span m="4349300">PROFESSOR:</span>
  <span m="4349480">Not</span> <span m="4349660">in</span> <span m="4349810">this</span>
  <span m="4350010">system.</span> <span m="4351310">There</span> <span m="4351580">are</span>
  <span m="4351670">people--</span> <span m="4352870">Henry</span> <span m="4353210">Chueh</span>
  <span m="4353490">at</span> <span m="4353800">Mass</span> <span m="4354100">General</span>
  <span m="4354760">spent</span> <span m="4355150">10</span> <span m="4355450">years</span>
  <span m="4355840">building</span> <span m="4356290">a</span> <span m="4356350">system</span>
  <span m="4357310">that</span> <span m="4357520">had</span> <span m="4357790">autocomplete</span>
  <span m="4358780">and</span> <span m="4358930">so</span> <span m="4359200">on.</span>
  <span m="4359890">And</span> <span m="4360430">some</span> <span m="4360790">doctors</span>
  <span m="4361330">liked</span> <span m="4361630">it</span> <span m="4361900">and</span>
  <span m="4362020">some</span> <span m="4362260">doctors</span> <span m="4362770">hated</span>
  <span m="4363130">it.</span> <span m="4363820">And</span> <span m="4364300">the</span>
  <span m="4364930">MGH</span> <span m="4365800">threw</span> <span m="4366175">out</span>
  <span m="4366550">all</span> <span m="4366790">of</span> <span m="4366940">their</span>
  <span m="4367120">old</span> <span m="4367360">systems</span> <span m="4368050">in</span>
  <span m="4368230">order</span> <span m="4368500">to</span> <span m="4368650">buy</span>
  <span m="4369030">Epic,</span> <span m="4370270">and</span> <span m="4370480">so</span>
  <span m="4370700">it's</span> <span m="4370850">gone.</span> <span m="4371090">It</span>
  <span m="4371340">was</span> <span m="4371560">like</span> <span m="4371800">10</span>
  <span m="4372040">years</span> <span m="4372310">of</span> <span m="4372430">work</span>
  <span m="4372700">down</span> <span m="4372940">the</span> <span m="4373030">drain.</span>
  <span m="4374390">But</span> <span m="4374500">it</span> <span m="4374560">was</span>
  <span m="4374770">not</span> <span m="4375040">a</span> <span m="4375100">spectacular</span>
  <span m="4375880">success.</span></p><p><span m="4377740">Because</span> <span m="4378310">whenever</span>
  <span m="4378700">you</span> <span m="4378850">have</span> <span m="4379330">auto</span>
  <span m="4379570">complete,</span> <span m="4380500">you</span> <span m="4380710">have</span>
  <span m="4380890">to</span> <span m="4381040">anticipate</span> <span m="4381790">every</span>
  <span m="4382060">possible</span> <span m="4382660">answer.</span> <span m="4383740">And</span>
  <span m="4383890">people</span> <span m="4384250">are</span> <span m="4384340">very</span>
  <span m="4384610">creative,</span> <span m="4385270">and</span> <span m="4385360">they</span>
  <span m="4385510">always</span> <span m="4385840">want</span> <span m="4386020">to</span>
  <span m="4386080">type</span> <span m="4386380">something</span> <span m="4386890">that</span>
  <span m="4387120">you</span> <span m="4387190">didn't</span> <span m="4387490">anticipate.</span>
  <span m="4389050">So</span> <span m="4389480">it's</span> <span m="4390010">hard</span>
  <span m="4390280">to</span> <span m="4390400">support</span> <span m="4390880">it.</span></p><p><span
  m="4391450">AUDIENCE:</span> <span m="4391562">What</span> <span m="4391674">is</span>
  <span m="4391786">Epic?</span> <span m="4392350">That's like the</span> <span m="4392800">new--</span></p><p><span
  m="4393250">PROFESSOR:</span> <span m="4393430">Epic</span> <span m="4393610">is</span>
  <span m="4393820">a</span> <span m="4393970">big</span> <span m="4394210">company</span>
  <span m="4394690">that</span> <span m="4395290">has</span> <span m="4395530">been</span>
  <span m="4395740">winning</span> <span m="4396160">all</span> <span m="4396370">the</span>
  <span m="4396490">recent</span> <span m="4396880">contests</span> <span m="4397630">for</span>
  <span m="4397930">installing</span> <span m="4399190">electronic</span> <span m="4399760">medical</span>
  <span m="4400150">record</span> <span m="4400540">systems.</span> <span m="4401620">Remember</span>
  <span m="4402040">in</span> <span m="4402130">my</span> <span m="4402310">last</span>
  <span m="4402640">lecture,</span> <span m="4403160">I</span> <span m="4403180">showed</span>
  <span m="4403540">that</span> <span m="4403720">we're</span> <span m="4403930">reaching</span>
  <span m="4404410">about</span> <span m="4404650">100%</span> <span m="4405460">saturation?</span>
  <span m="4406780">So</span> <span m="4407020">they've</span> <span m="4407290">been</span>
  <span m="4407500">winning</span> <span m="4407890">a</span> <span m="4407950">lot</span>
  <span m="4408220">of</span> <span m="4411760">the</span> <span m="4411910">installation</span>
  <span m="4412630">deals.</span> <span m="4414340">And</span> <span m="4414520">they're</span>
  <span m="4414670">getting</span> <span m="4415000">a</span> <span m="4415060">lot</span>
  <span m="4415270">of</span> <span m="4415390">the</span> <span m="4415690">subsidy.</span>
  <span m="4418360">The</span> <span m="4418570">estimate</span> <span m="4419050">I</span>
  <span m="4419200">heard</span> <span m="4419530">was</span> <span m="4419770">that</span>
  <span m="4420460">Partners</span> <span m="4420560">Healthcare,</span> <span m="4421540">which</span>
  <span m="4421780">is</span> <span m="4422140">MGH</span> <span m="4422560">at</span>
  <span m="4422800">the</span> <span m="4422950">Brigham</span> <span m="4423460">and</span>
  <span m="4423610">a</span> <span m="4423670">couple</span> <span m="4423970">of</span>
  <span m="4424090">other</span> <span m="4424240">hospitals,</span> <span m="4425350">spent</span>
  <span m="4425740">somewhere</span> <span m="4426130">on</span> <span m="4426310">the</span>
  <span m="4426460">order</span> <span m="4426910">of</span> <span m="4427180">two</span>
  <span m="4427420">billion</span> <span m="4427900">dollars</span> <span m="4428680">installing</span>
  <span m="4429310">the</span> <span m="4429410">system.</span> <span m="4430940">So</span>
  <span m="4431020">that</span> <span m="4431200">included</span> <span m="4431800">all</span>
  <span m="4431980">the</span> <span m="4432100">customizations</span> <span m="4433270">and</span>
  <span m="4433390">all</span> <span m="4433540">the</span> <span m="4433660">training</span>
  <span m="4434260">and</span> <span m="4434710">all</span> <span m="4434920">the</span>
  <span m="4435220">administrative</span> <span m="4435970">stuff</span> <span m="4436330">that</span>
  <span m="4436510">went</span> <span m="4436750">with</span> <span m="4436990">it.</span>
  <span m="4437560">But</span> <span m="4437740">that's</span> <span m="4437980">a</span>
  <span m="4438040">huge</span> <span m="4438400">amount</span> <span m="4438700">of</span>
  <span m="4438820">money.</span></p><p><span m="4440040">AUDIENCE:</span> <span m="4440270">I</span>
  <span m="4440500">agree.</span></p><p><span m="4441880">PROFESSOR:</span> <span
  m="4442025">OK,</span> <span m="4443110">so</span> <span m="4443440">we</span> <span
  m="4443620">have</span> <span m="4443830">past</span> <span m="4444190">medical</span>
  <span m="4444610">history--</span> <span m="4446600">pack</span> <span m="4446930">a</span>
  <span m="4446960">day</span> <span m="4447200">smoker,</span> <span m="4448430">abused</span>
  <span m="4448970">cocaine</span> <span m="4450320">but</span> <span m="4450600">says</span>
  <span m="4450830">she</span> <span m="4451070">stopped</span> <span m="4451670">six</span>
  <span m="4451970">months</span> <span m="4452300">ago,</span> <span m="4452660">has</span>
  <span m="4452930">asthma,</span> <span m="4453770">type</span> <span m="4454040">2</span>
  <span m="4454220">diabetes.</span> <span m="4456000">Social</span> <span m="4456500">history,</span>
  <span m="4457160">family</span> <span m="4457670">history.</span> <span m="4462890">These</span>
  <span m="4463070">are</span> <span m="4463260">of</span> <span m="4463330">the</span>
  <span m="4463400">physical</span> <span m="4463940">exam</span> <span m="4464330">results.</span>
  <span m="4467400">So</span> <span m="4467540">it's</span> <span m="4467690">giving</span>
  <span m="4468050">you</span> <span m="4468260">a</span> <span m="4468320">lot</span>
  <span m="4468620">of</span> <span m="4468740">information</span> <span m="4469760">about</span>
  <span m="4470690">the</span> <span m="4470840">person.</span> <span m="4471740">Description</span>
  <span m="4472400">of</span> <span m="4472550">the</span> <span m="4472670">wound</span>
  <span m="4473330">down</span> <span m="4473660">at</span> <span m="4473780">the</span>
  <span m="4473900">bottom.</span> <span m="4475250">Pertinent</span> <span m="4475820">lab</span>
  <span m="4476090">results.</span> <span m="4477030">So</span> <span m="4477140">these</span>
  <span m="4477410">are</span> <span m="4477530">copied</span> <span m="4478070">out</span>
  <span m="4478250">of</span> <span m="4478370">the</span> <span m="4478460">laboratory</span>
  <span m="4479090">tables.</span> <span m="4479750">Yeah.</span></p><p><span m="4479920">AUDIENCE:</span>
  <span m="4480167">Just to</span> <span m="4480415">double check with</span> <span
  m="4480910">the</span> <span m="4481405">drug results--</span></p><p><span m="4481900">PROFESSOR:</span>
  <span m="4482075">Sorry?</span></p><p><span m="4482510">AUDIENCE:</span> <span m="4482600">Just</span>
  <span m="4482690">to</span> <span m="4482780">double</span> <span m="4482990">check</span>
  <span m="4483380">with the drug</span> <span m="4483800">results two slides</span>
  <span m="4484010">back--</span></p><p><span m="4484930">PROFESSOR:</span> <span
  m="4485005">Yeah</span></p><p><span m="4485511">AUDIENCE:</span> <span m="4485654">It</span>
  <span m="4485797">said--</span> <span m="4488100">so</span> <span m="4488370">it</span>
  <span m="4488460">has</span> <span m="4488850">the</span> <span m="4489446">fake</span>
  <span m="4490220">dates</span> <span m="4491015">of</span> <span m="4491420">2190</span>
  <span m="4492050">up</span> <span m="4492480">there.</span></p><p><span m="4493050">PROFESSOR:</span>
  <span m="4493260">Yep.</span></p><p><span m="4493470">AUDIENCE:</span> <span m="4493545">So</span>
  <span m="4493620">the</span> <span m="4493740">fact</span> <span m="4494040">that</span>
  <span m="4494250">there</span> <span m="4494470">was</span> <span m="4494700">a</span>
  <span m="4495000">positive test</span> <span m="4495430">in</span> <span m="4495610">2187</span>
  <span m="4496345">would</span> <span m="4496610">mean</span> <span m="4497310">a</span>
  <span m="4497430">year</span> <span m="4497610">ago.</span></p><p><span m="4498260">PROFESSOR:</span>
  <span m="4498350">Yeah.</span></p><p><span m="4498440">AUDIENCE:</span> <span m="4498606">So</span>
  <span m="4498772">that's</span> <span m="4498940">the</span> <span m="4499106">medication.</span></p><p><span
  m="4500440">PROFESSOR:</span> <span m="4500595">Yeah,</span> <span m="4500750">the</span>
  <span m="4501070">deindenfication</span> <span m="4502340">technology</span> <span
  m="4503100">here</span> <span m="4503910">maintains</span> <span m="4504630">the</span>
  <span m="4504750">relative</span> <span m="4505380">dates</span> <span m="4505890">but</span>
  <span m="4506160">not</span> <span m="4506430">the</span> <span m="4506580">absolute</span>
  <span m="4507160">dates.</span> <span m="4514510">So</span> <span m="4514750">these</span>
  <span m="4515110">are</span> <span m="4515830">results,</span> <span m="4516490">again,</span>
  <span m="4516850">copied</span> <span m="4517450">out</span> <span m="4517690">of</span>
  <span m="4517900">the</span> <span m="4518140">laboratory</span> <span m="4518830">database</span>
  <span m="4520360">into</span> <span m="4520660">the</span> <span m="4520870">discharge</span>
  <span m="4521380">summary.</span> <span m="4522490">Brief</span> <span m="4522790">hospital</span>
  <span m="4523330">course,</span> <span m="4524830">and</span> <span m="4525010">then</span>
  <span m="4525520">a</span> <span m="4525640">review</span> <span m="4526060">of</span>
  <span m="4526180">systems,</span> <span m="4526820">so</span> <span m="4526960">what's</span>
  <span m="4527230">going</span> <span m="4527560">on</span> <span m="4527770">neurologically,</span>
  <span m="4528670">cardiovascular,</span> <span m="4529690">pulmonary,</span> <span
  m="4531210">GI,</span> <span m="4531850">GU,</span> <span m="4532210">et</span>
  <span m="4532520">cetera.</span></p><p><span m="4534130">Infectious</span> <span
  m="4534790">disease,</span> <span m="4535300">endocrine,</span> <span m="4535900">hematology,</span>
  <span m="4537280">prophylaxis.</span> <span m="4538930">And</span> <span m="4539290">at</span>
  <span m="4539470">the</span> <span m="4539590">time</span> <span m="4539890">was</span>
  <span m="4540010">discharged,</span> <span m="4540550">the</span> <span m="4540640">patient</span>
  <span m="4541090">was</span> <span m="4541300">doing</span> <span m="4541600">well,</span>
  <span m="4543010">no</span> <span m="4543220">fever</span> <span m="4543730">and</span>
  <span m="4543850">stable</span> <span m="4544300">vital</span> <span m="4544660">signs,</span>
  <span m="4545170">tolerating</span> <span m="4545800">a</span> <span m="4545860">regular</span>
  <span m="4546220">diet,</span> <span m="4546670">ambulating,</span> <span m="4547270">voiding</span>
  <span m="4547630">without</span> <span m="4547960">assistance,</span> <span m="4548560">and</span>
  <span m="4548650">pain</span> <span m="4548950">was</span> <span m="4549130">well</span>
  <span m="4549340">controlled.</span> <span m="4551980">Medications</span> <span
  m="4552850">on</span> <span m="4553000">admission,</span> <span m="4553780">so</span>
  <span m="4554020">this</span> <span m="4554260">was</span> <span m="4554470">the</span>
  <span m="4554560">medication</span> <span m="4555220">reconciliation.</span> <span
  m="4557280">Discharge</span> <span m="4557880">medication,</span> <span m="4558730">so</span>
  <span m="4558880">this</span> <span m="4559120">is</span> <span m="4559270">what</span>
  <span m="4559450">she's</span> <span m="4559720">being</span> <span m="4559990">sent</span>
  <span m="4560290">home</span> <span m="4560570">on.</span></p><p><span m="4561780">Discharge</span>
  <span m="4562400">disposition</span> <span m="4562960">is</span> <span m="4563380">to</span>
  <span m="4563530">the</span> <span m="4563650">home</span> <span m="4564490">with</span>
  <span m="4564760">some</span> <span m="4565840">follow</span> <span m="4566230">up</span>
  <span m="4566380">service,</span> <span m="4567970">and</span> <span m="4568810">she's</span>
  <span m="4569110">going</span> <span m="4570040">home.</span> <span m="4571630">And</span>
  <span m="4572890">the</span> <span m="4573010">discharge</span> <span m="4573580">diagnosis</span>
  <span m="4574420">is</span> <span m="4574840">infected</span> <span m="4575410">left</span>
  <span m="4575680">femoral</span> <span m="4576130">popliteal</span> <span m="4577150">bypass</span>
  <span m="4577690">graft</span> <span m="4579070">and</span> <span m="4579310">the</span>
  <span m="4579400">condition.</span> <span m="4580180">And</span> <span m="4580480">these</span>
  <span m="4580780">are</span> <span m="4580930">the</span> <span m="4581080">instructions</span>
  <span m="4581830">to</span> <span m="4581980">the</span> <span m="4582070">patient</span>
  <span m="4583090">that</span> <span m="4583330">say,</span> <span m="4584110">you
  know,</span> <span m="4584380">here's</span> <span m="4584680">what</span> <span
  m="4584890">you</span> <span m="4584980">can</span> <span m="4585190">do,</span>
  <span m="4585550">here</span> <span m="4585760">is</span> <span m="4585910">when</span>
  <span m="4586120">you</span> <span m="4586240">should</span> <span m="4586450">come</span>
  <span m="4586690">back</span> <span m="4586990">and</span> <span m="4587140">tell</span>
  <span m="4587440">us</span> <span m="4587650">if</span> <span m="4587740">something</span>
  <span m="4588160">is</span> <span m="4588310">going</span> <span m="4588610">wrong,</span>
  <span m="4588950">et</span> <span m="4589200">cetera.</span> <span m="4592330">And</span>
  <span m="4593080">here's</span> <span m="4593410">what</span> <span m="4593650">you</span>
  <span m="4593740">should</span> <span m="4593980">report</span> <span m="4594740">if</span>
  <span m="4595270">it</span> <span m="4595360">happens.</span></p><p><span m="4597340">You</span>
  <span m="4597460">know,</span> <span m="4597670">if</span> <span m="4597820">you</span>
  <span m="4597970">have</span> <span m="4598150">sudden</span> <span m="4598480">severe</span>
  <span m="4598900">bleeding</span> <span m="4599350">or</span> <span m="4599470">swelling,</span>
  <span m="4600040">do</span> <span m="4600220">this.</span> <span m="4601120">Follow</span>
  <span m="4601570">up</span> <span m="4601810">with</span> <span m="4602020">doctor</span>
  <span m="4602440">somebody</span> <span m="4602950">or</span> <span m="4603070">other.</span>
  <span m="4604060">Call</span> <span m="4604390">his</span> <span m="4604660">clinic</span>
  <span m="4605140">at</span> <span m="4605410">this</span> <span m="4605800">number</span>
  <span m="4606160">to</span> <span m="4606340">schedule</span> <span m="4606820">an</span>
  <span m="4606940">appointment</span> <span m="4609140">and</span> <span m="4609910">then</span>
  <span m="4610120">follow</span> <span m="4610540">up</span> <span m="4610750">with</span>
  <span m="4610990">doctor</span> <span m="4611380">somebody</span> <span m="4611860">else</span>
  <span m="4613000">in two</span> <span m="4613420">weeks.</span></p><p><span m="4619670">I</span>
  <span m="4619770">think</span> <span m="4619870">this</span> <span m="4620080">is</span>
  <span m="4620230">the</span> <span m="4620320">same</span> <span m="4620620">one.</span>
  <span m="4622040">So</span> <span m="4622330">just</span> <span m="4623200">a</span>
  <span m="4623290">couple</span> <span m="4623650">of</span> <span m="4623740">final</span>
  <span m="4624160">words</span> <span m="4624790">about</span> <span m="4625120">standards.</span>
  <span m="4626260">So</span> <span m="4626500">you</span> <span m="4626680">saw</span>
  <span m="4627250">in</span> <span m="4627550">David's</span> <span m="4628030">introductory</span>
  <span m="4628660">lecture</span> <span m="4629650">a</span> <span m="4629710">reference</span>
  <span m="4630250">to</span> <span m="4630400">Odyssey,</span> <span m="4631030">which</span>
  <span m="4631300">is</span> <span m="4631600">a</span> <span m="4631660">standard</span>
  <span m="4632170">method</span> <span m="4632620">of</span> <span m="4632740">encoding</span>
  <span m="4633790">the</span> <span m="4633910">kind</span> <span m="4634210">of</span>
  <span m="4634300">data</span> <span m="4634660">that</span> <span m="4634930">we're</span>
  <span m="4635440">talking</span> <span m="4635890">about</span> <span m="4636160">today.</span>
  <span m="4637640">There</span> <span m="4637800">is</span> <span m="4638020">a</span>
  <span m="4638140">likelihood</span> <span m="4639040">that</span> <span m="4639340">the</span>
  <span m="4639460">next</span> <span m="4639940">release</span> <span m="4640420">of</span>
  <span m="4640570">the</span> <span m="4640690">MIMIC</span> <span m="4641020">database</span>
  <span m="4642130">will</span> <span m="4642370">adopt</span> <span m="4642790">the</span>
  <span m="4642970">Odyssey</span> <span m="4643420">formats</span> <span m="4644080">rather</span>
  <span m="4644500">than</span> <span m="4644830">the--</span> <span m="4646620">yeah.</span>
  <span m="4647740">David's</span> <span m="4647980">shaking</span> <span m="4648460">his</span>
  <span m="4648640">head,</span> <span m="4649630">wondering</span> <span m="4650140">why.</span>
  <span m="4651300">Me,</span> <span m="4651480">too.</span></p><p><span m="4654430">AUDIENCE:</span>
  <span m="4654505">Odyssey</span> <span m="4654580">hasn't</span> <span m="4654700">handled</span>
  <span m="4655170">clinical</span> <span m="4655660">notes</span> <span m="4656480">very
  well yet.</span></p><p><span m="4657460">PROFESSOR:</span> <span m="4657625">Well,</span>
  <span m="4657790">so,</span> <span m="4658420">you</span> <span m="4658810">know,</span>
  <span m="4659230">what</span> <span m="4659470">always</span> <span m="4659890">happens,</span>
  <span m="4660430">as</span> <span m="4660610">you</span> <span m="4660730">say,</span>
  <span m="4660970">I'm</span> <span m="4661090">going</span> <span m="4661220">to</span>
  <span m="4661360">adopt</span> <span m="4661750">the</span> <span m="4661910">standard</span>
  <span m="4663010">asterisk</span> <span m="4664090">with</span> <span m="4664360">the</span>
  <span m="4664450">following</span> <span m="4665020">extensions.</span> <span m="4666460">And</span>
  <span m="4666580">that's</span> <span m="4666820">probably</span> <span m="4667210">what's</span>
  <span m="4667420">going</span> <span m="4667540">to</span> <span m="4667630">happen.</span>
  <span m="4668470">But</span> <span m="4668680">it</span> <span m="4668800">means</span>
  <span m="4669160">that</span> <span m="4669400">the</span> <span m="4670330">central</span>
  <span m="4670810">tables,</span> <span m="4671860">you</span> <span m="4671980">know,</span>
  <span m="4672160">the</span> <span m="4672340">ICD-9</span> <span m="4673090">code</span>
  <span m="4673390">tables</span> <span m="4674050">and</span> <span m="4674200">the</span>
  <span m="4674590">drug</span> <span m="4674860">tables,</span> <span m="4675340">some</span>
  <span m="4675550">things</span> <span m="4675820">like</span> <span m="4676030">that,</span>
  <span m="4676780">are</span> <span m="4676900">likely</span> <span m="4677380">to</span>
  <span m="4677530">wind</span> <span m="4677860">up</span> <span m="4678040">adopting</span>
  <span m="4678550">the</span> <span m="4678670">formats</span> <span m="4679270">of</span>
  <span m="4679690">the</span> <span m="4679810">Odyssey</span> <span m="4680830">database.</span></p><p><span
  m="4683260">You</span> <span m="4683410">should</span> <span m="4683620">also</span>
  <span m="4683980">know</span> <span m="4684190">about</span> <span m="4684490">this</span>
  <span m="4684700">thing</span> <span m="4684940">called</span> <span m="4685210">FHIR,</span>
  <span m="4686950">F-H-I-R,</span> <span m="4687850">the</span> <span m="4687970">Fast</span>
  <span m="4688720">Health</span> <span m="4689110">Interoperability</span> <span
  m="4690280">Resources.</span> <span m="4691720">So</span> <span m="4692560">HL7</span>
  <span m="4693370">is</span> <span m="4693520">the</span> <span m="4693670">standards</span>
  <span m="4694300">organization</span> <span m="4695950">that</span> <span m="4697090">had</span>
  <span m="4697390">a</span> <span m="4697450">tremendous</span> <span m="4698020">success</span>
  <span m="4698800">in</span> <span m="4698980">the</span> <span m="4699100">early</span>
  <span m="4699370">1990s</span> <span m="4701110">in</span> <span m="4701320">solving</span>
  <span m="4701830">the</span> <span m="4701920">problem</span> <span m="4702460">of</span>
  <span m="4702610">how</span> <span m="4702790">to</span> <span m="4702940">allow</span>
  <span m="4703270">laboratories</span> <span m="4704080">to</span> <span m="4704260">report</span>
  <span m="4704740">lab</span> <span m="4705010">data</span> <span m="4705820">back</span>
  <span m="4706120">to</span> <span m="4706270">the</span> <span m="4706360">hospitals</span>
  <span m="4707020">or</span> <span m="4707140">the</span> <span m="4707260">clinics</span>
  <span m="4707770">that</span> <span m="4707950">ordered</span> <span m="4708310">the</span>
  <span m="4708430">labs.</span> <span m="4709990">And</span> <span m="4710170">that</span>
  <span m="4710920">character</span> <span m="4711460">string</span> <span m="4711970">with</span>
  <span m="4712270">the</span> <span m="4713110">up</span> <span m="4713320">arrows</span>
  <span m="4713860">and</span> <span m="4713980">the</span> <span m="4714190">vertical</span>
  <span m="4714700">bars</span> <span m="4715150">and</span> <span m="4715270">so</span>
  <span m="4715540">on</span> <span m="4715720">that</span> <span m="4715870">I</span>
  <span m="4715990">showed</span> <span m="4716320">you</span> <span m="4716470">before</span>
  <span m="4717610">that</span> <span m="4717790">had</span> <span m="4718000">LOINK</span>
  <span m="4718540">encoded</span> <span m="4719110">in</span> <span m="4719260">it</span>
  <span m="4719950">is</span> <span m="4720220">that</span> <span m="4720520">standard.</span>
  <span m="4721210">That's</span> <span m="4721510">called</span> <span m="4721810">HL7</span>
  <span m="4722560">Version</span> <span m="4723010">2.</span></p><p><span m="4724090">It's</span>
  <span m="4724270">still</span> <span m="4724570">in</span> <span m="4724720">use</span>
  <span m="4725050">very</span> <span m="4725320">widely,</span> <span m="4726700">they</span>
  <span m="4726910">then</span> <span m="4727150">got</span> <span m="4727570">ambitious</span>
  <span m="4728440">and</span> <span m="4728590">suffered</span> <span m="4729190">second</span>
  <span m="4729610">system</span> <span m="4730090">syndrome,</span> <span m="4731390">which</span>
  <span m="4731590">is</span> <span m="4731800">they</span> <span m="4731980">decided</span>
  <span m="4732490">to</span> <span m="4732640">build</span> <span m="4733030">HL7</span>
  <span m="4733360">Version</span> <span m="4734260">3,</span> <span m="4735440">which</span>
  <span m="4735670">I</span> <span m="4735790">used</span> <span m="4736060">to</span>
  <span m="4736180">teach</span> <span m="4736570">in</span> <span m="4736690">a</span>
  <span m="4736750">class</span> <span m="4737710">here</span> <span m="4737980">10</span>
  <span m="4738280">years</span> <span m="4738580">ago.</span> <span m="4739390">But</span>
  <span m="4741220">one</span> <span m="4741490">of</span> <span m="4741550">my</span>
  <span m="4741730">friends</span> <span m="4742180">who</span> <span m="4742300">works</span>
  <span m="4742720">for</span> <span m="4742930">a</span> <span m="4742990">company</span>
  <span m="4743500">that</span> <span m="4743740">helps</span> <span m="4744040">hospitals</span>
  <span m="4744700">implement</span> <span m="4745210">that</span> <span m="4745960">sent</span>
  <span m="4746350">me</span> <span m="4747550">a</span> <span m="4747610">38</span>
  <span m="4748330">megabyte</span> <span m="4749050">PDF</span> <span m="4749530">file</span>
  <span m="4750640">that</span> <span m="4750940">describes</span> <span m="4751840">what</span>
  <span m="4752110">you</span> <span m="4752200">need</span> <span m="4752470">to</span>
  <span m="4752620">know</span> <span m="4752950">in</span> <span m="4753100">order</span>
  <span m="4753370">to</span> <span m="4753490">implement</span> <span m="4754060">that</span>
  <span m="4754300">system.</span> <span m="4755480">And</span> <span m="4755530">as</span>
  <span m="4755710">a</span> <span m="4755770">result,</span> <span m="4756190">nobody</span>
  <span m="4756610">was</span> <span m="4756760">doing</span> <span m="4757060">it.</span></p><p><span
  m="4758440">So</span> <span m="4759190">FHIR</span> <span m="4759880">is</span>
  <span m="4760120">a</span> <span m="4760390">gross</span> <span m="4760780">simplification</span>
  <span m="4761800">of</span> <span m="4761920">that</span> <span m="4762850">that</span>
  <span m="4763030">starts</span> <span m="4763510">off</span> <span m="4763810">and</span>
  <span m="4763930">says,</span> <span m="4764500">if</span> <span m="4764980">a</span>
  <span m="4765040">doctor</span> <span m="4765520">refers</span> <span m="4766180">a</span>
  <span m="4766270">new</span> <span m="4766510">patient</span> <span m="4766990">to</span>
  <span m="4767230">you,</span> <span m="4768460">what</span> <span m="4768670">is</span>
  <span m="4768820">the</span> <span m="4768940">minimum</span> <span m="4769420">set</span>
  <span m="4769690">of</span> <span m="4769810">data</span> <span m="4770170">that</span>
  <span m="4770410">you</span> <span m="4770530">need</span> <span m="4770740">to</span>
  <span m="4770890">know</span> <span m="4771520">in</span> <span m="4771700">order</span>
  <span m="4771970">to</span> <span m="4772150">take</span> <span m="4772360">care</span>
  <span m="4772600">of</span> <span m="4772720">that</span> <span m="4772900">person?</span>
  <span m="4773950">And</span> <span m="4774100">FHIR</span> <span m="4774580">tries</span>
  <span m="4775030">to</span> <span m="4775180">provide</span> <span m="4775870">just</span>
  <span m="4776260">that</span> <span m="4776590">subset</span> <span m="4777400">of</span>
  <span m="4777580">all</span> <span m="4777730">of</span> <span m="4777790">the</span>
  <span m="4777880">data.</span> <span m="4779620">It</span> <span m="4779770">has</span>
  <span m="4780040">become</span> <span m="4780460">a</span> <span m="4780520">standard</span>
  <span m="4781150">mainly</span> <span m="4781600">because,</span> <span m="4782560">after</span>
  <span m="4782950">Congress</span> <span m="4783370">spent</span> <span m="4783730">$42</span>
  <span m="4784240">billion</span> <span m="4784630">dollars</span> <span m="4785110">or</span>
  <span m="4785230">so</span> <span m="4786160">bribing</span> <span m="4786640">people</span>
  <span m="4787060">into</span> <span m="4787330">buying</span> <span m="4787690">these</span>
  <span m="4787930">information</span> <span m="4788560">systems,</span> <span m="4789520">they</span>
  <span m="4789730">got</span> <span m="4789970">mad</span> <span m="4790330">that</span>
  <span m="4790570">the</span> <span m="4790690">information</span> <span m="4791350">systems</span>
  <span m="4791860">they</span> <span m="4792040">bought</span> <span m="4792700">couldn't</span>
  <span m="4793000">talk</span> <span m="4793300">to</span> <span m="4793450">each</span>
  <span m="4793660">other.</span></p><p><span m="4794590">And</span> <span m="4794770">so</span>
  <span m="4794980">they</span> <span m="4795160">called</span> <span m="4795610">in,</span>
  <span m="4795970">on</span> <span m="4796150">the</span> <span m="4796270">carpet,</span>
  <span m="4796840">the</span> <span m="4796990">heads</span> <span m="4797350">of</span>
  <span m="4797500">these</span> <span m="4798520">IT</span> <span m="4798880">companies,</span>
  <span m="4799480">health</span> <span m="4799780">IT</span> <span m="4800080">companies,</span>
  <span m="4801280">and</span> <span m="4801460">they</span> <span m="4801580">yelled</span>
  <span m="4801910">at</span> <span m="4802080">them</span> <span m="4802360">and</span>
  <span m="4802480">they</span> <span m="4802630">made</span> <span m="4802900">them</span>
  <span m="4803050">promise</span> <span m="4803620">that</span> <span m="4803830">there</span>
  <span m="4804010">would</span> <span m="4804220">be</span> <span m="4804400">interoperability.</span>
  <span m="4806260">They</span> <span m="4806440">promised.</span> <span m="4807220">And</span>
  <span m="4807400">out</span> <span m="4807670">of</span> <span m="4807820">that</span>
  <span m="4808120">came</span> <span m="4808420">FHIR.</span> <span m="4809800">It</span>
  <span m="4809920">was</span> <span m="4810130">probably</span> <span m="4810670">simultaneously</span>
  <span m="4812050">developed</span> <span m="4812530">but</span> <span m="4812680">they</span>
  <span m="4812890">adopted</span> <span m="4813430">it.</span> <span m="4814210">And</span>
  <span m="4814390">so</span> <span m="4814630">now,</span> <span m="4815590">in</span>
  <span m="4815740">principle,</span> <span m="4816610">it's</span> <span m="4816850">possible</span>
  <span m="4817450">to</span> <span m="4817660">exchange</span> <span m="4818260">data</span>
  <span m="4818650">between</span> <span m="4819100">different</span> <span m="4819460">hospitals,</span>
  <span m="4820570">at</span> <span m="4820720">least</span> <span m="4821020">to</span>
  <span m="4821170">the</span> <span m="4821320">level</span> <span m="4821860">of</span>
  <span m="4822070">that</span> <span m="4822340">degree</span> <span m="4822910">of</span>
  <span m="4823540">harmonization</span> <span m="4824710">of</span> <span m="4824890">the</span>
  <span m="4825010">data.</span></p><p><span m="4826180">In</span> <span m="4826330">reality,</span>
  <span m="4827470">the</span> <span m="4827740">companies</span> <span m="4828400">don't</span>
  <span m="4828730">want</span> <span m="4829070">you</span> <span m="4829170">to</span>
  <span m="4829360">do</span> <span m="4829570">that</span> <span m="4830080">because</span>
  <span m="4830980">they</span> <span m="4831190">like</span> <span m="4831550">there</span>
  <span m="4831790">to</span> <span m="4831970">be</span> <span m="4832150">friction</span>
  <span m="4833200">in</span> <span m="4833380">not</span> <span m="4833650">being</span>
  <span m="4833950">able</span> <span m="4834220">to</span> <span m="4834370">take</span>
  <span m="4834700">all</span> <span m="4834850">your</span> <span m="4835030">data</span>
  <span m="4835390">to</span> <span m="4835600">a</span> <span m="4835660">different</span>
  <span m="4836050">hospital,</span> <span m="4836710">because</span> <span m="4836950">it</span>
  <span m="4837520">is</span> <span m="4837670">more</span> <span m="4837910">likely</span>
  <span m="4838360">to</span> <span m="4838480">leave</span> <span m="4838780">you</span>
  <span m="4839170">at</span> <span m="4839350">the</span> <span m="4839470">one</span>
  <span m="4839710">that</span> <span m="4839920">you're</span> <span m="4840070">at.</span>
  <span m="4841450">So</span> <span m="4841720">there</span> <span m="4841830">is</span>
  <span m="4842110">complicated</span> <span m="4843340">socioeconomic</span> <span
  m="4844600">kinds</span> <span m="4844960">of</span> <span m="4845080">issues</span>
  <span m="4845650">in</span> <span m="4845800">all</span> <span m="4845980">this.</span>
  <span m="4846700">But</span> <span m="4846910">at</span> <span m="4847030">least</span>
  <span m="4847300">the</span> <span m="4847420">standard</span> <span m="4847990">exists</span>
  <span m="4848620">and</span> <span m="4848710">is</span> <span m="4848890">becoming</span>
  <span m="4849400">more</span> <span m="4849670">and</span> <span m="4849760">more</span>
  <span m="4850000">widely</span> <span m="4850960">deployed</span> <span m="4851500">as</span>
  <span m="4851650">long</span> <span m="4851920">as</span> <span m="4852040">Congress</span>
  <span m="4852520">pays</span> <span m="4852820">attention.</span></p><p><span m="4853810">It's</span>
  <span m="4854080">ugly.</span> <span m="4854860">So</span> <span m="4855100">here</span>
  <span m="4855410">is</span> <span m="4855490">what</span> <span m="4855700">a</span>
  <span m="4855760">patient</span> <span m="4856300">looks</span> <span m="4856540">like,</span>
  <span m="4857680">right?</span> <span m="4858100">It's</span> <span m="4858340">the</span>
  <span m="4858490">usual</span> <span m="4859180">unreadable</span> <span m="4860000">XML</span>
  <span m="4860470">garbage.</span> <span m="4861790">But</span> <span m="4862210">fortunately,</span>
  <span m="4863020">there</span> <span m="4863230">are</span> <span m="4863320">parsers</span>
  <span m="4863980">that</span> <span m="4864160">can</span> <span m="4864370">turn</span>
  <span m="4864670">it</span> <span m="4864790">into</span> <span m="4865060">JSON</span>
  <span m="4865660">and</span> <span m="4866350">simpler</span> <span m="4867100">representations.</span>
  <span m="4868340">And</span> <span m="4868360">so</span> <span m="4868570">that's</span>
  <span m="4869140">pretty</span> <span m="4869380">common.</span></p><p><span m="4871370">So</span>
  <span m="4871510">the</span> <span m="4871630">terminologies</span> <span m="4873220">that</span>
  <span m="4873460">exist</span> <span m="4874090">are</span> <span m="4874260">LOINK,</span>
  <span m="4875080">NBC,</span> <span m="4875860">ICD-9</span> <span m="4876700">and</span>
  <span m="4876820">10.</span> <span m="4877660">SNOMED</span> <span m="4878260">I</span>
  <span m="4878350">didn't</span> <span m="4878560">talk</span> <span m="4878890">about</span>
  <span m="4879160">today.</span> <span m="4879520">DSM-5</span> <span m="4881020">is</span>
  <span m="4881290">the</span> <span m="4881590">Diagnostic</span> <span m="4882340">and</span>
  <span m="4882460">Statistical</span> <span m="4883210">Manual</span> <span m="4883870">for</span>
  <span m="4884230">Psychiatrists.</span> <span m="4885850">That's</span> <span m="4886150">used</span>
  <span m="4886510">as</span> <span m="4886690">a</span> <span m="4886750">common</span>
  <span m="4887170">coding</span> <span m="4887770">method</span> <span m="4888220">for</span>
  <span m="4889360">describing</span> <span m="4890470">psychiatric</span> <span m="4891220">disease.</span>
  <span m="4891730">And</span> <span m="4891850">there</span> <span m="4892000">are</span>
  <span m="4892030">many</span> <span m="4892300">more</span> <span m="4892570">of</span>
  <span m="4892690">these.</span></p><p><span m="4893800">There's</span> <span m="4894010">something</span>
  <span m="4894400">called</span> <span m="4894700">the</span> <span m="4895360">Unified</span>
  <span m="4895900">Medical</span> <span m="4896290">Language</span> <span m="4896740">Systems</span>
  <span m="4897280">Metathesaurus</span> <span m="4898750">from</span> <span m="4899020">the</span>
  <span m="4899110">National</span> <span m="4899500">Library</span> <span m="4899890">of</span>
  <span m="4899980">Medicine</span> <span m="4901060">that</span> <span m="4902140">integrates</span>
  <span m="4903040">about</span> <span m="4904290">180</span> <span m="4905230">of</span>
  <span m="4905380">these</span> <span m="4905680">different</span> <span m="4906130">terminologies.</span>
  <span m="4907660">And</span> <span m="4907810">so</span> <span m="4908050">there</span>
  <span m="4908260">is</span> <span m="4909040">a</span> <span m="4909130">nice</span>
  <span m="4910810">one-stop</span> <span m="4911800">shop</span> <span m="4912400">where</span>
  <span m="4912670">you</span> <span m="4912820">can</span> <span m="4913060">get</span>
  <span m="4913270">all</span> <span m="4913460">these</span> <span m="4913690">things</span>
  <span m="4914920">from</span> <span m="4915250">them.</span></p><p><span m="4919670">So</span>
  <span m="4919910">takeaway</span> <span m="4920450">lessons,</span> <span m="4921520">know</span>
  <span m="4921770">your</span> <span m="4921950">data.</span> <span m="4922860">Remember</span>
  <span m="4923240">that</span> <span m="4923450">first</span> <span m="4923840">example</span>
  <span m="4924410">of</span> <span m="4924530">the</span> <span m="4924620">heart</span>
  <span m="4924890">rates,</span> <span m="4925850">that</span> <span m="4926060">comes</span>
  <span m="4926360">up</span> <span m="4926600">over</span> <span m="4926870">and</span>
  <span m="4927020">over</span> <span m="4927350">again.</span> <span m="4928010">And</span>
  <span m="4928430">doing</span> <span m="4929420">machine</span> <span m="4929840">learning</span>
  <span m="4930440">and</span> <span m="4930620">analysis</span> <span m="4931460">on</span>
  <span m="4931760">data</span> <span m="4932150">that</span> <span m="4932390">you</span>
  <span m="4932480">don't</span> <span m="4932720">understand</span> <span m="4933860">is</span>
  <span m="4934070">likely</span> <span m="4934520">to</span> <span m="4934670">lead</span>
  <span m="4934970">you</span> <span m="4935270">to</span> <span m="4935510">false</span>
  <span m="4935870">conclusions.</span></p><p><span m="4938480">Harmonization</span>
  <span m="4939320">is</span> <span m="4939500">difficult</span> <span m="4940070">and</span>
  <span m="4940190">time</span> <span m="4940490">consuming.</span> <span m="4941150">And</span>
  <span m="4941270">there</span> <span m="4941420">are</span> <span m="4941480">lots</span>
  <span m="4941810">of</span> <span m="4941930">things</span> <span m="4942290">for</span>
  <span m="4942470">which</span> <span m="4942710">we</span> <span m="4942860">just</span>
  <span m="4943070">don't</span> <span m="4943310">have</span> <span m="4943520">standards,</span>
  <span m="4944600">and</span> <span m="4944720">so</span> <span m="4944930">everybody</span>
  <span m="4945410">develops</span> <span m="4945920">their</span> <span m="4946130">own</span>
  <span m="4946280">representations.</span> <span m="4947930">I</span> <span m="4948320">had</span>
  <span m="4948620">a</span> <span m="4949040">PhD</span> <span m="4949580">student</span>
  <span m="4950120">about</span> <span m="4950420">a</span> <span m="4950480">decade</span>
  <span m="4950870">ago</span> <span m="4951740">who,</span> <span m="4951950">in</span>
  <span m="4952100">his</span> <span m="4952310">thesis,</span> <span m="4953270">wrote</span>
  <span m="4953660">that</span> <span m="4953870">he</span> <span m="4953930">spent</span>
  <span m="4954320">about</span> <span m="4954590">half</span> <span m="4954860">his</span>
  <span m="4955040">time</span> <span m="4955550">cleaning</span> <span m="4955910">data.</span>
  <span m="4957620">And</span> <span m="4957800">I</span> <span m="4957920">gave</span>
  <span m="4958190">that</span> <span m="4958370">thesis</span> <span m="4958880">to</span>
  <span m="4959690">another</span> <span m="4960050">student</span> <span m="4960650">who</span>
  <span m="4960800">started</span> <span m="4961250">a</span> <span m="4961310">few</span>
  <span m="4961550">years</span> <span m="4961790">later</span> <span m="4962470">who</span>
  <span m="4962690">read</span> <span m="4962990">it,</span> <span m="4963270">and
  he</span> <span m="4963350">comes</span> <span m="4963680">to</span> <span m="4963800">me</span>
  <span m="4964790">just</span> <span m="4965120">awestruck</span> <span m="4966170">and</span>
  <span m="4966380">he</span> <span m="4966500">says,</span> <span m="4966890">what?</span>
  <span m="4967280">He</span> <span m="4967550">only</span> <span m="4967850">spent</span>
  <span m="4968240">half</span> <span m="4968540">his</span> <span m="4968720">time</span>
  <span m="4968990">cleaning?</span></p><p><span m="4971900">Unfortunately,</span>
  <span m="4973310">that's</span> <span m="4973610">roughly</span> <span m="4974090">where</span>
  <span m="4974270">we</span> <span m="4974480">are</span> <span m="4974900">in</span>
  <span m="4975050">this</span> <span m="4975260">field.</span> <span m="4975830">So</span>
  <span m="4976820">sorry</span> <span m="4977210">to</span> <span m="4977360">be</span>
  <span m="4977540">a</span> <span m="4977600">downer,</span> <span m="4978110">but</span>
  <span m="4978320">that's</span> <span m="4978980">the</span> <span m="4979100">current</span>
  <span m="4979460">state</span> <span m="4979760">of</span> <span m="4979880">the</span>
  <span m="4980030">art.</span> <span m="4981050">And</span> <span m="4981210">next</span>
  <span m="4981470">time,</span> <span m="4981710">David</span> <span m="4982070">will</span>
  <span m="4982250">start</span> <span m="4982700">by</span> <span m="4983150">looking</span>
  <span m="4983600">at</span> <span m="4984020">actually</span> <span m="4984470">building</span>
  <span m="4984890">some</span> <span m="4985130">models</span> <span m="4986060">with</span>
  <span m="4986690">these</span> <span m="4986990">kinds</span> <span m="4987410">of</span>
  <span m="4987530">data</span> <span m="4988370">and</span> <span m="4988970">showing</span>
  <span m="4989360">you</span> <span m="4989450">what</span> <span m="4990020">we</span>
  <span m="4990140">can</span> <span m="4990410">accomplish.</span> <span m="4991580">Thank</span>
  <span m="4991820">you.</span></p>
type: course
uid: 6418339f00fd3ae0b9d063f65ba1df17

---
None