---
about_this_resource_text: "<p>In the first half, Prof. Sontag discusses how to evaluate\
  \ different policies in causal inference and how it is related to reinforcement\
  \ learning. In the second half, Dr. Barbra Dickerman talks about evaluating dynamic\
  \ treatment strategies.</p>\r\n<p>Speakers:&nbsp;David Sontag, Barbra Dickerman</p>\r\
  \n            <p><a href=\"./resolveuid/9eac32a56066df6eaa3d20329a52c11d\">Lecture\
  \ 17: Evaluating Dynamic Treatment Strategies slides (PDF)</a></p>\r\n"
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: zdotUAxiPGM
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: Video-YouTube-Stream
  type: Video
  uid: 68c05b89956e557707f4d4c1a4cef63b
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/zdotUAxiPGM/default.jpg
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 4cfd33371b11f9d9c9e9406732e9206a
- id: 3Play-3PlayYouTubeid-MP4
  media_location: zdotUAxiPGM
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: c2b55d57c1337ee72fda7aca4307538c
- id: zdotUAxiPGM.srt
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-17-reinforcement-learning-part-2/zdotUAxiPGM.srt
  title: 3play caption file
  type: null
  uid: 2519c2ee2a46c0bc16e565f10d1b94f8
- id: zdotUAxiPGM.pdf
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-17-reinforcement-learning-part-2/zdotUAxiPGM.pdf
  title: 3play pdf file
  type: null
  uid: e43b75d9952cd9101b62e87d6d2fe9b9
- id: Caption-3Play YouTube id-SRT
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: a85bd6d398d540b44ad5b8924a21380a
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 3de32ecd420e1e1d552c3af331a3652e
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec17_300k.mp4
  parent_uid: 6173239e857ad3f825f77bdca48adbaf
  title: Video-Internet Archive-MP4
  type: Video
  uid: e3407b2b3a965c881cd4bef9124e4b3b
inline_embed_id: 263653lecture17reinforcementlearningpart284463829
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-17-reinforcement-learning-part-2
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-17-reinforcement-learning-part-2
template_type: Tabbed
title: 'Lecture 17: Reinforcement Learning, Part 2'
transcript: <p><span m="15020">DAVID SONTAG:</span> <span m="15070">A</span> <span
  m="15120">three-part</span> <span m="15750">lecture</span> <span m="16050">today,</span>
  <span m="16470">and I'm</span> <span m="16720">still</span> <span m="16950">continuing</span>
  <span m="17310">on</span> <span m="17400">the</span> <span m="17460">theme</span>
  <span m="17760">of</span> <span m="17880">reinforcement</span> <span m="18330">learning.</span>
  <span m="20160">Part</span> <span m="20400">one,</span> <span m="21120">I'm</span>
  <span m="21270">going</span> <span m="21450">to</span> <span m="21630">be</span>
  <span m="21750">speaking,</span> <span m="22380">and</span> <span m="22800">I'll</span>
  <span m="23010">be</span> <span m="23160">following</span> <span m="23610">up</span>
  <span m="23880">on</span> <span m="24600">last</span> <span m="25020">week's</span>
  <span m="25860">discussion</span> <span m="26400">about</span> <span m="26550">causal</span>
  <span m="26820">inference</span> <span m="27240">and</span> <span m="27360">Tuesday's</span>
  <span m="27750">discussion</span> <span m="28170">on</span> <span m="28440">reinforcement</span>
  <span m="28950">learning.</span> <span m="29820">And</span> <span m="29910">I'll</span>
  <span m="30060">be</span> <span m="30150">going</span> <span m="30390">into</span>
  <span m="32600">sort</span> <span m="32780">of</span> <span m="33210">one</span>
  <span m="33600">more</span> <span m="33810">subtlety</span> <span m="34680">that</span>
  <span m="35160">arises</span> <span m="35700">there</span> <span m="36180">and</span>
  <span m="36330">where</span> <span m="36750">we</span> <span m="36900">can</span>
  <span m="37350">develop</span> <span m="37680">some</span> <span m="37860">nice</span>
  <span m="38100">mathematical</span> <span m="38700">methods</span> <span m="39090">to</span>
  <span m="39180">help</span> <span m="39390">with.</span></p><p><span m="40650">And</span>
  <span m="40800">then</span> <span m="41670">I'm</span> <span m="41730">going</span>
  <span m="41850">to</span> <span m="41910">turn</span> <span m="42090">over</span>
  <span m="42510">the</span> <span m="42780">show</span> <span m="43140">to</span>
  <span m="44760">Barbra,</span> <span m="45260">who I'll</span> <span m="45450">formally</span>
  <span m="45810">introduce</span> <span m="46200">when</span> <span m="46350">the</span>
  <span m="46410">time</span> <span m="46680">comes.</span> <span m="47550">And</span>
  <span m="47790">she's</span> <span m="48000">going</span> <span m="48270">to</span>
  <span m="48630">both</span> <span m="48990">talk</span> <span m="49350">about</span>
  <span m="50100">some</span> <span m="50310">of</span> <span m="50400">her</span>
  <span m="50550">work</span> <span m="51120">on</span> <span m="51660">developing</span>
  <span m="53490">and</span> <span m="53610">evaluating</span> <span m="54750">dynamic</span>
  <span m="55140">treatment</span> <span m="55410">regimes,</span> <span m="56520">and</span>
  <span m="56970">then she will</span> <span m="57340">lead</span> <span m="57450">a</span>
  <span m="57480">discussion</span> <span m="58350">on</span> <span m="58650">the</span>
  <span m="59550">sepsis</span> <span m="60030">paper,</span> <span m="60390">which</span>
  <span m="60540">was</span> <span m="60700">required</span> <span m="61080">reading</span>
  <span m="61350">from</span> <span m="61530">today's</span> <span m="61800">class.</span>
  <span m="62650">So</span> <span m="62850">those</span> <span m="63030">are</span>
  <span m="63090">the</span> <span m="63180">three</span> <span m="63420">parts of</span>
  <span m="63700">today's</span> <span m="64800">lecture.</span></p><p><span m="67920">So</span>
  <span m="68000">I</span> <span m="68040">want</span> <span m="68150">you</span>
  <span m="68210">to</span> <span m="68420">return</span> <span m="68900">back,</span>
  <span m="69680">put</span> <span m="70490">yourself</span> <span m="70850">back</span>
  <span m="71060">in</span> <span m="71150">the</span> <span m="71210">mindset</span>
  <span m="71660">of</span> <span m="71720">Tuesday's</span> <span m="72110">lecture</span>
  <span m="72500">where</span> <span m="72650">we</span> <span m="72740">talked</span>
  <span m="72890">about</span> <span m="73010">reinforcement</span> <span m="73550">learning.</span>
  <span m="74510">Now,</span> <span m="74580">remember</span> <span m="74960">that</span>
  <span m="75230">the</span> <span m="75320">goal</span> <span m="75560">of</span>
  <span m="75650">reinforcement</span> <span m="76160">learning</span> <span m="76490">was</span>
  <span m="76610">to</span> <span m="76700">optimize</span> <span m="77270">some</span>
  <span m="77580">reward.</span></p><p><span m="84930">Specifically,</span> <span
  m="88610">our</span> <span m="88730">goal</span> <span m="89090">is</span> <span
  m="89210">to</span> <span m="89300">find</span> <span m="89660">some</span> <span
  m="90050">policy,</span> <span m="90800">which</span> <span m="90920">I</span> <span
  m="90980">can</span> <span m="91120">note</span> <span m="91340">as</span> <span
  m="91490">pi</span> <span m="91760">star,</span> <span m="93500">which</span> <span
  m="95510">is</span> <span m="95780">the</span> <span m="96560">arg</span> <span
  m="96910">max</span> <span m="98890">over</span> <span m="99340">all</span> <span
  m="99610">possible</span> <span m="100150">policies</span> <span m="100870">pi</span>
  <span m="103140">of</span> <span m="103890">v</span> <span m="104460">of</span>
  <span m="104640">pi,</span> <span m="105240">where</span> <span m="105420">just</span>
  <span m="105580">to</span> <span m="105630">remind</span> <span m="106020">you,
  v</span> <span m="106480">of</span> <span m="106620">pi</span> <span m="106950">is</span>
  <span m="107130">the</span> <span m="107340">value</span> <span m="108030">of</span>
  <span m="108150">the</span> <span m="108240">policy</span> <span m="108660">pi.</span>
  <span m="109490">Formally,</span> <span m="110100">it's</span> <span m="112170">defined</span>
  <span m="112680">as the</span> <span m="113140">expectation</span> <span m="116370">of</span>
  <span m="116700">the</span> <span m="116820">sum</span> <span m="117930">of</span>
  <span m="118110">the</span> <span m="118230">rewards</span> <span m="118800">across</span>
  <span m="119160">time.</span></p><p><span m="122060">So</span> <span m="122480">the</span>
  <span m="122630">reason</span> <span m="122900">why</span> <span m="122970">I'm</span>
  <span m="123050">calling</span> <span m="123290">this</span> <span m="123410">an</span>
  <span m="123500">expectation</span> <span m="123785">with</span> <span m="124070">like</span>
  <span m="124130">the</span> <span m="124340">pi</span> <span m="125270">is</span>
  <span m="125450">because</span> <span m="126090">there's</span> <span m="126540">stochasticity</span>
  <span m="127460">both</span> <span m="127850">in</span> <span m="128000">the</span>
  <span m="128090">environment,</span> <span m="129259">and</span> <span m="129470">possibly</span>
  <span m="129919">pi</span> <span m="130340">is</span> <span m="130639">going</span>
  <span m="130820">to</span> <span m="130910">be</span> <span m="131000">a</span>
  <span m="131030">stochastic</span> <span m="131480">policy.</span> <span m="132740">And</span>
  <span m="132980">this</span> <span m="133220">is</span> <span m="133310">summing</span>
  <span m="133730">over</span> <span m="133970">the</span> <span m="134090">time</span>
  <span m="134510">steps,</span> <span m="134960">because</span> <span m="135140">this</span>
  <span m="135950">is</span> <span m="136070">not</span> <span m="136280">just</span>
  <span m="136490">a</span> <span m="136520">single</span> <span m="137350">time</span>
  <span m="137630">step</span> <span m="138080">problem.</span></p><p><span m="138500">But</span>
  <span m="138860">we're</span> <span m="139010">going</span> <span m="139190">to</span>
  <span m="139280">be</span> <span m="139370">considering</span> <span m="139790">interventions</span>
  <span m="140330">across</span> <span m="140780">time</span> <span m="141680">of</span>
  <span m="141860">the</span> <span m="141950">reward</span> <span m="142460">at</span>
  <span m="142520">each</span> <span m="142700">point</span> <span m="142940">in</span>
  <span m="143030">time.</span> <span m="143780">And</span> <span m="143870">that</span>
  <span m="143930">reward</span> <span m="144200">function</span> <span m="144560">could</span>
  <span m="144800">either</span> <span m="145010">be</span> <span m="145190">at</span>
  <span m="145280">each</span> <span m="145400">point</span> <span m="145550">in</span>
  <span m="145610">time</span> <span m="145910">or</span> <span m="146060">you</span>
  <span m="146150">might</span> <span m="146300">imagine</span> <span m="146570">that</span>
  <span m="146690">this</span> <span m="146840">is</span> <span m="146900">0</span>
  <span m="147380">for</span> <span m="147500">all</span> <span m="147620">time</span>
  <span m="147860">steps,</span> <span m="148230">except</span> <span m="148340">for</span>
  <span m="148430">the</span> <span m="148520">last</span> <span m="148760">time</span>
  <span m="149030">step.</span></p><p><span m="152020">So</span> <span m="152460">the</span>
  <span m="152550">first</span> <span m="152850">question</span> <span m="153150">I</span>
  <span m="153210">want</span> <span m="153390">us to</span> <span m="153480">think</span>
  <span m="153690">about</span> <span m="154020">is,</span> <span m="154750">well,</span>
  <span m="155080">what</span> <span m="155340">are</span> <span m="155430">the</span>
  <span m="155520">implications</span> <span m="156480">of</span> <span m="156810">this</span>
  <span m="157440">as</span> <span m="157890">a</span> <span m="158100">learning</span>
  <span m="158580">paradigm?</span> <span m="160560">If</span> <span m="160680">we</span>
  <span m="160770">look</span> <span m="160950">what's</span> <span m="161100">going</span>
  <span m="161280">on</span> <span m="161400">over</span> <span m="161550">here,</span>
  <span m="161910">hidden</span> <span m="162330">in</span> <span m="162450">my</span>
  <span m="162600">story</span> <span m="163140">is</span> <span m="163260">also</span>
  <span m="163560">an</span> <span m="163620">expectation</span> <span m="164190">over</span>
  <span m="164520">x,</span> <span m="165090">the</span> <span m="167100">patient,</span>
  <span m="167610">for</span> <span m="167760">example,</span> <span m="168360">or</span>
  <span m="168630">the</span> <span m="168810">initial</span> <span m="169140">state.</span>
  <span m="171100">And</span> <span m="171180">so</span> <span m="171270">this</span>
  <span m="171450">intuitively</span> <span m="171725">is</span> <span m="172000">saying,</span>
  <span m="172320">let's</span> <span m="172440">try</span> <span m="172560">to</span>
  <span m="172650">find</span> <span m="172860">a</span> <span m="172920">policy</span>
  <span m="173760">that</span> <span m="173970">has</span> <span m="174660">high</span>
  <span m="175770">expected</span> <span m="176730">reward,</span> <span m="177480">average</span>
  <span m="178050">[INAUDIBLE]</span> <span m="178590">over</span> <span m="178875">all</span>
  <span m="179160">patients.</span></p><p><span m="181370">And</span> <span m="181490">I</span>
  <span m="181550">just</span> <span m="181670">want</span> <span m="182480">you</span>
  <span m="182600">to</span> <span m="182660">think</span> <span m="182930">about</span>
  <span m="183200">whether</span> <span m="183440">that</span> <span m="183620">is</span>
  <span m="183770">indeed</span> <span m="184160">the</span> <span m="184250">right</span>
  <span m="184820">goal.</span> <span m="186180">Can</span> <span m="186620">anyone</span>
  <span m="186800">think</span> <span m="186980">about</span> <span m="187100">a</span>
  <span m="187130">setting</span> <span m="187370">where</span> <span m="187490">that</span>
  <span m="187670">might</span> <span m="187910">not</span> <span m="188150">be</span>
  <span m="188330">desirable?</span> <span m="194420">Yeah.</span></p><p><span m="196170">AUDIENCE:</span>
  <span m="196220">What</span> <span m="196270">if</span> <span m="196360">the</span>
  <span m="196480">reward</span> <span m="196840">is</span> <span m="197080">the</span>
  <span m="197200">patient</span> <span m="197770">living</span> <span m="198100">or</span>
  <span m="198220">dying?</span> <span m="198590">You</span> <span m="198700">don't</span>
  <span m="198850">want</span> <span m="199090">it</span> <span m="199180">to</span>
  <span m="199450">have</span> <span m="199720">high</span> <span m="199990">ratings</span>
  <span m="200120">like</span> <span m="200650">saving</span> <span m="201000">two</span>
  <span m="201340">patients</span> <span m="201740">and</span> <span m="201900">[INAUDIBLE]</span>
  <span m="202360">and</span> <span m="202790">expect</span> <span m="203100">the</span>
  <span m="203225">same</span> <span m="203350">[INAUDIBLE].</span></p><p><span m="204730">DAVID
  SONTAG:</span> <span m="204865">So</span> <span m="205000">what</span> <span m="205180">happens</span>
  <span m="205390">if</span> <span m="205480">this</span> <span m="205660">reward</span>
  <span m="205990">is</span> <span m="206050">something</span> <span m="207700">mission</span>
  <span m="208030">critical</span> <span m="208460">like</span> <span m="209870">a</span>
  <span m="209980">patient</span> <span m="210280">dying?</span> <span m="212230">You</span>
  <span m="213250">really</span> <span m="213580">want</span> <span m="213790">to</span>
  <span m="213880">try</span> <span m="214060">to</span> <span m="214120">avoid</span>
  <span m="214510">that</span> <span m="214780">from</span> <span m="214960">happening</span>
  <span m="215350">as</span> <span m="215440">much</span> <span m="215590">as</span>
  <span m="215680">possible.</span> <span m="216550">Of</span> <span m="216640">course,</span>
  <span m="216850">there</span> <span m="216970">are</span> <span m="217030">other</span>
  <span m="217270">criteria</span> <span m="217720">that</span> <span m="217840">we</span>
  <span m="217930">might</span> <span m="218050">be</span> <span m="218110">interested</span>
  <span m="218410">in</span> <span m="218530">as</span> <span m="218650">well.</span></p><p><span
  m="219430">And</span> <span m="220300">both</span> <span m="220750">in</span> <span
  m="220870">Frederick's</span> <span m="221260">lecture</span> <span m="221590">on</span>
  <span m="221680">Tuesday</span> <span m="222220">and</span> <span m="222460">in</span>
  <span m="222580">the</span> <span m="222670">readings,</span> <span m="223600">we</span>
  <span m="223690">talked</span> <span m="223960">about</span> <span m="224080">how</span>
  <span m="224200">there</span> <span m="224320">might</span> <span m="224500">be</span>
  <span m="224620">other</span> <span m="225340">aspects</span> <span m="226390">about</span>
  <span m="227530">making</span> <span m="227800">sure</span> <span m="227920">that</span>
  <span m="228040">a</span> <span m="228070">patient</span> <span m="228370">is</span>
  <span m="228700">not</span> <span m="228910">just</span> <span m="229090">alive</span>
  <span m="229360">but</span> <span m="229480">also</span> <span m="229780">healthy,</span>
  <span m="231680">which</span> <span m="231850">might</span> <span m="232060">play</span>
  <span m="232300">into</span> <span m="232460">your</span> <span m="232500">reward</span>
  <span m="232810">functions.</span> <span m="233230">And</span> <span m="233320">there</span>
  <span m="233390">might</span> <span m="233460">be</span> <span m="233530">rewards</span>
  <span m="233910">associated with</span> <span m="234190">those.</span></p><p><span
  m="235690">And</span> <span m="236050">if</span> <span m="236110">you</span> <span
  m="236170">were</span> <span m="236230">to</span> <span m="236350">just,</span>
  <span m="236590">for</span> <span m="236680">example,</span> <span m="236980">put</span>
  <span m="237340">a</span> <span m="237430">positive</span> <span m="238810">or</span>
  <span m="238900">negative</span> <span m="239290">infinity</span> <span m="240190">for</span>
  <span m="240440">a</span> <span m="240460">patient</span> <span m="240790">dying,</span>
  <span m="241990">that's</span> <span m="242350">a</span> <span m="242380">nonstarter,</span>
  <span m="243050">right,</span> <span m="243310">because</span> <span m="243550">if</span>
  <span m="243610">you</span> <span m="243670">did</span> <span m="243880">that,</span>
  <span m="244720">unfortunately</span> <span m="245770">in</span> <span m="246640">this</span>
  <span m="246820">world,</span> <span m="247390">we're</span> <span m="247600">not</span>
  <span m="247750">always</span> <span m="248050">going</span> <span m="248110">to</span>
  <span m="248230">be</span> <span m="248290">able</span> <span m="248410">to</span>
  <span m="248470">keep</span> <span m="248590">patients</span> <span m="248950">alive.</span>
  <span m="249910">And</span> <span m="250000">so</span> <span m="250150">you're</span>
  <span m="250240">going</span> <span m="250390">to</span> <span m="250480">get</span>
  <span m="250600">into</span> <span m="250930">an</span> <span m="251140">infeasible</span>
  <span m="251650">optimization</span> <span m="252280">problem.</span> <span m="253460">So</span>
  <span m="253630">minus</span> <span m="253960">infinity</span> <span m="254320">is</span>
  <span m="254380">not</span> <span m="254530">an</span> <span m="254650">option.</span></p><p><span
  m="255130">We're</span> <span m="255490">going</span> <span m="255640">to</span>
  <span m="255700">have</span> <span m="255790">to</span> <span m="255910">put</span>
  <span m="256149">some</span> <span m="256450">number</span> <span m="256990">to</span>
  <span m="257260">it</span> <span m="257560">in</span> <span m="257709">this</span>
  <span m="257860">type</span> <span m="258070">of</span> <span m="258160">approach.</span>
  <span m="260450">But</span> <span m="260529">then</span> <span m="260829">you're</span>
  <span m="260950">going</span> <span m="261050">to</span> <span m="261130">start</span>
  <span m="261310">trading</span> <span m="261640">off</span> <span m="261850">between</span>
  <span m="263080">patients.</span> <span m="264730">In</span> <span m="264820">some</span>
  <span m="265030">cases,</span> <span m="265480">you</span> <span m="265570">might</span>
  <span m="267430">have</span> <span m="268430">a</span> <span m="269050">very</span>
  <span m="269410">high</span> <span m="269710">reward</span> <span m="270160">for--</span>
  <span m="271510">there</span> <span m="271690">are</span> <span m="271750">two</span>
  <span m="271960">different</span> <span m="273100">solutions</span> <span m="273670">that</span>
  <span m="273760">you</span> <span m="273970">might</span> <span m="274150">imagine,</span>
  <span m="275000">one</span> <span m="275110">solution</span> <span m="275560">where</span>
  <span m="275830">the</span> <span m="276190">reward</span> <span m="276700">is</span>
  <span m="276790">somewhat</span> <span m="277090">balanced</span> <span m="277600">across</span>
  <span m="278020">patients</span> <span m="279210">and</span> <span m="279310">another</span>
  <span m="279670">situation</span> <span m="280300">where</span> <span m="280660">you</span>
  <span m="280780">have</span> <span m="281060">really</span> <span m="281350">small</span>
  <span m="281680">values</span> <span m="281950">of</span> <span m="282010">reward</span>
  <span m="282370">for</span> <span m="282490">some</span> <span m="282670">patients</span>
  <span m="283660">and</span> <span m="283930">a</span> <span m="283960">few</span>
  <span m="284140">patients</span> <span m="284410">with</span> <span m="284530">very</span>
  <span m="284860">large</span> <span m="285110">values and</span> <span m="285340">rewards.</span></p><p><span
  m="285760">And</span> <span m="285850">both</span> <span m="286030">of them</span>
  <span m="286120">could</span> <span m="286240">be</span> <span m="286300">the</span>
  <span m="286390">same</span> <span m="286600">average,</span> <span m="287080">obviously.</span>
  <span m="289200">But</span> <span m="289240">both</span> <span m="289480">are</span>
  <span m="289540">not</span> <span m="289660">necessarily</span> <span m="290050">equally</span>
  <span m="291010">useful.</span> <span m="291910">We</span> <span m="292030">might</span>
  <span m="292210">want</span> <span m="292450">to</span> <span m="292570">say</span>
  <span m="292810">that</span> <span m="292930">we</span> <span m="293050">prefer</span>
  <span m="293440">to</span> <span m="293620">avoid</span> <span m="294190">that</span>
  <span m="294460">worst-case</span> <span m="295060">situation.</span></p><p><span
  m="296560">So</span> <span m="296710">one</span> <span m="296800">could</span> <span
  m="296950">imagine</span> <span m="297250">other</span> <span m="297460">ways</span>
  <span m="297730">of</span> <span m="297790">formulating</span> <span m="298390">this</span>
  <span m="298510">optimization</span> <span m="299020">problem,</span> <span m="299350">like</span>
  <span m="300400">maybe</span> <span m="300610">you</span> <span m="300670">want</span>
  <span m="300850">to</span> <span m="300940">control</span> <span m="301420">the</span>
  <span m="301660">worst-case</span> <span m="302620">reward</span> <span m="303160">instead</span>
  <span m="303460">of</span> <span m="303550">the</span> <span m="303790">average-case</span>
  <span m="304570">reward.</span> <span m="305650">Or</span> <span m="305710">maybe</span>
  <span m="305890">you</span> <span m="305950">want</span> <span m="306000">to</span>
  <span m="306070">say</span> <span m="306190">something</span> <span m="306460">about</span>
  <span m="307300">different</span> <span m="307660">quartiles.</span> <span m="309580">I</span>
  <span m="309640">just</span> <span m="309760">wanted</span> <span m="309940">to</span>
  <span m="310000">point</span> <span m="310210">that</span> <span m="310330">out,</span>
  <span m="310510">because</span> <span m="310810">really</span> <span m="311150">that's</span>
  <span m="311410">the</span> <span m="311500">starting</span> <span m="311950">place</span>
  <span m="312280">for</span> <span m="312670">a</span> <span m="312730">lot</span>
  <span m="312970">of</span> <span m="313300">the</span> <span m="313450">work</span>
  <span m="313720">that</span> <span m="313870">we're</span> <span m="313960">doing</span>
  <span m="314230">here.</span></p><p><span m="316340">So</span> <span m="316360">now
  I want</span> <span m="316540">us</span> <span m="316740">to</span> <span m="316810">think</span>
  <span m="317050">through,</span> <span m="317230">OK,</span> <span m="317620">returning</span>
  <span m="318040">back</span> <span m="318310">to</span> <span m="318430">this</span>
  <span m="318640">goal,</span> <span m="320160">we've</span> <span m="320370">done</span>
  <span m="321120">our</span> <span m="322260">policy</span> <span m="322800">iteration</span>
  <span m="324870">or</span> <span m="325200">we've</span> <span m="325590">done</span>
  <span m="325770">our</span> <span m="325830">Q</span> <span m="326040">learning,</span>
  <span m="326310">that</span> <span m="326430">is,</span> <span m="327120">and</span>
  <span m="327930">we</span> <span m="328290">get</span> <span m="328500">a</span>
  <span m="328560">policy</span> <span m="329040">out.</span> <span m="329220">And</span>
  <span m="329340">we</span> <span m="329670">might</span> <span m="330090">now</span>
  <span m="330240">want</span> <span m="330360">to</span> <span m="330420">know</span>
  <span m="330610">what</span> <span m="330780">is</span> <span m="330870">the</span>
  <span m="330960">value</span> <span m="331320">of</span> <span m="331410">that</span>
  <span m="331530">policy?</span> <span m="332400">So</span> <span m="333060">what</span>
  <span m="333270">is</span> <span m="333390">our</span> <span m="333540">estimate</span>
  <span m="333990">of</span> <span m="334110">that</span> <span m="334260">quantity?</span></p><p><span
  m="336050">Well,</span> <span m="337170">to</span> <span m="337330">get</span> <span
  m="337540">that,</span> <span m="338110">one</span> <span m="338320">could</span>
  <span m="338440">just</span> <span m="338590">try</span> <span m="338710">to</span>
  <span m="338800">read</span> <span m="339100">it</span> <span m="339220">off</span>
  <span m="339460">from</span> <span m="339610">the</span> <span m="339670">results</span>
  <span m="339970">of</span> <span m="340060">Q</span> <span m="340300">learning</span>
  <span m="341230">by</span> <span m="341500">just</span> <span m="341680">computing</span>
  <span m="342430">that</span> <span m="342970">the</span> <span m="343330">pi--</span>
  <span m="343900">what</span> <span m="343960">I'm</span> <span m="344020">calling
  v</span> <span m="344320">pi</span> <span m="344530">hat--</span> <span m="344890">the</span>
  <span m="345010">estimate</span> <span m="346120">is</span> <span m="346300">just</span>
  <span m="347140">equal</span> <span m="347530">to</span> <span m="347830">now</span>
  <span m="348280">a</span> <span m="348370">maximum</span> <span m="349480">over</span>
  <span m="350260">actions</span> <span m="350860">a</span> <span m="351640">of</span>
  <span m="352420">your</span> <span m="352630">Q</span> <span m="353020">function</span>
  <span m="354310">evaluated</span> <span m="354910">at</span> <span m="355180">whatever</span>
  <span m="355390">your</span> <span m="355480">initial</span> <span m="355780">state</span>
  <span m="356290">is</span> <span m="357460">and</span> <span m="360180">the</span>
  <span m="360550">optimal</span> <span m="360940">choice</span> <span m="361180">of</span>
  <span m="361270">action</span> <span m="361780">a.</span></p><p><span m="363820">So</span>
  <span m="364500">all</span> <span m="364680">I'm</span> <span m="364800">saying</span>
  <span m="365100">here</span> <span m="365310">is</span> <span m="365460">that</span>
  <span m="366090">the</span> <span m="366240">last</span> <span m="366630">step</span>
  <span m="367200">of</span> <span m="367350">the</span> <span m="367500">algorithm</span>
  <span m="367590">might be</span> <span m="367680">to</span> <span m="368040">ask,</span>
  <span m="368280">well,</span> <span m="368430">what</span> <span m="368670">is</span>
  <span m="368940">the</span> <span m="369120">expected</span> <span m="369930">reward</span>
  <span m="370470">of</span> <span m="370590">this</span> <span m="370800">policy?</span>
  <span m="371990">And</span> <span m="372090">if you</span> <span m="372150">remember,</span>
  <span m="372690">the</span> <span m="373020">Q</span> <span m="373230">learning</span>
  <span m="373470">algorithm</span> <span m="373770">is,</span> <span m="373860">in
  essence,</span> <span m="374110">a</span> <span m="374220">dynamic</span> <span
  m="374730">programming</span> <span m="375180">algorithm</span> <span m="375540">working</span>
  <span m="375840">its</span> <span m="375960">way</span> <span m="376200">from</span>
  <span m="376920">the</span> <span m="377320">sort</span> <span m="377460">of</span>
  <span m="378510">large</span> <span m="378840">values</span> <span m="379050">of</span>
  <span m="379110">time</span> <span m="379410">up</span> <span m="379530">to</span>
  <span m="380040">the</span> <span m="380250">present.</span> <span m="381160">And</span>
  <span m="381420">it</span> <span m="381690">is</span> <span m="382050">indeed</span>
  <span m="382590">actually</span> <span m="383490">computing</span> <span m="384120">this</span>
  <span m="384330">expected</span> <span m="384840">value</span> <span m="385110">that</span>
  <span m="385230">you're</span> <span m="385350">interested</span> <span m="385740">in.</span>
  <span m="385990">So</span> <span m="386010">you</span> <span m="386070">could</span>
  <span m="386160">just</span> <span m="386280">read</span> <span m="386520">it</span>
  <span m="386640">off</span> <span m="386940">from</span> <span m="387120">the</span>
  <span m="387240">Q</span> <span m="387480">values</span> <span m="387870">at</span>
  <span m="387960">the</span> <span m="388020">very</span> <span m="388290">end.</span></p><p><span
  m="390600">But</span> <span m="390990">I</span> <span m="391020">want</span> <span
  m="391140">to</span> <span m="391200">point</span> <span m="391410">out</span> <span
  m="391560">that</span> <span m="391710">here</span> <span m="392140">there's</span>
  <span m="392520">an</span> <span m="392670">implicit</span> <span m="393180">policy</span>
  <span m="393660">built</span> <span m="394020">in.</span> <span m="394500">So</span>
  <span m="395100">I'm</span> <span m="395220">going</span> <span m="395340">to</span>
  <span m="395400">compare</span> <span m="395790">this</span> <span m="396010">in
  just a</span> <span m="396350">second</span> <span m="396810">to</span> <span m="396990">what</span>
  <span m="397140">happens</span> <span m="397830">under</span> <span m="398700">the</span>
  <span m="399030">causal</span> <span m="399390">inference</span> <span m="400050">scenario.</span>
  <span m="400540">So</span> <span m="400650">just</span> <span m="400830">a</span>
  <span m="400860">single</span> <span m="401160">time</span> <span m="401410">step</span>
  <span m="401710">in</span> <span m="401880">potential</span> <span m="402210">outcomes</span>
  <span m="402600">framework</span> <span m="402840">that</span> <span m="402930">we're</span>
  <span m="403020">used</span> <span m="403230">to.</span></p><p><span m="405170">Notice</span>
  <span m="405510">that</span> <span m="405610">the</span> <span m="406050">value</span>
  <span m="406350">of</span> <span m="406440">this</span> <span m="406620">policy,</span>
  <span m="408870">the</span> <span m="408990">reason</span> <span m="409290">why</span>
  <span m="409470">it's</span> <span m="409590">a</span> <span m="409620">function</span>
  <span m="410190">of</span> <span m="410480">pi</span> <span m="411210">is</span>
  <span m="411390">because</span> <span m="412770">the</span> <span m="413070">value</span>
  <span m="413440">is</span> <span m="415560">a</span> <span m="415590">function</span>
  <span m="415950">of</span> <span m="416340">every</span> <span m="416580">subsequent</span>
  <span m="417180">action</span> <span m="417510">that</span> <span m="417600">you're</span>
  <span m="417690">taking</span> <span m="417990">as</span> <span m="418170">well.</span>
  <span m="418640">And</span> <span m="418650">so</span> <span m="420810">now</span>
  <span m="420960">let's</span> <span m="421110">just</span> <span m="421260">compare</span>
  <span m="421620">that</span> <span m="421770">for</span> <span m="421860">a</span>
  <span m="421890">second</span> <span m="422220">to</span> <span m="422340">what</span>
  <span m="422460">happens</span> <span m="422990">in</span> <span m="423180">the</span>
  <span m="423960">potential</span> <span m="424320">outcomes</span> <span m="424740">framework.</span>
  <span m="428180">So</span> <span m="428290">there,</span> <span m="428960">our</span>
  <span m="429160">starting</span> <span m="429550">place--</span> <span m="430640">so</span>
  <span m="430690">now</span> <span m="430960">I'm</span> <span m="431050">going</span>
  <span m="431320">to</span> <span m="434500">turn</span> <span m="435700">our</span>
  <span m="435820">attention</span> <span m="436720">for</span> <span m="437170">just</span>
  <span m="437410">one</span> <span m="437560">moment</span> <span m="438460">from</span>
  <span m="438910">reinforcement</span> <span m="439600">learning</span> <span m="440440">now</span>
  <span m="440800">back</span> <span m="441310">to</span> <span m="441790">just</span>
  <span m="442120">causal</span> <span m="442570">inference.</span></p><p><span m="444240">In</span>
  <span m="444340">reinforcement</span> <span m="444820">learning,</span> <span m="445160">we</span>
  <span m="445260">talked</span> <span m="445510">about</span> <span m="445780">policies.</span>
  <span m="446720">How</span> <span m="446800">do</span> <span m="446890">we</span>
  <span m="446980">find</span> <span m="448030">policies</span> <span m="448840">to</span>
  <span m="449050">do</span> <span m="449200">well</span> <span m="449560">in</span>
  <span m="449650">terms</span> <span m="449920">of</span> <span m="450040">some</span>
  <span m="450310">expected</span> <span m="451120">reward</span> <span m="451600">of</span>
  <span m="451720">this</span> <span m="451870">policy?</span> <span m="453040">But</span>
  <span m="453190">yet</span> <span m="453340">when</span> <span m="453510">we were</span>
  <span m="453610">talking</span> <span m="454030">about</span> <span m="455690">causal</span>
  <span m="456050">inference,</span> <span m="457250">we</span> <span m="458150">only</span>
  <span m="458450">used</span> <span m="458690">words</span> <span m="459080">like</span>
  <span m="460310">average</span> <span m="460610">treatment</span> <span m="460940">effect</span>
  <span m="461420">or</span> <span m="461600">conditional</span> <span m="462050">average</span>
  <span m="462290">treatment</span> <span m="462560">effect,</span> <span m="464390">where</span>
  <span m="465020">for</span> <span m="465230">example,</span> <span m="465770">to</span>
  <span m="465950">estimate</span> <span m="466530">the</span> <span m="467180">conditional</span>
  <span m="467600">average</span> <span m="467870">treatment</span> <span m="468110">effect,</span>
  <span m="468540">what</span> <span m="468560">we</span> <span m="468650">said</span>
  <span m="468920">is</span> <span m="469040">we're</span> <span m="469130">going</span>
  <span m="469240">to</span> <span m="469310">first</span> <span m="469610">learn,</span>
  <span m="469970">if</span> <span m="470090">we</span> <span m="470150">use</span>
  <span m="471500">a</span> <span m="471920">covariate</span> <span m="472130">adjustment</span>
  <span m="472430">approach,</span> <span m="472790">we</span> <span m="472940">learn</span>
  <span m="473210">some</span> <span m="473390">function</span> <span m="475010">f</span>
  <span m="475340">of</span> <span m="476690">x</span> <span m="477080">comma</span>
  <span m="477530">t,</span> <span m="478580">which</span> <span m="478790">is</span>
  <span m="479030">intended</span> <span m="479570">to</span> <span m="479720">be</span>
  <span m="479900">an</span> <span m="480020">approximation</span> <span m="481370">of</span>
  <span m="482450">the</span> <span m="482540">expected</span> <span m="483110">value</span>
  <span m="483620">of</span> <span m="483740">your</span> <span m="483920">outcome</span>
  <span m="484580">y</span> <span m="485590">given</span> <span m="487520">x</span>
  <span m="488060">comma--</span> <span m="492370">I'll</span> <span m="492560">say</span>
  <span m="496630">y</span> <span m="497110">of</span> <span m="497590">t.</span>
  <span m="498960">There.</span> <span m="499360">So</span> <span m="499990">that</span>
  <span m="500140">notation.</span></p><p><span m="500970">So</span> <span m="501910">the</span>
  <span m="502000">goal</span> <span m="502300">of covariate</span> <span m="502540">adjustment</span>
  <span m="502840">was</span> <span m="502930">to</span> <span m="503020">estimate</span>
  <span m="503320">this</span> <span m="503470">quantity.</span> <span m="505030">And</span>
  <span m="506490">we</span> <span m="506700">could</span> <span m="507210">use</span>
  <span m="507480">that</span> <span m="507660">then</span> <span m="507960">to</span>
  <span m="508110">try</span> <span m="508290">to</span> <span m="508380">construct</span>
  <span m="508800">a</span> <span m="508860">policy.</span> <span m="509470">For</span>
  <span m="509610">example,</span> <span m="511510">you</span> <span m="512110">could</span>
  <span m="512230">think</span> <span m="512409">about</span> <span m="512620">the</span>
  <span m="512679">policy</span> <span m="515230">pi</span> <span m="516010">of</span>
  <span m="516400">x,</span> <span m="517690">which</span> <span m="517929">simply</span>
  <span m="518260">looks</span> <span m="518530">to</span> <span m="518679">see</span>
  <span m="519580">is--</span> <span m="522309">we'll</span> <span m="522460">say</span>
  <span m="522669">it's</span> <span m="523390">1</span> <span m="524650">if</span>
  <span m="525940">CATE</span> <span m="527590">or</span> <span m="527680">your</span>
  <span m="527830">estimate</span> <span m="528220">of</span> <span m="528370">CATE</span>
  <span m="529150">for</span> <span m="529540">x</span> <span m="530860">is</span>
  <span m="531250">positive</span> <span m="532750">and</span> <span m="533650">0</span>
  <span m="534770">otherwise.</span> <span m="536290">Just</span> <span m="536500">remind</span>
  <span m="536890">you,</span> <span m="537280">the</span> <span m="537400">way</span>
  <span m="537610">that</span> <span m="537760">we</span> <span m="537860">got</span>
  <span m="538000">the</span> <span m="538090">estimate</span> <span m="538450">of</span>
  <span m="538570">CATE</span> <span m="542490">for</span> <span m="542700">an</span>
  <span m="542760">individual</span> <span m="543120">x</span> <span m="543630">was</span>
  <span m="543840">just</span> <span m="544050">by</span> <span m="544560">looking</span>
  <span m="545070">at</span> <span m="545790">f</span> <span m="546270">of</span>
  <span m="546750">x</span> <span m="547450">comma</span> <span m="547800">1</span>
  <span m="548730">minus</span> <span m="549510">f</span> <span m="550110">of</span>
  <span m="550320">x</span> <span m="550640">comma</span> <span m="551310">0.</span></p><p><span
  m="570620">So</span> <span m="571490">if</span> <span m="571640">we</span> <span
  m="571760">have</span> <span m="572000">a</span> <span m="572060">policy--</span>
  <span m="572690">so</span> <span m="573020">now</span> <span m="573230">we're</span>
  <span m="573320">going</span> <span m="573380">to</span> <span m="573440">start</span>
  <span m="573620">thinking</span> <span m="573830">about</span> <span m="574550">policies</span>
  <span m="575300">in</span> <span m="575390">the</span> <span m="575450">context</span>
  <span m="575840">of</span> <span m="575930">causal</span> <span m="576110">inference,</span>
  <span m="576410">just</span> <span m="576680">like</span> <span m="576860">we</span>
  <span m="576950">were</span> <span m="577070">doing</span> <span m="577400">in</span>
  <span m="577640">reinforcement</span> <span m="578150">learning.</span> <span m="579070">And</span>
  <span m="579350">I</span> <span m="579410">want</span> <span m="579530">us</span>
  <span m="579590">to</span> <span m="579680">think</span> <span m="579920">through</span>
  <span m="580790">what</span> <span m="581180">would</span> <span m="581630">the</span>
  <span m="581840">analogous</span> <span m="582770">value</span> <span m="583610">of</span>
  <span m="583760">the</span> <span m="583850">policy</span> <span m="584420">be?</span>
  <span m="586720">How</span> <span m="586990">good</span> <span m="588550">is</span>
  <span m="588790">that</span> <span m="589150">policy?</span> <span m="590050">It</span>
  <span m="590150">could</span> <span m="590170">be</span> <span m="590260">another</span>
  <span m="590530">policy,</span> <span m="590860">but</span> <span m="590950">right</span>
  <span m="591100">now</span> <span m="591220">I'm</span> <span m="591340">assuming</span>
  <span m="591850">I'm</span> <span m="592000">just</span> <span m="592150">going</span>
  <span m="592270">to</span> <span m="592330">focus</span> <span m="592600">on</span>
  <span m="592690">this</span> <span m="592840">policy</span> <span m="593160">that
  I</span> <span m="593290">show</span> <span m="593470">up</span> <span m="593620">here.</span></p><p><span
  m="596690">Well,</span> <span m="597790">one</span> <span m="598090">approach</span>
  <span m="598460">to</span> <span m="598510">try</span> <span m="598690">to</span>
  <span m="598780">evaluate</span> <span m="599140">how</span> <span m="599290">good</span>
  <span m="599470">that</span> <span m="599590">policy</span> <span m="600430">is,</span>
  <span m="600685">is</span> <span m="600940">exactly</span> <span m="601630">analogous</span>
  <span m="602050">to</span> <span m="602110">what</span> <span m="602230">we</span>
  <span m="602350">did</span> <span m="602500">in</span> <span m="602590">reinforcement</span>
  <span m="603160">learning.</span> <span m="603610">In</span> <span m="603730">essence,</span>
  <span m="604100">what</span> <span m="604200">we're</span> <span m="604300">going</span>
  <span m="604400">to</span> <span m="604500">say</span> <span m="604960">is</span>
  <span m="606070">we</span> <span m="606670">evaluate</span> <span m="607360">the</span>
  <span m="607450">quality</span> <span m="607780">of the</span> <span m="607840">policy</span>
  <span m="608470">by</span> <span m="609100">summing</span> <span m="609580">over</span>
  <span m="609850">your</span> <span m="609970">empirical</span> <span m="610450">data</span>
  <span m="611830">of</span> <span m="620270">pi</span> <span m="621050">of</span>
  <span m="621530">xi.</span> <span m="622420">So</span> <span m="622580">this</span>
  <span m="622730">is</span> <span m="622820">going</span> <span m="623030">to</span>
  <span m="623180">be</span> <span m="623930">1</span> <span m="624950">if</span>
  <span m="625730">the</span> <span m="625850">policy</span> <span m="626480">says</span>
  <span m="626960">to</span> <span m="627290">give</span> <span m="627560">treatment</span>
  <span m="628130">1</span> <span m="628460">to</span> <span m="628850">individual</span>
  <span m="629420">xi.</span></p><p><span m="631910">In</span> <span m="632000">that</span>
  <span m="632180">case,</span> <span m="632730">we</span> <span m="632990">say</span>
  <span m="633200">that</span> <span m="633320">the</span> <span m="633410">value</span>
  <span m="633920">is</span> <span m="634160">f</span> <span m="634550">of</span>
  <span m="634700">x</span> <span m="634910">comma</span> <span m="635240">1.</span>
  <span m="637730">Or</span> <span m="638360">if</span> <span m="638540">you</span>
  <span m="638720">gave</span> <span m="639320">the</span> <span m="639440">second--</span>
  <span m="641550">if</span> <span m="641570">the</span> <span m="641660">policy</span>
  <span m="642080">would</span> <span m="642530">give</span> <span m="642980">treatment</span>
  <span m="643340">0,</span> <span m="645540">the</span> <span m="645660">value</span>
  <span m="646260">of</span> <span m="646380">the</span> <span m="646470">policy</span>
  <span m="646920">on</span> <span m="647010">that</span> <span m="647130">individual</span>
  <span m="648120">is</span> <span m="648300">1</span> <span m="648570">minus</span>
  <span m="648960">pi</span> <span m="649260">of</span> <span m="649470">x</span>
  <span m="649950">times</span> <span m="651390">f</span> <span m="651930">of</span>
  <span m="652140">x</span> <span m="652530">comma</span> <span m="652890">0.</span></p><p><span
  m="657357">So</span> <span m="657810">I'm</span> <span m="657870">going</span> <span
  m="657990">to</span> <span m="658050">call</span> <span m="658320">this</span> <span
  m="662540">sort</span> <span m="662740">of</span> <span m="662840">an</span> <span
  m="662900">empirical</span> <span m="663500">estimate</span> <span m="664250">of</span>
  <span m="665790">what</span> <span m="666140">you</span> <span m="666230">should</span>
  <span m="666380">think</span> <span m="666530">about</span> <span m="666800">as</span>
  <span m="667070">the</span> <span m="667190">reward</span> <span m="668420">for</span>
  <span m="668570">a</span> <span m="668630">policy</span> <span m="669360">pi.</span>
  <span m="674690">And it's</span> <span m="674920">exactly</span> <span m="675430">analogous</span>
  <span m="676060">to</span> <span m="677050">the</span> <span m="677320">estimate</span>
  <span m="678260">of</span> <span m="679520">v</span> <span m="679860">of</span>
  <span m="679990">pie</span> <span m="680440">that</span> <span m="680620">you</span>
  <span m="680740">would</span> <span m="680860">get</span> <span m="681100">from</span>
  <span m="681550">a</span> <span m="681610">reinforcement</span> <span m="682120">learning</span>
  <span m="682360">context.</span> <span m="683180">But</span> <span m="683230">now</span>
  <span m="683560">we're</span> <span m="683680">talking</span> <span m="683980">about</span>
  <span m="684160">policies</span> <span m="684880">explicitly.</span></p><p><span
  m="688090">So</span> <span m="688750">let's</span> <span m="688900">try</span> <span
  m="689020">to</span> <span m="689110">dig</span> <span m="689320">down</span> <span
  m="689500">a</span> <span m="689530">little</span> <span m="689650">bit</span> <span
  m="689740">deeper</span> <span m="690040">and</span> <span m="690130">think</span>
  <span m="690340">about</span> <span m="690580">what</span> <span m="690700">this</span>
  <span m="690810">is</span> <span m="690940">actually</span> <span m="691210">saying.</span>
  <span m="694040">Imagine</span> <span m="694520">the</span> <span m="694610">story</span>
  <span m="695240">where</span> <span m="695660">you</span> <span m="695780">just</span>
  <span m="696020">have</span> <span m="696350">a</span> <span m="696440">single</span>
  <span m="698490">covariate</span> <span m="699680">x.</span> <span m="700430">We'll</span>
  <span m="700520">think</span> <span m="700700">about</span> <span m="700880">x</span>
  <span m="701120">as</span> <span m="701240">being,</span> <span m="701780">let's</span>
  <span m="701930">say,</span> <span m="702050">the</span> <span m="702140">patient's</span>
  <span m="702740">age.</span> <span m="705440">And</span> <span m="708910">unfortunately</span>
  <span m="709210">there's</span> <span m="709300">just</span> <span m="709450">one</span>
  <span m="709630">color</span> <span m="709930">here.</span> <span m="710260">But
  I'll</span> <span m="710350">do</span> <span m="710470">my</span> <span m="710590">best</span>
  <span m="710860">with</span> <span m="711010">that.</span> <span m="712100">And</span>
  <span m="712180">imagine</span> <span m="712570">that</span> <span m="713680">the</span>
  <span m="713950">potential</span> <span m="714430">outcome</span> <span m="716410">y0</span>
  <span m="720010">as</span> <span m="720160">a</span> <span m="720190">function</span>
  <span m="720700">of</span> <span m="720960">the</span> <span m="721180">patient's</span>
  <span m="721600">age</span> <span m="722130">x</span> <span m="723280">looks</span>
  <span m="723520">like</span> <span m="723730">this.</span></p><p><span m="726090">Now</span>
  <span m="726140">imagine</span> <span m="726380">that</span> <span m="726470">the</span>
  <span m="726560">other</span> <span m="726830">potential</span> <span m="727220">outcome</span>
  <span m="727700">y1</span> <span m="732030">looked</span> <span m="732210">like</span>
  <span m="732420">that.</span> <span m="734060">So</span> <span m="734230">I'll</span>
  <span m="734310">call</span> <span m="734490">this</span> <span m="734700">the</span>
  <span m="735090">y1</span> <span m="735780">potential</span> <span m="736170">outcome.</span>
  <span m="741610">Suppose</span> <span m="742180">now</span> <span m="742600">that</span>
  <span m="743020">the</span> <span m="743200">policy</span> <span m="744070">that</span>
  <span m="744220">we're</span> <span m="744340">defining</span> <span m="745040">is</span>
  <span m="745240">this.</span> <span m="745750">So</span> <span m="745960">we're</span>
  <span m="746080">going</span> <span m="746320">to</span> <span m="746440">give</span>
  <span m="746680">treatment</span> <span m="746750">one</span> <span m="747550">if</span>
  <span m="747820">the</span> <span m="747940">condition</span> <span m="748240">of</span>
  <span m="748360">our</span> <span m="748460">treatment</span> <span m="748690">effect</span>
  <span m="749110">is</span> <span m="749260">positive</span> <span m="749800">and</span>
  <span m="749890">0</span> <span m="750250">otherwise.</span></p><p><span m="752240">I</span>
  <span m="752300">want</span> <span m="752420">everyone</span> <span m="752780">to</span>
  <span m="752900">draw</span> <span m="753740">what</span> <span m="753980">the</span>
  <span m="754190">value</span> <span m="755150">of</span> <span m="755330">that</span>
  <span m="755510">policy</span> <span m="756320">is</span> <span m="757010">on</span>
  <span m="757130">a</span> <span m="757190">piece</span> <span m="757370">of</span>
  <span m="757460">paper.</span> <span m="758940">It's</span> <span m="758960">going</span>
  <span m="759200">to</span> <span m="759320">be--</span> <span m="764250">I'm</span>
  <span m="764370">sorry--</span> <span m="764580">I</span> <span m="764820">want</span>
  <span m="764970">everyone</span> <span m="765300">to</span> <span m="765510">write</span>
  <span m="765690">on</span> <span m="765810">a</span> <span m="765840">piece</span>
  <span m="765990">of</span> <span m="766050">paper</span> <span m="766360">what</span>
  <span m="766560">the</span> <span m="766650">value</span> <span m="767250">of</span>
  <span m="767520">the</span> <span m="767610">policy</span> <span m="768090">would</span>
  <span m="768240">be</span> <span m="768390">for</span> <span m="768540">each</span>
  <span m="768720">individual.</span> <span m="769630">So</span> <span m="769710">it's</span>
  <span m="769800">going</span> <span m="769920">to</span> <span m="769980">be</span>
  <span m="770130">a</span> <span m="770190">function</span> <span m="772260">of</span>
  <span m="772430">x.</span></p><p><span m="775650">And</span> <span m="775770">now</span>
  <span m="775920">I</span> <span m="776010">want</span> <span m="776370">it</span>
  <span m="776490">to</span> <span m="776610">be--</span> <span m="777420">I'm</span>
  <span m="777510">looking</span> <span m="777840">for</span> <span m="778620">y</span>
  <span m="780180">of</span> <span m="780480">pi</span> <span m="781650">of</span>
  <span m="781980">x.</span> <span m="783690">So</span> <span m="784770">I'm</span>
  <span m="784830">looking</span> <span m="785040">for</span> <span m="785130">you</span>
  <span m="785220">to</span> <span m="785310">draw</span> <span m="785670">that</span>
  <span m="785940">plot.</span> <span m="789010">And</span> <span m="789160">feel</span>
  <span m="789340">free</span> <span m="789430">to</span> <span m="789520">talk</span>
  <span m="789700">to</span> <span m="789760">your</span> <span m="789850">neighbor.</span>
  <span m="793190">In</span> <span m="793250">fact,</span> <span m="793490">I</span>
  <span m="793550">encourage</span> <span m="793880">you</span> <span m="793940">to</span>
  <span m="794030">talk</span> <span m="794180">to</span> <span m="794240">your</span>
  <span m="794330">neighbor.</span></p><p><span m="795584">[SIDE CONVERSATION]</span></p><p>&nbsp;</p><p><span
  m="803230">Just</span> <span m="803450">to</span> <span m="803520">try</span> <span
  m="803640">to</span> <span m="803730">connect</span> <span m="804000">this</span>
  <span m="804150">a</span> <span m="804210">little</span> <span m="804360">bit</span>
  <span m="804450">better</span> <span m="804750">to</span> <span m="804840">what</span>
  <span m="804960">I</span> <span m="805020">have</span> <span m="805170">up</span>
  <span m="805290">here,</span> <span m="805710">I'm</span> <span m="805830">going</span>
  <span m="805910">to</span> <span m="806010">assume</span> <span m="806520">that</span>
  <span m="807060">f--</span> <span m="808304">this</span> <span m="808761">is</span>
  <span m="809220">f of</span> <span m="809340">x1,</span> <span m="810350">and</span>
  <span m="810450">this</span> <span m="810690">is</span> <span m="811230">f</span>
  <span m="811740">of</span> <span m="812040">x0.</span> <span m="819450">All</span>
  <span m="819550">right.</span> <span m="819940">Any</span> <span m="820690">guesses?</span>
  <span m="823540">What</span> <span m="823690">does</span> <span m="823840">this</span>
  <span m="823990">plot</span> <span m="824260">look</span> <span m="824470">like?</span>
  <span m="826630">Someone</span> <span m="826960">who</span> <span m="827020">hasn't</span>
  <span m="827230">spoken</span> <span m="827680">in</span> <span m="827770">the</span>
  <span m="827830">last</span> <span m="828100">one</span> <span m="828400">week</span>
  <span m="828640">and</span> <span m="828730">a</span> <span m="828760">half,</span>
  <span m="829030">if</span> <span m="829120">possible.</span> <span m="838870">Yeah?</span></p><p><span
  m="839500">AUDIENCE:</span> <span m="839560">Does</span> <span m="839620">it</span>
  <span m="839720">take</span> <span m="839910">like</span> <span m="840310">the</span>
  <span m="840400">max of the</span> <span m="840750">functions</span> <span m="841860">at</span>
  <span m="842040">all</span> <span m="842210">point,</span> <span m="842530">like,</span>
  <span m="842835">it would be</span> <span m="843140">y0</span> <span m="843460">up</span>
  <span m="843780">until they</span> <span m="844130">intersect</span> <span m="844500">and</span>
  <span m="844740">then</span> <span m="845040">y1</span> <span m="845350">afterward?</span></p><p><span
  m="846500">DAVID SONTAG:</span> <span m="846705">So</span> <span m="846910">it would
  be something</span> <span m="847210">like</span> <span m="847630">this</span> <span
  m="848200">until</span> <span m="848440">the</span> <span m="848500">intersection</span>
  <span m="848950">point.</span></p><p><span m="849430">AUDIENCE:</span> <span m="849625">Yeah.</span></p><p><span
  m="850210">DAVID SONTAG:</span> <span m="850300">And</span> <span m="850390">then</span>
  <span m="850660">like</span> <span m="850840">that</span> <span m="851080">afterwards.</span>
  <span m="852310">Yeah.</span> <span m="852550">That's</span> <span m="852990">exactly</span>
  <span m="853360">what I'm</span> <span m="853420">going</span> <span m="853630">for.</span>
  <span m="855310">And</span> <span m="855610">let's</span> <span m="855760">try</span>
  <span m="855880">to</span> <span m="855970">think</span> <span m="856150">through</span>
  <span m="856810">why</span> <span m="857200">is</span> <span m="857350">that</span>
  <span m="857650">the</span> <span m="857800">value</span> <span m="858490">of</span>
  <span m="858730">the</span> <span m="858880">policy?</span> <span m="860910">Well,</span>
  <span m="862560">here</span> <span m="863570">the</span> <span m="863950">CATE,</span>
  <span m="864600">which</span> <span m="864840">is</span> <span m="864960">looking</span>
  <span m="865260">at</span> <span m="865350">a</span> <span m="865440">difference</span>
  <span m="865890">between</span> <span m="866580">these</span> <span m="866850">two</span>
  <span m="867060">lines</span> <span m="867540">as</span> <span m="867660">negative--</span>
  <span m="869190">so</span> <span m="869910">for</span> <span m="870210">every</span>
  <span m="871050">x</span> <span m="871560">up</span> <span m="871740">to</span>
  <span m="871890">this</span> <span m="872070">crossing</span> <span m="872550">point,</span>
  <span m="873600">the</span> <span m="873840">policy</span> <span m="874410">that</span>
  <span m="874560">we've</span> <span m="874710">defined</span> <span m="875280">over</span>
  <span m="875520">there</span> <span m="876270">is</span> <span m="876420">going</span>
  <span m="876660">to</span> <span m="876840">perform</span> <span m="879360">action--</span>
  <span m="882520">wait.</span> <span m="883050">Am</span> <span m="883160">I</span>
  <span m="883300">drawing</span> <span m="883500">this</span> <span m="883590">correctly?</span></p><p><span
  m="885460">Maybe</span> <span m="885590">it's</span> <span m="885720">actually</span>
  <span m="885850">the</span> <span m="885910">opposite,</span> <span m="886180">right?</span>
  <span m="887948">This</span> <span m="888550">should</span> <span m="888690">be</span>
  <span m="888750">doing</span> <span m="888930">action</span> <span m="889170">one.</span>
  <span m="894200">Here.</span> <span m="894600">OK.</span> <span m="894780">So</span>
  <span m="894930">here</span> <span m="895230">the</span> <span m="895350">CATE</span>
  <span m="895920">is</span> <span m="898710">negative.</span> <span m="900250">And</span>
  <span m="900270">so</span> <span m="900390">by</span> <span m="900570">my</span>
  <span m="900840">definition,</span> <span m="901590">the</span> <span m="901710">action</span>
  <span m="902040">performed</span> <span m="902370">is</span> <span m="902490">action</span>
  <span m="902850">0.</span> <span m="903990">And</span> <span m="904110">so</span>
  <span m="904450">the</span> <span m="904650">value</span> <span m="905070">of</span>
  <span m="905160">the</span> <span m="905250">policy</span> <span m="905790">is</span>
  <span m="905970">actually</span> <span m="906240">this</span> <span m="906420">one.</span></p><p><span
  m="907828">[INTERPOSING VOICES]</span></p><p><span m="910516">DAVID SONTAG:</span>
  <span m="910970">Oh.</span> <span m="911500">Wait.</span> <span m="911840">Oh,</span>
  <span m="912080">good.</span> <span m="912470">[INAUDIBLE].</span> <span m="914210">Because</span>
  <span m="914360">this</span> <span m="914480">is</span> <span m="914540">the</span>
  <span m="914630">graph</span> <span m="914870">I</span> <span m="914930">have</span>
  <span m="915060">in</span> <span m="915380">my</span> <span m="915500">notes.</span>
  <span m="915800">Oh, good.</span> <span m="916270">OK.</span> <span m="918050">I</span>
  <span m="918080">was</span> <span m="918200">getting</span> <span m="918410">worried.</span>
  <span m="920040">OK.</span> <span m="920240">So</span> <span m="920360">it's</span>
  <span m="920480">this</span> <span m="920690">action,</span> <span m="921530">all</span>
  <span m="921740">the</span> <span m="921830">way</span> <span m="921980">up</span>
  <span m="922070">until</span> <span m="922280">you</span> <span m="922340">get</span>
  <span m="922430">over</span> <span m="922610">here.</span> <span m="923690">And</span>
  <span m="923840">then</span> <span m="924260">over</span> <span m="924500">here,</span>
  <span m="925670">now</span> <span m="925940">the</span> <span m="926060">CATE</span>
  <span m="926450">suddenly</span> <span m="926870">becomes</span> <span m="927620">positive.</span>
  <span m="928890">And</span> <span m="928940">so</span> <span m="929450">the</span>
  <span m="930860">action</span> <span m="931340">chosen</span> <span m="931970">is</span>
  <span m="932900">1.</span> <span m="934280">And</span> <span m="934460">so</span>
  <span m="936830">the</span> <span m="936980">value</span> <span m="937700">of</span>
  <span m="937940">that</span> <span m="938150">policy</span> <span m="938810">is</span>
  <span m="939050">y1.</span></p><p><span m="941570">So</span> <span m="941720">one</span>
  <span m="941900">could</span> <span m="942050">write</span> <span m="942290">this</span>
  <span m="942470">a</span> <span m="942530">little</span> <span m="942650">bit</span>
  <span m="942740">differently</span> <span m="943940">for--</span> <span m="950260">in</span>
  <span m="950400">the</span> <span m="950460">case</span> <span m="950640">of</span>
  <span m="950730">just</span> <span m="951030">two</span> <span m="951360">policies,</span>
  <span m="952020">and</span> <span m="952200">now</span> <span m="952320">I'm</span>
  <span m="952380">going</span> <span m="952500">to</span> <span m="952560">write</span>
  <span m="952680">this</span> <span m="952800">in</span> <span m="952890">a</span>
  <span m="952920">way</span> <span m="953520">that</span> <span m="953700">it's</span>
  <span m="953820">really</span> <span m="954030">clear.</span> <span m="955020">In</span>
  <span m="955110">the</span> <span m="955200">case</span> <span m="955410">of</span>
  <span m="955680">just</span> <span m="957030">two</span> <span m="957240">actions,</span>
  <span m="958290">one</span> <span m="958500">could</span> <span m="958650">write</span>
  <span m="958890">this</span> <span m="959040">equivalently</span> <span m="960000">as</span>
  <span m="964130">an</span> <span m="964280">average</span> <span m="964970">over</span>
  <span m="965150">the</span> <span m="965270">data</span> <span m="965570">points</span>
  <span m="967750">of</span> <span m="967990">the</span> <span m="968200">maximum</span>
  <span m="970600">of</span> <span m="971550">fx</span> <span m="973550">comma</span>
  <span m="973720">0</span> <span m="974860">and</span> <span m="976180">f</span>
  <span m="976750">of</span> <span m="977170">x</span> <span m="977560">comma</span>
  <span m="977950">1.</span></p><p><span m="979450">And</span> <span m="979840">this</span>
  <span m="980920">simplification</span> <span m="981700">turning</span> <span m="982000">this</span>
  <span m="982300">formula</span> <span m="982930">into</span> <span m="984550">this</span>
  <span m="984760">formula</span> <span m="985660">is</span> <span m="986080">making</span>
  <span m="986470">the</span> <span m="986560">assumption</span> <span m="987220">that</span>
  <span m="987610">the</span> <span m="987760">pi</span> <span m="988240">that</span>
  <span m="988510">we're</span> <span m="988660">being</span> <span m="988840">evaluated</span>
  <span m="989440">on</span> <span m="989620">is</span> <span m="989770">precisely</span>
  <span m="990160">this</span> <span m="990370">pi.</span> <span m="991100">So</span>
  <span m="993210">this</span> <span m="993450">simplification</span> <span m="993810">is</span>
  <span m="993900">only</span> <span m="994200">for</span> <span m="994410">that</span>
  <span m="994590">pi.</span> <span m="994840">For</span> <span m="994970">another</span>
  <span m="995250">policy,</span> <span m="995610">which</span> <span m="995730">is</span>
  <span m="995820">not</span> <span m="996030">looking</span> <span m="996270">at</span>
  <span m="996360">CATE</span> <span m="996600">or</span> <span m="996690">for</span>
  <span m="996780">example,</span> <span m="997120">which</span> <span m="997140">might</span>
  <span m="997320">threshold</span> <span m="997740">CATE</span> <span m="998040">at</span>
  <span m="998220">a</span> <span m="998340">gamma,</span> <span m="998910">it</span>
  <span m="999030">wouldn't</span> <span m="999300">quite</span> <span m="999570">be</span>
  <span m="999690">this.</span> <span m="1000170">It would be</span> <span m="1000290">something</span>
  <span m="1000530">else.</span></p><p><span m="1003280">But</span> <span m="1003440">I've</span>
  <span m="1004190">gone</span> <span m="1004430">a</span> <span m="1004460">step</span>
  <span m="1004790">further</span> <span m="1005270">here.</span> <span m="1005790">So</span>
  <span m="1005810">what</span> <span m="1006290">I've</span> <span m="1006380">shown</span>
  <span m="1006590">you</span> <span m="1006680">right</span> <span m="1006890">here</span>
  <span m="1007280">is</span> <span m="1007490">not</span> <span m="1007790">the</span>
  <span m="1008090">average</span> <span m="1008660">value</span> <span m="1009020">but</span>
  <span m="1009170">sort</span> <span m="1009320">of</span> <span m="1009380">individual</span>
  <span m="1009800">values.</span> <span m="1010270">I</span> <span m="1010290">have</span>
  <span m="1010400">shown</span> <span m="1010640">you</span> <span m="1010730">the</span>
  <span m="1010820">max</span> <span m="1011480">function.</span> <span m="1012920">But</span>
  <span m="1013100">what</span> <span m="1013310">this</span> <span m="1013520">is</span>
  <span m="1013700">actually</span> <span m="1014240">looking</span> <span m="1014630">at</span>
  <span m="1014870">is</span> <span m="1015080">the</span> <span m="1015380">expected</span>
  <span m="1016700">reward,</span> <span m="1017870">which</span> <span m="1018080">is</span>
  <span m="1018200">now</span> <span m="1018530">averaging</span> <span m="1019250">across</span>
  <span m="1019670">all</span> <span m="1019850">x.</span></p><p><span m="1020390">So</span>
  <span m="1021320">to</span> <span m="1021560">truly</span> <span m="1022100">draw</span>
  <span m="1022340">a</span> <span m="1022400">connection</span> <span m="1022820">between</span>
  <span m="1023150">this</span> <span m="1023300">plot</span> <span m="1023570">we're</span>
  <span m="1023690">drawing</span> <span m="1024200">and</span> <span m="1024950">the</span>
  <span m="1025250">average</span> <span m="1025849">reward</span> <span m="1026300">of</span>
  <span m="1026390">that</span> <span m="1026540">policy,</span> <span m="1027599">what</span>
  <span m="1027619">we</span> <span m="1027710">should</span> <span m="1027829">be</span>
  <span m="1027920">looking</span> <span m="1028190">at</span> <span m="1028280">is</span>
  <span m="1028400">the</span> <span m="1028520">average</span> <span m="1028940">of</span>
  <span m="1029000">these</span> <span m="1029180">two</span> <span m="1029329">functions,</span>
  <span m="1031069">which</span> <span m="1031339">is</span> <span m="1031579">we'll</span>
  <span m="1031700">say</span> <span m="1034440">something</span> <span m="1034740">like</span>
  <span m="1034920">that.</span> <span m="1037050">And</span> <span m="1037710">that</span>
  <span m="1038010">value</span> <span m="1038670">is</span> <span m="1038970">the</span>
  <span m="1039390">expected</span> <span m="1039930">reward.</span></p><p><span m="1041660">Now,</span>
  <span m="1043349">this</span> <span m="1043560">all</span> <span m="1043710">goes</span>
  <span m="1043950">to</span> <span m="1044040">show</span> <span m="1044550">that</span>
  <span m="1045210">the</span> <span m="1045630">expected</span> <span m="1046170">reward</span>
  <span m="1046740">of</span> <span m="1046920">this</span> <span m="1047220">policy</span>
  <span m="1048510">is</span> <span m="1048660">not</span> <span m="1049020">a</span>
  <span m="1049080">quantity</span> <span m="1049560">that</span> <span m="1049680">we've</span>
  <span m="1049860">considered</span> <span m="1050550">in</span> <span m="1050730">the</span>
  <span m="1050850">previous</span> <span m="1051240">lectures,</span> <span m="1051970">at</span>
  <span m="1052090">least</span> <span m="1052210">not</span> <span m="1052320">in
  the</span> <span m="1052380">previous</span> <span m="1052620">lectures</span> <span
  m="1052750">in</span> <span m="1052950">causal</span> <span m="1053250">inference.</span>
  <span m="1054300">This</span> <span m="1054450">is</span> <span m="1054570">not</span>
  <span m="1054780">the</span> <span m="1054870">same</span> <span m="1055110">as</span>
  <span m="1055260">the</span> <span m="1055950">average</span> <span m="1056310">treatment</span>
  <span m="1056640">effect,</span> <span m="1056970">for</span> <span m="1057060">example.</span></p><p><span
  m="1065840">So</span> <span m="1067420">I've</span> <span m="1067570">just</span>
  <span m="1067780">given</span> <span m="1068050">you</span> <span m="1068140">one</span>
  <span m="1068470">way</span> <span m="1068680">to</span> <span m="1068770">think</span>
  <span m="1069100">through,</span> <span m="1069340">number</span> <span m="1069550">one,</span>
  <span m="1069790">what</span> <span m="1070030">is</span> <span m="1070180">the</span>
  <span m="1070300">policy</span> <span m="1071200">that</span> <span m="1071620">you</span>
  <span m="1071770">might</span> <span m="1071950">want</span> <span m="1072130">to</span>
  <span m="1072190">derive</span> <span m="1072910">when</span> <span m="1073240">you're</span>
  <span m="1073360">doing</span> <span m="1073570">causal</span> <span m="1073840">inference?</span>
  <span m="1075190">And</span> <span m="1075340">number</span> <span m="1075700">two,</span>
  <span m="1077170">what</span> <span m="1077410">is</span> <span m="1077560">one</span>
  <span m="1077860">way</span> <span m="1078070">to</span> <span m="1078160">estimate</span>
  <span m="1078760">the</span> <span m="1078880">value</span> <span m="1079360">of</span>
  <span m="1079450">that</span> <span m="1079600">policy,</span> <span m="1080890">which</span>
  <span m="1081130">goes</span> <span m="1081610">through</span> <span m="1082240">the</span>
  <span m="1082330">process</span> <span m="1083200">of</span> <span m="1085000">estimating</span>
  <span m="1085510">potential</span> <span m="1086440">outcomes</span> <span m="1087070">via</span>
  <span m="1087210">covariate</span> <span m="1087670">adjustment?</span></p><p><span
  m="1089790">But</span> <span m="1089940">we</span> <span m="1090090">might</span>
  <span m="1090270">wonder,</span> <span m="1091590">just</span> <span m="1091950">like</span>
  <span m="1092430">when</span> <span m="1092610">we</span> <span m="1092700">talked</span>
  <span m="1093030">about</span> <span m="1093980">in</span> <span m="1094240">causal
  inference</span> <span m="1094590">where</span> <span m="1094680">I</span> <span
  m="1094770">said</span> <span m="1094920">there</span> <span m="1095040">are</span>
  <span m="1095100">two</span> <span m="1095370">approaches</span> <span m="1095950">or</span>
  <span m="1096360">more</span> <span m="1096570">than</span> <span m="1096690">two,</span>
  <span m="1096840">but</span> <span m="1096960">we</span> <span m="1097110">focused</span>
  <span m="1097440">on</span> <span m="1097530">two,</span> <span m="1098190">using</span>
  <span m="1098520">covariate</span> <span m="1098760">adjustment</span> <span m="1099160">and</span>
  <span m="1099330">doing</span> <span m="1100440">inverse</span> <span m="1100710">propensity</span>
  <span m="1101070">score</span> <span m="1101310">weighting,</span> <span m="1102210">you</span>
  <span m="1102300">might</span> <span m="1102450">wonder</span> <span m="1102960">is</span>
  <span m="1103140">there</span> <span m="1103290">another</span> <span m="1103740">approach</span>
  <span m="1104130">to</span> <span m="1104280">this</span> <span m="1104490">problem</span>
  <span m="1104970">all together?</span> <span m="1106590">Is</span> <span m="1106740">there
  an</span> <span m="1106860">approach</span> <span m="1107340">which</span> <span
  m="1107550">wouldn't</span> <span m="1107880">have</span> <span m="1108000">had</span>
  <span m="1108240">to</span> <span m="1108390">go</span> <span m="1108660">through</span>
  <span m="1109320">estimating</span> <span m="1109860">the</span> <span m="1109950">potential</span>
  <span m="1110340">outcomes?</span> <span m="1112430">And</span> <span m="1112440">that's</span>
  <span m="1112620">what</span> <span m="1112710">I'll</span> <span m="1112770">spend</span>
  <span m="1113310">the</span> <span m="1113430">rest</span> <span m="1113700">of</span>
  <span m="1114170">this</span> <span m="1114600">third</span> <span m="1114900">of</span>
  <span m="1114990">the</span> <span m="1115050">lecture</span> <span m="1115590">focused</span>
  <span m="1116430">talking</span> <span m="1116760">about.</span></p><p><span m="1118960">And</span>
  <span m="1118980">so</span> <span m="1119480">to</span> <span m="1120210">help</span>
  <span m="1120450">you</span> <span m="1120570">page</span> <span m="1120960">this</span>
  <span m="1121230">back</span> <span m="1121590">in,</span> <span m="1123620">remember</span>
  <span m="1124430">that</span> <span m="1125300">we</span> <span m="1126020">derived</span>
  <span m="1126920">in</span> <span m="1127070">last</span> <span m="1127400">Thursday's</span>
  <span m="1127790">lecture</span> <span m="1128690">an</span> <span m="1128840">estimator</span>
  <span m="1129590">for</span> <span m="1129800">the</span> <span m="1129890">average</span>
  <span m="1130220">treatment</span> <span m="1130550">effect,</span> <span m="1131910">which</span>
  <span m="1132080">was</span> <span m="1133040">1</span> <span m="1133340">over</span>
  <span m="1133580">n</span> <span m="1134840">times</span> <span m="1135230">the</span>
  <span m="1135350">sum</span> <span m="1136220">over</span> <span m="1136520">data</span>
  <span m="1136820">points</span> <span m="1138230">that</span> <span m="1138590">got</span>
  <span m="1138920">treatment</span> <span m="1140620">1</span> <span m="1142460">of</span>
  <span m="1143660">yi,</span> <span m="1145400">the</span> <span m="1146270">observed</span>
  <span m="1147380">outcome</span> <span m="1148460">for</span> <span m="1148670">that</span>
  <span m="1148850">data</span> <span m="1149120">point,</span> <span m="1150200">divided</span>
  <span m="1150920">by</span> <span m="1152420">the</span> <span m="1152510">propensity</span>
  <span m="1153170">score,</span> <span m="1153500">which</span> <span m="1153710">I'm</span>
  <span m="1153830">just</span> <span m="1153980">going</span> <span m="1154190">to</span>
  <span m="1154490">write</span> <span m="1154820">as</span> <span m="1155120">ei.</span></p><p><span
  m="1155660">So</span> <span m="1156040">ei</span> <span m="1157400">is</span> <span
  m="1157640">equal</span> <span m="1158060">to</span> <span m="1158300">the</span>
  <span m="1158420">probability</span> <span m="1159830">of</span> <span m="1163160">observing</span>
  <span m="1164270">t</span> <span m="1164630">equals</span> <span m="1167240">1</span>
  <span m="1168320">given</span> <span m="1169790">the</span> <span m="1169880">data</span>
  <span m="1170120">point</span> <span m="1170510">xi</span> <span m="1174200">minus</span>
  <span m="1176760">a</span> <span m="1176880">sum</span> <span m="1177690">over</span>
  <span m="1177930">data</span> <span m="1178230">point</span> <span m="1178710">i</span>
  <span m="1179370">such</span> <span m="1179730">that</span> <span m="1180270">ti</span>
  <span m="1181170">equals</span> <span m="1181510">0</span> <span m="1182880">of</span>
  <span m="1183720">yi</span> <span m="1184800">divided</span> <span m="1185250">by</span>
  <span m="1185460">1</span> <span m="1185760">minus</span> <span m="1186330">ei.</span></p><p><span
  m="1189300">And</span> <span m="1189400">by</span> <span m="1189520">the</span>
  <span m="1189610">way,</span> <span m="1189670">there</span> <span m="1189750">was</span>
  <span m="1189850">a</span> <span m="1189880">lot</span> <span m="1190000">of</span>
  <span m="1190090">confusion</span> <span m="1190540">in</span> <span m="1190630">class</span>
  <span m="1191020">why</span> <span m="1191320">do</span> <span m="1191410">I</span>
  <span m="1191530">have</span> <span m="1192490">a</span> <span m="1192550">1</span>
  <span m="1192730">over</span> <span m="1193000">n here,</span> <span m="1193180">a
  1</span> <span m="1193300">over</span> <span m="1193370">n</span> <span m="1193540">here,</span>
  <span m="1193810">but</span> <span m="1194110">right</span> <span m="1194290">now</span>
  <span m="1194410">I</span> <span m="1194470">just</span> <span m="1194830">took</span>
  <span m="1195040">it</span> <span m="1195130">out</span> <span m="1195280">all together,</span>
  <span m="1196210">and</span> <span m="1196300">not</span> <span m="1196630">1</span>
  <span m="1196960">over</span> <span m="1197230">the</span> <span m="1197320">number</span>
  <span m="1197800">of</span> <span m="1198970">positive</span> <span m="1199570">points</span>
  <span m="1199840">and</span> <span m="1199930">1</span> <span m="1200110">over</span>
  <span m="1200260">the</span> <span m="1200350">number</span> <span m="1200620">of</span>
  <span m="1201760">0</span> <span m="1202030">data</span> <span m="1202240">points.</span>
  <span m="1203470">And</span> <span m="1203980">I</span> <span m="1204880">expanded</span>
  <span m="1205330">the</span> <span m="1205390">derivation</span> <span m="1205930">that</span>
  <span m="1206020">I</span> <span m="1206110">gave</span> <span m="1206290">in</span>
  <span m="1206380">class,</span> <span m="1206770">and I</span> <span m="1206830">posted</span>
  <span m="1207220">new</span> <span m="1207430">slides</span> <span m="1207870">online</span>
  <span m="1208420">after</span> <span m="1208780">class.</span> <span m="1209300">So</span>
  <span m="1209380">if</span> <span m="1209470">you're</span> <span m="1209590">curious</span>
  <span m="1210040">about</span> <span m="1210400">that,</span> <span m="1211030">go</span>
  <span m="1211240">to</span> <span m="1211300">those</span> <span m="1211480">slides</span>
  <span m="1211840">and</span> <span m="1211930">look</span> <span m="1212110">at</span>
  <span m="1212170">the</span> <span m="1212230">derivation.</span></p><p><span m="1215450">So</span>
  <span m="1215780">in</span> <span m="1215900">a</span> <span m="1215930">very</span>
  <span m="1216380">analogous</span> <span m="1217100">way</span> <span m="1217370">now,</span>
  <span m="1217730">I'm</span> <span m="1217850">going</span> <span m="1217930">to</span>
  <span m="1218030">give</span> <span m="1218180">you</span> <span m="1218240">a</span>
  <span m="1218300">new</span> <span m="1218630">estimator</span> <span m="1219410">for</span>
  <span m="1219770">this</span> <span m="1220000">same</span> <span m="1220460">quantity</span>
  <span m="1220980">that</span> <span m="1221180">I</span> <span m="1221300">had</span>
  <span m="1221510">over</span> <span m="1221720">here,</span> <span m="1222110">the</span>
  <span m="1222260">expected</span> <span m="1222860">reward</span> <span m="1223250">of</span>
  <span m="1223430">a</span> <span m="1223460">policy.</span> <span m="1225180">Notice</span>
  <span m="1225500">that</span> <span m="1225680">this</span> <span m="1225980">estimator</span>
  <span m="1226490">here,</span> <span m="1228680">it</span> <span m="1228800">made</span>
  <span m="1229040">sense</span> <span m="1229490">for</span> <span m="1229670">any</span>
  <span m="1229940">policy.</span> <span m="1230520">It</span> <span m="1230570">didn't</span>
  <span m="1230780">have</span> <span m="1230960">to</span> <span m="1231050">be</span>
  <span m="1231110">the</span> <span m="1231200">policy</span> <span m="1231650">which</span>
  <span m="1231830">looked</span> <span m="1232190">at,</span> <span m="1234230">is</span>
  <span m="1234560">CATE</span> <span m="1234950">just</span> <span m="1235160">greater</span>
  <span m="1235370">than</span> <span m="1235520">0</span> <span m="1235790">or</span>
  <span m="1235820">not?</span> <span m="1236150">This</span> <span m="1236390">held</span>
  <span m="1236600">for</span> <span m="1236720">any</span> <span m="1236930">policy.</span>
  <span m="1237360">The</span> <span m="1237530">simplification</span> <span m="1238370">I</span>
  <span m="1238460">gave</span> <span m="1238880">was</span> <span m="1239060">only</span>
  <span m="1239720">in</span> <span m="1239810">this</span> <span m="1239990">particular</span>
  <span m="1240440">setting.</span></p><p><span m="1242130">I'm</span> <span m="1242190">going</span>
  <span m="1242300">to</span> <span m="1242370">give</span> <span m="1242490">you</span>
  <span m="1242580">now</span> <span m="1242760">another</span> <span m="1243210">estimator</span>
  <span m="1243900">for</span> <span m="1244200">the</span> <span m="1244410">average</span>
  <span m="1245250">value</span> <span m="1245670">of</span> <span m="1245760">a</span>
  <span m="1245790">policy,</span> <span m="1246690">which</span> <span m="1246870">doesn't</span>
  <span m="1247290">go</span> <span m="1247560">through</span> <span m="1248130">estimating</span>
  <span m="1248520">potential</span> <span m="1248880">outcomes</span> <span m="1249300">at</span>
  <span m="1249420">all.</span> <span m="1251040">Analogous</span> <span m="1251940">to</span>
  <span m="1252060">this</span> <span m="1252390">is</span> <span m="1252510">just</span>
  <span m="1252780">going</span> <span m="1252990">to</span> <span m="1253350">make</span>
  <span m="1253590">use</span> <span m="1253980">of</span> <span m="1254220">the</span>
  <span m="1254340">propensity</span> <span m="1254970">scores.</span> <span m="1256690">And</span>
  <span m="1256830">I'll</span> <span m="1256920">call</span> <span m="1258830">it</span>
  <span m="1258960">R</span> <span m="1259170">hat.</span></p><p><span m="1260070">Now</span>
  <span m="1260190">I'm</span> <span m="1260250">going</span> <span m="1260370">to</span>
  <span m="1260430">put</span> <span m="1260580">a</span> <span m="1260640">superscript</span>
  <span m="1261390">IPW</span> <span m="1262170">for</span> <span m="1262350">inverse</span>
  <span m="1262620">propensity</span> <span m="1263100">weighted.</span> <span m="1263890">And</span>
  <span m="1264030">it's</span> <span m="1264120">a</span> <span m="1264180">function</span>
  <span m="1264630">of</span> <span m="1264750">pi,</span> <span m="1265890">and</span>
  <span m="1266010">it's</span> <span m="1266130">given</span> <span m="1266400">to</span>
  <span m="1266520">you by</span> <span m="1266670">the</span> <span m="1266760">following</span>
  <span m="1267180">formula--</span> <span m="1268200">1</span> <span m="1268470">over</span>
  <span m="1268800">n</span> <span m="1269970">sum</span> <span m="1270510">over</span>
  <span m="1270750">the</span> <span m="1270870">data</span> <span m="1271200">points</span>
  <span m="1273420">of</span> <span m="1273570">an</span> <span m="1273690">indicator</span>
  <span m="1274350">function</span> <span m="1275580">for</span> <span m="1276270">if</span>
  <span m="1276990">the</span> <span m="1277110">treatment,</span> <span m="1278040">which</span>
  <span m="1278250">was</span> <span m="1278400">actually</span> <span m="1278880">given</span>
  <span m="1279240">to</span> <span m="1279390">the</span> <span m="1279480">i-th</span>
  <span m="1279810">patient,</span> <span m="1280950">is</span> <span m="1281310">equal</span>
  <span m="1281790">to</span> <span m="1282660">what</span> <span m="1283140">the</span>
  <span m="1283320">policy</span> <span m="1284340">would</span> <span m="1284730">have</span>
  <span m="1285000">done</span> <span m="1285900">before</span> <span m="1286140">the</span>
  <span m="1286290">i-th</span> <span m="1286650">patient.</span></p><p><span m="1288040">And</span>
  <span m="1288180">by</span> <span m="1288300">the</span> <span m="1288390">way,</span>
  <span m="1288630">here</span> <span m="1289020">I'm</span> <span m="1289140">assuming</span>
  <span m="1289530">that</span> <span m="1289650">pi</span> <span m="1290040">is</span>
  <span m="1290220">a</span> <span m="1290340">deterministic</span> <span m="1291030">function.</span>
  <span m="1292320">So</span> <span m="1292560">the</span> <span m="1292650">policy</span>
  <span m="1293010">says</span> <span m="1293640">for</span> <span m="1293850">this</span>
  <span m="1294060">patient,</span> <span m="1294450">you</span> <span m="1294540">should</span>
  <span m="1294690">do</span> <span m="1294840">this</span> <span m="1295050">treatment.</span>
  <span m="1296760">So</span> <span m="1297360">we're</span> <span m="1297480">going</span>
  <span m="1297540">to</span> <span m="1297690">look</span> <span m="1298170">at</span>
  <span m="1298290">just</span> <span m="1298710">the</span> <span m="1298860">data</span>
  <span m="1299130">points</span> <span m="1299700">for</span> <span m="1299910">which</span>
  <span m="1300180">the</span> <span m="1300360">observed</span> <span m="1300870">treatment</span>
  <span m="1301290">is</span> <span m="1301440">consistent</span> <span m="1302400">with</span>
  <span m="1304170">what</span> <span m="1304350">the</span> <span m="1304440">policy</span>
  <span m="1304890">would</span> <span m="1305110">have</span> <span m="1305220">done</span>
  <span m="1305430">for</span> <span m="1305550">that</span> <span m="1305700">patient.</span>
  <span m="1306180">And</span> <span m="1306600">this</span> <span m="1306810">indicator</span>
  <span m="1307260">function</span> <span m="1307590">is</span> <span m="1307680">0</span>
  <span m="1307980">otherwise.</span> <span m="1308880">And</span> <span m="1309210">we're</span>
  <span m="1309300">going</span> <span m="1309380">to</span> <span m="1309450">divide</span>
  <span m="1309765">it</span> <span m="1310080">by</span> <span m="1313770">the</span>
  <span m="1313890">probability</span> <span m="1315690">of</span> <span m="1318540">ti</span>
  <span m="1320210">given</span> <span m="1320640">xi.</span></p><p><span m="1322750">So</span>
  <span m="1322960">the</span> <span m="1323080">way</span> <span m="1323260">I'm</span>
  <span m="1323350">writing</span> <span m="1323590">this,</span> <span m="1323840">by</span>
  <span m="1324100">the</span> <span m="1324190">way,</span> <span m="1325620">is</span>
  <span m="1326140">very</span> <span m="1326380">general.</span> <span m="1326860">So</span>
  <span m="1327370">this</span> <span m="1327580">formula</span> <span m="1328150">will</span>
  <span m="1328330">hold</span> <span m="1328590">for</span> <span m="1329590">nonbinary</span>
  <span m="1330430">treatments as</span> <span m="1330550">well.</span> <span m="1331270">And</span>
  <span m="1331360">that's</span> <span m="1331480">one</span> <span m="1331600">of</span>
  <span m="1331660">the</span> <span m="1331720">really</span> <span m="1331900">nice</span>
  <span m="1332110">things</span> <span m="1332320">about</span> <span m="1332500">thinking</span>
  <span m="1332740">about</span> <span m="1332890">policies,</span> <span m="1333770">which</span>
  <span m="1333850">is</span> <span m="1334120">whereas</span> <span m="1337480">when</span>
  <span m="1337750">talking</span> <span m="1338050">about</span> <span m="1338830">average</span>
  <span m="1339100">treatment</span> <span m="1339400">effect,</span> <span m="1339720">average</span>
  <span m="1339890">treatment</span> <span m="1340090">effect</span> <span m="1340430">sort</span>
  <span m="1340660">of</span> <span m="1340720">makes</span> <span m="1340930">sense</span>
  <span m="1341200">in</span> <span m="1341330">the</span> <span m="1341380">comparative</span>
  <span m="1341950">sense,</span> <span m="1342470">comparing</span> <span m="1342790">one</span>
  <span m="1343060">to</span> <span m="1343240">another.</span></p><p><span m="1344500">But</span>
  <span m="1344650">when</span> <span m="1344770">we</span> <span m="1344860">talk</span>
  <span m="1345070">about</span> <span m="1345430">how</span> <span m="1345700">good</span>
  <span m="1345940">is</span> <span m="1346090">a</span> <span m="1346150">policy,</span>
  <span m="1347590">it's</span> <span m="1348790">not</span> <span m="1348940">a</span>
  <span m="1349000">comparative</span> <span m="1349450">statement</span> <span m="1349750">at</span>
  <span m="1349810">all.</span> <span m="1350010">The</span> <span m="1350080">policy</span>
  <span m="1350410">does</span> <span m="1350590">something</span> <span m="1350980">for</span>
  <span m="1351100">everyone.</span> <span m="1351560">You</span> <span m="1351660">could</span>
  <span m="1351760">ask,</span> <span m="1351820">well,</span> <span m="1351940">what</span>
  <span m="1352090">is</span> <span m="1352210">the</span> <span m="1352360">average</span>
  <span m="1352900">value</span> <span m="1353260">of</span> <span m="1353350">the</span>
  <span m="1353440">outcomes</span> <span m="1354010">that</span> <span m="1354130">you</span>
  <span m="1354250">get</span> <span m="1354490">for</span> <span m="1354730">those</span>
  <span m="1355330">actions</span> <span m="1355690">that</span> <span m="1355780">we're</span>
  <span m="1355870">taking</span> <span m="1356170">for</span> <span m="1356260">those</span>
  <span m="1356410">individuals?</span> <span m="1358040">So</span> <span m="1358140">that's</span>
  <span m="1358180">why</span> <span m="1358240">I'm</span> <span m="1358330">writing</span>
  <span m="1358630">a</span> <span m="1358690">slightly</span> <span m="1359050">more</span>
  <span m="1359200">general</span> <span m="1359530">fashion</span> <span m="1359920">already</span>
  <span m="1360160">here.</span> <span m="1361030">Times</span> <span m="1361540">yi</span>
  <span m="1362020">obviously.</span></p><p><span m="1364660">So</span> <span m="1365080">this</span>
  <span m="1365470">is</span> <span m="1365710">now</span> <span m="1365950">a</span>
  <span m="1366010">new</span> <span m="1366220">estimator.</span> <span m="1366880">I'm</span>
  <span m="1366970">not</span> <span m="1367120">going</span> <span m="1367240">to</span>
  <span m="1367330">derive</span> <span m="1367660">it</span> <span m="1367750">for</span>
  <span m="1367900">you</span> <span m="1368050">in</span> <span m="1368140">class,</span>
  <span m="1368500">but</span> <span m="1368620">the</span> <span m="1368680">derivation</span>
  <span m="1369190">is</span> <span m="1369310">very</span> <span m="1369520">similar</span>
  <span m="1369940">to</span> <span m="1370030">what</span> <span m="1370180">we</span>
  <span m="1370300">did</span> <span m="1370540">last</span> <span m="1370960">week</span>
  <span m="1371590">when</span> <span m="1371770">we</span> <span m="1371860">tried</span>
  <span m="1372100">to</span> <span m="1372190">drive</span> <span m="1372430">the</span>
  <span m="1372490">average</span> <span m="1372700">treatment</span> <span m="1372930">effect.</span>
  <span m="1373240">And</span> <span m="1373720">the</span> <span m="1373780">critical</span>
  <span m="1374110">point</span> <span m="1374530">is</span> <span m="1375280">we're</span>
  <span m="1376120">dividing</span> <span m="1376930">by</span> <span m="1377410">that</span>
  <span m="1377650">propensity</span> <span m="1378280">score,</span> <span m="1379820">just</span>
  <span m="1380090">like</span> <span m="1380270">we</span> <span m="1380390">did</span>
  <span m="1380540">over</span> <span m="1380750">there.</span></p><p><span m="1384390">So</span>
  <span m="1385770">this,</span> <span m="1387870">if</span> <span m="1388080">all</span>
  <span m="1388390">of</span> <span m="1388470">the</span> <span m="1388530">assumptions</span>
  <span m="1389220">made</span> <span m="1389430">sense,</span> <span m="1389890">you
  had</span> <span m="1390030">infinite</span> <span m="1390360">data,</span> <span
  m="1391560">should</span> <span m="1391770">give</span> <span m="1391980">you</span>
  <span m="1392130">exactly</span> <span m="1392550">the</span> <span m="1392640">same</span>
  <span m="1392910">estimate</span> <span m="1394230">as</span> <span m="1394800">this.</span>
  <span m="1396280">But</span> <span m="1397480">here,</span> <span m="1398170">you're</span>
  <span m="1398410">not</span> <span m="1398770">estimating</span> <span m="1399310">potential</span>
  <span m="1399670">outcomes</span> <span m="1400090">at</span> <span m="1400180">all.</span>
  <span m="1400900">So</span> <span m="1401050">you</span> <span m="1401140">never</span>
  <span m="1401380">have</span> <span m="1401590">to</span> <span m="1401710">try</span>
  <span m="1401920">to</span> <span m="1402010">impute</span> <span m="1402530">the</span>
  <span m="1403150">counterfactuals.</span> <span m="1404900">Here,</span> <span m="1405340">all</span>
  <span m="1405610">it</span> <span m="1405700">relies</span> <span m="1406150">on</span>
  <span m="1406240">knowing</span> <span m="1406990">is</span> <span m="1407260">that</span>
  <span m="1407650">you</span> <span m="1407800">have</span> <span m="1408190">the</span>
  <span m="1408280">propensity</span> <span m="1408970">scores</span> <span m="1410110">for</span>
  <span m="1410260">each</span> <span m="1410410">of</span> <span m="1410470">the</span>
  <span m="1410560">data</span> <span m="1410800">points</span> <span m="1411100">in</span>
  <span m="1411190">your</span> <span m="1411250">training</span> <span m="1411580">set</span>
  <span m="1412170">or</span> <span m="1412330">in</span> <span m="1412510">a</span>
  <span m="1412540">data</span> <span m="1412800">set.</span></p><p><span m="1413620">So</span>
  <span m="1414220">for</span> <span m="1414520">example,</span> <span m="1415270">this</span>
  <span m="1415630">opens</span> <span m="1415990">the</span> <span m="1416110">door</span>
  <span m="1416380">to</span> <span m="1416530">tons</span> <span m="1417010">of</span>
  <span m="1417130">new</span> <span m="1417490">exciting</span> <span m="1417970">directions.</span>
  <span m="1420280">Imagine</span> <span m="1420680">that</span> <span m="1420800">you</span>
  <span m="1420890">had</span> <span m="1421010">a</span> <span m="1421070">very</span>
  <span m="1421460">large</span> <span m="1422480">observational</span> <span m="1422990">data</span>
  <span m="1423150">set.</span> <span m="1424610">And</span> <span m="1426020">you</span>
  <span m="1427460">learned</span> <span m="1428300">a</span> <span m="1428450">policy</span>
  <span m="1428990">from</span> <span m="1429230">it.</span> <span m="1429420">For</span>
  <span m="1429500">example,</span> <span m="1430200">you</span> <span m="1430220">might</span>
  <span m="1430460">have</span> <span m="1430670">done</span> <span m="1431600">covariate</span>
  <span m="1432110">adjustment</span> <span m="1433250">and</span> <span m="1433370">then</span>
  <span m="1433700">said,</span> <span m="1434070">OK,</span> <span m="1434630">based</span>
  <span m="1435260">on</span> <span m="1435480">covariate</span> <span m="1435770">adjustment,</span>
  <span m="1436280">this</span> <span m="1436640">is</span> <span m="1436790">my</span>
  <span m="1436910">new</span> <span m="1437060">policy.</span></p><p><span m="1438970">So</span>
  <span m="1439300">you</span> <span m="1439390">might</span> <span m="1439540">have</span>
  <span m="1439630">gotten</span> <span m="1439890">it</span> <span m="1439990">via</span>
  <span m="1440170">that</span> <span m="1440380">approach.</span> <span m="1442270">Now</span>
  <span m="1442390">you</span> <span m="1442450">want</span> <span m="1442520">to</span>
  <span m="1442590">know</span> <span m="1442720">how</span> <span m="1442900">good</span>
  <span m="1443170">is</span> <span m="1443290">that.</span> <span m="1444260">Well,</span>
  <span m="1444460">suppose</span> <span m="1444790">that</span> <span m="1444940">you</span>
  <span m="1445090">then</span> <span m="1445390">run</span> <span m="1445900">a</span>
  <span m="1445960">randomized</span> <span m="1446620">control</span> <span m="1447010">trial.</span>
  <span m="1448810">And</span> <span m="1448900">then</span> <span m="1449020">you
  run</span> <span m="1449180">a</span> <span m="1449270">randomized</span> <span
  m="1449470">control</span> <span m="1449800">trial,</span> <span m="1451030">you</span>
  <span m="1451240">have</span> <span m="1451780">100</span> <span m="1452290">people,</span>
  <span m="1452920">maybe</span> <span m="1453130">200</span> <span m="1453550">people,</span>
  <span m="1453790">and</span> <span m="1453850">so</span> <span m="1453970">not</span>
  <span m="1454240">that</span> <span m="1454420">many.</span> <span m="1455320">So</span>
  <span m="1455440">not</span> <span m="1455620">nearly</span> <span m="1456070">enough</span>
  <span m="1456280">people</span> <span m="1456550">to</span> <span m="1456670">have</span>
  <span m="1457090">actually</span> <span m="1457480">estimated</span> <span m="1458110">your</span>
  <span m="1459010">policy</span> <span m="1459640">alone.</span></p><p><span m="1460190">You</span>
  <span m="1460270">might</span> <span m="1460390">have</span> <span m="1460480">needed</span>
  <span m="1460750">thousands</span> <span m="1461260">or</span> <span m="1461320">millions</span>
  <span m="1461590">of</span> <span m="1461680">individuals</span> <span m="1462010">to</span>
  <span m="1462070">estimate</span> <span m="1462370">your</span> <span m="1462460">policy.</span>
  <span m="1463450">Now</span> <span m="1463630">you're</span> <span m="1463750">only</span>
  <span m="1463920">going</span> <span m="1463980">to</span> <span m="1464060">have</span>
  <span m="1464170">a</span> <span m="1464230">couple</span> <span m="1464490">individuals</span>
  <span m="1465280">that</span> <span m="1465370">you</span> <span m="1465460">could</span>
  <span m="1465580">actually</span> <span m="1465880">afford</span> <span m="1466210">to</span>
  <span m="1466300">do</span> <span m="1466450">a</span> <span m="1466510">randomized</span>
  <span m="1466870">control</span> <span m="1467170">trial</span> <span m="1467470">on.</span></p><p><span
  m="1468980">For</span> <span m="1469190">those</span> <span m="1469460">people,</span>
  <span m="1470120">because</span> <span m="1470510">you're</span> <span m="1470870">flipping</span>
  <span m="1471560">a</span> <span m="1471620">coin</span> <span m="1473050">for</span>
  <span m="1474110">which</span> <span m="1474350">treatment</span> <span m="1474660">they're</span>
  <span m="1474770">going</span> <span m="1474860">to</span> <span m="1474950">get,</span>
  <span m="1476210">suppose</span> <span m="1476570">that</span> <span m="1476720">were</span>
  <span m="1476840">in</span> <span m="1476960">a</span> <span m="1477020">binary</span>
  <span m="1477500">setting</span> <span m="1477800">where</span> <span m="1477920">the
  only</span> <span m="1478100">two</span> <span m="1478250">treatments,</span> <span
  m="1479100">then</span> <span m="1479180">this</span> <span m="1479450">value</span>
  <span m="1479960">is</span> <span m="1480320">always</span> <span m="1480620">1/2</span>
  <span m="1481040">1/2.</span> <span m="1482900">And</span> <span m="1483200">what</span>
  <span m="1483350">I'm</span> <span m="1483470">giving</span> <span m="1483830">you</span>
  <span m="1483950">here</span> <span m="1484370">is</span> <span m="1484670">going</span>
  <span m="1484940">to</span> <span m="1485060">be</span> <span m="1485270">an</span>
  <span m="1485480">unbiased</span> <span m="1486380">estimate</span> <span m="1487490">of</span>
  <span m="1487910">how</span> <span m="1488240">good</span> <span m="1488510">that</span>
  <span m="1488750">policy</span> <span m="1489590">is,</span> <span m="1491130">which</span>
  <span m="1491310">one</span> <span m="1491460">can</span> <span m="1491640">now</span>
  <span m="1491820">estimate</span> <span m="1492390">using</span> <span m="1492750">that</span>
  <span m="1492900">randomized</span> <span m="1493320">control</span> <span m="1493680">trial.</span></p><p><span
  m="1497350">Now,</span> <span m="1501050">this</span> <span m="1501830">also</span>
  <span m="1502220">might</span> <span m="1502430">lead</span> <span m="1502760">you</span>
  <span m="1502880">to</span> <span m="1502970">think</span> <span m="1503300">through</span>
  <span m="1503780">the</span> <span m="1503840">question</span> <span m="1504290">of,</span>
  <span m="1504620">well,</span> <span m="1505100">rather</span> <span m="1505640">than</span>
  <span m="1506480">estimating</span> <span m="1506930">the</span> <span m="1507020">policy</span>
  <span m="1508700">through--</span> <span m="1510230">rather</span> <span m="1510440">than</span>
  <span m="1510560">obtaining</span> <span m="1510890">a</span> <span m="1510950">policy</span>
  <span m="1511400">through</span> <span m="1511670">the</span> <span m="1511760">lens</span>
  <span m="1512120">of</span> <span m="1512850">optimizing</span> <span m="1514250">CATE,</span>
  <span m="1515636">of</span> <span m="1516030">figuring</span> <span m="1516440">how</span>
  <span m="1516530">to</span> <span m="1516620">estimate</span> <span m="1517010">CATE,</span>
  <span m="1517880">maybe</span> <span m="1518390">we</span> <span m="1518540">could</span>
  <span m="1518810">have</span> <span m="1519020">skipped</span> <span m="1519590">that</span>
  <span m="1519860">all together.</span></p><p><span m="1521370">For</span> <span
  m="1521450">example,</span> <span m="1524030">suppose</span> <span m="1524420">that</span>
  <span m="1524540">we</span> <span m="1524660">had</span> <span m="1524870">that</span>
  <span m="1525230">randomized</span> <span m="1525710">control</span> <span m="1526070">trial</span>
  <span m="1526280">data.</span> <span m="1526670">Now</span> <span m="1526940">imagine</span>
  <span m="1527330">that</span> <span m="1527480">rather</span> <span m="1527750">than</span>
  <span m="1529420">100</span> <span m="1529760">individuals,</span> <span m="1530240">you</span>
  <span m="1530330">had</span> <span m="1530870">a</span> <span m="1530900">really</span>
  <span m="1531320">large</span> <span m="1531590">randomized</span> <span m="1531980">control</span>
  <span m="1532260">trial</span> <span m="1532500">with</span> <span m="1532640">10,000</span>
  <span m="1533180">individuals</span> <span m="1533600">in</span> <span m="1533690">it.</span></p><p><span
  m="1535640">This</span> <span m="1536030">now</span> <span m="1536240">opens</span>
  <span m="1536630">the</span> <span m="1536750">door</span> <span m="1537470">to</span>
  <span m="1537620">thinking</span> <span m="1538070">about</span> <span m="1539060">directly</span>
  <span m="1541010">maximizing</span> <span m="1541940">or</span> <span m="1542000">minimizing,</span>
  <span m="1542480">depending</span> <span m="1543500">whether</span> <span m="1543560">you</span>
  <span m="1543620">want</span> <span m="1543740">this</span> <span m="1543830">to</span>
  <span m="1543890">be</span> <span m="1543980">large</span> <span m="1544160">or</span>
  <span m="1544250">small,</span> <span m="1544760">pi</span> <span m="1546070">with</span>
  <span m="1546260">respect</span> <span m="1546590">to</span> <span m="1546710">this</span>
  <span m="1546950">quantity,</span> <span m="1549090">which</span> <span m="1549410">completely</span>
  <span m="1549980">bypasses</span> <span m="1550820">the</span> <span m="1550910">goal</span>
  <span m="1551360">of</span> <span m="1551630">estimating</span> <span m="1552380">the</span>
  <span m="1553520">condition</span> <span m="1553830">of average</span> <span m="1554030">treatment</span>
  <span m="1554300">effect.</span></p><p><span m="1556190">And</span> <span m="1556410">you'll</span>
  <span m="1556520">notice</span> <span m="1556940">how</span> <span m="1557330">this</span>
  <span m="1557720">looks</span> <span m="1557990">exactly</span> <span m="1558530">like</span>
  <span m="1558860">a</span> <span m="1558920">classification</span> <span m="1559730">problem.</span>
  <span m="1560390">This</span> <span m="1560630">quantity</span> <span m="1561020">here</span>
  <span m="1561260">looks</span> <span m="1561410">exactly</span> <span m="1561890">like</span>
  <span m="1562160">a</span> <span m="1562220">0</span> <span m="1562580">1</span>
  <span m="1562850">loss.</span> <span m="1564450">And</span> <span m="1564540">the</span>
  <span m="1564600">only</span> <span m="1564840">difference</span> <span m="1565380">is</span>
  <span m="1565740">that</span> <span m="1566040">you're</span> <span m="1566280">weighting</span>
  <span m="1567150">each</span> <span m="1567360">of</span> <span m="1567420">the</span>
  <span m="1567510">data</span> <span m="1567780">points</span> <span m="1568140">by</span>
  <span m="1568470">this</span> <span m="1569350">inverse</span> <span m="1569640">propensity.</span></p><p><span
  m="1572640">So</span> <span m="1573450">one</span> <span m="1573690">can</span>
  <span m="1573870">reduce</span> <span m="1574560">the</span> <span m="1574680">problem</span>
  <span m="1575280">of</span> <span m="1575460">actually</span> <span m="1576780">finding</span>
  <span m="1577260">an</span> <span m="1577410">optimal</span> <span m="1577920">policy</span>
  <span m="1578640">here</span> <span m="1579240">to</span> <span m="1579390">that</span>
  <span m="1579570">of</span> <span m="1579690">a</span> <span m="1579790">weighted</span>
  <span m="1580380">classification</span> <span m="1581250">problem,</span> <span
  m="1581880">in</span> <span m="1581970">the</span> <span m="1582030">case</span>
  <span m="1582240">of</span> <span m="1583160">a</span> <span m="1583290">discrete</span>
  <span m="1583920">set</span> <span m="1584160">of</span> <span m="1584250">treatments.</span>
  <span m="1588370">There</span> <span m="1588490">are</span> <span m="1588610">two</span>
  <span m="1588910">big</span> <span m="1589150">caveats</span> <span m="1589720">to</span>
  <span m="1589810">that</span> <span m="1589960">line</span> <span m="1590170">of</span>
  <span m="1590260">thinking.</span> <span m="1591010">The</span> <span m="1591130">first</span>
  <span m="1591430">major</span> <span m="1591730">caveat</span> <span m="1592450">is</span>
  <span m="1592660">that</span> <span m="1595470">you</span> <span m="1596790">have</span>
  <span m="1597090">to</span> <span m="1597210">know</span> <span m="1597510">these</span>
  <span m="1597660">propensity</span> <span m="1598140">scores.</span></p><p><span
  m="1601720">And</span> <span m="1601810">so</span> <span m="1603040">if</span> <span
  m="1603220">you</span> <span m="1603400">have</span> <span m="1604120">data</span>
  <span m="1604450">coming</span> <span m="1604690">from randomized</span> <span m="1605620">control</span>
  <span m="1605920">trial,</span> <span m="1606700">you</span> <span m="1606820">will</span>
  <span m="1606970">know</span> <span m="1607180">this</span> <span m="1607330">propensity</span>
  <span m="1607790">scores</span> <span m="1608570">or</span> <span m="1609130">if</span>
  <span m="1609220">you</span> <span m="1609340">have,</span> <span m="1609580">for</span>
  <span m="1609670">example,</span> <span m="1609940">some</span> <span m="1610120">control</span>
  <span m="1610750">over</span> <span m="1611350">the</span> <span m="1612430">data</span>
  <span m="1612970">generation</span> <span m="1613510">process.</span> <span m="1614290">For</span>
  <span m="1614350">example,</span> <span m="1614810">if</span> <span m="1614830">you</span>
  <span m="1615130">are</span> <span m="1615580">an</span> <span m="1615880">ad</span>
  <span m="1616150">company</span> <span m="1617140">and</span> <span m="1618910">you</span>
  <span m="1619000">get</span> <span m="1619150">to</span> <span m="1619210">choose</span>
  <span m="1619570">which</span> <span m="1619750">ad</span> <span m="1620050">to</span>
  <span m="1620230">show</span> <span m="1621010">to</span> <span m="1621130">your</span>
  <span m="1621220">customers,</span> <span m="1621860">then</span> <span m="1621880">you</span>
  <span m="1621970">look</span> <span m="1622090">to</span> <span m="1622180">see</span>
  <span m="1622420">who</span> <span m="1622570">clicks</span> <span m="1622900">on</span>
  <span m="1623050">what,</span> <span m="1623920">you</span> <span m="1624040">might</span>
  <span m="1624250">know</span> <span m="1624520">what</span> <span m="1624730">that</span>
  <span m="1624910">policy</span> <span m="1625390">was</span> <span m="1625600">that</span>
  <span m="1625720">was</span> <span m="1625870">showing</span> <span m="1626230">things.</span>
  <span m="1626740">In</span> <span m="1626800">that</span> <span m="1626920">case,</span>
  <span m="1627200">you</span> <span m="1627300">might</span> <span m="1627340">exactly</span>
  <span m="1627850">know</span> <span m="1627970">the</span> <span m="1628030">propensity</span>
  <span m="1628480">scores.</span></p><p><span m="1629890">In</span> <span m="1630030">health</span>
  <span m="1630210">care,</span> <span m="1631420">other</span> <span m="1631690">than</span>
  <span m="1631850">in</span> <span m="1631940">randomized</span> <span m="1632200">control</span>
  <span m="1632440">trials,</span> <span m="1632680">we</span> <span m="1632770">typically</span>
  <span m="1633130">don't</span> <span m="1633370">know</span> <span m="1633550">this</span>
  <span m="1633790">value.</span> <span m="1634390">So</span> <span m="1635080">we</span>
  <span m="1635230">either</span> <span m="1635530">have</span> <span m="1635680">to</span>
  <span m="1635770">have</span> <span m="1635890">a</span> <span m="1635950">large</span>
  <span m="1636340">enough</span> <span m="1636640">randomized</span> <span m="1637030">control</span>
  <span m="1637330">trial</span> <span m="1638020">that</span> <span m="1638170">we</span>
  <span m="1638320">won't</span> <span m="1638680">over-fit</span> <span m="1640210">by</span>
  <span m="1640750">trying</span> <span m="1641050">to</span> <span m="1641140">directly</span>
  <span m="1641530">minimize</span> <span m="1642010">this</span> <span m="1643390">or</span>
  <span m="1644980">we</span> <span m="1645130">have</span> <span m="1645370">to</span>
  <span m="1645550">work</span> <span m="1645790">within</span> <span m="1646090">an</span>
  <span m="1646210">observational</span> <span m="1647080">data</span> <span m="1647380">setting.</span></p><p><span
  m="1647740">But</span> <span m="1647860">we</span> <span m="1647950">have</span>
  <span m="1648100">to</span> <span m="1648220">estimate</span> <span m="1648700">the</span>
  <span m="1648790">propensity</span> <span m="1649300">scores</span> <span m="1649630">directly.</span>
  <span m="1651190">So</span> <span m="1651340">you</span> <span m="1651550">would
  then</span> <span m="1651730">have</span> <span m="1651850">a</span> <span m="1651910">two-step</span>
  <span m="1652330">procedure,</span> <span m="1652750">where</span> <span m="1652870">first</span>
  <span m="1653200">you</span> <span m="1653320">estimate</span> <span m="1653770">these</span>
  <span m="1653890">propensity</span> <span m="1654250">scores,</span> <span m="1654940">for</span>
  <span m="1655090">example,</span> <span m="1655520">by</span> <span m="1655540">doing</span>
  <span m="1655780">logistic</span> <span m="1656140">regression.</span> <span m="1657220">And</span>
  <span m="1657850">then</span> <span m="1658720">you</span> <span m="1658840">attempt</span>
  <span m="1659140">to</span> <span m="1659680">maximize</span> <span m="1660100">or</span>
  <span m="1660160">minimize</span> <span m="1660640">this</span> <span m="1660820">quantity</span>
  <span m="1661780">in</span> <span m="1661900">order</span> <span m="1662020">to</span>
  <span m="1662110">find</span> <span m="1662420">the</span> <span m="1662500">optimal</span>
  <span m="1662860">policy.</span></p><p><span m="1665890">And</span> <span m="1666030">that</span>
  <span m="1666360">has</span> <span m="1667200">a</span> <span m="1667260">lot</span>
  <span m="1667530">of</span> <span m="1667620">challenges,</span> <span m="1668400">because</span>
  <span m="1669450">this</span> <span m="1669930">quantity</span> <span m="1670380">shown</span>
  <span m="1670620">in</span> <span m="1670680">the</span> <span m="1670740">very</span>
  <span m="1670950">bottom</span> <span m="1671370">here</span> <span m="1672090">could</span>
  <span m="1672390">be</span> <span m="1672690">really</span> <span m="1673050">small</span>
  <span m="1673380">or</span> <span m="1673440">really</span> <span m="1673710">large</span>
  <span m="1674160">in an</span> <span m="1674310">observational</span> <span m="1675570">data</span>
  <span m="1675840">set</span> <span m="1676230">due</span> <span m="1676500">to</span>
  <span m="1676740">these</span> <span m="1676950">issues</span> <span m="1677370">of</span>
  <span m="1678150">having</span> <span m="1678480">very</span> <span m="1678750">small</span>
  <span m="1679110">overlap</span> <span m="1679590">between</span> <span m="1680460">your</span>
  <span m="1680610">treatments.</span></p><p><span m="1681990">And</span> <span m="1682260">this</span>
  <span m="1682560">being</span> <span m="1682830">very</span> <span m="1683100">small</span>
  <span m="1684270">implies</span> <span m="1684990">then</span> <span m="1685200">that</span>
  <span m="1685320">the</span> <span m="1685470">variant</span> <span m="1686130">of</span>
  <span m="1686190">this</span> <span m="1686400">estimator</span> <span m="1687060">is</span>
  <span m="1687300">very,</span> <span m="1687700">very</span> <span m="1687900">large.</span>
  <span m="1690120">And</span> <span m="1690630">so</span> <span m="1691170">when</span>
  <span m="1691410">one</span> <span m="1691590">wants</span> <span m="1691800">to</span>
  <span m="1691890">use</span> <span m="1692250">an</span> <span m="1692340">approach</span>
  <span m="1692670">like</span> <span m="1692910">this,</span> <span m="1693570">similar</span>
  <span m="1694050">to</span> <span m="1694410">when</span> <span m="1694620">one</span>
  <span m="1694770">wants</span> <span m="1694920">to</span> <span m="1694980">use</span>
  <span m="1695310">an</span> <span m="1695430">average</span> <span m="1695670">treatment</span>
  <span m="1695910">effect</span> <span m="1696240">estimator,</span> <span m="1697560">and</span>
  <span m="1697980">when</span> <span m="1698130">you're</span> <span m="1698220">estimating</span>
  <span m="1698820">these</span> <span m="1699150">propensities,</span> <span m="1699870">often</span>
  <span m="1700200">you</span> <span m="1700260">might</span> <span m="1700680">need</span>
  <span m="1700860">to</span> <span m="1700920">do</span> <span m="1701070">things</span>
  <span m="1701340">like</span> <span m="1701490">clipping</span> <span m="1702240">of</span>
  <span m="1702450">the</span> <span m="1702540">propensity</span> <span m="1703090">scores</span>
  <span m="1703620">in</span> <span m="1703740">order</span> <span m="1703920">to</span>
  <span m="1704100">prevent</span> <span m="1704520">the</span> <span m="1704610">variants</span>
  <span m="1705120">from</span> <span m="1705300">being</span> <span m="1705480">too</span>
  <span m="1705630">large.</span> <span m="1706110">That</span> <span m="1706320">then,</span>
  <span m="1706590">however,</span> <span m="1706920">leads</span> <span m="1707190">to</span>
  <span m="1707340">a</span> <span m="1707430">biased</span> <span m="1707940">estimate</span>
  <span m="1708470">typically.</span></p><p><span m="1711420">I</span> <span m="1711480">wanted</span>
  <span m="1711660">to</span> <span m="1711720">give</span> <span m="1711810">you</span>
  <span m="1711870">a</span> <span m="1711900">couple</span> <span m="1712170">of</span>
  <span m="1712260">references</span> <span m="1712800">here.</span> <span m="1713800">So</span>
  <span m="1714210">one</span> <span m="1714750">is</span> <span m="1717760">Swaminathan</span>
  <span m="1721530">and</span> <span m="1723120">Joachims,</span> <span m="1725530">J-O-A-C-H-I-M-S</span>
  <span m="1729766">ACML</span> <span m="1731380">2015.</span> <span m="1735250">In</span>
  <span m="1735340">that</span> <span m="1735490">paper,</span> <span m="1736240">they</span>
  <span m="1736660">tackle</span> <span m="1737200">this</span> <span m="1737410">question.</span>
  <span m="1738370">They</span> <span m="1738550">focus</span> <span m="1738910">on</span>
  <span m="1739000">the</span> <span m="1739060">setting</span> <span m="1739330">where</span>
  <span m="1739420">the</span> <span m="1739480">propensity</span> <span m="1739900">scores</span>
  <span m="1740200">are</span> <span m="1740290">known,</span> <span m="1740590">such</span>
  <span m="1740830">as</span> <span m="1741010">do it</span> <span m="1741100">half</span>
  <span m="1741280">from</span> <span m="1741430">a</span> <span m="1741490">randomized</span>
  <span m="1741820">controlled</span> <span m="1742150">trial.</span> <span m="1743470">And</span>
  <span m="1743980">they</span> <span m="1744130">recognize</span> <span m="1744880">that</span>
  <span m="1745720">you</span> <span m="1745960">might</span> <span m="1746380">decide</span>
  <span m="1746950">that</span> <span m="1747490">you</span> <span m="1747580">prefer</span>
  <span m="1748150">something</span> <span m="1748450">like</span> <span m="1748570">a</span>
  <span m="1748630">biased</span> <span m="1749050">estimator</span> <span m="1749450">because</span>
  <span m="1749710">of</span> <span m="1749770">the</span> <span m="1749830">fact</span>
  <span m="1750070">that</span> <span m="1750190">these</span> <span m="1750310">propensity</span>
  <span m="1750690">scores</span> <span m="1751030">could</span> <span m="1751120">be</span>
  <span m="1751210">really</span> <span m="1751390">small.</span></p><p><span m="1752650">And</span>
  <span m="1752740">so</span> <span m="1752860">they</span> <span m="1753010">use</span>
  <span m="1753550">some</span> <span m="1753820">generalization</span> <span m="1754570">results</span>
  <span m="1755110">from</span> <span m="1755290">the</span> <span m="1755380">machine</span>
  <span m="1755710">learning</span> <span m="1756220">theory</span> <span m="1756790">community</span>
  <span m="1758080">in</span> <span m="1758200">order</span> <span m="1758320">to</span>
  <span m="1758440">try</span> <span m="1758620">to</span> <span m="1758710">control</span>
  <span m="1759640">the</span> <span m="1759760">variants</span> <span m="1760450">of</span>
  <span m="1760600">the</span> <span m="1761064">estimator</span> <span m="1762456">as</span>
  <span m="1762920">a</span> <span m="1762980">function</span> <span m="1763430">of</span>
  <span m="1763550">these</span> <span m="1763820">propensity</span> <span m="1764390">scores.</span>
  <span m="1765440">And</span> <span m="1765950">they</span> <span m="1766130">then</span>
  <span m="1766520">learn,</span> <span m="1767090">directly</span> <span m="1767570">minimize</span>
  <span m="1768140">the</span> <span m="1768230">policy</span> <span m="1768680">which</span>
  <span m="1768800">is</span> <span m="1768890">what</span> <span m="1768980">they</span>
  <span m="1769070">call</span> <span m="1769280">counterfactual</span> <span m="1770030">regret</span>
  <span m="1770460">minimization,</span> <span m="1773570">in</span> <span m="1773690">order</span>
  <span m="1773870">to</span> <span m="1774620">allow</span> <span m="1774950">one</span>
  <span m="1775160">to</span> <span m="1775310">generalize</span> <span m="1775880">as</span>
  <span m="1776000">best</span> <span m="1776210">as</span> <span m="1776300">possible</span>
  <span m="1776630">from</span> <span m="1777110">the</span> <span m="1777230">small</span>
  <span m="1777530">amount</span> <span m="1777710">of</span> <span m="1777800">data</span>
  <span m="1777980">you</span> <span m="1778040">might</span> <span m="1778190">have</span>
  <span m="1778340">available.</span></p><p><span m="1780030">A</span> <span m="1780100">second</span>
  <span m="1780460">reference</span> <span m="1780940">that</span> <span m="1781030">I</span>
  <span m="1781090">want</span> <span m="1781240">to</span> <span m="1781300">give</span>
  <span m="1781840">just</span> <span m="1782110">to</span> <span m="1782230">point</span>
  <span m="1782530">you</span> <span m="1782680">into</span> <span m="1782850">this</span>
  <span m="1783010">literature,</span> <span m="1783340">if</span> <span m="1783410">you're</span>
  <span m="1783460">interested,</span> <span m="1784450">is</span> <span m="1784750">by</span>
  <span m="1785290">Nathan</span> <span m="1785680">Kallus</span> <span m="1786670">and</span>
  <span m="1787240">his</span> <span m="1787420">student,</span> <span m="1789030">I</span>
  <span m="1789090">believe</span> <span m="1789300">Angela</span> <span m="1789650">Zhou,</span>
  <span m="1790350">from</span> <span m="1791030">NeurIPS</span> <span m="1792220">2018.</span>
  <span m="1795960">And</span> <span m="1796620">that</span> <span m="1796800">was</span>
  <span m="1796950">a</span> <span m="1797010">paper</span> <span m="1797250">which</span>
  <span m="1797430">was</span> <span m="1797580">one</span> <span m="1797700">of</span>
  <span m="1797760">the</span> <span m="1797850">optional</span> <span m="1798150">readings</span>
  <span m="1798510">for</span> <span m="1798630">last</span> <span m="1798870">Thursday's</span>
  <span m="1799290">class.</span> <span m="1800490">Now,</span> <span m="1800580">that</span>
  <span m="1800760">paper</span> <span m="1801030">they</span> <span m="1801180">also</span>
  <span m="1801480">start</span> <span m="1801840">from</span> <span m="1802020">something</span>
  <span m="1802320">like</span> <span m="1802530">this,</span> <span m="1802770">from</span>
  <span m="1802920">this</span> <span m="1803070">perspective.</span></p><p><span
  m="1804300">And</span> <span m="1804420">they</span> <span m="1804570">say</span>
  <span m="1804870">that,</span> <span m="1805260">oh,</span> <span m="1805590">now</span>
  <span m="1805830">that</span> <span m="1807060">we're</span> <span m="1807300">working</span>
  <span m="1807630">in</span> <span m="1807720">this</span> <span m="1807990">framework,</span>
  <span m="1809160">one</span> <span m="1809370">could</span> <span m="1809490">think</span>
  <span m="1809670">about</span> <span m="1809850">what</span> <span m="1810030">happens</span>
  <span m="1810630">if</span> <span m="1810780">you</span> <span m="1810960">have</span>
  <span m="1811410">actually</span> <span m="1812340">unobserved</span> <span m="1812880">confounding.</span>
  <span m="1814820">So</span> <span m="1814930">there,</span> <span m="1815230">you</span>
  <span m="1815380">might</span> <span m="1815650">not</span> <span m="1815920">actually</span>
  <span m="1816280">know</span> <span m="1816760">the</span> <span m="1816910">true</span>
  <span m="1817120">propensity</span> <span m="1817700">scores,</span> <span m="1818290">because</span>
  <span m="1818920">there</span> <span m="1819160">are</span> <span m="1819370">unobserved</span>
  <span m="1819970">confounders</span> <span m="1820720">that</span> <span m="1820840">you</span>
  <span m="1820960">don't</span> <span m="1821260">observe.</span> <span m="1822650">And</span>
  <span m="1823240">that</span> <span m="1823470">you</span> <span m="1823630">can</span>
  <span m="1823780">think</span> <span m="1824020">about</span> <span m="1824230">trying</span>
  <span m="1824530">to</span> <span m="1824740">bound</span> <span m="1825520">how</span>
  <span m="1826660">wrong</span> <span m="1827380">your</span> <span m="1827750">estimator</span>
  <span m="1828310">can</span> <span m="1828580">be</span> <span m="1828820">as</span>
  <span m="1828940">a</span> <span m="1829000">function</span> <span m="1829420">of</span>
  <span m="1829570">how</span> <span m="1829840">much</span> <span m="1830080">you</span>
  <span m="1830170">don't</span> <span m="1830440">know</span> <span m="1830650">this</span>
  <span m="1830830">quantity.</span></p><p><span m="1832180">And</span> <span m="1832270">they</span>
  <span m="1832390">show</span> <span m="1832660">that</span> <span m="1832900">when</span>
  <span m="1833140">you</span> <span m="1833440">try</span> <span m="1833770">to--</span>
  <span m="1834430">if</span> <span m="1834550">you</span> <span m="1834610">think</span>
  <span m="1834850">about</span> <span m="1835030">having</span> <span m="1835420">some</span>
  <span m="1835630">backup</span> <span m="1836020">strategy,</span> <span m="1836620">like</span>
  <span m="1836890">if</span> <span m="1838000">your</span> <span m="1838270">goal</span>
  <span m="1838630">is</span> <span m="1838750">to</span> <span m="1838870">find</span>
  <span m="1839890">a</span> <span m="1840040">new</span> <span m="1840310">policy</span>
  <span m="1840880">which</span> <span m="1841040">performs</span> <span m="1841480">as</span>
  <span m="1841630">best</span> <span m="1841930">as</span> <span m="1842050">possible</span>
  <span m="1843190">with</span> <span m="1844240">respect</span> <span m="1844750">to</span>
  <span m="1845050">an</span> <span m="1845200">old</span> <span m="1845470">policy,</span>
  <span m="1846730">then</span> <span m="1846970">it</span> <span m="1847060">gives</span>
  <span m="1847300">you</span> <span m="1847360">a</span> <span m="1847390">really</span>
  <span m="1847750">elegant</span> <span m="1848140">framework</span> <span m="1848620">for</span>
  <span m="1848740">trying</span> <span m="1848980">to</span> <span m="1849100">think</span>
  <span m="1849280">about</span> <span m="1849430">a</span> <span m="1849490">robust</span>
  <span m="1850030">optimization</span> <span m="1850960">of</span> <span m="1851140">this,</span>
  <span m="1851800">even</span> <span m="1852100">taking</span> <span m="1852370">into</span>
  <span m="1852430">consideration</span> <span m="1852970">the</span> <span m="1853060">fact</span>
  <span m="1853270">that</span> <span m="1853360">there</span> <span m="1853440">might</span>
  <span m="1853570">be</span> <span m="1853690">unobserved</span> <span m="1854040">confounding.</span>
  <span m="1854870">And</span> <span m="1854980">that</span> <span m="1855130">works</span>
  <span m="1855490">also</span> <span m="1855850">in</span> <span m="1856270">this</span>
  <span m="1856420">framework.</span></p><p><span m="1859040">So</span> <span m="1859280">I'm</span>
  <span m="1859370">nearly</span> <span m="1859700">done</span> <span m="1859920">now.</span>
  <span m="1863700">I</span> <span m="1863730">just</span> <span m="1863850">want</span>
  <span m="1864000">to</span> <span m="1864060">now</span> <span m="1864240">finish</span>
  <span m="1864630">with</span> <span m="1864770">a</span> <span m="1864820">thought,</span>
  <span m="1865110">can</span> <span m="1865320">we</span> <span m="1865410">do</span>
  <span m="1865530">the</span> <span m="1865620">same</span> <span m="1866040">thing</span>
  <span m="1866580">for</span> <span m="1866790">policies</span> <span m="1867360">learned</span>
  <span m="1867570">by</span> <span m="1867690">reinforcement</span> <span m="1868290">learning?</span>
  <span m="1869710">So</span> <span m="1869760">now</span> <span m="1870660">that</span>
  <span m="1870810">we've</span> <span m="1870990">sort</span> <span m="1871170">of</span>
  <span m="1871260">built</span> <span m="1871620">up</span> <span m="1871710">this</span>
  <span m="1871920">language</span> <span m="1872400">that's</span> <span m="1872610">returned</span>
  <span m="1873330">to</span> <span m="1873570">the</span> <span m="1873660">RL</span>
  <span m="1874020">setting.</span></p><p><span m="1875850">And</span> <span m="1875970">there</span>
  <span m="1876660">one</span> <span m="1876870">can</span> <span m="1877050">show</span>
  <span m="1877710">that</span> <span m="1878790">you</span> <span m="1878880">can</span>
  <span m="1879030">get</span> <span m="1879150">a</span> <span m="1879210">similar</span>
  <span m="1879750">estimate</span> <span m="1880260">for</span> <span m="1880410">the</span>
  <span m="1880500">value</span> <span m="1880830">of</span> <span m="1880920">a</span>
  <span m="1880950">policy</span> <span m="1882900">by</span> <span m="1883890">summing</span>
  <span m="1884550">over</span> <span m="1885360">your</span> <span m="1885600">observed</span>
  <span m="1886300">sequences,</span> <span m="1887520">summing</span> <span m="1888180">over</span>
  <span m="1888840">the</span> <span m="1889620">time</span> <span m="1890070">steps</span>
  <span m="1890580">of</span> <span m="1890730">that</span> <span m="1890910">sequence</span>
  <span m="1892230">of</span> <span m="1892530">the</span> <span m="1892680">reward</span>
  <span m="1895080">observed</span> <span m="1896130">at</span> <span m="1896370">that</span>
  <span m="1896730">time</span> <span m="1897090">step</span> <span m="1898200">times</span>
  <span m="1900460">a</span> <span m="1900520">ratio</span> <span m="1901150">of</span>
  <span m="1901210">probabilities,</span> <span m="1902450">which</span> <span m="1902590">is</span>
  <span m="1903460">going</span> <span m="1903850">from</span> <span m="1905260">the</span>
  <span m="1905500">first</span> <span m="1905860">time</span> <span m="1906130">step</span>
  <span m="1906610">up</span> <span m="1906820">to</span> <span m="1907390">time</span>
  <span m="1907880">little</span> <span m="1908170">t</span> <span m="1909700">of</span>
  <span m="1911660">the</span> <span m="1912200">probability</span> <span m="1913430">that</span>
  <span m="1914270">you</span> <span m="1914480">would</span> <span m="1914690">actually</span>
  <span m="1915140">take</span> <span m="1915530">the</span> <span m="1915680">observed</span>
  <span m="1916220">action</span> <span m="1917260">t</span> <span m="1917570">prime,</span>
  <span m="1918350">given</span> <span m="1918680">that</span> <span m="1918860">you</span>
  <span m="1919020">are</span> <span m="1919160">in</span> <span m="1919340">the</span>
  <span m="1919460">observed</span> <span m="1919880">state</span> <span m="1920720">t</span>
  <span m="1920990">prime,</span> <span m="1922100">divided</span> <span m="1922760">by</span>
  <span m="1924920">the</span> <span m="1925020">probability--</span> <span m="1926370">this</span>
  <span m="1927150">is</span> <span m="1927240">the</span> <span m="1927300">analogy</span>
  <span m="1927630">of the</span> <span m="1927690">propensity</span> <span m="1928200">score,</span>
  <span m="1928470">the</span> <span m="1928560">probability</span> <span m="1929040">under</span>
  <span m="1929220">the</span> <span m="1929310">data</span> <span m="1929610">generating</span>
  <span m="1930090">process--</span> <span m="1931500">of</span> <span m="1934980">seeing</span>
  <span m="1936180">action</span> <span m="1936720">a</span> <span m="1937740">given</span>
  <span m="1937980">that</span> <span m="1938130">you</span> <span m="1938260">are</span>
  <span m="1938370">in</span> <span m="1938460">state</span> <span m="1938940">t</span>
  <span m="1939240">prime.</span></p><p><span m="1941190">So</span> <span m="1941460">if,</span>
  <span m="1942060">as</span> <span m="1942300">we</span> <span m="1942420">discussed</span>
  <span m="1942840">there,</span> <span m="1943200">you</span> <span m="1943380">had</span>
  <span m="1943560">a</span> <span m="1943620">deterministic</span> <span m="1944730">policy,</span>
  <span m="1945960">then</span> <span m="1946620">this</span> <span m="1947010">pi,</span>
  <span m="1947940">it</span> <span m="1948300">would</span> <span m="1948450">just</span>
  <span m="1948630">be</span> <span m="1948720">a</span> <span m="1948780">delta</span>
  <span m="1949110">function.</span> <span m="1949660">And</span> <span m="1949680">so</span>
  <span m="1950730">this</span> <span m="1951090">would</span> <span m="1951240">just</span>
  <span m="1951540">be</span> <span m="1951720">looking</span> <span m="1952260">at--</span>
  <span m="1954030">this</span> <span m="1954210">estimator</span> <span m="1954680">would</span>
  <span m="1954840">only</span> <span m="1955140">be</span> <span m="1955260">looking</span>
  <span m="1955680">at</span> <span m="1955880">sequences</span> <span m="1957150">where</span>
  <span m="1957450">the</span> <span m="1957930">precise</span> <span m="1958770">sequence</span>
  <span m="1959550">of</span> <span m="1959760">actions</span> <span m="1960330">taken</span>
  <span m="1960960">are</span> <span m="1961140">identical</span> <span m="1962040">to</span>
  <span m="1962160">the</span> <span m="1962250">precise</span> <span m="1963150">sequence</span>
  <span m="1963540">of</span> <span m="1963630">actions</span> <span m="1964080">that</span>
  <span m="1964170">the</span> <span m="1964230">policy</span> <span m="1964680">would</span>
  <span m="1964820">have</span> <span m="1964920">taken.</span></p><p><span m="1967790">And</span>
  <span m="1967910">the</span> <span m="1968000">difference</span> <span m="1968420">here</span>
  <span m="1968720">is</span> <span m="1968810">that</span> <span m="1968960">now</span>
  <span m="1969440">instead</span> <span m="1969740">of</span> <span m="1969830">having</span>
  <span m="1970250">a</span> <span m="1970400">single</span> <span m="1970820">propensity</span>
  <span m="1971390">score,</span> <span m="1972230">one</span> <span m="1972410">has</span>
  <span m="1972590">a</span> <span m="1972650">product</span> <span m="1973370">of</span>
  <span m="1973490">these</span> <span m="1973790">propensity</span> <span m="1974450">scores</span>
  <span m="1975350">corresponding</span> <span m="1976010">to</span> <span m="1976460">the</span>
  <span m="1976970">propensity</span> <span m="1977750">of</span> <span m="1978440">observing</span>
  <span m="1979190">that</span> <span m="1979490">action</span> <span m="1980000">given</span>
  <span m="1980360">the</span> <span m="1980450">corresponding</span> <span m="1981110">state</span>
  <span m="1981620">at</span> <span m="1981860">each</span> <span m="1982100">point</span>
  <span m="1982430">along</span> <span m="1982670">the</span> <span m="1982730">sequence.</span></p><p><span
  m="1984240">And</span> <span m="1984320">so</span> <span m="1984800">this</span>
  <span m="1985010">is</span> <span m="1985130">nice,</span> <span m="1985460">because</span>
  <span m="1985700">this</span> <span m="1985850">gives</span> <span m="1986120">you</span>
  <span m="1986210">one</span> <span m="1986510">way</span> <span m="1986720">to</span>
  <span m="1986840">do</span> <span m="1987050">what's</span> <span m="1987260">called</span>
  <span m="1987830">off-policy</span> <span m="1988610">evaluation.</span> <span m="1995570">And</span>
  <span m="1996770">this</span> <span m="1998270">is</span> <span m="1998480">an</span>
  <span m="1998600">estimator,</span> <span m="1999230">which</span> <span m="1999680">is</span>
  <span m="2000640">completely</span> <span m="2001030">analogous</span> <span m="2001630">to</span>
  <span m="2001720">the</span> <span m="2001810">estimator</span> <span m="2002200">that</span>
  <span m="2002350">we</span> <span m="2002470">got</span> <span m="2002800">from</span>
  <span m="2003250">Q</span> <span m="2003520">learning.</span> <span m="2004370">So</span>
  <span m="2004870">if</span> <span m="2005020">all</span> <span m="2005260">assumptions</span>
  <span m="2005980">were</span> <span m="2006160">correct,</span> <span m="2006670">and</span>
  <span m="2006790">you</span> <span m="2006880">had</span> <span m="2007090">a</span>
  <span m="2007150">lot</span> <span m="2007360">of</span> <span m="2007480">data,</span>
  <span m="2008600">then</span> <span m="2009220">those</span> <span m="2009580">two</span>
  <span m="2009850">should</span> <span m="2010000">give</span> <span m="2010150">you</span>
  <span m="2010240">precisely</span> <span m="2010750">the</span> <span m="2010840">same</span>
  <span m="2011170">answer.</span></p><p><span m="2012980">But</span> <span m="2013190">here,</span>
  <span m="2013730">like</span> <span m="2014090">in</span> <span m="2014180">the</span>
  <span m="2014270">causal</span> <span m="2014600">inference</span> <span m="2014900">setting,</span>
  <span m="2015800">we</span> <span m="2016100">are</span> <span m="2016280">not</span>
  <span m="2016700">making</span> <span m="2017000">the</span> <span m="2017060">assumption</span>
  <span m="2017540">that</span> <span m="2017750">we</span> <span m="2017960">can</span>
  <span m="2018170">do</span> <span m="2018500">covariate</span> <span m="2019070">adjustment</span>
  <span m="2019520">well.</span> <span m="2020780">Or</span> <span m="2020900">said</span>
  <span m="2021050">differently,</span> <span m="2021450">we're</span> <span m="2021550">not</span>
  <span m="2021650">assuming</span> <span m="2021980">that</span> <span m="2022100">we</span>
  <span m="2022190">can</span> <span m="2022310">fit</span> <span m="2022760">the</span>
  <span m="2023240">Q</span> <span m="2023570">function</span> <span m="2024020">well.</span></p><p><span
  m="2025450">And</span> <span m="2025600">this</span> <span m="2025900">is</span>
  <span m="2026020">now,</span> <span m="2026830">just</span> <span m="2027160">like</span>
  <span m="2027400">there,</span> <span m="2028060">based</span> <span m="2028480">on</span>
  <span m="2028570">the</span> <span m="2028630">assumption</span> <span m="2029050">that</span>
  <span m="2029170">we</span> <span m="2029320">have</span> <span m="2030220">the</span>
  <span m="2030310">ability</span> <span m="2030640">to</span> <span m="2031120">really</span>
  <span m="2031480">accurately</span> <span m="2031870">know</span> <span m="2031960">what</span>
  <span m="2032050">the</span> <span m="2032110">propensity</span> <span m="2032590">scores</span>
  <span m="2033040">are.</span> <span m="2033730">So</span> <span m="2033970">it</span>
  <span m="2034040">now</span> <span m="2034240">gives</span> <span m="2034480">you</span>
  <span m="2034540">an</span> <span m="2034630">alternative</span> <span m="2035290">approach</span>
  <span m="2035650">to</span> <span m="2035770">do</span> <span m="2035830">evaluation.</span>
  <span m="2036850">And</span> <span m="2036970">you</span> <span m="2037030">could</span>
  <span m="2037180">think</span> <span m="2037420">about</span> <span m="2037690">looking</span>
  <span m="2038020">at</span> <span m="2038080">the</span> <span m="2038260">robustness</span>
  <span m="2038950">of</span> <span m="2039070">your</span> <span m="2039190">estimates</span>
  <span m="2040120">from</span> <span m="2040330">these</span> <span m="2040480">two</span>
  <span m="2040660">different</span> <span m="2041860">estimators.</span></p><p><span
  m="2044340">And</span> <span m="2047070">this</span> <span m="2047280">is</span>
  <span m="2047400">the</span> <span m="2047640">most</span> <span m="2047910">naive</span>
  <span m="2048449">of</span> <span m="2048630">the</span> <span m="2048719">estimators.</span>
  <span m="2049290">There</span> <span m="2049409">are</span> <span m="2049440">many</span>
  <span m="2049679">ways</span> <span m="2049889">to</span> <span m="2049980">try</span>
  <span m="2050400">to</span> <span m="2050520">make</span> <span m="2050670">this</span>
  <span m="2050820">better,</span> <span m="2051880">such</span> <span m="2052050">as</span>
  <span m="2052260">by</span> <span m="2054420">doing</span> <span m="2055110">w</span>
  <span m="2055440">robust</span> <span m="2055770">estimators.</span> <span m="2056800">And</span>
  <span m="2056940">if</span> <span m="2057030">you</span> <span m="2057120">want</span>
  <span m="2057300">to</span> <span m="2057360">learn</span> <span m="2057630">more,</span>
  <span m="2058330">I</span> <span m="2058429">recommend</span> <span m="2058739">reading</span>
  <span m="2059639">this</span> <span m="2059940">paper</span> <span m="2060659">by</span>
  <span m="2061980">Thomas</span> <span m="2062730">and</span> <span m="2063800">Emma</span>
  <span m="2064040">Brunskill</span> <span m="2066270">in</span> <span m="2066750">ICML</span>
  <span m="2068010">2016.</span></p><p><span m="2070170">And</span> <span m="2070260">with</span>
  <span m="2070409">that,</span> <span m="2071100">I</span> <span m="2071219">want</span>
  <span m="2071550">Barbra</span> <span m="2071880">to</span> <span m="2071969">come</span>
  <span m="2072179">up</span> <span m="2072360">and</span> <span m="2072449">get</span>
  <span m="2072600">set</span> <span m="2072810">up.</span> <span m="2073110">And</span>
  <span m="2073199">we're</span> <span m="2073290">going</span> <span m="2073409">to</span>
  <span m="2073469">transition</span> <span m="2073830">to</span> <span m="2073889">the</span>
  <span m="2073980">next</span> <span m="2074190">part</span> <span m="2074310">of</span>
  <span m="2074370">the</span> <span m="2074429">lecture.</span> <span m="2078300">Yes.</span></p><p><span
  m="2079039">AUDIENCE:</span> <span m="2079129">Why</span> <span m="2079219">do</span>
  <span m="2079309">we</span> <span m="2079400">sum</span> <span m="2079810">over</span>
  <span m="2080050">t</span> <span m="2080610">and</span> <span m="2081070">take</span>
  <span m="2081530">the</span> <span m="2081600">project</span> <span m="2082550">across</span>
  <span m="2082949">all</span> <span m="2083365">t?</span></p><p><span m="2084199">DAVID
  SONTAG:</span> <span m="2084364">One</span> <span m="2084530">easy</span> <span
  m="2084800">way</span> <span m="2084889">to</span> <span m="2084980">think</span>
  <span m="2085219">about</span> <span m="2085520">this</span> <span m="2086000">is</span>
  <span m="2086750">suppose</span> <span m="2087230">that</span> <span m="2087380">you</span>
  <span m="2087500">only</span> <span m="2087710">had</span> <span m="2087870">a</span>
  <span m="2087920">reward</span> <span m="2088290">of the</span> <span m="2088370">last</span>
  <span m="2088610">time</span> <span m="2088880">step.</span> <span m="2089770">If</span>
  <span m="2090020">you</span> <span m="2090080">only</span> <span m="2090230">had</span>
  <span m="2090350">a</span> <span m="2090469">reward</span> <span m="2090770">of</span>
  <span m="2090830">the</span> <span m="2090920">last</span> <span m="2091130">time</span>
  <span m="2091440">step,</span> <span m="2091730">then</span> <span m="2091940">you</span>
  <span m="2092060">wouldn't</span> <span m="2092330">have</span> <span m="2092480">this</span>
  <span m="2092620">sum</span> <span m="2092820">over</span> <span m="2092929">t,</span>
  <span m="2093290">because</span> <span m="2093469">the</span> <span m="2093590">rewards</span>
  <span m="2093949">in</span> <span m="2094010">the</span> <span m="2094070">earlier</span>
  <span m="2094310">steps</span> <span m="2094550">would</span> <span m="2094639">be</span>
  <span m="2094730">0.</span> <span m="2095510">You</span> <span m="2095600">would</span>
  <span m="2095690">just</span> <span m="2095870">have</span> <span m="2096020">that</span>
  <span m="2096170">product</span> <span m="2096739">going</span> <span m="2096980">from</span>
  <span m="2097130">0 up</span> <span m="2097460">to</span> <span m="2097550">capital</span>
  <span m="2097880">T</span> <span m="2098040">of</span> <span m="2098150">last</span>
  <span m="2098360">time</span> <span m="2098600">step.</span></p><p><span m="2099590">The</span>
  <span m="2099650">reason</span> <span m="2099950">why</span> <span m="2100160">you</span>
  <span m="2100340">have</span> <span m="2100700">it</span> <span m="2101840">up</span>
  <span m="2102020">to</span> <span m="2102570">at</span> <span m="2102710">each</span>
  <span m="2102860">time</span> <span m="2103100">step</span> <span m="2103340">is</span>
  <span m="2103430">because</span> <span m="2104090">one</span> <span m="2104300">wants</span>
  <span m="2104540">to</span> <span m="2104630">be</span> <span m="2104720">able</span>
  <span m="2104900">to</span> <span m="2105050">appropriately</span> <span m="2105620">weigh</span>
  <span m="2105890">the</span> <span m="2107090">likelihood</span> <span m="2107590">of</span>
  <span m="2108290">seeing</span> <span m="2109220">that</span> <span m="2109400">reward</span>
  <span m="2109670">at</span> <span m="2109730">that</span> <span m="2109880">point</span>
  <span m="2110090">in</span> <span m="2110210">time.</span> <span m="2111150">One</span>
  <span m="2111320">could</span> <span m="2111470">rewrite</span> <span m="2111830">this</span>
  <span m="2111950">in</span> <span m="2112040">other</span> <span m="2112250">ways.</span>
  <span m="2112940">I</span> <span m="2112970">want</span> <span m="2113090">to</span>
  <span m="2113150">hold</span> <span m="2113360">other</span> <span m="2113540">questions,</span>
  <span m="2113930">because</span> <span m="2114620">this</span> <span m="2114800">part</span>
  <span m="2114920">of</span> <span m="2114980">the</span> <span m="2115040">lecture</span>
  <span m="2115250">is</span> <span m="2115310">going</span> <span m="2115390">to</span>
  <span m="2115460">be</span> <span m="2115520">much</span> <span m="2115700">more</span>
  <span m="2115790">interesting</span> <span m="2116120">than</span> <span m="2116210">my</span>
  <span m="2116330">part</span> <span m="2116460">of the</span> <span m="2116540">lecture.</span></p><p><span
  m="2118730">And</span> <span m="2118850">with</span> <span m="2119000">that,</span>
  <span m="2119360">I</span> <span m="2119570">want</span> <span m="2119750">introduce</span>
  <span m="2120550">Barbra.</span> <span m="2121900">Barbra,</span> <span m="2122720">I</span>
  <span m="2122810">first</span> <span m="2123080">met</span> <span m="2123230">her</span>
  <span m="2123350">when</span> <span m="2123500">she</span> <span m="2123620">invited</span>
  <span m="2123920">me</span> <span m="2124040">to</span> <span m="2124130">give</span>
  <span m="2124280">a</span> <span m="2124340">talk</span> <span m="2124520">in</span>
  <span m="2124610">her</span> <span m="2124790">class</span> <span m="2125810">last</span>
  <span m="2126110">year.</span> <span m="2127370">She's</span> <span m="2127910">an</span>
  <span m="2128270">instructor</span> <span m="2128990">at</span> <span m="2129920">Harvard</span>
  <span m="2131570">Medical</span> <span m="2131960">School--</span> <span m="2133550">or</span>
  <span m="2133940">School</span> <span m="2134180">of</span> <span m="2134240">Public</span>
  <span m="2134510">Health.</span></p><p><span m="2136370">She</span> <span m="2136820">recently</span>
  <span m="2137180">finished</span> <span m="2137410">her</span> <span m="2137510">PhD</span>
  <span m="2137770">in</span> <span m="2137870">2018.</span> <span m="2139530">And</span>
  <span m="2140390">her</span> <span m="2140540">PhD</span> <span m="2141140">looked</span>
  <span m="2141410">at</span> <span m="2141770">many</span> <span m="2142340">questions</span>
  <span m="2142820">related</span> <span m="2143090">to</span> <span m="2143210">the</span>
  <span m="2143300">themes</span> <span m="2143930">of</span> <span m="2144050">the</span>
  <span m="2144140">last</span> <span m="2144350">couple</span> <span m="2144590">of</span>
  <span m="2144710">weeks.</span> <span m="2145910">Since</span> <span m="2146330">that</span>
  <span m="2146540">time,</span> <span m="2147080">in</span> <span m="2147200">addition</span>
  <span m="2147470">continuing</span> <span m="2147860">her</span> <span m="2147950">research,</span>
  <span m="2148500">she's</span> <span m="2148760">been</span> <span m="2149570">really</span>
  <span m="2149840">leading</span> <span m="2150200">the</span> <span m="2150260">way</span>
  <span m="2150500">in</span> <span m="2150590">creating</span> <span m="2151400">data</span>
  <span m="2151670">science</span> <span m="2152000">curriculum</span> <span m="2152840">over</span>
  <span m="2153050">at</span> <span m="2153140">Harvard.</span> <span m="2154100">So</span>
  <span m="2154610">please</span> <span m="2154790">take</span> <span m="2154910">it</span>
  <span m="2154980">away.</span></p><p><span m="2155210">BARBRA DICKERMAN:</span>
  <span m="2155345">Thank</span> <span m="2155480">you</span> <span m="2155570">so</span>
  <span m="2155720">much</span> <span m="2155930">for</span> <span m="2156020">the</span>
  <span m="2156110">introduction,</span> <span m="2156650">David.</span> <span m="2157870">I'm</span>
  <span m="2158400">very</span> <span m="2158720">happy</span> <span m="2158990">to</span>
  <span m="2159080">be</span> <span m="2159260">here</span> <span m="2159500">to</span>
  <span m="2159620">share</span> <span m="2159920">some</span> <span m="2160220">of</span>
  <span m="2160340">my</span> <span m="2160610">work</span> <span m="2161180">on</span>
  <span m="2161540">evaluating</span> <span m="2162320">dynamic</span> <span m="2162950">treatment</span>
  <span m="2163340">strategies,</span> <span m="2164420">which</span> <span m="2164600">you've</span>
  <span m="2164750">been</span> <span m="2164930">talking</span> <span m="2165320">about</span>
  <span m="2165710">over</span> <span m="2165950">the</span> <span m="2166040">past</span>
  <span m="2166490">few</span> <span m="2167330">lectures.</span></p><p><span m="2168800">So</span>
  <span m="2168980">my</span> <span m="2169130">goals</span> <span m="2169610">for</span>
  <span m="2170030">today,</span> <span m="2170690">I'm</span> <span m="2170870">just</span>
  <span m="2171020">going</span> <span m="2171130">to</span> <span m="2171200">breeze</span>
  <span m="2171620">over</span> <span m="2172430">defining</span> <span m="2173270">dynamic</span>
  <span m="2173720">treatment</span> <span m="2173990">strategies,</span> <span m="2174500">as</span>
  <span m="2174680">you're</span> <span m="2174800">already</span> <span m="2175040">familiar</span>
  <span m="2175430">with</span> <span m="2175610">it.</span> <span m="2176220">But</span>
  <span m="2176270">I</span> <span m="2176360">would</span> <span m="2176600">like</span>
  <span m="2176840">to</span> <span m="2176960">touch</span> <span m="2177410">on</span>
  <span m="2178160">when</span> <span m="2178520">we</span> <span m="2178730">need</span>
  <span m="2179240">a</span> <span m="2179300">special</span> <span m="2179750">class</span>
  <span m="2180140">of</span> <span m="2180230">methods</span> <span m="2180710">called</span>
  <span m="2181130">g-methods.</span> <span m="2182760">And</span> <span m="2182780">then</span>
  <span m="2182900">we'll</span> <span m="2183020">talk</span> <span m="2183290">about</span>
  <span m="2183590">two</span> <span m="2183830">different</span> <span m="2184250">applications,</span>
  <span m="2185910">different</span> <span m="2186110">analyses,</span> <span m="2186860">that</span>
  <span m="2187070">have</span> <span m="2187220">focused</span> <span m="2187820">on</span>
  <span m="2188030">evaluating</span> <span m="2188840">dynamic</span> <span m="2189470">treatment</span>
  <span m="2189890">strategies.</span></p><p><span m="2191250">So</span> <span m="2191330">the</span>
  <span m="2191420">first</span> <span m="2191930">will</span> <span m="2192110">be</span>
  <span m="2192410">an</span> <span m="2192530">application</span> <span m="2193490">of</span>
  <span m="2194210">the</span> <span m="2194300">parametric</span> <span m="2194990">g-formula,</span>
  <span m="2195870">which</span> <span m="2196010">is</span> <span m="2196190">a</span>
  <span m="2196250">powerful</span> <span m="2196850">g-method</span> <span m="2197960">to</span>
  <span m="2198230">cancer</span> <span m="2198710">research.</span> <span m="2199890">And</span>
  <span m="2199970">so</span> <span m="2200750">the</span> <span m="2200870">goal</span>
  <span m="2201110">here</span> <span m="2201380">is</span> <span m="2201500">to</span>
  <span m="2201620">give</span> <span m="2201860">you</span> <span m="2202070">my</span>
  <span m="2202400">causal</span> <span m="2202820">inference</span> <span m="2203240">perspective</span>
  <span m="2204290">on</span> <span m="2204440">how</span> <span m="2204650">we</span>
  <span m="2204800">think</span> <span m="2205100">about</span> <span m="2205400">this</span>
  <span m="2205610">task</span> <span m="2206150">of</span> <span m="2206270">sequential</span>
  <span m="2206780">decision</span> <span m="2207200">making</span> <span m="2208100">and</span>
  <span m="2208250">then</span> <span m="2208610">with</span> <span m="2208880">whatever</span>
  <span m="2209240">time</span> <span m="2209510">remains,</span> <span m="2210140">we'll</span>
  <span m="2210350">be</span> <span m="2210500">discussing</span> <span m="2211760">a</span>
  <span m="2211880">recent</span> <span m="2212210">publication</span> <span m="2213020">on</span>
  <span m="2213290">the</span> <span m="2213510">AI</span> <span m="2213980">clinician</span>
  <span m="2215030">to</span> <span m="2215180">talk</span> <span m="2215480">through</span>
  <span m="2215750">the</span> <span m="2215870">reinforcement</span> <span m="2216530">learning</span>
  <span m="2216890">perspective.</span></p><p><span m="2218010">So</span> <span m="2218110">I</span>
  <span m="2218210">think</span> <span m="2218270">it'll</span> <span m="2218390">be</span>
  <span m="2218510">a</span> <span m="2218570">really</span> <span m="2218900">interesting</span>
  <span m="2219410">discussion,</span> <span m="2219920">where</span> <span m="2220040">we</span>
  <span m="2220160">can</span> <span m="2220340">share</span> <span m="2220580">these</span>
  <span m="2220790">perspectives,</span> <span m="2221720">talk</span> <span m="2221960">about</span>
  <span m="2222200">the</span> <span m="2222260">relative</span> <span m="2222740">strengths</span>
  <span m="2223190">and</span> <span m="2223280">limitations</span> <span m="2224000">as</span>
  <span m="2224150">well.</span> <span m="2226200">And</span> <span m="2226220">please</span>
  <span m="2226430">stop</span> <span m="2226730">me</span> <span m="2226880">if</span>
  <span m="2226970">you</span> <span m="2227060">have</span> <span m="2227150">any</span>
  <span m="2227330">questions.</span></p><p><span m="2230310">So</span> <span m="2230460">you</span>
  <span m="2230610">already</span> <span m="2230850">know</span> <span m="2231060">this.</span>
  <span m="2231420">When</span> <span m="2231600">it</span> <span m="2231660">comes</span>
  <span m="2231960">to</span> <span m="2232050">treatment</span> <span m="2232380">strategies,</span>
  <span m="2233020">there's</span> <span m="2233160">three</span> <span m="2233340">main</span>
  <span m="2233550">types.</span> <span m="2233980">There's</span> <span m="2234090">point</span>
  <span m="2234360">interventions</span> <span m="2235050">happening</span> <span
  m="2235470">at</span> <span m="2235560">a</span> <span m="2235620">single</span>
  <span m="2235890">point</span> <span m="2236100">in</span> <span m="2236220">time.</span>
  <span m="2236840">There's</span> <span m="2237030">sustained</span> <span m="2237690">interventions</span>
  <span m="2238470">happening</span> <span m="2238920">over</span> <span m="2239250">time.</span>
  <span m="2240000">When</span> <span m="2240120">it</span> <span m="2240180">comes</span>
  <span m="2240420">to</span> <span m="2240510">clinical</span> <span m="2240870">care,</span>
  <span m="2241270">this</span> <span m="2241320">is</span> <span m="2241440">often</span>
  <span m="2241770">what</span> <span m="2241950">we're</span> <span m="2242400">most</span>
  <span m="2242700">interested</span> <span m="2243150">in.</span> <span m="2243960">Within</span>
  <span m="2244320">that,</span> <span m="2244560">there are</span> <span m="2244710">static</span>
  <span m="2245160">strategies,</span> <span m="2245880">which</span> <span m="2246120">are</span>
  <span m="2246240">constant</span> <span m="2246900">over</span> <span m="2247170">time.</span>
  <span m="2248050">And</span> <span m="2248070">then</span> <span m="2248250">there's</span>
  <span m="2248520">dynamic</span> <span m="2249120">strategies,</span> <span m="2249810">which</span>
  <span m="2250020">we're</span> <span m="2250110">going</span> <span m="2250260">to</span>
  <span m="2250320">focus</span> <span m="2250740">on.</span> <span m="2251910">And</span>
  <span m="2252030">these</span> <span m="2252300">differ</span> <span m="2252780">in</span>
  <span m="2252960">that</span> <span m="2253320">the</span> <span m="2253470">intervention</span>
  <span m="2254160">over</span> <span m="2254400">time</span> <span m="2254970">depends</span>
  <span m="2255660">on</span> <span m="2255960">evolving</span> <span m="2256800">characteristics.</span></p><p><span
  m="2258300">So</span> <span m="2258510">for</span> <span m="2258720">example,</span>
  <span m="2259800">initiate</span> <span m="2260310">treatment</span> <span m="2260670">at</span>
  <span m="2260730">baseline</span> <span m="2261330">and</span> <span m="2261450">continue</span>
  <span m="2261870">it</span> <span m="2261960">over</span> <span m="2262140">follow</span>
  <span m="2262500">up</span> <span m="2262710">until</span> <span m="2263130">a</span>
  <span m="2263160">contraindication</span> <span m="2264120">occurs,</span> <span
  m="2265050">at</span> <span m="2265170">which</span> <span m="2265440">point</span>
  <span m="2265800">you</span> <span m="2265980">may</span> <span m="2266310">stop</span>
  <span m="2266760">treatment</span> <span m="2267750">and</span> <span m="2267870">decide</span>
  <span m="2268320">with</span> <span m="2268500">your</span> <span m="2268620">doctor</span>
  <span m="2269200">whether</span> <span m="2269370">you're</span> <span m="2269520">going</span>
  <span m="2269790">to</span> <span m="2269910">switch</span> <span m="2270420">to</span>
  <span m="2270630">an</span> <span m="2270750">alternate</span> <span m="2271230">treatment.</span>
  <span m="2272610">You</span> <span m="2272760">would</span> <span m="2272910">still</span>
  <span m="2273180">be</span> <span m="2273330">adhering</span> <span m="2273840">to</span>
  <span m="2273990">that</span> <span m="2274170">strategy,</span> <span m="2274770">even</span>
  <span m="2275040">though</span> <span m="2275160">you</span> <span m="2275310">quit.</span></p><p><span
  m="2276390">The</span> <span m="2276510">comparison</span> <span m="2277140">here</span>
  <span m="2277320">being</span> <span m="2277590">do</span> <span m="2277800">not</span>
  <span m="2278070">initiate</span> <span m="2278550">treatment</span> <span m="2279000">over</span>
  <span m="2279270">follow</span> <span m="2279630">up,</span> <span m="2280540">likewise</span>
  <span m="2280950">unless</span> <span m="2281460">an</span> <span m="2281610">indication</span>
  <span m="2282210">occurs,</span> <span m="2282930">at</span> <span m="2283020">which</span>
  <span m="2283200">point</span> <span m="2283470">you</span> <span m="2283590">may</span>
  <span m="2283770">start</span> <span m="2284100">treatment</span> <span m="2284550">and</span>
  <span m="2284640">still</span> <span m="2284880">be</span> <span m="2285000">adhering</span>
  <span m="2285360">to</span> <span m="2285480">the</span> <span m="2285570">strategy.</span>
  <span m="2286600">So</span> <span m="2286700">we're</span> <span m="2286710">focusing</span>
  <span m="2287160">on</span> <span m="2287250">these</span> <span m="2287490">because</span>
  <span m="2287790">they're</span> <span m="2287940">the</span> <span m="2288030">most</span>
  <span m="2288360">clinically</span> <span m="2288810">relevant.</span></p><p><span
  m="2291710">And</span> <span m="2291860">so</span> <span m="2292040">clinicians</span>
  <span m="2292640">encounter</span> <span m="2293060">these</span> <span m="2293540">every</span>
  <span m="2293770">day</span> <span m="2294110">in</span> <span m="2294200">practice.</span>
  <span m="2294860">So</span> <span m="2294920">when</span> <span m="2295070">they're</span>
  <span m="2295460">making</span> <span m="2295880">a</span> <span m="2296120">recommendation</span>
  <span m="2296870">to</span> <span m="2296990">their</span> <span m="2297140">patient</span>
  <span m="2297620">about</span> <span m="2298010">a</span> <span m="2298160">prevention</span>
  <span m="2299360">intervention,</span> <span m="2300410">they're</span> <span m="2300530">going</span>
  <span m="2300770">to</span> <span m="2300860">be</span> <span m="2301040">taking</span>
  <span m="2301430">into</span> <span m="2301610">consideration</span> <span m="2302360">the</span>
  <span m="2302420">patient's</span> <span m="2302870">evolving</span> <span m="2303350">comorbidities.</span></p><p><span
  m="2304700">Or</span> <span m="2304820">when</span> <span m="2305000">they're</span>
  <span m="2305150">deciding</span> <span m="2305720">the</span> <span m="2305810">next</span>
  <span m="2306050">screening</span> <span m="2306500">interval,</span> <span m="2307280">they'll</span>
  <span m="2307430">consider</span> <span m="2307850">the</span> <span m="2307970">previous</span>
  <span m="2308570">result</span> <span m="2309020">from</span> <span m="2309230">the</span>
  <span m="2309320">last</span> <span m="2309620">screening</span> <span m="2310130">test</span>
  <span m="2310550">when</span> <span m="2310730">deciding</span> <span m="2311150">that.</span>
  <span m="2312080">Likewise</span> <span m="2312590">for</span> <span m="2312740">treatment,</span>
  <span m="2313610">deciding</span> <span m="2314060">whether</span> <span m="2314360">to</span>
  <span m="2314480">keep</span> <span m="2314690">the</span> <span m="2314780">patient</span>
  <span m="2315140">on</span> <span m="2315230">treatment</span> <span m="2315590">or</span>
  <span m="2315650">not.</span> <span m="2316400">Is</span> <span m="2316580">the</span>
  <span m="2316670">patient</span> <span m="2317360">having</span> <span m="2317690">any</span>
  <span m="2317840">changes</span> <span m="2318290">in</span> <span m="2318380">symptoms</span>
  <span m="2319190">or</span> <span m="2319700">lab</span> <span m="2320000">values</span>
  <span m="2320570">that</span> <span m="2320720">may</span> <span m="2320870">reflect</span>
  <span m="2321290">toxicity?</span></p><p><span m="2323210">So</span> <span m="2323420">one</span>
  <span m="2323600">thing</span> <span m="2323780">to</span> <span m="2323900">note</span>
  <span m="2324230">is</span> <span m="2324410">that</span> <span m="2325310">while</span>
  <span m="2325730">many</span> <span m="2326090">of</span> <span m="2326210">the</span>
  <span m="2326300">strategies</span> <span m="2327110">that</span> <span m="2327440">you</span>
  <span m="2327590">may</span> <span m="2327800">see</span> <span m="2328220">in</span>
  <span m="2328340">clinical</span> <span m="2328700">guidelines</span> <span m="2329360">and</span>
  <span m="2329600">in</span> <span m="2329720">clinical</span> <span m="2330080">practice</span>
  <span m="2331040">are</span> <span m="2331310">dynamic</span> <span m="2331880">strategies,</span>
  <span m="2333140">these</span> <span m="2333380">may</span> <span m="2333590">not</span>
  <span m="2333980">be</span> <span m="2334610">the</span> <span m="2334820">optimal</span>
  <span m="2335450">strategies.</span> <span m="2336210">So</span> <span m="2336290">maybe</span>
  <span m="2336590">what</span> <span m="2336740">we're</span> <span m="2336830">recommending</span>
  <span m="2337430">and</span> <span m="2337520">doing</span> <span m="2337820">is</span>
  <span m="2337910">not</span> <span m="2338180">optimal</span> <span m="2338600">for</span>
  <span m="2338720">patients.</span> <span m="2339840">However,</span> <span m="2340190">the</span>
  <span m="2340400">optimal</span> <span m="2341000">strategies</span> <span m="2341750">will</span>
  <span m="2342020">be</span> <span m="2342230">dynamic</span> <span m="2342980">in</span>
  <span m="2343190">some</span> <span m="2343580">way,</span> <span m="2344360">in</span>
  <span m="2344540">that</span> <span m="2344750">they</span> <span m="2344960">will</span>
  <span m="2345200">be</span> <span m="2345380">adapting</span> <span m="2346160">to</span>
  <span m="2346340">individuals'</span> <span m="2347420">unique</span> <span m="2348110">and</span>
  <span m="2348230">evolving</span> <span m="2348860">characteristics.</span> <span
  m="2350310">So</span> <span m="2350330">that's</span> <span m="2350510">why</span>
  <span m="2350660">we</span> <span m="2350780">care</span> <span m="2351020">about</span>
  <span m="2351260">them.</span></p><p><span m="2353060">So</span> <span m="2353210">what's</span>
  <span m="2353420">the</span> <span m="2353510">problem?</span> <span m="2356270">So</span>
  <span m="2356420">one</span> <span m="2356630">problem</span> <span m="2357260">deals</span>
  <span m="2357590">with</span> <span m="2357770">something</span> <span m="2358130">called</span>
  <span m="2358370">treatment</span> <span m="2358820">confounder</span> <span m="2359390">feedback,</span>
  <span m="2359990">which</span> <span m="2360290">you</span> <span m="2360440">may</span>
  <span m="2360590">have</span> <span m="2360740">spoken</span> <span m="2361100">about</span>
  <span m="2361340">in</span> <span m="2361430">this</span> <span m="2361580">class.</span>
  <span m="2362510">So</span> <span m="2362900">conventional</span> <span m="2363710">statistical</span>
  <span m="2364460">methods</span> <span m="2365090">cannot</span> <span m="2365780">appropriately</span>
  <span m="2366710">compare</span> <span m="2368000">dynamic</span> <span m="2368600">treatment</span>
  <span m="2368990">strategies</span> <span m="2369740">in</span> <span m="2369890">the</span>
  <span m="2369950">presence</span> <span m="2370490">of</span> <span m="2370580">treatment</span>
  <span m="2370940">confounder</span> <span m="2371420">feedback.</span></p><p><span
  m="2372320">So</span> <span m="2372470">this</span> <span m="2372680">is</span>
  <span m="2372830">when</span> <span m="2373310">time</span> <span m="2373730">varying</span>
  <span m="2374180">confounders</span> <span m="2375410">are</span> <span m="2375560">affected</span>
  <span m="2376190">by</span> <span m="2376550">previous</span> <span m="2377150">treatment.</span>
  <span m="2378330">So</span> <span m="2378480">if</span> <span m="2378560">we</span>
  <span m="2379340">kind</span> <span m="2379550">of</span> <span m="2379640">ground</span>
  <span m="2380000">this</span> <span m="2380240">in</span> <span m="2380330">a</span>
  <span m="2380390">concrete</span> <span m="2380960">example</span> <span m="2381620">with</span>
  <span m="2381800">this</span> <span m="2381950">causal</span> <span m="2382310">diagram,</span>
  <span m="2383540">let's</span> <span m="2383750">say</span> <span m="2383960">we're</span>
  <span m="2384110">interested</span> <span m="2384770">in</span> <span m="2384860">estimating</span>
  <span m="2385460">the</span> <span m="2385550">effect</span> <span m="2385970">of</span>
  <span m="2386120">some</span> <span m="2386420">intervention</span> <span m="2387140">A,</span>
  <span m="2387530">vasopressors</span> <span m="2388970">or</span> <span m="2389090">it</span>
  <span m="2389150">could</span> <span m="2389330">be</span> <span m="2389510">IV</span>
  <span m="2389810">fluids,</span> <span m="2390980">on</span> <span m="2391760">some</span>
  <span m="2392040">outcome</span> <span m="2392390">Y,</span> <span m="2392750">which</span>
  <span m="2392990">we'll</span> <span m="2393140">call</span> <span m="2393410">survival</span>
  <span m="2394070">here.</span></p><p><span m="2395090">We</span> <span m="2395270">know</span>
  <span m="2395510">that</span> <span m="2395660">vasopressors</span> <span m="2396710">affect</span>
  <span m="2397220">blood</span> <span m="2397490">pressure,</span> <span m="2398630">and</span>
  <span m="2398750">blood</span> <span m="2398990">pressure</span> <span m="2399410">will</span>
  <span m="2399620">affect</span> <span m="2400130">subsequent</span> <span m="2401300">decisions</span>
  <span m="2402140">to</span> <span m="2402320">treat</span> <span m="2402560">with</span>
  <span m="2402850">vasopressors.</span> <span m="2404210">We</span> <span m="2404330">also</span>
  <span m="2404570">know</span> <span m="2404750">that</span> <span m="2404930">hypotension--</span>
  <span m="2405920">so</span> <span m="2406070">again,</span> <span m="2406340">blood</span>
  <span m="2406580">pressure,</span> <span m="2406970">L1,</span> <span m="2407840">affects</span>
  <span m="2408260">survival,</span> <span m="2410300">based</span> <span m="2410570">on</span>
  <span m="2410690">our</span> <span m="2410750">clinical</span> <span m="2411110">knowledge.</span></p><p><span
  m="2412130">And</span> <span m="2412280">then</span> <span m="2412490">in</span>
  <span m="2412640">this</span> <span m="2412940">DAG,</span> <span m="2413420">we</span>
  <span m="2413570">also</span> <span m="2413900">have</span> <span m="2414230">the</span>
  <span m="2414350">node</span> <span m="2414920">U,</span> <span m="2415970">which</span>
  <span m="2416180">represents</span> <span m="2416870">disease</span> <span m="2417410">severity.</span>
  <span m="2418560">So</span> <span m="2418580">these</span> <span m="2418790">could</span>
  <span m="2419030">be</span> <span m="2419570">potentially</span> <span m="2420440">unmeasured</span>
  <span m="2421250">markers</span> <span m="2421910">of</span> <span m="2422060">disease</span>
  <span m="2422390">severity</span> <span m="2423440">that</span> <span m="2423740">are</span>
  <span m="2424070">affecting</span> <span m="2424580">your</span> <span m="2424700">blood</span>
  <span m="2424910">pressure</span> <span m="2425810">and</span> <span m="2425960">also</span>
  <span m="2426440">affecting</span> <span m="2427460">your</span> <span m="2427820">probability</span>
  <span m="2428420">of</span> <span m="2428480">survival.</span></p><p><span m="2430260">So</span>
  <span m="2430370">if</span> <span m="2430580">we're</span> <span m="2430730">interested</span>
  <span m="2431330">in</span> <span m="2431450">estimating</span> <span m="2432500">the</span>
  <span m="2432650">effect</span> <span m="2433340">of</span> <span m="2433520">a</span>
  <span m="2433670">sustained</span> <span m="2434660">treatment</span> <span m="2435230">strategy,</span>
  <span m="2437510">then</span> <span m="2437780">we</span> <span m="2437930">want</span>
  <span m="2438140">to</span> <span m="2438200">know</span> <span m="2438590">something</span>
  <span m="2439010">about</span> <span m="2439280">the</span> <span m="2439400">total</span>
  <span m="2439850">effect</span> <span m="2440140">of</span> <span m="2440300">treatment</span>
  <span m="2440720">at</span> <span m="2440840">all</span> <span m="2440960">time</span>
  <span m="2441230">points.</span> <span m="2442430">We</span> <span m="2442550">can</span>
  <span m="2442700">see</span> <span m="2442940">that</span> <span m="2443120">L1</span>
  <span m="2443540">here</span> <span m="2443780">is</span> <span m="2443900">a</span>
  <span m="2443930">confounder</span> <span m="2444470">for</span> <span m="2444620">the</span>
  <span m="2444740">effect</span> <span m="2445040">of</span> <span m="2445130">A1</span>
  <span m="2445520">on</span> <span m="2445670">Y</span> <span m="2446030">so</span>
  <span m="2446180">we</span> <span m="2446300">have</span> <span m="2446450">to</span>
  <span m="2446540">do</span> <span m="2446750">something</span> <span m="2447170">to</span>
  <span m="2447290">adjust</span> <span m="2447620">for</span> <span m="2447740">that.</span>
  <span m="2448560">And</span> <span m="2448670">if</span> <span m="2448790">we</span>
  <span m="2448940">were</span> <span m="2449150">to</span> <span m="2449300">apply</span>
  <span m="2449670">a</span> <span m="2449720">conventional</span> <span m="2450380">statistical</span>
  <span m="2450980">method,</span> <span m="2451980">we</span> <span m="2452030">would</span>
  <span m="2452210">essentially</span> <span m="2452750">be</span> <span m="2452900">conditioning</span>
  <span m="2453650">on</span> <span m="2453800">a</span> <span m="2453860">collider</span>
  <span m="2454970">and</span> <span m="2455150">inducing</span> <span m="2455660">a</span>
  <span m="2455720">selection</span> <span m="2456260">bias.</span> <span m="2456780">So</span>
  <span m="2457010">an</span> <span m="2457160">open</span> <span m="2457460">path</span>
  <span m="2457820">from</span> <span m="2458060">A0</span> <span m="2458630">to</span>
  <span m="2458780">L1</span> <span m="2459290">to</span> <span m="2459410">U</span>
  <span m="2459620">to</span> <span m="2459800">Y.</span></p><p><span m="2461210">What's</span>
  <span m="2461480">the</span> <span m="2461570">consequence</span> <span m="2462170">of</span>
  <span m="2462290">this?</span> <span m="2462750">If</span> <span m="2462800">we</span>
  <span m="2462920">look</span> <span m="2463130">in</span> <span m="2463220">our</span>
  <span m="2463310">data</span> <span m="2463610">set,</span> <span m="2463910">we</span>
  <span m="2464060">may</span> <span m="2464270">see</span> <span m="2464630">an</span>
  <span m="2464750">association</span> <span m="2465620">between</span> <span m="2465905">A</span>
  <span m="2466190">and</span> <span m="2466610">Y.</span> <span m="2468040">But</span>
  <span m="2468170">that</span> <span m="2468320">association</span> <span m="2469280">is</span>
  <span m="2469490">not</span> <span m="2469820">because</span> <span m="2470390">there's</span>
  <span m="2470840">necessarily</span> <span m="2471410">an</span> <span m="2471500">effect</span>
  <span m="2471960">of</span> <span m="2472130">A</span> <span m="2472250">on</span>
  <span m="2472400">Y.</span> <span m="2472650">It</span> <span m="2472760">might</span>
  <span m="2472910">not</span> <span m="2473060">be</span> <span m="2473180">causal.</span>
  <span m="2474080">It</span> <span m="2474200">may</span> <span m="2474380">be</span>
  <span m="2474560">due</span> <span m="2474920">to</span> <span m="2475220">this</span>
  <span m="2475490">selection</span> <span m="2476030">bias</span> <span m="2476510">that</span>
  <span m="2476690">we</span> <span m="2476870">created.</span></p><p><span m="2479100">So</span>
  <span m="2479810">this</span> <span m="2480050">is</span> <span m="2480170">the</span>
  <span m="2480260">problem.</span> <span m="2480930">And</span> <span m="2480950">so</span>
  <span m="2481190">in</span> <span m="2481370">these</span> <span m="2481580">cases,</span>
  <span m="2482250">we</span> <span m="2482330">need</span> <span m="2482840">a</span>
  <span m="2482930">special</span> <span m="2484040">type</span> <span m="2484370">of</span>
  <span m="2484490">method</span> <span m="2484910">that</span> <span m="2485060">can</span>
  <span m="2485240">handle</span> <span m="2486050">these</span> <span m="2486290">settings.</span>
  <span m="2488210">And</span> <span m="2488330">so</span> <span m="2488900">a</span>
  <span m="2488960">class</span> <span m="2489500">of</span> <span m="2489620">methods</span>
  <span m="2490130">that</span> <span m="2490280">was</span> <span m="2490430">designed</span>
  <span m="2491240">specifically</span> <span m="2492260">to</span> <span m="2492410">handle</span>
  <span m="2492890">this</span> <span m="2494120">is</span> <span m="2494270">g-methods.</span></p><p><span
  m="2495110">And</span> <span m="2495230">so</span> <span m="2495410">these</span>
  <span m="2496010">are</span> <span m="2496130">sometimes</span> <span m="2496580">referred</span>
  <span m="2496880">to</span> <span m="2497000">as</span> <span m="2497120">causal</span>
  <span m="2497480">methods.</span> <span m="2498380">They've</span> <span m="2498560">been</span>
  <span m="2498770">developed</span> <span m="2499220">by</span> <span m="2499400">Jamie</span>
  <span m="2499730">Robins</span> <span m="2500210">and</span> <span m="2500450">colleagues</span>
  <span m="2501530">and</span> <span m="2501620">collaborators</span> <span m="2502250">since</span>
  <span m="2502520">1986.</span> <span m="2503480">And</span> <span m="2503570">they</span>
  <span m="2503660">include</span> <span m="2504140">the</span> <span m="2504230">parametric</span>
  <span m="2504770">g-formula,</span> <span m="2505970">g-estimation</span> <span
  m="2506690">of</span> <span m="2506780">structural</span> <span m="2507200">nested</span>
  <span m="2507500">models,</span> <span m="2508100">and</span> <span m="2508370">inverse</span>
  <span m="2508730">probability</span> <span m="2509270">weighting</span> <span m="2509660">of</span>
  <span m="2509780">marginal</span> <span m="2510200">structural</span> <span m="2510650">models.</span></p><p><span
  m="2515140">So</span> <span m="2515370">in</span> <span m="2515460">my</span> <span
  m="2516060">research,</span> <span m="2516850">what</span> <span m="2516930">I</span>
  <span m="2517080">do</span> <span m="2517410">is</span> <span m="2517560">I</span>
  <span m="2517770">combine</span> <span m="2518340">g-methods</span> <span m="2519360">with</span>
  <span m="2519630">large</span> <span m="2520200">longitudinal</span> <span m="2521190">databases</span>
  <span m="2522420">to</span> <span m="2522540">try</span> <span m="2522870">to</span>
  <span m="2523050">evaluate</span> <span m="2523860">dynamic</span> <span m="2524580">treatment</span>
  <span m="2525060">strategies.</span> <span m="2526290">So</span> <span m="2526440">I'm</span>
  <span m="2526560">particularly</span> <span m="2527310">interested</span> <span
  m="2527940">in</span> <span m="2528150">bringing</span> <span m="2528570">these</span>
  <span m="2528810">methods</span> <span m="2529320">to</span> <span m="2529530">cancer</span>
  <span m="2529980">research,</span> <span m="2530520">because</span> <span m="2530790">they</span>
  <span m="2530910">haven't</span> <span m="2531180">been</span> <span m="2531330">applied</span>
  <span m="2531780">much</span> <span m="2532110">there.</span> <span m="2533010">So</span>
  <span m="2533160">a</span> <span m="2533220">lot</span> <span m="2533370">of</span>
  <span m="2533430">my</span> <span m="2533550">research</span> <span m="2533970">questions</span>
  <span m="2534420">are</span> <span m="2534510">focused</span> <span m="2535020">on</span>
  <span m="2535170">answering</span> <span m="2535620">questions</span> <span m="2536250">like,</span>
  <span m="2536950">how</span> <span m="2537330">and</span> <span m="2537450">when</span>
  <span m="2537870">can</span> <span m="2538140">we</span> <span m="2538320">intervene</span>
  <span m="2539520">to</span> <span m="2539730">best</span> <span m="2540240">prevent,</span>
  <span m="2540850">detect,</span> <span m="2541420">and</span> <span m="2541440">treat</span>
  <span m="2541740">cancer?</span></p><p><span m="2543860">And</span> <span m="2543960">so</span>
  <span m="2543990">I'd</span> <span m="2544110">like</span> <span m="2544260">to</span>
  <span m="2544350">share</span> <span m="2544650">one</span> <span m="2545010">example</span>
  <span m="2545610">with</span> <span m="2545850">you,</span> <span m="2548040">which</span>
  <span m="2548370">focused</span> <span m="2549000">on</span> <span m="2549330">evaluating</span>
  <span m="2550980">the</span> <span m="2551130">effect</span> <span m="2551760">of</span>
  <span m="2551910">adhering</span> <span m="2552480">to</span> <span m="2552690">guideline-based</span>
  <span m="2554070">physical</span> <span m="2554490">activity</span> <span m="2554940">interventions</span>
  <span m="2556290">on</span> <span m="2556530">survival</span> <span m="2557310">among</span>
  <span m="2557760">men</span> <span m="2558000">with</span> <span m="2558180">prostate</span>
  <span m="2558630">cancer.</span> <span m="2559870">So</span> <span m="2559920">the</span>
  <span m="2560010">motivation</span> <span m="2560610">for</span> <span m="2560760">this</span>
  <span m="2560940">study,</span> <span m="2561390">there's</span> <span m="2561570">a</span>
  <span m="2561630">large</span> <span m="2562050">clinical</span> <span m="2562530">organization,</span>
  <span m="2563370">ASCO,</span> <span m="2563910">the</span> <span m="2564030">American</span>
  <span m="2564420">Society</span> <span m="2564810">of</span> <span m="2564870">Clinical</span>
  <span m="2565200">Oncology,</span> <span m="2566160">that</span> <span m="2566340">had</span>
  <span m="2566430">actually</span> <span m="2566790">called</span> <span m="2567180">for</span>
  <span m="2567450">randomized</span> <span m="2568020">trials</span> <span m="2568680">to</span>
  <span m="2568800">generate</span> <span m="2569310">these</span> <span m="2569640">estimates</span>
  <span m="2570360">for</span> <span m="2570840">several</span> <span m="2571320">cancers.</span></p><p><span
  m="2572720">The thing</span> <span m="2573060">with</span> <span m="2573270">prostate</span>
  <span m="2573660">cancer</span> <span m="2574080">is</span> <span m="2574200">it's</span>
  <span m="2574320">a</span> <span m="2574350">very</span> <span m="2574590">slowly</span>
  <span m="2574980">progressing</span> <span m="2575520">disease.</span> <span m="2576580">So</span>
  <span m="2576600">the</span> <span m="2576690">feasibility</span> <span m="2577320">of</span>
  <span m="2577410">doing</span> <span m="2577710">a</span> <span m="2577770">trial</span>
  <span m="2578370">to</span> <span m="2578610">evaluate</span> <span m="2579120">this</span>
  <span m="2579840">is</span> <span m="2580020">very</span> <span m="2580380">limited.</span>
  <span m="2581040">The</span> <span m="2581130">trial</span> <span m="2581400">would</span>
  <span m="2581520">have</span> <span m="2581670">to</span> <span m="2581760">be</span>
  <span m="2581910">10</span> <span m="2582210">years</span> <span m="2582540">long</span>
  <span m="2582900">probably.</span> <span m="2584370">So</span> <span m="2585090">given</span>
  <span m="2585450">that,</span> <span m="2585750">given</span> <span m="2585990">the</span>
  <span m="2586110">absence</span> <span m="2586620">of</span> <span m="2586770">this</span>
  <span m="2586920">randomized</span> <span m="2587490">evidence,</span> <span m="2588390">we</span>
  <span m="2588510">did</span> <span m="2588690">the</span> <span m="2588780">next</span>
  <span m="2589080">best</span> <span m="2589380">thing</span> <span m="2589650">that</span>
  <span m="2589800">we</span> <span m="2589920">could</span> <span m="2590190">do</span>
  <span m="2590430">to</span> <span m="2590550">generate</span> <span m="2591060">this</span>
  <span m="2591330">estimate,</span> <span m="2592200">which</span> <span m="2592380">was</span>
  <span m="2592560">combine</span> <span m="2593190">high-quality</span> <span m="2593820">observational</span>
  <span m="2594510">data</span> <span m="2595230">with</span> <span m="2596550">advanced
  EPI</span> <span m="2596970">methods,</span> <span m="2597660">in</span> <span m="2597750">this</span>
  <span m="2597900">case</span> <span m="2598190">parametric</span> <span m="2598720">g-formula.</span>
  <span m="2600090">And</span> <span m="2600210">so</span> <span m="2600600">we</span>
  <span m="2600780">leveraged</span> <span m="2601280">data</span> <span m="2601620">from</span>
  <span m="2601890">the</span> <span m="2601980">Health</span> <span m="2602160">Professionals</span>
  <span m="2602730">Follow-up</span> <span m="2603000">Study,</span> <span m="2603510">which</span>
  <span m="2603690">is</span> <span m="2603810">a</span> <span m="2603870">well-characterized</span>
  <span m="2604890">prospective</span> <span m="2605430">cohort</span> <span m="2605820">study.</span></p><p><span
  m="2609670">So</span> <span m="2609740">in</span> <span m="2609860">these</span>
  <span m="2610070">cases,</span> <span m="2610670">there's</span> <span m="2611000">a</span>
  <span m="2611060">three-step</span> <span m="2611690">process</span> <span m="2612530">that</span>
  <span m="2612740">we</span> <span m="2612920">take</span> <span m="2613490">to</span>
  <span m="2613730">extract</span> <span m="2614540">the</span> <span m="2614690">most</span>
  <span m="2615080">meaningful</span> <span m="2616040">and</span> <span m="2616340">actionable</span>
  <span m="2617090">insights</span> <span m="2617810">from</span> <span m="2618230">observational</span>
  <span m="2618980">data.</span> <span m="2619980">So</span> <span m="2620030">the</span>
  <span m="2620120">first</span> <span m="2620450">thing</span> <span m="2620630">that</span>
  <span m="2620780">we</span> <span m="2620930">do</span> <span m="2621320">is</span>
  <span m="2621500">we</span> <span m="2621650">specify</span> <span m="2622400">the</span>
  <span m="2622490">protocol</span> <span m="2623570">of</span> <span m="2623720">the</span>
  <span m="2623810">target</span> <span m="2624230">trial</span> <span m="2624740">that</span>
  <span m="2624890">we</span> <span m="2625070">would</span> <span m="2625310">have</span>
  <span m="2625550">liked</span> <span m="2626060">to</span> <span m="2626210">conduct</span>
  <span m="2627080">had</span> <span m="2627350">it</span> <span m="2627470">been</span>
  <span m="2627770">feasible.</span></p><p><span m="2629420">The</span> <span m="2629540">second</span>
  <span m="2629900">thing</span> <span m="2630080">we</span> <span m="2630230">do</span>
  <span m="2630620">is</span> <span m="2630770">we</span> <span m="2630890">make</span>
  <span m="2631130">sure</span> <span m="2631340">that</span> <span m="2631490">we</span>
  <span m="2631640">measure</span> <span m="2632210">enough</span> <span m="2632540">covariates</span>
  <span m="2633470">to</span> <span m="2633710">approximately</span> <span m="2634670">adjust</span>
  <span m="2635090">for</span> <span m="2635240">confounding</span> <span m="2636500">and</span>
  <span m="2636770">achieve</span> <span m="2637280">conditional</span> <span m="2637850">exchangeability.</span>
  <span m="2639890">And</span> <span m="2640040">then</span> <span m="2640190">the</span>
  <span m="2640280">third</span> <span m="2640550">thing</span> <span m="2640730">we</span>
  <span m="2640850">do</span> <span m="2641060">is</span> <span m="2641180">we</span>
  <span m="2641330">apply</span> <span m="2641750">an</span> <span m="2641840">appropriate</span>
  <span m="2642440">method</span> <span m="2642920">to</span> <span m="2643070">compare</span>
  <span m="2643700">the</span> <span m="2643910">specified</span> <span m="2644510">treatment</span>
  <span m="2644930">strategies</span> <span m="2646040">under</span> <span m="2646370">this</span>
  <span m="2646580">assumption</span> <span m="2647360">of</span> <span m="2647690">conditional</span>
  <span m="2648200">exchangeability.</span></p><p><span m="2650670">And</span> <span
  m="2650820">so</span> <span m="2651090">in</span> <span m="2651210">this</span>
  <span m="2651450">case,</span> <span m="2652140">eligible</span> <span m="2652650">men</span>
  <span m="2652920">for</span> <span m="2653100">this</span> <span m="2653280">study</span>
  <span m="2653730">had</span> <span m="2653910">been</span> <span m="2654090">diagnosed</span>
  <span m="2654750">with</span> <span m="2654930">non-metastatic</span> <span m="2655830">prostate</span>
  <span m="2656280">cancer.</span> <span m="2657430">And</span> <span m="2657450">at</span>
  <span m="2657510">baseline,</span> <span m="2658140">they</span> <span m="2658260">were</span>
  <span m="2658440">free</span> <span m="2658980">of</span> <span m="2659310">cardiovascular</span>
  <span m="2660240">and</span> <span m="2660360">neurologic</span> <span m="2660870">conditions</span>
  <span m="2661470">that</span> <span m="2661650">may</span> <span m="2661920">limit</span>
  <span m="2662310">physical</span> <span m="2662760">ability.</span></p><p><span
  m="2664320">For</span> <span m="2664440">the</span> <span m="2664530">treatment</span>
  <span m="2664890">strategies,</span> <span m="2665670">men</span> <span m="2666030">were</span>
  <span m="2666240">to</span> <span m="2666450">initiate</span> <span m="2666990">one</span>
  <span m="2667350">of</span> <span m="2667530">six</span> <span m="2668220">physical</span>
  <span m="2668670">activity</span> <span m="2669150">strategies</span> <span m="2669990">at</span>
  <span m="2670200">diagnosis</span> <span m="2671520">and</span> <span m="2671790">continue</span>
  <span m="2672330">it</span> <span m="2672480">over</span> <span m="2672720">followup</span>
  <span m="2673410">until</span> <span m="2673920">the</span> <span m="2674070">development</span>
  <span m="2675360">of</span> <span m="2675510">a</span> <span m="2675570">condition</span>
  <span m="2676170">limiting</span> <span m="2676620">physical</span> <span m="2677040">activity.</span>
  <span m="2678010">So</span> <span m="2678090">this</span> <span m="2678330">is</span>
  <span m="2678480">what</span> <span m="2678720">made</span> <span m="2678990">the</span>
  <span m="2679080">strategies</span> <span m="2679770">dynamic.</span> <span m="2680900">The</span>
  <span m="2681060">intervention</span> <span m="2681690">over</span> <span m="2681930">time</span>
  <span m="2682470">depended</span> <span m="2683010">on</span> <span m="2683130">these</span>
  <span m="2683520">evolving</span> <span m="2684090">conditions.</span> <span m="2685620">And</span>
  <span m="2685770">so</span> <span m="2686100">just</span> <span m="2686310">to</span>
  <span m="2686370">note,</span> <span m="2686640">we</span> <span m="2687090">pre-specified</span>
  <span m="2688530">these</span> <span m="2688770">strategies</span> <span m="2689490">that</span>
  <span m="2689610">we</span> <span m="2689730">were</span> <span m="2689880">evaluating</span>
  <span m="2691670">as</span> <span m="2691850">well</span> <span m="2692000">as</span>
  <span m="2692090">the</span> <span m="2692180">conditions.</span></p><p><span m="2694040">Men</span>
  <span m="2694250">were</span> <span m="2694370">followed</span> <span m="2695030">until</span>
  <span m="2695510">diagnosis,</span> <span m="2696380">until</span> <span m="2696650">death,</span>
  <span m="2697230">and</span> <span m="2697310">to</span> <span m="2697400">followup</span>
  <span m="2697970">10</span> <span m="2698210">years</span> <span m="2698480">after</span>
  <span m="2698750">diagnosis</span> <span m="2699830">or</span> <span m="2699950">administrative</span>
  <span m="2700550">end</span> <span m="2700660">to</span> <span m="2700730">followup,</span>
  <span m="2701210">whichever</span> <span m="2701630">happened</span> <span m="2701960">first.</span>
  <span m="2702970">Our</span> <span m="2703130">outcome</span> <span m="2703460">of</span>
  <span m="2703580">interest</span> <span m="2703970">was</span> <span m="2704120">all</span>
  <span m="2704270">cause</span> <span m="2704570">mortality</span> <span m="2705140">within</span>
  <span m="2705440">10</span> <span m="2705740">years.</span> <span m="2707000">And</span>
  <span m="2707120">we</span> <span m="2707240">were</span> <span m="2707360">interested</span>
  <span m="2708080">in</span> <span m="2708320">estimating</span> <span m="2709010">the</span>
  <span m="2709190">per</span> <span m="2709430">protocol</span> <span m="2710000">effect</span>
  <span m="2710780">of</span> <span m="2710900">not</span> <span m="2711080">just</span>
  <span m="2711260">initiating</span> <span m="2711920">these</span> <span m="2712040">strategies</span>
  <span m="2712670">but</span> <span m="2712820">adhering</span> <span m="2713330">to</span>
  <span m="2713480">them</span> <span m="2713780">over</span> <span m="2714090">followup.</span>
  <span m="2715200">And</span> <span m="2715250">again,</span> <span m="2715490">we</span>
  <span m="2715610">applied</span> <span m="2715910">the</span> <span m="2716000">parametric</span>
  <span m="2716570">g-formula.</span></p><p><span m="2719760">So</span> <span m="2719910">I</span>
  <span m="2719970">think</span> <span m="2720150">you've</span> <span m="2720300">already</span>
  <span m="2720510">heard</span> <span m="2720750">about</span> <span m="2720960">the</span>
  <span m="2721020">g-formula</span> <span m="2721740">in</span> <span m="2721860">a</span>
  <span m="2721890">previous</span> <span m="2722370">lecture,</span> <span m="2723000">possibly</span>
  <span m="2723450">in</span> <span m="2723540">a</span> <span m="2723570">slightly</span>
  <span m="2723990">different</span> <span m="2724290">way.</span> <span m="2724720">So</span>
  <span m="2725310">I</span> <span m="2725400">won't</span> <span m="2725610">spend</span>
  <span m="2725820">too</span> <span m="2725970">much</span> <span m="2726180">time</span>
  <span m="2726420">on</span> <span m="2726540">this.</span> <span m="2726850">So</span>
  <span m="2728280">the</span> <span m="2728370">g-formula,</span> <span m="2729120">essentially</span>
  <span m="2729570">the</span> <span m="2729630">way</span> <span m="2729750">I</span>
  <span m="2729810">think</span> <span m="2730020">about</span> <span m="2730260">it</span>
  <span m="2730380">is</span> <span m="2730530">a</span> <span m="2730590">generalization</span>
  <span m="2731670">of</span> <span m="2731790">standardization</span> <span m="2733200">to</span>
  <span m="2733320">time</span> <span m="2733650">varying</span> <span m="2734130">exposures</span>
  <span m="2734970">and</span> <span m="2735150">confounders.</span></p><p><span m="2736380">So</span>
  <span m="2736590">it's</span> <span m="2736710">basically</span> <span m="2737340">a</span>
  <span m="2737430">weighted</span> <span m="2737820">average</span> <span m="2738360">of</span>
  <span m="2738540">risks,</span> <span m="2739530">where</span> <span m="2739710">you</span>
  <span m="2739830">can</span> <span m="2739980">think</span> <span m="2740220">of</span>
  <span m="2740340">the</span> <span m="2740430">weights</span> <span m="2740880">being</span>
  <span m="2741120">the</span> <span m="2741210">probability</span> <span m="2741870">density</span>
  <span m="2742320">functions</span> <span m="2742950">of</span> <span m="2743070">the</span>
  <span m="2743160">time</span> <span m="2743540">varying</span> <span m="2743910">confounders,</span>
  <span m="2745080">which</span> <span m="2745260">we</span> <span m="2745410">estimate</span>
  <span m="2745950">using</span> <span m="2746250">parametric</span> <span m="2746940">regression</span>
  <span m="2747390">models.</span> <span m="2748350">And</span> <span m="2748500">we</span>
  <span m="2748770">approximate</span> <span m="2749370">the</span> <span m="2749460">weighted</span>
  <span m="2749730">average</span> <span m="2750090">using</span> <span m="2750420">Monte</span>
  <span m="2750660">Carlo</span> <span m="2750990">simulation.</span></p><p><span
  m="2754110">So</span> <span m="2754880">practically</span> <span m="2755600">how</span>
  <span m="2755780">do</span> <span m="2755870">we</span> <span m="2755990">do</span>
  <span m="2756170">this?</span> <span m="2756840">So</span> <span m="2757040">the</span>
  <span m="2757130">first</span> <span m="2757370">thing</span> <span m="2757520">we</span>
  <span m="2757640">do</span> <span m="2757880">is</span> <span m="2758000">we</span>
  <span m="2758120">fit</span> <span m="2758450">parametric</span> <span m="2759110">regression</span>
  <span m="2759560">models</span> <span m="2760310">for</span> <span m="2760490">all</span>
  <span m="2760760">of</span> <span m="2760850">the</span> <span m="2760940">variables</span>
  <span m="2761780">that</span> <span m="2761930">we're</span> <span m="2762020">going</span>
  <span m="2762320">to</span> <span m="2762440">be</span> <span m="2762740">studying.</span>
  <span m="2763460">So</span> <span m="2763640">for</span> <span m="2763820">treatment</span>
  <span m="2764240">confounders</span> <span m="2764870">and</span> <span m="2764960">death</span>
  <span m="2765740">at</span> <span m="2765920">each</span> <span m="2766190">followup</span>
  <span m="2766760">time.</span></p><p><span m="2768690">The</span> <span m="2768790">next</span>
  <span m="2768920">thing</span> <span m="2769070">we</span> <span m="2769190">do</span>
  <span m="2769430">is</span> <span m="2769550">Monte</span> <span m="2769820">Carlo</span>
  <span m="2770120">simulation</span> <span m="2770840">where</span> <span m="2771020">essentially</span>
  <span m="2771620">what</span> <span m="2771770">we</span> <span m="2771890">want</span>
  <span m="2772040">to</span> <span m="2772130">do</span> <span m="2772310">is</span>
  <span m="2772580">simulate</span> <span m="2773450">the</span> <span m="2773660">outcome</span>
  <span m="2774170">distribution</span> <span m="2775880">under</span> <span m="2776480">each</span>
  <span m="2777530">treatment</span> <span m="2778010">strategy</span> <span m="2778760">that</span>
  <span m="2778910">we're</span> <span m="2779030">interested</span> <span m="2779600">in.</span>
  <span m="2781140">And</span> <span m="2781190">then</span> <span m="2781400">we</span>
  <span m="2781730">bootstrap</span> <span m="2782420">the</span> <span m="2782510">confidence</span>
  <span m="2783020">intervals.</span></p><p><span m="2785100">So</span> <span m="2785150">I'd</span>
  <span m="2785240">like</span> <span m="2785390">to</span> <span m="2785480">show</span>
  <span m="2785780">you</span> <span m="2785960">kind</span> <span m="2786200">of</span>
  <span m="2786320">in</span> <span m="2786440">a</span> <span m="2786530">schematic</span>
  <span m="2787430">what</span> <span m="2787610">this</span> <span m="2787820">looks</span>
  <span m="2788090">like,</span> <span m="2788360">because</span> <span m="2788540">it</span>
  <span m="2788660">might</span> <span m="2788870">be</span> <span m="2789050">a</span>
  <span m="2789110">little</span> <span m="2789290">bit</span> <span m="2789440">easier</span>
  <span m="2789770">to</span> <span m="2789890">see.</span> <span m="2791040">So</span>
  <span m="2791240">again,</span> <span m="2791570">the</span> <span m="2791690">idea</span>
  <span m="2792050">is</span> <span m="2792260">we're</span> <span m="2792410">going</span>
  <span m="2792490">to</span> <span m="2792620">make</span> <span m="2792800">copies</span>
  <span m="2793430">of</span> <span m="2793550">our</span> <span m="2793670">data</span>
  <span m="2793960">set,</span> <span m="2794600">where</span> <span m="2795050">in</span>
  <span m="2795350">each</span> <span m="2795680">copy</span> <span m="2796730">everyone</span>
  <span m="2797420">is</span> <span m="2797600">adhering</span> <span m="2798410">to</span>
  <span m="2798560">the</span> <span m="2798650">strategy</span> <span m="2799490">that</span>
  <span m="2799640">we're</span> <span m="2799730">focusing</span> <span m="2800300">on</span>
  <span m="2800530">in</span> <span m="2800720">that</span> <span m="2800930">copy.</span></p><p><span
  m="2802070">So</span> <span m="2802250">how</span> <span m="2802430">do</span> <span
  m="2802520">we</span> <span m="2802640">construct</span> <span m="2803240">each</span>
  <span m="2803510">of</span> <span m="2803600">these</span> <span m="2803780">copies</span>
  <span m="2804410">of</span> <span m="2804500">the</span> <span m="2804590">data</span>
  <span m="2804880">set?</span> <span m="2805650">We</span> <span m="2805670">have</span>
  <span m="2805760">to</span> <span m="2805880">build</span> <span m="2806270">them</span>
  <span m="2806540">each</span> <span m="2807020">from</span> <span m="2807350">the</span>
  <span m="2807440">ground</span> <span m="2807890">up,</span> <span m="2808350">starting</span>
  <span m="2808730">with</span> <span m="2808880">time</span> <span m="2809180">0.</span>
  <span m="2810290">So</span> <span m="2810470">the</span> <span m="2810590">values</span>
  <span m="2811310">of</span> <span m="2811490">all</span> <span m="2811760">of</span>
  <span m="2811850">the</span> <span m="2811940">time</span> <span m="2812210">varying</span>
  <span m="2812480">covariates</span> <span m="2813260">at</span> <span m="2813470">time</span>
  <span m="2813770">0</span> <span m="2814580">are</span> <span m="2814700">sampled</span>
  <span m="2815330">from</span> <span m="2815690">their</span> <span m="2815900">empirical</span>
  <span m="2816410">distribution.</span> <span m="2817320">So</span> <span m="2817420">these</span>
  <span m="2817520">are</span> <span m="2817610">actually</span> <span m="2818150">observed</span>
  <span m="2818750">values</span> <span m="2819380">of</span> <span m="2819530">the</span>
  <span m="2819620">covariates.</span></p><p><span m="2821780">How</span> <span m="2821960">do</span>
  <span m="2822020">we</span> <span m="2822170">get</span> <span m="2822800">the</span>
  <span m="2822920">values</span> <span m="2823670">at</span> <span m="2823820">the</span>
  <span m="2823910">next</span> <span m="2824240">time</span> <span m="2824540">point?</span>
  <span m="2825590">We</span> <span m="2825770">use</span> <span m="2826190">the</span>
  <span m="2826310">parametric</span> <span m="2827000">regression</span> <span m="2827450">models</span>
  <span m="2827900">that</span> <span m="2828050">I</span> <span m="2828110">mentioned</span>
  <span m="2828530">that</span> <span m="2828680">we</span> <span m="2828830">fit</span>
  <span m="2829160">in</span> <span m="2829310">step</span> <span m="2829670">1.</span>
  <span m="2832040">Then</span> <span m="2832280">what</span> <span m="2832430">we</span>
  <span m="2832550">do</span> <span m="2833120">is</span> <span m="2833390">we</span>
  <span m="2834470">force</span> <span m="2834920">the</span> <span m="2835070">level</span>
  <span m="2835670">of</span> <span m="2835820">the</span> <span m="2835970">intervention</span>
  <span m="2836900">variable</span> <span m="2837590">to</span> <span m="2837770">be</span>
  <span m="2837950">whatever</span> <span m="2838670">was</span> <span m="2838910">specified</span>
  <span m="2839870">by</span> <span m="2840110">that</span> <span m="2840350">intervention</span>
  <span m="2840920">strategy.</span> <span m="2843320">And</span> <span m="2843440">then</span>
  <span m="2843590">we</span> <span m="2843710">estimate</span> <span m="2844190">the</span>
  <span m="2844310">risk</span> <span m="2844730">of</span> <span m="2845210">the</span>
  <span m="2845390">outcome</span> <span m="2846260">at</span> <span m="2846410">each</span>
  <span m="2846650">time</span> <span m="2846890">period</span> <span m="2847400">given</span>
  <span m="2847820">these</span> <span m="2848120">variables,</span> <span m="2849890">again</span>
  <span m="2850190">using</span> <span m="2850520">the</span> <span m="2850610">parametric</span>
  <span m="2851180">regression</span> <span m="2851540">model</span> <span m="2851840">for</span>
  <span m="2851990">the</span> <span m="2852110">outcome</span> <span m="2852410">now.</span></p><p><span
  m="2853520">And</span> <span m="2853670">so</span> <span m="2853820">we</span> <span
  m="2853970">repeat</span> <span m="2854360">this</span> <span m="2854680">over</span>
  <span m="2854870">all</span> <span m="2855080">time</span> <span m="2855380">periods</span>
  <span m="2856070">to</span> <span m="2856190">estimate</span> <span m="2856790">a</span>
  <span m="2857230">cumulative</span> <span m="2857510">risk</span> <span m="2858410">under</span>
  <span m="2859100">that</span> <span m="2859340">strategy,</span> <span m="2860840">which</span>
  <span m="2861110">is</span> <span m="2861230">taken</span> <span m="2861680">as</span>
  <span m="2862190">the</span> <span m="2862490">average</span> <span m="2863180">of</span>
  <span m="2863390">the</span> <span m="2863510">subject-specific</span> <span m="2864620">risks.</span>
  <span m="2865650">So</span> <span m="2865700">this</span> <span m="2865880">is</span>
  <span m="2866030">what</span> <span m="2866270">I'm</span> <span m="2866480">doing.</span>
  <span m="2866750">This</span> <span m="2866930">is</span> <span m="2867020">kind</span>
  <span m="2867200">of</span> <span m="2867290">under</span> <span m="2867500">the</span>
  <span m="2867620">hood</span> <span m="2867890">what's</span> <span m="2868130">going</span>
  <span m="2868460">on</span> <span m="2868640">with</span> <span m="2869600">this</span>
  <span m="2869780">method.</span></p><p><span m="2870410">DAVID SONTAG:</span> <span
  m="2870455">So</span> <span m="2870500">maybe</span> <span m="2870790">we</span>
  <span m="2870890">should</span> <span m="2871010">try</span> <span m="2871130">to</span>
  <span m="2871220">put</span> <span m="2871370">that</span> <span m="2871490">in</span>
  <span m="2871590">language</span> <span m="2872000">of what we</span> <span m="2872375">saw
  in the</span> <span m="2872750">class.</span> <span m="2873890">And</span> <span
  m="2874490">let</span> <span m="2874640">me</span> <span m="2874730">know</span>
  <span m="2874790">if</span> <span m="2874880">I'm</span> <span m="2874970">getting</span>
  <span m="2875210">this</span> <span m="2875360">wrong.</span> <span m="2877770">So</span>
  <span m="2877850">you</span> <span m="2878240">first</span> <span m="2878540">estimate</span>
  <span m="2879020">the</span> <span m="2879220">markup</span> <span m="2879440">decision</span>
  <span m="2879800">process,</span> <span m="2882410">which</span> <span m="2883100">allows</span>
  <span m="2883460">you</span> <span m="2883850">to</span> <span m="2883940">simulate</span>
  <span m="2885250">from</span> <span m="2886160">the</span> <span m="2886550">underlying</span>
  <span m="2886855">data</span> <span m="2887160">distribution.</span></p><p><span
  m="2888020">So</span> <span m="2888230">you</span> <span m="2888860">know</span>
  <span m="2889190">that</span> <span m="2889520">probability</span> <span m="2890090">of</span>
  <span m="2890270">this</span> <span m="2890600">sort of next</span> <span m="2890930">sequence</span>
  <span m="2891350">of</span> <span m="2891440">observations,</span> <span m="2892960">given</span>
  <span m="2893650">the</span> <span m="2893750">previous</span> <span m="2894050">sequence</span>
  <span m="2894560">and</span> <span m="2895100">action</span> <span m="2895820">and</span>
  <span m="2896000">previous</span> <span m="2896450">actions,</span> <span m="2897710">and</span>
  <span m="2897800">then</span> <span m="2897950">with</span> <span m="2898130">that,</span>
  <span m="2898400">then</span> <span m="2898550">you</span> <span m="2898640">could</span>
  <span m="2900230">then</span> <span m="2900440">intervene</span> <span m="2900980">and</span>
  <span m="2901070">simulate the</span> <span m="2901460">forms.</span> <span m="2901930">Because</span>
  <span m="2902120">that</span> <span m="2902480">was,</span> <span m="2903080">if</span>
  <span m="2903190">you</span> <span m="2903250">remember</span> <span m="2903710">Frederick</span>
  <span m="2904100">gave</span> <span m="2904340">you</span> <span m="2904460">three</span>
  <span m="2904850">different</span> <span m="2905180">buckets</span> <span m="2906110">of</span>
  <span m="2906950">approaches.</span> <span m="2908040">Then</span> <span m="2908180">he</span>
  <span m="2908240">focused</span> <span m="2908570">on</span> <span m="2908660">the</span>
  <span m="2908750">middle</span> <span m="2909020">one.</span> <span m="2909540">This</span>
  <span m="2909620">is</span> <span m="2909740">the</span> <span m="2909830">left-most</span>
  <span m="2910470">bucket.</span> <span m="2911180">The right?</span></p><p><span
  m="2911710">AUDIENCE:</span> <span m="2911800">Yes.</span></p><p><span m="2913490">DAVID
  SONTAG:</span> <span m="2913625">So</span> <span m="2913760">we</span> <span m="2913880">didn't</span>
  <span m="2914120">talk</span> <span m="2914360">about</span> <span m="2914600">it.</span></p><p><span
  m="2914660">AUDIENCE:</span> <span m="2914830">No,</span> <span m="2915000">[INAUDIBLE]</span>
  <span m="2915340">model</span> <span m="2915630">based</span> <span m="2916023">on
  relevance.</span></p><p><span m="2916810">BARBRA DICKERMAN:</span> <span m="2916970">Yeah.</span>
  <span m="2917130">Yes.</span></p><p><span m="2918020">DAVID SONTAG:</span> <span
  m="2918110">But</span> <span m="2918200">it's</span> <span m="2918320">very</span>
  <span m="2918470">sensible.</span></p><p><span m="2921180">AUDIENCE:</span> <span
  m="2921235">Yeah.</span> <span m="2921530">But it</span> <span m="2921800">seems</span>
  <span m="2922100">very</span> <span m="2922400">hard.</span></p><p><span m="2924140">BARBRA
  DICKERMAN:</span> <span m="2924245">What's</span> <span m="2924350">that?</span></p><p><span
  m="2925220">AUDIENCE:</span> <span m="2925570">Sorry.</span> <span m="2926080">Oh,</span>
  <span m="2926260">it</span> <span m="2926320">seems</span> <span m="2926680">very</span>
  <span m="2926920">hard</span> <span m="2927220">to</span> <span m="2927410">model</span>
  <span m="2927790">this</span> <span m="2928120">[INAUDIBLE].</span></p><p><span
  m="2929530">BARBRA DICKERMAN:</span> <span m="2929750">Yeah.</span> <span m="2929970">So</span>
  <span m="2930220">that</span> <span m="2930430">is</span> <span m="2930550">a</span>
  <span m="2930580">challenge.</span> <span m="2931150">That</span> <span m="2931330">is</span>
  <span m="2931450">the</span> <span m="2931510">hardest</span> <span m="2931810">part</span>
  <span m="2932020">about</span> <span m="2932260">this.</span> <span m="2933370">And</span>
  <span m="2933520">it's</span> <span m="2933670">relying</span> <span m="2934060">on</span>
  <span m="2934180">a</span> <span m="2934210">lot</span> <span m="2934420">of</span>
  <span m="2934510">assumptions,</span> <span m="2935590">yeah.</span> <span m="2939530">So</span>
  <span m="2939950">the</span> <span m="2940070">primary</span> <span m="2940790">results</span>
  <span m="2941640">that</span> <span m="2941780">kind</span> <span m="2941960">of</span>
  <span m="2942050">come</span> <span m="2942290">out</span> <span m="2942500">after</span>
  <span m="2942740">we</span> <span m="2942860">do</span> <span m="2943100">all</span>
  <span m="2943280">of</span> <span m="2943370">this.</span> <span m="2944640">So</span>
  <span m="2944690">this</span> <span m="2944840">is</span> <span m="2944960">the</span>
  <span m="2945110">estimated</span> <span m="2945680">risk</span> <span m="2946280">of</span>
  <span m="2946640">all</span> <span m="2946790">cause</span> <span m="2947030">mortality</span>
  <span m="2947720">under</span> <span m="2948110">several</span> <span m="2948470">physical</span>
  <span m="2948860">activity</span> <span m="2949340">interventions.</span></p><p><span
  m="2950780">So</span> <span m="2951710">I'm</span> <span m="2951830">not</span>
  <span m="2951920">going</span> <span m="2952040">to</span> <span m="2952100">focus</span>
  <span m="2952370">too</span> <span m="2952520">much</span> <span m="2952730">on</span>
  <span m="2952820">the</span> <span m="2952910">results.</span> <span m="2953390">I</span>
  <span m="2953450">want</span> <span m="2953570">to</span> <span m="2953630">focus</span>
  <span m="2953960">on</span> <span m="2954410">two</span> <span m="2954680">main</span>
  <span m="2955370">takeaways</span> <span m="2955880">from</span> <span m="2956060">this</span>
  <span m="2956150">slide.</span> <span m="2957120">One</span> <span m="2957560">thing</span>
  <span m="2957800">to</span> <span m="2957890">emphasize</span> <span m="2958520">is</span>
  <span m="2958670">we</span> <span m="2958970">pre-specified</span> <span m="2960680">the</span>
  <span m="2960800">weekly</span> <span m="2961220">duration</span> <span m="2961820">of</span>
  <span m="2961910">physical</span> <span m="2962390">activity.</span> <span m="2963450">Or</span>
  <span m="2963470">you</span> <span m="2963560">can</span> <span m="2963680">think</span>
  <span m="2963890">of</span> <span m="2963980">this</span> <span m="2964250">like</span>
  <span m="2964430">the</span> <span m="2964550">dose</span> <span m="2965090">of</span>
  <span m="2965210">the</span> <span m="2965360">intervention.</span></p><p><span
  m="2966200">We</span> <span m="2966440">pre-specified</span> <span m="2967190">that.</span>
  <span m="2967850">And</span> <span m="2968000">this</span> <span m="2968180">was</span>
  <span m="2968330">based</span> <span m="2968840">on</span> <span m="2969110">current</span>
  <span m="2969470">guidelines.</span> <span m="2970730">So</span> <span m="2970880">the</span>
  <span m="2971000">third</span> <span m="2971360">row</span> <span m="2971690">of</span>
  <span m="2971810">each</span> <span m="2972050">band,</span> <span m="2972620">we</span>
  <span m="2972830">did</span> <span m="2973070">look</span> <span m="2973400">at</span>
  <span m="2973550">some</span> <span m="2973970">dose</span> <span m="2974450">or</span>
  <span m="2974570">level</span> <span m="2974960">beyond</span> <span m="2975410">the</span>
  <span m="2975500">guidelines</span> <span m="2976610">to</span> <span m="2976730">see</span>
  <span m="2976940">if</span> <span m="2977030">there</span> <span m="2977210">might</span>
  <span m="2977570">be</span> <span m="2977750">additional</span> <span m="2978260">survival</span>
  <span m="2978830">benefits.</span> <span m="2980060">But</span> <span m="2980210">these</span>
  <span m="2980390">were</span> <span m="2980480">all</span> <span m="2980570">pre-specified.</span></p><p><span
  m="2981930">We</span> <span m="2982010">also</span> <span m="2982370">pre-specified</span>
  <span m="2983570">all</span> <span m="2983840">of</span> <span m="2983930">the</span>
  <span m="2984020">time</span> <span m="2984350">varying</span> <span m="2984680">covariates</span>
  <span m="2985430">that</span> <span m="2985610">made</span> <span m="2985940">these</span>
  <span m="2986150">strategies</span> <span m="2986840">dynamic.</span> <span m="2987890">So</span>
  <span m="2988010">I</span> <span m="2988070">mentioned</span> <span m="2988490">that</span>
  <span m="2988640">men</span> <span m="2988910">were</span> <span m="2989060">excused</span>
  <span m="2989780">from</span> <span m="2989930">following</span> <span m="2990590">the</span>
  <span m="2990710">recommended</span> <span m="2991370">physical</span> <span m="2991760">activity</span>
  <span m="2992210">levels</span> <span m="2993050">if</span> <span m="2993260">they</span>
  <span m="2993440">developed</span> <span m="2994010">one</span> <span m="2994310">of</span>
  <span m="2994430">these</span> <span m="2994730">listed</span> <span m="2995150">conditions,</span>
  <span m="2996140">metastasis,</span> <span m="2996575">MI,</span> <span m="2997430">stroke,</span>
  <span m="2997960">et</span> <span m="2998240">cetera.</span> <span m="2999470">We</span>
  <span m="2999620">pre-specified</span> <span m="3000370">all</span> <span m="3000550">of</span>
  <span m="3000670">those.</span> <span m="3001060">It's</span> <span m="3001180">possible</span>
  <span m="3001810">that</span> <span m="3002060">maybe</span> <span m="3003280">a</span>
  <span m="3003370">different</span> <span m="3004330">dependence</span> <span m="3005020">on</span>
  <span m="3005110">a</span> <span m="3005170">different</span> <span m="3005470">time</span>
  <span m="3005680">varying</span> <span m="3005920">covariate</span> <span m="3006370">may</span>
  <span m="3006520">have</span> <span m="3006700">led</span> <span m="3006910">to</span>
  <span m="3007060">a</span> <span m="3007120">more</span> <span m="3007480">optimal</span>
  <span m="3007960">strategy.</span> <span m="3008860">There</span> <span m="3008980">was</span>
  <span m="3009100">a</span> <span m="3009130">lot</span> <span m="3009400">that</span>
  <span m="3009520">remained</span> <span m="3010000">unexplored.</span></p><p><span
  m="3013560">So</span> <span m="3013860">we</span> <span m="3014010">did</span> <span
  m="3014310">a</span> <span m="3014370">lot</span> <span m="3014850">of</span> <span
  m="3015240">sensitivity</span> <span m="3016020">analyses</span> <span m="3016830">as</span>
  <span m="3017010">part</span> <span m="3017370">of</span> <span m="3017550">this</span>
  <span m="3018480">project.</span> <span m="3019500">I'd</span> <span m="3019590">like</span>
  <span m="3019740">to</span> <span m="3019830">focus,</span> <span m="3020350">though,</span>
  <span m="3020710">on</span> <span m="3020730">the</span> <span m="3020970">sensitivity</span>
  <span m="3021510">analyses</span> <span m="3021930">that</span> <span m="3022050">we</span>
  <span m="3022200">did</span> <span m="3022530">for</span> <span m="3022830">potential</span>
  <span m="3023490">unmeasured</span> <span m="3024090">confounding</span> <span m="3025200">by</span>
  <span m="3025500">chronic</span> <span m="3025950">disease</span> <span m="3027090">that</span>
  <span m="3027300">may</span> <span m="3027570">be</span> <span m="3027780">severe</span>
  <span m="3028290">enough</span> <span m="3028680">to</span> <span m="3028860">affect</span>
  <span m="3029400">both</span> <span m="3029820">physical</span> <span m="3030270">activity</span>
  <span m="3031230">and</span> <span m="3031640">survival.</span></p><p><span m="3033280">And</span>
  <span m="3033330">so</span> <span m="3033600">the</span> <span m="3033720">g-formula</span>
  <span m="3034440">is</span> <span m="3034590">actually</span> <span m="3035010">providing</span>
  <span m="3035880">a</span> <span m="3035940">natural</span> <span m="3036540">way</span>
  <span m="3036870">to</span> <span m="3037020">at</span> <span m="3037140">least</span>
  <span m="3037440">partly</span> <span m="3038010">address</span> <span m="3038460">this</span>
  <span m="3039210">by</span> <span m="3039480">estimating</span> <span m="3040110">the</span>
  <span m="3040200">risk</span> <span m="3040710">of</span> <span m="3040950">these</span>
  <span m="3041580">physical</span> <span m="3041940">activity</span> <span m="3042330">interventions</span>
  <span m="3044660">that</span> <span m="3044900">are</span> <span m="3045170">at</span>
  <span m="3045410">each</span> <span m="3045650">time</span> <span m="3045950">point</span>
  <span m="3046250">t</span> <span m="3046670">only</span> <span m="3047030">applied</span>
  <span m="3047750">to</span> <span m="3047900">men</span> <span m="3048290">who</span>
  <span m="3048590">are</span> <span m="3048890">healthy</span> <span m="3049430">enough</span>
  <span m="3049970">to</span> <span m="3050150">maintain</span> <span m="3050690">a</span>
  <span m="3050780">physical</span> <span m="3051170">activity</span> <span m="3051650">level</span>
  <span m="3052130">at</span> <span m="3052310">that</span> <span m="3052490">time.</span>
  <span m="3053760">And</span> <span m="3053860">so</span> <span m="3053870">again</span>
  <span m="3054140">in</span> <span m="3054200">the</span> <span m="3054290">main</span>
  <span m="3054470">analysis,</span> <span m="3055070">we</span> <span m="3055250">excused</span>
  <span m="3055850">men</span> <span m="3056150">from</span> <span m="3056360">following</span>
  <span m="3057080">the</span> <span m="3057320">recommended</span> <span m="3057890">levels</span>
  <span m="3058400">if</span> <span m="3058550">they</span> <span m="3058670">developed</span>
  <span m="3059210">one</span> <span m="3059480">of</span> <span m="3059630">these</span>
  <span m="3059900">serious</span> <span m="3060470">conditions.</span></p><p><span
  m="3063020">So</span> <span m="3063230">in</span> <span m="3063350">sensitivity</span>
  <span m="3064040">analyses,</span> <span m="3064830">we</span> <span m="3064910">then</span>
  <span m="3065180">expanded</span> <span m="3066020">this</span> <span m="3066260">list</span>
  <span m="3066800">of</span> <span m="3066980">serious</span> <span m="3067490">conditions</span>
  <span m="3068180">to</span> <span m="3068330">also</span> <span m="3068720">include</span>
  <span m="3069170">the</span> <span m="3069890">conditions</span> <span m="3070490">that</span>
  <span m="3070640">are</span> <span m="3070730">shown</span> <span m="3071090">in</span>
  <span m="3071210">blue</span> <span m="3071510">text.</span> <span m="3072590">And</span>
  <span m="3072710">so</span> <span m="3072860">this</span> <span m="3073100">attenuated</span>
  <span m="3073730">our</span> <span m="3073850">estimates</span> <span m="3074490">but</span>
  <span m="3074510">didn't</span> <span m="3074720">change</span> <span m="3075110">our</span>
  <span m="3075260">conclusions.</span></p><p><span m="3077120">One</span> <span m="3077330">thing</span>
  <span m="3077540">to</span> <span m="3077660">point</span> <span m="3077930">out</span>
  <span m="3078200">is</span> <span m="3078410">that</span> <span m="3078800">the</span>
  <span m="3078950">validity</span> <span m="3079820">of</span> <span m="3079970">this</span>
  <span m="3080210">approach</span> <span m="3081620">rests</span> <span m="3082190">on</span>
  <span m="3082340">the</span> <span m="3082460">assumption</span> <span m="3083240">that</span>
  <span m="3083840">at</span> <span m="3083990">each</span> <span m="3084260">time</span>
  <span m="3084590">t</span> <span m="3085070">we</span> <span m="3085310">had</span>
  <span m="3085700">available</span> <span m="3086330">data</span> <span m="3087350">needed</span>
  <span m="3088100">to</span> <span m="3088340">identify</span> <span m="3089960">which</span>
  <span m="3090350">men</span> <span m="3090680">were</span> <span m="3090800">healthy</span>
  <span m="3091250">at</span> <span m="3091520">that</span> <span m="3091730">time</span>
  <span m="3092150">enough</span> <span m="3092600">to</span> <span m="3092780">do</span>
  <span m="3092960">the</span> <span m="3093050">physical</span> <span m="3093410">activity.</span>
  <span m="3094230">Yeah.</span></p><p><span m="3094440">AUDIENCE:</span> <span m="3094630">Sorry,</span>
  <span m="3094820">just to</span> <span m="3095200">double-check,</span> <span m="3095580">does</span>
  <span m="3095960">excuse</span> <span m="3096560">mean</span> <span m="3096720">that</span>
  <span m="3096830">you</span> <span m="3097310">remove them?</span></p><p><span m="3098270">BARBRA
  DICKERMAN:</span> <span m="3098375">Great</span> <span m="3098480">question.</span>
  <span m="3099110">So</span> <span m="3100580">because</span> <span m="3101060">the</span>
  <span m="3101180">strategy</span> <span m="3101690">was</span> <span m="3101840">pre-specified</span>
  <span m="3102590">to</span> <span m="3102710">say</span> <span m="3102980">that</span>
  <span m="3103190">if</span> <span m="3103430">you</span> <span m="3103550">develop</span>
  <span m="3103940">one</span> <span m="3104120">of</span> <span m="3104180">these</span>
  <span m="3104390">conditions,</span> <span m="3105950">you</span> <span m="3106280">may</span>
  <span m="3107300">essentially</span> <span m="3107840">do</span> <span m="3108230">whatever</span>
  <span m="3108770">level</span> <span m="3109130">of</span> <span m="3109190">physical</span>
  <span m="3109550">activity</span> <span m="3110090">you're</span> <span m="3110300">able</span>
  <span m="3110660">to</span> <span m="3110780">do.</span> <span m="3111440">So</span>
  <span m="3111650">importantly--</span> <span m="3112440">I'm</span> <span m="3112460">glad</span>
  <span m="3112700">you</span> <span m="3112790">brought</span> <span m="3113000">this</span>
  <span m="3113180">up--</span> <span m="3113690">we</span> <span m="3113870">did</span>
  <span m="3113990">not</span> <span m="3114290">censor</span> <span m="3114920">men</span>
  <span m="3115490">at</span> <span m="3115670">that</span> <span m="3115850">time.</span>
  <span m="3116420">They</span> <span m="3116540">were</span> <span m="3116690">still</span>
  <span m="3117020">followed,</span> <span m="3117500">because</span> <span m="3117830">they</span>
  <span m="3117950">were</span> <span m="3118040">still</span> <span m="3119000">adhering</span>
  <span m="3119690">to</span> <span m="3119930">the</span> <span m="3120020">strategy</span>
  <span m="3120620">as</span> <span m="3120860">defined.</span> <span m="3122330">Thanks</span>
  <span m="3122570">for</span> <span m="3122690">asking.</span></p><p><span m="3125060">And</span>
  <span m="3125240">so</span> <span m="3126800">given</span> <span m="3127130">that</span>
  <span m="3127250">we</span> <span m="3127370">don't</span> <span m="3127580">know</span>
  <span m="3127880">whether</span> <span m="3128240">the</span> <span m="3128330">data</span>
  <span m="3128630">contain</span> <span m="3129290">at</span> <span m="3129440">each</span>
  <span m="3129650">time</span> <span m="3129920">t</span> <span m="3130430">the</span>
  <span m="3130670">information</span> <span m="3131570">necessary</span> <span m="3132740">to</span>
  <span m="3132890">know,</span> <span m="3133290">are</span> <span m="3133340">these</span>
  <span m="3133550">men</span> <span m="3133790">healthy</span> <span m="3134090">enough</span>
  <span m="3134360">at</span> <span m="3134570">that</span> <span m="3134750">time,</span>
  <span m="3135530">we</span> <span m="3135650">therefore</span> <span m="3136070">conducted</span>
  <span m="3136640">a</span> <span m="3136700">few</span> <span m="3137030">alternate</span>
  <span m="3137540">analyses</span> <span m="3138290">in</span> <span m="3138410">which</span>
  <span m="3138650">we</span> <span m="3138800">lagged</span> <span m="3139610">physical</span>
  <span m="3140000">activity</span> <span m="3140600">and</span> <span m="3140880">covariate</span>
  <span m="3141290">data</span> <span m="3141560">by</span> <span m="3141710">two</span>
  <span m="3141980">years.</span> <span m="3142880">And</span> <span m="3143000">we</span>
  <span m="3143150">also</span> <span m="3143510">used</span> <span m="3143930">a</span>
  <span m="3144020">negative</span> <span m="3144470">outcome</span> <span m="3144950">control</span>
  <span m="3145580">to</span> <span m="3145760">explore</span> <span m="3146690">potential</span>
  <span m="3147320">unmeasured</span> <span m="3147920">confounding</span> <span m="3148670">by</span>
  <span m="3148820">clinical</span> <span m="3149270">disease</span> <span m="3149810">or</span>
  <span m="3149960">disease</span> <span m="3150440">severity.</span></p><p><span
  m="3151950">So</span> <span m="3152000">what's</span> <span m="3152180">the</span>
  <span m="3152270">rationale</span> <span m="3152810">behind</span> <span m="3153110">this?</span>
  <span m="3153440">So</span> <span m="3154420">in</span> <span m="3154610">the</span>
  <span m="3154670">DAGs</span> <span m="3155000">below</span> <span m="3155360">for</span>
  <span m="3155480">the</span> <span m="3155630">original</span> <span m="3156050">analysis,</span>
  <span m="3156770">we</span> <span m="3157010">have</span> <span m="3157790">physical</span>
  <span m="3158180">activity</span> <span m="3158690">A.</span> <span m="3159590">We</span>
  <span m="3159740">have</span> <span m="3159860">survival</span> <span m="3160450">Y.</span>
  <span m="3161120">And</span> <span m="3161420">this</span> <span m="3161660">may</span>
  <span m="3161870">be</span> <span m="3162050">confounded</span> <span m="3162860">by</span>
  <span m="3163430">disease</span> <span m="3163850">severity</span> <span m="3164450">U.</span>
  <span m="3165590">So</span> <span m="3165770">when</span> <span m="3165920">we</span>
  <span m="3166040">see</span> <span m="3166310">an</span> <span m="3166400">association</span>
  <span m="3167210">between</span> <span m="3167540">A and</span> <span m="3167790">Y</span>
  <span m="3168170">in</span> <span m="3168380">our</span> <span m="3168470">data,</span>
  <span m="3169250">we</span> <span m="3169370">want</span> <span m="3169520">to</span>
  <span m="3169580">make</span> <span m="3169760">sure</span> <span m="3170000">that</span>
  <span m="3170210">it's</span> <span m="3170450">causal,</span> <span m="3171070">that</span>
  <span m="3171200">it's</span> <span m="3171350">because</span> <span m="3171650">of</span>
  <span m="3171740">the</span> <span m="3171830">blue</span> <span m="3172190">arrow,</span>
  <span m="3173000">and</span> <span m="3173120">not</span> <span m="3173330">because</span>
  <span m="3173690">of</span> <span m="3173810">this</span> <span m="3174020">confounding</span>
  <span m="3174710">bias,</span> <span m="3175280">the</span> <span m="3175400">red</span>
  <span m="3175670">arrow.</span></p><p><span m="3176640">So</span> <span m="3176690">how</span>
  <span m="3176900">can</span> <span m="3177080">we</span> <span m="3177410">potentially</span>
  <span m="3178130">provide</span> <span m="3178610">evidence</span> <span m="3179120">for</span>
  <span m="3179300">whether</span> <span m="3179660">that</span> <span m="3180260">red</span>
  <span m="3180710">pathway</span> <span m="3181340">is</span> <span m="3181550">there?</span>
  <span m="3182480">We</span> <span m="3182660">selected</span> <span m="3183260">questionnaire</span>
  <span m="3184020">nonresponse</span> <span m="3185000">as</span> <span m="3185270">an</span>
  <span m="3185450">alternate</span> <span m="3186050">outcome,</span> <span m="3187190">instead</span>
  <span m="3187550">of</span> <span m="3187610">survival,</span> <span m="3188750">that</span>
  <span m="3189410">we</span> <span m="3189620">assumed</span> <span m="3190340">was</span>
  <span m="3190580">not</span> <span m="3190850">directly</span> <span m="3191540">affected</span>
  <span m="3192350">by</span> <span m="3192560">physical</span> <span m="3192980">activity,</span>
  <span m="3193940">but</span> <span m="3194090">that</span> <span m="3194270">we</span>
  <span m="3194420">thought</span> <span m="3194900">would</span> <span m="3195200">be</span>
  <span m="3195350">similarly</span> <span m="3196040">confounded</span> <span m="3196820">by</span>
  <span m="3197060">disease</span> <span m="3197480">severity.</span></p><p><span
  m="3199230">And</span> <span m="3199280">so</span> <span m="3199490">when</span>
  <span m="3199670">we</span> <span m="3199790">repeated</span> <span m="3200210">the</span>
  <span m="3200360">analysis</span> <span m="3200870">with</span> <span m="3201040">a</span>
  <span m="3201080">negative</span> <span m="3201440">outcome</span> <span m="3201800">control,</span>
  <span m="3203030">we</span> <span m="3203270">found</span> <span m="3203660">that</span>
  <span m="3203780">physical</span> <span m="3204110">activity</span> <span m="3204590">had</span>
  <span m="3204780">a</span> <span m="3204840">nearly</span> <span m="3205250">null</span>
  <span m="3205580">effect</span> <span m="3206000">on</span> <span m="3206120">questionnaire</span>
  <span m="3206600">nonresponse,</span> <span m="3207290">as</span> <span m="3207530">we</span>
  <span m="3207680">would</span> <span m="3207890">expect,</span> <span m="3208940">which</span>
  <span m="3209180">provides</span> <span m="3209650">some</span> <span m="3209930">support</span>
  <span m="3210920">that</span> <span m="3211310">in</span> <span m="3211490">our</span>
  <span m="3211610">original</span> <span m="3212120">analysis,</span> <span m="3214400">the</span>
  <span m="3214460">effect</span> <span m="3214690">of</span> <span m="3214760">physical</span>
  <span m="3215030">activity</span> <span m="3215420">on</span> <span m="3215570">death</span>
  <span m="3216020">was</span> <span m="3216230">not</span> <span m="3216470">confounded</span>
  <span m="3217040">through</span> <span m="3217430">the</span> <span m="3217550">pathways</span>
  <span m="3218180">explored</span> <span m="3219380">through</span> <span m="3219530">the</span>
  <span m="3219650">negative</span> <span m="3220010">control.</span></p><p><span
  m="3222000">So</span> <span m="3222020">one</span> <span m="3222170">thing</span>
  <span m="3222320">to</span> <span m="3222410">highlight</span> <span m="3222770">here</span>
  <span m="3223040">is</span> <span m="3223190">the</span> <span m="3223310">sensitivity</span>
  <span m="3223910">analyses</span> <span m="3224420">were</span> <span m="3224540">driven</span>
  <span m="3224990">by</span> <span m="3225440">our</span> <span m="3225710">subject</span>
  <span m="3226220">matter</span> <span m="3226520">knowledge.</span> <span m="3227820">And</span>
  <span m="3227870">there's</span> <span m="3228170">nothing</span> <span m="3228680">in</span>
  <span m="3228890">the</span> <span m="3229010">data</span> <span m="3229730">that</span>
  <span m="3229880">kind</span> <span m="3230090">of</span> <span m="3230210">drove</span>
  <span m="3230660">this.</span></p><p><span m="3233700">And</span> <span m="3233800">so</span>
  <span m="3233850">just</span> <span m="3234060">to</span> <span m="3234180">recap</span>
  <span m="3235230">this</span> <span m="3235440">portion.</span> <span m="3235980">So</span>
  <span m="3236130">g-methods</span> <span m="3237630">are</span> <span m="3237810">a</span>
  <span m="3237840">useful</span> <span m="3238230">tool,</span> <span m="3238620">because</span>
  <span m="3239010">they</span> <span m="3239160">let</span> <span m="3239370">us</span>
  <span m="3239490">validly</span> <span m="3240150">estimate</span> <span m="3240690">the</span>
  <span m="3240810">effect</span> <span m="3241710">of</span> <span m="3241980">pre-specified</span>
  <span m="3243510">dynamic</span> <span m="3244110">strategies</span> <span m="3245490">and</span>
  <span m="3245640">estimate</span> <span m="3246300">adjusted</span> <span m="3246780">absolute</span>
  <span m="3247230">risks,</span> <span m="3247710">which</span> <span m="3247920">are</span>
  <span m="3247980">clinically</span> <span m="3248460">meaningful</span> <span m="3248940">to</span>
  <span m="3249060">us,</span> <span m="3250090">and</span> <span m="3250170">appropriately</span>
  <span m="3250710">adjusted</span> <span m="3251100">survival</span> <span m="3251520">curves,</span>
  <span m="3252270">even</span> <span m="3252570">in</span> <span m="3252660">the</span>
  <span m="3252720">presence</span> <span m="3253260">of</span> <span m="3253470">treatment</span>
  <span m="3253860">confounder</span> <span m="3254370">feedback,</span> <span m="3255270">which</span>
  <span m="3255990">occurs</span> <span m="3256410">often</span> <span m="3256860">in</span>
  <span m="3256980">clinical</span> <span m="3258480">questions.</span> <span m="3259770">And</span>
  <span m="3259890">of</span> <span m="3259980">course,</span> <span m="3260250">this</span>
  <span m="3260430">is</span> <span m="3260550">under</span> <span m="3260880">our</span>
  <span m="3261060">typical</span> <span m="3262170">identifiability</span> <span
  m="3263100">assumptions.</span></p><p><span m="3265020">So</span> <span m="3265170">this</span>
  <span m="3265350">makes</span> <span m="3265620">it</span> <span m="3265710">a</span>
  <span m="3265770">powerful</span> <span m="3266250">approach</span> <span m="3266700">to</span>
  <span m="3266820">estimate</span> <span m="3267240">the</span> <span m="3267360">effects</span>
  <span m="3267690">of</span> <span m="3267810">currently</span> <span m="3268320">recommended</span>
  <span m="3269070">or</span> <span m="3269280">proposed</span> <span m="3269700">strategies</span>
  <span m="3270420">that</span> <span m="3270540">therefore</span> <span m="3271080">we</span>
  <span m="3271320">can</span> <span m="3271770">specify</span> <span m="3272730">and</span>
  <span m="3273180">write</span> <span m="3273570">out</span> <span m="3273750">precisely</span>
  <span m="3274380">as</span> <span m="3274530">we</span> <span m="3274650">did</span>
  <span m="3274860">here.</span> <span m="3276000">However,</span> <span m="3276600">these</span>
  <span m="3276900">pre-specified</span> <span m="3277620">strategies</span> <span
  m="3278280">may</span> <span m="3278550">not</span> <span m="3278910">be</span>
  <span m="3279630">the</span> <span m="3279780">optimal</span> <span m="3280470">strategies.</span></p><p><span
  m="3281740">So</span> <span m="3281790">again,</span> <span m="3283060">when</span>
  <span m="3283080">I</span> <span m="3283140">was</span> <span m="3283230">doing</span>
  <span m="3283500">this</span> <span m="3283650">analysis,</span> <span m="3284310">I</span>
  <span m="3284370">was</span> <span m="3284520">thinking</span> <span m="3285370">there</span>
  <span m="3285530">are</span> <span m="3285630">so</span> <span m="3285900">many</span>
  <span m="3286140">different</span> <span m="3286800">weekly</span> <span m="3287250">durations</span>
  <span m="3287790">of</span> <span m="3287850">physical</span> <span m="3288180">activity</span>
  <span m="3288720">that</span> <span m="3288840">we're</span> <span m="3288960">not</span>
  <span m="3289260">looking</span> <span m="3289650">at.</span> <span m="3290320">There
  are</span> <span m="3290370">so</span> <span m="3290640">many</span> <span m="3290850">different</span>
  <span m="3291210">time-varying</span> <span m="3292150">covariates</span> <span
  m="3293550">where</span> <span m="3293760">we</span> <span m="3293910">could</span>
  <span m="3294120">have</span> <span m="3294270">different</span> <span m="3294690">dependencies</span>
  <span m="3295770">on</span> <span m="3296010">those</span> <span m="3296430">for</span>
  <span m="3296580">these</span> <span m="3296730">strategies</span> <span m="3297300">over</span>
  <span m="3297720">time.</span> <span m="3298080">And</span> <span m="3298170">maybe</span>
  <span m="3298500">those</span> <span m="3298800">would</span> <span m="3299040">have</span>
  <span m="3299250">led</span> <span m="3299940">to</span> <span m="3300120">better</span>
  <span m="3300450">survival</span> <span m="3300960">outcomes</span> <span m="3301530">among</span>
  <span m="3301800">these</span> <span m="3302010">men,</span> <span m="3302610">but</span>
  <span m="3302790">all</span> <span m="3302970">of</span> <span m="3303060">that</span>
  <span m="3303450">was</span> <span m="3303810">unexplored.</span></p>
type: course
uid: 6173239e857ad3f825f77bdca48adbaf

---
None