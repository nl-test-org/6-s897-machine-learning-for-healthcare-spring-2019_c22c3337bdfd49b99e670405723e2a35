---
about_this_resource_text: '<p>Dr. Johansson covers an overview of treatment policies
  and potential outcomes, an introduction to reinforcement learning, decision processes,
  reinforcement learning paradigms, and learning from off-policy data.</p> <p>Speaker:&nbsp;Fredrik
  D. Johansson</p>             <p><a href="./resolveuid/05cad3aca76d2c2da9fcdf91e2048b0f">Lecture
  16: Reinforcement Learning slides (PDF)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: YZ5pOgY5hEE
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: Video-YouTube-Stream
  type: Video
  uid: 9a28549dc1bb1693978dbe2f44571489
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/YZ5pOgY5hEE/default.jpg
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: f8893986b876e03dd361ea44240e445d
- id: 3Play-3PlayYouTubeid-MP4
  media_location: YZ5pOgY5hEE
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: fdf1bc6ae5cfa94bab80475e57078085
- id: YZ5pOgY5hEE.srt
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-16-reinforcement-learning-part-1/YZ5pOgY5hEE.srt
  title: 3play caption file
  type: null
  uid: 39dbf9181de074afd699923d4a132933
- id: YZ5pOgY5hEE.pdf
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-16-reinforcement-learning-part-1/YZ5pOgY5hEE.pdf
  title: 3play pdf file
  type: null
  uid: 4eafbb01d0dbd32fd69e15914ac96885
- id: Caption-3Play YouTube id-SRT
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 172a612475b57e87aaac12d28332cf96
- id: Transcript-3Play YouTube id-PDF
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 87fa5a60f43e60ed2c5e6d1681557b89
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec16_300k.mp4
  parent_uid: a36d0da4a9b40aa41d0825258394995e
  title: Video-Internet Archive-MP4
  type: Video
  uid: 725edfd53a8c97aace9f9c787920b62f
inline_embed_id: 44845698lecture16reinforcementlearningpart183875690
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-16-reinforcement-learning-part-1
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-16-reinforcement-learning-part-1
template_type: Tabbed
title: 'Lecture 16: Reinforcement Learning, Part 1'
transcript: <p><span m="15950">PROFESSOR:</span> <span m="16020">Hi,</span> <span
  m="16090">everyone.</span> <span m="16520">We're</span> <span m="16620">getting</span>
  <span m="16860">started now.</span> <span m="18930">So</span> <span m="19260">this</span>
  <span m="19560">week's</span> <span m="19830">lecture</span> <span m="20280">is</span>
  <span m="20630">really picking</span> <span m="20930">up</span> <span m="21150">where</span>
  <span m="21480">last</span> <span m="21870">week's</span> <span m="22100">left</span>
  <span m="22410">off.</span> <span m="23320">You</span> <span m="23410">may</span>
  <span m="23580">remember</span> <span m="23820">we</span> <span m="23910">spent</span>
  <span m="24270">the</span> <span m="24330">last</span> <span m="24570">week</span>
  <span m="24720">talking</span> <span m="25020">about</span> <span m="25200">cause</span>
  <span m="25650">inference.</span> <span m="26430">And</span> <span m="26550">I</span>
  <span m="26610">told</span> <span m="26820">you</span> <span m="26940">how,</span>
  <span m="27270">for</span> <span m="27720">last</span> <span m="28140">week,</span>
  <span m="28440">we're</span> <span m="28590">going</span> <span m="28710">to</span>
  <span m="28950">focus</span> <span m="29250">on</span> <span m="29340">a</span>
  <span m="29430">one-time</span> <span m="30150">setting.</span></p><p><span m="31590">Well,</span>
  <span m="32159">as</span> <span m="32369">we</span> <span m="32520">know,</span>
  <span m="33630">lots</span> <span m="33960">of</span> <span m="34050">medicine</span>
  <span m="34380">has</span> <span m="34530">to</span> <span m="34590">do</span> <span
  m="34680">with</span> <span m="34830">multiple</span> <span m="35580">sequential</span>
  <span m="36090">decisions</span> <span m="36510">across</span> <span m="36800">time.</span>
  <span m="37590">And</span> <span m="37710">that'll</span> <span m="37860">be the</span>
  <span m="38040">focus</span> <span m="38490">of</span> <span m="38610">this</span>
  <span m="38880">whole</span> <span m="39150">week's</span> <span m="39480">worth</span>
  <span m="39780">of</span> <span m="40050">discussions.</span> <span m="41210">And</span>
  <span m="41340">as</span> <span m="41490">I</span> <span m="41550">thought</span>
  <span m="41790">about</span> <span m="42300">really</span> <span m="43740">what</span>
  <span m="43980">should</span> <span m="44160">I</span> <span m="44280">teach</span>
  <span m="44550">in</span> <span m="44640">this</span> <span m="44790">lecture,</span>
  <span m="45180">I</span> <span m="45300">realized</span> <span m="45750">that</span>
  <span m="45880">the</span> <span m="45960">person</span> <span m="46380">who</span>
  <span m="46500">knew</span> <span m="46740">the</span> <span m="46860">most</span>
  <span m="47370">about</span> <span m="47610">the</span> <span m="47700">topic</span>
  <span m="48630">was</span> <span m="48750">in</span> <span m="48810">fact</span>
  <span m="49050">a</span> <span m="49080">postdoctoral</span> <span m="49590">researcher</span>
  <span m="49950">in</span> <span m="50040">my</span> <span m="50130">lab.</span>
  <span m="52200">Most</span> <span m="52470">about</span> <span m="52620">this</span>
  <span m="52740">topic</span> <span m="53180">in</span> <span m="53320">the</span>
  <span m="53805">general</span> <span m="54290">area</span> <span m="54775">of</span>
  <span m="55260">the medical field.</span></p><p><span m="55745">FREDRIK D. JOHANSSON:</span>
  <span m="55987">Thanks.</span> <span m="56230">I'll</span> <span m="56720">take</span>
  <span m="56960">it.</span></p><p><span m="59260">AUDIENCE:</span> <span m="59495">Global</span>
  <span m="59730">[INAUDIBLE].</span></p><p><span m="59940">FREDRIK D. JOHANSSON:</span>
  <span m="60045">It's</span> <span m="60150">very</span> <span m="60510">fair.</span></p><p><span
  m="63240">PROFESSOR:</span> <span m="63335">And</span> <span m="63430">so</span>
  <span m="63810">I</span> <span m="64140">invited</span> <span m="64500">him</span>
  <span m="65319">to</span> <span m="65730">come to us</span> <span m="66330">today</span>
  <span m="66760">and</span> <span m="67120">to</span> <span m="67230">give</span>
  <span m="67410">this</span> <span m="67740">as</span> <span m="67890">an</span>
  <span m="67980">invited</span> <span m="68310">lecture.</span> <span m="69150">And</span>
  <span m="69510">this</span> <span m="69660">is</span> <span m="69780">Fredrik</span>
  <span m="70050">Johansson.</span> <span m="71150">He'll</span> <span m="71280">be</span>
  <span m="71430">a</span> <span m="71520">professor</span> <span m="72270">in</span>
  <span m="72870">Chalmers,</span> <span m="73380">in</span> <span m="73530">Sweden,</span>
  <span m="73890">starting</span> <span m="74250">in</span> <span m="74310">September.</span></p><p><span
  m="75540">FREDRIK D. JOHANSSON:</span> <span m="75615">Thank</span> <span m="75690">you</span>
  <span m="75810">so</span> <span m="75960">much,</span> <span m="76200">David.</span>
  <span m="76430">That's</span> <span m="76560">very</span> <span m="76800">generous.</span>
  <span m="78470">Yeah,</span> <span m="78870">so</span> <span m="79440">as</span>
  <span m="79560">David</span> <span m="79770">mentioned,</span> <span m="80100">last</span>
  <span m="80340">time</span> <span m="80610">we</span> <span m="80760">looked</span>
  <span m="81000">a</span> <span m="81050">lot</span> <span m="81330">at</span> <span
  m="81520">causal</span> <span m="81870">effects.</span> <span m="82410">And</span>
  <span m="84030">that's</span> <span m="84300">where</span> <span m="84480">we will</span>
  <span m="84810">start</span> <span m="85620">on</span> <span m="86010">this</span>
  <span m="86190">discussion,</span> <span m="86580">too.</span></p><p><span m="87570">So</span>
  <span m="87660">I'll</span> <span m="87720">just</span> <span m="87870">start</span>
  <span m="88050">with</span> <span m="88140">this</span> <span m="88260">reminder,</span>
  <span m="88650">here--</span> <span m="88860">we</span> <span m="89320">essentially</span>
  <span m="89670">introduced</span> <span m="90060">four</span> <span m="90270">quantities</span>
  <span m="90810">last</span> <span m="91140">time,</span> <span m="91500">or</span>
  <span m="91620">the</span> <span m="91710">last</span> <span m="91950">two</span>
  <span m="93360">lectures,</span> <span m="93750">as</span> <span m="94140">far</span>
  <span m="94260">as</span> <span m="94350">I</span> <span m="94410">know.</span>
  <span m="95340">We</span> <span m="95490">had</span> <span m="95610">two</span>
  <span m="95760">potential</span> <span m="96150">outcomes,</span> <span m="96720">which</span>
  <span m="97020">represented</span> <span m="97530">the</span> <span m="98280">outcomes</span>
  <span m="98580">that</span> <span m="98670">we</span> <span m="98790">would</span>
  <span m="98940">see</span> <span m="99360">of</span> <span m="99540">some</span>
  <span m="100440">treatment</span> <span m="100800">choice</span> <span m="101670">under</span>
  <span m="102090">the</span> <span m="102240">various</span> <span m="102840">choices.</span>
  <span m="103210">So,</span> <span m="103320">the</span> <span m="103410">two</span>
  <span m="103560">different</span> <span m="103800">choices--</span> <span m="104480">1</span>
  <span m="104750">and</span> <span m="104870">0.</span></p><p><span m="107580">We</span>
  <span m="107760">had</span> <span m="107790">a</span> <span m="108710">set</span>
  <span m="108860">of</span> <span m="108930">covariates,</span> <span m="109500">x</span>
  <span m="109890">and</span> <span m="110220">a</span> <span m="110310">treatment,</span>
  <span m="110610">t.</span> <span m="111840">And</span> <span m="112050">we</span>
  <span m="112170">were</span> <span m="112290">interested</span> <span m="112650">in,</span>
  <span m="112710">essentially,</span> <span m="113040">what</span> <span m="113190">is</span>
  <span m="113280">the</span> <span m="113370">effect</span> <span m="113640">of</span>
  <span m="113700">this</span> <span m="113880">treatment,</span> <span m="114270">t,</span>
  <span m="114600">on</span> <span m="114840">the</span> <span m="114990">outcome,</span>
  <span m="115350">y,</span> <span m="116190">given</span> <span m="116490">the</span>
  <span m="116580">covariates,</span> <span m="117240">x.</span> <span m="118320">And</span>
  <span m="118800">the</span> <span m="118950">effect</span> <span m="119850">that</span>
  <span m="119970">we</span> <span m="120090">focused</span> <span m="120780">on</span>
  <span m="121050">that</span> <span m="121230">time</span> <span m="121500">was</span>
  <span m="121730">the</span> <span m="121860">conditional</span> <span m="122280">average</span>
  <span m="122580">treatment</span> <span m="122910">effect,</span> <span m="123600">which</span>
  <span m="123810">is</span> <span m="124020">exactly</span> <span m="124470">the</span>
  <span m="124560">difference</span> <span m="124920">between</span> <span m="125220">these</span>
  <span m="125400">potential</span> <span m="125880">outcomes--</span> <span m="126870">a</span>
  <span m="127200">condition</span> <span m="127630">on</span> <span m="127740">the</span>
  <span m="127800">features.</span></p><p><span m="129030">So</span> <span m="129210">the</span>
  <span m="129300">whole</span> <span m="130050">last</span> <span m="130350">week</span>
  <span m="130530">was</span> <span m="130650">about</span> <span m="130949">trying</span>
  <span m="131190">to</span> <span m="131280">identify</span> <span m="131880">this</span>
  <span m="132090">quantity</span> <span m="133290">using</span> <span m="133800">various</span>
  <span m="134130">methods.</span> <span m="135340">And</span> <span m="136950">the</span>
  <span m="137040">question</span> <span m="137430">that</span> <span m="137550">didn't</span>
  <span m="137820">come</span> <span m="137970">up</span> <span m="138090">so</span>
  <span m="138240">much--</span> <span m="138720">or</span> <span m="138810">one</span>
  <span m="139050">question</span> <span m="139290">that</span> <span m="139380">didn't</span>
  <span m="139530">come</span> <span m="139680">up</span> <span m="139770">too</span>
  <span m="139860">much--</span> <span m="140130">is</span> <span m="140460">how</span>
  <span m="140640">do</span> <span m="140730">we</span> <span m="140850">use</span>
  <span m="141060">this</span> <span m="141210">quantity?</span> <span m="142140">We</span>
  <span m="142260">might</span> <span m="142500">be</span> <span m="142590">interested</span>
  <span m="143040">in</span> <span m="143540">it,</span> <span m="143700">just</span>
  <span m="144000">in</span> <span m="144120">terms</span> <span m="144480">of</span>
  <span m="145950">its</span> <span m="146160">absolute</span> <span m="146820">magnitude.</span>
  <span m="147930">How</span> <span m="148080">large</span> <span m="148410">is</span>
  <span m="148530">the</span> <span m="148620">effect?</span> <span m="148950">But</span>
  <span m="149070">we</span> <span m="149160">might</span> <span m="149310">also</span>
  <span m="149670">be</span> <span m="149760">interested</span> <span m="150120">in</span>
  <span m="150510">designing</span> <span m="151350">a</span> <span m="151410">policy</span>
  <span m="152040">for</span> <span m="152250">how</span> <span m="152460">to</span>
  <span m="152580">treat</span> <span m="152880">our</span> <span m="152970">patients</span>
  <span m="153960">based</span> <span m="154290">on</span> <span m="154410">this</span>
  <span m="154800">quantity.</span></p><p><span m="156280">So</span> <span m="156420">today,</span>
  <span m="157740">we</span> <span m="157890">will</span> <span m="158010">focus</span>
  <span m="158490">on</span> <span m="158730">policies.</span> <span m="159990">And</span>
  <span m="160110">what</span> <span m="160260">I</span> <span m="160320">mean</span>
  <span m="160530">by</span> <span m="160650">that,</span> <span m="160770">specifically,</span>
  <span m="161430">is</span> <span m="161610">something</span> <span m="162000">that</span>
  <span m="162120">takes</span> <span m="162420">into</span> <span m="163110">account</span>
  <span m="163500">what</span> <span m="163710">we</span> <span m="163830">know</span>
  <span m="164340">about</span> <span m="165030">a</span> <span m="165090">patient</span>
  <span m="166080">and</span> <span m="166260">produces</span> <span m="166980">a</span>
  <span m="167070">choice</span> <span m="167610">or</span> <span m="167700">an</span>
  <span m="167850">action</span> <span m="169370">as</span> <span m="169530">an</span>
  <span m="169620">output.</span> <span m="171030">Typically,</span> <span m="171510">we'll</span>
  <span m="171660">think</span> <span m="171840">of</span> <span m="171900">policies</span>
  <span m="172430">as</span> <span m="172690">depending</span> <span m="173130">on</span>
  <span m="173610">medical</span> <span m="173940">history,</span> <span m="174810">perhaps</span>
  <span m="175260">which</span> <span m="175530">treatments</span> <span m="175980">they</span>
  <span m="176100">have</span> <span m="176220">received</span> <span m="176550">previously,</span>
  <span m="177150">what</span> <span m="177390">state</span> <span m="177690">is</span>
  <span m="177810">the</span> <span m="178320">patient</span> <span m="178620">currently</span>
  <span m="179070">in.</span> <span m="181560">But</span> <span m="181770">we</span>
  <span m="181860">can</span> <span m="182010">also</span> <span m="182220">base</span>
  <span m="182520">it</span> <span m="182720">purely</span> <span m="183180">on</span>
  <span m="183300">this</span> <span m="183450">number</span> <span m="183780">that</span>
  <span m="183900">we</span> <span m="184050">produce</span> <span m="184590">last</span>
  <span m="184860">time--</span> <span m="185070">the</span> <span m="185160">conditional</span>
  <span m="185520">average</span> <span m="185790">treatment</span> <span m="186090">effect.</span>
  <span m="186720">And</span> <span m="186810">one</span> <span m="187020">very</span>
  <span m="187380">natural</span> <span m="187860">policy</span> <span m="188340">is</span>
  <span m="188490">to</span> <span m="188610">say,</span> <span m="189300">pi</span>
  <span m="189540">of</span> <span m="189660">x</span> <span m="189930">is</span>
  <span m="190050">equal</span> <span m="190320">to</span> <span m="190470">the</span>
  <span m="190590">indicator</span> <span m="191130">function</span> <span m="191580">representing</span>
  <span m="192360">if</span> <span m="193080">this</span> <span m="193260">CATE</span>
  <span m="193440">is</span> <span m="193530">positive.</span></p><p><span m="194500">So</span>
  <span m="194850">if</span> <span m="195180">the</span> <span m="195690">effect</span>
  <span m="195930">is</span> <span m="196020">positive,</span> <span m="196440">we</span>
  <span m="196620">treat</span> <span m="196830">the</span> <span m="196920">patient.</span>
  <span m="197280">If</span> <span m="197370">the</span> <span m="197440">effect</span>
  <span m="197670">is</span> <span m="197760">negative,</span> <span m="198120">we</span>
  <span m="198270">don't.</span> <span m="199060">And</span> <span m="199170">of</span>
  <span m="199260">course,</span> <span m="199780">positive</span> <span m="200280">will</span>
  <span m="200400">be</span> <span m="200580">relative</span> <span m="200970">to</span>
  <span m="201180">the</span> <span m="201720">usefulness</span> <span m="202380">of</span>
  <span m="202680">the</span> <span m="202800">outcome</span> <span m="203070">being</span>
  <span m="203280">high.</span> <span m="203640">But</span> <span m="204940">yeah,</span>
  <span m="205500">this</span> <span m="205680">is</span> <span m="205740">a</span>
  <span m="205770">very</span> <span m="205950">natural</span> <span m="206220">policy</span>
  <span m="206550">to</span> <span m="206670">consider.</span> <span m="207990">However,</span>
  <span m="210450">we</span> <span m="210540">can</span> <span m="210690">also</span>
  <span m="210870">think</span> <span m="211110">about</span> <span m="211650">much</span>
  <span m="211920">more</span> <span m="212430">complicated</span> <span m="212970">policies</span>
  <span m="213530">that</span> <span m="214860">are</span> <span m="214950">not</span>
  <span m="215280">just</span> <span m="215550">based</span> <span m="215970">on</span>
  <span m="216600">this</span> <span m="217620">number--</span> <span m="217980">the</span>
  <span m="218100">quality</span> <span m="218610">of</span> <span m="218700">the</span>
  <span m="218820">outcome.</span></p><p><span m="219550">We</span> <span m="219570">can</span>
  <span m="220080">think</span> <span m="220260">about</span> <span m="220470">policies</span>
  <span m="220830">that</span> <span m="220890">take</span> <span m="221180">into</span>
  <span m="221290">account</span> <span m="221520">legislation</span> <span m="222330">or</span>
  <span m="222900">cost</span> <span m="223470">of</span> <span m="223530">medication</span>
  <span m="224130">or</span> <span m="224370">side</span> <span m="224670">effects.</span>
  <span m="225330">We're</span> <span m="225450">not</span> <span m="225630">going</span>
  <span m="225700">to</span> <span m="225810">do</span> <span m="225930">that</span>
  <span m="226050">today,</span> <span m="226380">but</span> <span m="226500">that's</span>
  <span m="226620">something</span> <span m="226860">that</span> <span m="226950">you</span>
  <span m="227010">can</span> <span m="227130">keep</span> <span m="227310">in</span>
  <span m="227400">mind</span> <span m="227640">as</span> <span m="227760">we</span>
  <span m="227880">discuss</span> <span m="228180">these</span> <span m="228360">things.</span>
  <span m="231600">So</span> <span m="232440">David</span> <span m="232650">mentioned,</span>
  <span m="233080">we</span> <span m="233100">should</span> <span m="233460">now</span>
  <span m="233730">move</span> <span m="234150">from</span> <span m="234480">the</span>
  <span m="234600">one-step</span> <span m="235290">setting,</span> <span m="235650">where</span>
  <span m="235890">we</span> <span m="235980">have</span> <span m="236190">a</span>
  <span m="236250">single</span> <span m="236700">treatment</span> <span m="237330">acting</span>
  <span m="237660">at</span> <span m="237750">a</span> <span m="237780">single</span>
  <span m="238050">time</span> <span m="238810">and</span> <span m="238980">we</span>
  <span m="239100">only</span> <span m="239340">have</span> <span m="239430">to</span>
  <span m="239520">take</span> <span m="239760">into</span> <span m="239910">account</span>
  <span m="240530">the</span> <span m="240750">state</span> <span m="241020">of</span>
  <span m="241110">a</span> <span m="241170">patient</span> <span m="242030">once,</span>
  <span m="242460">basically.</span> <span m="243490">And</span> <span m="243660">we</span>
  <span m="243780">will</span> <span m="243900">move</span> <span m="244080">from</span>
  <span m="244230">that</span> <span m="244410">to</span> <span m="244950">the</span>
  <span m="245070">sequential</span> <span m="245520">setting.</span> <span m="246040">And</span>
  <span m="246210">my</span> <span m="246360">first</span> <span m="246600">example</span>
  <span m="247110">of</span> <span m="247290">such</span> <span m="247500">a</span>
  <span m="247560">setting</span> <span m="248280">is</span> <span m="248430">sepsis</span>
  <span m="248910">management.</span></p><p><span m="251280">So,</span> <span m="251440">sepsis</span>
  <span m="251870">is</span> <span m="251990">a</span> <span m="252290">complication</span>
  <span m="253310">of</span> <span m="253430">an</span> <span m="253520">infection,</span>
  <span m="255510">which</span> <span m="255680">can</span> <span m="255860">have</span>
  <span m="256040">very</span> <span m="256279">disastrous</span> <span m="257089">consequences.</span>
  <span m="257870">It</span> <span m="257970">can</span> <span m="258019">lead</span>
  <span m="258140">to</span> <span m="258230">organ</span> <span m="258529">failure</span>
  <span m="258890">and</span> <span m="259010">ultimately</span> <span m="259399">death.</span>
  <span m="259899">And</span> <span m="260029">it's</span> <span m="260120">actually</span>
  <span m="260329">one</span> <span m="260480">of</span> <span m="260540">the</span>
  <span m="260630">leading</span> <span m="260899">causes</span> <span m="261260">of</span>
  <span m="261350">deaths</span> <span m="261800">in</span> <span m="261980">the</span>
  <span m="262160">ICU.</span> <span m="263880">So</span> <span m="263900">it's</span>
  <span m="264290">of</span> <span m="264410">course</span> <span m="264770">important</span>
  <span m="265160">that</span> <span m="265280">we</span> <span m="265370">can</span>
  <span m="265850">manage</span> <span m="266270">and</span> <span m="266390">treat</span>
  <span m="266660">this</span> <span m="266930">condition.</span></p><p><span m="269180">When</span>
  <span m="269330">you</span> <span m="269420">start</span> <span m="269690">treating</span>
  <span m="269930">sepsis,</span> <span m="270290">the</span> <span m="270380">primary</span>
  <span m="270830">target--</span> <span m="271130">the</span> <span m="271220">first</span>
  <span m="271520">things</span> <span m="271730">you</span> <span m="271820">should</span>
  <span m="271970">think</span> <span m="272180">about</span> <span m="272360">fixing--</span>
  <span m="273980">is</span> <span m="274130">the</span> <span m="274220">infection</span>
  <span m="274580">itself.</span> <span m="275030">If</span> <span m="275180">we</span>
  <span m="275300">don't</span> <span m="275450">treat</span> <span m="275660">the</span>
  <span m="275720">infection,</span> <span m="276880">things</span> <span m="277130">are</span>
  <span m="277190">going</span> <span m="277280">to</span> <span m="277400">keep</span>
  <span m="277670">being</span> <span m="278000">bad.</span> <span m="279440">But</span>
  <span m="279620">even</span> <span m="279860">if</span> <span m="279950">we</span>
  <span m="280010">figure</span> <span m="280280">out</span> <span m="280400">the</span>
  <span m="280490">right</span> <span m="280730">antibiotic</span> <span m="281330">to</span>
  <span m="281420">treat</span> <span m="281630">the</span> <span m="281690">infection</span>
  <span m="282230">that</span> <span m="282380">is</span> <span m="282560">the</span>
  <span m="282800">source</span> <span m="283190">of</span> <span m="283280">the</span>
  <span m="283370">septic</span> <span m="284480">shock</span> <span m="284780">or</span>
  <span m="284840">the</span> <span m="284930">septic</span> <span m="285200">inflammation,</span>
  <span m="287690">there</span> <span m="287870">are</span> <span m="287930">a</span>
  <span m="287960">lot</span> <span m="288230">of</span> <span m="288350">different</span>
  <span m="288680">conditions</span> <span m="289070">that</span> <span m="289160">we</span>
  <span m="289220">need</span> <span m="289340">to</span> <span m="289430">manage.</span>
  <span m="290660">Because</span> <span m="291395">the</span> <span m="291710">infection</span>
  <span m="292040">itself</span> <span m="292400">can</span> <span m="292520">lead</span>
  <span m="292700">to</span> <span m="293480">fever,</span> <span m="294020">breathing</span>
  <span m="294410">difficulties,</span> <span m="296120">low</span> <span m="296300">blood</span>
  <span m="296540">pressure,</span> <span m="297560">high</span> <span m="297770">heart</span>
  <span m="297980">rate--</span> <span m="298430">all</span> <span m="298550">these</span>
  <span m="298730">kinds</span> <span m="299030">of</span> <span m="299090">things</span>
  <span m="299510">that</span> <span m="300250">are</span> <span m="300500">symptoms,</span>
  <span m="301680">but</span> <span m="301790">not</span> <span m="302030">the</span>
  <span m="302300">cause in</span> <span m="302630">themselves.</span> <span m="303140">But</span>
  <span m="303260">we</span> <span m="303350">still</span> <span m="303590">have</span>
  <span m="303740">to</span> <span m="303830">manage</span> <span m="304130">them</span>
  <span m="304250">somehow</span> <span m="304700">so</span> <span m="304880">that</span>
  <span m="305000">the</span> <span m="305060">patient</span> <span m="306500">survives</span>
  <span m="306980">and</span> <span m="307070">is</span> <span m="307160">comfortable.</span></p><p><span
  m="309370">So</span> <span m="309550">when I</span> <span m="309610">say</span>
  <span m="309790">sepsis</span> <span m="310090">management,</span> <span m="310630">I'm</span>
  <span m="311950">talking</span> <span m="312250">about</span> <span m="312550">managing</span>
  <span m="313150">such</span> <span m="313570">quantities</span> <span m="314110">over</span>
  <span m="314350">time--</span> <span m="315580">over a</span> <span m="315910">patient's</span>
  <span m="316240">stay</span> <span m="316420">in</span> <span m="317050">the</span>
  <span m="317140">hospital.</span> <span m="319300">So,</span> <span m="320530">last</span>
  <span m="320800">time--</span> <span m="320980">again,</span> <span m="321460">just</span>
  <span m="321710">to</span> <span m="322180">really</span> <span m="322540">hammer</span>
  <span m="322820">this</span> <span m="323080">in--</span> <span m="323200">we</span>
  <span m="323320">talked</span> <span m="323560">about</span> <span m="323770">potential</span>
  <span m="324220">outcomes</span> <span m="325120">and</span> <span m="325210">the</span>
  <span m="325300">choice</span> <span m="325780">of</span> <span m="325900">a</span>
  <span m="325960">single</span> <span m="326350">treatment.</span> <span m="327490">So</span>
  <span m="327910">we</span> <span m="328090">can</span> <span m="328210">think</span>
  <span m="328390">about</span> <span m="328600">this</span> <span m="328780">in</span>
  <span m="328870">the</span> <span m="328960">septic</span> <span m="329470">setting</span>
  <span m="329980">as</span> <span m="330310">a</span> <span m="330370">patient</span>
  <span m="330670">coming</span> <span m="330970">in--</span> <span m="331240">or</span>
  <span m="331580">a</span> <span m="331660">patient</span> <span m="331930">already</span>
  <span m="332230">being</span> <span m="332420">in</span> <span m="332490">the</span>
  <span m="332540">hospital,</span> <span m="333510">presumably--</span> <span m="334550">and</span>
  <span m="334720">is</span> <span m="334840">presenting</span> <span m="335170">with</span>
  <span m="335260">breathing</span> <span m="335560">difficulties.</span> <span m="336670">So</span>
  <span m="336940">that</span> <span m="337060">means</span> <span m="337300">that</span>
  <span m="337390">their</span> <span m="337600">blood</span> <span m="337870">oxygen</span>
  <span m="338380">will</span> <span m="338590">be</span> <span m="338710">low</span>
  <span m="339040">because</span> <span m="339280">they</span> <span m="339370">can't</span>
  <span m="339580">breathe</span> <span m="339820">on</span> <span m="339940">their</span>
  <span m="340150">own.</span> <span m="340640">And</span> <span m="340740">we</span>
  <span m="340750">might</span> <span m="340990">want</span> <span m="341230">to</span>
  <span m="341410">put</span> <span m="341620">them</span> <span m="341800">on</span>
  <span m="342130">mechanical</span> <span m="342580">ventilation</span> <span m="343150">so</span>
  <span m="343300">that</span> <span m="343390">we</span> <span m="343450">can</span>
  <span m="343570">ensure</span> <span m="343930">that</span> <span m="344050">they</span>
  <span m="344110">get</span> <span m="344290">sufficient</span> <span m="344980">oxygen.</span></p><p><span
  m="346850">We</span> <span m="347000">can</span> <span m="347150">view</span> <span
  m="347330">this</span> <span m="347510">as</span> <span m="347630">a</span> <span
  m="347690">single</span> <span m="348080">choice.</span> <span m="348950">Should</span>
  <span m="349250">we</span> <span m="349490">put</span> <span m="350030">the</span>
  <span m="350630">patient</span> <span m="350990">on</span> <span m="351530">mechanical</span>
  <span m="351950">ventilation</span> <span m="352460">or</span> <span m="352550">not?</span>
  <span m="353480">But</span> <span m="354170">what</span> <span m="354350">we</span>
  <span m="354440">need</span> <span m="354650">to</span> <span m="354710">take</span>
  <span m="354920">into</span> <span m="355070">account</span> <span m="355940">here</span>
  <span m="356630">is</span> <span m="356780">what</span> <span m="356930">will</span>
  <span m="357080">happen</span> <span m="357470">after</span> <span m="357800">we</span>
  <span m="357920">make</span> <span m="358130">that</span> <span m="358280">choice.</span>
  <span m="359210">What</span> <span m="359750">will</span> <span m="359900">be</span>
  <span m="360050">the</span> <span m="360230">side</span> <span m="360560">effects</span>
  <span m="360860">of</span> <span m="360950">this</span> <span m="361160">choice</span>
  <span m="361490">going</span> <span m="361760">further?</span> <span m="362210">Because</span>
  <span m="362420">we</span> <span m="362510">want</span> <span m="362690">to</span>
  <span m="362780">make</span> <span m="362930">sure</span> <span m="363260">that</span>
  <span m="363410">the</span> <span m="363500">patient</span> <span m="363770">is</span>
  <span m="363860">comfortable</span> <span m="364790">and</span> <span m="365060">in</span>
  <span m="365180">good</span> <span m="365330">health</span> <span m="365690">throughout</span>
  <span m="366110">their</span> <span m="366260">stay.</span></p><p><span m="368370">So</span>
  <span m="368820">today,</span> <span m="369690">we</span> <span m="369810">will</span>
  <span m="369960">move</span> <span m="370320">towards</span> <span m="370770">sequential</span>
  <span m="371310">decision</span> <span m="371670">making.</span> <span m="373500">And</span>
  <span m="373680">in</span> <span m="373740">particular,</span> <span m="374790">what</span>
  <span m="374970">I</span> <span m="375090">alluded</span> <span m="375390">to</span>
  <span m="375510">just</span> <span m="375690">now</span> <span m="376050">is</span>
  <span m="376200">that</span> <span m="376730">decisions</span> <span m="377400">made</span>
  <span m="377610">in</span> <span m="377700">sequence</span> <span m="378540">may</span>
  <span m="378690">have</span> <span m="378810">the</span> <span m="378870">property</span>
  <span m="379290">that</span> <span m="379410">choices</span> <span m="379890">early</span>
  <span m="380190">on</span> <span m="381240">rule</span> <span m="381510">out</span>
  <span m="381750">certain</span> <span m="382080">choices</span> <span m="382440">later.</span>
  <span m="383420">And</span> <span m="383780">we'll</span> <span m="383910">see</span>
  <span m="384030">an</span> <span m="384120">example</span> <span m="384450">of</span>
  <span m="384510">that</span> <span m="385060">very</span> <span m="385140">soon.</span></p><p><span
  m="386730">And</span> <span m="386880">in</span> <span m="386940">particular,</span>
  <span m="387490">we'll</span> <span m="387540">be</span> <span m="387720">interested</span>
  <span m="388140">in</span> <span m="388380">coming</span> <span m="388680">up</span>
  <span m="388800">with</span> <span m="388920">a</span> <span m="388980">policy</span>
  <span m="389550">for</span> <span m="389700">making</span> <span m="390060">decisions</span>
  <span m="390870">repeatedly</span> <span m="393090">that</span> <span m="393270">optimizes</span>
  <span m="393930">a</span> <span m="393990">given</span> <span m="394260">outcome--</span>
  <span m="394980">something</span> <span m="395250">that</span> <span m="395340">we</span>
  <span m="395430">care</span> <span m="395610">about.</span> <span m="396210">It</span>
  <span m="396300">could</span> <span m="396420">be</span> <span m="398790">minimize</span>
  <span m="399270">the</span> <span m="399360">risk</span> <span m="399750">of</span>
  <span m="399840">death.</span> <span m="400620">It</span> <span m="400710">could</span>
  <span m="400860">be</span> <span m="402090">a</span> <span m="402180">reward</span>
  <span m="402540">that</span> <span m="402690">says</span> <span m="402990">that</span>
  <span m="403170">the</span> <span m="403320">vitals</span> <span m="403890">of</span>
  <span m="403980">a</span> <span m="404040">patients</span> <span m="404400">are</span>
  <span m="404490">in</span> <span m="404580">the</span> <span m="404640">right</span>
  <span m="404940">range.</span> <span m="405810">We</span> <span m="405890">might</span>
  <span m="406050">want</span> <span m="406230">to</span> <span m="406290">optimize</span>
  <span m="406710">that.</span> <span m="407830">But</span> <span m="407880">essentially,</span>
  <span m="408270">think</span> <span m="408480">about</span> <span m="408750">it</span>
  <span m="408810">now</span> <span m="409120">as</span> <span m="409890">having</span>
  <span m="410180">this</span> <span m="411570">choice</span> <span m="411870">of</span>
  <span m="412710">administering</span> <span m="413280">a</span> <span m="413460">medication</span>
  <span m="413940">or</span> <span m="414000">an</span> <span m="414090">intervention</span>
  <span m="414660">at</span> <span m="414780">any</span> <span m="414890">time,</span>
  <span m="415290">t--</span> <span m="416730">and</span> <span m="416850">having</span>
  <span m="417090">the</span> <span m="417150">best</span> <span m="417300">policy</span>
  <span m="417630">for</span> <span m="417750">doing</span> <span m="417960">so.</span></p><p><span
  m="420440">OK,</span> <span m="420710">I'm</span> <span m="421168">going to</span>
  <span m="421626">skip</span> <span m="422084">that one.</span> <span m="423460">OK,</span>
  <span m="423740">so</span> <span m="424490">I</span> <span m="424580">mentioned</span>
  <span m="424880">already</span> <span m="425240">one</span> <span m="425780">potential</span>
  <span m="426200">choice</span> <span m="426470">that</span> <span m="426590">we</span>
  <span m="426860">might</span> <span m="427100">want</span> <span m="427220">to</span>
  <span m="427280">make</span> <span m="427550">in</span> <span m="427610">the</span>
  <span m="427700">management</span> <span m="428210">of</span> <span m="428300">a</span>
  <span m="428330">septic</span> <span m="428660">patient,</span> <span m="429060">which</span>
  <span m="429140">is</span> <span m="429320">to</span> <span m="429410">put</span>
  <span m="429620">them</span> <span m="429830">on</span> <span m="429920">mechanical</span>
  <span m="430400">ventilation</span> <span m="430910">because</span> <span m="431140">they</span>
  <span m="431210">can't</span> <span m="431480">breathe</span> <span m="432110">on</span>
  <span m="432230">their</span> <span m="432410">own.</span> <span m="434040">A</span>
  <span m="434210">side</span> <span m="434480">effect</span> <span m="434720">of</span>
  <span m="434810">doing</span> <span m="435050">so</span> <span m="435290">is</span>
  <span m="435410">that</span> <span m="435560">they</span> <span m="435650">might</span>
  <span m="436910">suffer</span> <span m="437180">discomfort</span> <span m="438380">from</span>
  <span m="438560">being</span> <span m="438710">intubated.</span> <span m="441650">The</span>
  <span m="441920">procedure</span> <span m="442310">is</span> <span m="442880">not</span>
  <span m="443150">painless,</span> <span m="443540">it's</span> <span m="443660">not</span>
  <span m="443960">without</span> <span m="444200">discomfort.</span></p><p><span
  m="444680">So</span> <span m="445280">something</span> <span m="445640">that</span>
  <span m="445760">you</span> <span m="445820">might</span> <span m="446060">have</span>
  <span m="446180">to</span> <span m="446270">do--</span> <span m="447020">putting</span>
  <span m="447260">them</span> <span m="447410">on</span> <span m="447500">mechanical</span>
  <span m="447860">ventilation--</span> <span m="448370">is</span> <span m="448580">to</span>
  <span m="448850">sedate</span> <span m="449210">the</span> <span m="449270">patient.</span>
  <span m="451440">So</span> <span m="451490">this</span> <span m="451640">is</span>
  <span m="452690">an</span> <span m="453320">action</span> <span m="453740">that</span>
  <span m="453920">is</span> <span m="454100">informed</span> <span m="454490">by</span>
  <span m="454610">the</span> <span m="454700">previous</span> <span m="455150">action,</span>
  <span m="455450">because</span> <span m="455750">if</span> <span m="455840">we</span>
  <span m="455960">didn't</span> <span m="456260">put</span> <span m="456410">the</span>
  <span m="456530">patient</span> <span m="456800">on</span> <span m="456950">mechanical</span>
  <span m="457370">ventilation,</span> <span m="457850">maybe</span> <span m="458150">we</span>
  <span m="458270">wouldn't</span> <span m="458600">consider</span> <span m="458990">them</span>
  <span m="459110">for</span> <span m="459260">sedation.</span> <span m="463920">When</span>
  <span m="464070">we</span> <span m="464190">sedate</span> <span m="464430">a</span>
  <span m="464490">patient,</span> <span m="464970">we</span> <span m="465160">run</span>
  <span m="465330">the</span> <span m="465420">risk</span> <span m="465810">of</span>
  <span m="466200">lowering</span> <span m="466980">their</span> <span m="467520">blood</span>
  <span m="467700">pressure.</span> <span m="468970">So</span> <span m="469020">we</span>
  <span m="469170">might</span> <span m="469410">need</span> <span m="469560">to</span>
  <span m="469650">manage</span> <span m="470010">that,</span> <span m="470250">too.</span></p><p><span
  m="471780">So</span> <span m="472440">if</span> <span m="472740">their</span> <span
  m="472890">blood</span> <span m="473070">pressure</span> <span m="473310">gets</span>
  <span m="473550">too</span> <span m="473790">low,</span> <span m="474270">maybe</span>
  <span m="474570">we</span> <span m="474660">need</span> <span m="474810">to</span>
  <span m="474990">administer</span> <span m="475440">vasopressors,</span> <span m="476310">which</span>
  <span m="476580">artificially</span> <span m="477090">raise</span> <span m="477320">the</span>
  <span m="477420">blood</span> <span m="477570">pressure,</span> <span m="478200">or</span>
  <span m="478440">fluids</span> <span m="478920">or</span> <span m="479010">anything</span>
  <span m="479370">else</span> <span m="479820">that</span> <span m="480030">takes</span>
  <span m="480300">care</span> <span m="480510">of</span> <span m="480570">this</span>
  <span m="480900">issue.</span> <span m="482670">So</span> <span m="483330">just</span>
  <span m="484020">think</span> <span m="484230">of</span> <span m="484320">this</span>
  <span m="484470">as</span> <span m="484590">an</span> <span m="484680">example</span>
  <span m="485050">of</span> <span m="485550">choices</span> <span m="486150">cascading,</span>
  <span m="486750">in</span> <span m="486840">terms</span> <span m="487110">of</span>
  <span m="487200">their</span> <span m="487620">consequences,</span> <span m="489000">as</span>
  <span m="489150">we</span> <span m="489660">roll</span> <span m="489900">forward</span>
  <span m="490200">in</span> <span m="490320">time.</span></p><p><span m="493190">Ultimately,</span>
  <span m="494540">we</span> <span m="494750">will</span> <span m="495290">face</span>
  <span m="495590">the</span> <span m="495710">end</span> <span m="496040">of</span>
  <span m="496460">the</span> <span m="496520">patient's</span> <span m="496910">stay.</span>
  <span m="497690">And</span> <span m="497960">hopefully,</span> <span m="498470">we</span>
  <span m="498620">managed</span> <span m="499340">the</span> <span m="499430">patient</span>
  <span m="499730">in</span> <span m="499820">a</span> <span m="499880">successful</span>
  <span m="500330">way</span> <span m="500990">so</span> <span m="501200">that</span>
  <span m="501440">their</span> <span m="502970">response</span> <span m="503570">or</span>
  <span m="503720">their</span> <span m="504170">outcome</span> <span m="504560">is</span>
  <span m="504710">a</span> <span m="504770">good</span> <span m="504920">one.</span>
  <span m="506330">What</span> <span m="507710">I'm</span> <span m="507920">illustrating</span>
  <span m="508490">here</span> <span m="509000">is</span> <span m="509240">that,</span>
  <span m="509990">for</span> <span m="510170">any</span> <span m="510410">one</span>
  <span m="510650">patient</span> <span m="511070">in</span> <span m="511190">our</span>
  <span m="511310">hospitals</span> <span m="511880">or</span> <span m="511970">in</span>
  <span m="512059">the</span> <span m="512120">health</span> <span m="512210">care</span>
  <span m="512419">system,</span> <span m="512990">we</span> <span m="513140">will</span>
  <span m="513289">only</span> <span m="513590">observe</span> <span m="513950">one</span>
  <span m="514220">trajectory</span> <span m="515659">through</span> <span m="515840">these</span>
  <span m="516049">options.</span></p><p><span m="516409">So</span> <span m="516770">I</span>
  <span m="516919">will</span> <span m="517130">show</span> <span m="517340">this</span>
  <span m="518210">type</span> <span m="518539">of</span> <span m="518659">illustration</span>
  <span m="519480">many</span> <span m="519590">times,</span> <span m="521250">but</span>
  <span m="521630">I</span> <span m="521690">hope</span> <span m="521870">that</span>
  <span m="522890">you</span> <span m="523039">can</span> <span m="523409">realize</span>
  <span m="524179">the</span> <span m="525530">scope</span> <span m="526160">of</span>
  <span m="526370">the</span> <span m="526520">decision</span> <span m="526970">space</span>
  <span m="527300">here.</span> <span m="527990">Essentially,</span> <span m="528470">at</span>
  <span m="528590">any</span> <span m="528860">point,</span> <span m="529320">we</span>
  <span m="529340">can</span> <span m="529490">choose</span> <span m="529760">a</span>
  <span m="529820">different</span> <span m="530120">action.</span> <span m="530840">And</span>
  <span m="530990">usually,</span> <span m="531560">the</span> <span m="531680">number</span>
  <span m="531980">of</span> <span m="532070">decisions</span> <span m="532520">that</span>
  <span m="532640">we</span> <span m="532730">make</span> <span m="533750">in</span>
  <span m="535610">an</span> <span m="536150">ICU</span> <span m="536570">setting,</span>
  <span m="536870">for</span> <span m="536960">example,</span> <span m="537810">is</span>
  <span m="537890">much</span> <span m="538520">larger</span> <span m="539120">than</span>
  <span m="539270">we</span> <span m="539360">could</span> <span m="539480">ever</span>
  <span m="539720">test</span> <span m="541030">in</span> <span m="541670">a</span>
  <span m="541730">randomized</span> <span m="542180">trial.</span></p><p><span m="542480">Think</span>
  <span m="542720">of</span> <span m="543740">all</span> <span m="544010">of</span>
  <span m="544130">these</span> <span m="544430">different</span> <span m="544820">trajectories</span>
  <span m="545450">as</span> <span m="545570">being</span> <span m="545900">different</span>
  <span m="546920">arms</span> <span m="547640">in</span> <span m="547790">a</span>
  <span m="547850">randomized</span> <span m="548210">controlled</span> <span m="548540">trial</span>
  <span m="549100">that</span> <span m="549200">you</span> <span m="549290">want</span>
  <span m="549410">to</span> <span m="549470">compare</span> <span m="549830">the</span>
  <span m="549920">effects</span> <span m="551210">or</span> <span m="551330">the</span>
  <span m="551450">outcomes</span> <span m="551810">of.</span> <span m="553010">It's</span>
  <span m="553400">infeasible</span> <span m="553970">to</span> <span m="554060">run</span>
  <span m="554270">such</span> <span m="554450">a</span> <span m="554510">trial,</span>
  <span m="554810">typically.</span> <span m="555290">So</span> <span m="555920">one</span>
  <span m="556220">of</span> <span m="556280">the</span> <span m="556400">big</span>
  <span m="556700">reasons</span> <span m="557060">that</span> <span m="557150">we</span>
  <span m="557210">are</span> <span m="557300">talking</span> <span m="557540">about</span>
  <span m="557660">reinforcement</span> <span m="558200">learning</span> <span m="558410">today</span>
  <span m="559130">and</span> <span m="559340">talking</span> <span m="559640">about</span>
  <span m="559910">learning</span> <span m="560150">policies,</span> <span m="560690">rather</span>
  <span m="561020">than</span> <span m="561800">causal</span> <span m="562190">effects</span>
  <span m="562900">in</span> <span m="563030">the</span> <span m="563150">setup</span>
  <span m="563420">that</span> <span m="563540">we</span> <span m="563630">did</span>
  <span m="563750">last</span> <span m="563960">week,</span> <span m="564440">is</span>
  <span m="564620">because</span> <span m="564920">the</span> <span m="565220">space</span>
  <span m="565730">of</span> <span m="565790">possible</span> <span m="566240">action</span>
  <span m="566510">trajectories</span> <span m="566930">is</span> <span m="567020">so</span>
  <span m="567170">large.</span></p><p><span m="575010">Having</span> <span m="575250">said</span>
  <span m="575400">that,</span> <span m="576990">we</span> <span m="577170">now</span>
  <span m="577710">turn</span> <span m="578010">to</span> <span m="578700">trying</span>
  <span m="579000">to</span> <span m="579090">find,</span> <span m="580620">essentially,</span>
  <span m="581160">the</span> <span m="581250">policy</span> <span m="581610">that</span>
  <span m="582150">picks</span> <span m="582480">this</span> <span m="582720">orange</span>
  <span m="583620">path</span> <span m="584010">here--</span> <span m="584190">that</span>
  <span m="584340">leads</span> <span m="584580">to</span> <span m="584670">a</span>
  <span m="584730">good</span> <span m="584940">outcome.</span> <span m="585390">And</span>
  <span m="586660">to</span> <span m="586890">reason</span> <span m="587340">about</span>
  <span m="587700">such</span> <span m="587970">a</span> <span m="588030">thing,</span>
  <span m="588290">we</span> <span m="588420">need</span> <span m="588570">to</span>
  <span m="588930">also</span> <span m="589230">reason</span> <span m="589530">about</span>
  <span m="589740">what</span> <span m="590130">is</span> <span m="590340">a</span>
  <span m="590400">good</span> <span m="590640">outcome?</span> <span m="591220">What</span>
  <span m="591360">is</span> <span m="591750">good</span> <span m="592020">reward</span>
  <span m="592920">for</span> <span m="594300">our</span> <span m="594630">agent,</span>
  <span m="595140">as</span> <span m="595290">it</span> <span m="595710">proceeds</span>
  <span m="596220">through</span> <span m="596430">time</span> <span m="596840">and</span>
  <span m="596970">makes</span> <span m="597270">choices?</span></p><p><span m="598890">Some</span>
  <span m="599130">policies</span> <span m="601660">that</span> <span m="601770">we</span>
  <span m="601890">produce</span> <span m="602370">as</span> <span m="602530">machine
  learners</span> <span m="602970">might</span> <span m="603150">not</span> <span
  m="603270">be</span> <span m="603360">appropriate</span> <span m="603840">for</span>
  <span m="603930">a</span> <span m="603960">health</span> <span m="604130">care</span>
  <span m="604290">setting.</span> <span m="606270">We</span> <span m="606690">have</span>
  <span m="606780">to</span> <span m="606870">somehow</span> <span m="607200">restrict</span>
  <span m="607890">ourself</span> <span m="608130">to</span> <span m="608220">something</span>
  <span m="608520">that's</span> <span m="608700">realistic.</span> <span m="610230">I</span>
  <span m="610350">won't</span> <span m="610770">focus</span> <span m="611190">very</span>
  <span m="611400">much</span> <span m="611610">on</span> <span m="611730">this</span>
  <span m="611880">today.</span> <span m="612270">It's</span> <span m="612390">something</span>
  <span m="612630">that</span> <span m="612720">will</span> <span m="612840">come</span>
  <span m="613050">up</span> <span m="613140">in</span> <span m="613230">the</span>
  <span m="613290">discussion</span> <span m="613740">tomorrow,</span> <span m="614580">hopefully.</span>
  <span m="615390">And</span> <span m="615900">also</span> <span m="616220">the</span>
  <span m="616500">notion</span> <span m="616830">of</span> <span m="616920">evaluating</span>
  <span m="617580">something</span> <span m="618330">for</span> <span m="619350">use</span>
  <span m="619680">in</span> <span m="619770">the</span> <span m="619830">health</span>
  <span m="619930">care</span> <span m="620100">system</span> <span m="620400">will</span>
  <span m="620550">also</span> <span m="620730">be</span> <span m="620850">talked</span>
  <span m="621090">about</span> <span m="621240">tomorrow.</span></p><p><span m="623478">AUDIENCE:</span>
  <span m="623709">Thursday.</span></p><p><span m="624270">FREDRIK D. JOHANSSON:</span>
  <span m="624405">Sorry,</span> <span m="624960">Thursday.</span> <span m="626370">Next</span>
  <span m="626580">time.</span> <span m="628200">OK,</span> <span m="629220">so</span>
  <span m="629880">I'll</span> <span m="630000">start</span> <span m="630270">by</span>
  <span m="631140">just</span> <span m="631470">briefly</span> <span m="631800">mentioning</span>
  <span m="633030">some</span> <span m="633210">success</span> <span m="633510">stories.</span>
  <span m="634260">And</span> <span m="634560">these</span> <span m="634890">are</span>
  <span m="635040">not</span> <span m="635250">from</span> <span m="635400">the</span>
  <span m="635460">health</span> <span m="635560">care</span> <span m="635760">setting,</span>
  <span m="636120">as</span> <span m="636240">you</span> <span m="636330">can</span>
  <span m="636600">guess</span> <span m="636810">from</span> <span m="636960">the</span>
  <span m="637020">pictures.</span> <span m="637980">How</span> <span m="638160">many</span>
  <span m="638370">have</span> <span m="638520">seen</span> <span m="639600">some</span>
  <span m="639900">of</span> <span m="639990">these</span> <span m="641370">pictures?</span>
  <span m="641760">OK,</span> <span m="643410">great--</span> <span m="643710">almost</span>
  <span m="643980">everyone.</span></p><p><span m="647360">Yeah,</span> <span m="647580">so</span>
  <span m="647700">these</span> <span m="647880">are</span> <span m="647940">from</span>
  <span m="648840">various</span> <span m="649760">video</span> <span m="650070">games--</span>
  <span m="650490">almost</span> <span m="650760">all</span> <span m="650880">of</span>
  <span m="650970">them.</span> <span m="651710">Well,</span> <span m="652410">games</span>
  <span m="652740">anyhow.</span> <span m="654630">And</span> <span m="656530">these</span>
  <span m="657550">are</span> <span m="657670">good</span> <span m="657940">examples</span>
  <span m="658390">of</span> <span m="658540">when</span> <span m="658810">reinforcement</span>
  <span m="659350">learning</span> <span m="659680">works,</span> <span m="660240">essentially.</span>
  <span m="660970">That's</span> <span m="661330">why</span> <span m="661480">I</span>
  <span m="661580">use</span> <span m="662000">these</span> <span m="663370">in</span>
  <span m="663630">this</span> <span m="664440">slide</span> <span m="664780">here--</span>
  <span m="665560">because,</span> <span m="665890">essentially,</span> <span m="666220">it's</span>
  <span m="666340">very</span> <span m="666520">hard</span> <span m="666670">to</span>
  <span m="666790">argue</span> <span m="667150">that</span> <span m="667450">the</span>
  <span m="667750">computer</span> <span m="668230">or</span> <span m="668380">the</span>
  <span m="668860">program</span> <span m="669310">that</span> <span m="669460">eventually</span>
  <span m="671020">beat</span> <span m="671530">Lee</span> <span m="671800">Sedol.</span>
  <span m="672160">I</span> <span m="672220">think</span> <span m="672460">it's</span>
  <span m="672610">in</span> <span m="672700">this</span> <span m="672850">picture</span>
  <span m="673210">but</span> <span m="673330">also,</span> <span m="673840">later,</span>
  <span m="674530">Go</span> <span m="674830">champions,</span> <span m="675430">essentially.</span></p><p><span
  m="676480">In</span> <span m="676600">the</span> <span m="676720">AlphaGo</span>
  <span m="677050">picture</span> <span m="677350">in</span> <span m="677440">the</span>
  <span m="678130">top</span> <span m="678370">left,</span> <span m="678940">it's</span>
  <span m="679060">hard</span> <span m="679180">to</span> <span m="679240">argue</span>
  <span m="679480">that</span> <span m="679600">they're</span> <span m="679720">not</span>
  <span m="679900">doing</span> <span m="680110">a</span> <span m="680170">good</span>
  <span m="680290">job,</span> <span m="680660">because</span> <span m="680800">they</span>
  <span m="680950">clearly</span> <span m="681400">beat</span> <span m="681580">humans</span>
  <span m="681910">here.</span> <span m="684220">But</span> <span m="684370">one</span>
  <span m="685210">of</span> <span m="685300">the</span> <span m="685870">things</span>
  <span m="686110">I</span> <span m="686170">want</span> <span m="686260">you</span>
  <span m="686380">to</span> <span m="686440">keep</span> <span m="686620">in</span>
  <span m="686710">mind</span> <span m="687700">throughout</span> <span m="688090">this</span>
  <span m="688270">talk</span> <span m="688600">is</span> <span m="688720">what</span>
  <span m="688930">is</span> <span m="689050">different</span> <span m="689380">between</span>
  <span m="689770">these</span> <span m="690010">kinds</span> <span m="690250">of</span>
  <span m="690340">scenarios?</span> <span m="690850">And</span> <span m="690940">we'll</span>
  <span m="691270">come</span> <span m="691480">back</span> <span m="691630">to</span>
  <span m="691720">that</span> <span m="691870">later.</span> <span m="692500">And</span>
  <span m="693340">what</span> <span m="693520">is</span> <span m="693580">different</span>
  <span m="693850">to</span> <span m="694240">the</span> <span m="694330">health</span>
  <span m="694530">care</span> <span m="694660">setting,</span> <span m="694900">essentially?</span></p><p><span
  m="696400">So</span> <span m="697270">I</span> <span m="697500">simply</span> <span
  m="697830">added</span> <span m="698490">another</span> <span m="698850">example</span>
  <span m="699310">here,</span> <span m="699450">that's why</span> <span m="699600">I</span>
  <span m="699660">recognize it.</span> <span m="699930">So</span> <span m="700050">there</span>
  <span m="700140">was</span> <span m="700350">recently</span> <span m="700740">one</span>
  <span m="700950">that's</span> <span m="701340">a</span> <span m="701400">little</span>
  <span m="701550">bit</span> <span m="701700">closer</span> <span m="701970">to</span>
  <span m="702060">my</span> <span m="702180">heart,</span> <span m="702420">which</span>
  <span m="702600">is</span> <span m="702770">AlphaStar.</span> <span m="703680">I</span>
  <span m="703770">play</span> <span m="703950">StarCraft.</span> <span m="705500">I</span>
  <span m="705570">like</span> <span m="705750">StarCraft,</span> <span m="706350">so</span>
  <span m="707325">it</span> <span m="707790">should</span> <span m="708000">be</span>
  <span m="708120">on</span> <span m="708180">the</span> <span m="708280">slide.</span>
  <span m="709380">Anyway,</span> <span m="711120">let's</span> <span m="711300">move</span>
  <span m="711480">on.</span></p><p><span m="713400">Broadly</span> <span m="713760">speaking,</span>
  <span m="714250">these</span> <span m="714330">can</span> <span m="714570">be</span>
  <span m="715290">summarized</span> <span m="715800">in</span> <span m="715890">the</span>
  <span m="715950">following</span> <span m="716280">picture.</span> <span m="716590">What</span>
  <span m="717030">goes</span> <span m="717390">into</span> <span m="717780">those</span>
  <span m="717960">systems?</span> <span m="719330">There's</span> <span m="719640">a</span>
  <span m="719700">lot</span> <span m="719850">more</span> <span m="720000">nuance</span>
  <span m="720330">when</span> <span m="720480">it</span> <span m="720540">comes</span>
  <span m="720720">to</span> <span m="720810">something</span> <span m="721650">like</span>
  <span m="722010">Go.</span> <span m="722960">But</span> <span m="723670">for</span>
  <span m="723960">the</span> <span m="724170">purpose</span> <span m="724440">of</span>
  <span m="724500">this</span> <span m="724650">class,</span> <span m="725520">we</span>
  <span m="725670">will</span> <span m="725880">summarize</span> <span m="726270">them</span>
  <span m="726390">with</span> <span m="726510">a</span> <span m="726540">slide.</span>
  <span m="727350">So</span> <span m="727470">essentially,</span> <span m="728580">one</span>
  <span m="729270">of</span> <span m="729330">the</span> <span m="729450">three</span>
  <span m="729900">quantities</span> <span m="730560">that</span> <span m="730680">matters</span>
  <span m="731070">for</span> <span m="731240">a</span> <span m="731280">reinforcement</span>
  <span m="731760">learning</span> <span m="732000">is</span> <span m="732150">the</span>
  <span m="732240">state</span> <span m="733290">of</span> <span m="733410">the</span>
  <span m="733470">environment,</span> <span m="733980">the</span> <span m="734070">state</span>
  <span m="734340">of</span> <span m="734430">the</span> <span m="734520">game,</span>
  <span m="735090">the</span> <span m="735180">state</span> <span m="735390">of</span>
  <span m="735450">the</span> <span m="735540">patient--</span> <span m="736260">the</span>
  <span m="736350">state</span> <span m="736650">of</span> <span m="736770">the</span>
  <span m="736830">thing</span> <span m="737130">that</span> <span m="737280">we</span>
  <span m="737370">want</span> <span m="737580">to</span> <span m="737790">optimize,</span>
  <span m="738270">essentially.</span></p><p><span m="740500">So</span> <span m="740550">in</span>
  <span m="740640">this</span> <span m="740760">case,</span> <span m="741070">I've</span>
  <span m="741170">chosen</span> <span m="741390">Tic-tac-toe</span> <span m="741960">here.</span>
  <span m="742770">We</span> <span m="742950">have</span> <span m="743100">a</span>
  <span m="743160">state</span> <span m="743490">which</span> <span m="743670">represents</span>
  <span m="744120">the</span> <span m="744240">current</span> <span m="745320">positions</span>
  <span m="745830">of</span> <span m="746460">the</span> <span m="747000">circles</span>
  <span m="747390">and</span> <span m="747480">crosses.</span> <span m="748620">And</span>
  <span m="750000">given</span> <span m="751050">that</span> <span m="751260">state</span>
  <span m="751620">of</span> <span m="751710">the</span> <span m="751800">game,</span>
  <span m="752310">my</span> <span m="752550">job</span> <span m="753000">as</span>
  <span m="753120">a</span> <span m="753180">player</span> <span m="753540">is</span>
  <span m="753690">to</span> <span m="753750">choose</span> <span m="754290">one</span>
  <span m="754560">of</span> <span m="756825">the</span> <span m="757200">possible</span>
  <span m="757470">actions--</span> <span m="757830">one</span> <span m="757980">of</span>
  <span m="758040">the</span> <span m="758100">free</span> <span m="758460">squares</span>
  <span m="758880">to</span> <span m="758970">put</span> <span m="759150">my</span>
  <span m="759300">cross</span> <span m="759730">in.</span> <span m="761270">So I'm</span>
  <span m="761630">the</span> <span m="761700">blue</span> <span m="761910">player</span>
  <span m="762180">here</span> <span m="762480">and</span> <span m="762630">I</span>
  <span m="762690">can</span> <span m="762810">consider</span> <span m="763230">these</span>
  <span m="764280">five</span> <span m="764970">choices</span> <span m="766050">for</span>
  <span m="766200">where</span> <span m="766350">to</span> <span m="766440">put</span>
  <span m="766590">my</span> <span m="766680">next</span> <span m="766920">cross.</span>
  <span m="767680">And</span> <span m="767850">each</span> <span m="768030">of</span>
  <span m="768150">those</span> <span m="768420">will</span> <span m="768570">lead</span>
  <span m="768720">me</span> <span m="768810">to</span> <span m="768960">a</span>
  <span m="769020">new</span> <span m="769230">state</span> <span m="770250">of</span>
  <span m="770370">the</span> <span m="770430">game.</span></p><p><span m="771480">If</span>
  <span m="771630">I</span> <span m="771720">put</span> <span m="771960">my</span>
  <span m="772890">cross</span> <span m="773220">over</span> <span m="773520">here,</span>
  <span m="774270">that</span> <span m="774390">means</span> <span m="774630">that</span>
  <span m="774750">I'm</span> <span m="775020">now</span> <span m="775180">in</span>
  <span m="775290">this</span> <span m="775500">box.</span> <span m="775770">And</span>
  <span m="775860">I</span> <span m="775890">have</span> <span m="776010">a</span>
  <span m="776070">new</span> <span m="776280">set</span> <span m="776520">of</span>
  <span m="776610">actions</span> <span m="777210">available</span> <span m="777570">to</span>
  <span m="777780">me</span> <span m="777960">for</span> <span m="778140">the</span>
  <span m="778230">next</span> <span m="779370">round,</span> <span m="779790">depending</span>
  <span m="780150">on</span> <span m="780240">what</span> <span m="780390">the</span>
  <span m="780690">red</span> <span m="780870">player</span> <span m="781140">does.</span>
  <span m="782950">So</span> <span m="783000">we</span> <span m="783090">have</span>
  <span m="783210">the</span> <span m="783270">state,</span> <span m="783750">we</span>
  <span m="783850">have</span> <span m="783950">the</span> <span m="783990">actions,</span>
  <span m="784470">and</span> <span m="784560">we</span> <span m="784620">have</span>
  <span m="784740">the</span> <span m="784800">next</span> <span m="785100">state,</span>
  <span m="785310">essentially--</span> <span m="785550">we</span> <span m="785610">have</span>
  <span m="785700">a</span> <span m="785730">trajectory</span> <span m="786390">or</span>
  <span m="786660">a</span> <span m="786930">transition</span> <span m="787500">of</span>
  <span m="787590">states.</span></p><p><span m="788330">And</span> <span m="788460">the</span>
  <span m="788520">last</span> <span m="788700">quantity</span> <span m="789060">that</span>
  <span m="789180">we</span> <span m="789300">need</span> <span m="789630">is</span>
  <span m="789780">the</span> <span m="789870">notion</span> <span m="790200">of</span>
  <span m="790290">a</span> <span m="790350">reward.</span> <span m="791280">That's</span>
  <span m="791550">very</span> <span m="791790">important</span> <span m="792120">for</span>
  <span m="792240">reinforcement</span> <span m="792750">learning,</span> <span m="792990">because</span>
  <span m="793290">that's</span> <span m="793590">what's</span> <span m="793860">driving</span>
  <span m="794290">the</span> <span m="794370">learning</span> <span m="794670">itself.</span>
  <span m="795420">We</span> <span m="795540">strive</span> <span m="795930">to</span>
  <span m="796050">optimize</span> <span m="796530">the</span> <span m="796590">reward</span>
  <span m="797130">or</span> <span m="797220">the</span> <span m="797340">outcome</span>
  <span m="797730">of</span> <span m="797820">something.</span></p><p><span m="799390">So</span>
  <span m="799530">if</span> <span m="799680">we</span> <span m="799770">look</span>
  <span m="799950">at</span> <span m="800040">the</span> <span m="800160">action</span>
  <span m="801140">to</span> <span m="801300">the</span> <span m="801450">farthest</span>
  <span m="801870">right</span> <span m="802200">here,</span> <span m="802410">essentially</span>
  <span m="802950">I</span> <span m="803550">left</span> <span m="803730">myself</span>
  <span m="804180">open</span> <span m="804540">to</span> <span m="804660">an</span>
  <span m="804750">attack</span> <span m="805050">by</span> <span m="805140">the</span>
  <span m="805230">red</span> <span m="805410">player</span> <span m="805710">here,</span>
  <span m="805950">because</span> <span m="806190">I</span> <span m="806280">didn't</span>
  <span m="806640">put</span> <span m="806820">my</span> <span m="806940">cross</span>
  <span m="807240">there.</span> <span m="808050">Which</span> <span m="808230">means</span>
  <span m="808470">that,</span> <span m="808590">probably,</span> <span m="809130">if</span>
  <span m="809250">the</span> <span m="809340">red</span> <span m="809490">player</span>
  <span m="809730">is</span> <span m="809850">decent,</span> <span m="810630">he</span>
  <span m="810720">will</span> <span m="810810">put</span> <span m="810980">his</span>
  <span m="811080">circle</span> <span m="811560">here</span> <span m="812220">and</span>
  <span m="812370">I</span> <span m="812460">will</span> <span m="813120">incur</span>
  <span m="813390">a</span> <span m="813450">loss,</span> <span m="814050">essentially.</span>
  <span m="815070">So</span> <span m="815280">my</span> <span m="815460">reward</span>
  <span m="815910">will</span> <span m="816030">be</span> <span m="816180">negative,</span>
  <span m="816930">if</span> <span m="817050">we</span> <span m="817140">take</span>
  <span m="817320">positive</span> <span m="817710">to</span> <span m="817830">be</span>
  <span m="817980">good.</span> <span m="818550">And</span> <span m="818640">this</span>
  <span m="818790">is</span> <span m="818850">something</span> <span m="819120">that</span>
  <span m="819240">I</span> <span m="819300">can</span> <span m="819480">learn</span>
  <span m="819780">from</span> <span m="820410">going</span> <span m="820710">forward.</span></p><p><span
  m="821430">Essentially,</span> <span m="821850">what</span> <span m="822000">I</span>
  <span m="822090">want</span> <span m="822240">to</span> <span m="822360">avoid</span>
  <span m="822750">is</span> <span m="822900">ending</span> <span m="823170">up</span>
  <span m="823290">in</span> <span m="823380">this</span> <span m="823470">state</span>
  <span m="823740">that's</span> <span m="823950">shown</span> <span m="824220">in</span>
  <span m="824310">the</span> <span m="824640">bottom</span> <span m="824970">right</span>
  <span m="825240">here.</span> <span m="826470">This</span> <span m="826650">is</span>
  <span m="826760">the</span> <span m="828120">basic</span> <span m="828510">idea</span>
  <span m="828780">of</span> <span m="829320">reinforcement</span> <span m="829830">learning</span>
  <span m="830310">for</span> <span m="830670">video games</span> <span m="831210">and</span>
  <span m="831300">for</span> <span m="831420">anything</span> <span m="831750">else.</span>
  <span m="834160">So</span> <span m="834300">if</span> <span m="834420">we</span>
  <span m="834510">take</span> <span m="834750">this</span> <span m="835020">board</span>
  <span m="835290">analogy</span> <span m="835740">or</span> <span m="835980">this</span>
  <span m="836520">example</span> <span m="837060">and</span> <span m="837480">move</span>
  <span m="837750">to</span> <span m="837900">the</span> <span m="838050">health</span>
  <span m="838270">care</span> <span m="838440">setting,</span> <span m="839290">we</span>
  <span m="839310">can</span> <span m="839430">think</span> <span m="839640">of</span>
  <span m="839730">the</span> <span m="839820">state</span> <span m="840120">of</span>
  <span m="840210">a</span> <span m="840300">patient</span> <span m="842220">as</span>
  <span m="842550">the</span> <span m="842670">game</span> <span m="843030">board</span>
  <span m="843870">or</span> <span m="844050">the</span> <span m="844560">state</span>
  <span m="844800">of</span> <span m="844860">the</span> <span m="844920">game.</span>
  <span m="846120">We</span> <span m="846270">will</span> <span m="846720">always</span>
  <span m="847020">call</span> <span m="847200">this</span> <span m="847590">St</span>
  <span m="848280">in</span> <span m="848430">this</span> <span m="848580">talk.</span>
  <span m="849960">The</span> <span m="850530">treatments</span> <span m="851010">that</span>
  <span m="851100">we</span> <span m="851190">prescribe</span> <span m="851640">or</span>
  <span m="851730">interventions</span> <span m="852660">will</span> <span m="852780">be</span>
  <span m="852930">At.</span> <span m="854170">And</span> <span m="854340">these</span>
  <span m="854490">are</span> <span m="854580">like</span> <span m="854730">the</span>
  <span m="854820">actions</span> <span m="855120">in</span> <span m="855210">the</span>
  <span m="855330">game,</span> <span m="855640">obviously.</span></p><p><span m="856440">The</span>
  <span m="856620">outcomes</span> <span m="857040">of</span> <span m="857130">a</span>
  <span m="857190">patient--</span> <span m="857580">could</span> <span m="857730">be</span>
  <span m="857820">mortality,</span> <span m="858480">could</span> <span m="858660">be</span>
  <span m="859200">managing</span> <span m="859650">vitals--</span> <span m="860330">will</span>
  <span m="860460">be</span> <span m="860580">as</span> <span m="861060">the</span>
  <span m="861210">rewards</span> <span m="861690">in</span> <span m="861750">the</span>
  <span m="861840">game,</span> <span m="862210">having</span> <span m="862380">lost</span>
  <span m="862770">or</span> <span m="862830">won.</span> <span m="864540">And</span>
  <span m="864660">then</span> <span m="864840">up</span> <span m="865050">at</span>
  <span m="865140">the</span> <span m="865230">end</span> <span m="865350">here,</span>
  <span m="865500">what</span> <span m="865620">could</span> <span m="865740">possibly</span>
  <span m="866190">go</span> <span m="866370">wrong.</span> <span m="867340">Well,</span>
  <span m="868350">as</span> <span m="868470">I</span> <span m="868560">alluded</span>
  <span m="868800">to</span> <span m="868920">before,</span> <span m="869310">health</span>
  <span m="869640">is</span> <span m="869760">not</span> <span m="870030">a</span>
  <span m="870060">game</span> <span m="870420">in</span> <span m="870480">the</span>
  <span m="870570">same</span> <span m="870900">sense</span> <span m="871290">that</span>
  <span m="871560">a</span> <span m="871620">video game</span> <span m="872070">is</span>
  <span m="872190">a</span> <span m="872250">game.</span> <span m="873840">But</span>
  <span m="874020">they</span> <span m="874110">share</span> <span m="874320">a</span>
  <span m="874380">lot</span> <span m="874560">of</span> <span m="874650">mathematical</span>
  <span m="875190">structure.</span> <span m="875860">So</span> <span m="876030">that's</span>
  <span m="876210">why</span> <span m="876330">I</span> <span m="876360">make</span>
  <span m="876570">the</span> <span m="876630">analogy</span> <span m="877020">here.</span></p><p><span
  m="878630">These</span> <span m="879020">quantities</span> <span m="879860">here--</span>
  <span m="880280">S,</span> <span m="880640">A,</span> <span m="881090">and</span>
  <span m="881510">R--</span> <span m="883190">will</span> <span m="883340">form</span>
  <span m="884030">something</span> <span m="884390">called</span> <span m="884780">a</span>
  <span m="884840">decision</span> <span m="885320">process.</span> <span m="887120">And</span>
  <span m="887240">that's</span> <span m="887390">what</span> <span m="887480">we'll</span>
  <span m="887630">talk</span> <span m="887810">about</span> <span m="888020">next.</span>
  <span m="888470">This</span> <span m="888680">is</span> <span m="888800">the</span>
  <span m="888950">outline</span> <span m="889310">for</span> <span m="889490">today</span>
  <span m="889940">and</span> <span m="890120">Thursday.</span> <span m="892310">I</span>
  <span m="892610">won't</span> <span m="892940">get to</span> <span m="893150">this</span>
  <span m="893540">today,</span> <span m="894140">but</span> <span m="894380">this</span>
  <span m="894570">is</span> <span m="894800">the</span> <span m="895010">talks</span>
  <span m="895160">we're</span> <span m="895580">considering.</span></p><p><span m="896810">So</span>
  <span m="897730">a</span> <span m="897800">decision</span> <span m="898160">process</span>
  <span m="898610">is</span> <span m="898700">essentially</span> <span m="899300">the</span>
  <span m="899990">world</span> <span m="901100">that</span> <span m="901250">describes</span>
  <span m="901640">the</span> <span m="901730">data</span> <span m="902060">that</span>
  <span m="902180">we</span> <span m="902300">access</span> <span m="902690">or</span>
  <span m="902810">the</span> <span m="903440">world</span> <span m="903710">that</span>
  <span m="904470">we're</span> <span m="905210">managing</span> <span m="905750">our</span>
  <span m="905840">agent</span> <span m="906290">in.</span> <span m="909920">Very</span>
  <span m="910250">often,</span> <span m="910550">if</span> <span m="910670">you've</span>
  <span m="911270">ever</span> <span m="911510">seen</span> <span m="911720">reinforcement</span>
  <span m="912290">learning</span> <span m="912560">taught,</span> <span m="913460">you</span>
  <span m="913670">have</span> <span m="913790">seen</span> <span m="913970">this</span>
  <span m="914120">picture</span> <span m="914480">in</span> <span m="914630">some</span>
  <span m="914900">form,</span> <span m="915350">usually.</span> <span m="916100">Sometimes</span>
  <span m="916460">there's</span> <span m="916680">a</span> <span m="916770">mouse</span>
  <span m="917150">and</span> <span m="917240">some</span> <span m="917390">cheese</span>
  <span m="917870">and</span> <span m="917960">there's</span> <span m="918410">other</span>
  <span m="918590">things</span> <span m="918830">going</span> <span m="919070">on,</span>
  <span m="919370">but</span> <span m="920180">you</span> <span m="920270">know</span>
  <span m="920390">what</span> <span m="920480">I'm</span> <span m="920540">talking</span>
  <span m="921200">about.</span> <span m="923530">But</span> <span m="923750">there</span>
  <span m="923860">are</span> <span m="923930">the</span> <span m="924020">same</span>
  <span m="924290">basic</span> <span m="924560">components.</span></p><p><span m="925170">So</span>
  <span m="926810">there's</span> <span m="927020">the</span> <span m="927080">concept</span>
  <span m="927350">of</span> <span m="927470">an</span> <span m="927560">agent--</span>
  <span m="928490">let's</span> <span m="928700">think</span> <span m="928940">doctor</span>
  <span m="929420">for</span> <span m="929540">now--</span> <span m="930410">that</span>
  <span m="930560">takes</span> <span m="930890">actions</span> <span m="931310">repeatedly</span>
  <span m="932000">over</span> <span m="932180">time.</span> <span m="932540">So</span>
  <span m="932660">this</span> <span m="932870">t</span> <span m="933170">here</span>
  <span m="934190">indicates</span> <span m="934760">an</span> <span m="934910">index</span>
  <span m="935270">of</span> <span m="935360">time</span> <span m="935990">and</span>
  <span m="936170">we</span> <span m="936470">see</span> <span m="936670">that</span>
  <span m="936950">essentially</span> <span m="937400">increasing</span> <span m="937940">as</span>
  <span m="938030">we</span> <span m="938120">spin</span> <span m="938420">around</span>
  <span m="938890">this</span> <span m="939050">wheel</span> <span m="939240">here.</span>
  <span m="940010">We</span> <span m="940250">move</span> <span m="940400">forward</span>
  <span m="940730">in</span> <span m="940820">time.</span> <span m="941690">So</span>
  <span m="941780">an</span> <span m="941900">agent</span> <span m="942170">takes</span>
  <span m="942410">an</span> <span m="942500">action</span> <span m="943870">and,</span>
  <span m="944030">at</span> <span m="944120">any</span> <span m="944280">time</span>
  <span m="944630">point,</span> <span m="944870">receives</span> <span m="945230">a</span>
  <span m="945350">reward</span> <span m="946310">for</span> <span m="946460">that</span>
  <span m="946700">action.</span> <span m="947210">And</span> <span m="947330">that</span>
  <span m="947420">would</span> <span m="947510">be</span> <span m="947630">Rt,</span>
  <span m="947970">as</span> <span m="948110">I</span> <span m="948170">said</span>
  <span m="948290">before.</span> <span m="949190">The</span> <span m="949310">environment</span>
  <span m="950660">is</span> <span m="950810">responsible</span> <span m="951440">for</span>
  <span m="951560">giving</span> <span m="951830">that</span> <span m="951980">reward.</span></p><p><span
  m="952560">So</span> <span m="952670">for</span> <span m="952820">example,</span>
  <span m="953370">if</span> <span m="953390">I'm</span> <span m="953510">the</span>
  <span m="953600">doctor,</span> <span m="954020">I'm</span> <span m="954140">the</span>
  <span m="954260">agent,</span> <span m="955750">I</span> <span m="956330">make</span>
  <span m="956570">an</span> <span m="956660">action</span> <span m="957080">or</span>
  <span m="957200">an</span> <span m="957290">intervention</span> <span m="957830">to</span>
  <span m="957950">my</span> <span m="958070">patient,</span> <span m="958790">the</span>
  <span m="958850">patient</span> <span m="959300">will</span> <span m="959420">be</span>
  <span m="959570">the</span> <span m="959660">environment.</span> <span m="960620">And</span>
  <span m="960740">essentially,</span> <span m="961060">responses</span> <span m="961630">do</span>
  <span m="961880">not</span> <span m="962090">respond</span> <span m="962480">to</span>
  <span m="962570">my</span> <span m="962720">intervention.</span> <span m="965200">The</span>
  <span m="965320">state</span> <span m="965710">here</span> <span m="966820">is</span>
  <span m="966940">the</span> <span m="967030">state</span> <span m="967300">of</span>
  <span m="967390">the</span> <span m="967450">patient,</span> <span m="967780">as</span>
  <span m="967870">I</span> <span m="967930">mentioned</span> <span m="968170">before,</span>
  <span m="968470">for</span> <span m="968590">example.</span> <span m="969730">But</span>
  <span m="969880">it</span> <span m="969940">might</span> <span m="970090">also</span>
  <span m="970390">be</span> <span m="971410">a</span> <span m="971500">state</span>
  <span m="972340">more</span> <span m="972730">broadly</span> <span m="973180">than</span>
  <span m="973330">the</span> <span m="973420">patient,</span> <span m="973780">like</span>
  <span m="974080">the</span> <span m="975310">settings</span> <span m="975790">of</span>
  <span m="975910">the</span> <span m="975970">machine</span> <span m="976450">that</span>
  <span m="976590">they're</span> <span m="976840">attached</span> <span m="977260">to</span>
  <span m="977590">or</span> <span m="977930">the</span> <span m="978280">availability</span>
  <span m="979100">of</span> <span m="980410">certain</span> <span m="980710">drugs</span>
  <span m="981040">in</span> <span m="981130">the</span> <span m="981190">hospital</span>
  <span m="981610">or</span> <span m="981700">something</span> <span m="982000">like</span>
  <span m="982150">that.</span> <span m="982970">So</span> <span m="983070">we</span>
  <span m="983170">can</span> <span m="983270">think</span> <span m="983320">a</span>
  <span m="983380">little</span> <span m="983560">bit</span> <span m="983710">more</span>
  <span m="983860">broadly</span> <span m="984310">around the</span> <span m="984370">patient,</span>
  <span m="984640">too.</span></p><p><span m="986170">I</span> <span m="986440">said</span>
  <span m="986770">partially</span> <span m="987400">observed</span> <span m="987820">here,</span>
  <span m="988030">in</span> <span m="988180">that</span> <span m="988360">I</span>
  <span m="988480">might</span> <span m="988750">not</span> <span m="988930">actually</span>
  <span m="989320">know</span> <span m="989650">everything</span> <span m="990040">about</span>
  <span m="990220">the</span> <span m="990280">patient</span> <span m="990610">that's</span>
  <span m="990820">relevant</span> <span m="991180">to</span> <span m="991330">me.</span>
  <span m="991540">And</span> <span m="991660">we will</span> <span m="991840">come</span>
  <span m="991990">back</span> <span m="992200">a</span> <span m="992260">little</span>
  <span m="992380">bit</span> <span m="992500">later</span> <span m="992770">to</span>
  <span m="992920">that.</span> <span m="994420">So</span> <span m="995020">there</span>
  <span m="995290">are</span> <span m="995950">two</span> <span m="996160">different</span>
  <span m="996730">formalizations</span> <span m="997600">that</span> <span m="997690">are</span>
  <span m="997750">very</span> <span m="997930">close</span> <span m="998200">to</span>
  <span m="998260">each</span> <span m="998410">other,</span> <span m="999140">which</span>
  <span m="999280">is</span> <span m="999430">when</span> <span m="999610">you'd</span>
  <span m="999760">know</span> <span m="1000120">everything</span> <span m="1000510">about</span>
  <span m="1000750">s</span> <span m="1001010">and</span> <span m="1001330">when</span>
  <span m="1001530">you</span> <span m="1001650">don't.</span> <span m="1002360">We</span>
  <span m="1002680">will,</span> <span m="1003030">for</span> <span m="1003330">the</span>
  <span m="1003450">longest</span> <span m="1003780">part</span> <span m="1003990">of</span>
  <span m="1004050">this</span> <span m="1004230">talk,</span> <span m="1004550">focus</span>
  <span m="1004950">on</span> <span m="1005280">the way</span> <span m="1005490">I</span>
  <span m="1005640">know</span> <span m="1005880">everything</span> <span m="1006390">that</span>
  <span m="1006540">is</span> <span m="1006660">relevant</span> <span m="1007740">about</span>
  <span m="1007980">the</span> <span m="1008070">environment.</span></p><p><span m="1009640">OK,</span>
  <span m="1009870">to</span> <span m="1009960">make</span> <span m="1010140">this</span>
  <span m="1010320">all</span> <span m="1010560">a</span> <span m="1010650">bit</span>
  <span m="1010770">more</span> <span m="1010920">concrete,</span> <span m="1011650">I'll</span>
  <span m="1011730">return</span> <span m="1012030">to</span> <span m="1012120">the</span>
  <span m="1012210">picture</span> <span m="1012540">that</span> <span m="1012690">I</span>
  <span m="1012750">showed</span> <span m="1012990">you</span> <span m="1013050">before,</span>
  <span m="1014080">but</span> <span m="1014180">now</span> <span m="1014370">put</span>
  <span m="1014610">it</span> <span m="1014700">in</span> <span m="1014790">context</span>
  <span m="1015330">of</span> <span m="1015510">the</span> <span m="1015720">paper</span>
  <span m="1016080">that</span> <span m="1016230">you</span> <span m="1016380">read.</span>
  <span m="1017460">Was</span> <span m="1017640">that</span> <span m="1017790">the</span>
  <span m="1017880">compulsory</span> <span m="1018330">one?</span> <span m="1018450">The</span>
  <span m="1018540">mechanical</span> <span m="1018930">ventilation?</span> <span
  m="1021020">OK,</span> <span m="1021420">great.</span></p><p><span m="1023690">So</span>
  <span m="1024859">in</span> <span m="1024980">this</span> <span m="1025130">case,</span>
  <span m="1025710">they</span> <span m="1025880">had</span> <span m="1027770">an</span>
  <span m="1027890">interesting</span> <span m="1028369">reward</span> <span m="1028700">structure,</span>
  <span m="1029150">essentially.</span> <span m="1029569">The</span> <span m="1029690">thing</span>
  <span m="1029839">that</span> <span m="1029960">they</span> <span m="1030050">were</span>
  <span m="1030170">trying</span> <span m="1030380">to</span> <span m="1030470">optimize</span>
  <span m="1030980">was</span> <span m="1031130">the</span> <span m="1031190">reward</span>
  <span m="1031550">related</span> <span m="1031880">to</span> <span m="1032089">the</span>
  <span m="1032450">vitals</span> <span m="1033020">of</span> <span m="1033140">the</span>
  <span m="1033230">patient.</span> <span m="1033890">But</span> <span m="1034069">also</span>
  <span m="1035569">whether</span> <span m="1035900">they</span> <span m="1036079">were</span>
  <span m="1036230">kept</span> <span m="1036589">on</span> <span m="1036829">mechanical</span>
  <span m="1037250">ventilation</span> <span m="1037760">or</span> <span m="1037849">not.</span>
  <span m="1038270">And</span> <span m="1038390">the</span> <span m="1039050">idea</span>
  <span m="1039470">of</span> <span m="1039530">this</span> <span m="1039710">paper</span>
  <span m="1040040">is</span> <span m="1040250">that</span> <span m="1041510">you</span>
  <span m="1041690">don't</span> <span m="1041930">want</span> <span m="1042079">to</span>
  <span m="1042170">keep</span> <span m="1042440">a</span> <span m="1042500">patient</span>
  <span m="1043099">unnecessarily</span> <span m="1043880">on</span> <span m="1044000">mechanical</span>
  <span m="1044390">ventilation,</span> <span m="1045260">because</span> <span m="1045500">it</span>
  <span m="1045589">has</span> <span m="1045770">the</span> <span m="1045859">side</span>
  <span m="1046040">effects</span> <span m="1046310">that</span> <span m="1046400">we</span>
  <span m="1046490">talked</span> <span m="1046730">about</span> <span m="1046880">before.</span></p><p><span
  m="1049260">So</span> <span m="1049320">at</span> <span m="1049410">any</span> <span
  m="1049990">point</span> <span m="1050250">in</span> <span m="1050340">time,</span>
  <span m="1050760">essentially,</span> <span m="1051000">we</span> <span m="1051090">can</span>
  <span m="1051180">think</span> <span m="1051360">about</span> <span m="1051720">taking</span>
  <span m="1052230">a</span> <span m="1052320">patient</span> <span m="1052650">on</span>
  <span m="1053010">or</span> <span m="1053160">off--</span> <span m="1054330">and</span>
  <span m="1054510">also</span> <span m="1055650">dealing</span> <span m="1056010">with</span>
  <span m="1056160">the</span> <span m="1056490">sedatives</span> <span m="1057690">that</span>
  <span m="1057840">are</span> <span m="1057930">prescribed</span> <span m="1058350">to</span>
  <span m="1058470">them.</span> <span m="1060490">So</span> <span m="1060690">in</span>
  <span m="1060810">this</span> <span m="1061200">example,</span> <span m="1062170">the</span>
  <span m="1062270">state</span> <span m="1063210">that</span> <span m="1063360">they</span>
  <span m="1063510">considered</span> <span m="1064320">in</span> <span m="1066750">this</span>
  <span m="1066960">application</span> <span m="1067770">included</span> <span m="1068190">the</span>
  <span m="1068280">demographic</span> <span m="1069120">information</span> <span
  m="1069570">of</span> <span m="1069660">the</span> <span m="1069720">patient,</span>
  <span m="1070260">which</span> <span m="1070290">doesn't</span> <span m="1070530">really</span>
  <span m="1070740">change</span> <span m="1071040">over</span> <span m="1071220">time.</span>
  <span m="1072660">Their</span> <span m="1072810">physiological</span> <span m="1073470">measurements,</span>
  <span m="1074160">ventilator</span> <span m="1074700">settings,</span> <span m="1076080">consciousness</span>
  <span m="1076590">level,</span> <span m="1077670">the</span> <span m="1077790">dosages</span>
  <span m="1078390">of</span> <span m="1078510">the</span> <span m="1078570">sedatives</span>
  <span m="1079010">they</span> <span m="1079160">use,</span> <span m="1079410">which</span>
  <span m="1079950">could</span> <span m="1080130">be</span> <span m="1080970">an</span>
  <span m="1081120">action,</span> <span m="1081480">I</span> <span m="1081540">suppose--</span>
  <span m="1082740">and</span> <span m="1082980">a</span> <span m="1083010">number</span>
  <span m="1083430">of</span> <span m="1083580">other</span> <span m="1083730">things.</span>
  <span m="1084440">And</span> <span m="1084540">these</span> <span m="1084870">are</span>
  <span m="1085320">the</span> <span m="1086130">values</span> <span m="1086430">that</span>
  <span m="1086520">we</span> <span m="1086640">have</span> <span m="1086760">to</span>
  <span m="1086850">keep</span> <span m="1087030">track</span> <span m="1087960">of,</span>
  <span m="1088530">moving</span> <span m="1088860">forward</span> <span m="1089160">in</span>
  <span m="1089250">time.</span> <span m="1090840">The</span> <span m="1090990">actions</span>
  <span m="1091620">concretely</span> <span m="1093180">included</span> <span m="1094050">whether</span>
  <span m="1094290">to</span> <span m="1094380">intubate</span> <span m="1094860">or</span>
  <span m="1094970">extubate</span> <span m="1095400">the</span> <span m="1095490">patient,</span>
  <span m="1096210">as</span> <span m="1096360">well</span> <span m="1096600">as</span>
  <span m="1096720">the</span> <span m="1097020">administer</span> <span m="1097680">and</span>
  <span m="1098430">dosing</span> <span m="1099160">the</span> <span m="1099370">sedatives.</span></p><p><span
  m="1102370">So</span> <span m="1103180">this</span> <span m="1103390">is,</span>
  <span m="1103540">again,</span> <span m="1104000">an</span> <span m="1104020">example</span>
  <span m="1104470">of</span> <span m="1104790">a</span> <span m="1104860">so-called</span>
  <span m="1105220">decision</span> <span m="1105610">process.</span> <span m="1106180">And</span>
  <span m="1106270">essentially,</span> <span m="1108850">the</span> <span m="1109210">process</span>
  <span m="1109720">is</span> <span m="1109900">the</span> <span m="1110020">distribution</span>
  <span m="1110710">of</span> <span m="1110800">these</span> <span m="1111130">quantities</span>
  <span m="1111425">that</span> <span m="1111720">I've</span> <span m="1111880">been</span>
  <span m="1112000">talking</span> <span m="1112240">about</span> <span m="1112480">over</span>
  <span m="1112650">time.</span> <span m="1113170">So</span> <span m="1113350">we</span>
  <span m="1113500">have</span> <span m="1114160">the</span> <span m="1114250">states,</span>
  <span m="1114760">the</span> <span m="1114880">actions,</span> <span m="1115240">and</span>
  <span m="1115360">the</span> <span m="1115420">rewards.</span> <span m="1115960">They</span>
  <span m="1116170">all</span> <span m="1116470">traverse</span> <span m="1117370">or</span>
  <span m="1117490">they</span> <span m="1117610">all</span> <span m="1118120">evolve</span>
  <span m="1118570">over</span> <span m="1118720">time.</span> <span m="1119440">And</span>
  <span m="1119610">the</span> <span m="1120250">loss</span> <span m="1120610">of</span>
  <span m="1120730">how</span> <span m="1121000">that</span> <span m="1121300">happens</span>
  <span m="1121960">is</span> <span m="1122110">the</span> <span m="1122170">decision</span>
  <span m="1122530">process.</span></p><p><span m="1124300">I</span> <span m="1124360">mentioned</span>
  <span m="1124690">before</span> <span m="1125110">that</span> <span m="1125230">we</span>
  <span m="1125350">will</span> <span m="1125500">be</span> <span m="1125620">talking</span>
  <span m="1125830">about</span> <span m="1126010">policies</span> <span m="1127270">today.</span>
  <span m="1128320">And</span> <span m="1129460">typically,</span> <span m="1130840">there's</span>
  <span m="1131080">a</span> <span m="1131110">distinction</span> <span m="1131650">between</span>
  <span m="1132400">what</span> <span m="1132580">is</span> <span m="1132700">called</span>
  <span m="1132940">a</span> <span m="1133000">behavior</span> <span m="1133420">policy</span>
  <span m="1134320">and</span> <span m="1134440">a</span> <span m="1134500">target</span>
  <span m="1134860">policy--</span> <span m="1135340">or</span> <span m="1135520">there</span>
  <span m="1135640">are</span> <span m="1135790">different</span> <span m="1136120">words</span>
  <span m="1136330">for</span> <span m="1136480">this.</span> <span m="1137140">Essentially,</span>
  <span m="1137620">the</span> <span m="1137860">thing</span> <span m="1138130">that</span>
  <span m="1138250">we</span> <span m="1138370">observe</span> <span m="1138910">is</span>
  <span m="1139030">usually</span> <span m="1139300">called</span> <span m="1139510">a</span>
  <span m="1139540">behavior</span> <span m="1139930">policy.</span> <span m="1140740">By</span>
  <span m="1140920">that,</span> <span m="1141100">I</span> <span m="1141130">mean</span>
  <span m="1141400">if</span> <span m="1141580">we</span> <span m="1141970">go</span>
  <span m="1142240">to</span> <span m="1142330">a</span> <span m="1142360">hospital</span>
  <span m="1142780">and</span> <span m="1142870">watch</span> <span m="1143080">what's</span>
  <span m="1143620">happening</span> <span m="1144040">there</span> <span m="1144400">at</span>
  <span m="1144490">the</span> <span m="1144580">moment,</span> <span m="1145270">that</span>
  <span m="1145390">will</span> <span m="1145540">be</span> <span m="1145630">the</span>
  <span m="1145720">behavior</span> <span m="1146050">policy.</span> <span m="1146470">And</span>
  <span m="1146560">I</span> <span m="1146620">will</span> <span m="1146780">denote</span>
  <span m="1147000">that</span> <span m="1147180">mu.</span></p><p><span m="1148160">So</span>
  <span m="1148180">that</span> <span m="1148330">is</span> <span m="1148450">what</span>
  <span m="1148570">we</span> <span m="1148690">have</span> <span m="1148840">to</span>
  <span m="1148930">learn</span> <span m="1149230">from,</span> <span m="1149860">essentially.</span>
  <span m="1152630">So</span> <span m="1153110">decision</span> <span m="1153470">processes</span>
  <span m="1154520">so</span> <span m="1154730">far</span> <span m="1156320">are</span>
  <span m="1156920">incredibly</span> <span m="1157490">general.</span> <span m="1157850">I</span>
  <span m="1157910">haven't</span> <span m="1158150">said</span> <span m="1158360">anything</span>
  <span m="1158720">about</span> <span m="1158930">what</span> <span m="1159200">this</span>
  <span m="1159740">distribution</span> <span m="1160310">is</span> <span m="1160430">like,</span>
  <span m="1161150">but</span> <span m="1161630">the</span> <span m="1162140">absolutely</span>
  <span m="1162890">dominant</span> <span m="1164030">restriction</span> <span m="1164600">that</span>
  <span m="1164720">people</span> <span m="1164960">make</span> <span m="1165290">when</span>
  <span m="1165410">they</span> <span m="1165530">study</span> <span m="1165880">system</span>
  <span m="1166100">processes</span> <span m="1166880">is</span> <span m="1167000">to</span>
  <span m="1167090">look</span> <span m="1167390">at</span> <span m="1167790">Markov</span>
  <span m="1168140">decision</span> <span m="1168500">processes.</span> <span m="1169920">And</span>
  <span m="1169940">these</span> <span m="1170180">have</span> <span m="1170390">a</span>
  <span m="1170450">specific</span> <span m="1170990">conditional</span> <span m="1171500">independent</span>
  <span m="1172010">structure</span> <span m="1172400">that</span> <span m="1172550">I</span>
  <span m="1172640">will</span> <span m="1172820">illustrate</span> <span m="1173260">in</span>
  <span m="1173360">the</span> <span m="1173420">next</span> <span m="1173660">slide--</span>
  <span m="1173990">well,</span> <span m="1174110">I'll</span> <span m="1174170">just</span>
  <span m="1174380">define</span> <span m="1174740">it</span> <span m="1174800">mathematically</span>
  <span m="1175370">here.</span></p><p><span m="1176380">It</span> <span m="1176850">says,</span>
  <span m="1177110">essentially,</span> <span m="1177530">that</span> <span m="1177680">all</span>
  <span m="1177920">of</span> <span m="1178010">the</span> <span m="1178100">quantities</span>
  <span m="1178640">that</span> <span m="1178730">we</span> <span m="1178820">care</span>
  <span m="1179060">about--</span> <span m="1179450">the</span> <span m="1179990">states.</span>
  <span m="1180980">I</span> <span m="1181040">guess</span> <span m="1181190">that</span>
  <span m="1181350">should</span> <span m="1181510">say</span> <span m="1181630">state.</span>
  <span m="1182720">Rewards</span> <span m="1183170">and</span> <span m="1183260">the</span>
  <span m="1183380">actions</span> <span m="1184370">only</span> <span m="1184670">depend</span>
  <span m="1185060">on</span> <span m="1185150">the</span> <span m="1185210">most</span>
  <span m="1186080">recent</span> <span m="1186980">state</span> <span m="1187430">in</span>
  <span m="1187550">action.</span></p><p><span m="1191780">If</span> <span m="1191930">we</span>
  <span m="1192110">observe</span> <span m="1192650">an</span> <span m="1192740">action</span>
  <span m="1193190">taken</span> <span m="1193580">by</span> <span m="1194870">a</span>
  <span m="1194960">doctor</span> <span m="1195410">in</span> <span m="1195530">the</span>
  <span m="1195620">hospital,</span> <span m="1196160">for</span> <span m="1196280">example--</span>
  <span m="1197130">to</span> <span m="1197180">make</span> <span m="1197450">a</span>
  <span m="1197510">mark</span> <span m="1197780">of</span> <span m="1197870">assumption,</span>
  <span m="1199010">we'd</span> <span m="1199190">say</span> <span m="1199430">that</span>
  <span m="1199970">this</span> <span m="1200210">doctor</span> <span m="1200600">did</span>
  <span m="1200750">not</span> <span m="1201050">look</span> <span m="1201290">at</span>
  <span m="1201410">anything</span> <span m="1201830">that</span> <span m="1201950">happened</span>
  <span m="1203030">earlier</span> <span m="1203360">in</span> <span m="1203480">time</span>
  <span m="1203930">or</span> <span m="1204320">any</span> <span m="1204620">other</span>
  <span m="1204830">information</span> <span m="1205820">than</span> <span m="1206030">what</span>
  <span m="1206210">is</span> <span m="1206300">in</span> <span m="1206450">the</span>
  <span m="1206540">state</span> <span m="1206840">variable</span> <span m="1207200">that</span>
  <span m="1207320">we</span> <span m="1207410">observe</span> <span m="1207680">at</span>
  <span m="1207740">that</span> <span m="1207860">time.</span> <span m="1209240">That</span>
  <span m="1209390">is</span> <span m="1209510">the</span> <span m="1209600">assumption</span>
  <span m="1209960">that</span> <span m="1210050">we</span> <span m="1210110">make.</span>
  <span m="1210230">Yeah?</span></p><p><span m="1210700">AUDIENCE:</span> <span m="1210760">Is</span>
  <span m="1210820">that</span> <span m="1212620">an</span> <span m="1213540">assumption</span>
  <span m="1214100">you</span> <span m="1214190">can</span> <span m="1214360">make</span>
  <span m="1214670">for</span> <span m="1214910">a</span> <span m="1214970">health</span>
  <span m="1215190">care?</span> <span m="1215630">Because</span> <span m="1216175">in
  the end,</span> <span m="1217910">you</span> <span m="1218000">don't</span> <span
  m="1218390">have</span> <span m="1218720">access</span> <span m="1219110">to</span>
  <span m="1219250">the</span> <span m="1219320">real</span> <span m="1219530">state,</span>
  <span m="1219890">but</span> <span m="1220070">only</span> <span m="1220370">about</span>
  <span m="1220740">what's</span> <span m="1221390">measured</span> <span m="1221930">about</span>
  <span m="1222290">the</span> <span m="1222410">state</span> <span m="1222725">in</span>
  <span m="1223040">health</span> <span m="1223250">care.</span></p><p><span m="1223700">FREDRIK
  D. JOHANSSON:</span> <span m="1223760">It's</span> <span m="1223820">a</span> <span
  m="1223880">very</span> <span m="1224030">good</span> <span m="1224150">question.</span>
  <span m="1226340">So</span> <span m="1226640">the</span> <span m="1226970">nice</span>
  <span m="1227240">thing</span> <span m="1227420">in</span> <span m="1227510">terms</span>
  <span m="1227810">of</span> <span m="1228050">inferring</span> <span m="1229310">causal</span>
  <span m="1229670">quantities</span> <span m="1230330">is</span> <span m="1230480">that</span>
  <span m="1230600">we</span> <span m="1230750">only</span> <span m="1231020">need</span>
  <span m="1231230">the</span> <span m="1231320">things</span> <span m="1231680">that</span>
  <span m="1231890">were</span> <span m="1232010">used</span> <span m="1232250">to</span>
  <span m="1232340">make</span> <span m="1232490">the</span> <span m="1232580">decision</span>
  <span m="1233000">in</span> <span m="1233090">the</span> <span m="1233150">first</span>
  <span m="1233360">place.</span> <span m="1234210">So</span> <span m="1234260">the</span>
  <span m="1234350">doctor</span> <span m="1235340">can</span> <span m="1235520">only</span>
  <span m="1235820">act</span> <span m="1236090">on</span> <span m="1236180">such</span>
  <span m="1236390">information,</span> <span m="1236750">too.</span> <span m="1237530">Unless</span>
  <span m="1238400">we</span> <span m="1238550">don't</span> <span m="1238760">record</span>
  <span m="1239060">everything</span> <span m="1239360">that</span> <span m="1239480">the</span>
  <span m="1239540">doctor</span> <span m="1239840">knows--</span> <span m="1240140">which</span>
  <span m="1240320">is</span> <span m="1240440">also</span> <span m="1240650">the</span>
  <span m="1240740">case.</span> <span m="1240990">So</span> <span m="1241100">that</span>
  <span m="1241200">is</span> <span m="1241550">something</span> <span m="1241850">that</span>
  <span m="1241970">we</span> <span m="1242060">have</span> <span m="1242210">to</span>
  <span m="1242840">worry</span> <span m="1243050">about</span> <span m="1243230">for</span>
  <span m="1243380">sure.</span> <span m="1245300">Another</span> <span m="1245630">way</span>
  <span m="1245930">to</span> <span m="1246530">lose</span> <span m="1246980">information,</span>
  <span m="1247560">as</span> <span m="1247700">I</span> <span m="1247760">mentioned,</span>
  <span m="1248900">that</span> <span m="1249050">is</span> <span m="1249170">relevant</span>
  <span m="1249530">for</span> <span m="1249680">this</span> <span m="1250120">is</span>
  <span m="1250360">if</span> <span m="1250610">we</span> <span m="1251420">look</span>
  <span m="1251920">to--</span> <span m="1256700">What's</span> <span m="1256850">the</span>
  <span m="1256910">opposite</span> <span m="1257120">of</span> <span m="1257180">far?</span></p><p><span
  m="1258710">AUDIENCE:</span> <span m="1258855">Near.</span></p><p><span m="1259000">FREDRIK
  D. JOHANSSON:</span> <span m="1259075">Too</span> <span m="1259150">near</span>
  <span m="1259340">back</span> <span m="1259610">in</span> <span m="1259700">time,</span>
  <span m="1260030">essentially.</span> <span m="1261930">So</span> <span m="1261980">we</span>
  <span m="1262070">don't</span> <span m="1262250">look</span> <span m="1262430">at</span>
  <span m="1262490">the</span> <span m="1262640">entire</span> <span m="1262970">history</span>
  <span m="1263240">of</span> <span m="1263300">the</span> <span m="1263390">patient.</span>
  <span m="1264270">And</span> <span m="1264590">when</span> <span m="1264710">I</span>
  <span m="1264770">say</span> <span m="1265040">St</span> <span m="1265610">here,</span>
  <span m="1267450">it</span> <span m="1267470">doesn't</span> <span m="1267710">have</span>
  <span m="1267860">to</span> <span m="1267950">be</span> <span m="1268970">the</span>
  <span m="1269390">instantaneous</span> <span m="1272060">snapshot</span> <span m="1272690">of</span>
  <span m="1272780">a</span> <span m="1272840">patient.</span> <span m="1273170">We</span>
  <span m="1273230">can</span> <span m="1273380">also</span> <span m="1273560">Include</span>
  <span m="1273830">history</span> <span m="1274220">there.</span> <span m="1274530">Again,</span>
  <span m="1274920">we'll</span> <span m="1275230">come</span> <span m="1275360">back</span>
  <span m="1275510">to</span> <span m="1275570">that</span> <span m="1275740">a</span>
  <span m="1275870">little</span> <span m="1275960">later.</span></p><p><span m="1280350">OK,</span>
  <span m="1280760">so</span> <span m="1281050">the</span> <span m="1281180">Markov</span>
  <span m="1281460">assumption</span> <span m="1281880">essentially</span> <span m="1283020">looks</span>
  <span m="1283290">like</span> <span m="1283470">this.</span> <span m="1284890">Or</span>
  <span m="1285180">this</span> <span m="1285330">is</span> <span m="1285810">how</span>
  <span m="1286020">I</span> <span m="1286110">will</span> <span m="1286290">illustrate,</span>
  <span m="1286730">anyway.</span> <span m="1287100">We</span> <span m="1287220">have</span>
  <span m="1287700">a</span> <span m="1287760">sequence</span> <span m="1288150">of</span>
  <span m="1288210">states</span> <span m="1288600">here</span> <span m="1289260">that</span>
  <span m="1289380">evolve</span> <span m="1289770">over</span> <span m="1289920">time.</span>
  <span m="1290620">I'm</span> <span m="1290980">allowing</span> <span m="1291300">myself</span>
  <span m="1291600">to</span> <span m="1291690">put</span> <span m="1291840">some</span>
  <span m="1292020">dots</span> <span m="1292320">here,</span> <span m="1292470">because</span>
  <span m="1292680">I</span> <span m="1292790">don't</span> <span m="1292920">want
  to</span> <span m="1293250">draw</span> <span m="1293640">forever.</span> <span
  m="1295450">But</span> <span m="1295710">essentially,</span> <span m="1296040">you</span>
  <span m="1296100">could</span> <span m="1296190">think</span> <span m="1296370">of</span>
  <span m="1296460">this</span> <span m="1296670">pattern</span> <span m="1297120">repeating--</span>
  <span m="1297630">where</span> <span m="1298050">the</span> <span m="1298200">previous</span>
  <span m="1298590">state</span> <span m="1298950">goes</span> <span m="1299220">into</span>
  <span m="1299460">the</span> <span m="1299550">next</span> <span m="1299790">state,</span>
  <span m="1300570">the</span> <span m="1300750">action</span> <span m="1301170">goes</span>
  <span m="1301410">into</span> <span m="1301680">the</span> <span m="1301770">next</span>
  <span m="1301980">state,</span> <span m="1302460">and</span> <span m="1302670">the</span>
  <span m="1302820">action</span> <span m="1303180">and</span> <span m="1303330">state</span>
  <span m="1303630">goes</span> <span m="1303930">in through</span> <span m="1304110">the</span>
  <span m="1304290">reward.</span></p><p><span m="1305320">This</span> <span m="1305370">is</span>
  <span m="1305490">the</span> <span m="1305640">world</span> <span m="1305910">that</span>
  <span m="1306000">we</span> <span m="1306120">will</span> <span m="1306300">live</span>
  <span m="1306480">in</span> <span m="1306570">for</span> <span m="1306690">this</span>
  <span m="1306870">lecture.</span> <span m="1308160">Something</span> <span m="1308520">that's</span>
  <span m="1308760">not</span> <span m="1309120">allowed</span> <span m="1309840">under</span>
  <span m="1310050">the</span> <span m="1310140">mark</span> <span m="1310370">of</span>
  <span m="1310470">assumption</span> <span m="1310950">is</span> <span m="1311370">an</span>
  <span m="1311730">edge</span> <span m="1311940">like</span> <span m="1312180">this,</span>
  <span m="1312640">which</span> <span m="1312720">says</span> <span m="1312930">that</span>
  <span m="1313410">an</span> <span m="1313650">action</span> <span m="1313990">at</span>
  <span m="1314090">an</span> <span m="1314160">early</span> <span m="1314430">time</span>
  <span m="1315230">influences</span> <span m="1315650">an</span> <span m="1315780">action</span>
  <span m="1316080">at</span> <span m="1316170">a</span> <span m="1316230">later</span>
  <span m="1316470">time.</span> <span m="1318150">And</span> <span m="1318450">specifically,</span>
  <span m="1320190">it</span> <span m="1320430">can't</span> <span m="1320790">do</span>
  <span m="1321030">so</span> <span m="1321570">without</span> <span m="1321990">passing</span>
  <span m="1322500">through</span> <span m="1322980">a</span> <span m="1323040">state,</span>
  <span m="1323620">for</span> <span m="1323720">example.</span> <span m="1324360">It</span>
  <span m="1324900">very</span> <span m="1325410">well</span> <span m="1325680">can</span>
  <span m="1325830">have</span> <span m="1325950">an</span> <span m="1326040">influence</span>
  <span m="1326670">on</span> <span m="1326820">At</span> <span m="1327570">by</span>
  <span m="1328050">this</span> <span m="1328440">trajectory</span> <span m="1329070">here,</span>
  <span m="1330120">but</span> <span m="1330300">not</span> <span m="1330510">directly.</span>
  <span m="1331280">That</span> <span m="1331510">that's</span> <span m="1331760">the</span>
  <span m="1332070">Markov</span> <span m="1332330">assumption</span> <span m="1332640">in</span>
  <span m="1332700">this</span> <span m="1332850">case.</span></p><p><span m="1338300">So</span>
  <span m="1339010">you</span> <span m="1339130">can</span> <span m="1339280">see</span>
  <span m="1339430">that</span> <span m="1340090">if</span> <span m="1340450">I</span>
  <span m="1340540">were</span> <span m="1340690">to</span> <span m="1340810">draw</span>
  <span m="1342310">the</span> <span m="1342430">graph</span> <span m="1342850">of</span>
  <span m="1342970">all</span> <span m="1343330">the</span> <span m="1343600">different</span>
  <span m="1344140">measurements</span> <span m="1344800">that</span> <span m="1347290">we</span>
  <span m="1348220">see</span> <span m="1349270">during</span> <span m="1349570">a</span>
  <span m="1349630">state,</span> <span m="1350320">essentially</span> <span m="1350920">there</span>
  <span m="1351100">are</span> <span m="1351250">a</span> <span m="1351340">lot</span>
  <span m="1351610">of</span> <span m="1351700">errors</span> <span m="1352090">that</span>
  <span m="1352250">I</span> <span m="1352750">could</span> <span m="1352960">have</span>
  <span m="1353080">had</span> <span m="1353290">in</span> <span m="1353410">this</span>
  <span m="1353830">picture</span> <span m="1354100">that</span> <span m="1354250">I</span>
  <span m="1354310">don't</span> <span m="1354550">have.</span> <span m="1355090">So</span>
  <span m="1355180">it</span> <span m="1355240">may</span> <span m="1355390">seem</span>
  <span m="1355660">that</span> <span m="1355780">the</span> <span m="1355850">Markov</span>
  <span m="1356140">assumption</span> <span m="1356620">is</span> <span m="1356710">a</span>
  <span m="1357170">very</span> <span m="1357280">strong</span> <span m="1357670">one,</span>
  <span m="1358600">but</span> <span m="1358780">one</span> <span m="1359020">way</span>
  <span m="1359200">to</span> <span m="1360200">ensure</span> <span m="1361000">that</span>
  <span m="1361120">the</span> <span m="1361180">Markov</span> <span m="1361420">assumption</span>
  <span m="1361750">is</span> <span m="1361810">more</span> <span m="1362020">likely</span>
  <span m="1362410">is</span> <span m="1362560">to</span> <span m="1362650">include</span>
  <span m="1362950">more</span> <span m="1363100">things</span> <span m="1363370">in</span>
  <span m="1363460">your</span> <span m="1363580">state,</span> <span m="1364010">including</span>
  <span m="1364600">summaries</span> <span m="1364960">of</span> <span m="1365050">the</span>
  <span m="1365110">history,</span> <span m="1365450">et</span> <span m="1365620">cetera,</span>
  <span m="1366240">that</span> <span m="1366490">I</span> <span m="1366790">mentioned</span>
  <span m="1367090">before.</span> <span m="1368810">An</span> <span m="1368960">even</span>
  <span m="1369170">stronger</span> <span m="1370670">restriction</span> <span m="1371360">of</span>
  <span m="1371540">decision</span> <span m="1371900">processes</span> <span m="1372500">is</span>
  <span m="1372650">to</span> <span m="1372770">assume</span> <span m="1373160">that</span>
  <span m="1373790">the</span> <span m="1373880">states</span> <span m="1374810">over</span>
  <span m="1375020">time</span> <span m="1375590">are</span> <span m="1375980">themselves</span>
  <span m="1376700">independent.</span></p><p><span m="1378350">So</span> <span m="1379760">this</span>
  <span m="1380030">goes</span> <span m="1380300">by</span> <span m="1380450">different</span>
  <span m="1380720">names--</span> <span m="1381530">sometimes</span> <span m="1381980">under</span>
  <span m="1382190">the</span> <span m="1382280">name</span> <span m="1382460">contextual</span>
  <span m="1382970">bandits.</span> <span m="1384350">But</span> <span m="1384770">the</span>
  <span m="1385060">bandits</span> <span m="1385790">part</span> <span m="1386060">of</span>
  <span m="1386150">that</span> <span m="1386360">itself</span> <span m="1386720">is</span>
  <span m="1386810">not</span> <span m="1386930">so</span> <span m="1387050">relevant</span>
  <span m="1387410">here.</span> <span m="1387590">So</span> <span m="1387800">let's</span>
  <span m="1388070">not</span> <span m="1388280">go</span> <span m="1388370">into</span>
  <span m="1388580">that</span> <span m="1388730">name</span> <span m="1389090">too</span>
  <span m="1389240">much.</span> <span m="1390380">But</span> <span m="1390530">essentially,</span>
  <span m="1390920">what</span> <span m="1391040">we</span> <span m="1391130">can</span>
  <span m="1391250">say</span> <span m="1391460">is</span> <span m="1391580">here,</span>
  <span m="1392240">the</span> <span m="1392600">state</span> <span m="1393020">at</span>
  <span m="1393170">a</span> <span m="1393200">later</span> <span m="1393530">time</span>
  <span m="1393800">point</span> <span m="1394010">is</span> <span m="1394160">not</span>
  <span m="1394460">influenced</span> <span m="1394850">directly</span> <span m="1395300">by</span>
  <span m="1395450">the</span> <span m="1395540">state</span> <span m="1395810">at</span>
  <span m="1395900">a</span> <span m="1395960">previous</span> <span m="1396290">time</span>
  <span m="1396470">point,</span> <span m="1396890">nor</span> <span m="1397220">the</span>
  <span m="1397460">action</span> <span m="1397940">of the</span> <span m="1398030">previous</span>
  <span m="1398360">time</span> <span m="1398540">point.</span></p><p><span m="1399620">So</span>
  <span m="1400430">if</span> <span m="1400550">you</span> <span m="1400640">remember</span>
  <span m="1401570">what</span> <span m="1401730">you</span> <span m="1401870">did</span>
  <span m="1402020">last</span> <span m="1402410">week,</span> <span m="1402950">this</span>
  <span m="1403280">looks</span> <span m="1403580">like</span> <span m="1404060">basically</span>
  <span m="1404480">T</span> <span m="1404840">repetitions</span> <span m="1405710">of</span>
  <span m="1405830">the</span> <span m="1405920">very</span> <span m="1406130">simple</span>
  <span m="1406430">graph</span> <span m="1406760">that</span> <span m="1406910">we</span>
  <span m="1407000">had</span> <span m="1407210">for</span> <span m="1407600">estimating</span>
  <span m="1407960">potential</span> <span m="1408290">outcomes.</span> <span m="1409250">And</span>
  <span m="1409340">that</span> <span m="1409460">is</span> <span m="1409670">indeed</span>
  <span m="1410420">mathematically</span> <span m="1410990">equivalent.</span> <span
  m="1411740">If</span> <span m="1411890">we</span> <span m="1412010">assume</span>
  <span m="1412370">that</span> <span m="1412550">this</span> <span m="1415200">S</span>
  <span m="1415540">here</span> <span m="1416520">represents</span> <span m="1417390">the</span>
  <span m="1417480">state</span> <span m="1417780">of</span> <span m="1417960">a</span>
  <span m="1418110">patient</span> <span m="1419000">and</span> <span m="1419130">all</span>
  <span m="1419280">patients</span> <span m="1419730">are</span> <span m="1419820">drawn</span>
  <span m="1420180">from</span> <span m="1420360">some</span> <span m="1421550">sum</span>
  <span m="1421920">process,</span> <span m="1422640">essentially.</span> <span m="1423360">So</span>
  <span m="1423540">that</span> <span m="1423930">S0,</span> <span m="1425160">1,</span>
  <span m="1425580">et</span> <span m="1425830">cetera,</span> <span m="1426590">up</span>
  <span m="1426750">to</span> <span m="1426870">St</span> <span m="1427740">are</span>
  <span m="1427890">all</span> <span m="1428070">i.i.d.</span> <span m="1428550">draws</span>
  <span m="1428970">of</span> <span m="1429060">the</span> <span m="1429150">same</span>
  <span m="1429450">distribution.</span></p><p><span m="1431490">Then</span> <span
  m="1431640">we</span> <span m="1431760">have,</span> <span m="1432030">essentially,</span>
  <span m="1432510">a</span> <span m="1433110">model</span> <span m="1433440">for</span>
  <span m="1434250">t</span> <span m="1434490">different</span> <span m="1434790">patients</span>
  <span m="1435870">with</span> <span m="1436160">a</span> <span m="1436350">single</span>
  <span m="1436800">time</span> <span m="1437220">step</span> <span m="1437970">or</span>
  <span m="1438090">single</span> <span m="1439170">action,</span> <span m="1440040">instead</span>
  <span m="1440430">of</span> <span m="1441970">them</span> <span m="1442170">being</span>
  <span m="1442410">dependent</span> <span m="1442800">in</span> <span m="1442860">some</span>
  <span m="1443060">way.</span> <span m="1443490">So</span> <span m="1443640">we</span>
  <span m="1443730">can</span> <span m="1443850">see</span> <span m="1444030">that</span>
  <span m="1444600">by</span> <span m="1446610">going</span> <span m="1446940">backwards</span>
  <span m="1447390">through</span> <span m="1447570">my</span> <span m="1447720">slides,</span>
  <span m="1448530">this</span> <span m="1448800">is</span> <span m="1448950">essentially</span>
  <span m="1449340">what</span> <span m="1449490">we</span> <span m="1449640">had</span>
  <span m="1449820">last</span> <span m="1450120">week.</span> <span m="1450720">And</span>
  <span m="1450870">we</span> <span m="1451350">just</span> <span m="1451620">have</span>
  <span m="1451770">to</span> <span m="1451890">add</span> <span m="1452160">more</span>
  <span m="1452430">arrows</span> <span m="1452820">to</span> <span m="1452940">get</span>
  <span m="1453090">to</span> <span m="1453240">whatever</span> <span m="1453870">we</span>
  <span m="1453990">have</span> <span m="1454170">this</span> <span m="1454380">week,</span>
  <span m="1454830">which</span> <span m="1455100">indicates</span> <span m="1455610">that</span>
  <span m="1456360">last</span> <span m="1456720">week</span> <span m="1456870">was</span>
  <span m="1456990">a</span> <span m="1457020">special</span> <span m="1457350">case</span>
  <span m="1457530">of</span> <span m="1457620">this--</span> <span m="1457790">just</span>
  <span m="1458000">as</span> <span m="1458070">David</span> <span m="1458310">said</span>
  <span m="1458460">before.</span> <span m="1460850">It</span> <span m="1460970">also</span>
  <span m="1461390">hints</span> <span m="1461780">at</span> <span m="1462980">the</span>
  <span m="1463160">reinforcement</span> <span m="1463640">learning</span> <span m="1463880">problem</span>
  <span m="1464210">being</span> <span m="1464360">more</span> <span m="1464570">complicated</span>
  <span m="1465770">than</span> <span m="1465920">the</span> <span m="1466010">potential</span>
  <span m="1466310">outcomes</span> <span m="1466610">problem.</span> <span m="1466940">And</span>
  <span m="1467120">we'll</span> <span m="1467630">see</span> <span m="1467780">more</span>
  <span m="1467900">examples</span> <span m="1468230">of</span> <span m="1468290">that</span>
  <span m="1468410">later.</span></p><p><span m="1470820">But,</span> <span m="1472760">like</span>
  <span m="1473120">with</span> <span m="1473780">causal</span> <span m="1474080">effect</span>
  <span m="1474290">estimation</span> <span m="1474740">that</span> <span m="1474860">we</span>
  <span m="1474950">did</span> <span m="1475070">last</span> <span m="1475340">week,</span>
  <span m="1475550">we're</span> <span m="1475700">interested</span> <span m="1476240">in</span>
  <span m="1476990">the</span> <span m="1477140">influences</span> <span m="1477710">of</span>
  <span m="1479210">just</span> <span m="1479690">a</span> <span m="1479750">few</span>
  <span m="1479960">variables,</span> <span m="1480410">essentially.</span> <span
  m="1480890">So</span> <span m="1481070">last</span> <span m="1481340">time</span>
  <span m="1481550">we</span> <span m="1481610">studied</span> <span m="1481930">the</span>
  <span m="1482030">effect</span> <span m="1482330">of</span> <span m="1482420">a</span>
  <span m="1482480">single</span> <span m="1482870">treatment</span> <span m="1483710">choice.</span>
  <span m="1484450">And</span> <span m="1484550">in</span> <span m="1484640">this</span>
  <span m="1484790">case,</span> <span m="1485160">we</span> <span m="1485260">will</span>
  <span m="1485270">study</span> <span m="1485660">the</span> <span m="1485840">influence</span>
  <span m="1486560">of</span> <span m="1486950">these</span> <span m="1487310">various</span>
  <span m="1487790">actions</span> <span m="1488210">that</span> <span m="1488300">we</span>
  <span m="1488390">take</span> <span m="1488600">along</span> <span m="1488810">the</span>
  <span m="1488900">way.</span> <span m="1489440">That</span> <span m="1489560">will</span>
  <span m="1489680">be</span> <span m="1489800">the</span> <span m="1489860">goal.</span>
  <span m="1490460">And</span> <span m="1490580">it</span> <span m="1490640">could</span>
  <span m="1490790">be</span> <span m="1491450">either</span> <span m="1491810">through</span>
  <span m="1492830">an</span> <span m="1492920">immediate</span> <span m="1493820">effect</span>
  <span m="1494540">on</span> <span m="1494810">the</span> <span m="1495140">immediate</span>
  <span m="1495530">reward</span> <span m="1496190">or</span> <span m="1496310">it</span>
  <span m="1496370">can</span> <span m="1496550">be</span> <span m="1497090">through</span>
  <span m="1497660">the</span> <span m="1497900">impact</span> <span m="1498410">that</span>
  <span m="1498530">an</span> <span m="1498620">action</span> <span m="1498950">has</span>
  <span m="1499220">on</span> <span m="1499340">the</span> <span m="1499400">state</span>
  <span m="1499670">trajectory</span> <span m="1500060">itself.</span></p><p><span
  m="1507760">I</span> <span m="1507850">told</span> <span m="1508060">you</span>
  <span m="1508510">about</span> <span m="1508720">the</span> <span m="1508810">world</span>
  <span m="1509240">now</span> <span m="1509410">that</span> <span m="1509530">we</span>
  <span m="1509800">live</span> <span m="1509980">in.</span> <span m="1510090">We</span>
  <span m="1510220">have</span> <span m="1510370">these</span> <span m="1510580">Ss</span>
  <span m="1511030">and</span> <span m="1511160">As</span> <span m="1511520">and</span>
  <span m="1511800">Rs.</span> <span m="1512080">And</span> <span m="1513180">I</span>
  <span m="1513430">haven't</span> <span m="1513700">told</span> <span m="1513880">you</span>
  <span m="1513940">so</span> <span m="1514030">much</span> <span m="1514180">about</span>
  <span m="1514510">the</span> <span m="1514720">goal</span> <span m="1514960">that</span>
  <span m="1515050">we're</span> <span m="1515140">trying</span> <span m="1515350">to</span>
  <span m="1515410">solve</span> <span m="1515860">or</span> <span m="1516010">the</span>
  <span m="1516490">problem</span> <span m="1516700">that</span> <span m="1516790">we're</span>
  <span m="1516880">trying</span> <span m="1517090">to</span> <span m="1517150">solve.</span>
  <span m="1518890">Most</span> <span m="1519850">RL--</span> <span m="1520900">or</span>
  <span m="1521020">reinforcement</span> <span m="1521275">and</span> <span m="1521530">learning--</span>
  <span m="1522130">is</span> <span m="1522310">aimed</span> <span m="1522580">at</span>
  <span m="1523450">optimizing</span> <span m="1524200">the</span> <span m="1524320">value</span>
  <span m="1526330">of</span> <span m="1526630">a</span> <span m="1526750">policy</span>
  <span m="1527590">or</span> <span m="1527680">finding</span> <span m="1528010">a</span>
  <span m="1528070">policy</span> <span m="1528550">that</span> <span m="1529060">has</span>
  <span m="1529300">a</span> <span m="1529360">good</span> <span m="1530110">return,</span>
  <span m="1531010">a</span> <span m="1531130">good</span> <span m="1531400">sum</span>
  <span m="1531730">of</span> <span m="1531820">rewards.</span> <span m="1532420">There</span>
  <span m="1532600">are</span> <span m="1532660">many</span> <span m="1533000">names</span>
  <span m="1533230">for</span> <span m="1533350">this,</span> <span m="1533590">but</span>
  <span m="1533710">essentially</span> <span m="1534220">a</span> <span m="1534310">policy</span>
  <span m="1534640">that</span> <span m="1534760">does</span> <span m="1534970">well.</span></p><p><span
  m="1536740">The</span> <span m="1537190">notion</span> <span m="1537610">of</span>
  <span m="1537730">well</span> <span m="1538120">that</span> <span m="1538240">we</span>
  <span m="1538360">will</span> <span m="1538480">be</span> <span m="1538570">using</span>
  <span m="1538990">in</span> <span m="1539140">this</span> <span m="1540070">lecture</span>
  <span m="1540970">is</span> <span m="1542140">that</span> <span m="1542320">of</span>
  <span m="1542470">a</span> <span m="1542500">return.</span> <span m="1543350">So</span>
  <span m="1544740">the</span> <span m="1544940">return</span> <span m="1546230">at</span>
  <span m="1546370">a</span> <span m="1546430">time</span> <span m="1546740">step</span>
  <span m="1546890">t,</span> <span m="1548590">following</span> <span m="1549130">the</span>
  <span m="1549220">policy,</span> <span m="1549730">pi,</span> <span m="1550330">that</span>
  <span m="1550460">I</span> <span m="1550540">had</span> <span m="1550690">before,</span>
  <span m="1551530">is</span> <span m="1551680">the</span> <span m="1551740">sum</span>
  <span m="1552040">of</span> <span m="1552160">the</span> <span m="1552220">future</span>
  <span m="1552700">rewards</span> <span m="1553300">that</span> <span m="1553420">we</span>
  <span m="1553540">see</span> <span m="1555250">if</span> <span m="1555400">we</span>
  <span m="1555490">were</span> <span m="1555610">to</span> <span m="1555730">act</span>
  <span m="1555970">according</span> <span m="1556210">to</span> <span m="1556330">that</span>
  <span m="1556450">policy.</span></p><p><span m="1557900">So</span> <span m="1557950">essentially,</span>
  <span m="1558440">I</span> <span m="1558610">stop</span> <span m="1558950">now.</span>
  <span m="1559450">I</span> <span m="1559600">ask,</span> <span m="1559960">OK,</span>
  <span m="1560680">if</span> <span m="1560980">I</span> <span m="1561250">keep</span>
  <span m="1561550">on</span> <span m="1561670">doing</span> <span m="1561940">the</span>
  <span m="1562030">same</span> <span m="1562330">as</span> <span m="1562450">I've</span>
  <span m="1562570">done</span> <span m="1562900">through</span> <span m="1563140">my</span>
  <span m="1563260">whole</span> <span m="1563590">life--</span> <span m="1564500">maybe</span>
  <span m="1564670">that</span> <span m="1564790">was</span> <span m="1564910">a</span>
  <span m="1564940">good</span> <span m="1565090">policy.</span> <span m="1565480">I</span>
  <span m="1565540">don't</span> <span m="1565660">know.</span> <span m="1566860">And</span>
  <span m="1567040">keep</span> <span m="1567280">going</span> <span m="1567850">until</span>
  <span m="1568090">the</span> <span m="1568150">end</span> <span m="1568300">of</span>
  <span m="1568390">time,</span> <span m="1569260">how</span> <span m="1569510">well</span>
  <span m="1569750">will</span> <span m="1569860">I</span> <span m="1569950">do?</span>
  <span m="1570400">What</span> <span m="1570550">is</span> <span m="1570640">the</span>
  <span m="1570730">sum</span> <span m="1571060">of</span> <span m="1571180">those</span>
  <span m="1571990">rewards</span> <span m="1572440">that</span> <span m="1572560">I</span>
  <span m="1572650">get,</span> <span m="1572890">essentially?</span> <span m="1573790">That's</span>
  <span m="1573970">the</span> <span m="1574060">return.</span></p><p><span m="1575680">The</span>
  <span m="1575800">value</span> <span m="1576520">is</span> <span m="1576700">the</span>
  <span m="1576820">expectation</span> <span m="1577540">of</span> <span m="1577630">such</span>
  <span m="1577900">things.</span> <span m="1578830">So</span> <span m="1579190">if</span>
  <span m="1579400">I'm</span> <span m="1579640">not</span> <span m="1579790">the</span>
  <span m="1579910">only</span> <span m="1580120">person,</span> <span m="1580580">but</span>
  <span m="1580600">there</span> <span m="1580840">is the</span> <span m="1580960">whole</span>
  <span m="1581080">population</span> <span m="1581560">of</span> <span m="1581710">us,</span>
  <span m="1581800">the</span> <span m="1581890">expectation</span> <span m="1582460">over</span>
  <span m="1582640">that</span> <span m="1582790">population</span> <span m="1583420">is</span>
  <span m="1583570">the</span> <span m="1583660">value</span> <span m="1584050">of</span>
  <span m="1584170">the</span> <span m="1584230">policy.</span> <span m="1585080">So</span>
  <span m="1585250">if</span> <span m="1585460">we</span> <span m="1585610">take</span>
  <span m="1585880">patients</span> <span m="1586360">as</span> <span m="1586510">a</span>
  <span m="1586570">better</span> <span m="1586840">analogy</span> <span m="1587320">than</span>
  <span m="1587500">my</span> <span m="1587680">life,</span> <span m="1588410">maybe,</span>
  <span m="1589510">the</span> <span m="1589890">expectation is</span> <span m="1590350">over</span>
  <span m="1590620">patients.</span> <span m="1591370">If we</span> <span m="1591670">fact</span>
  <span m="1592450">on</span> <span m="1592600">every</span> <span m="1592840">patient</span>
  <span m="1593320">in</span> <span m="1593470">our</span> <span m="1593530">population</span>
  <span m="1594040">the</span> <span m="1594130">same</span> <span m="1594400">way--</span>
  <span m="1594700">according</span> <span m="1595000">to</span> <span m="1595090">the</span>
  <span m="1595180">same</span> <span m="1595420">policy,</span> <span m="1595810">that</span>
  <span m="1595930">is--</span> <span m="1596590">what</span> <span m="1596830">is</span>
  <span m="1596950">the</span> <span m="1597100">expected</span> <span m="1597910">return</span>
  <span m="1598450">over</span> <span m="1598690">those</span> <span m="1599230">patients?</span></p><p><span
  m="1601610">So</span> <span m="1601720">as</span> <span m="1601870">an</span> <span
  m="1601960">example,</span> <span m="1603610">I</span> <span m="1603910">drew</span>
  <span m="1604090">a</span> <span m="1604120">few</span> <span m="1604300">trajectories</span>
  <span m="1604810">again,</span> <span m="1605170">because</span> <span m="1605380">I</span>
  <span m="1605410">like</span> <span m="1605590">drawing.</span> <span m="1606610">And</span>
  <span m="1607150">we</span> <span m="1607270">can</span> <span m="1607360">think</span>
  <span m="1607510">about</span> <span m="1607990">three</span> <span m="1608230">different</span>
  <span m="1608500">patients</span> <span m="1608920">here.</span> <span m="1609120">They</span>
  <span m="1609250">start</span> <span m="1609610">in</span> <span m="1609700">different</span>
  <span m="1610030">states.</span> <span m="1610990">And</span> <span m="1611140">they</span>
  <span m="1611260">will</span> <span m="1611410">have</span> <span m="1611620">different</span>
  <span m="1612220">action</span> <span m="1612550">trajectories</span> <span m="1613270">as</span>
  <span m="1613450">a</span> <span m="1613480">result.</span></p><p><span m="1614570">So</span>
  <span m="1615400">we're</span> <span m="1615820">treating</span> <span m="1616150">them</span>
  <span m="1616270">with</span> <span m="1616420">the</span> <span m="1616510">same</span>
  <span m="1616810">policy.</span> <span m="1617320">Let's</span> <span m="1617500">call</span>
  <span m="1617650">it</span> <span m="1617740">pi.</span> <span m="1618460">But</span>
  <span m="1618700">because</span> <span m="1619030">they're</span> <span m="1619150">in</span>
  <span m="1619270">different</span> <span m="1619540">states,</span> <span m="1619870">they</span>
  <span m="1619990">will</span> <span m="1620110">have</span> <span m="1620260">different</span>
  <span m="1620590">actions</span> <span m="1620950">at</span> <span m="1621550">the</span>
  <span m="1621640">same</span> <span m="1621880">times.</span> <span m="1622600">So</span>
  <span m="1623200">here</span> <span m="1623560">we</span> <span m="1623890">take</span>
  <span m="1624570">a</span> <span m="1624670">0</span> <span m="1625090">action,</span>
  <span m="1625450">we</span> <span m="1625570">go</span> <span m="1625720">down.</span>
  <span m="1626110">Here,</span> <span m="1626290">we</span> <span m="1626350">take</span>
  <span m="1626500">a</span> <span m="1626590">0</span> <span m="1626650">action,</span>
  <span m="1626950">we</span> <span m="1627070">go</span> <span m="1627190">down.</span>
  <span m="1627580">That's</span> <span m="1627760">what</span> <span m="1627880">that</span>
  <span m="1628030">means</span> <span m="1628240">here.</span></p><p><span m="1629560">The</span>
  <span m="1629680">specifics</span> <span m="1630220">of</span> <span m="1630310">this</span>
  <span m="1630520">is</span> <span m="1630640">not</span> <span m="1630850">so</span>
  <span m="1630940">important.</span> <span m="1631660">But</span> <span m="1631690">what</span>
  <span m="1631840">I</span> <span m="1631900">want</span> <span m="1632070">you</span>
  <span m="1632200">to</span> <span m="1632290">pay</span> <span m="1632440">attention</span>
  <span m="1632830">to</span> <span m="1633010">is</span> <span m="1633130">that,</span>
  <span m="1633490">after</span> <span m="1634270">each</span> <span m="1634570">action,</span>
  <span m="1634930">we</span> <span m="1635080">get</span> <span m="1635290">a</span>
  <span m="1635360">reward.</span> <span m="1636860">And</span> <span m="1637030">at</span>
  <span m="1637120">the</span> <span m="1637270">end,</span> <span m="1637810">we</span>
  <span m="1637930">can</span> <span m="1638050">sum</span> <span m="1638290">those</span>
  <span m="1638560">up</span> <span m="1639050">and</span> <span m="1639070">that's</span>
  <span m="1639250">our</span> <span m="1639340">return.</span> <span m="1641790">So</span>
  <span m="1641940">each</span> <span m="1642150">patient</span> <span m="1642570">has</span>
  <span m="1645780">one</span> <span m="1646200">value</span> <span m="1646590">for</span>
  <span m="1646740">their</span> <span m="1646890">own</span> <span m="1647010">trajectory.</span>
  <span m="1647820">And</span> <span m="1647940">the</span> <span m="1648030">value</span>
  <span m="1648330">of</span> <span m="1648420">the</span> <span m="1648510">policy</span>
  <span m="1649020">is</span> <span m="1649140">then</span> <span m="1649260">the</span>
  <span m="1649380">average</span> <span m="1649770">value</span> <span m="1650070">of</span>
  <span m="1650130">such</span> <span m="1650490">trajectories.</span></p><p><span
  m="1655570">So</span> <span m="1655620">that</span> <span m="1655770">is</span>
  <span m="1655860">what</span> <span m="1655980">we're</span> <span m="1656090">trying</span>
  <span m="1656310">to</span> <span m="1656400">optimize.</span> <span m="1657570">We</span>
  <span m="1657690">have</span> <span m="1657900">now</span> <span m="1658140">a</span>
  <span m="1658200">notion</span> <span m="1658800">of</span> <span m="1659250">good</span>
  <span m="1660250">and</span> <span m="1660450">we</span> <span m="1660540">want</span>
  <span m="1660750">to</span> <span m="1660840">find</span> <span m="1661110">a</span>
  <span m="1661140">pi</span> <span m="1661590">such</span> <span m="1661950">that</span>
  <span m="1662220">V</span> <span m="1662430">pi</span> <span m="1662790">up</span>
  <span m="1662910">there</span> <span m="1663210">is</span> <span m="1663450">good.</span>
  <span m="1665220">That's</span> <span m="1665430">the</span> <span m="1665510">goal.</span>
  <span m="1668690">So</span> <span m="1668810">I</span> <span m="1668840">think</span>
  <span m="1669020">it's</span> <span m="1669170">time</span> <span m="1669540">for</span>
  <span m="1669850">a</span> <span m="1670520">bit</span> <span m="1670670">of</span>
  <span m="1670730">an</span> <span m="1670820">example</span> <span m="1671240">here.</span>
  <span m="1673640">I</span> <span m="1673790">want</span> <span m="1674150">you</span>
  <span m="1674240">to</span> <span m="1674330">play</span> <span m="1674600">along</span>
  <span m="1674990">in</span> <span m="1675080">a</span> <span m="1675110">second.</span></p><p><span
  m="1676430">You're</span> <span m="1677630">going</span> <span m="1677730">to</span>
  <span m="1677810">solve</span> <span m="1678020">this</span> <span m="1678140">problem.</span>
  <span m="1679800">It's</span> <span m="1679850">not</span> <span m="1680000">a</span>
  <span m="1680060">hard</span> <span m="1680240">one.</span> <span m="1680480">So</span>
  <span m="1680720">I</span> <span m="1680810">think</span> <span m="1680960">you'll</span>
  <span m="1681080">manage.</span> <span m="1681740">I</span> <span m="1681800">think</span>
  <span m="1681920">you'll</span> <span m="1682010">be</span> <span m="1682100">fine.</span>
  <span m="1683540">But</span> <span m="1683600">this</span> <span m="1683720">is</span>
  <span m="1683810">now</span> <span m="1684290">yet</span> <span m="1684500">another</span>
  <span m="1684800">example</span> <span m="1685390">of</span> <span m="1685570">a</span>
  <span m="1685670">world</span> <span m="1686000">to</span> <span m="1686180">be</span>
  <span m="1686360">in.</span></p><p><span m="1686720">This</span> <span m="1686930">is</span>
  <span m="1687230">the</span> <span m="1687350">robot</span> <span m="1687650">in</span>
  <span m="1687770">a</span> <span m="1687830">room.</span> <span m="1688250">And</span>
  <span m="1688370">I've</span> <span m="1688790">stolen</span> <span m="1689150">this</span>
  <span m="1689630">slide</span> <span m="1689930">from</span> <span m="1690110">David,</span>
  <span m="1690470">who</span> <span m="1690560">stole</span> <span m="1690830">it</span>
  <span m="1690890">from</span> <span m="1691130">Peter</span> <span m="1691460">Bodik.</span>
  <span m="1695010">Yeah,</span> <span m="1695510">so</span> <span m="1695810">credits</span>
  <span m="1696140">to</span> <span m="1696260">him.</span> <span m="1698930">The</span>
  <span m="1699050">rules</span> <span m="1699320">of</span> <span m="1699410">this</span>
  <span m="1699560">world</span> <span m="1699770">says</span> <span m="1700070">the</span>
  <span m="1700160">following--</span> <span m="1701210">if</span> <span m="1701420">you</span>
  <span m="1702170">tell</span> <span m="1702500">the</span> <span m="1702590">robot,</span>
  <span m="1703910">who</span> <span m="1704090">is</span> <span m="1704420">traversing</span>
  <span m="1705100">this</span> <span m="1705290">set</span> <span m="1705500">of</span>
  <span m="1705590">tiles</span> <span m="1705980">here--</span> <span m="1706620">if</span>
  <span m="1706720">you</span> <span m="1706820">tell</span> <span m="1706910">the</span>
  <span m="1707000">robot</span> <span m="1707240">to</span> <span m="1707330">go</span>
  <span m="1707570">up,</span> <span m="1708230">there's</span> <span m="1708440">a</span>
  <span m="1708500">chance</span> <span m="1708800">he</span> <span m="1708890">doesn't</span>
  <span m="1709130">go</span> <span m="1709310">up,</span> <span m="1710060">but</span>
  <span m="1710180">goes</span> <span m="1710330">somewhere</span> <span m="1710630">else.</span>
  <span m="1711930">So</span> <span m="1711980">we</span> <span m="1712130">have</span>
  <span m="1712400">the</span> <span m="1712490">stochastic</span> <span m="1713210">transitions,</span>
  <span m="1713840">essentially.</span></p><p><span m="1714420">If</span> <span m="1714470">I</span>
  <span m="1714560">say</span> <span m="1714830">up,</span> <span m="1715500">he</span>
  <span m="1715610">goes</span> <span m="1716060">up</span> <span m="1716300">with</span>
  <span m="1716720">point</span> <span m="1716990">a</span> <span m="1717140">probability</span>
  <span m="1718070">and</span> <span m="1718730">somewhere</span> <span m="1719150">else</span>
  <span m="1719450">with</span> <span m="1719750">uniform</span> <span m="1720200">probability,</span>
  <span m="1720680">say.</span> <span m="1720950">So</span> <span m="1722440">0.8</span>
  <span m="1723380">up</span> <span m="1723920">and</span> <span m="1724040">then</span>
  <span m="1724310">0.2--</span> <span m="1724910">this</span> <span m="1725090">is
  the</span> <span m="1725180">only</span> <span m="1725570">possible</span> <span
  m="1726050">direction</span> <span m="1727280">to</span> <span m="1727430">go</span>
  <span m="1727670">in</span> <span m="1727910">if</span> <span m="1728030">you</span>
  <span m="1728120">start</span> <span m="1728360">here.</span> <span m="1728960">So</span>
  <span m="1729110">0.2</span> <span m="1729530">in</span> <span m="1729620">that</span>
  <span m="1729770">way.</span> <span m="1730910">There's</span> <span m="1731090">a</span>
  <span m="1731150">chance</span> <span m="1731420">you</span> <span m="1731810">move</span>
  <span m="1732010">in</span> <span m="1732110">the</span> <span m="1732170">wrong</span>
  <span m="1732320">direction</span> <span m="1732650">is</span> <span m="1732980">what</span>
  <span m="1733100">I'm</span> <span m="1733160">trying</span> <span m="1733370">to</span>
  <span m="1733430">illustrate</span> <span m="1733840">here.</span></p><p><span m="1735980">There's</span>
  <span m="1736190">no</span> <span m="1736370">chance</span> <span m="1736640">that</span>
  <span m="1736780">they're</span> <span m="1737120">going</span> <span m="1737600">in</span>
  <span m="1737690">the</span> <span m="1737780">opposite</span> <span m="1738140">direction.</span>
  <span m="1738690">So</span> <span m="1738740">if</span> <span m="1738890">I</span>
  <span m="1738980">say</span> <span m="1739250">right</span> <span m="1739760">here,</span>
  <span m="1740570">it</span> <span m="1740660">can't</span> <span m="1740870">go</span>
  <span m="1740990">that</span> <span m="1741110">way.</span> <span m="1744960">The</span>
  <span m="1745150">rewards</span> <span m="1745600">in</span> <span m="1745690">this</span>
  <span m="1745810">game</span> <span m="1746650">is</span> <span m="1747100">plus</span>
  <span m="1747430">1</span> <span m="1747700">in</span> <span m="1747790">the</span>
  <span m="1747880">green</span> <span m="1748120">box</span> <span m="1748390">up</span>
  <span m="1748480">there,</span> <span m="1749020">minus</span> <span m="1749350">1</span>
  <span m="1749680">in</span> <span m="1750010">the</span> <span m="1750790">box</span>
  <span m="1751270">here.</span> <span m="1752020">And</span> <span m="1752170">these</span>
  <span m="1752410">are</span> <span m="1752500">also</span> <span m="1753100">terminal</span>
  <span m="1753550">states.</span> <span m="1753970">So</span> <span m="1754120">I</span>
  <span m="1754180">haven't</span> <span m="1754390">told</span> <span m="1754540">you</span>
  <span m="1754620">what that</span> <span m="1754910">is,</span> <span m="1755440">but</span>
  <span m="1755590">it's</span> <span m="1755680">essentially</span> <span m="1756120">a</span>
  <span m="1756190">state</span> <span m="1756520">in</span> <span m="1756640">which</span>
  <span m="1756820">the</span> <span m="1756910">game</span> <span m="1757180">ends.</span>
  <span m="1758590">So</span> <span m="1758710">once</span> <span m="1758950">you</span>
  <span m="1759040">get</span> <span m="1759220">to</span> <span m="1759340">either</span>
  <span m="1759550">plus</span> <span m="1759850">1</span> <span m="1760090">or</span>
  <span m="1760180">minus</span> <span m="1760510">1,</span> <span m="1760810">the</span>
  <span m="1760900">game</span> <span m="1761050">is</span> <span m="1761140">over.</span></p><p><span
  m="1763680">For</span> <span m="1763890">each</span> <span m="1764190">step</span>
  <span m="1764520">that</span> <span m="1764640">the</span> <span m="1764730">robot</span>
  <span m="1765030">takes,</span> <span m="1765960">it</span> <span m="1766020">incurs</span>
  <span m="1766890">0.04</span> <span m="1767760">negative</span> <span m="1768240">reward.</span>
  <span m="1769260">So</span> <span m="1769560">that</span> <span m="1769860">says,</span>
  <span m="1770260">essentially,</span> <span m="1770610">that</span> <span m="1770730">if</span>
  <span m="1770850">you</span> <span m="1770910">keep</span> <span m="1771120">going</span>
  <span m="1771390">for</span> <span m="1771510">a</span> <span m="1771540">long</span>
  <span m="1771750">time,</span> <span m="1772540">your</span> <span m="1772640">reward</span>
  <span m="1772800">would</span> <span m="1772950">be</span> <span m="1773070">bad.</span>
  <span m="1774720">The</span> <span m="1774810">value</span> <span m="1775080">of</span>
  <span m="1775170">the</span> <span m="1775230">policy</span> <span m="1775590">will</span>
  <span m="1775710">be</span> <span m="1775860">bad.</span> <span m="1777490">So</span>
  <span m="1777610">you</span> <span m="1777730">want</span> <span m="1777880">to</span>
  <span m="1777940">be</span> <span m="1778030">efficient.</span></p><p><span m="1779840">So</span>
  <span m="1779960">basically,</span> <span m="1780950">you</span> <span m="1781040">can</span>
  <span m="1781160">figure</span> <span m="1781430">out--</span> <span m="1781550">you
  want</span> <span m="1781850">to</span> <span m="1781910">get</span> <span m="1782090">to</span>
  <span m="1782180">the</span> <span m="1782300">green</span> <span m="1782570">thing,</span>
  <span m="1784280">that's</span> <span m="1784490">one</span> <span m="1784670">part</span>
  <span m="1784880">of</span> <span m="1784970">it.</span> <span m="1785910">But</span>
  <span m="1785930">you</span> <span m="1785990">also</span> <span m="1786110">want</span>
  <span m="1786230">to</span> <span m="1786290">do</span> <span m="1786380">it</span>
  <span m="1786470">quickly.</span> <span m="1787410">So</span> <span m="1787520">what</span>
  <span m="1787730">I</span> <span m="1787820">want</span> <span m="1788050">you</span>
  <span m="1788120">to</span> <span m="1788240">do</span> <span m="1788450">now</span>
  <span m="1789110">is</span> <span m="1789290">to</span> <span m="1790340">essentially</span>
  <span m="1790790">figure</span> <span m="1791120">out</span> <span m="1791210">what</span>
  <span m="1791420">is</span> <span m="1791510">the</span> <span m="1791600">best</span>
  <span m="1791840">policy,</span> <span m="1794180">in</span> <span m="1794270">terms</span>
  <span m="1794630">of</span> <span m="1795220">in</span> <span m="1795380">which</span>
  <span m="1795650">way</span> <span m="1796010">should</span> <span m="1796280">the</span>
  <span m="1796460">arrows</span> <span m="1796940">point</span> <span m="1797690">in</span>
  <span m="1797840">each</span> <span m="1798020">of</span> <span m="1798110">these</span>
  <span m="1798440">different</span> <span m="1798740">boxes?</span></p><p><span m="1801190">Fill</span>
  <span m="1801400">in</span> <span m="1801520">the</span> <span m="1801580">question</span>
  <span m="1801880">mark</span> <span m="1802090">with</span> <span m="1802270">an</span>
  <span m="1802450">arrow</span> <span m="1802780">pointing</span> <span m="1803080">in</span>
  <span m="1803140">some</span> <span m="1803320">direction.</span> <span m="1804070">We</span>
  <span m="1804190">know</span> <span m="1804340">the</span> <span m="1804490">different</span>
  <span m="1804870">transitions</span> <span m="1805630">will</span> <span m="1805780">be</span>
  <span m="1806710">stochastic,</span> <span m="1807340">so</span> <span m="1807460">you</span>
  <span m="1807580">might</span> <span m="1807760">need</span> <span m="1807910">to</span>
  <span m="1808000">take</span> <span m="1808180">that</span> <span m="1808330">into</span>
  <span m="1808480">account.</span> <span m="1809210">But</span> <span m="1809290">essentially,</span>
  <span m="1810130">figure</span> <span m="1810490">out</span> <span m="1810820">how</span>
  <span m="1811120">do</span> <span m="1811240">I</span> <span m="1811330">have</span>
  <span m="1811480">a</span> <span m="1811540">policy</span> <span m="1811960">that</span>
  <span m="1812110">gives</span> <span m="1812350">me</span> <span m="1812470">the</span>
  <span m="1812560">biggest</span> <span m="1813010">expected</span> <span m="1813520">reward?</span>
  <span m="1814300">And</span> <span m="1814420">I'll</span> <span m="1814510">ask</span>
  <span m="1814690">you</span> <span m="1814750">in</span> <span m="1814810">a</span>
  <span m="1814840">few</span> <span m="1815020">minutes</span> <span m="1815500">if</span>
  <span m="1815830">one</span> <span m="1816190">of</span> <span m="1816250">you</span>
  <span m="1816340">is</span> <span m="1816430">brave</span> <span m="1816610">enough</span>
  <span m="1816760">to</span> <span m="1816850">put</span> <span m="1817030">it</span>
  <span m="1817120">on</span> <span m="1817210">the</span> <span m="1817300">board</span>
  <span m="1817590">or something</span> <span m="1818070">like that.</span></p><p><span
  m="1821520">AUDIENCE:</span> <span m="1821590">We</span> <span m="1821660">start</span>
  <span m="1821860">the discount over</span> <span m="1822266">time?</span></p><p><span
  m="1823890">FREDRIK D. JOHANSSON:</span> <span m="1823995">There's</span> <span
  m="1824100">no</span> <span m="1824190">discount.</span></p><p><span m="1826400">AUDIENCE:</span>
  <span m="1826436">Can</span> <span m="1826472">we</span> <span m="1826510">talk</span>
  <span m="1826740">to</span> <span m="1826880">our</span> <span m="1826920">neighbor?</span></p><p><span
  m="1827650">FREDRIK D. JOHANSSON:</span> <span m="1827785">Yes.</span> <span m="1828760">It's</span>
  <span m="1828990">encouraged.</span></p><p><span m="1833260">[INTERPOSING VOICES]</span></p><p><span
  m="1836160">FREDRIK D. JOHANSSON:</span> <span m="1836310">So</span> <span m="1836460">I</span>
  <span m="1836550">had</span> <span m="1836670">a</span> <span m="1836730">question.</span>
  <span m="1838440">What</span> <span m="1838590">is</span> <span m="1838680">the</span>
  <span m="1838800">action</span> <span m="1839130">space?</span> <span m="1841170">And</span>
  <span m="1841590">essentially,</span> <span m="1841980">the</span> <span m="1842070">action</span>
  <span m="1842310">space</span> <span m="1842550">is</span> <span m="1842730">always</span>
  <span m="1844050">up,</span> <span m="1844260">down,</span> <span m="1844660">left,</span>
  <span m="1844800">or</span> <span m="1844860">right,</span> <span m="1845160">depending</span>
  <span m="1845610">on</span> <span m="1845730">if</span> <span m="1845850">there's</span>
  <span m="1846060">a</span> <span m="1846120">wall</span> <span m="1846330">or</span>
  <span m="1846420">not.</span> <span m="1847710">So</span> <span m="1847980">you</span>
  <span m="1848490">can't</span> <span m="1848700">go</span> <span m="1848880">right</span>
  <span m="1849300">here,</span> <span m="1849780">for</span> <span m="1849900">example.</span></p><p><span
  m="1851820">AUDIENCE:</span> <span m="1851960">You</span> <span m="1852100">can't</span>
  <span m="1852240">go left</span> <span m="1852660">either.</span></p><p><span m="1852750">FREDRIK
  D. JOHANSSON:</span> <span m="1852800">You</span> <span m="1852850">can't</span>
  <span m="1852900">go</span> <span m="1852990">left,</span> <span m="1853350">exactly.</span>
  <span m="1854520">Good</span> <span m="1854640">point.</span> <span m="1856470">So</span>
  <span m="1856830">each</span> <span m="1857070">box</span> <span m="1857460">at</span>
  <span m="1857580">the</span> <span m="1857670">end,</span> <span m="1857850">when</span>
  <span m="1858000">you're</span> <span m="1858090">done,</span> <span m="1858330">should</span>
  <span m="1858480">contain</span> <span m="1858810">an</span> <span m="1858900">arrow</span>
  <span m="1859170">pointing</span> <span m="1859470">in</span> <span m="1859530">some</span>
  <span m="1859680">direction.</span> <span m="1861240">All</span> <span m="1861300">right,</span>
  <span m="1861480">I</span> <span m="1861600">think</span> <span m="1861780">we'll</span>
  <span m="1863040">see</span> <span m="1863490">if</span> <span m="1863670">anybody</span>
  <span m="1864000">has</span> <span m="1864120">solved</span> <span m="1864450">this</span>
  <span m="1864660">problem</span> <span m="1865080">now.</span> <span m="1866420">Who</span>
  <span m="1866580">thinks</span> <span m="1866790">they</span> <span m="1866910">have</span>
  <span m="1867000">solved</span> <span m="1867230">it?</span> <span m="1869200">Great.</span>
  <span m="1870690">Would</span> <span m="1870870">you</span> <span m="1870990">like</span>
  <span m="1871140">to</span> <span m="1871260">share</span> <span m="1871470">your</span>
  <span m="1871650">solution?</span></p><p><span m="1873890">AUDIENCE:</span> <span
  m="1874135">Yeah,</span> <span m="1874380">so I</span> <span m="1874440">think</span>
  <span m="1874980">it's</span> <span m="1875190">going</span> <span m="1875430">to</span>
  <span m="1876840">go</span> <span m="1877000">up</span> <span m="1877220">first.</span></p><p><span
  m="1879510">FREDRIK D. JOHANSSON:</span> <span m="1879555">I'm</span> <span m="1879600">going</span>
  <span m="1879720">to</span> <span m="1879960">try</span> <span m="1880200">and</span>
  <span m="1880290">replicate</span> <span m="1880650">this.</span> <span m="1880920">Ooh,</span>
  <span m="1881210">sorry</span> <span m="1881430">about</span> <span m="1881540">that.</span>
  <span m="1884130">OK,</span> <span m="1884610">you're</span> <span m="1884760">saying</span>
  <span m="1885330">up</span> <span m="1885510">here?</span></p><p><span m="1886050">AUDIENCE:</span>
  <span m="1886135">Yeah.</span> <span m="1887850">The</span> <span m="1887940">basic</span>
  <span m="1888270">idea</span> <span m="1888540">is</span> <span m="1888690">you</span>
  <span m="1888780">want</span> <span m="1888960">to</span> <span m="1889620">reduce</span>
  <span m="1890040">the</span> <span m="1890130">chance</span> <span m="1890460">that</span>
  <span m="1890550">you're</span> <span m="1890620">ever</span> <span m="1891010">adjacent</span>
  <span m="1891590">to</span> <span m="1891720">the</span> <span m="1891810">red</span>
  <span m="1892050">box.</span> <span m="1893070">So</span> <span m="1893430">just</span>
  <span m="1893660">do everything</span> <span m="1893910">you</span> <span m="1894090">can</span>
  <span m="1894330">to</span> <span m="1894620">stay</span> <span m="1894910">far</span>
  <span m="1895050">from</span> <span m="1895260">it.</span> <span m="1896380">Yeah,</span>
  <span m="1896610">so</span> <span m="1896750">attempt to</span> <span m="1897020">go</span>
  <span m="1897180">up</span> <span m="1897450">and</span> <span m="1897570">then</span>
  <span m="1898020">once</span> <span m="1898230">you</span> <span m="1898300">eventually</span>
  <span m="1898680">get</span> <span m="1898860">there,</span> <span m="1899880">you
  just</span> <span m="1900020">have to go</span> <span m="1900330">right.</span></p><p><span
  m="1900970">FREDRIK D. JOHANSSON:</span> <span m="1901065">OK.</span> <span m="1902330">And</span>
  <span m="1902440">then?</span></p><p><span m="1903876">AUDIENCE:</span> <span m="1904013">[INAUDIBLE].</span></p><p><span
  m="1904700">FREDRIK D. JOHANSSON:</span> <span m="1904805">OK.</span> <span m="1905430">So</span>
  <span m="1905580">what</span> <span m="1905730">about</span> <span m="1905940">these</span>
  <span m="1906160">ones?</span> <span m="1910170">This</span> <span m="1910350">is</span>
  <span m="1910470">also</span> <span m="1910650">part</span> <span m="1910860">of</span>
  <span m="1910920">the</span> <span m="1911010">policy,</span> <span m="1911380">by
  the</span> <span m="1911520">way.</span></p><p><span m="1914412">AUDIENCE:</span>
  <span m="1914566">I</span> <span m="1914720">hadn't</span> <span m="1914874">thought</span>
  <span m="1915336">about this.</span></p><p><span m="1916260">FREDRIK D. JOHANSSON:</span>
  <span m="1916325">OK.</span></p><p><span m="1917320">AUDIENCE:</span> <span m="1917475">But</span>
  <span m="1917630">those,</span> <span m="1917785">you</span> <span m="1918250">[INAUDIBLE],</span>
  <span m="1918715">right?</span></p><p><span m="1919940">FREDRIK D. JOHANSSON:</span>
  <span m="1920055">No.</span></p><p><span m="1921260">AUDIENCE:</span> <span m="1921387">Minus</span>
  <span m="1921770">0.04.</span></p><p><span m="1923970">FREDRIK D. JOHANSSON:</span>
  <span m="1923995">So</span> <span m="1924020">discount</span> <span m="1924320">usually</span>
  <span m="1924590">means</span> <span m="1924740">something</span> <span m="1925040">else.</span>
  <span m="1925400">We'll</span> <span m="1925610">get</span> <span m="1925760">to</span>
  <span m="1925850">that</span> <span m="1925970">later.</span> <span m="1926900">But</span>
  <span m="1927020">that</span> <span m="1927340">is</span> <span m="1927500">a</span>
  <span m="1927560">reward</span> <span m="1927950">for</span> <span m="1928880">just</span>
  <span m="1929090">taking</span> <span m="1929390">any</span> <span m="1929570">step.</span>
  <span m="1931880">If</span> <span m="1932270">you</span> <span m="1932570">move</span>
  <span m="1932840">into</span> <span m="1933200">a</span> <span m="1933260">space</span>
  <span m="1933620">that</span> <span m="1933740">is</span> <span m="1933830">not</span>
  <span m="1933980">terminal,</span> <span m="1934480">you</span> <span m="1934610">incur</span>
  <span m="1934880">that</span> <span m="1935360">negative</span> <span m="1935690">reward.</span></p><p><span
  m="1936580">AUDIENCE:</span> <span m="1936640">So</span> <span m="1936700">if</span>
  <span m="1936760">you</span> <span m="1936820">keep</span> <span m="1937070">bouncing</span>
  <span m="1937430">around</span> <span m="1937690">for a really long time,</span>
  <span m="1938210">you incur</span> <span m="1938570">a</span> <span m="1938670">long</span>
  <span m="1938930">negative</span> <span m="1939160">reward.</span></p><p><span m="1939440">FREDRIK
  D. JOHANSSON:</span> <span m="1939480">If</span> <span m="1939520">we</span> <span
  m="1939560">had</span> <span m="1939740">this,</span> <span m="1941060">there's</span>
  <span m="1941270">some</span> <span m="1941480">chance</span> <span m="1941750">I'd</span>
  <span m="1941900">never</span> <span m="1942170">get</span> <span m="1942350">out</span>
  <span m="1942590">of</span> <span m="1942680">all</span> <span m="1942860">this.</span>
  <span m="1943160">And very</span> <span m="1943370">little</span> <span m="1943580">chance</span>
  <span m="1943840">of that</span> <span m="1943910">working</span> <span m="1944060">out.</span>
  <span m="1944300">But</span> <span m="1944420">it's</span> <span m="1944780">a</span>
  <span m="1944840">very</span> <span m="1944990">bad</span> <span m="1945140">policy,</span>
  <span m="1945500">because</span> <span m="1945740">you</span> <span m="1945950">keep</span>
  <span m="1946130">moving</span> <span m="1946310">back</span> <span m="1946400">and</span>
  <span m="1946460">forth.</span> <span m="1949220">All</span> <span m="1949290">right,</span>
  <span m="1949890">we</span> <span m="1949980">had</span> <span m="1950280">an</span>
  <span m="1950490">arm</span> <span m="1950700">somewhere.</span> <span m="1952230">What</span>
  <span m="1952350">should</span> <span m="1952500">I</span> <span m="1952530">do</span>
  <span m="1952680">here?</span></p><p><span m="1955080">AUDIENCE:</span> <span m="1955125">You</span>
  <span m="1955170">could</span> <span m="1955260">take</span> <span m="1955350">a</span>
  <span m="1955420">vote.</span></p><p><span m="1956190">FREDRIK D. JOHANSSON:</span>
  <span m="1956295">OK.</span> <span m="1956730">Who</span> <span m="1956880">thinks</span>
  <span m="1957210">right?</span> <span m="1958468">Really?</span> <span m="1959860">Who
  thinks</span> <span m="1960230">left?</span> <span m="1961416">OK,</span> <span
  m="1961860">interesting.</span> <span m="1963540">I</span> <span m="1963800">don't</span>
  <span m="1964130">actually</span> <span m="1964460">remember.</span> <span m="1966020">Let's</span>
  <span m="1966230">see.</span> <span m="1968630">Go</span> <span m="1968870">ahead.</span></p><p><span
  m="1969292">AUDIENCE:</span> <span m="1969376">I</span> <span m="1969460">was</span>
  <span m="1969544">just</span> <span m="1969628">saying,</span> <span m="1969714">that's</span>
  <span m="1970136">an easy</span> <span m="1970558">one.</span></p><p><span m="1970980">FREDRIK
  D. JOHANSSON:</span> <span m="1971140">Yeah,</span> <span m="1971300">so</span>
  <span m="1971450">this</span> <span m="1971750">is</span> <span m="1971870">the</span>
  <span m="1971960">part</span> <span m="1972170">that</span> <span m="1972290">we</span>
  <span m="1972500">already</span> <span m="1973490">determined.</span> <span m="1974200">If</span>
  <span m="1974360">we</span> <span m="1974450">had</span> <span m="1974540">deterministic</span>
  <span m="1975080">transitions,</span> <span m="1975560">this</span> <span m="1975710">would</span>
  <span m="1975830">be</span> <span m="1976280">great,</span> <span m="1977450">because</span>
  <span m="1977690">we</span> <span m="1977780">don't</span> <span m="1977900">have</span>
  <span m="1977990">to</span> <span m="1978050">think</span> <span m="1978200">about</span>
  <span m="1978350">the</span> <span m="1978410">other</span> <span m="1978490">ones.</span>
  <span m="1979800">This</span> <span m="1979910">is</span> <span m="1980030">what</span>
  <span m="1981530">Peter</span> <span m="1982400">put</span> <span m="1982550">on</span>
  <span m="1982640">the</span> <span m="1982700">slide.</span> <span m="1983040">So</span>
  <span m="1983120">I'm</span> <span m="1983210">going</span> <span m="1983320">to</span>
  <span m="1983390">have</span> <span m="1983480">to</span> <span m="1983570">disagree</span>
  <span m="1983930">with</span> <span m="1984410">the</span> <span m="1984530">vote</span>
  <span m="1984770">there,</span> <span m="1984950">actually.</span> <span m="1987370">It</span>
  <span m="1987590">depends,</span> <span m="1988040">actually,</span> <span m="1988430">heavily</span>
  <span m="1988940">on</span> <span m="1990530">the</span> <span m="1990650">minus</span>
  <span m="1991040">0.04.</span></p><p><span m="1993680">So</span> <span m="1993920">if</span>
  <span m="1994100">you</span> <span m="1994220">increase</span> <span m="1994610">that</span>
  <span m="1994760">by</span> <span m="1994910">a</span> <span m="1994970">little</span>
  <span m="1995180">bit,</span> <span m="1995540">you</span> <span m="1995690">might</span>
  <span m="1995870">want</span> <span m="1996020">to</span> <span m="1996080">go</span>
  <span m="1996230">that</span> <span m="1996410">way</span> <span m="1996530">instead.</span>
  <span m="1997790">Or</span> <span m="1997940">if</span> <span m="1998060">you</span>
  <span m="1998240">decrease--</span> <span m="1998590">I don't</span> <span m="1998750">remember.</span>
  <span m="1999110">Decrease,</span> <span m="1999450">exactly.</span> <span m="2000080">And</span>
  <span m="2000190">if</span> <span m="2000310">you</span> <span m="2000400">increase</span>
  <span m="2000700">it,</span> <span m="2000890">you</span> <span m="2000990">might</span>
  <span m="2001360">get</span> <span m="2001510">something</span> <span m="2001810">else.</span>
  <span m="2002090">It</span> <span m="2002190">might</span> <span m="2002200">actually</span>
  <span m="2002380">be</span> <span m="2002500">good</span> <span m="2002650">to terminate.</span></p><p><span
  m="2004390">So</span> <span m="2004990">those</span> <span m="2005260">details</span>
  <span m="2005620">matter</span> <span m="2005950">a</span> <span m="2005980">little</span>
  <span m="2006160">bit.</span> <span m="2006310">But</span> <span m="2006520">I</span>
  <span m="2006730">think</span> <span m="2006880">you've</span> <span m="2006960">got</span>
  <span m="2007090">the</span> <span m="2007210">general</span> <span m="2007510">idea.</span>
  <span m="2008140">And</span> <span m="2008240">especially</span> <span m="2008500">I</span>
  <span m="2008590">like</span> <span m="2008770">that</span> <span m="2008860">you</span>
  <span m="2008950">commented</span> <span m="2009340">that</span> <span m="2010000">you</span>
  <span m="2010120">want</span> <span m="2010270">to</span> <span m="2010330">stay</span>
  <span m="2010480">away</span> <span m="2010720">from</span> <span m="2010930">the</span>
  <span m="2011020">red</span> <span m="2011200">one,</span> <span m="2011710">because</span>
  <span m="2011980">if</span> <span m="2012070">you</span> <span m="2012160">look</span>
  <span m="2012430">at</span> <span m="2012640">these</span> <span m="2013180">different</span>
  <span m="2013510">paths.</span> <span m="2013960">You</span> <span m="2014050">go</span>
  <span m="2014290">up</span> <span m="2014500">there</span> <span m="2015160">and</span>
  <span m="2015310">there--</span> <span m="2015850">they</span> <span m="2015910">have</span>
  <span m="2016000">the</span> <span m="2016060">same</span> <span m="2016300">number</span>
  <span m="2016540">of</span> <span m="2016600">states,</span> <span m="2017170">but</span>
  <span m="2017350">there's</span> <span m="2017530">less</span> <span m="2017800">chance</span>
  <span m="2018070">you</span> <span m="2018160">end</span> <span m="2018310">up</span>
  <span m="2018430">in</span> <span m="2018520">the</span> <span m="2018610">red</span>
  <span m="2018760">box</span> <span m="2019060">if</span> <span m="2019120">you</span>
  <span m="2019210">take</span> <span m="2019390">the</span> <span m="2019960">upper</span>
  <span m="2020170">route.</span> <span m="2022030">Great.</span></p><p><span m="2023200">So</span>
  <span m="2023320">we</span> <span m="2023410">have</span> <span m="2023530">an</span>
  <span m="2023590">example</span> <span m="2023920">of</span> <span m="2024010">a</span>
  <span m="2024040">policy</span> <span m="2024840">and</span> <span m="2024940">we</span>
  <span m="2025000">have</span> <span m="2025090">an</span> <span m="2025150">example</span>
  <span m="2025510">of</span> <span m="2025660">a</span> <span m="2025900">decision</span>
  <span m="2026320">process.</span> <span m="2026680">And</span> <span m="2026830">things</span>
  <span m="2027040">are</span> <span m="2027280">working</span> <span m="2027550">out</span>
  <span m="2028360">so</span> <span m="2028540">far.</span> <span m="2029560">But</span>
  <span m="2029680">how</span> <span m="2029770">do</span> <span m="2029860">we</span>
  <span m="2030040">do</span> <span m="2030220">this?</span> <span m="2032560">As</span>
  <span m="2032650">far</span> <span m="2032800">as</span> <span m="2033670">the</span>
  <span m="2033760">class</span> <span m="2034090">goes,</span> <span m="2034510">this</span>
  <span m="2034750">was</span> <span m="2034900">a</span> <span m="2034990">blackbox</span>
  <span m="2035620">experiment.</span> <span m="2036110">I</span> <span m="2036210">don't</span>
  <span m="2036310">know</span> <span m="2036340">anything</span> <span m="2036640">about</span>
  <span m="2036880">how</span> <span m="2037000">you</span> <span m="2037120">figured</span>
  <span m="2037360">that</span> <span m="2037540">out.</span></p><p><span m="2038710">So</span>
  <span m="2039370">reinforcement</span> <span m="2039850">learning</span> <span m="2040060">is</span>
  <span m="2040180">about</span> <span m="2040390">that--</span> <span m="2041080">reinforcement</span>
  <span m="2041470">learning</span> <span m="2041680">is</span> <span m="2041890">try</span>
  <span m="2042110">and</span> <span m="2042190">come</span> <span m="2042340">up</span>
  <span m="2042460">with</span> <span m="2042580">a</span> <span m="2042610">policy</span>
  <span m="2043060">in</span> <span m="2043190">a</span> <span m="2044170">rigorous</span>
  <span m="2044500">way,</span> <span m="2044710">hopefully--</span> <span m="2045180">ideally.</span>
  <span m="2046690">So</span> <span m="2046930">that</span> <span m="2047050">would</span>
  <span m="2047170">be</span> <span m="2047290">the</span> <span m="2047380">next</span>
  <span m="2048429">topic</span> <span m="2048820">here.</span> <span m="2050380">Up</span>
  <span m="2050530">until</span> <span m="2050770">this</span> <span m="2050920">point,</span>
  <span m="2051260">are</span> <span m="2051360">there</span> <span m="2051380">any</span>
  <span m="2051460">questions</span> <span m="2051820">that</span> <span m="2052000">you've</span>
  <span m="2052150">been</span> <span m="2052270">dying</span> <span m="2052510">to</span>
  <span m="2052600">ask,</span> <span m="2052810">but</span> <span m="2052900">haven't?</span></p><p><span
  m="2055170">AUDIENCE:</span> <span m="2055414">I'm</span> <span m="2055659">curious</span>
  <span m="2056110">how</span> <span m="2056590">much</span> <span m="2056889">behavioral</span>
  <span m="2057699">biases</span> <span m="2058210">could</span> <span m="2058389">play</span>
  <span m="2058690">into</span> <span m="2058870">the</span> <span m="2058960">first</span>
  <span m="2059320">Markov</span> <span m="2059710">assumption?</span> <span m="2060699">So
  for</span> <span m="2060790">example,</span> <span m="2061340">if</span> <span m="2061389">you're</span>
  <span m="2062199">a</span> <span m="2062260">clinician</span> <span m="2062650">who's</span>
  <span m="2062770">been</span> <span m="2062860">working</span> <span m="2063190">for</span>
  <span m="2063400">30</span> <span m="2063699">years</span> <span m="2064070">and</span>
  <span m="2064170">you're</span> <span m="2064179">just</span> <span m="2064360">really</span>
  <span m="2064690">used</span> <span m="2064960">to</span> <span m="2065050">giving</span>
  <span m="2065360">a</span> <span m="2065380">certain</span> <span m="2065650">treatment.</span>
  <span m="2066580">An</span> <span m="2066699">action</span> <span m="2067000">that</span>
  <span m="2067090">you</span> <span m="2067179">gave</span> <span m="2067360">in</span>
  <span m="2067420">the</span> <span m="2067510">past--</span> <span m="2067840">that</span>
  <span m="2067989">habit</span> <span m="2068380">might</span> <span m="2068650">influence</span>
  <span m="2069300">an</span> <span m="2069429">action</span> <span m="2069790">in
  the</span> <span m="2069860">future.</span> <span m="2070800">And</span> <span m="2071500">if</span>
  <span m="2071650">that</span> <span m="2071800">is</span> <span m="2071929">a</span>
  <span m="2071969">worry,</span> <span m="2072250">how</span> <span m="2073060">one</span>
  <span m="2073270">might</span> <span m="2073420">think</span> <span m="2073570">about</span>
  <span m="2073900">addressing</span> <span m="2074260">it.</span></p><p><span m="2076510">FREDRIK
  D. JOHANSSON:</span> <span m="2076655">Interesting.</span> <span m="2078460">I</span>
  <span m="2078550">guess</span> <span m="2078730">it</span> <span m="2078790">depends</span>
  <span m="2079060">a</span> <span m="2079120">little</span> <span m="2079300">bit</span>
  <span m="2079420">on</span> <span m="2079540">how</span> <span m="2079719">it</span>
  <span m="2079810">manifests,</span> <span m="2080830">in</span> <span m="2081010">that</span>
  <span m="2081850">if</span> <span m="2082000">it</span> <span m="2082120">also</span>
  <span m="2082480">influenced</span> <span m="2083860">your</span> <span m="2084010">most</span>
  <span m="2084310">recent</span> <span m="2084610">action,</span> <span m="2085000">maybe</span>
  <span m="2085239">you</span> <span m="2085659">have</span> <span m="2085870">an</span>
  <span m="2085929">observation</span> <span m="2086469">of</span> <span m="2086590">that</span>
  <span m="2086980">already</span> <span m="2087280">in</span> <span m="2087370">some</span>
  <span m="2087550">sense.</span> <span m="2091929">It's</span> <span m="2092050">a</span>
  <span m="2092080">very</span> <span m="2092230">broad</span> <span m="2092469">question.</span>
  <span m="2093130">What</span> <span m="2093429">effect</span> <span m="2093670">will</span>
  <span m="2093820">that</span> <span m="2093940">have?</span> <span m="2094690">Did</span>
  <span m="2094810">you</span> <span m="2094870">have</span> <span m="2094989">something</span>
  <span m="2095260">specific</span> <span m="2095679">in</span> <span m="2095770">mind?</span></p><p><span
  m="2096639">AUDIENCE:</span> <span m="2096684">I</span> <span m="2096730">guess</span>
  <span m="2096909">I</span> <span m="2096969">was</span> <span m="2097090">just</span>
  <span m="2097270">wondering</span> <span m="2097690">if</span> <span m="2097810">it</span>
  <span m="2097990">violated</span> <span m="2098620">that</span> <span m="2099550">assumption,</span>
  <span m="2100260">that</span> <span m="2100960">an</span> <span m="2101260">action</span>
  <span m="2101580">of</span> <span m="2101640">the</span> <span m="2101710">past</span>
  <span m="2102010">influenced</span> <span m="2102400">an action--</span></p><p><span
  m="2102750">FREDRIK D. JOHANSSON:</span> <span m="2102925">Interesting.</span> <span
  m="2103450">So</span> <span m="2103780">I</span> <span m="2104020">guess</span>
  <span m="2104750">my</span> <span m="2105280">response</span> <span m="2105730">there</span>
  <span m="2105970">is</span> <span m="2106120">that</span> <span m="2106270">the</span>
  <span m="2108640">action</span> <span m="2108940">didn't</span> <span m="2109210">really</span>
  <span m="2109450">depend</span> <span m="2109990">on</span> <span m="2110080">the</span>
  <span m="2110170">choice</span> <span m="2110530">of</span> <span m="2110650">action</span>
  <span m="2110890">before,</span> <span m="2111160">because</span> <span m="2111430">the</span>
  <span m="2111490">policy</span> <span m="2111880">remained</span> <span m="2112210">the</span>
  <span m="2112300">same.</span> <span m="2113140">You</span> <span m="2113650">could</span>
  <span m="2113770">have</span> <span m="2113890">a</span> <span m="2113950">bias</span>
  <span m="2114280">towards</span> <span m="2115090">an</span> <span m="2115180">action</span>
  <span m="2115510">without</span> <span m="2115960">that</span> <span m="2116230">being</span>
  <span m="2116440">dependent</span> <span m="2116770">on</span> <span m="2116890">what</span>
  <span m="2117070">you</span> <span m="2117340">gave</span> <span m="2118390">as</span>
  <span m="2118570">action</span> <span m="2118840">before,</span> <span m="2119200">if</span>
  <span m="2119290">you</span> <span m="2119380">know</span> <span m="2119470">what</span>
  <span m="2119560">I</span> <span m="2119590">mean.</span></p><p><span m="2120700">Say</span>
  <span m="2120970">my</span> <span m="2121090">probability</span> <span m="2121540">of</span>
  <span m="2121630">giving</span> <span m="2121870">action</span> <span m="2122110">one</span>
  <span m="2122380">is</span> <span m="2122530">1,</span> <span m="2123220">then</span>
  <span m="2123340">it</span> <span m="2123400">doesn't</span> <span m="2123640">matter</span>
  <span m="2123910">that</span> <span m="2124030">I</span> <span m="2124090">give</span>
  <span m="2124240">it</span> <span m="2124390">in</span> <span m="2124480">the</span>
  <span m="2124540">past.</span> <span m="2124870">My</span> <span m="2124990">policy</span>
  <span m="2125260">is</span> <span m="2125320">still</span> <span m="2125560">the</span>
  <span m="2125620">same.</span> <span m="2127450">So,</span> <span m="2127810">not</span>
  <span m="2128020">necessarily.</span> <span m="2129290">It</span> <span m="2129310">could</span>
  <span m="2129460">have</span> <span m="2129580">other</span> <span m="2129760">consequences.</span>
  <span m="2130720">We</span> <span m="2131170">might</span> <span m="2131680">have</span>
  <span m="2131800">reason</span> <span m="2131980">to</span> <span m="2132070">come</span>
  <span m="2132190">back</span> <span m="2132340">to</span> <span m="2132430">that</span>
  <span m="2132520">question</span> <span m="2132790">later.</span> <span m="2134740">Yup.</span></p><p><span
  m="2135700">AUDIENCE:</span> <span m="2135865">Just</span> <span m="2136850">practically,</span>
  <span m="2137880">I</span> <span m="2138000">would</span> <span m="2139330">think</span>
  <span m="2139500">that</span> <span m="2140570">a doctor</span> <span m="2140810">would</span>
  <span m="2140910">want to be</span> <span m="2141350">consistent.</span> <span m="2142820">And
  so</span> <span m="2143420">you</span> <span m="2143600">wouldn't,</span> <span
  m="2143900">for</span> <span m="2144140">example,</span> <span m="2144720">want</span>
  <span m="2144830">to</span> <span m="2144890">put</span> <span m="2145100">somebody</span>
  <span m="2145580">on</span> <span m="2145760">a</span> <span m="2145890">ventilator</span>
  <span m="2146240">and</span> <span m="2146637">then</span> <span m="2147034">immediately</span>
  <span m="2147431">take them</span> <span m="2147830">off</span> <span m="2148378">and</span>
  <span m="2148796">then immediately</span> <span m="2149214">put them</span> <span
  m="2149632">back on</span> <span m="2150050">again.</span> <span m="2150810">So</span>
  <span m="2151010">that would</span> <span m="2151463">be</span> <span m="2151916">an
  example</span> <span m="2152550">where</span> <span m="2152990">the</span> <span
  m="2153110">past</span> <span m="2153500">action</span> <span m="2153720">influences</span>
  <span m="2154260">what</span> <span m="2154670">you're</span> <span m="2155115">going
  to do.</span></p><p><span m="2155560">FREDRIK D. JOHANSSON:</span> <span m="2155805">Completely,</span>
  <span m="2156050">yeah.</span> <span m="2156560">I</span> <span m="2156620">think</span>
  <span m="2156770">that's</span> <span m="2156920">a</span> <span m="2156980">great</span>
  <span m="2157190">example.</span> <span m="2158300">And</span> <span m="2159560">what</span>
  <span m="2160460">you</span> <span m="2160550">would</span> <span m="2160700">hope</span>
  <span m="2161270">is</span> <span m="2161450">that</span> <span m="2161690">the</span>
  <span m="2162230">state</span> <span m="2162530">variable</span> <span m="2162860">in</span>
  <span m="2162950">that</span> <span m="2163070">case</span> <span m="2163340">includes</span>
  <span m="2163730">some</span> <span m="2164000">notion</span> <span m="2164360">of</span>
  <span m="2164510">treatment</span> <span m="2164810">history.</span> <span m="2166020">That's</span>
  <span m="2166370">what</span> <span m="2167060">your</span> <span m="2167150">job</span>
  <span m="2167390">is</span> <span m="2167510">then.</span> <span m="2168740">So</span>
  <span m="2169190">that's</span> <span m="2169430">why</span> <span m="2169570">state</span>
  <span m="2169940">can</span> <span m="2170090">be</span> <span m="2170210">somewhat</span>
  <span m="2170660">misleading</span> <span m="2171230">as</span> <span m="2171380">a</span>
  <span m="2171620">term--</span> <span m="2171890">at</span> <span m="2171950">least</span>
  <span m="2172100">for</span> <span m="2172190">me,</span> <span m="2172790">I'm</span>
  <span m="2172910">not</span> <span m="2173030">American</span> <span m="2173870">or</span>
  <span m="2174020">English-speaking.</span> <span m="2177190">But</span> <span m="2177350">yeah,</span>
  <span m="2177710">I</span> <span m="2177920">think</span> <span m="2178100">of</span>
  <span m="2178220">it</span> <span m="2178580">as</span> <span m="2178730">too</span>
  <span m="2178970">instantaneous</span> <span m="2179480">sometimes.</span></p><p><span
  m="2180560">So</span> <span m="2180710">we'll</span> <span m="2180830">move</span>
  <span m="2180980">into</span> <span m="2181160">reinforcement</span> <span m="2181790">learning</span>
  <span m="2182030">now.</span> <span m="2182660">And</span> <span m="2184340">what</span>
  <span m="2184550">I</span> <span m="2184700">had</span> <span m="2184960">you</span>
  <span m="2185120">do</span> <span m="2186050">on</span> <span m="2186440">the</span>
  <span m="2186920">last</span> <span m="2187310">slide--</span> <span m="2188540">well,</span>
  <span m="2189110">I</span> <span m="2189170">don't</span> <span m="2189320">know</span>
  <span m="2189440">which</span> <span m="2189890">method</span> <span m="2190430">you</span>
  <span m="2190490">use,</span> <span m="2190730">but</span> <span m="2190850">most</span>
  <span m="2191090">likely</span> <span m="2191990">the</span> <span m="2192080">middle</span>
  <span m="2192320">one.</span> <span m="2193160">There</span> <span m="2193340">are</span>
  <span m="2193460">three</span> <span m="2193910">very</span> <span m="2194690">common</span>
  <span m="2195080">paradigms</span> <span m="2196730">for</span> <span m="2197060">reinforcement</span>
  <span m="2197570">learning.</span> <span m="2198290">And</span> <span m="2198470">they</span>
  <span m="2198650">are</span> <span m="2198740">essentially</span> <span m="2199250">divided</span>
  <span m="2199640">by</span> <span m="2200420">what</span> <span m="2200660">they</span>
  <span m="2200780">focus</span> <span m="2201200">on</span> <span m="2201380">modeling.</span>
  <span m="2203630">Unsurprisingly,</span> <span m="2204350">model-based</span> <span
  m="2204980">RL</span> <span m="2205340">focused</span> <span m="2205760">on--</span>
  <span m="2206900">well,</span> <span m="2207500">it</span> <span m="2207710">has</span>
  <span m="2207920">some</span> <span m="2208160">sort</span> <span m="2208340">of</span>
  <span m="2208400">model</span> <span m="2208730">in</span> <span m="2208850">it,</span>
  <span m="2209000">at</span> <span m="2209120">least.</span></p><p><span m="2212750">What</span>
  <span m="2212900">you</span> <span m="2212960">mean</span> <span m="2213110">by</span>
  <span m="2213200">model</span> <span m="2213470">in</span> <span m="2213530">this</span>
  <span m="2213680">case</span> <span m="2214160">is</span> <span m="2214280">a</span>
  <span m="2214340">model</span> <span m="2214520">of</span> <span m="2214640">the</span>
  <span m="2214730">transitions.</span> <span m="2215720">So</span> <span m="2216230">what</span>
  <span m="2216560">state</span> <span m="2216950">will</span> <span m="2217130">I</span>
  <span m="2217220">end</span> <span m="2217400">up</span> <span m="2217580">in,</span>
  <span m="2217760">given</span> <span m="2218210">the</span> <span m="2218390">action</span>
  <span m="2218690">in</span> <span m="2218810">the</span> <span m="2218990">state</span>
  <span m="2219290">I'm</span> <span m="2219410">in</span> <span m="2219630">at</span>
  <span m="2219770">the</span> <span m="2219830">moment?</span> <span m="2221160">So</span>
  <span m="2221330">model-based</span> <span m="2221750">RL</span> <span m="2221990">tries</span>
  <span m="2222320">to</span> <span m="2222380">essentially</span> <span m="2222980">create</span>
  <span m="2223250">a</span> <span m="2223280">model</span> <span m="2223550">for</span>
  <span m="2223730">the</span> <span m="2223820">environment</span> <span m="2224390">or</span>
  <span m="2224510">of</span> <span m="2224720">the</span> <span m="2224840">environment.</span>
  <span m="2228740">There</span> <span m="2229130">are</span> <span m="2229190">several</span>
  <span m="2229580">examples</span> <span m="2230180">of</span> <span m="2230300">model-based</span>
  <span m="2230800">RL.</span> <span m="2231770">One</span> <span m="2231980">of</span>
  <span m="2232070">them</span> <span m="2232220">is</span> <span m="2232520">G-computation,</span>
  <span m="2233220">which</span> <span m="2233300">comes</span> <span m="2233570">out</span>
  <span m="2233690">of</span> <span m="2233750">the</span> <span m="2233930">statistic</span>
  <span m="2234410">literature,</span> <span m="2235340">if</span> <span m="2235460">you</span>
  <span m="2235520">like.</span> <span m="2235910">And</span> <span m="2236090">MDPs</span>
  <span m="2236900">are</span> <span m="2237050">essentially--</span> <span m="2239300">that's
  a</span> <span m="2239440">Markov</span> <span m="2239790">decision</span> <span
  m="2240140">process,</span> <span m="2240470">which</span> <span m="2240650">is</span>
  <span m="2240770">essentially</span> <span m="2241160">trying</span> <span m="2241460">to</span>
  <span m="2241550">estimate</span> <span m="2242000">the</span> <span m="2242150">whole</span>
  <span m="2242360">distribution</span> <span m="2242780">that</span> <span m="2242870">we</span>
  <span m="2242960">talked</span> <span m="2243230">about</span> <span m="2243410">before.</span></p><p><span
  m="2248620">There</span> <span m="2248770">are</span> <span m="2248810">various</span>
  <span m="2249560">ups</span> <span m="2249830">and</span> <span m="2249920">downsides</span>
  <span m="2250330">of</span> <span m="2250400">this.</span> <span m="2250580">We</span>
  <span m="2250700">won't</span> <span m="2250970">have</span> <span m="2251180">time</span>
  <span m="2251450">to</span> <span m="2251540">go</span> <span m="2251720">into</span>
  <span m="2251960">all</span> <span m="2252140">of</span> <span m="2252200">these</span>
  <span m="2252380">paradigms</span> <span m="2252770">today.</span> <span m="2253100">We</span>
  <span m="2253220">will</span> <span m="2253370">actually</span> <span m="2253640">focus</span>
  <span m="2254420">only</span> <span m="2254660">on</span> <span m="2254900">value-based</span>
  <span m="2255410">RL</span> <span m="2255650">today.</span> <span m="2258200">Yeah,</span>
  <span m="2258350">you</span> <span m="2258410">can</span> <span m="2258530">ask</span>
  <span m="2258650">me</span> <span m="2258740">offline</span> <span m="2259010">if</span>
  <span m="2259100">you</span> <span m="2259340">are</span> <span m="2259460">interested</span>
  <span m="2259790">in</span> <span m="2259850">model-based</span> <span m="2260210">RL.</span></p><p><span
  m="2261500">The</span> <span m="2261590">rightmost</span> <span m="2261980">one</span>
  <span m="2262160">here</span> <span m="2262240">is</span> <span m="2262430">policy-based</span>
  <span m="2262970">RL,</span> <span m="2264320">where</span> <span m="2264860">you</span>
  <span m="2265040">essentially</span> <span m="2265430">focus</span> <span m="2265760">only</span>
  <span m="2266000">on</span> <span m="2266120">modeling</span> <span m="2266720">the</span>
  <span m="2266870">policy</span> <span m="2270360">that</span> <span m="2270470">was</span>
  <span m="2270590">used</span> <span m="2270830">in</span> <span m="2270920">the</span>
  <span m="2271010">data</span> <span m="2271520">that</span> <span m="2271610">you</span>
  <span m="2271700">observed.</span> <span m="2272570">And</span> <span m="2272970">the</span>
  <span m="2273200">policy</span> <span m="2273620">that</span> <span m="2274580">you</span>
  <span m="2274670">want</span> <span m="2274940">to</span> <span m="2275060">essentially</span>
  <span m="2275660">arrive</span> <span m="2276050">at.</span> <span m="2276590">So</span>
  <span m="2276740">you're</span> <span m="2276920">optimizing</span> <span m="2277490">a</span>
  <span m="2277610">policy</span> <span m="2278030">and</span> <span m="2278150">you</span>
  <span m="2278390">are</span> <span m="2278570">estimating</span> <span m="2279080">a</span>
  <span m="2279140">policy</span> <span m="2279740">that</span> <span m="2279920">was</span>
  <span m="2280070">used</span> <span m="2280310">in</span> <span m="2280400">the</span>
  <span m="2280460">past.</span> <span m="2281570">And</span> <span m="2282620">the</span>
  <span m="2282740">middle</span> <span m="2283040">one</span> <span m="2283430">focuses</span>
  <span m="2283940">on</span> <span m="2284060">neither</span> <span m="2284420">of</span>
  <span m="2284540">those</span> <span m="2284990">and</span> <span m="2285500">focuses</span>
  <span m="2285800">on</span> <span m="2286280">only</span> <span m="2286610">estimating</span>
  <span m="2287000">the</span> <span m="2287120">return--</span> <span m="2287720">that</span>
  <span m="2287840">was</span> <span m="2287960">the</span> <span m="2288455">G.</span>
  <span m="2289445">Or the</span> <span m="2289940">reward</span> <span m="2290270">function</span>
  <span m="2290630">as</span> <span m="2290720">a</span> <span m="2290780">function</span>
  <span m="2291080">of</span> <span m="2291170">your</span> <span m="2291560">actions</span>
  <span m="2291950">and</span> <span m="2292040">states.</span></p><p><span m="2293120">And</span>
  <span m="2293270">it's</span> <span m="2293810">interesting</span> <span m="2294140">to</span>
  <span m="2294200">me</span> <span m="2294350">that</span> <span m="2294470">you</span>
  <span m="2294560">can</span> <span m="2294950">pick</span> <span m="2295610">any</span>
  <span m="2295970">of</span> <span m="2296210">the</span> <span m="2296660">variables--</span>
  <span m="2297260">A,</span> <span m="2297515">S,</span> <span m="2297770">and</span>
  <span m="2297870">R--</span> <span m="2298330">and</span> <span m="2298460">model</span>
  <span m="2298730">those.</span> <span m="2299180">And</span> <span m="2299300">you</span>
  <span m="2299390">can</span> <span m="2299510">arrive</span> <span m="2299780">at</span>
  <span m="2299840">something</span> <span m="2300170">reasonable</span> <span m="2300620">in</span>
  <span m="2300800">reinforcement</span> <span m="2301280">learning.</span> <span
  m="2302710">This</span> <span m="2302950">one</span> <span m="2303220">is</span>
  <span m="2303370">particularly</span> <span m="2303850">interesting,</span> <span
  m="2304330">because</span> <span m="2307600">it</span> <span m="2307660">doesn't</span>
  <span m="2307900">try</span> <span m="2308170">to</span> <span m="2308470">understand</span>
  <span m="2309010">how</span> <span m="2309400">do</span> <span m="2309460">you</span>
  <span m="2309670">arrive</span> <span m="2310060">at</span> <span m="2310150">a</span>
  <span m="2310180">certain</span> <span m="2311920">return</span> <span m="2312490">based</span>
  <span m="2312820">on</span> <span m="2312940">the</span> <span m="2313060">actions</span>
  <span m="2313390">in</span> <span m="2313450">the</span> <span m="2313540">states?</span>
  <span m="2313840">It's</span> <span m="2313960">just</span> <span m="2314350">optimize</span>
  <span m="2314750">the</span> <span m="2314830">policy</span> <span m="2315130">directly.</span>
  <span m="2315880">And</span> <span m="2316000">it</span> <span m="2316060">has</span>
  <span m="2316240">some</span> <span m="2316570">obvious--</span> <span m="2317110">well,</span>
  <span m="2317530">not</span> <span m="2317710">obvious,</span> <span m="2318140">but</span>
  <span m="2318220">it</span> <span m="2318340">has</span> <span m="2318490">some</span>
  <span m="2318610">downsides,</span> <span m="2319930">not</span> <span m="2320140">doing</span>
  <span m="2320420">that.</span></p><p><span m="2322010">OK,</span> <span m="2322450">anyway,</span>
  <span m="2322720">we're</span> <span m="2322810">going</span> <span m="2322890">to</span>
  <span m="2322990">focus</span> <span m="2323290">on</span> <span m="2323590">value-based</span>
  <span m="2324390">RL.</span> <span m="2324980">And</span> <span m="2325330">the</span>
  <span m="2325940">very</span> <span m="2326110">dominant</span> <span m="2327610">instantiation</span>
  <span m="2328420">of</span> <span m="2328480">value-based</span> <span m="2328960">RL</span>
  <span m="2329090">is</span> <span m="2329350">Q-learning.</span> <span m="2329920">I'm</span>
  <span m="2330010">sure</span> <span m="2330190">you've</span> <span m="2330340">heard</span>
  <span m="2330490">of</span> <span m="2330550">it.</span> <span m="2331870">It</span>
  <span m="2332020">is</span> <span m="2332140">what</span> <span m="2332320">drove</span>
  <span m="2332650">the</span> <span m="2333370">success</span> <span m="2333730">stories</span>
  <span m="2334030">that</span> <span m="2334150">I</span> <span m="2334330">showed</span>
  <span m="2334540">before,</span> <span m="2334990">the</span> <span m="2335740">goal</span>
  <span m="2336160">in</span> <span m="2336280">the</span> <span m="2336490">StarCraft</span>
  <span m="2337030">and</span> <span m="2337120">everything.</span> <span m="2338120">G-estimation</span>
  <span m="2339220">is</span> <span m="2339340">another</span> <span m="2339670">example</span>
  <span m="2340030">of</span> <span m="2340120">this,</span> <span m="2340420">which,</span>
  <span m="2340570">again,</span> <span m="2340810">has</span> <span m="2340900">come</span>
  <span m="2341170">from</span> <span m="2341320">the</span> <span m="2341410">statistic</span>
  <span m="2341850">literature.</span> <span m="2342670">But</span> <span m="2343210">we'll</span>
  <span m="2343360">focus</span> <span m="2343600">on</span> <span m="2343690">Q-learning</span>
  <span m="2344110">today.</span></p><p><span m="2346600">So</span> <span m="2347150">Q-learning</span>
  <span m="2347650">is</span> <span m="2347800">an</span> <span m="2348220">example</span>
  <span m="2348700">of</span> <span m="2348970">dynamic</span> <span m="2349390">programming,</span>
  <span m="2350210">in</span> <span m="2350400">some</span> <span m="2350620">sense.</span>
  <span m="2350890">That's</span> <span m="2351100">how</span> <span m="2351250">it's</span>
  <span m="2351400">usually</span> <span m="2351760">explained.</span> <span m="2352260">And</span>
  <span m="2352390">I</span> <span m="2352450">just</span> <span m="2352600">wanted</span>
  <span m="2352780">to</span> <span m="2352870">check--</span> <span m="2353140">how</span>
  <span m="2353230">many</span> <span m="2353410">have</span> <span m="2353530">heard</span>
  <span m="2353740">the</span> <span m="2353830">phrase</span> <span m="2354100">dynamic</span>
  <span m="2354400">programming</span> <span m="2354770">before?</span> <span m="2355930">OK,</span>
  <span m="2356420">great.</span> <span m="2358030">So</span> <span m="2359140">I</span>
  <span m="2359410">won't</span> <span m="2359560">go</span> <span m="2359650">into</span>
  <span m="2359830">details</span> <span m="2360130">of</span> <span m="2360330">dynamic</span>
  <span m="2360590">programming</span> <span m="2360940">in</span> <span m="2361030">general.</span>
  <span m="2361360">But</span> <span m="2361480">the</span> <span m="2361600">general</span>
  <span m="2362020">idea</span> <span m="2362770">is</span> <span m="2362950">one</span>
  <span m="2363100">of</span> <span m="2363220">recursion.</span></p><p><span m="2365950">In</span>
  <span m="2366220">this</span> <span m="2366430">case,</span> <span m="2367700">you</span>
  <span m="2368055">know</span> <span m="2368410">something about</span> <span m="2368770">what</span>
  <span m="2370120">is</span> <span m="2370210">a</span> <span m="2370270">good</span>
  <span m="2370450">terminal</span> <span m="2370840">state.</span> <span m="2371500">And</span>
  <span m="2371590">then</span> <span m="2371710">you</span> <span m="2371770">want</span>
  <span m="2371920">to</span> <span m="2371980">figure</span> <span m="2372190">out</span>
  <span m="2372340">how</span> <span m="2372430">to</span> <span m="2372520">get</span>
  <span m="2372730">there</span> <span m="2373090">and</span> <span m="2373690">how</span>
  <span m="2374170">to</span> <span m="2374260">get</span> <span m="2374410">to</span>
  <span m="2374530">the</span> <span m="2374620">state</span> <span m="2374860">before</span>
  <span m="2375160">that</span> <span m="2375340">and</span> <span m="2375460">the</span>
  <span m="2375550">state</span> <span m="2375730">before</span> <span m="2375970">that</span>
  <span m="2376090">and</span> <span m="2376180">so</span> <span m="2376370">on.</span>
  <span m="2377470">That</span> <span m="2377650">is</span> <span m="2377740">the</span>
  <span m="2377860">recursion</span> <span m="2378220">that</span> <span m="2378310">we're</span>
  <span m="2378520">talking</span> <span m="2378760">about.</span> <span m="2379990">The</span>
  <span m="2380140">end</span> <span m="2380290">state</span> <span m="2380500">that</span>
  <span m="2380620">is</span> <span m="2380710">the</span> <span m="2380800">best</span>
  <span m="2381160">here</span> <span m="2381430">is</span> <span m="2381580">fairly</span>
  <span m="2381850">obvious--</span> <span m="2382180">that</span> <span m="2382300">is</span>
  <span m="2382420">the</span> <span m="2382480">plus</span> <span m="2382795">1</span>
  <span m="2383110">here.</span></p><p><span m="2387130">The</span> <span m="2387250">only</span>
  <span m="2387550">way</span> <span m="2387670">to</span> <span m="2387790">get</span>
  <span m="2387970">there</span> <span m="2388150">is</span> <span m="2388340">by</span>
  <span m="2389830">stopping</span> <span m="2390370">here</span> <span m="2390610">first,</span>
  <span m="2390940">because</span> <span m="2391270">you</span> <span m="2391360">can't</span>
  <span m="2391630">move</span> <span m="2391810">from</span> <span m="2392020">here</span>
  <span m="2392260">since</span> <span m="2392460">it's</span> <span m="2392590">a</span>
  <span m="2392650">terminal</span> <span m="2392980">state.</span> <span m="2395170">Your</span>
  <span m="2395290">only</span> <span m="2395470">bet</span> <span m="2395710">is
  that</span> <span m="2395840">one.</span> <span m="2397010">And</span> <span m="2397120">then</span>
  <span m="2397210">we</span> <span m="2397300">can</span> <span m="2397420">ask</span>
  <span m="2397570">what</span> <span m="2397680">is</span> <span m="2397750">the</span>
  <span m="2397810">best</span> <span m="2398110">way</span> <span m="2398320">to</span>
  <span m="2398470">get</span> <span m="2398650">to</span> <span m="2398770">3,</span>
  <span m="2399070">1?</span> <span m="2399550">How</span> <span m="2399670">do</span>
  <span m="2399760">we</span> <span m="2399820">get</span> <span m="2399940">to</span>
  <span m="2400030">the</span> <span m="2400120">state</span> <span m="2400330">before</span>
  <span m="2400660">the</span> <span m="2400750">best</span> <span m="2400930">state?</span>
  <span m="2402100">Well,</span> <span m="2402850">we</span> <span m="2402970">can</span>
  <span m="2403090">say</span> <span m="2403300">that</span> <span m="2404170">one</span>
  <span m="2404440">way</span> <span m="2404740">is</span> <span m="2405700">go</span>
  <span m="2405820">from</span> <span m="2405970">here.</span> <span m="2406370">And</span>
  <span m="2406470">one</span> <span m="2406570">way</span> <span m="2406690">from</span>
  <span m="2406900">here.</span></p><p><span m="2407470">And</span> <span m="2407610">as</span>
  <span m="2407740">we</span> <span m="2407830">got</span> <span m="2407980">from</span>
  <span m="2408130">the</span> <span m="2408250">audience</span> <span m="2408550">before,</span>
  <span m="2409300">this</span> <span m="2409510">is</span> <span m="2409630">a</span>
  <span m="2409690">slightly</span> <span m="2410200">worse</span> <span m="2410560">way</span>
  <span m="2411010">to</span> <span m="2411130">get</span> <span m="2411490">there</span>
  <span m="2412270">then</span> <span m="2412600">from</span> <span m="2412870">there,</span>
  <span m="2413410">because</span> <span m="2413740">here</span> <span m="2413980">we</span>
  <span m="2414100">have</span> <span m="2414740">a</span> <span m="2414790">possibility</span>
  <span m="2415330">of</span> <span m="2415450">ending</span> <span m="2415690">up</span>
  <span m="2415810">in</span> <span m="2415900">minus</span> <span m="2416180">1.</span>
  <span m="2417950">So then</span> <span m="2418100">we</span> <span m="2418460">recurse</span>
  <span m="2419330">further</span> <span m="2420170">and</span> <span m="2420290">essentially,</span>
  <span m="2421010">we</span> <span m="2421130">end</span> <span m="2421220">up</span>
  <span m="2421340">with</span> <span m="2421430">something</span> <span m="2421700">like</span>
  <span m="2421850">this</span> <span m="2422370">that</span> <span m="2422570">says--</span>
  <span m="2425860">or</span> <span m="2426010">what</span> <span m="2426230">I</span>
  <span m="2426440">tried</span> <span m="2426620">to</span> <span m="2426710">illustrate</span>
  <span m="2427040">here</span> <span m="2427220">is</span> <span m="2427370">that</span>
  <span m="2427930">the</span> <span m="2428180">green</span> <span m="2428510">boxes--</span>
  <span m="2430160">I'm</span> <span m="2430310">sorry</span> <span m="2430580">for</span>
  <span m="2430910">any</span> <span m="2431470">colorblind</span> <span m="2432410">members</span>
  <span m="2432800">of</span> <span m="2432890">the</span> <span m="2432980">audience,</span>
  <span m="2433340">because</span> <span m="2433640">this</span> <span m="2433820">was</span>
  <span m="2434460">a</span> <span m="2434530">poor</span> <span m="2434720">choice</span>
  <span m="2434990">of</span> <span m="2435050">mine.</span> <span m="2435870">Anyway,</span>
  <span m="2436310">this</span> <span m="2436700">bottom</span> <span m="2437030">side</span>
  <span m="2437300">here</span> <span m="2437420">is</span> <span m="2437540">mostly</span>
  <span m="2437870">red</span> <span m="2438110">and</span> <span m="2438230">this</span>
  <span m="2438380">is</span> <span m="2438470">mostly</span> <span m="2438770">green.</span>
  <span m="2439490">And</span> <span m="2439760">you</span> <span m="2439880">can</span>
  <span m="2440000">follow</span> <span m="2440300">the</span> <span m="2440390">green</span>
  <span m="2440630">color</span> <span m="2440900">here,</span> <span m="2441200">essentially,</span>
  <span m="2441620">to</span> <span m="2441740">get</span> <span m="2441950">to</span>
  <span m="2442130">the</span> <span m="2442640">best</span> <span m="2442940">end</span>
  <span m="2443120">state.</span></p><p><span m="2445460">And</span> <span m="2445790">what</span>
  <span m="2446030">I</span> <span m="2446120">used</span> <span m="2446510">here</span>
  <span m="2446750">to</span> <span m="2447200">color</span> <span m="2447530">this</span>
  <span m="2447730">in</span> <span m="2447950">is</span> <span m="2448040">this</span>
  <span m="2448280">idea</span> <span m="2448670">of</span> <span m="2449330">knowing</span>
  <span m="2449690">how</span> <span m="2449930">good</span> <span m="2450200">a</span>
  <span m="2450230">state</span> <span m="2450560">is,</span> <span m="2450860">depending</span>
  <span m="2451400">on</span> <span m="2452090">how</span> <span m="2452270">good</span>
  <span m="2452480">the</span> <span m="2452570">state</span> <span m="2453020">after</span>
  <span m="2453410">that</span> <span m="2453590">state is.</span> <span m="2454550">So</span>
  <span m="2454610">I</span> <span m="2454700">knew</span> <span m="2455060">that</span>
  <span m="2455270">plus</span> <span m="2455600">1</span> <span m="2455960">is</span>
  <span m="2456080">a</span> <span m="2456140">good</span> <span m="2456320">end</span>
  <span m="2456470">state</span> <span m="2456770">over</span> <span m="2456980">there.</span>
  <span m="2457960">And</span> <span m="2458120">that</span> <span m="2458300">led</span>
  <span m="2458510">me</span> <span m="2458630">to</span> <span m="2459740">recurse</span>
  <span m="2460160">backwards,</span> <span m="2460690">essentially.</span></p><p><span
  m="2463870">So</span> <span m="2464370">the</span> <span m="2464460">question,</span>
  <span m="2464850">then,</span> <span m="2465000">is</span> <span m="2465180">how</span>
  <span m="2467340">do</span> <span m="2467430">we</span> <span m="2467520">know</span>
  <span m="2468330">that</span> <span m="2468750">that</span> <span m="2469080">state</span>
  <span m="2469410">over</span> <span m="2469590">there</span> <span m="2469740">is</span>
  <span m="2469860">a</span> <span m="2469920">good</span> <span m="2470100">one?</span>
  <span m="2470400">When</span> <span m="2470550">we</span> <span m="2470670">have</span>
  <span m="2470800">it</span> <span m="2470980">visualized</span> <span m="2471420">in</span>
  <span m="2471510">front</span> <span m="2471720">of</span> <span m="2471810">us,</span>
  <span m="2471960">it's</span> <span m="2472140">very</span> <span m="2472410">easy</span>
  <span m="2472620">to</span> <span m="2472710">see.</span> <span m="2473340">And</span>
  <span m="2473520">it's</span> <span m="2473610">very</span> <span m="2473820">easy</span>
  <span m="2474060">because</span> <span m="2474360">we</span> <span m="2474480">know</span>
  <span m="2474750">that</span> <span m="2475170">plus</span> <span m="2475470">1</span>
  <span m="2475680">is</span> <span m="2475850">a</span> <span m="2475920">terminal</span>
  <span m="2476310">state</span> <span m="2476580">here.</span> <span m="2476730">It</span>
  <span m="2476880">ends</span> <span m="2477210">there,</span> <span m="2477660">so</span>
  <span m="2478680">those</span> <span m="2479100">are</span> <span m="2479160">the</span>
  <span m="2479280">only</span> <span m="2479850">states</span> <span m="2480120">we</span>
  <span m="2480180">need</span> <span m="2480300">to</span> <span m="2480360">consider</span>
  <span m="2480660">in</span> <span m="2480750">this</span> <span m="2480870">case.</span>
  <span m="2481680">But</span> <span m="2482100">more</span> <span m="2482280">in</span>
  <span m="2482400">general,</span> <span m="2482940">how</span> <span m="2483240">do</span>
  <span m="2483330">we</span> <span m="2483510">learn</span> <span m="2485370">what</span>
  <span m="2485580">is</span> <span m="2485820">the</span> <span m="2485940">value</span>
  <span m="2486990">of</span> <span m="2487140">a</span> <span m="2487170">state?</span>
  <span m="2488520">That</span> <span m="2488640">will</span> <span m="2488760">be</span>
  <span m="2488880">the</span> <span m="2488970">purpose</span> <span m="2489300">of</span>
  <span m="2489450">Q-learning.</span></p><p><span m="2492730">If</span> <span m="2492940">we</span>
  <span m="2493090">have</span> <span m="2493420">an</span> <span m="2493510">idea</span>
  <span m="2493780">of</span> <span m="2493900">what</span> <span m="2494110">is</span>
  <span m="2494380">a</span> <span m="2494470">good</span> <span m="2494740">state,</span>
  <span m="2495040">we</span> <span m="2495130">can</span> <span m="2495250">always</span>
  <span m="2497860">do</span> <span m="2498130">that</span> <span m="2498310">recursion</span>
  <span m="2498730">that</span> <span m="2498850">I</span> <span m="2498940">explained</span>
  <span m="2499300">very</span> <span m="2499510">briefly.</span> <span m="2500260">You</span>
  <span m="2500350">find</span> <span m="2500720">a</span> <span m="2500800">state</span>
  <span m="2501190">that</span> <span m="2501520">has</span> <span m="2501710">the</span>
  <span m="2501790">high</span> <span m="2502120">value</span> <span m="2502900">and</span>
  <span m="2503020">you</span> <span m="2503140">figure</span> <span m="2503410">out</span>
  <span m="2503560">how</span> <span m="2503770">to</span> <span m="2503890">get</span>
  <span m="2504070">there.</span> <span m="2507930">So</span> <span m="2508080">we're</span>
  <span m="2508350">going</span> <span m="2508450">to</span> <span m="2508560">have</span>
  <span m="2508650">to</span> <span m="2508740">define</span> <span m="2509270">now</span>
  <span m="2511750">what</span> <span m="2512290">I</span> <span m="2512380">mean</span>
  <span m="2512560">by</span> <span m="2512710">value.</span> <span m="2513070">I've</span>
  <span m="2513160">used</span> <span m="2513340">that</span> <span m="2513460">word</span>
  <span m="2514210">a</span> <span m="2514270">few</span> <span m="2514450">different</span>
  <span m="2514660">times.</span> <span m="2516970">I</span> <span m="2517060">say</span>
  <span m="2517240">recall</span> <span m="2517660">here,</span> <span m="2517810">but</span>
  <span m="2517920">I</span> <span m="2517960">don't</span> <span m="2518140">know</span>
  <span m="2518230">if</span> <span m="2518350">I</span> <span m="2518440">actually</span>
  <span m="2518740">had</span> <span m="2518920">it</span> <span m="2519010">on</span>
  <span m="2519100">a</span> <span m="2519160">slide</span> <span m="2519430">before.</span></p><p><span
  m="2519830">So</span> <span m="2520150">let's</span> <span m="2520390">just</span>
  <span m="2520570">say</span> <span m="2521290">this</span> <span m="2521470">is</span>
  <span m="2521560">the</span> <span m="2521680">definition</span> <span m="2522160">of</span>
  <span m="2522250">value</span> <span m="2522670">that</span> <span m="2522760">we</span>
  <span m="2522860">will</span> <span m="2523000">be</span> <span m="2523090">working</span>
  <span m="2523390">with.</span> <span m="2527340">I</span> <span m="2527440">think</span>
  <span m="2527480">I</span> <span m="2527570">had</span> <span m="2527690">it</span>
  <span m="2527780">on a</span> <span m="2527900">slide</span> <span m="2527990">before,</span>
  <span m="2528400">actually.</span> <span m="2529050">This</span> <span m="2529130">is</span>
  <span m="2529460">the</span> <span m="2529640">expected</span> <span m="2530360">return.</span>
  <span m="2531050">Remember,</span> <span m="2531410">this</span> <span m="2531800">G</span>
  <span m="2532100">here</span> <span m="2532280">was</span> <span m="2532410">the</span>
  <span m="2532490">sum of</span> <span m="2532850">rewards</span> <span m="2533690">going</span>
  <span m="2533990">into</span> <span m="2534200">the</span> <span m="2534320">future,</span>
  <span m="2535160">starting</span> <span m="2535580">at</span> <span m="2535670">time,</span>
  <span m="2535940">t.</span> <span m="2537470">And</span> <span m="2539300">the</span>
  <span m="2539420">value,</span> <span m="2539780">then,</span> <span m="2539930">of</span>
  <span m="2540020">this</span> <span m="2540140">state</span> <span m="2540680">is</span>
  <span m="2540860">the</span> <span m="2540950">expectation</span> <span m="2541460">of</span>
  <span m="2541550">such</span> <span m="2541730">returns.</span></p><p><span m="2545690">Before,</span>
  <span m="2546080">I</span> <span m="2546140">said</span> <span m="2546290">that</span>
  <span m="2546410">the</span> <span m="2546500">value</span> <span m="2546800">of</span>
  <span m="2546890">an</span> <span m="2546950">policy</span> <span m="2548000">was</span>
  <span m="2548570">the</span> <span m="2548960">expectation</span> <span m="2549770">of</span>
  <span m="2550250">returns,</span> <span m="2550760">period.</span> <span m="2552140">And</span>
  <span m="2552230">the</span> <span m="2553130">value</span> <span m="2553430">of</span>
  <span m="2553520">a</span> <span m="2553580">state</span> <span m="2554180">and</span>
  <span m="2554270">the</span> <span m="2554360">policy</span> <span m="2554900">is</span>
  <span m="2555050">the</span> <span m="2555140">value</span> <span m="2556100">of</span>
  <span m="2556410">that</span> <span m="2556640">return</span> <span m="2556980">starting</span>
  <span m="2557510">in</span> <span m="2557600">a</span> <span m="2557660">certain</span>
  <span m="2557960">state.</span> <span m="2561220">We</span> <span m="2561340">can</span>
  <span m="2562060">stratify</span> <span m="2562630">this</span> <span m="2562810">further</span>
  <span m="2563170">if</span> <span m="2563310">we</span> <span m="2563410">like</span>
  <span m="2563810">and</span> <span m="2563830">say</span> <span m="2564010">that</span>
  <span m="2564130">the</span> <span m="2564220">value</span> <span m="2564550">of</span>
  <span m="2564640">a</span> <span m="2564670">state</span> <span m="2565120">action</span>
  <span m="2565480">pair</span> <span m="2567090">is</span> <span m="2567270">the</span>
  <span m="2567420">expected</span> <span m="2567930">return,</span> <span m="2568800">starting</span>
  <span m="2569520">in</span> <span m="2569640">a</span> <span m="2569700">certain</span>
  <span m="2569970">state</span> <span m="2570270">and</span> <span m="2570450">taking</span>
  <span m="2570810">an</span> <span m="2570930">action,</span> <span m="2571320">a.</span>
  <span m="2571580">And</span> <span m="2571980">after</span> <span m="2572370">that,</span>
  <span m="2572700">following</span> <span m="2573240">the</span> <span m="2573330">policy,</span>
  <span m="2573690">pi.</span></p><p><span m="2575990">This</span> <span m="2576170">would</span>
  <span m="2576260">be</span> <span m="2577990">the</span> <span m="2578210">so-called</span>
  <span m="2578600">Q</span> <span m="2578870">value</span> <span m="2579260">of a</span>
  <span m="2579530">state-action</span> <span m="2580100">pair--</span> <span m="2580460">s,</span>
  <span m="2580790">a.</span> <span m="2583650">And</span> <span m="2583770">this</span>
  <span m="2583920">is</span> <span m="2584010">where</span> <span m="2584670">Q-learning</span>
  <span m="2585180">gets</span> <span m="2585330">its</span> <span m="2585450">name.</span>
  <span m="2587540">So</span> <span m="2588180">Q-learning</span> <span m="2588920">attempts</span>
  <span m="2589370">to</span> <span m="2589520">estimate</span> <span m="2590960">the</span>
  <span m="2591050">Q</span> <span m="2591350">function--</span> <span m="2592100">the</span>
  <span m="2592190">expected</span> <span m="2592610">return</span> <span m="2593000">starting</span>
  <span m="2593600">in</span> <span m="2593750">a</span> <span m="2593810">state,</span>
  <span m="2594080">s,</span> <span m="2594280">and</span> <span m="2594380">taking</span>
  <span m="2594620">action,</span> <span m="2594860">a--</span> <span m="2597920">from</span>
  <span m="2598190">data.</span></p><p><span m="2602090">The</span> <span m="2602210">Q-learning</span>
  <span m="2602510">is</span> <span m="2602720">also</span> <span m="2603080">associated</span>
  <span m="2603740">with</span> <span m="2603920">a</span> <span m="2604340">deterministic</span>
  <span m="2605060">policy.</span> <span m="2606050">So</span> <span m="2606200">the</span>
  <span m="2606290">policy</span> <span m="2607220">and</span> <span m="2607340">the</span>
  <span m="2607430">Q</span> <span m="2607700">function</span> <span m="2608030">go</span>
  <span m="2608240">together</span> <span m="2608840">in</span> <span m="2609020">this</span>
  <span m="2609170">specific</span> <span m="2609680">way.</span> <span m="2610740">If</span>
  <span m="2610820">we</span> <span m="2610940">have</span> <span m="2611360">a</span>
  <span m="2611570">Q</span> <span m="2611630">function,</span> <span m="2612290">Q,</span>
  <span m="2612590">that</span> <span m="2612740">tries</span> <span m="2613040">to</span>
  <span m="2613160">estimate</span> <span m="2613550">the</span> <span m="2613670">value</span>
  <span m="2614180">of</span> <span m="2614330">a</span> <span m="2614780">policy,</span>
  <span m="2615260">pi,</span> <span m="2616250">the</span> <span m="2616340">pi</span>
  <span m="2616760">itself</span> <span m="2617240">is</span> <span m="2617330">the</span>
  <span m="2617450">arg</span> <span m="2617740">max</span> <span m="2618320">according</span>
  <span m="2618620">to</span> <span m="2618740">that</span> <span m="2618920">Q.</span>
  <span m="2619660">It</span> <span m="2619730">sounds</span> <span m="2619940">a</span>
  <span m="2619970">little</span> <span m="2620090">recursive,</span> <span m="2620750">but</span>
  <span m="2621110">hopefully</span> <span m="2621460">it will</span> <span m="2621620">be</span>
  <span m="2621740">OK.</span></p><p><span m="2624010">Maybe</span> <span m="2624260">it's</span>
  <span m="2624380">more</span> <span m="2624560">obvious</span> <span m="2624890">if</span>
  <span m="2625010">we</span> <span m="2625070">look</span> <span m="2625280">here.</span>
  <span m="2626090">So</span> <span m="2626360">Q,</span> <span m="2626750">I</span>
  <span m="2626930">said</span> <span m="2627140">before,</span> <span m="2627630">was</span>
  <span m="2627680">the</span> <span m="2627770">value</span> <span m="2628130">of</span>
  <span m="2628190">starting</span> <span m="2628490">an</span> <span m="2628590">s,</span>
  <span m="2628790">taking</span> <span m="2629060">action,</span> <span m="2629390">a,</span>
  <span m="2629870">and then</span> <span m="2630020">following</span> <span m="2630560">policy,</span>
  <span m="2630920">pi.</span> <span m="2633560">This</span> <span m="2633740">is</span>
  <span m="2633860">defined</span> <span m="2634310">by</span> <span m="2634790">the</span>
  <span m="2635990">decision</span> <span m="2636350">process</span> <span m="2636650">itself.</span></p><p><span
  m="2637670">The</span> <span m="2637760">best</span> <span m="2638630">pi,</span>
  <span m="2640140">the</span> <span m="2640230">best</span> <span m="2640440">policy,</span>
  <span m="2640950">is</span> <span m="2641070">the</span> <span m="2641130">one</span>
  <span m="2641280">that</span> <span m="2641400">has</span> <span m="2641520">the</span>
  <span m="2641610">highest</span> <span m="2641910">Q.</span> <span m="2642750">And</span>
  <span m="2642870">this</span> <span m="2643020">is</span> <span m="2643110">what</span>
  <span m="2643230">we</span> <span m="2643320">call</span> <span m="2643530">a</span>
  <span m="2643560">Q-star.</span> <span m="2646540">Well,</span> <span m="2646900">that</span>
  <span m="2647060">is</span> <span m="2647160">not</span> <span m="2647280">what</span>
  <span m="2647370">we</span> <span m="2647460">call</span> <span m="2647610">Q-star,</span>
  <span m="2647940">that</span> <span m="2648120">is what we</span> <span m="2648210">call</span>
  <span m="2648495">little</span> <span m="2648780">q-star.</span> <span m="2650030">Q-star,</span>
  <span m="2650550">the</span> <span m="2650640">best</span> <span m="2651000">estimate</span>
  <span m="2651450">of</span> <span m="2651540">this,</span> <span m="2651720">is</span>
  <span m="2651840">obviously</span> <span m="2652230">the</span> <span m="2652320">thing</span>
  <span m="2652530">itself.</span></p><p><span m="2653320">So</span> <span m="2653460">if</span>
  <span m="2653640">you</span> <span m="2653730">can</span> <span m="2653850">find</span>
  <span m="2654150">a</span> <span m="2654210">good</span> <span m="2654480">function</span>
  <span m="2655320">that</span> <span m="2655440">assigns</span> <span m="2655860">a</span>
  <span m="2655920">value</span> <span m="2656400">to</span> <span m="2656580">a</span>
  <span m="2656640">state-action</span> <span m="2657150">pair,</span> <span m="2657780">the</span>
  <span m="2657870">best</span> <span m="2658230">such</span> <span m="2658530">function</span>
  <span m="2658830">you</span> <span m="2658920">can</span> <span m="2659070">get</span>
  <span m="2659310">is</span> <span m="2659430">the</span> <span m="2659520">one</span>
  <span m="2659760">that</span> <span m="2660360">is</span> <span m="2660450">equal</span>
  <span m="2660750">to</span> <span m="2660900">little</span> <span m="2661110">q-star.</span>
  <span m="2664270">I hope</span> <span m="2664420">that</span> <span m="2664510">wasn't</span>
  <span m="2664720">too</span> <span m="2664840">confusing.</span> <span m="2666670">I'll
  show</span> <span m="2667000">on</span> <span m="2667090">the</span> <span m="2667150">next</span>
  <span m="2667360">slide</span> <span m="2667500">why</span> <span m="2667720">that</span>
  <span m="2667780">might</span> <span m="2667930">be</span> <span m="2668050">reasonable.</span></p><p><span
  m="2670300">So</span> <span m="2670690">Q-learning</span> <span m="2671220">is</span>
  <span m="2671340">based</span> <span m="2671700">on</span> <span m="2673170">a</span>
  <span m="2673260">general</span> <span m="2673860">idea</span> <span m="2674190">from</span>
  <span m="2674340">dynamic</span> <span m="2674700">programming,</span> <span m="2675250">which</span>
  <span m="2675390">is</span> <span m="2676380">the</span> <span m="2676750">so-called</span>
  <span m="2678880">Bellman</span> <span m="2679150">question.</span> <span m="2679450">There</span>
  <span m="2679570">we</span> <span m="2679630">go.</span> <span m="2686680">This</span>
  <span m="2686920">is</span> <span m="2687010">an</span> <span m="2687580">instantiation</span>
  <span m="2688120">of</span> <span m="2688180">Bellman</span> <span m="2688500">optimality,</span>
  <span m="2688960">which</span> <span m="2689230">says</span> <span m="2689530">that</span>
  <span m="2693700">the</span> <span m="2693820">best</span> <span m="2694510">state-action</span>
  <span m="2695620">value</span> <span m="2695950">function</span> <span m="2696790">has</span>
  <span m="2696970">the</span> <span m="2697060">property</span> <span m="2697660">that</span>
  <span m="2698510">it</span> <span m="2698670">is</span> <span m="2698830">equal</span>
  <span m="2699340">to</span> <span m="2700540">the</span> <span m="2700660">immediate</span>
  <span m="2701200">reward</span> <span m="2701710">of</span> <span m="2701830">taking</span>
  <span m="2702250">action,</span> <span m="2702580">a,</span> <span m="2702900">and
  state,</span> <span m="2703210">s,</span> <span m="2704050">plus</span> <span m="2704860">this,</span>
  <span m="2705910">which</span> <span m="2706150">is</span> <span m="2706270">the</span>
  <span m="2706360">maximum</span> <span m="2707020">Q</span> <span m="2707290">value</span>
  <span m="2707770">for</span> <span m="2708010">the</span> <span m="2708100">next</span>
  <span m="2708370">state.</span></p><p><span m="2709130">So</span> <span m="2709230">we're</span>
  <span m="2709330">going</span> <span m="2709430">to</span> <span m="2709530">stare</span>
  <span m="2709590">at</span> <span m="2709660">this</span> <span m="2709810">for</span>
  <span m="2709900">a</span> <span m="2709930">bit,</span> <span m="2710170">because</span>
  <span m="2712230">there's</span> <span m="2712430">a bit</span> <span m="2712570">here</span>
  <span m="2712690">to</span> <span m="2712810">digest.</span> <span m="2714500">Remember,</span>
  <span m="2714820">q-star</span> <span m="2715570">assigns</span> <span m="2715930">a</span>
  <span m="2715990">value</span> <span m="2716380">to</span> <span m="2716500">any</span>
  <span m="2716740">state</span> <span m="2716980">action</span> <span m="2717250">pair.</span>
  <span m="2719390">So</span> <span m="2719540">we</span> <span m="2719660">have</span>
  <span m="2719810">q-star</span> <span m="2720200">here,</span> <span m="2720440">we</span>
  <span m="2720560">have</span> <span m="2720680">q-star</span> <span m="2721100">here.</span>
  <span m="2722160">This</span> <span m="2722330">thing</span> <span m="2722540">here</span>
  <span m="2723230">is</span> <span m="2723320">supposed</span> <span m="2723740">to</span>
  <span m="2723830">represent</span> <span m="2724280">the</span> <span m="2724370">value</span>
  <span m="2724760">going</span> <span m="2725030">forward</span> <span m="2725480">in</span>
  <span m="2725570">time</span> <span m="2726380">after</span> <span m="2726770">I've</span>
  <span m="2726920">made</span> <span m="2727550">this</span> <span m="2727820">choice,</span>
  <span m="2728330">action,</span> <span m="2728870">a,</span> <span m="2729260">and
  state,</span> <span m="2729650">s.</span></p><p><span m="2733470">If</span> <span
  m="2733650">I</span> <span m="2733710">have</span> <span m="2733890">a</span> <span
  m="2733950">good</span> <span m="2734160">idea</span> <span m="2734490">of</span>
  <span m="2734640">how</span> <span m="2734880">good</span> <span m="2735150">it</span>
  <span m="2735270">is</span> <span m="2735870">to</span> <span m="2735990">take</span>
  <span m="2736470">action,</span> <span m="2736790">a,</span> <span m="2737030">instead</span>
  <span m="2737220">of s,</span> <span m="2737850">it</span> <span m="2737970">should</span>
  <span m="2738330">both</span> <span m="2738930">incorporate</span> <span m="2739380">the</span>
  <span m="2739470">immediate</span> <span m="2739830">reward</span> <span m="2740130">that</span>
  <span m="2740250">I</span> <span m="2740310">get--</span> <span m="2740520">that's</span>
  <span m="2740730">RT--</span> <span m="2741600">and</span> <span m="2741960">how</span>
  <span m="2742200">good</span> <span m="2742410">that</span> <span m="2742530">choice</span>
  <span m="2742860">was</span> <span m="2743160">going</span> <span m="2743400">forward.</span>
  <span m="2744220">So</span> <span m="2744240">think</span> <span m="2744420">about</span>
  <span m="2744600">mechanical</span> <span m="2745020">ventilation,</span> <span
  m="2745560">as</span> <span m="2745680">I</span> <span m="2745740">said</span> <span
  m="2745890">before.</span> <span m="2746590">If</span> <span m="2746690">we</span>
  <span m="2746790">put</span> <span m="2746850">a</span> <span m="2746910">patient</span>
  <span m="2747180">on</span> <span m="2747240">mechanical</span> <span m="2747600">ventilation,</span>
  <span m="2748350">we</span> <span m="2748440">have</span> <span m="2748530">to</span>
  <span m="2748620">do</span> <span m="2748740">a</span> <span m="2748800">bunch</span>
  <span m="2749010">of</span> <span m="2749100">other</span> <span m="2749280">things</span>
  <span m="2749700">after</span> <span m="2750000">that.</span> <span m="2750720">If</span>
  <span m="2750870">none</span> <span m="2751140">of</span> <span m="2751230">those</span>
  <span m="2751440">other</span> <span m="2751680">things</span> <span m="2752040">lead</span>
  <span m="2752520">to</span> <span m="2752760">a</span> <span m="2752820">good</span>
  <span m="2753000">outcome,</span> <span m="2753930">this</span> <span m="2754170">part</span>
  <span m="2754440">will</span> <span m="2754560">be</span> <span m="2754710">low.</span>
  <span m="2756630">Even</span> <span m="2756840">if</span> <span m="2756960">the</span>
  <span m="2757020">immediate</span> <span m="2757410">return</span> <span m="2757710">is</span>
  <span m="2757830">good.</span></p><p><span m="2759620">So</span> <span m="2760380">for</span>
  <span m="2760740">the</span> <span m="2760980">optimal</span> <span m="2761610">q-star,</span>
  <span m="2762750">this</span> <span m="2763050">quantity</span> <span m="2763470">holds.</span>
  <span m="2763710">We</span> <span m="2763860">know</span> <span m="2764100">that--</span>
  <span m="2764250">we</span> <span m="2764340">can</span> <span m="2764460">prove</span>
  <span m="2764700">that.</span> <span m="2765840">So</span> <span m="2765960">the</span>
  <span m="2766050">question</span> <span m="2766410">is</span> <span m="2766660">how</span>
  <span m="2766800">do</span> <span m="2766890">we</span> <span m="2767070">find</span>
  <span m="2767460">this</span> <span m="2767640">thing?</span> <span m="2767820">How</span>
  <span m="2767970">do we</span> <span m="2768090">find</span> <span m="2768420">q-star?</span>
  <span m="2769290">Because</span> <span m="2769620">q-star</span> <span m="2770000">is</span>
  <span m="2770100">not</span> <span m="2770280">only</span> <span m="2771120">the</span>
  <span m="2771240">thing</span> <span m="2771480">that</span> <span m="2771600">gives</span>
  <span m="2771840">you</span> <span m="2771930">the</span> <span m="2772050">optimal</span>
  <span m="2772380">policy--</span> <span m="2773070">it</span> <span m="2773190">also</span>
  <span m="2773460">satisfied</span> <span m="2773970">this</span> <span m="2774120">equality.</span></p><p><span
  m="2776230">This</span> <span m="2776310">is</span> <span m="2776370">not</span>
  <span m="2776520">true</span> <span m="2776670">for</span> <span m="2776820">every</span>
  <span m="2777030">Q</span> <span m="2777210">function,</span> <span m="2777570">but</span>
  <span m="2777690">it's</span> <span m="2777870">true</span> <span m="2778080">for</span>
  <span m="2778200">the</span> <span m="2778290">optimal</span> <span m="2778620">one.</span>
  <span m="2781460">Questions?</span> <span m="2786990">If</span> <span m="2787110">you</span>
  <span m="2787200">haven't</span> <span m="2787380">seen</span> <span m="2787550">this</span>
  <span m="2787630">before,</span> <span m="2787920">it</span> <span m="2788010">might</span>
  <span m="2788160">be</span> <span m="2788370">a</span> <span m="2789210">little</span>
  <span m="2789510">tough</span> <span m="2789750">to</span> <span m="2789870">digest.</span></p><p><span
  m="2792130">Is</span> <span m="2792410">the</span> <span m="2792500">notation</span>
  <span m="2792920">clear?</span> <span m="2793130">Essentially,</span> <span m="2793490">here</span>
  <span m="2793760">you</span> <span m="2793880">have</span> <span m="2794280">the</span>
  <span m="2794420">state</span> <span m="2794750">that</span> <span m="2794870">you</span>
  <span m="2794960">are</span> <span m="2795080">arriving</span> <span m="2795380">at</span>
  <span m="2795470">the</span> <span m="2795560">next</span> <span m="2795830">time.</span>
  <span m="2796780">A</span> <span m="2796910">prime</span> <span m="2797220">is</span>
  <span m="2797970">the</span> <span m="2799100">parameter</span> <span m="2799490">of</span>
  <span m="2799610">this</span> <span m="2799820">here,</span> <span m="2800060">or</span>
  <span m="2800180">the</span> <span m="2800300">argument</span> <span m="2800570">to</span>
  <span m="2800690">this.</span> <span m="2800990">You're</span> <span m="2801140">taking</span>
  <span m="2801500">the</span> <span m="2801620">best</span> <span m="2802130">possible</span>
  <span m="2802580">q-star</span> <span m="2803810">value</span> <span m="2804440">and</span>
  <span m="2804530">then</span> <span m="2804680">state</span> <span m="2804950">that</span>
  <span m="2805040">you</span> <span m="2805160">arrive</span> <span m="2805400">at</span>
  <span m="2805460">after.</span> <span m="2805800">Yeah,</span> <span m="2805910">go</span>
  <span m="2806250">ahead.</span></p><p><span m="2806390">AUDIENCE:</span> <span m="2806495">Can</span>
  <span m="2806600">you</span> <span m="2806705">instantiate</span> <span m="2807230">an
  example</span> <span m="2807570">you</span> <span m="2807650">have</span> <span
  m="2807730">on</span> <span m="2807800">the</span> <span m="2807870">board?</span></p><p><span
  m="2809105">FREDRIK D. JOHANSSON:</span> <span m="2809182">Yes.</span> <span m="2809570">Actually,</span>
  <span m="2809960">I</span> <span m="2810050">might</span> <span m="2810500">do</span>
  <span m="2810830">a</span> <span m="2810950">full</span> <span m="2811400">example</span>
  <span m="2811910">of</span> <span m="2812030">Q-learning</span> <span m="2812840">in</span>
  <span m="2812990">a</span> <span m="2813050">second.</span> <span m="2813530">Yes,</span>
  <span m="2813830">I</span> <span m="2813890">will.</span> <span m="2814760">I'll</span>
  <span m="2814940">get</span> <span m="2815090">to</span> <span m="2815180">that</span>
  <span m="2815330">example</span> <span m="2815732">then.</span></p><p><span m="2820670">Yeah,</span>
  <span m="2820850">I</span> <span m="2820910">was</span> <span m="2821210">debating</span>
  <span m="2821630">whether</span> <span m="2821750">to</span> <span m="2821800">do</span>
  <span m="2821960">that.</span> <span m="2822120">It might</span> <span m="2822290">take</span>
  <span m="2822440">some</span> <span m="2822560">time,</span> <span m="2822840">but</span>
  <span m="2822940">it</span> <span m="2823040">could</span> <span m="2823140">be</span>
  <span m="2823240">useful.</span> <span m="2824090">So</span> <span m="2824330">where</span>
  <span m="2824570">are</span> <span m="2824690">we?</span></p><p><span m="2829510">So</span>
  <span m="2830560">what</span> <span m="2830710">I</span> <span m="2830800">showed</span>
  <span m="2831040">you</span> <span m="2831100">before--</span> <span m="2831460">the</span>
  <span m="2831580">Bellman</span> <span m="2831880">inequality.</span> <span m="2832930">We</span>
  <span m="2833080">know</span> <span m="2833320">that</span> <span m="2833410">this</span>
  <span m="2833590">holds</span> <span m="2833890">for</span> <span m="2834010">the</span>
  <span m="2834130">optimal</span> <span m="2834460">thing.</span> <span m="2834880">And</span>
  <span m="2835300">if</span> <span m="2835510">there</span> <span m="2835710">is</span>
  <span m="2836140">a</span> <span m="2836260">quality</span> <span m="2836680">that</span>
  <span m="2836800">is</span> <span m="2836950">true</span> <span m="2837310">at an</span>
  <span m="2837610">optimum,</span> <span m="2838330">one</span> <span m="2838600">general</span>
  <span m="2839260">idea</span> <span m="2839680">in</span> <span m="2839800">optimization</span>
  <span m="2840400">is</span> <span m="2840830">this</span> <span m="2841120">so-called</span>
  <span m="2841420">fixed</span> <span m="2841690">point</span> <span m="2841900">iteration</span>
  <span m="2842630">that</span> <span m="2842830">you</span> <span m="2842920">can</span>
  <span m="2843070">do</span> <span m="2843220">to</span> <span m="2843340">arrive</span>
  <span m="2843610">there.</span> <span m="2846230">And</span> <span m="2846340">that's</span>
  <span m="2846460">essentially</span> <span m="2846880">what</span> <span m="2847000">we</span>
  <span m="2847130">will</span> <span m="2847240">do</span> <span m="2847420">to</span>
  <span m="2847540">get</span> <span m="2847750">to</span> <span m="2847870">a</span>
  <span m="2847930">good</span> <span m="2848140">Q.</span></p><p><span m="2849610">So</span>
  <span m="2850120">a</span> <span m="2850210">nice</span> <span m="2850480">thing</span>
  <span m="2850630">about</span> <span m="2851290">Q-learning</span> <span m="2851830">is</span>
  <span m="2851980">that</span> <span m="2852760">if</span> <span m="2853150">your</span>
  <span m="2853330">states</span> <span m="2853990">and</span> <span m="2854140">action</span>
  <span m="2854470">spaces</span> <span m="2854890">are</span> <span m="2854980">small</span>
  <span m="2855550">and</span> <span m="2855640">discrete,</span> <span m="2856750">you</span>
  <span m="2856870">can</span> <span m="2857020">represent</span> <span m="2857530">the</span>
  <span m="2857620">Q</span> <span m="2857830">function</span> <span m="2858160">as</span>
  <span m="2858250">a</span> <span m="2858310">table.</span> <span m="2859240">So</span>
  <span m="2859420">all</span> <span m="2859570">you</span> <span m="2859660">have</span>
  <span m="2859780">to</span> <span m="2859870">keep</span> <span m="2860050">track</span>
  <span m="2860320">of</span> <span m="2860470">is,</span> <span m="2860690">how</span>
  <span m="2860860">good</span> <span m="2861100">is</span> <span m="2861520">the</span>
  <span m="2863350">certain</span> <span m="2863620">action</span> <span m="2864010">in</span>
  <span m="2864130">a</span> <span m="2864190">certain</span> <span m="2864430">state?</span>
  <span m="2864970">Or</span> <span m="2865270">all</span> <span m="2865570">actions</span>
  <span m="2865900">in</span> <span m="2866260">all</span> <span m="2866440">states,</span>
  <span m="2866740">rather?</span> <span m="2867670">So</span> <span m="2867790">that's</span>
  <span m="2867940">what</span> <span m="2868030">we</span> <span m="2868120">did</span>
  <span m="2868240">here.</span> <span m="2868680">This</span> <span m="2868780">is</span>
  <span m="2868810">a</span> <span m="2868870">table.</span></p><p><span m="2871330">I've</span>
  <span m="2872200">described</span> <span m="2872650">to</span> <span m="2872710">you</span>
  <span m="2872830">the</span> <span m="2872920">policy</span> <span m="2873370">here,</span>
  <span m="2873880">but</span> <span m="2874030">what</span> <span m="2874190">we'll</span>
  <span m="2874390">do</span> <span m="2874570">next</span> <span m="2874990">is</span>
  <span m="2875200">to</span> <span m="2876400">describe</span> <span m="2876940">the</span>
  <span m="2877300">value</span> <span m="2877690">of</span> <span m="2877780">each</span>
  <span m="2878080">action.</span> <span m="2878560">So you</span> <span m="2878650">can</span>
  <span m="2878770">think</span> <span m="2878920">of</span> <span m="2879490">a</span>
  <span m="2879550">value</span> <span m="2879850">of</span> <span m="2879910">taking</span>
  <span m="2880240">the</span> <span m="2880660">right</span> <span m="2880990">one,</span>
  <span m="2881530">bottom,</span> <span m="2882370">top,</span> <span m="2882730">and</span>
  <span m="2883120">left,</span> <span m="2883390">essentially.</span> <span m="2884080">Those</span>
  <span m="2884290">will</span> <span m="2884380">be</span> <span m="2884500">the</span>
  <span m="2885100">values</span> <span m="2885400">that</span> <span m="2885520">we</span>
  <span m="2885580">need</span> <span m="2885700">to</span> <span m="2885760">consider.</span>
  <span m="2888600">And</span> <span m="2888680">so</span> <span m="2888830">what</span>
  <span m="2889010">Q-learning</span> <span m="2889370">can</span> <span m="2889490">do</span>
  <span m="2889640">with</span> <span m="2889790">discrete</span> <span m="2890120">states</span>
  <span m="2890660">is</span> <span m="2890930">to</span> <span m="2891980">essentially</span>
  <span m="2892400">start</span> <span m="2892760">from</span> <span m="2892940">somewhere,</span>
  <span m="2894110">start</span> <span m="2894380">from</span> <span m="2894530">some</span>
  <span m="2895070">idea</span> <span m="2895430">of</span> <span m="2895480">what</span>
  <span m="2895580">Q is--</span> <span m="2895760">could</span> <span m="2896010">be</span>
  <span m="2896120">random,</span> <span m="2896450">could</span> <span m="2896600">be</span>
  <span m="2896690">0.</span></p><p><span m="2897710">And</span> <span m="2897860">then</span>
  <span m="2898040">repeat</span> <span m="2898490">the</span> <span m="2898580">following</span>
  <span m="2899840">fixed-point</span> <span m="2900230">iteration,</span> <span m="2900890">where</span>
  <span m="2901730">you</span> <span m="2902000">update</span> <span m="2903050">your</span>
  <span m="2903500">former</span> <span m="2904520">idea</span> <span m="2904820">of</span>
  <span m="2904880">what</span> <span m="2905000">Q</span> <span m="2905240">should</span>
  <span m="2905390">be,</span> <span m="2906520">with</span> <span m="2906940">its</span>
  <span m="2907100">current</span> <span m="2907370">value</span> <span m="2907820">plus</span>
  <span m="2909860">essentially</span> <span m="2910220">a</span> <span m="2910310">mixture</span>
  <span m="2910760">of</span> <span m="2911300">the</span> <span m="2911510">immediate</span>
  <span m="2911840">reward</span> <span m="2912290">for</span> <span m="2912530">taking</span>
  <span m="2912830">action,</span> <span m="2913150">At,</span> <span m="2913520">in</span>
  <span m="2913640">that</span> <span m="2913790">state,</span> <span m="2914480">and</span>
  <span m="2914720">the</span> <span m="2915110">future</span> <span m="2915500">reward,</span>
  <span m="2915980">as</span> <span m="2916160">judged</span> <span m="2916460">by</span>
  <span m="2916580">your</span> <span m="2916700">current</span> <span m="2917120">estimate</span>
  <span m="2917870">of</span> <span m="2917960">the</span> <span m="2918050">Q</span>
  <span m="2918230">function.</span> <span m="2918810">So</span> <span m="2919020">we'll</span>
  <span m="2919460">do</span> <span m="2919670">that</span> <span m="2919820">now</span>
  <span m="2920000">in</span> <span m="2920090">practice.</span> <span m="2920390">Yeah.</span></p><p><span
  m="2921200">AUDIENCE:</span> <span m="2921380">Throughout</span> <span m="2921560">this,</span>
  <span m="2921920">where</span> <span m="2922210">are</span> <span m="2922290">we</span>
  <span m="2922490">getting</span> <span m="2923210">the</span> <span m="2923430">transition</span>
  <span m="2923850">probabilities</span> <span m="2924350">or</span> <span m="2924520">the</span>
  <span m="2924950">behavior</span> <span m="2925350">of the game?</span></p><p><span
  m="2926120">FREDRIK D. JOHANSSON:</span> <span m="2926195">So</span> <span m="2926270">they're</span>
  <span m="2926630">not</span> <span m="2926810">used</span> <span m="2926990">here,</span>
  <span m="2927140">actually.</span> <span m="2927510">A</span> <span m="2927590">value-based</span>
  <span m="2928610">RL--</span> <span m="2928850">I</span> <span m="2928910">didn't</span>
  <span m="2929090">say</span> <span m="2929240">that</span> <span m="2929420">explicitly,</span>
  <span m="2930030">but</span> <span m="2930080">they</span> <span m="2930200">don't</span>
  <span m="2930500">rely</span> <span m="2930800">on</span> <span m="2930920">knowing</span>
  <span m="2931190">the</span> <span m="2931280">transition</span> <span m="2931670">probabilities.</span>
  <span m="2933240">What</span> <span m="2933590">you</span> <span m="2933770">might</span>
  <span m="2934190">ask</span> <span m="2934520">is</span> <span m="2934730">where</span>
  <span m="2934910">do</span> <span m="2935000">we</span> <span m="2935120">get</span>
  <span m="2935360">the</span> <span m="2935510">S</span> <span m="2935780">and</span>
  <span m="2935900">the</span> <span m="2936020">As</span> <span m="2936290">and</span>
  <span m="2936380">the</span> <span m="2936470">Rs</span> <span m="2936740">from?</span>
  <span m="2938060">And</span> <span m="2938180">we'll</span> <span m="2938330">get</span>
  <span m="2938480">to</span> <span m="2938600">that.</span></p><p><span m="2939560">How</span>
  <span m="2939680">do</span> <span m="2939740">we</span> <span m="2939830">estimate</span>
  <span m="2940130">these?</span> <span m="2940780">We'll</span> <span m="2941060">get</span>
  <span m="2941180">to</span> <span m="2941270">that</span> <span m="2941420">later.</span>
  <span m="2943130">Good</span> <span m="2943250">question,</span> <span m="2943520">though.</span>
  <span m="2945720">I'm</span> <span m="2945800">going</span> <span m="2945950">to</span>
  <span m="2946280">throw</span> <span m="2946540">a</span> <span m="2946610">very</span>
  <span m="2946810">messy</span> <span m="2947140">slide</span> <span m="2947410">at</span>
  <span m="2947570">you.</span> <span m="2947770">Here you go.</span> <span m="2949780">A
  lot</span> <span m="2949930">of</span> <span m="2949990">numbers.</span></p><p><span
  m="2951620">So</span> <span m="2952210">what</span> <span m="2952400">I've</span>
  <span m="2952790">done</span> <span m="2953080">now</span> <span m="2953380">here</span>
  <span m="2953740">is</span> <span m="2953830">a</span> <span m="2953980">more</span>
  <span m="2954130">exhaustive</span> <span m="2954550">version</span> <span m="2954790">of</span>
  <span m="2954850">what</span> <span m="2954970">I</span> <span m="2955030">put</span>
  <span m="2955210">on</span> <span m="2955300">the</span> <span m="2955360">board.</span>
  <span m="2955720">For</span> <span m="2955900">each</span> <span m="2956710">little</span>
  <span m="2956980">triangle</span> <span m="2957460">here</span> <span m="2957700">represents</span>
  <span m="2958270">the</span> <span m="2958480">Q</span> <span m="2958780">value</span>
  <span m="2960070">for</span> <span m="2960280">the</span> <span m="2960400">state-action</span>
  <span m="2960970">pair.</span> <span m="2961300">So</span> <span m="2961600">this</span>
  <span m="2961930">triangle</span> <span m="2962320">is,</span> <span m="2962560">again,</span>
  <span m="2962830">for</span> <span m="2962950">the</span> <span m="2963070">action</span>
  <span m="2963350">right</span> <span m="2964090">if</span> <span m="2964210">you're</span>
  <span m="2964360">in</span> <span m="2964450">this</span> <span m="2964630">state.</span></p><p><span
  m="2967870">So</span> <span m="2968470">what</span> <span m="2968650">I've</span>
  <span m="2968800">put</span> <span m="2970060">on</span> <span m="2970300">the</span>
  <span m="2970420">first</span> <span m="2970720">slide</span> <span m="2970990">here</span>
  <span m="2971470">is</span> <span m="2972130">the</span> <span m="2972250">immediate</span>
  <span m="2972640">reward</span> <span m="2975280">of</span> <span m="2976030">each</span>
  <span m="2976270">action.</span> <span m="2978770">So</span> <span m="2978920">we</span>
  <span m="2979010">know</span> <span m="2979160">that</span> <span m="2979340">any</span>
  <span m="2979580">step</span> <span m="2979910">will</span> <span m="2980720">cost</span>
  <span m="2981140">us</span> <span m="2981500">minus</span> <span m="2982010">0.04.</span>
  <span m="2982970">So</span> <span m="2983120">that's</span> <span m="2983300">why</span>
  <span m="2983450">there's</span> <span m="2983630">a</span> <span m="2983660">lot</span>
  <span m="2983810">of</span> <span m="2983930">those</span> <span m="2984200">here.</span>
  <span m="2984710">These</span> <span m="2985190">white</span> <span m="2985460">boxes</span>
  <span m="2985820">here</span> <span m="2986000">are</span> <span m="2986630">not</span>
  <span m="2986810">possible</span> <span m="2987200">actions.</span> <span m="2989250">Up</span>
  <span m="2989400">here,</span> <span m="2989670">you</span> <span m="2989790">have
  a</span> <span m="2989940">0.96,</span> <span m="2990870">because</span> <span m="2991170">it's</span>
  <span m="2991350">1,</span> <span m="2992010">which</span> <span m="2992190">is</span>
  <span m="2992280">the</span> <span m="2992370">immediate</span> <span m="2992640">reward</span>
  <span m="2992930">of</span> <span m="2993090">going</span> <span m="2993390">right</span>
  <span m="2993600">here,</span> <span m="2994170">minus</span> <span m="2994560">0.04.</span></p><p><span
  m="2996330">These</span> <span m="2996570">two</span> <span m="2997350">are</span>
  <span m="2997830">minus</span> <span m="2998190">1.04</span> <span m="2999690">for</span>
  <span m="2999870">the</span> <span m="2999960">same</span> <span m="3000140">reason--</span>
  <span m="3001220">because</span> <span m="3001730">you</span> <span m="3001820">arrive</span>
  <span m="3002090">in</span> <span m="3002180">minus</span> <span m="3002420">1.</span>
  <span m="3003910">OK,</span> <span m="3004220">so</span> <span m="3004340">that's</span>
  <span m="3004490">the</span> <span m="3004580">first</span> <span m="3005840">step</span>
  <span m="3006450">and</span> <span m="3006470">the</span> <span m="3006560">second</span>
  <span m="3006890">step</span> <span m="3007100">done.</span> <span m="3007370">We</span>
  <span m="3007550">initialize</span> <span m="3008040">Qs</span> <span m="3008360">to</span>
  <span m="3008450">be</span> <span m="3008570">0.</span> <span m="3009470">And</span>
  <span m="3009590">then</span> <span m="3009710">we</span> <span m="3009830">picked</span>
  <span m="3010160">these</span> <span m="3011030">two</span> <span m="3011240">parameters</span>
  <span m="3011900">of</span> <span m="3012020">the</span> <span m="3012110">problem,</span>
  <span m="3012770">alpha</span> <span m="3013070">and</span> <span m="3013190">gamma,</span>
  <span m="3013460">to</span> <span m="3013550">be</span> <span m="3013640">1.</span>
  <span m="3014430">And</span> <span m="3014450">then</span> <span m="3014600">we</span>
  <span m="3014720">did</span> <span m="3014870">the</span> <span m="3014960">first</span>
  <span m="3016340">iteration</span> <span m="3017000">of</span> <span m="3017290">Q-learning,</span>
  <span m="3018170">where</span> <span m="3018530">we</span> <span m="3018890">set</span>
  <span m="3019100">the</span> <span m="3019190">Q</span> <span m="3019430">to</span>
  <span m="3019520">be</span> <span m="3020690">the</span> <span m="3020840">old</span>
  <span m="3021050">version</span> <span m="3021290">of</span> <span m="3021350">Q,</span>
  <span m="3021560">which</span> <span m="3021740">was</span> <span m="3021830">0,</span>
  <span m="3022520">plus</span> <span m="3022910">alpha</span> <span m="3023420">times</span>
  <span m="3023750">this</span> <span m="3024890">thing</span> <span m="3025130">here.</span></p><p><span
  m="3025850">So</span> <span m="3025940">Q</span> <span m="3026150">was</span> <span
  m="3026280">0,</span> <span m="3026600">that</span> <span m="3026720">means</span>
  <span m="3026900">that</span> <span m="3027050">this</span> <span m="3027320">is</span>
  <span m="3027470">also</span> <span m="3027740">0.</span> <span m="3028340">So</span>
  <span m="3028460">the</span> <span m="3028550">only</span> <span m="3028820">thing</span>
  <span m="3029000">we</span> <span m="3029090">need</span> <span m="3029210">to</span>
  <span m="3029270">look</span> <span m="3029450">at</span> <span m="3029850">is</span>
  <span m="3030110">this</span> <span m="3030530">thing</span> <span m="3030710">here.</span>
  <span m="3031820">This</span> <span m="3032870">also</span> <span m="3033200">is</span>
  <span m="3033290">0,</span> <span m="3033620">because</span> <span m="3034250">the</span>
  <span m="3034370">Qs</span> <span m="3034640">for</span> <span m="3034790">all</span>
  <span m="3035060">states</span> <span m="3035300">were</span> <span m="3035420">0,</span>
  <span m="3035720">so</span> <span m="3035840">the</span> <span m="3035930">only</span>
  <span m="3036110">thing</span> <span m="3036260">we</span> <span m="3036320">end</span>
  <span m="3036410">up</span> <span m="3036530">with</span> <span m="3036610">is</span>
  <span m="3036830">R.</span> <span m="3037890">And</span> <span m="3038090">that's</span>
  <span m="3038330">what</span> <span m="3038480">populated</span> <span m="3038930">this</span>
  <span m="3039080">table</span> <span m="3039350">here.</span></p><p><span m="3044000">Next</span>
  <span m="3044270">timestep--</span> <span m="3046940">I'm</span> <span m="3047240">doing</span>
  <span m="3047430">Q-learning</span> <span m="3047720">now</span> <span m="3047900">in</span>
  <span m="3047960">a</span> <span m="3048020">way</span> <span m="3048170">where</span>
  <span m="3048290">I</span> <span m="3048380">update</span> <span m="3049730">all</span>
  <span m="3049850">the</span> <span m="3049940">state-action</span> <span m="3050480">pairs</span>
  <span m="3050660">at</span> <span m="3050720">once.</span> <span m="3051380">How</span>
  <span m="3051530">can</span> <span m="3051680">I</span> <span m="3051740">do</span>
  <span m="3051920">that?</span> <span m="3052470">Well,</span> <span m="3052520">it</span>
  <span m="3052580">depends</span> <span m="3052850">on</span> <span m="3052910">the</span>
  <span m="3053000">question</span> <span m="3053330">I</span> <span m="3053390">got</span>
  <span m="3053600">there,</span> <span m="3053780">essentially.</span> <span m="3054200">What</span>
  <span m="3054440">data</span> <span m="3054740">do</span> <span m="3054920">I</span>
  <span m="3055070">observe?</span> <span m="3055550">Or</span> <span m="3055670">how</span>
  <span m="3055850">do</span> <span m="3055970">I</span> <span m="3056180">get</span>
  <span m="3056390">to</span> <span m="3056480">know</span> <span m="3056810">the</span>
  <span m="3058220">rewards</span> <span m="3058730">of</span> <span m="3058790">the</span>
  <span m="3058910">S&amp;A</span> <span m="3059210">pairs?</span> <span m="3059800">We'll</span>
  <span m="3060050">come</span> <span m="3060170">back</span> <span m="3060320">to</span>
  <span m="3060410">that.</span></p><p><span m="3062530">So</span> <span m="3062610">in</span>
  <span m="3062670">the</span> <span m="3062760">next</span> <span m="3062970">step,</span>
  <span m="3066210">I</span> <span m="3066540">have</span> <span m="3066750">to</span>
  <span m="3066930">update</span> <span m="3067980">everything</span> <span m="3068400">again.</span>
  <span m="3069360">So</span> <span m="3069750">it's</span> <span m="3069910">the</span>
  <span m="3069990">previous</span> <span m="3070410">Q</span> <span m="3070570">value,</span>
  <span m="3071050">which</span> <span m="3071130">was</span> <span m="3071400">minus</span>
  <span m="3071790">0.04</span> <span m="3072390">for</span> <span m="3072510">a</span>
  <span m="3072540">lot</span> <span m="3072690">of</span> <span m="3072750">things,</span>
  <span m="3073440">then</span> <span m="3073620">plus</span> <span m="3074760">the</span>
  <span m="3074880">immediate</span> <span m="3075600">reward,</span> <span m="3076440">which</span>
  <span m="3076590">was</span> <span m="3076770">this</span> <span m="3076950">RT.</span>
  <span m="3077460">And</span> <span m="3077580">I</span> <span m="3077740">have</span>
  <span m="3077820">to</span> <span m="3077910">keep</span> <span m="3078090">going.</span>
  <span m="3079260">So</span> <span m="3080550">the</span> <span m="3081210">dominant</span>
  <span m="3081660">thing</span> <span m="3081990">for</span> <span m="3082230">the</span>
  <span m="3082320">table</span> <span m="3082680">this</span> <span m="3082890">time</span>
  <span m="3083100">was</span> <span m="3083280">that</span> <span m="3083400">the</span>
  <span m="3083520">best</span> <span m="3083970">Q</span> <span m="3084210">value</span>
  <span m="3084540">for</span> <span m="3086070">almost</span> <span m="3086490">all</span>
  <span m="3086670">of</span> <span m="3086730">these</span> <span m="3086880">boxes</span>
  <span m="3087240">was</span> <span m="3087390">minus</span> <span m="3087780">0.04.</span></p><p><span
  m="3089580">So</span> <span m="3090210">essentially</span> <span m="3090630">I</span>
  <span m="3090720">will</span> <span m="3090900">add</span> <span m="3091110">the</span>
  <span m="3091170">immediate</span> <span m="3091440">reward</span> <span m="3091770">plus</span>
  <span m="3092070">that</span> <span m="3092340">almost</span> <span m="3092610">everywhere.</span>
  <span m="3093940">What</span> <span m="3094090">is</span> <span m="3094210">interesting,</span>
  <span m="3094700">though,</span> <span m="3095090">is</span> <span m="3095170">that</span>
  <span m="3095350">here,</span> <span m="3095770">the</span> <span m="3095890">best</span>
  <span m="3096820">Q</span> <span m="3097000">value</span> <span m="3097240">was</span>
  <span m="3097390">0.96.</span> <span m="3098590">And</span> <span m="3098710">it</span>
  <span m="3098800">will</span> <span m="3098950">remain</span> <span m="3100310">so.</span>
  <span m="3101050">That</span> <span m="3101200">means</span> <span m="3101440">that</span>
  <span m="3101560">the</span> <span m="3101650">best</span> <span m="3101860">Q</span>
  <span m="3102070">value</span> <span m="3102340">for</span> <span m="3102520">the</span>
  <span m="3102820">adjacent</span> <span m="3103300">states--</span> <span m="3104020">we</span>
  <span m="3104170">look</span> <span m="3104440">at</span> <span m="3104530">this</span>
  <span m="3104800">max</span> <span m="3105220">here</span> <span m="3106270">and</span>
  <span m="3106360">get</span> <span m="3106540">0.96</span> <span m="3107200">out.</span>
  <span m="3109840">And</span> <span m="3109960">then</span> <span m="3110110">add</span>
  <span m="3110350">the</span> <span m="3110470">immediate</span> <span m="3110800">reward.</span></p><p><span
  m="3112840">Getting</span> <span m="3113230">to</span> <span m="3113350">here</span>
  <span m="3113950">gives</span> <span m="3114120">me</span> <span m="3114220">0.96</span>
  <span m="3115210">minus</span> <span m="3115600">0.04</span> <span m="3116230">for</span>
  <span m="3116380">the</span> <span m="3116470">immediate</span> <span m="3116770">reward.</span>
  <span m="3118920">And</span> <span m="3119030">now</span> <span m="3119110">we</span>
  <span m="3119170">can</span> <span m="3119650">figure</span> <span m="3119920">out</span>
  <span m="3120010">what</span> <span m="3120130">will</span> <span m="3120280">happen</span>
  <span m="3120580">next.</span> <span m="3122890">These</span> <span m="3123100">values</span>
  <span m="3123580">will</span> <span m="3124000">spread</span> <span m="3124420">out</span>
  <span m="3125200">as</span> <span m="3125350">you</span> <span m="3125440">go</span>
  <span m="3129190">further</span> <span m="3129490">away</span> <span m="3129730">from</span>
  <span m="3129910">the</span> <span m="3130000">plus</span> <span m="3130400">1.</span>
  <span m="3130690">I</span> <span m="3130720">don't</span> <span m="3130840">think</span>
  <span m="3130990">we</span> <span m="3131080">should</span> <span m="3131200">go</span>
  <span m="3131350">through</span> <span m="3131680">all</span> <span m="3131830">of</span>
  <span m="3131920">this,</span> <span m="3132560">but</span> <span m="3132670">you</span>
  <span m="3132760">get</span> <span m="3132880">a</span> <span m="3132940">sense,</span>
  <span m="3133760">essentially,</span> <span m="3134260">how</span> <span m="3135130">information</span>
  <span m="3135790">is</span> <span m="3135910">moved</span> <span m="3136300">from</span>
  <span m="3136630">the</span> <span m="3136720">plus</span> <span m="3137065">1</span>
  <span m="3137410">and</span> <span m="3137840">away.</span> <span m="3139000">And</span>
  <span m="3139090">I'm</span> <span m="3139210">sure</span> <span m="3139390">that's</span>
  <span m="3140230">how</span> <span m="3140410">you</span> <span m="3140530">solved</span>
  <span m="3140830">it</span> <span m="3140920">yourself,</span> <span m="3142960">in</span>
  <span m="3143080">your</span> <span m="3143200">head.</span> <span m="3144220">But</span>
  <span m="3144610">this</span> <span m="3144850">makes</span> <span m="3145090">it</span>
  <span m="3145150">clear</span> <span m="3145390">why</span> <span m="3145510">you</span>
  <span m="3145600">can</span> <span m="3145750">do</span> <span m="3145900">that,</span>
  <span m="3146110">even</span> <span m="3146440">if</span> <span m="3146530">you</span>
  <span m="3146620">don't</span> <span m="3147130">know</span> <span m="3147460">where</span>
  <span m="3147880">the</span> <span m="3148000">terminal</span> <span m="3148300">states</span>
  <span m="3148570">are</span> <span m="3148720">or</span> <span m="3150820">where</span>
  <span m="3151250">the</span> <span m="3151330">value</span> <span m="3151660">of</span>
  <span m="3151750">the</span> <span m="3151880">state-action</span> <span m="3152340">pairs</span>
  <span m="3152560">are.</span></p><p><span m="3155320">AUDIENCE:</span> <span m="3155375">Doesn't</span>
  <span m="3155430">this</span> <span m="3156480">calculation</span> <span m="3157070">assume</span>
  <span m="3158090">that</span> <span m="3158270">if</span> <span m="3158450">you</span>
  <span m="3158640">want to</span> <span m="3158840">move</span> <span m="3159140">in</span>
  <span m="3159260">a</span> <span m="3159320">certain</span> <span m="3159710">direction,</span>
  <span m="3160250">you</span> <span m="3160655">will move</span> <span m="3161060">in
  that</span> <span m="3161465">direction?</span></p><p><span m="3161870">FREDRIK
  D. JOHANSSON:</span> <span m="3162005">Yes.</span> <span m="3163160">Sorry.</span>
  <span m="3163490">Thanks</span> <span m="3163700">for</span> <span m="3163760">reminding</span>
  <span m="3164120">me.</span> <span m="3164710">That</span> <span m="3164900">should
  have</span> <span m="3165060">been in the</span> <span m="3165360">slide,</span>
  <span m="3165700">yes.</span> <span m="3166520">Thank</span> <span m="3166670">you.</span></p><p><span
  m="3170240">I'm</span> <span m="3170340">going</span> <span m="3170430">to</span>
  <span m="3170510">skip</span> <span m="3170720">the</span> <span m="3170810">rest</span>
  <span m="3171020">of</span> <span m="3171110">this.</span> <span m="3171350">I</span>
  <span m="3171410">hope</span> <span m="3171560">you</span> <span m="3171620">forgive</span>
  <span m="3171890">me.</span> <span m="3172030">We</span> <span m="3172100">can</span>
  <span m="3172220">talk</span> <span m="3172550">more</span> <span m="3172730">about</span>
  <span m="3172940">it</span> <span m="3173090">later.</span></p><p><span m="3178700">Thanks</span>
  <span m="3178880">for</span> <span m="3178970">reminding</span> <span m="3179240">me,</span>
  <span m="3179330">Pete,</span> <span m="3179480">there,</span> <span m="3179680">that</span>
  <span m="3180260">one</span> <span m="3180410">of</span> <span m="3180470">the</span>
  <span m="3180530">things</span> <span m="3180740">I</span> <span m="3180830">exploited</span>
  <span m="3181250">here</span> <span m="3181430">was</span> <span m="3181760">that</span>
  <span m="3182600">I</span> <span m="3182990">assume</span> <span m="3183230">just</span>
  <span m="3183450">deterministic</span> <span m="3183920">transitions.</span> <span
  m="3185000">Another</span> <span m="3185420">thing</span> <span m="3185630">that</span>
  <span m="3185750">I</span> <span m="3185840">relied</span> <span m="3186170">very</span>
  <span m="3186470">heavily</span> <span m="3186800">on</span> <span m="3186950">here</span>
  <span m="3187160">is</span> <span m="3187370">that</span> <span m="3187610">I</span>
  <span m="3187700">can</span> <span m="3187880">represent</span> <span m="3188300">this</span>
  <span m="3188420">Q</span> <span m="3188600">function</span> <span m="3188930">as</span>
  <span m="3189050">a</span> <span m="3189110">table.</span> <span m="3190190">I</span>
  <span m="3190430">drew</span> <span m="3190670">all</span> <span m="3190790">these</span>
  <span m="3190940">boxes</span> <span m="3191330">and</span> <span m="3191420">I</span>
  <span m="3191480">filled</span> <span m="3191660">the</span> <span m="3191720">numbers</span>
  <span m="3192080">in.</span> <span m="3192290">That's</span> <span m="3192590">easy</span>
  <span m="3192830">enough.</span></p><p><span m="3193440">But</span> <span m="3193460">what</span>
  <span m="3193700">if</span> <span m="3193850">I</span> <span m="3193970">have</span>
  <span m="3194390">thousands</span> <span m="3194900">of</span> <span m="3194960">states</span>
  <span m="3195320">and</span> <span m="3195410">thousands</span> <span m="3195830">of</span>
  <span m="3195950">actions?</span> <span m="3197510">That's</span> <span m="3197690">a</span>
  <span m="3197720">large</span> <span m="3197990">table.</span> <span m="3199000">And</span>
  <span m="3199130">not</span> <span m="3199280">only</span> <span m="3199550">is</span>
  <span m="3199660">it</span> <span m="3199760">a</span> <span m="3199790">large</span>
  <span m="3200060">table</span> <span m="3200420">for</span> <span m="3200540">me</span>
  <span m="3200630">to</span> <span m="3200720">keep</span> <span m="3200870">in</span>
  <span m="3200990">memory--</span> <span m="3201450">it's</span> <span m="3201560">also</span>
  <span m="3202040">very</span> <span m="3202340">bad</span> <span m="3202670">for</span>
  <span m="3202790">me</span> <span m="3202880">statistically.</span> <span m="3204080">If</span>
  <span m="3204290">I</span> <span m="3204440">want</span> <span m="3204710">to</span>
  <span m="3204890">observe</span> <span m="3205490">anything</span> <span m="3205910">about</span>
  <span m="3206150">a</span> <span m="3206180">state-action</span> <span m="3206690">pair,</span>
  <span m="3206900">I</span> <span m="3207020">have</span> <span m="3207260">to</span>
  <span m="3207500">do</span> <span m="3207770">that</span> <span m="3207890">action</span>
  <span m="3208190">in</span> <span m="3208310">that</span> <span m="3208460">state.</span></p><p><span
  m="3208790">And</span> <span m="3208880">if</span> <span m="3208940">you</span>
  <span m="3209030">think</span> <span m="3209210">about</span> <span m="3210170">treating</span>
  <span m="3210500">patients</span> <span m="3210830">in</span> <span m="3210920">a</span>
  <span m="3210980">hospital,</span> <span m="3211340">you're</span> <span m="3211460">not</span>
  <span m="3211610">going</span> <span m="3211730">to</span> <span m="3211790">try</span>
  <span m="3212060">everything</span> <span m="3212570">in</span> <span m="3212690">every</span>
  <span m="3212870">state,</span> <span m="3213440">usually.</span> <span m="3214100">You're</span>
  <span m="3214190">also</span> <span m="3214400">not</span> <span m="3214490">going</span>
  <span m="3214610">to</span> <span m="3214670">have</span> <span m="3214820">infinite</span>
  <span m="3215630">numbers</span> <span m="3215990">of</span> <span m="3216050">patients.</span>
  <span m="3217490">So</span> <span m="3217850">how</span> <span m="3218030">do</span>
  <span m="3218090">you</span> <span m="3218600">figure</span> <span m="3218900">out</span>
  <span m="3219020">what</span> <span m="3219200">is</span> <span m="3219320">the</span>
  <span m="3219410">immediate</span> <span m="3219770">reward</span> <span m="3220220">of</span>
  <span m="3220280">taking</span> <span m="3220520">a</span> <span m="3220580">certain</span>
  <span m="3221270">action</span> <span m="3221630">in</span> <span m="3221690">a</span>
  <span m="3221720">certain</span> <span m="3221960">state?</span> <span m="3224160">And</span>
  <span m="3224260">this</span> <span m="3224320">is</span> <span m="3224410">where</span>
  <span m="3224620">a</span> <span m="3224650">function</span> <span m="3224990">approximation</span>
  <span m="3225550">comes</span> <span m="3225790">in.</span></p><p><span m="3227720">Essentially,</span>
  <span m="3229960">if</span> <span m="3230110">you</span> <span m="3230260">can't</span>
  <span m="3230650">represent</span> <span m="3231100">your</span> <span m="3231190">data</span>
  <span m="3231390">set</span> <span m="3231580">table,</span> <span m="3231940">either</span>
  <span m="3232180">for</span> <span m="3232330">statistical</span> <span m="3232870">reasons</span>
  <span m="3233440">or</span> <span m="3234160">for</span> <span m="3236680">memory</span>
  <span m="3237160">reasons,</span> <span m="3237610">let's</span> <span m="3237790">say,</span>
  <span m="3239920">you</span> <span m="3240040">might</span> <span m="3240250">want</span>
  <span m="3240460">to</span> <span m="3240580">approximate</span> <span m="3241150">the</span>
  <span m="3241240">Q</span> <span m="3241420">function</span> <span m="3241820">with</span>
  <span m="3242660">a</span> <span m="3242810">parametric</span> <span m="3243460">or</span>
  <span m="3243580">with</span> <span m="3243730">a</span> <span m="3243790">non-parametric</span>
  <span m="3244160">function.</span> <span m="3246150">And</span> <span m="3246330">this</span>
  <span m="3246510">is</span> <span m="3246630">exactly</span> <span m="3246960">what</span>
  <span m="3247080">we</span> <span m="3247140">can</span> <span m="3247260">do.</span>
  <span m="3247680">So</span> <span m="3247860">we</span> <span m="3247950">can</span>
  <span m="3248130">draw</span> <span m="3248430">now</span> <span m="3248760">an</span>
  <span m="3249120">analogy</span> <span m="3249480">to</span> <span m="3250350">what</span>
  <span m="3250500">we</span> <span m="3250590">did</span> <span m="3250710">last</span>
  <span m="3250980">week.</span> <span m="3251260">I'm</span> <span m="3251340">going
  to come</span> <span m="3251490">back</span> <span m="3251700">to</span> <span m="3251790">this,</span>
  <span m="3252090">but</span> <span m="3252810">essentially</span> <span m="3254490">instead</span>
  <span m="3256070">of</span> <span m="3257910">doing</span> <span m="3258240">this</span>
  <span m="3258390">fixed-point</span> <span m="3258870">iteration</span> <span m="3259320">that</span>
  <span m="3259440">we</span> <span m="3259500">did</span> <span m="3259650">before,</span>
  <span m="3260310">we</span> <span m="3260400">will</span> <span m="3260550">try</span>
  <span m="3260820">and</span> <span m="3260910">look</span> <span m="3261180">for</span>
  <span m="3261360">a</span> <span m="3261420">function</span> <span m="3261780">Q</span>
  <span m="3261990">theta</span> <span m="3262920">that</span> <span m="3263070">is</span>
  <span m="3263220">equal</span> <span m="3264030">to</span> <span m="3264660">R</span>
  <span m="3264900">plus</span> <span m="3265260">gamma</span> <span m="3266610">max</span>
  <span m="3266910">Q.</span></p><p><span m="3269190">Remember</span> <span m="3269520">before,</span>
  <span m="3269850">we</span> <span m="3270000">had</span> <span m="3270150">the</span>
  <span m="3270240">Bellman</span> <span m="3270540">inequality?</span> <span m="3271080">We</span>
  <span m="3271200">said</span> <span m="3271440">that</span> <span m="3272550">q-star</span>
  <span m="3274380">S,</span> <span m="3274665">A</span> <span m="3275550">is</span>
  <span m="3275700">equal</span> <span m="3276060">to</span> <span m="3277110">R</span>
  <span m="3278310">S,</span> <span m="3278800">A,</span> <span m="3278880">let's</span>
  <span m="3279180">say,</span> <span m="3279870">plus</span> <span m="3280290">gamma</span>
  <span m="3284750">max</span> <span m="3285020">A</span> <span m="3285110">prime</span>
  <span m="3295370">q</span> <span m="3295520">star</span> <span m="3296450">S</span>
  <span m="3296600">prime</span> <span m="3297080">A</span> <span m="3297430">prime,</span>
  <span m="3298880">where</span> <span m="3299130">S</span> <span m="3299340">prime</span>
  <span m="3299610">is</span> <span m="3299730">the</span> <span m="3299760">state</span>
  <span m="3300000">we</span> <span m="3300120">get</span> <span m="3300300">to</span>
  <span m="3300480">after</span> <span m="3300720">taking</span> <span m="3300990">action</span>
  <span m="3301380">A</span> <span m="3301690">in state</span> <span m="3302420">S.</span>
  <span m="3302940">So</span> <span m="3303090">the</span> <span m="3303210">only</span>
  <span m="3303420">thing</span> <span m="3303630">I've</span> <span m="3303750">done</span>
  <span m="3303990">here</span> <span m="3304230">is</span> <span m="3304380">to</span>
  <span m="3304470">take</span> <span m="3305760">this</span> <span m="3305940">equality</span>
  <span m="3306810">and</span> <span m="3306930">make</span> <span m="3307170">it</span>
  <span m="3307260">instead</span> <span m="3308460">a</span> <span m="3308520">loss</span>
  <span m="3308850">function</span> <span m="3309300">on</span> <span m="3309450">the</span>
  <span m="3309540">violation</span> <span m="3310050">of</span> <span m="3310110">this</span>
  <span m="3310260">equality.</span> <span m="3313140">So</span> <span m="3313400">by</span>
  <span m="3313610">minimizing</span> <span m="3314150">this</span> <span m="3314270">quantity,</span>
  <span m="3314720">I</span> <span m="3315080">will</span> <span m="3315290">find</span>
  <span m="3315590">something</span> <span m="3315860">that</span> <span m="3315950">has</span>
  <span m="3316520">approximately</span> <span m="3317270">the</span> <span m="3317390">Bellman</span>
  <span m="3318110">equality</span> <span m="3318560">that</span> <span m="3318650">we</span>
  <span m="3318770">talked</span> <span m="3318980">about</span> <span m="3319100">before.</span></p><p><span
  m="3320880">This</span> <span m="3321060">is</span> <span m="3321150">the</span>
  <span m="3321240">idea</span> <span m="3321430">of</span> <span m="3321580">fitted</span>
  <span m="3321840">Q-learning,</span> <span m="3322830">where</span> <span m="3323490">you</span>
  <span m="3323730">substitute</span> <span m="3324350">the</span> <span m="3326100">tabular</span>
  <span m="3326550">representation</span> <span m="3328270">with</span> <span m="3328480">the</span>
  <span m="3328830">function</span> <span m="3329140">approximations,</span> <span
  m="3329420">essentially.</span> <span m="3330910">So</span> <span m="3330960">just</span>
  <span m="3331140">to</span> <span m="3331200">make</span> <span m="3331350">this</span>
  <span m="3331470">a</span> <span m="3331530">bit</span> <span m="3331680">more</span>
  <span m="3331830">concrete,</span> <span m="3332250">we</span> <span m="3332370">can</span>
  <span m="3332490">think</span> <span m="3332640">about</span> <span m="3332820">the</span>
  <span m="3332880">case</span> <span m="3333210">where</span> <span m="3333360">we</span>
  <span m="3333510">have</span> <span m="3334110">only</span> <span m="3334350">a</span>
  <span m="3334410">single</span> <span m="3334740">step.</span> <span m="3335920">There's</span>
  <span m="3336120">only</span> <span m="3336720">a</span> <span m="3336810">single</span>
  <span m="3337200">action</span> <span m="3337530">to</span> <span m="3337650">make,</span>
  <span m="3338760">which</span> <span m="3338970">means</span> <span m="3339240">that</span>
  <span m="3339360">there</span> <span m="3339480">is</span> <span m="3339630">no</span>
  <span m="3340320">future</span> <span m="3340770">part</span> <span m="3341100">of</span>
  <span m="3341250">this</span> <span m="3341430">equation</span> <span m="3341790">here.</span>
  <span m="3342220">This</span> <span m="3342300">part</span> <span m="3342540">goes</span>
  <span m="3342750">away,</span> <span m="3342990">because</span> <span m="3343230">there's</span>
  <span m="3343410">only</span> <span m="3344700">one</span> <span m="3344970">stage</span>
  <span m="3345300">in</span> <span m="3345390">our</span> <span m="3345870">trajectory.</span>
  <span m="3346920">So</span> <span m="3347070">we</span> <span m="3347190">have</span>
  <span m="3347340">only</span> <span m="3347580">the</span> <span m="3347670">immediate</span>
  <span m="3348030">reward.</span> <span m="3348510">We</span> <span m="3348630">have</span>
  <span m="3348750">only</span> <span m="3348960">the</span> <span m="3349050">Q</span>
  <span m="3349200">function.</span></p><p><span m="3351080">Now,</span> <span m="3351170">this</span>
  <span m="3351350">is</span> <span m="3352250">exactly</span> <span m="3352820">a</span>
  <span m="3353090">regression</span> <span m="3355610">equation</span> <span m="3356350">in</span>
  <span m="3356480">the</span> <span m="3356570">way</span> <span m="3356720">that</span>
  <span m="3356840">you've</span> <span m="3356990">seen</span> <span m="3357170">it</span>
  <span m="3357260">when</span> <span m="3357410">estimating</span> <span m="3357800">potential</span>
  <span m="3358160">outcomes.</span> <span m="3359860">RT</span> <span m="3360290">here</span>
  <span m="3361250">represents</span> <span m="3361850">the</span> <span m="3365320">outcome</span>
  <span m="3365920">of</span> <span m="3366100">doing</span> <span m="3367060">action</span>
  <span m="3367390">A</span> <span m="3367660">and state</span> <span m="3367915">S.</span>
  <span m="3368850">And</span> <span m="3368950">Q</span> <span m="3369670">here</span>
  <span m="3369910">will</span> <span m="3370060">be</span> <span m="3370630">our</span>
  <span m="3370750">estimate</span> <span m="3371170">of</span> <span m="3371260">this</span>
  <span m="3371440">RT.</span></p><p><span m="3375620">Again,</span> <span m="3376090">I've</span>
  <span m="3376250">said</span> <span m="3376400">this</span> <span m="3376520">before--</span>
  <span m="3376860">if</span> <span m="3376910">we</span> <span m="3377000">have</span>
  <span m="3377120">a</span> <span m="3377180">single</span> <span m="3377930">time</span>
  <span m="3378230">point</span> <span m="3379040">in</span> <span m="3379220">our</span>
  <span m="3380690">process,</span> <span m="3381850">the</span> <span m="3382070">problem</span>
  <span m="3382400">reduces</span> <span m="3382820">to</span> <span m="3382940">estimating</span>
  <span m="3383270">potential</span> <span m="3383630">outcomes,</span> <span m="3384490">just</span>
  <span m="3384650">the</span> <span m="3384740">way</span> <span m="3384920">we</span>
  <span m="3385040">saw</span> <span m="3385250">it</span> <span m="3385340">last</span>
  <span m="3385640">time.</span> <span m="3386270">We</span> <span m="3386390">have</span>
  <span m="3387800">curves</span> <span m="3388100">that</span> <span m="3388190">correspond</span>
  <span m="3390080">outcomes</span> <span m="3390410">under</span> <span m="3390560">different</span>
  <span m="3390860">actions.</span> <span m="3391730">And</span> <span m="3391850">we</span>
  <span m="3391970">can</span> <span m="3392600">do</span> <span m="3392780">regression</span>
  <span m="3393260">adjustment,</span> <span m="3393710">trying</span> <span m="3393920">to</span>
  <span m="3393980">find</span> <span m="3394280">an</span> <span m="3394400">F</span>
  <span m="3394670">such</span> <span m="3394940">that</span> <span m="3395090">this</span>
  <span m="3395360">quantity</span> <span m="3395750">is</span> <span m="3395810">small</span>
  <span m="3397010">so</span> <span m="3397160">that</span> <span m="3397280">we</span>
  <span m="3397370">can</span> <span m="3397490">model</span> <span m="3398180">each</span>
  <span m="3398540">different</span> <span m="3398810">potential</span> <span m="3399140">outcomes.</span>
  <span m="3399740">And</span> <span m="3399830">that's</span> <span m="3399980">exactly</span>
  <span m="3400400">what</span> <span m="3400490">happens</span> <span m="3400880">with</span>
  <span m="3401060">the</span> <span m="3401620">fitted</span> <span m="3401880">Q</span>
  <span m="3402410">iteration</span> <span m="3402830">if</span> <span m="3402950">you</span>
  <span m="3403040">have</span> <span m="3403160">a</span> <span m="3403190">single</span>
  <span m="3403460">timestep,</span> <span m="3403880">too.</span></p><p><span m="3407670">So</span>
  <span m="3409620">to</span> <span m="3409770">make</span> <span m="3409980">it</span>
  <span m="3410070">even</span> <span m="3410340">more</span> <span m="3410550">concrete,</span>
  <span m="3411060">we</span> <span m="3411210">can</span> <span m="3411330">say</span>
  <span m="3411600">that</span> <span m="3412710">there's</span> <span m="3412950">some</span>
  <span m="3414180">target</span> <span m="3414690">value,</span> <span m="3415110">G
  hat,</span> <span m="3415680">which</span> <span m="3415860">represents</span> <span
  m="3416790">the</span> <span m="3416880">immediate</span> <span m="3417180">reward</span>
  <span m="3417570">and</span> <span m="3417660">the</span> <span m="3417750">future</span>
  <span m="3418980">rewards</span> <span m="3420120">that</span> <span m="3420480">is</span>
  <span m="3420690">the</span> <span m="3420810">target</span> <span m="3421170">of</span>
  <span m="3421260">our</span> <span m="3421350">regression.</span> <span m="3421980">And</span>
  <span m="3422100">we're</span> <span m="3422310">fitting</span> <span m="3422640">some</span>
  <span m="3422850">function</span> <span m="3423180">to</span> <span m="3423300">that</span>
  <span m="3423420">value.</span></p><p><span m="3430010">So</span> <span m="3430120">the</span>
  <span m="3430210">question</span> <span m="3430450">we</span> <span m="3430540">got</span>
  <span m="3430690">before</span> <span m="3431020">was</span> <span m="3435010">how</span>
  <span m="3435130">do</span> <span m="3435220">I</span> <span m="3435370">know</span>
  <span m="3435730">the</span> <span m="3435820">transition</span> <span m="3436240">matrix?</span>
  <span m="3436970">How</span> <span m="3437170">do</span> <span m="3437290">I</span>
  <span m="3437410">get</span> <span m="3438250">any</span> <span m="3438430">information</span>
  <span m="3438880">about</span> <span m="3439060">this</span> <span m="3439240">thing?</span>
  <span m="3440590">I</span> <span m="3440860">say</span> <span m="3441070">here</span>
  <span m="3441250">on</span> <span m="3441340">the</span> <span m="3441430">slide</span>
  <span m="3441820">that,</span> <span m="3442250">OK,</span> <span m="3442480">we</span>
  <span m="3442570">have</span> <span m="3442690">some</span> <span m="3442840">target</span>
  <span m="3443710">that's</span> <span m="3443890">R</span> <span m="3444130">plus</span>
  <span m="3444370">future</span> <span m="3445230">Q</span> <span m="3445450">values.</span>
  <span m="3446110">We</span> <span m="3446170">have</span> <span m="3446260">some</span>
  <span m="3446380">prediction</span> <span m="3446635">and</span> <span m="3446890">we</span>
  <span m="3446980">have</span> <span m="3447100">an</span> <span m="3447190">expectation</span>
  <span m="3447820">of our</span> <span m="3447970">transitions</span> <span m="3448510">here.</span></p><p><span
  m="3449470">But</span> <span m="3450010">how</span> <span m="3450250">do</span>
  <span m="3450370">I</span> <span m="3451240">evaluate</span> <span m="3451750">this</span>
  <span m="3451960">thing?</span> <span m="3453510">The</span> <span m="3453640">transitions</span>
  <span m="3454330">I</span> <span m="3454450">have</span> <span m="3454600">to</span>
  <span m="3454690">get</span> <span m="3454900">from</span> <span m="3455050">somewhere,</span>
  <span m="3455510">right?</span> <span m="3458050">And</span> <span m="3458320">another</span>
  <span m="3458560">way</span> <span m="3458650">to</span> <span m="3458740">say</span>
  <span m="3458950">that</span> <span m="3459040">is</span> <span m="3459190">what</span>
  <span m="3459520">are</span> <span m="3459610">the</span> <span m="3459730">inputs</span>
  <span m="3459970">and</span> <span m="3460060">the</span> <span m="3460150">outputs</span>
  <span m="3460450">of</span> <span m="3460540">our</span> <span m="3460600">regression?</span>
  <span m="3461470">Because</span> <span m="3462910">when</span> <span m="3463090">we</span>
  <span m="3463180">estimate</span> <span m="3463480">potential</span> <span m="3463870">outcomes,</span>
  <span m="3464800">we</span> <span m="3464950">have</span> <span m="3466270">a</span>
  <span m="3466360">very</span> <span m="3466570">clear</span> <span m="3467440">idea</span>
  <span m="3467770">of</span> <span m="3467860">this.</span> <span m="3468070">We</span>
  <span m="3468370">know</span> <span m="3468670">that</span> <span m="3468910">y,</span>
  <span m="3470660">the</span> <span m="3471580">outcome</span> <span m="3471910">itself,</span>
  <span m="3472420">is</span> <span m="3472530">a</span> <span m="3472600">target.</span>
  <span m="3473080">And</span> <span m="3473200">the</span> <span m="3473650">input</span>
  <span m="3474160">is</span> <span m="3474370">the</span> <span m="3475440">covariates,</span>
  <span m="3475960">x.</span></p><p><span m="3477670">But</span> <span m="3477850">here,</span>
  <span m="3478120">we</span> <span m="3478240">have</span> <span m="3478360">a</span>
  <span m="3478640">moving</span> <span m="3479020">target,</span> <span m="3479300">because</span>
  <span m="3480700">this</span> <span m="3480910">Q</span> <span m="3481190">hat,</span>
  <span m="3481510">it</span> <span m="3481630">has</span> <span m="3481750">to</span>
  <span m="3481810">come</span> <span m="3481990">from</span> <span m="3482140">somewhere,</span>
  <span m="3482500">too.</span> <span m="3483250">This</span> <span m="3483350">is</span>
  <span m="3483450">something</span> <span m="3483610">that</span> <span m="3483700">we</span>
  <span m="3483850">estimate</span> <span m="3484210">as</span> <span m="3484300">well.</span>
  <span m="3486260">So</span> <span m="3486610">usually</span> <span m="3487030">what</span>
  <span m="3487150">happens</span> <span m="3487420">is</span> <span m="3487540">that</span>
  <span m="3487660">we</span> <span m="3488830">alternate</span> <span m="3489550">between</span>
  <span m="3490120">updating</span> <span m="3490630">this</span> <span m="3490810">target,</span>
  <span m="3491230">Q,</span> <span m="3491800">and</span> <span m="3491980">Q</span>
  <span m="3492550">theta.</span> <span m="3492970">So</span> <span m="3493090">essentially,</span>
  <span m="3493420">we</span> <span m="3493510">copy</span> <span m="3493930">Q</span>
  <span m="3494140">theta</span> <span m="3494440">to</span> <span m="3494560">become</span>
  <span m="3494860">our</span> <span m="3494920">new</span> <span m="3495160">Q</span>
  <span m="3495520">hat</span> <span m="3495880">and</span> <span m="3496170">we</span>
  <span m="3496690">iterate</span> <span m="3497110">this</span> <span m="3497320">somehow.</span>
  <span m="3498010">But</span> <span m="3498190">I</span> <span m="3498280">still</span>
  <span m="3498490">haven't</span> <span m="3498730">told</span> <span m="3498910">you</span>
  <span m="3499000">how</span> <span m="3499120">to</span> <span m="3499240">evaluate</span>
  <span m="3499660">this</span> <span m="3499840">expectation.</span></p><p><span
  m="3502100">So</span> <span m="3502300">usually</span> <span m="3502720">in</span>
  <span m="3502870">RL,</span> <span m="3503230">there</span> <span m="3503410">are</span>
  <span m="3503440">a</span> <span m="3503500">few</span> <span m="3503710">different</span>
  <span m="3503950">ways</span> <span m="3504190">to</span> <span m="3504280">do</span>
  <span m="3504460">this.</span> <span m="3506080">And</span> <span m="3508300">either</span>
  <span m="3509620">depending</span> <span m="3509950">on</span> <span m="3510040">where</span>
  <span m="3510220">you</span> <span m="3510340">coming</span> <span m="3510610">from,</span>
  <span m="3510790">essentially,</span> <span m="3513190">these</span> <span m="3513430">are</span>
  <span m="3514030">varyingly</span> <span m="3514780">viable.</span> <span m="3515680">So</span>
  <span m="3516370">if</span> <span m="3516520">we</span> <span m="3516610">look</span>
  <span m="3516820">back</span> <span m="3517150">at</span> <span m="3517210">this</span>
  <span m="3521010">thing</span> <span m="3521190">here,</span> <span m="3521820">it</span>
  <span m="3521940">relies</span> <span m="3522360">on</span> <span m="3522450">having</span>
  <span m="3523080">tuples</span> <span m="3523500">of</span> <span m="3523620">transitions--</span>
  <span m="3524250">the</span> <span m="3524340">state,</span> <span m="3524820">the</span>
  <span m="3525000">action,</span> <span m="3525330">the</span> <span m="3525420">next</span>
  <span m="3525720">state,</span> <span m="3525930">and</span> <span m="3526020">the</span>
  <span m="3526080">reward</span> <span m="3526440">that</span> <span m="3526560">I</span>
  <span m="3526650">got.</span> <span m="3527850">So</span> <span m="3528000">I</span>
  <span m="3528090">have</span> <span m="3528270">to</span> <span m="3528360">somehow</span>
  <span m="3528870">observe</span> <span m="3529260">those.</span> <span m="3530760">And</span>
  <span m="3532350">I</span> <span m="3532440">can</span> <span m="3532560">obtain</span>
  <span m="3532890">them</span> <span m="3533040">in</span> <span m="3533100">various</span>
  <span m="3533370">ways.</span></p><p><span m="3534420">A</span> <span m="3534510">very</span>
  <span m="3534720">common</span> <span m="3535080">one</span> <span m="3535230">when</span>
  <span m="3535350">it</span> <span m="3535410">comes</span> <span m="3535680">to</span>
  <span m="3535830">learning</span> <span m="3536280">to</span> <span m="3536400">play</span>
  <span m="3536640">video</span> <span m="3536910">games,</span> <span m="3537150">for</span>
  <span m="3537210">example,</span> <span m="3537660">is that</span> <span m="3537810">you</span>
  <span m="3537900">do</span> <span m="3538050">something</span> <span m="3538320">called</span>
  <span m="3538560">on-policy</span> <span m="3539130">exploration.</span> <span m="3540110">That</span>
  <span m="3540210">means</span> <span m="3540480">that</span> <span m="3540660">you</span>
  <span m="3540810">observe</span> <span m="3541230">data</span> <span m="3541590">from</span>
  <span m="3541800">the</span> <span m="3541920">policy</span> <span m="3542310">that</span>
  <span m="3542440">you're</span> <span m="3542580">currently</span> <span m="3543120">optimizing.</span>
  <span m="3544200">You</span> <span m="3544290">just</span> <span m="3544500">play</span>
  <span m="3544830">the</span> <span m="3544920">game</span> <span m="3545340">according</span>
  <span m="3545760">to</span> <span m="3545850">the</span> <span m="3545940">policies</span>
  <span m="3546360">that you</span> <span m="3546420">have</span> <span m="3546600">at</span>
  <span m="3546690">the</span> <span m="3546750">moment.</span> <span m="3547810">And</span>
  <span m="3547830">the</span> <span m="3547890">analogy</span> <span m="3548490">in</span>
  <span m="3548610">health</span> <span m="3548740">care</span> <span m="3549000">would</span>
  <span m="3549150">be</span> <span m="3549300">that</span> <span m="3549540">you</span>
  <span m="3550050">have</span> <span m="3550170">some</span> <span m="3550380">idea</span>
  <span m="3550650">of</span> <span m="3550770">how</span> <span m="3551730">to</span>
  <span m="3551820">treat</span> <span m="3552060">patients</span> <span m="3552480">and</span>
  <span m="3552570">you</span> <span m="3552690">just</span> <span m="3552900">do</span>
  <span m="3553080">that</span> <span m="3553320">and</span> <span m="3553410">see</span>
  <span m="3553530">what</span> <span m="3553650">happens.</span> <span m="3555160">That</span>
  <span m="3555210">could</span> <span m="3555360">be</span> <span m="3555810">problematic,</span>
  <span m="3556870">especially</span> <span m="3557190">if</span> <span m="3557310">you've</span>
  <span m="3557400">got</span> <span m="3557640">that</span> <span m="3557790">policy--</span>
  <span m="3558810">if</span> <span m="3558870">you</span> <span m="3559290">randomly</span>
  <span m="3559710">initialized</span> <span m="3560180">it</span> <span m="3560310">or</span>
  <span m="3560490">if</span> <span m="3560580">you</span> <span m="3560670">got</span>
  <span m="3560850">it</span> <span m="3560910">for</span> <span m="3561030">some</span>
  <span m="3561540">somewhere</span> <span m="3562050">very</span> <span m="3562440">suboptimal.</span></p><p><span
  m="3564700">A</span> <span m="3564790">different</span> <span m="3565150">thing</span>
  <span m="3565390">that</span> <span m="3565480">we're</span> <span m="3565600">more,</span>
  <span m="3566710">perhaps,</span> <span m="3567370">comfortable</span> <span m="3567910">with</span>
  <span m="3568380">in</span> <span m="3568920">health</span> <span m="3569380">care,</span>
  <span m="3569610">in a</span> <span m="3569940">restricted</span> <span m="3570370">setting,</span>
  <span m="3570670">is</span> <span m="3570790">the</span> <span m="3570880">idea</span>
  <span m="3571030">of</span> <span m="3571120">a</span> <span m="3571180">randomized</span>
  <span m="3571630">trial,</span> <span m="3572500">where,</span> <span m="3572890">instead</span>
  <span m="3573220">of</span> <span m="3573310">trying</span> <span m="3573700">out</span>
  <span m="3574120">some</span> <span m="3574330">policy</span> <span m="3574690">that</span>
  <span m="3574810">you're</span> <span m="3574900">currently</span> <span m="3575230">learning,</span>
  <span m="3576070">you</span> <span m="3576190">decide</span> <span m="3576610">on</span>
  <span m="3577390">a</span> <span m="3577450">population</span> <span m="3578200">where</span>
  <span m="3578620">it's</span> <span m="3578860">OK</span> <span m="3579280">to</span>
  <span m="3579430">flip</span> <span m="3579670">a</span> <span m="3579700">coin,</span>
  <span m="3579970">essentially,</span> <span m="3581140">between</span> <span m="3581590">different</span>
  <span m="3581920">actions</span> <span m="3582250">that</span> <span m="3582340">you</span>
  <span m="3582430">have.</span> <span m="3585970">The</span> <span m="3586150">difference</span>
  <span m="3586480">between</span> <span m="3586690">the</span> <span m="3586780">sequential</span>
  <span m="3587230">setting</span> <span m="3587530">and</span> <span m="3587620">the</span>
  <span m="3587710">one-step</span> <span m="3588160">setting</span> <span m="3588400">is</span>
  <span m="3588730">that</span> <span m="3588850">now</span> <span m="3589040">we</span>
  <span m="3589150">have</span> <span m="3589270">to</span> <span m="3589360">randomize</span>
  <span m="3589870">a</span> <span m="3589930">sequence</span> <span m="3590650">of</span>
  <span m="3590770">actions,</span> <span m="3591850">which</span> <span m="3592000">is</span>
  <span m="3592240">a</span> <span m="3592330">little</span> <span m="3592480">bit</span>
  <span m="3592660">unlike</span> <span m="3593140">the</span> <span m="3593680">clinical</span>
  <span m="3593980">trials</span> <span m="3594280">that</span> <span m="3594430">you</span>
  <span m="3594580">have</span> <span m="3594670">seen</span> <span m="3594880">before,</span>
  <span m="3595180">I</span> <span m="3595270">think.</span></p><p><span m="3596740">The</span>
  <span m="3596830">last</span> <span m="3597040">one,</span> <span m="3597290">which</span>
  <span m="3597340">is</span> <span m="3597700">the</span> <span m="3598060">most</span>
  <span m="3598330">studied</span> <span m="3598660">one</span> <span m="3598840">when</span>
  <span m="3598990">it</span> <span m="3599650">comes</span> <span m="3599860">to</span>
  <span m="3599920">practice,</span> <span m="3600280">I</span> <span m="3600370">would</span>
  <span m="3600490">say,</span> <span m="3601750">is</span> <span m="3603040">the</span>
  <span m="3603220">one</span> <span m="3603400">that</span> <span m="3603490">we</span>
  <span m="3603580">talk</span> <span m="3603790">about</span> <span m="3604840">this</span>
  <span m="3604990">week--</span> <span m="3605470">is</span> <span m="3605620">off-policy</span>
  <span m="3606550">evaluation</span> <span m="3607180">or</span> <span m="3607570">learning,</span>
  <span m="3608290">in</span> <span m="3608380">which</span> <span m="3608650">case</span>
  <span m="3610750">you</span> <span m="3611050">observe</span> <span m="3611580">health</span>
  <span m="3611780">care</span> <span m="3611950">records,</span> <span m="3612250">for</span>
  <span m="3612310">example.</span> <span m="3612720">You</span> <span m="3612790">observe</span>
  <span m="3613150">registries.</span> <span m="3613660">You</span> <span m="3613720">observe</span>
  <span m="3613990">some</span> <span m="3614350">data</span> <span m="3614620">from</span>
  <span m="3614770">the</span> <span m="3614830">health</span> <span m="3615040">care</span>
  <span m="3615160">system</span> <span m="3615730">where</span> <span m="3615880">patients</span>
  <span m="3616240">have</span> <span m="3616360">already</span> <span m="3616720">been</span>
  <span m="3616870">treated</span> <span m="3617680">and</span> <span m="3617800">you</span>
  <span m="3617890">try</span> <span m="3618160">to</span> <span m="3618250">extract</span>
  <span m="3618700">a</span> <span m="3618760">good</span> <span m="3618910">policy</span>
  <span m="3619300">based</span> <span m="3619660">on</span> <span m="3619810">that</span>
  <span m="3619990">information.</span></p><p><span m="3621110">So</span> <span m="3621130">that</span>
  <span m="3621250">means</span> <span m="3621490">that</span> <span m="3621610">you</span>
  <span m="3621700">see</span> <span m="3622030">these</span> <span m="3622240">transitions</span>
  <span m="3622750">between</span> <span m="3623560">state</span> <span m="3624160">and</span>
  <span m="3624340">action</span> <span m="3624730">and</span> <span m="3624810">the</span>
  <span m="3624870">next</span> <span m="3625150">state</span> <span m="3625480">and</span>
  <span m="3625690">the</span> <span m="3625780">reward.</span> <span m="3626470">You</span>
  <span m="3626590">see</span> <span m="3626890">that</span> <span m="3627100">based</span>
  <span m="3627490">on</span> <span m="3627580">what</span> <span m="3627700">happened</span>
  <span m="3628120">in</span> <span m="3628210">the</span> <span m="3628300">past</span>
  <span m="3628960">and</span> <span m="3629080">you</span> <span m="3629170">have</span>
  <span m="3629290">to</span> <span m="3629350">figure</span> <span m="3629650">out</span>
  <span m="3629800">a</span> <span m="3629860">pattern</span> <span m="3630250">there</span>
  <span m="3630460">that</span> <span m="3630580">helps</span> <span m="3630880">you</span>
  <span m="3631120">come</span> <span m="3631300">up</span> <span m="3631420">with</span>
  <span m="3631540">a</span> <span m="3631570">good</span> <span m="3631720">action</span>
  <span m="3632410">or</span> <span m="3632530">a</span> <span m="3632680">good</span>
  <span m="3632830">policy.</span> <span m="3635250">So</span> <span m="3635520">we'll</span>
  <span m="3635700">focus</span> <span m="3636030">on</span> <span m="3636120">that</span>
  <span m="3636270">one</span> <span m="3636450">for</span> <span m="3636600">now.</span></p><p><span
  m="3638330">The</span> <span m="3638400">last</span> <span m="3638640">part</span>
  <span m="3638880">of</span> <span m="3638940">this</span> <span m="3639090">talk</span>
  <span m="3639300">will</span> <span m="3639450">be</span> <span m="3639630">about,</span>
  <span m="3644590">essentially,</span> <span m="3644910">what</span> <span m="3645030">we</span>
  <span m="3645150">have</span> <span m="3645240">to</span> <span m="3645330">be</span>
  <span m="3645450">careful</span> <span m="3645840">with</span> <span m="3646080">when</span>
  <span m="3646230">we</span> <span m="3646350">learn</span> <span m="3646620">with</span>
  <span m="3647760">off-policy</span> <span m="3648510">data.</span> <span m="3650380">Any</span>
  <span m="3650520">questions</span> <span m="3650790">up</span> <span m="3650940">until</span>
  <span m="3651210">this</span> <span m="3651360">point?</span> <span m="3654580">Yeah.</span></p><p><span
  m="3655910">AUDIENCE:</span> <span m="3656135">So</span> <span m="3657320">if</span>
  <span m="3657800">[INAUDIBLE]</span> <span m="3658640">getting</span> <span m="3658790">there</span>
  <span m="3659150">for</span> <span m="3659300">the</span> <span m="3659895">[INAUDIBLE],</span>
  <span m="3661450">are there any</span> <span m="3662280">requirements</span> <span
  m="3662900">that</span> <span m="3663060">has</span> <span m="3663320">to</span>
  <span m="3663380">be</span> <span m="3663500">met</span> <span m="3664120">by</span>
  <span m="3664811">[INAUDIBLE],</span> <span m="3665262">like</span> <span m="3665713">how</span>
  <span m="3666164">we</span> <span m="3666615">had</span> <span m="3667066">[INAUDIBLE]</span>
  <span m="3667968">and</span> <span m="3668420">cause inference?</span></p><p><span
  m="3669580">FREDRIK D. JOHANSSON:</span> <span m="3669660">Yeah,</span> <span m="3670220">I'll</span>
  <span m="3670310">get</span> <span m="3670430">to</span> <span m="3670520">that</span>
  <span m="3671300">on</span> <span m="3671390">the</span> <span m="3671450">next</span>
  <span m="3671630">set</span> <span m="3671720">of</span> <span m="3671840">slides.</span>
  <span m="3673520">Thank</span> <span m="3673570">you.</span> <span m="3674980">Any</span>
  <span m="3675070">other</span> <span m="3675200">questions</span> <span m="3675500">about</span>
  <span m="3675860">the</span> <span m="3675960">Q-learning</span> <span m="3676280">part?</span>
  <span m="3677560">A</span> <span m="3677660">colleague</span> <span m="3677930">of</span>
  <span m="3678020">mine,</span> <span m="3678320">Rahul,</span> <span m="3678710">he</span>
  <span m="3679040">said--</span> <span m="3679880">or</span> <span m="3680210">maybe</span>
  <span m="3680660">he</span> <span m="3680780">just</span> <span m="3681020">paraphrased</span>
  <span m="3681500">it</span> <span m="3681560">from</span> <span m="3681680">someone</span>
  <span m="3681950">else.</span> <span m="3682130">But</span> <span m="3682220">essentially,</span>
  <span m="3683120">you</span> <span m="3683210">have</span> <span m="3683330">to</span>
  <span m="3683420">see</span> <span m="3683750">RL</span> <span m="3684130">10</span>
  <span m="3684380">times</span> <span m="3684680">before</span> <span m="3684890">you</span>
  <span m="3684980">get</span> <span m="3685190">it,</span> <span m="3685310">or</span>
  <span m="3685400">something</span> <span m="3686300">to</span> <span m="3686450">that</span>
  <span m="3686630">effect.</span> <span m="3687350">I</span> <span m="3687500">had</span>
  <span m="3687620">the</span> <span m="3687710">same</span> <span m="3687890">experience.</span>
  <span m="3688440">So</span> <span m="3689240">hopefully</span> <span m="3689600">you</span>
  <span m="3689660">have</span> <span m="3689780">questions</span> <span m="3690080">for</span>
  <span m="3690170">me</span> <span m="3690320">after.</span></p><p><span m="3691770">AUDIENCE:</span>
  <span m="3692020">Human</span> <span m="3692270">reinforcement</span> <span m="3692585">learning.</span></p><p><span
  m="3696010">FREDRIK D. JOHANSSON:</span> <span m="3696205">Exactly.</span> <span
  m="3697800">But</span> <span m="3698540">I</span> <span m="3698600">think</span>
  <span m="3698810">what</span> <span m="3699170">you</span> <span m="3699260">should</span>
  <span m="3699380">take</span> <span m="3699590">from</span> <span m="3699770">the</span>
  <span m="3700220">last</span> <span m="3700520">two</span> <span m="3700790">sections,</span>
  <span m="3701180">if</span> <span m="3701540">not</span> <span m="3702170">how</span>
  <span m="3702320">to</span> <span m="3702460">do</span> <span m="3702560">Q-learning</span>
  <span m="3703040">in</span> <span m="3703130">detail,</span> <span m="3703490">because</span>
  <span m="3703760">I</span> <span m="3703820">glossed</span> <span m="3704090">over</span>
  <span m="3704210">a</span> <span m="3704240">lot</span> <span m="3704330">of</span>
  <span m="3704390">things.</span> <span m="3704930">You</span> <span m="3705110">should</span>
  <span m="3706130">take</span> <span m="3706370">with</span> <span m="3706550">you</span>
  <span m="3706640">the</span> <span m="3706790">idea</span> <span m="3707180">of</span>
  <span m="3707390">dynamic</span> <span m="3707780">programming</span> <span m="3708230">and</span>
  <span m="3708320">figuring</span> <span m="3708710">out,</span> <span m="3709230">how</span>
  <span m="3709310">can</span> <span m="3709490">I</span> <span m="3709580">learn</span>
  <span m="3709880">about</span> <span m="3710240">what's</span> <span m="3710450">good</span>
  <span m="3710900">early</span> <span m="3711200">on</span> <span m="3711500">in</span>
  <span m="3711560">my</span> <span m="3711680">process</span> <span m="3712010">from</span>
  <span m="3712160">what's</span> <span m="3712400">good</span> <span m="3712580">late?</span>
  <span m="3713330">And</span> <span m="3713630">the</span> <span m="3713780">idea</span>
  <span m="3714080">of</span> <span m="3714560">moving</span> <span m="3714950">towards</span>
  <span m="3715540">a</span> <span m="3715610">good</span> <span m="3715790">state</span>
  <span m="3716090">and</span> <span m="3716180">not</span> <span m="3716390">just</span>
  <span m="3716600">arriving</span> <span m="3716990">there</span> <span m="3717170">immediately.</span>
  <span m="3718640">And</span> <span m="3718940">there</span> <span m="3719030">are</span>
  <span m="3719090">many</span> <span m="3719300">ways</span> <span m="3719480">to</span>
  <span m="3720260">think</span> <span m="3720410">about</span> <span m="3720650">that.</span></p><p><span
  m="3721520">OK,</span> <span m="3722150">we'll</span> <span m="3722300">move on</span>
  <span m="3722740">to</span> <span m="3723640">off-policy</span> <span m="3724220">learning.</span>
  <span m="3725780">And</span> <span m="3726140">again,</span> <span m="3726570">the</span>
  <span m="3726670">set-up</span> <span m="3726860">here</span> <span m="3727040">is</span>
  <span m="3727190">that</span> <span m="3727320">we</span> <span m="3728420">receive</span>
  <span m="3728780">trajectories</span> <span m="3729470">of</span> <span m="3729560">patient</span>
  <span m="3730400">states,</span> <span m="3730880">actions,</span> <span m="3731180">and</span>
  <span m="3731300">rewards</span> <span m="3731900">from</span> <span m="3732290">some</span>
  <span m="3732530">source.</span> <span m="3732990">We</span> <span m="3733280">don't</span>
  <span m="3733490">know</span> <span m="3734330">what</span> <span m="3734570">these</span>
  <span m="3734690">sources</span> <span m="3735140">necessarily--</span> <span m="3735620">well,</span>
  <span m="3735950">we</span> <span m="3736040">probably</span> <span m="3736280">know</span>
  <span m="3736400">what</span> <span m="3736520">the</span> <span m="3736580">source</span>
  <span m="3736900">is.</span> <span m="3737000">But</span> <span m="3737120">we</span>
  <span m="3737210">don't</span> <span m="3737360">know</span> <span m="3737630">how</span>
  <span m="3737930">these</span> <span m="3738170">actions</span> <span m="3738500">were</span>
  <span m="3738620">performed,</span> <span m="3739400">i.e.,</span> <span m="3739730">we</span>
  <span m="3739850">don't</span> <span m="3740150">know</span> <span m="3740300">what</span>
  <span m="3740450">the</span> <span m="3740510">policy</span> <span m="3740930">was</span>
  <span m="3741170">that</span> <span m="3741290">generated</span> <span m="3741740">these</span>
  <span m="3741920">trajectories.</span> <span m="3742670">And</span> <span m="3742760">this</span>
  <span m="3742880">is</span> <span m="3742970">the</span> <span m="3743030">same</span>
  <span m="3743300">set-up</span> <span m="3743630">as</span> <span m="3744080">when</span>
  <span m="3744230">you</span> <span m="3744290">estimated</span> <span m="3744800">causal</span>
  <span m="3745100">effects</span> <span m="3745340">last</span> <span m="3745550">week,</span>
  <span m="3745820">to</span> <span m="3746290">a</span> <span m="3746530">large</span>
  <span m="3746990">extent.</span></p><p><span m="3748580">We</span> <span m="3749000">say</span>
  <span m="3749270">that</span> <span m="3749930">the</span> <span m="3750080">actions</span>
  <span m="3750440">are</span> <span m="3750500">drawn,</span> <span m="3750830">again,</span>
  <span m="3751190">according</span> <span m="3751460">to</span> <span m="3751610">some</span>
  <span m="3751760">behavior</span> <span m="3752060">policy</span> <span m="3752990">unknown</span>
  <span m="3753380">to</span> <span m="3753530">us.</span> <span m="3754010">But</span>
  <span m="3754190">we</span> <span m="3754340">want</span> <span m="3754550">to</span>
  <span m="3754640">figure</span> <span m="3754940">out</span> <span m="3755030">what</span>
  <span m="3755210">is</span> <span m="3755300">the</span> <span m="3755390">value</span>
  <span m="3755930">of</span> <span m="3756050">a</span> <span m="3756110">new</span>
  <span m="3756410">policy,</span> <span m="3756830">pi.</span> <span m="3757880">So</span>
  <span m="3758180">when</span> <span m="3758390">I</span> <span m="3758810">showed</span>
  <span m="3759130">you</span> <span m="3759260">very</span> <span m="3759680">early</span>
  <span m="3759950">on--</span> <span m="3760070">I</span> <span m="3760130">wish</span>
  <span m="3760310">I</span> <span m="3760400">had</span> <span m="3760520">that</span>
  <span m="3760640">slide</span> <span m="3760910">again.</span></p><p><span m="3761360">But</span>
  <span m="3761510">essentially,</span> <span m="3762530">a</span> <span m="3762590">bunch</span>
  <span m="3762950">of</span> <span m="3764090">patient</span> <span m="3764450">trajectories</span>
  <span m="3765260">and</span> <span m="3765440">some</span> <span m="3765740">return.</span>
  <span m="3766760">Patient</span> <span m="3767090">trajectories,</span> <span m="3767490">some</span>
  <span m="3767690">return.</span> <span m="3769400">The</span> <span m="3769550">average</span>
  <span m="3769910">of</span> <span m="3770000">those,</span> <span m="3770270">that's</span>
  <span m="3770810">called</span> <span m="3771070">a</span> <span m="3771140">value.</span>
  <span m="3772190">If</span> <span m="3772370">we</span> <span m="3772520">have</span>
  <span m="3773210">trajectories</span> <span m="3773870">according</span> <span m="3774200">to</span>
  <span m="3774320">a</span> <span m="3774380">certain</span> <span m="3774620">policy,</span>
  <span m="3775430">that</span> <span m="3775670">is</span> <span m="3775820">the</span>
  <span m="3775940">value</span> <span m="3776240">of</span> <span m="3776300">that</span>
  <span m="3776450">policy--</span> <span m="3777140">the</span> <span m="3777410">average</span>
  <span m="3777800">of</span> <span m="3777890">these</span> <span m="3778100">things.</span>
  <span m="3779030">But</span> <span m="3779150">when</span> <span m="3779300">we</span>
  <span m="3779420">have</span> <span m="3780230">trajectories</span> <span m="3780830">according</span>
  <span m="3781100">to</span> <span m="3781160">one</span> <span m="3781400">policy</span>
  <span m="3781760">and</span> <span m="3781850">want</span> <span m="3781970">to</span>
  <span m="3782030">figure</span> <span m="3782240">out</span> <span m="3782360">the</span>
  <span m="3782420">value</span> <span m="3782690">of</span> <span m="3782780">another</span>
  <span m="3783170">one,</span> <span m="3783980">that's</span> <span m="3784160">the</span>
  <span m="3784220">same</span> <span m="3784970">problem</span> <span m="3785600">as</span>
  <span m="3785870">the</span> <span m="3786050">covariate</span> <span m="3786400">adjustment</span>
  <span m="3786770">problem</span> <span m="3787010">that</span> <span m="3787100">you</span>
  <span m="3787190">had</span> <span m="3787340">last</span> <span m="3787610">week,</span>
  <span m="3787820">essentially.</span> <span m="3788400">Or</span> <span m="3788900">the</span>
  <span m="3789200">confounding</span> <span m="3789650">problem,</span> <span m="3789920">essentially.</span></p><p><span
  m="3793320">The</span> <span m="3793760">trajectories</span> <span m="3794330">that</span>
  <span m="3794540">we</span> <span m="3795230">draw</span> <span m="3795650">are</span>
  <span m="3795740">biased</span> <span m="3796220">according</span> <span m="3796550">to</span>
  <span m="3796730">the</span> <span m="3796940">policy</span> <span m="3797450">of</span>
  <span m="3797630">the</span> <span m="3797840">clinician</span> <span m="3798380">that</span>
  <span m="3798860">created</span> <span m="3799340">them.</span> <span m="3800000">And</span>
  <span m="3800120">we</span> <span m="3800210">want</span> <span m="3800390">to</span>
  <span m="3800450">figure</span> <span m="3800720">out</span> <span m="3800960">the</span>
  <span m="3802220">value</span> <span m="3802490">of</span> <span m="3802550">a</span>
  <span m="3802610">different</span> <span m="3802880">policy.</span> <span m="3803270">So</span>
  <span m="3803390">it's</span> <span m="3803480">the</span> <span m="3803540">same</span>
  <span m="3803780">as</span> <span m="3803870">the</span> <span m="3803930">confounding</span>
  <span m="3804320">problem</span> <span m="3804590">from the</span> <span m="3804770">last</span>
  <span m="3804980">time.</span></p><p><span m="3806030">And</span> <span m="3806150">because</span>
  <span m="3806540">it</span> <span m="3806600">is</span> <span m="3806720">the</span>
  <span m="3806780">same</span> <span m="3806990">as</span> <span m="3807080">the</span>
  <span m="3807140">confounding</span> <span m="3807530">from</span> <span m="3808130">last</span>
  <span m="3808400">time,</span> <span m="3810260">we</span> <span m="3810410">know</span>
  <span m="3810680">that</span> <span m="3810800">this</span> <span m="3810950">is</span>
  <span m="3811310">at</span> <span m="3811430">least</span> <span m="3811730">as</span>
  <span m="3811820">hard</span> <span m="3812480">as</span> <span m="3812600">doing</span>
  <span m="3812810">that.</span> <span m="3813160">We</span> <span m="3813320">have</span>
  <span m="3813440">confounding--</span> <span m="3814490">I</span> <span m="3814640">already</span>
  <span m="3814970">alluded</span> <span m="3815240">to</span> <span m="3815660">variance</span>
  <span m="3816050">issues.</span> <span m="3816310">And</span> <span m="3816420">you</span>
  <span m="3816560">mentioned</span> <span m="3816950">overlap</span> <span m="3817370">or</span>
  <span m="3817760">positivity</span> <span m="3818390">as</span> <span m="3818540">well.</span>
  <span m="3819210">And</span> <span m="3819230">in</span> <span m="3819290">fact,</span>
  <span m="3819650">we</span> <span m="3819890">need</span> <span m="3820130">to</span>
  <span m="3820220">make</span> <span m="3820610">the</span> <span m="3820730">same</span>
  <span m="3821060">assumptions</span> <span m="3821480">but</span> <span m="3821630">even</span>
  <span m="3822200">stronger</span> <span m="3822620">assumptions</span> <span m="3823070">for</span>
  <span m="3823220">this</span> <span m="3823370">to</span> <span m="3823490">be</span>
  <span m="3823580">possible.</span></p><p><span m="3827150">These</span> <span m="3827230">are</span>
  <span m="3827320">sufficient</span> <span m="3827740">conditions.</span> <span m="3828190">So,</span>
  <span m="3828370">under</span> <span m="3829120">very</span> <span m="3829360">certain</span>
  <span m="3829720">circumstances,</span> <span m="3830410">you</span> <span m="3830500">don't</span>
  <span m="3830800">need</span> <span m="3830980">them.</span> <span m="3833380">I</span>
  <span m="3833440">should</span> <span m="3833550">say,</span> <span m="3833710">these</span>
  <span m="3833890">are</span> <span m="3833980">fairly</span> <span m="3834310">general</span>
  <span m="3834760">assumptions</span> <span m="3835240">that</span> <span m="3835360">are</span>
  <span m="3835450">still</span> <span m="3835750">strict--</span> <span m="3836350">that's</span>
  <span m="3836500">how</span> <span m="3836630">I</span> <span m="3836700">should</span>
  <span m="3836790">put</span> <span m="3836920">it.</span></p><p><span m="3838430">So</span>
  <span m="3838540">last</span> <span m="3838780">time,</span> <span m="3839210">we</span>
  <span m="3839290">looked</span> <span m="3839500">at</span> <span m="3839590">something</span>
  <span m="3839830">called</span> <span m="3840070">strong</span> <span m="3840400">ignorability.</span>
  <span m="3840970">I</span> <span m="3841150">realized</span> <span m="3841450">the</span>
  <span m="3841540">text is</span> <span m="3841870">pretty</span> <span m="3842080">small</span>
  <span m="3842330">in here.</span> <span m="3842450">Can</span> <span m="3842560">you</span>
  <span m="3842620">see</span> <span m="3842830">in</span> <span m="3842950">the</span>
  <span m="3843040">back?</span> <span m="3843410">Is that OK?</span> <span m="3843820">OK,</span>
  <span m="3844420">great.</span></p><p><span m="3845140">So</span> <span m="3845260">strong</span>
  <span m="3845510">ignorability</span> <span m="3846250">said</span> <span m="3846550">that</span>
  <span m="3846760">the</span> <span m="3846880">potential</span> <span m="3847330">outcomes--</span>
  <span m="3847840">Y0</span> <span m="3848220">and</span> <span m="3848320">Y1--</span>
  <span m="3849190">are</span> <span m="3849280">conditionally</span> <span m="3849820">independent</span>
  <span m="3850390">of</span> <span m="3850540">the</span> <span m="3850660">treatment,</span>
  <span m="3851080">t,</span> <span m="3851740">given</span> <span m="3852430">the</span>
  <span m="3852760">set</span> <span m="3853150">of</span> <span m="3853300">variables,</span>
  <span m="3853840">x,</span> <span m="3854110">or</span> <span m="3854230">the</span>
  <span m="3854320">variable,</span> <span m="3854650">x.</span> <span m="3855940">And</span>
  <span m="3856360">that's</span> <span m="3857080">saying</span> <span m="3857410">that</span>
  <span m="3857800">it</span> <span m="3857890">doesn't</span> <span m="3858130">matter</span>
  <span m="3858670">if</span> <span m="3858820">we</span> <span m="3858940">know</span>
  <span m="3859120">what</span> <span m="3859300">treatment</span> <span m="3859630">was</span>
  <span m="3860200">given.</span> <span m="3860890">We</span> <span m="3861040">can</span>
  <span m="3861190">figure</span> <span m="3861520">out</span> <span m="3861730">just</span>
  <span m="3861940">based</span> <span m="3862180">on</span> <span m="3862300">x</span>
  <span m="3862930">what</span> <span m="3863140">would</span> <span m="3863260">happen</span>
  <span m="3863650">under</span> <span m="3863890">either</span> <span m="3864160">treatment</span>
  <span m="3864580">arm,</span> <span m="3865120">where</span> <span m="3865270">we</span>
  <span m="3865390">should</span> <span m="3865490">treat</span> <span m="3865720">this</span>
  <span m="3865840">patient,</span> <span m="3866170">with</span> <span m="3866520">t</span>
  <span m="3866870">equals</span> <span m="3867070">0,</span> <span m="3867360">t</span>
  <span m="3867460">equals</span> <span m="3867610">1.</span></p><p><span m="3869610">We</span>
  <span m="3869760">had</span> <span m="3869880">an</span> <span m="3869970">idea</span>
  <span m="3870240">of--</span> <span m="3870920">or</span> <span m="3871170">an</span>
  <span m="3871290">assumption</span> <span m="3871590">of--</span> <span m="3871740">overlap,</span>
  <span m="3872220">which</span> <span m="3872340">says</span> <span m="3872520">that</span>
  <span m="3872700">any</span> <span m="3872940">treatment</span> <span m="3873360">could</span>
  <span m="3873570">be</span> <span m="3874890">observed</span> <span m="3875970">in</span>
  <span m="3876090">any</span> <span m="3876360">state</span> <span m="3879030">or</span>
  <span m="3879300">any</span> <span m="3879630">context,</span> <span m="3880290">x.</span>
  <span m="3884250">That's</span> <span m="3884980">what</span> <span m="3885090">that</span>
  <span m="3885180">means.</span> <span m="3885660">And</span> <span m="3885840">that</span>
  <span m="3885990">is</span> <span m="3886410">only</span> <span m="3886680">to</span>
  <span m="3887550">ensure</span> <span m="3888030">that</span> <span m="3888450">we</span>
  <span m="3888600">can</span> <span m="3888930">estimate</span> <span m="3889290">at</span>
  <span m="3889350">least</span> <span m="3889620">a</span> <span m="3889680">conditional</span>
  <span m="3890130">average</span> <span m="3890490">treatment</span> <span m="3890820">effect</span>
  <span m="3891180">at</span> <span m="3891390">x.</span> <span m="3894210">And</span>
  <span m="3895020">if</span> <span m="3895170">we</span> <span m="3895290">want</span>
  <span m="3895470">to</span> <span m="3895830">estimate</span> <span m="3896130">the</span>
  <span m="3896220">average</span> <span m="3896610">treatment</span> <span m="3896970">effect</span>
  <span m="3897210">in</span> <span m="3897330">a</span> <span m="3897390">population,</span>
  <span m="3898150">we</span> <span m="3898200">would</span> <span m="3898340">need</span>
  <span m="3898500">to</span> <span m="3899460">have</span> <span m="3899640">that</span>
  <span m="3899760">for</span> <span m="3899880">every</span> <span m="3900240">x</span>
  <span m="3900480">in</span> <span m="3900570">that</span> <span m="3900660">population.</span></p><p><span
  m="3902620">So</span> <span m="3902700">what</span> <span m="3902850">happens</span>
  <span m="3903120">in</span> <span m="3903210">the</span> <span m="3903330">sequential</span>
  <span m="3903810">case</span> <span m="3904200">is</span> <span m="3904350">that</span>
  <span m="3904500">we</span> <span m="3904650">need</span> <span m="3905070">even</span>
  <span m="3905370">stronger</span> <span m="3906000">assumptions.</span> <span m="3908070">There's</span>
  <span m="3908250">some</span> <span m="3908520">notation</span> <span m="3909000">I</span>
  <span m="3909090">haven't</span> <span m="3909480">introduced</span> <span m="3909990">here</span>
  <span m="3910160">and I</span> <span m="3910260">apologize</span> <span m="3910740">for</span>
  <span m="3910860">that.</span> <span m="3911230">But</span> <span m="3911730">there's</span>
  <span m="3912630">a</span> <span m="3912720">bar</span> <span m="3913140">here</span>
  <span m="3913500">over</span> <span m="3913770">these</span> <span m="3914370">Ss</span>
  <span m="3914700">and</span> <span m="3914820">As--</span> <span m="3915540">I</span>
  <span m="3915570">don't</span> <span m="3915690">know</span> <span m="3915810">if</span>
  <span m="3915900">you</span> <span m="3915990">can</span> <span m="3916110">see</span>
  <span m="3916230">it.</span> <span m="3916800">That</span> <span m="3916950">usually</span>
  <span m="3917370">indicates</span> <span m="3917820">in</span> <span m="3917920">this</span>
  <span m="3918090">literature</span> <span m="3918660">that</span> <span m="3919020">you're</span>
  <span m="3919200">looking</span> <span m="3919500">at</span> <span m="3919590">the</span>
  <span m="3919920">sequence,</span> <span m="3920760">up</span> <span m="3920910">to</span>
  <span m="3922020">the</span> <span m="3922200">index</span> <span m="3922560">here.</span>
  <span m="3923100">So</span> <span m="3923550">all</span> <span m="3923790">the</span>
  <span m="3923880">states</span> <span m="3924420">up</span> <span m="3924600">until</span>
  <span m="3924930">t</span> <span m="3926400">have</span> <span m="3926530">observed</span>
  <span m="3927140">and</span> <span m="3927280">all</span> <span m="3927400">the</span>
  <span m="3927520">actions</span> <span m="3927940">up</span> <span m="3928090">until</span>
  <span m="3928330">t</span> <span m="3928480">minus</span> <span m="3928780">1.</span></p><p><span
  m="3934790">So</span> <span m="3935000">in</span> <span m="3935120">order</span>
  <span m="3935510">for</span> <span m="3936470">the</span> <span m="3937850">best</span>
  <span m="3938210">policy</span> <span m="3938630">to</span> <span m="3938750">be</span>
  <span m="3938930">identifiable--</span> <span m="3939560">or</span> <span m="3939680">the</span>
  <span m="3939800">value</span> <span m="3940130">of</span> <span m="3940220">a</span>
  <span m="3940260">positive</span> <span m="3940640">to</span> <span m="3940730">be</span>
  <span m="3940850">identifiable--</span> <span m="3941480">we</span> <span m="3941630">need</span>
  <span m="3941930">this</span> <span m="3942530">strong</span> <span m="3942800">condition.</span>
  <span m="3943880">So</span> <span m="3944540">the</span> <span m="3944930">return</span>
  <span m="3945380">of</span> <span m="3945440">a</span> <span m="3945470">policy</span>
  <span m="3945980">is</span> <span m="3946220">independent</span> <span m="3946700">of</span>
  <span m="3946760">the</span> <span m="3946850">current</span> <span m="3947120">action,</span>
  <span m="3947450">given</span> <span m="3947810">everything</span> <span m="3948140">that</span>
  <span m="3948230">happened</span> <span m="3948470">in</span> <span m="3948530">the</span>
  <span m="3948620">past.</span> <span m="3954380">This</span> <span m="3954530">is</span>
  <span m="3954650">weaker</span> <span m="3955130">than</span> <span m="3955280">the</span>
  <span m="3955370">Markov</span> <span m="3955700">assumption,</span> <span m="3956060">to</span>
  <span m="3956150">be</span> <span m="3956240">clear,</span> <span m="3956570">because</span>
  <span m="3956870">there,</span> <span m="3957110">we</span> <span m="3957230">said</span>
  <span m="3957500">that</span> <span m="3958280">anything</span> <span m="3958550">that</span>
  <span m="3958640">happens</span> <span m="3958850">in</span> <span m="3958940">the</span>
  <span m="3959000">future</span> <span m="3959330">is</span> <span m="3959450">conditionally</span>
  <span m="3959830">independent,</span> <span m="3960500">given</span> <span m="3960890">the</span>
  <span m="3960980">current</span> <span m="3961220">state.</span> <span m="3962430">So</span>
  <span m="3962480">this</span> <span m="3962630">is</span> <span m="3962750">weaker,</span>
  <span m="3964070">because</span> <span m="3964580">we</span> <span m="3965300">now</span>
  <span m="3965480">just</span> <span m="3965990">need</span> <span m="3966260">to</span>
  <span m="3966410">observe</span> <span m="3967190">something</span> <span m="3967580">in</span>
  <span m="3967730">the</span> <span m="3967850">history.</span> <span m="3969010">We</span>
  <span m="3969200">need</span> <span m="3969290">to</span> <span m="3969440">observe</span>
  <span m="3969810">all</span> <span m="3969950">confounders</span> <span m="3970310">in</span>
  <span m="3970420">the</span> <span m="3970520">history,</span> <span m="3971040">in</span>
  <span m="3971270">this</span> <span m="3971450">instance.</span></p><p><span m="3972180">We</span>
  <span m="3972280">don't</span> <span m="3972350">need</span> <span m="3972500">to</span>
  <span m="3972590">summarize</span> <span m="3973010">them</span> <span m="3973130">in</span>
  <span m="3973220">S.</span> <span m="3974090">And</span> <span m="3974310">we'll</span>
  <span m="3974480">get</span> <span m="3974570">back</span> <span m="3974720">to</span>
  <span m="3974810">this in the</span> <span m="3975070">next</span> <span m="3975290">slide.</span>
  <span m="3976010">Positivity</span> <span m="3976610">is</span> <span m="3976740">the</span>
  <span m="3976820">real</span> <span m="3977600">difficult</span> <span m="3977990">one,</span>
  <span m="3978200">though,</span> <span m="3978410">because</span> <span m="3978920">what</span>
  <span m="3979130">we're</span> <span m="3979220">saying</span> <span m="3979550">is</span>
  <span m="3979640">that</span> <span m="3980000">at</span> <span m="3980150">any</span>
  <span m="3980420">point</span> <span m="3980780">in</span> <span m="3980930">the</span>
  <span m="3981050">trajectory,</span> <span m="3982490">any</span> <span m="3982730">action</span>
  <span m="3983030">should</span> <span m="3983150">be</span> <span m="3983240">possible</span>
  <span m="3985880">in</span> <span m="3986030">order</span> <span m="3986120">for</span>
  <span m="3986240">us</span> <span m="3986330">to</span> <span m="3986450">estimate</span>
  <span m="3986720">the</span> <span m="3986810">value</span> <span m="3987110">of</span>
  <span m="3987290">any</span> <span m="3987530">possible</span> <span m="3987890">policy.</span>
  <span m="3988670">And</span> <span m="3988950">we</span> <span m="3989090">know</span>
  <span m="3989450">that</span> <span m="3989780">that's</span> <span m="3990020">not</span>
  <span m="3990140">going</span> <span m="3990250">to</span> <span m="3990320">be</span>
  <span m="3990410">true</span> <span m="3990620">in</span> <span m="3990740">practice.</span></p><p><span
  m="3991770">We're</span> <span m="3992000">not</span> <span m="3992270">going</span>
  <span m="3992380">to</span> <span m="3992480">consider</span> <span m="3992930">every</span>
  <span m="3993200">possible</span> <span m="3993590">action</span> <span m="3993890">at</span>
  <span m="3994010">every</span> <span m="3994940">possible</span> <span m="3995270">point</span>
  <span m="3996710">in</span> <span m="3997040">the</span> <span m="3997100">health</span>
  <span m="3997250">care</span> <span m="3997400">setting.</span> <span m="3997820">There's</span>
  <span m="3998000">just</span> <span m="3998180">no</span> <span m="3998330">way.</span>
  <span m="3999570">So</span> <span m="4000040">what</span> <span m="4000280">that</span>
  <span m="4000400">tells</span> <span m="4000700">us</span> <span m="4000820">is</span>
  <span m="4000940">that</span> <span m="4001990">we</span> <span m="4002140">can't</span>
  <span m="4002740">estimate</span> <span m="4003160">the</span> <span m="4003220">value</span>
  <span m="4003670">of</span> <span m="4003850">every</span> <span m="4004180">possible</span>
  <span m="4004630">policy.</span> <span m="4005440">We</span> <span m="4005530">can</span>
  <span m="4005680">only</span> <span m="4006010">estimate</span> <span m="4006730">the</span>
  <span m="4006820">value</span> <span m="4007090">of</span> <span m="4007180">policies</span>
  <span m="4007900">that</span> <span m="4008050">are</span> <span m="4008170">consistent</span>
  <span m="4008770">with</span> <span m="4012620">the</span> <span m="4012710">support</span>
  <span m="4013070">that</span> <span m="4013190">we</span> <span m="4013280">do</span>
  <span m="4013460">have.</span></p><p><span m="4014660">If</span> <span m="4014780">we</span>
  <span m="4014900">never</span> <span m="4015260">see</span> <span m="4015830">action</span>
  <span m="4016370">4</span> <span m="4016790">at</span> <span m="4017030">time</span>
  <span m="4017430">3,</span> <span m="4018050">there's</span> <span m="4018200">no</span>
  <span m="4018350">way</span> <span m="4018590">we</span> <span m="4018680">can</span>
  <span m="4019130">learn</span> <span m="4019400">about</span> <span m="4019640">a</span>
  <span m="4019670">policy</span> <span m="4020060">that</span> <span m="4020210">does</span>
  <span m="4020420">that--</span> <span m="4021130">that</span> <span m="4021650">takes</span>
  <span m="4021920">action</span> <span m="4022220">4</span> <span m="4022390">at</span>
  <span m="4022450">time</span> <span m="4022610">3.</span> <span m="4022880">That's</span>
  <span m="4023030">what</span> <span m="4023120">I'm</span> <span m="4023210">trying</span>
  <span m="4023390">to</span> <span m="4023450">say.</span> <span m="4024150">So</span>
  <span m="4024620">in</span> <span m="4024740">some</span> <span m="4024920">sense,</span>
  <span m="4025100">this</span> <span m="4025280">is</span> <span m="4028750">stronger,</span>
  <span m="4029950">just</span> <span m="4030160">because</span> <span m="4030610">of</span>
  <span m="4030730">how</span> <span m="4031390">sequential</span> <span m="4031960">settings</span>
  <span m="4032470">work.</span> <span m="4034030">It's</span> <span m="4034330">more</span>
  <span m="4034540">about</span> <span m="4034720">the</span> <span m="4034810">application</span>
  <span m="4035200">domain</span> <span m="4035470">than</span> <span m="4035590">anything,</span>
  <span m="4035950">I</span> <span m="4036010">would</span> <span m="4036130">say.</span></p><p><span
  m="4037770">In</span> <span m="4037900">the</span> <span m="4037960">next</span>
  <span m="4038140">set</span> <span m="4038230">of</span> <span m="4038290">slides,</span>
  <span m="4038620">we'll</span> <span m="4038740">focus</span> <span m="4039190">on</span>
  <span m="4040000">sequential</span> <span m="4040390">randomization</span> <span
  m="4041080">or</span> <span m="4041170">sequential</span> <span m="4041600">ignorability,</span>
  <span m="4041810">as</span> <span m="4042100">it's</span> <span m="4042210">sometimes</span>
  <span m="4042730">called.</span> <span m="4043520">And</span> <span m="4044830">tomorrow,</span>
  <span m="4045190">we'll</span> <span m="4045370">talk</span> <span m="4045580">a</span>
  <span m="4045640">little</span> <span m="4045820">bit</span> <span m="4045940">about</span>
  <span m="4046240">the</span> <span m="4046360">statistics</span> <span m="4046930">involved</span>
  <span m="4047380">in</span> <span m="4047920">or</span> <span m="4048370">resulting</span>
  <span m="4048820">from</span> <span m="4048970">the</span> <span m="4049060">positivity</span>
  <span m="4049570">assumption</span> <span m="4050410">and</span> <span m="4052000">things</span>
  <span m="4052180">like</span> <span m="4052300">importance</span> <span m="4052690">weighting,</span>
  <span m="4052930">et</span> <span m="4053080">cetera.</span> <span m="4053740">Did
  I</span> <span m="4053800">say</span> <span m="4054050">tomorrow?</span> <span m="4054310">I</span>
  <span m="4054380">meant</span> <span m="4054520">Thursday.</span></p><p><span m="4058350">So</span>
  <span m="4059310">last</span> <span m="4059640">recap</span> <span m="4060180">on</span>
  <span m="4060390">the</span> <span m="4061080">potential</span> <span m="4061470">outcome</span>
  <span m="4061730">story.</span> <span m="4062490">This</span> <span m="4062700">is</span>
  <span m="4062860">a</span> <span m="4063070">slide--</span> <span m="4063330">I'm</span>
  <span m="4063420">not</span> <span m="4063540">sure</span> <span m="4063750">if</span>
  <span m="4063840">he</span> <span m="4063930">showed</span> <span m="4064200">this</span>
  <span m="4064350">one,</span> <span m="4064500">but</span> <span m="4064590">it's</span>
  <span m="4064680">one</span> <span m="4064980">that</span> <span m="4065070">we</span>
  <span m="4065160">used</span> <span m="4065340">in</span> <span m="4065430">a</span>
  <span m="4065580">lot</span> <span m="4065760">of</span> <span m="4065820">talks.</span>
  <span m="4067470">And</span> <span m="4067750">it,</span> <span m="4068250">again,</span>
  <span m="4068550">just</span> <span m="4068700">serves</span> <span m="4068970">to</span>
  <span m="4069090">illustrate</span> <span m="4069680">the</span> <span m="4069930">idea</span>
  <span m="4070260">of</span> <span m="4070650">a</span> <span m="4070830">one-timestep</span>
  <span m="4071550">decision.</span></p><p><span m="4072000">So</span> <span m="4072750">we</span>
  <span m="4072870">have</span> <span m="4073020">here,</span> <span m="4073170">Anna.</span>
  <span m="4073520">A</span> <span m="4073620">patient</span> <span m="4073890">comes</span>
  <span m="4074130">in.</span> <span m="4074320">She has</span> <span m="4074640">high</span>
  <span m="4076020">blood</span> <span m="4076260">sugar</span> <span m="4077040">and</span>
  <span m="4077160">some</span> <span m="4077340">other</span> <span m="4078090">properties.</span>
  <span m="4079050">And</span> <span m="4079170">we're</span> <span m="4079290">debating</span>
  <span m="4079620">whether</span> <span m="4079830">to</span> <span m="4079950">give</span>
  <span m="4080130">her</span> <span m="4080280">medication</span> <span m="4080880">A</span>
  <span m="4081090">or</span> <span m="4081240">B.</span> <span m="4081870">And</span>
  <span m="4081990">to</span> <span m="4082080">do</span> <span m="4082260">that,</span>
  <span m="4082680">we</span> <span m="4083010">want</span> <span m="4083400">to</span>
  <span m="4083460">figure</span> <span m="4083760">out</span> <span m="4083910">what</span>
  <span m="4084120">would</span> <span m="4084270">be</span> <span m="4084450">her</span>
  <span m="4084570">blood</span> <span m="4084780">sugar</span> <span m="4085080">under</span>
  <span m="4085380">these</span> <span m="4085890">different</span> <span m="4086220">choices</span>
  <span m="4086970">a</span> <span m="4087000">few</span> <span m="4087150">months</span>
  <span m="4087420">down</span> <span m="4087660">the</span> <span m="4087720">line?</span></p><p><span
  m="4089170">So</span> <span m="4089940">I'm</span> <span m="4090210">just</span>
  <span m="4090390">using</span> <span m="4090660">this</span> <span m="4090810">here</span>
  <span m="4091020">to</span> <span m="4091530">introduce</span> <span m="4091950">you</span>
  <span m="4092010">to</span> <span m="4092130">the</span> <span m="4092220">patient,</span>
  <span m="4092550">Anna.</span> <span m="4093240">And</span> <span m="4093330">we're</span>
  <span m="4093480">going</span> <span m="4093570">to</span> <span m="4093660">talk</span>
  <span m="4093810">about</span> <span m="4094050">Anna</span> <span m="4094200">a</span>
  <span m="4094260">little</span> <span m="4094380">bit</span> <span m="4094500">more.</span>
  <span m="4095750">So</span> <span m="4096090">treating</span> <span m="4096479">Anna</span>
  <span m="4096779">once,</span> <span m="4097200">we</span> <span m="4097290">can</span>
  <span m="4097410">represent</span> <span m="4097890">as</span> <span m="4098010">this</span>
  <span m="4098609">causal</span> <span m="4099060">graph</span> <span m="4099899">that</span>
  <span m="4100050">you've</span> <span m="4100200">seen</span> <span m="4101220">a</span>
  <span m="4101279">lot</span> <span m="4101399">of</span> <span m="4101460">times</span>
  <span m="4101760">now.</span> <span m="4102410">We</span> <span m="4102540">had</span>
  <span m="4102689">some</span> <span m="4102870">treatment,</span> <span m="4103319">A,</span>
  <span m="4103710">we</span> <span m="4103830">had</span> <span m="4103920">some</span>
  <span m="4104069">state,</span> <span m="4104340">S,</span> <span m="4104670">and</span>
  <span m="4104760">some</span> <span m="4104910">outcome,</span> <span m="4105300">R.</span>
  <span m="4105870">We</span> <span m="4105960">want</span> <span m="4106109">to</span>
  <span m="4106170">figure</span> <span m="4106410">out</span> <span m="4106529">the</span>
  <span m="4106620">effect</span> <span m="4107069">of</span> <span m="4107399">this</span>
  <span m="4107609">A</span> <span m="4107970">on</span> <span m="4108120">the</span>
  <span m="4108870">outcome,</span> <span m="4109229">R.</span></p><p><span m="4110040">Ignorability</span>
  <span m="4110700">in</span> <span m="4110790">this</span> <span m="4110939">case</span>
  <span m="4111270">just</span> <span m="4111490">says</span> <span m="4111689">that</span>
  <span m="4112170">the</span> <span m="4112319">potential</span> <span m="4112680">outcomes</span>
  <span m="4113729">under</span> <span m="4114300">each</span> <span m="4115410">action,</span>
  <span m="4115910">A,</span> <span m="4116189">is</span> <span m="4116500">conditionally</span>
  <span m="4116880">independent</span> <span m="4117000">of A,</span> <span m="4117210">given</span>
  <span m="4117540">S.</span> <span m="4120930">And</span> <span m="4121380">so</span>
  <span m="4121529">we</span> <span m="4121649">know</span> <span m="4121830">that</span>
  <span m="4121970">ignorability</span> <span m="4125609">and</span> <span m="4125700">overlap</span>
  <span m="4126029">is</span> <span m="4126090">sufficient</span> <span m="4126779">conditions</span>
  <span m="4127380">for</span> <span m="4128160">identification</span> <span m="4128790">of</span>
  <span m="4128850">this</span> <span m="4129000">effect.</span> <span m="4130180">But</span>
  <span m="4130279">what</span> <span m="4130350">happens</span> <span m="4130649">now</span>
  <span m="4130859">if</span> <span m="4130979">we</span> <span m="4131130">add</span>
  <span m="4131430">another</span> <span m="4131760">time</span> <span m="4132000">point?</span>
  <span m="4133370">OK,</span> <span m="4133700">so</span> <span m="4134060">in</span>
  <span m="4134210">this</span> <span m="4134390">case,</span> <span m="4134910">if</span>
  <span m="4134960">I</span> <span m="4135080">have</span> <span m="4135229">no</span>
  <span m="4135439">extra</span> <span m="4135740">arrows</span> <span m="4136130">here--</span>
  <span m="4136340">I</span> <span m="4136460">just</span> <span m="4136640">have</span>
  <span m="4136910">completely</span> <span m="4137330">independent</span> <span m="4137870">time</span>
  <span m="4138140">points--</span> <span m="4138470">ignorability</span> <span m="4139010">clearly</span>
  <span m="4139370">still</span> <span m="4139550">holds.</span> <span m="4141040">There's</span>
  <span m="4141279">no</span> <span m="4141819">links</span> <span m="4142120">going</span>
  <span m="4142330">from</span> <span m="4142510">A</span> <span m="4142840">to</span>
  <span m="4143170">R,</span> <span m="4143319">there's no</span> <span m="4143500">from</span>
  <span m="4143680">S</span> <span m="4144130">to</span> <span m="4144310">R,</span>
  <span m="4144470">et</span> <span m="4144620">cetera.</span> <span m="4145870">So</span>
  <span m="4146010">ignorability</span> <span m="4146529">is</span> <span m="4146590">still</span>
  <span m="4146800">fine.</span></p><p><span m="4155260">If</span> <span m="4155620">Anna's</span>
  <span m="4156220">health</span> <span m="4156490">status</span> <span m="4157689">in</span>
  <span m="4157810">the</span> <span m="4157870">future</span> <span m="4158319">depends</span>
  <span m="4158859">on</span> <span m="4159130">the</span> <span m="4159250">actions</span>
  <span m="4159609">that</span> <span m="4159760">I</span> <span m="4159830">take</span>
  <span m="4160130">now,</span> <span m="4161350">here,</span> <span m="4165900">then</span>
  <span m="4166370">the</span> <span m="4166460">situation</span> <span m="4166850">is</span>
  <span m="4166939">a</span> <span m="4167000">little</span> <span m="4167149">bit</span>
  <span m="4167270">different.</span> <span m="4168060">So</span> <span m="4168080">this</span>
  <span m="4168260">is</span> <span m="4168380">now</span> <span m="4168970">not</span>
  <span m="4169930">in</span> <span m="4170080">the</span> <span m="4170420">completely</span>
  <span m="4170779">independent</span> <span m="4172279">actions</span> <span m="4172640">that</span>
  <span m="4172760">I</span> <span m="4172790">make,</span> <span m="4173210">but</span>
  <span m="4173390">the</span> <span m="4173510">actions</span> <span m="4174290">here</span>
  <span m="4174710">influence</span> <span m="4175160">the</span> <span m="4175580">state</span>
  <span m="4175850">in</span> <span m="4175939">the</span> <span m="4176000">future.</span>
  <span m="4176729">So</span> <span m="4176779">we've</span> <span m="4176930">seen</span>
  <span m="4177140">this.</span> <span m="4178160">This</span> <span m="4178310">is</span>
  <span m="4178370">a</span> <span m="4178430">Markov</span> <span m="4178700">decision</span>
  <span m="4179029">process,</span> <span m="4179330">as</span> <span m="4179420">you've</span>
  <span m="4179510">seen</span> <span m="4179720">before.</span> <span m="4182210">This</span>
  <span m="4182330">is</span> <span m="4182420">very</span> <span m="4182600">likely</span>
  <span m="4182840">in</span> <span m="4182899">practice.</span></p><p><span m="4185240">Also,</span>
  <span m="4185779">if</span> <span m="4186020">Anna,</span> <span m="4186359">for</span>
  <span m="4186470">example,</span> <span m="4186830">is</span> <span m="4186920">diabetic,</span>
  <span m="4187460">as</span> <span m="4187580">we</span> <span m="4187700">saw</span>
  <span m="4187910">in</span> <span m="4188000">the</span> <span m="4188090">example</span>
  <span m="4188479">that</span> <span m="4188569">I</span> <span m="4188630">mentioned,</span>
  <span m="4189620">it's</span> <span m="4189800">likely</span> <span m="4190040">that</span>
  <span m="4190189">she</span> <span m="4190340">will</span> <span m="4190490">remain</span>
  <span m="4190790">so.</span> <span m="4192890">This</span> <span m="4193370">previous</span>
  <span m="4193790">state</span> <span m="4194029">will</span> <span m="4194180">influence</span>
  <span m="4194510">the</span> <span m="4194570">future</span> <span m="4194840">state.</span>
  <span m="4196290">These</span> <span m="4196590">things</span> <span m="4196830">seem</span>
  <span m="4197040">very</span> <span m="4197250">reasonable,</span> <span m="4197730">right?</span>
  <span m="4198630">But</span> <span m="4198750">now</span> <span m="4198960">I'm</span>
  <span m="4199080">trying</span> <span m="4199320">to</span> <span m="4199380">argue</span>
  <span m="4199680">about</span> <span m="4200100">the</span> <span m="4201390">sequential</span>
  <span m="4201840">ignorability</span> <span m="4202320">assumption.</span> <span
  m="4203010">How</span> <span m="4203220">can</span> <span m="4203370">we</span>
  <span m="4203460">break</span> <span m="4203820">that?</span> <span m="4204210">How</span>
  <span m="4204390">can</span> <span m="4204540">we</span> <span m="4204690">break</span>
  <span m="4205170">ignorability</span> <span m="4205800">when</span> <span m="4205920">it</span>
  <span m="4205980">comes</span> <span m="4206220">to</span> <span m="4206310">the</span>
  <span m="4206700">sequential,</span> <span m="4207150">say?</span></p><p><span m="4215110">If</span>
  <span m="4215230">you</span> <span m="4215380">have</span> <span m="4215830">an</span>
  <span m="4216340">action</span> <span m="4216700">here--</span> <span m="4217700">so</span>
  <span m="4217750">the</span> <span m="4217900">outcome</span> <span m="4218350">at</span>
  <span m="4218440">a</span> <span m="4218500">later</span> <span m="4218860">point</span>
  <span m="4219580">depends</span> <span m="4219970">on</span> <span m="4220060">an</span>
  <span m="4220180">earlier</span> <span m="4220570">choice.</span> <span m="4221740">That</span>
  <span m="4221860">might</span> <span m="4222010">certainly</span> <span m="4222310">be</span>
  <span m="4222400">the</span> <span m="4222520">case,</span> <span m="4222790">because</span>
  <span m="4223060">we</span> <span m="4223150">could</span> <span m="4223270">have</span>
  <span m="4223630">a</span> <span m="4223690">delayed</span> <span m="4224050">effect</span>
  <span m="4224380">of</span> <span m="4224440">something.</span> <span m="4225320">So</span>
  <span m="4225430">if</span> <span m="4225550">we</span> <span m="4225640">measure,</span>
  <span m="4226510">say,</span> <span m="4226820">a</span> <span m="4226840">lab</span>
  <span m="4227110">value</span> <span m="4227710">which</span> <span m="4228460">could</span>
  <span m="4228640">be</span> <span m="4228820">in</span> <span m="4229330">the</span>
  <span m="4229450">right</span> <span m="4229690">range</span> <span m="4229960">or</span>
  <span m="4230020">not,</span> <span m="4231220">it</span> <span m="4231550">could</span>
  <span m="4231760">very</span> <span m="4232030">well</span> <span m="4232210">depend</span>
  <span m="4232450">on</span> <span m="4232510">medication</span> <span m="4232960">we</span>
  <span m="4233050">gave</span> <span m="4233260">a</span> <span m="4233290">long</span>
  <span m="4233470">time</span> <span m="4233620">ago.</span> <span m="4236170">And</span>
  <span m="4236260">it's</span> <span m="4236380">also</span> <span m="4236560">likely</span>
  <span m="4236830">that</span> <span m="4236980">the</span> <span m="4237040">reward</span>
  <span m="4237640">could</span> <span m="4237970">depend</span> <span m="4238420">on</span>
  <span m="4238690">a</span> <span m="4238750">state</span> <span m="4239620">which</span>
  <span m="4239830">is</span> <span m="4240520">much</span> <span m="4240880">earlier,</span>
  <span m="4241510">depending</span> <span m="4241840">on</span> <span m="4241930">what</span>
  <span m="4242080">we</span> <span m="4242170">include</span> <span m="4242420">in</span>
  <span m="4242530">that</span> <span m="4242680">state</span> <span m="4242890">variable.</span>
  <span m="4244660">We</span> <span m="4244780">already</span> <span m="4245050">have</span>
  <span m="4245230">an</span> <span m="4245320">example,</span> <span m="4245660">I</span>
  <span m="4245740">think,</span> <span m="4245890">from</span> <span m="4246040">the</span>
  <span m="4246130">audience</span> <span m="4246400">on</span> <span m="4246470">that.</span></p><p><span
  m="4247210">So</span> <span m="4247450">actually,</span> <span m="4247810">ignorability</span>
  <span m="4248530">should</span> <span m="4248740">have</span> <span m="4248830">a</span>
  <span m="4248890">big</span> <span m="4249040">red</span> <span m="4249190">cross</span>
  <span m="4249490">over</span> <span m="4249640">it,</span> <span m="4249730">because</span>
  <span m="4249940">it</span> <span m="4250000">doesn't</span> <span m="4250180">hold</span>
  <span m="4250420">there.</span> <span m="4250910">And</span> <span m="4251020">it's</span>
  <span m="4251110">luckily</span> <span m="4251440">on</span> <span m="4251530">the</span>
  <span m="4251590">next</span> <span m="4251860">slide.</span> <span m="4253580">Because</span>
  <span m="4253830">there</span> <span m="4253920">are</span> <span m="4253960">even</span>
  <span m="4254230">more</span> <span m="4254410">errors</span> <span m="4254790">that</span>
  <span m="4254810">we</span> <span m="4254890">can</span> <span m="4255250">have,</span>
  <span m="4255580">conceivably,</span> <span m="4256090">in</span> <span m="4256180">the</span>
  <span m="4256270">medical</span> <span m="4256570">setting.</span> <span m="4258520">The</span>
  <span m="4258820">example</span> <span m="4259120">that</span> <span m="4259210">we</span>
  <span m="4259300">got</span> <span m="4259420">from</span> <span m="4259570">Pete</span>
  <span m="4259720">before</span> <span m="4259990">was,</span> <span m="4260170">essentially,</span>
  <span m="4260620">that</span> <span m="4260740">if</span> <span m="4260890">we've</span>
  <span m="4261040">tried</span> <span m="4261400">an</span> <span m="4261490">action</span>
  <span m="4261940">previously,</span> <span m="4262450">we</span> <span m="4262570">might</span>
  <span m="4262750">not</span> <span m="4262840">want</span> <span m="4262960">to</span>
  <span m="4263020">try</span> <span m="4263230">it</span> <span m="4263290">again.</span>
  <span m="4264870">Or</span> <span m="4265550">if</span> <span m="4265680">we</span>
  <span m="4265770">knew</span> <span m="4266040">that</span> <span m="4266160">something</span>
  <span m="4266490">worked</span> <span m="4266730">previously,</span> <span m="4267150">we</span>
  <span m="4267270">might</span> <span m="4267510">want</span> <span m="4267690">to</span>
  <span m="4267750">do</span> <span m="4267900">it</span> <span m="4267990">again.</span></p><p><span
  m="4268290">So</span> <span m="4268470">if</span> <span m="4268800">we</span> <span
  m="4268920">had</span> <span m="4269010">a</span> <span m="4269070">good</span>
  <span m="4269220">reward</span> <span m="4269520">here,</span> <span m="4269700">we</span>
  <span m="4269790">might</span> <span m="4269970">want</span> <span m="4270090">to</span>
  <span m="4270450">do</span> <span m="4270690">the</span> <span m="4270780">same</span>
  <span m="4270960">thing</span> <span m="4271110">twice.</span> <span m="4272810">And</span>
  <span m="4273180">this</span> <span m="4273510">arrow</span> <span m="4273840">here</span>
  <span m="4274110">says</span> <span m="4274350">that</span> <span m="4274500">if</span>
  <span m="4275190">we</span> <span m="4275370">know</span> <span m="4275640">that</span>
  <span m="4277110">a</span> <span m="4277200">patient</span> <span m="4277500">had</span>
  <span m="4277650">a</span> <span m="4277710">symptom</span> <span m="4278280">earlier</span>
  <span m="4278670">on,</span> <span m="4278940">we</span> <span m="4279030">might</span>
  <span m="4279240">want</span> <span m="4279390">to</span> <span m="4279600">base</span>
  <span m="4279870">our</span> <span m="4279960">actions</span> <span m="4280320">on</span>
  <span m="4280470">it</span> <span m="4280560">later.</span> <span m="4281190">We've</span>
  <span m="4281290">known</span> <span m="4281520">that</span> <span m="4281620">the</span>
  <span m="4281730">patient</span> <span m="4282150">had</span> <span m="4282930">an</span>
  <span m="4283020">allergic</span> <span m="4283530">reaction</span> <span m="4284040">at</span>
  <span m="4284100">some</span> <span m="4284250">point,</span> <span m="4284530">for</span>
  <span m="4284550">example.</span> <span m="4285010">We</span> <span m="4285030">might</span>
  <span m="4285360">not</span> <span m="4285480">want</span> <span m="4285630">to</span>
  <span m="4285690">use</span> <span m="4285900">that</span> <span m="4285960">medication</span>
  <span m="4286560">at</span> <span m="4286680">a</span> <span m="4286710">later</span>
  <span m="4286920">time.</span></p><p><span m="4288270">AUDIENCE:</span> <span m="4288300">But</span>
  <span m="4288330">you</span> <span m="4288420">can</span> <span m="4288710">always</span>
  <span m="4288990">put</span> <span m="4289170">everything</span> <span m="4289530">in</span>
  <span m="4289600">a</span> <span m="4289650">state.</span></p><p><span m="4290250">FREDRIK
  D. JOHANSSON:</span> <span m="4290460">Exactly.</span> <span m="4292170">So</span>
  <span m="4292260">this</span> <span m="4292440">depends</span> <span m="4292740">on</span>
  <span m="4292830">what</span> <span m="4292950">you</span> <span m="4293010">put</span>
  <span m="4293190">in</span> <span m="4293280">the</span> <span m="4293350">state.</span>
  <span m="4296970">This</span> <span m="4297360">is</span> <span m="4297450">an</span>
  <span m="4297510">example</span> <span m="4297870">where</span> <span m="4298050">I</span>
  <span m="4298150">should</span> <span m="4298620">introduce</span> <span m="4298980">these</span>
  <span m="4299160">arrows</span> <span m="4300150">to</span> <span m="4300300">show</span>
  <span m="4300690">that,</span> <span m="4300900">if</span> <span m="4301080">I</span>
  <span m="4301170">haven't</span> <span m="4301740">got</span> <span m="4302040">that</span>
  <span m="4302220">information</span> <span m="4302760">here,</span> <span m="4303330">then</span>
  <span m="4303510">I</span> <span m="4303660">introduce</span> <span m="4304080">this</span>
  <span m="4304230">dependence.</span> <span m="4306030">So</span> <span m="4306150">if</span>
  <span m="4306540">I</span> <span m="4306600">don't</span> <span m="4306960">have</span>
  <span m="4307290">the</span> <span m="4307470">information</span> <span m="4308040">about</span>
  <span m="4310950">allergic</span> <span m="4311270">reaction</span> <span m="4311590">or</span>
  <span m="4311650">some</span> <span m="4311850">symptom</span> <span m="4312180">before</span>
  <span m="4312410">in</span> <span m="4312870">here,</span> <span m="4314660">then</span>
  <span m="4314790">I</span> <span m="4315060">have</span> <span m="4315210">to</span>
  <span m="4315300">do</span> <span m="4315450">something</span> <span m="4315720">else.</span></p><p><span
  m="4318220">So</span> <span m="4318760">exactly</span> <span m="4319540">that</span>
  <span m="4319870">is</span> <span m="4320020">the</span> <span m="4320080">point.</span>
  <span m="4320400">If</span> <span m="4320500">I</span> <span m="4320590">can</span>
  <span m="4320710">summarize</span> <span m="4321220">history</span> <span m="4321610">in</span>
  <span m="4321700">some</span> <span m="4321940">good</span> <span m="4322120">way--</span>
  <span m="4323410">if</span> <span m="4323560">I</span> <span m="4323750">can</span>
  <span m="4324370">compress</span> <span m="4325000">all</span> <span m="4325210">of</span>
  <span m="4325300">these</span> <span m="4325480">four</span> <span m="4326560">variables</span>
  <span m="4328570">into</span> <span m="4328840">some</span> <span m="4330130">variable</span>
  <span m="4330430">age</span> <span m="4331480">standard</span> <span m="4331720">for</span>
  <span m="4331840">the</span> <span m="4331930">history,</span> <span m="4332450">then</span>
  <span m="4332500">I</span> <span m="4332560">have</span> <span m="4333010">ignorability,</span>
  <span m="4333490">with</span> <span m="4333670">respect</span> <span m="4333970">to</span>
  <span m="4334030">that</span> <span m="4334210">history,</span> <span m="4334540">H.</span>
  <span m="4340090">This</span> <span m="4340690">is</span> <span m="4340780">your</span>
  <span m="4340930">solution</span> <span m="4341410">and</span> <span m="4341620">it</span>
  <span m="4341710">introduces</span> <span m="4342190">a</span> <span m="4342220">new</span>
  <span m="4342370">problem,</span> <span m="4343030">because</span> <span m="4343870">history</span>
  <span m="4344350">is</span> <span m="4344890">usually</span> <span m="4345370">a</span>
  <span m="4345460">really</span> <span m="4345910">large</span> <span m="4346390">thing.</span>
  <span m="4349060">We</span> <span m="4349150">know</span> <span m="4349330">that</span>
  <span m="4349440">history</span> <span m="4349750">grows</span> <span m="4349990">with</span>
  <span m="4350110">time,</span> <span m="4350350">obviously.</span> <span m="4350720">But</span>
  <span m="4350830">usually</span> <span m="4351490">we</span> <span m="4351610">don't</span>
  <span m="4352000">observe</span> <span m="4352330">patients</span> <span m="4352660">for</span>
  <span m="4352780">the</span> <span m="4352870">same</span> <span m="4353110">number</span>
  <span m="4353440">of</span> <span m="4353530">time</span> <span m="4353800">points.</span></p><p><span
  m="4354260">So</span> <span m="4354370">how</span> <span m="4354550">do</span> <span
  m="4354640">we</span> <span m="4355090">represent</span> <span m="4355570">that</span>
  <span m="4356050">for</span> <span m="4356230">a</span> <span m="4356290">program?</span>
  <span m="4356710">How</span> <span m="4356830">do</span> <span m="4356890">we</span>
  <span m="4356950">represent</span> <span m="4357310">that</span> <span m="4357400">to</span>
  <span m="4357520">a</span> <span m="4357550">learning</span> <span m="4357850">algorithm?</span>
  <span m="4358850">That's</span> <span m="4358960">something</span> <span m="4359200">we</span>
  <span m="4359290">have</span> <span m="4359380">to</span> <span m="4359740">deal</span>
  <span m="4359980">with.</span> <span m="4361270">You</span> <span m="4361390">can</span>
  <span m="4361510">pad</span> <span m="4362050">history</span> <span m="4362380">with</span>
  <span m="4362500">0s,</span> <span m="4362910">et</span> <span m="4363070">cetera,</span>
  <span m="4363260">but</span> <span m="4363370">if</span> <span m="4363460">you</span>
  <span m="4363550">keep</span> <span m="4363880">every</span> <span m="4364150">timestep</span>
  <span m="4364600">and</span> <span m="4364690">repeat</span> <span m="4365050">every</span>
  <span m="4365320">variable</span> <span m="4366020">in</span> <span m="4366160">every</span>
  <span m="4366280">timestep,</span> <span m="4366800">you</span> <span m="4366900">get</span>
  <span m="4367000">a</span> <span m="4367100">very</span> <span m="4367180">large</span>
  <span m="4367480">object.</span> <span m="4369070">That</span> <span m="4369230">might</span>
  <span m="4369550">introduce</span> <span m="4370210">statistical</span> <span m="4370720">problems,</span>
  <span m="4371050">because</span> <span m="4371260">now</span> <span m="4371440">you</span>
  <span m="4371530">have</span> <span m="4371650">much</span> <span m="4371830">more</span>
  <span m="4371980">variance</span> <span m="4372340">if</span> <span m="4372400">you</span>
  <span m="4372460">have</span> <span m="4372550">new</span> <span m="4372670">variables,</span>
  <span m="4373090">et</span> <span m="4373260">cetera.</span></p><p><span m="4374900">So</span>
  <span m="4375050">one</span> <span m="4375260">thing</span> <span m="4375410">that</span>
  <span m="4375500">people</span> <span m="4375740">do</span> <span m="4375980">is</span>
  <span m="4376100">that</span> <span m="4376220">they</span> <span m="4377330">look</span>
  <span m="4377690">some</span> <span m="4378050">amount</span> <span m="4378290">of</span>
  <span m="4378380">time</span> <span m="4379070">backwards--</span> <span m="4379590">so</span>
  <span m="4379790">instead</span> <span m="4380030">of</span> <span m="4380090">just</span>
  <span m="4380300">looking</span> <span m="4380480">at</span> <span m="4380540">one</span>
  <span m="4380780">timestep</span> <span m="4381200">back,</span> <span m="4381470">you</span>
  <span m="4381550">now</span> <span m="4381750">look</span> <span m="4381950">at</span>
  <span m="4382020">a</span> <span m="4382070">length</span> <span m="4382340">k</span>
  <span m="4382670">window.</span> <span m="4383330">And</span> <span m="4383420">your</span>
  <span m="4383540">state</span> <span m="4383900">essentially</span> <span m="4384410">grows</span>
  <span m="4384770">by</span> <span m="4386150">a</span> <span m="4386180">factor,</span>
  <span m="4386480">k.</span> <span m="4388120">And</span> <span m="4388490">another</span>
  <span m="4388910">alternative</span> <span m="4389360">is</span> <span m="4389480">to</span>
  <span m="4389570">try</span> <span m="4389750">and</span> <span m="4389840">learn</span>
  <span m="4390050">a</span> <span m="4390110">summary</span> <span m="4390530">function.</span>
  <span m="4391100">Learn</span> <span m="4391400">some</span> <span m="4391700">function</span>
  <span m="4392090">that</span> <span m="4392210">is</span> <span m="4392390">relevant</span>
  <span m="4392750">for</span> <span m="4392900">predicting</span> <span m="4393290">the</span>
  <span m="4393410">outcome</span> <span m="4394130">that</span> <span m="4394280">takes</span>
  <span m="4394610">all</span> <span m="4394760">of</span> <span m="4394850">the</span>
  <span m="4394940">history</span> <span m="4395240">into</span> <span m="4395420">account,</span>
  <span m="4396050">but</span> <span m="4396290">has</span> <span m="4396470">a</span>
  <span m="4396530">smaller</span> <span m="4397370">representation</span> <span m="4398060">than</span>
  <span m="4398210">just</span> <span m="4398750">t</span> <span m="4398990">times</span>
  <span m="4399980">the</span> <span m="4400160">variables</span> <span m="4400490">that</span>
  <span m="4400590">you</span> <span m="4400670">have.</span></p><p><span m="4402250">But</span>
  <span m="4402400">this</span> <span m="4402520">is</span> <span m="4402580">something</span>
  <span m="4402880">that</span> <span m="4403120">needs</span> <span m="4404350">to</span>
  <span m="4404530">happen,</span> <span m="4404980">usually.</span> <span m="4409180">Most</span>
  <span m="4409570">health care</span> <span m="4409830">data,</span> <span m="4410020">in</span>
  <span m="4410140">practice--</span> <span m="4410570">you</span> <span m="4410670">have</span>
  <span m="4410740">to</span> <span m="4410830">make</span> <span m="4411040">choices</span>
  <span m="4411370">about</span> <span m="4411580">this.</span> <span m="4411790">I</span>
  <span m="4411880">just</span> <span m="4412030">want</span> <span m="4412180">to</span>
  <span m="4412240">stress</span> <span m="4412570">that</span> <span m="4412660">that's</span>
  <span m="4412810">something</span> <span m="4413350">you</span> <span m="4413530">really</span>
  <span m="4413740">can't</span> <span m="4413950">avoid.</span></p><p><span m="4418300">The</span>
  <span m="4418390">last</span> <span m="4418570">point</span> <span m="4418720">I</span>
  <span m="4418750">want</span> <span m="4418870">to</span> <span m="4418930">make</span>
  <span m="4419110">is</span> <span m="4419260">that</span> <span m="4419530">unobserved</span>
  <span m="4419920">confounding</span> <span m="4420460">is</span> <span m="4420610">also</span>
  <span m="4421360">a</span> <span m="4421390">problem</span> <span m="4422320">that</span>
  <span m="4422530">is</span> <span m="4423310">not</span> <span m="4423640">avoidable</span>
  <span m="4424210">just</span> <span m="4424480">due</span> <span m="4424690">to</span>
  <span m="4424900">summarizing</span> <span m="4425350">history.</span> <span m="4426850">We</span>
  <span m="4427030">can</span> <span m="4427210">introduce</span> <span m="4427780">new</span>
  <span m="4428230">confounding.</span> <span m="4428890">That</span> <span m="4429040">is</span>
  <span m="4429160">a</span> <span m="4429190">problem,</span> <span m="4429520">if</span>
  <span m="4429670">we</span> <span m="4429760">don't</span> <span m="4430150">summarize</span>
  <span m="4430480">history</span> <span m="4430780">well.</span> <span m="4431230">But</span>
  <span m="4431350">we</span> <span m="4431410">can</span> <span m="4431530">also</span>
  <span m="4431710">have</span> <span m="4431800">unobserved</span> <span m="4432250">confounders,</span>
  <span m="4433480">just</span> <span m="4433720">like</span> <span m="4433810">we</span>
  <span m="4433900">can</span> <span m="4434100">in</span> <span m="4434200">the</span>
  <span m="4434290">one-step</span> <span m="4434530">setting.</span></p><p><span
  m="4438220">One</span> <span m="4438640">example</span> <span m="4439090">is</span>
  <span m="4439300">if</span> <span m="4439450">we</span> <span m="4439570">have</span>
  <span m="4439690">an</span> <span m="4439780">unobserved</span> <span m="4440080">confounded</span>
  <span m="4441460">in</span> <span m="4441730">the</span> <span m="4441820">same</span>
  <span m="4442090">way</span> <span m="4442330">as</span> <span m="4442450">we</span>
  <span m="4442540">did</span> <span m="4442660">before.</span> <span m="4443390">It</span>
  <span m="4443830">impacts</span> <span m="4444280">both</span> <span m="4446470">the</span>
  <span m="4446860">action</span> <span m="4447130">at</span> <span m="4447460">time</span>
  <span m="4447820">1</span> <span m="4448300">and</span> <span m="4448510">the</span>
  <span m="4448660">reward</span> <span m="4448870">at</span> <span m="4448930">time</span>
  <span m="4449190">1.</span> <span m="4449590">But</span> <span m="4449740">of</span>
  <span m="4449800">course,</span> <span m="4450010">now</span> <span m="4450190">we're</span>
  <span m="4450280">in</span> <span m="4450350">the</span> <span m="4450430">sequential</span>
  <span m="4450850">setting.</span> <span m="4451150">The</span> <span m="4451240">confounding</span>
  <span m="4451660">structure</span> <span m="4451960">could</span> <span m="4452110">be</span>
  <span m="4452200">much</span> <span m="4452410">more</span> <span m="4452530">complicated.</span></p><p><span
  m="4453340">We</span> <span m="4453460">could</span> <span m="4453580">have</span>
  <span m="4454330">a</span> <span m="4454780">confounder</span> <span m="4455260">that</span>
  <span m="4455440">influences</span> <span m="4455950">an</span> <span m="4456040">early</span>
  <span m="4456520">action</span> <span m="4457000">and</span> <span m="4457090">a</span>
  <span m="4457150">late</span> <span m="4457960">reward.</span> <span m="4458740">So</span>
  <span m="4458830">it</span> <span m="4458920">might</span> <span m="4459070">be</span>
  <span m="4459190">a</span> <span m="4459220">little</span> <span m="4459400">harder</span>
  <span m="4459730">for</span> <span m="4459850">us</span> <span m="4459940">to</span>
  <span m="4460000">characterize</span> <span m="4460840">what</span> <span m="4461050">is</span>
  <span m="4461140">the</span> <span m="4461200">set</span> <span m="4461410">of</span>
  <span m="4462310">potential</span> <span m="4462640">confounders?</span> <span m="4464430">So
  I</span> <span m="4464540">just</span> <span m="4464720">wanted</span> <span m="4464930">to</span>
  <span m="4464990">point</span> <span m="4465200">that</span> <span m="4465290">out</span>
  <span m="4465500">and</span> <span m="4465890">to</span> <span m="4466220">reinforce</span>
  <span m="4466850">that</span> <span m="4466940">this</span> <span m="4467090">is</span>
  <span m="4467210">only</span> <span m="4467510">harder</span> <span m="4467870">than</span>
  <span m="4468190">the one-step</span> <span m="4468460">setting.</span></p><p><span
  m="4469520">So</span> <span m="4469730">we're</span> <span m="4469880">wrapping</span>
  <span m="4470210">up</span> <span m="4470360">now.</span> <span m="4470900">I</span>
  <span m="4471410">just</span> <span m="4471560">want</span> <span m="4471710">to</span>
  <span m="4471920">end</span> <span m="4472280">on</span> <span m="4474230">a</span>
  <span m="4474290">point</span> <span m="4474590">about</span> <span m="4475070">the</span>
  <span m="4476630">games</span> <span m="4477050">that</span> <span m="4477140">we</span>
  <span m="4477230">looked</span> <span m="4477410">at</span> <span m="4477470">before.</span>
  <span m="4478820">One</span> <span m="4479060">of</span> <span m="4479120">the</span>
  <span m="4479240">big</span> <span m="4479510">reasons</span> <span m="4480110">that</span>
  <span m="4482150">these</span> <span m="4482660">algorithms</span> <span m="4483050">were</span>
  <span m="4483170">so</span> <span m="4483440">successful</span> <span m="4483980">in</span>
  <span m="4484070">playing</span> <span m="4484310">games</span> <span m="4485180">was</span>
  <span m="4485390">that</span> <span m="4485480">we</span> <span m="4485630">have</span>
  <span m="4486290">full</span> <span m="4486680">observability</span> <span m="4487430">in</span>
  <span m="4487580">these</span> <span m="4487700">settings.</span> <span m="4488030">We
  know</span> <span m="4488150">everything</span> <span m="4489410">from</span> <span
  m="4492170">the</span> <span m="4492380">game</span> <span m="4492680">board</span>
  <span m="4492950">itself--</span> <span m="4493520">when</span> <span m="4493640">it</span>
  <span m="4493700">comes</span> <span m="4493940">to</span> <span m="4494060">Go,</span>
  <span m="4494420">at</span> <span m="4494510">least.</span> <span m="4495470">We</span>
  <span m="4495560">can</span> <span m="4495680">debate</span> <span m="4495900">that</span>
  <span m="4496280">when</span> <span m="4496400">it</span> <span m="4496460">comes</span>
  <span m="4496610">to</span> <span m="4496670">the</span> <span m="4496730">video</span>
  <span m="4496930">games.</span></p><p><span m="4497650">But</span> <span m="4499040">in</span>
  <span m="4499490">Go,</span> <span m="4499850">we</span> <span m="4500000">have</span>
  <span m="4500270">complete</span> <span m="4500660">observability</span> <span m="4501230">of</span>
  <span m="4501320">the</span> <span m="4501380">board.</span> <span m="4501650">Everything</span>
  <span m="4502130">we</span> <span m="4502250">need</span> <span m="4502490">to</span>
  <span m="4502610">know</span> <span m="4503030">for</span> <span m="4503390">an</span>
  <span m="4503540">optimal</span> <span m="4503900">decision</span> <span m="4504320">is</span>
  <span m="4504500">there</span> <span m="4505000">at</span> <span m="4505120">any</span>
  <span m="4505370">time</span> <span m="4505640">point.</span> <span m="4509900">Not</span>
  <span m="4510050">only</span> <span m="4510320">can</span> <span m="4510530">we</span>
  <span m="4510620">observe</span> <span m="4510950">it</span> <span m="4511010">through</span>
  <span m="4511160">the</span> <span m="4511250">history,</span> <span m="4511670">but</span>
  <span m="4511820">in</span> <span m="4511950">the</span> <span m="4512000">case</span>
  <span m="4512270">of</span> <span m="4512360">Go,</span> <span m="4513260">you</span>
  <span m="4513440">don't</span> <span m="4513680">even</span> <span m="4513890">need</span>
  <span m="4514070">to</span> <span m="4514160">look</span> <span m="4514370">at</span>
  <span m="4514430">history.</span> <span m="4514980">We</span> <span m="4515000">certainly</span>
  <span m="4515390">have</span> <span m="4515540">Markov</span> <span m="4516530">dynamics</span>
  <span m="4516920">with</span> <span m="4517100">respect</span> <span m="4517430">to</span>
  <span m="4517550">the</span> <span m="4517640">board</span> <span m="4517880">itself.</span></p><p><span
  m="4518810">You</span> <span m="4518900">don't</span> <span m="4519170">ever</span>
  <span m="4519410">have</span> <span m="4519530">to</span> <span m="4519650">remember</span>
  <span m="4520070">what</span> <span m="4520630">was</span> <span m="4520770">a</span>
  <span m="4520860">move</span> <span m="4521210">earlier</span> <span m="4521570">on,</span>
  <span m="4522560">unless</span> <span m="4522770">you</span> <span m="4522830">want</span>
  <span m="4522980">to</span> <span m="4523070">read</span> <span m="4523280">into</span>
  <span m="4523490">your</span> <span m="4523580">opponent,</span> <span m="4523970">I</span>
  <span m="4524030">suppose.</span> <span m="4524390">But</span> <span m="4524510">that's</span>
  <span m="4525200">a</span> <span m="4525260">game</span> <span m="4525470">theoretic</span>
  <span m="4527160">notion</span> <span m="4527420">we're</span> <span m="4527510">not</span>
  <span m="4527600">going</span> <span m="4527720">to</span> <span m="4527780">get</span>
  <span m="4527870">into</span> <span m="4528020">here.</span> <span m="4529890">But</span>
  <span m="4530060">more</span> <span m="4530300">importantly,</span> <span m="4531360">we</span>
  <span m="4531410">can</span> <span m="4531740">explore</span> <span m="4532880">the</span>
  <span m="4532970">dynamics</span> <span m="4533450">of</span> <span m="4533510">these</span>
  <span m="4533630">systems</span> <span m="4534290">almost</span> <span m="4534590">limitlessly,</span>
  <span m="4535190">just</span> <span m="4535460">by</span> <span m="4536480">simulation</span>
  <span m="4537140">and</span> <span m="4537230">self-play.</span> <span m="4538040">And</span>
  <span m="4538130">that's</span> <span m="4538340">true</span> <span m="4538910">regardless</span>
  <span m="4539330">if</span> <span m="4539420">you</span> <span m="4539540">have</span>
  <span m="4539670">full</span> <span m="4539980">observability</span> <span m="4540740">or</span>
  <span m="4540860">not--</span> <span m="4541080">like</span> <span m="4541230">in</span>
  <span m="4541310">StarCraft,</span> <span m="4541730">you</span> <span m="4541790">might</span>
  <span m="4541940">not</span> <span m="4542090">have</span> <span m="4542210">full</span>
  <span m="4542390">observability.</span> <span m="4543170">But</span> <span m="4543320">you</span>
  <span m="4543440">can</span> <span m="4543680">try</span> <span m="4544010">your</span>
  <span m="4544130">things</span> <span m="4544400">out</span> <span m="4545120">endlessly.</span></p><p><span
  m="4546780">And</span> <span m="4547470">contrast</span> <span m="4547860">that</span>
  <span m="4547950">with</span> <span m="4548070">having,</span> <span m="4548580">I</span>
  <span m="4548670">don't</span> <span m="4548790">know,</span> <span m="4549390">700</span>
  <span m="4550050">patients</span> <span m="4550500">with</span> <span m="4550920">rheumatoid</span>
  <span m="4551340">arthritis</span> <span m="4552390">or</span> <span m="4552510">something</span>
  <span m="4552750">like</span> <span m="4552870">that.</span> <span m="4553420">Those</span>
  <span m="4553560">are</span> <span m="4553650">the</span> <span m="4553740">samples</span>
  <span m="4554040">you</span> <span m="4554110">have.</span> <span m="4556100">You're</span>
  <span m="4556400">not</span> <span m="4556550">going</span> <span m="4556630">to</span>
  <span m="4556730">get</span> <span m="4556820">new</span> <span m="4556970">ones.</span>
  <span m="4559270">So</span> <span m="4559570">that</span> <span m="4559830">is</span>
  <span m="4560110">an</span> <span m="4560230">amazing</span> <span m="4561130">obstacle</span>
  <span m="4561790">for</span> <span m="4562000">us</span> <span m="4562150">to</span>
  <span m="4562270">overcome</span> <span m="4562690">if</span> <span m="4562810">we</span>
  <span m="4562930">want</span> <span m="4563080">to</span> <span m="4563170">do</span>
  <span m="4563320">this</span> <span m="4563470">in</span> <span m="4563560">a</span>
  <span m="4563620">good</span> <span m="4563770">way.</span></p><p><span m="4564780">The</span>
  <span m="4564850">current</span> <span m="4565120">algorithms</span> <span m="4565810">are</span>
  <span m="4566560">really</span> <span m="4567640">inefficient</span> <span m="4568420">with</span>
  <span m="4568570">the</span> <span m="4568630">data</span> <span m="4568990">that
  they</span> <span m="4569110">use.</span> <span m="4569980">And</span> <span m="4570100">that's</span>
  <span m="4570280">why</span> <span m="4571990">this</span> <span m="4572500">limitless</span>
  <span m="4573040">exploration</span> <span m="4573490">or</span> <span m="4573580">simulation</span>
  <span m="4574150">has</span> <span m="4575620">been</span> <span m="4575860">so</span>
  <span m="4576070">important</span> <span m="4577150">for</span> <span m="4577300">these</span>
  <span m="4577480">games.</span> <span m="4577720">And</span> <span m="4577810">that's</span>
  <span m="4577990">also</span> <span m="4578200">why</span> <span m="4578410">the</span>
  <span m="4578710">games</span> <span m="4579190">are</span> <span m="4579310">the</span>
  <span m="4579550">success</span> <span m="4579850">stories</span> <span m="4580150">of</span>
  <span m="4580240">this.</span></p><p><span m="4581716">A</span> <span m="4582140">last</span>
  <span m="4582380">point</span> <span m="4582620">is</span> <span m="4582740">that</span>
  <span m="4583040">typically</span> <span m="4583460">for</span> <span m="4583610">these</span>
  <span m="4584360">settings</span> <span m="4584690">that</span> <span m="4584780">I</span>
  <span m="4584840">put</span> <span m="4585230">here,</span> <span m="4586280">we</span>
  <span m="4586400">have</span> <span m="4586520">no</span> <span m="4586670">noise,</span>
  <span m="4587000">essentially.</span> <span m="4588390">We</span> <span m="4588620">get</span>
  <span m="4588800">perfect</span> <span m="4589220">observations</span> <span m="4589730">of</span>
  <span m="4589820">actions</span> <span m="4590870">and</span> <span m="4591140">states</span>
  <span m="4591650">and</span> <span m="4591860">outcomes</span> <span m="4592250">and</span>
  <span m="4592340">everything</span> <span m="4592610">like</span> <span m="4592760">that.</span>
  <span m="4593370">And</span> <span m="4593470">that's</span> <span m="4593540">really</span>
  <span m="4593810">true</span> <span m="4593990">in</span> <span m="4594080">any</span>
  <span m="4594260">real-world</span> <span m="4594680">application.</span></p><p><span
  m="4596160">All</span> <span m="4596260">right.</span> <span m="4596510">I'm</span>
  <span m="4596630">going</span> <span m="4596720">to</span> <span m="4596810">wrap</span>
  <span m="4597020">up.</span> <span m="4597590">Tomorrow--</span> <span m="4599100">nope,</span>
  <span m="4600650">Thursday,</span> <span m="4602540">David</span> <span m="4602870">is</span>
  <span m="4602960">going</span> <span m="4603070">to</span> <span m="4603200">talk</span>
  <span m="4603470">about</span> <span m="4603920">more</span> <span m="4604250">explicitly</span>
  <span m="4605690">if</span> <span m="4605840">we</span> <span m="4605930">want</span>
  <span m="4606110">to</span> <span m="4606170">do</span> <span m="4606350">this</span>
  <span m="4606530">properly</span> <span m="4607040">in</span> <span m="4607180">health</span>
  <span m="4607520">care,</span> <span m="4607720">what's</span> <span m="4607820">going
  to</span> <span m="4607940">happen?</span> <span m="4608230">We're</span> <span
  m="4608300">going</span> <span m="4608360">to</span> <span m="4608420">have</span>
  <span m="4608540">a</span> <span m="4608570">great</span> <span m="4608780">discussion,</span>
  <span m="4609360">I'm</span> <span m="4609380">sure,</span> <span m="4610100">as</span>
  <span m="4610220">well.</span> <span m="4610760">So</span> <span m="4612200">don't</span>
  <span m="4612380">mind</span> <span m="4612530">the</span> <span m="4612620">slide.</span>
  <span m="4613190">It's</span> <span m="4613370">Thursday.</span> <span m="4613930">All</span>
  <span m="4614000">right.</span> <span m="4614210">Thanks</span> <span m="4614420">a</span>
  <span m="4614450">lot.</span></p><p><span m="4615350">[APPLAUSE]</span></p><p>&nbsp;</p>
type: course
uid: a36d0da4a9b40aa41d0825258394995e

---
None