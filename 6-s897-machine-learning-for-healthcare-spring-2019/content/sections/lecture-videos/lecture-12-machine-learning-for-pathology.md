---
about_this_resource_text: '<p>Dr. Beck begins with a short background of pathology
  and his work at PathAI. He then discusses computational pathology, building image
  processing models, and precision immunotherapy.</p><p>Speaker: Andy Beck</p><p><a
  href="./resolveuid/5b28c3a5a47a51faf2c97f17d2a8f5a1">Lecture 12: Machine Learning
  for Pathology slides (PDF - 6.5MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: PKCMH5KOcxQ
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: Video-YouTube-Stream
  type: Video
  uid: 01165de782e0b7a7cf1c0e81562a6816
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/PKCMH5KOcxQ/default.jpg
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: eece2a1e643079fd298fd8adb595620d
- id: 3Play-3PlayYouTubeid-MP4
  media_location: PKCMH5KOcxQ
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: 21d03d5f1568d79b950ef06695c48f46
- id: PKCMH5KOcxQ.srt
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-12-machine-learning-for-pathology/PKCMH5KOcxQ.srt
  title: 3play caption file
  type: null
  uid: 80afa2005fb58b70e11399a2e03e5cc4
- id: PKCMH5KOcxQ.pdf
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-12-machine-learning-for-pathology/PKCMH5KOcxQ.pdf
  title: 3play pdf file
  type: null
  uid: 2f44215dbbf6a90a539694f1a8bca4b5
- id: Caption-3Play YouTube id-SRT
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 1d2a76ff13b879f975f3e4abe47edd4d
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 342fcf1d137cc5d6fb1b092d4936e0ef
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec12_300k.mp4
  parent_uid: 657574bd0575b7aa68db5dfea1969336
  title: Video-Internet Archive-MP4
  type: Video
  uid: e662ea7e95c76fdcf2e0df70177f230b
inline_embed_id: 83474569lecture12machinelearningforpathology98608231
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-12-machine-learning-for-pathology
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-12-machine-learning-for-pathology
template_type: Tabbed
title: 'Lecture 12: Machine Learning for Pathology'
transcript: <p><span m="15350">PROFESSOR:</span> <span m="15380">All</span> <span
  m="15410">right,</span> <span m="15560">everyone,</span> <span m="16860">so</span>
  <span m="17210">we</span> <span m="17450">are</span> <span m="17720">very</span>
  <span m="17990">happy</span> <span m="18230">to</span> <span m="18320">have</span>
  <span m="18630">Andy</span> <span m="18860">Beck</span> <span m="19160">as</span>
  <span m="19310">our</span> <span m="19440">invited</span> <span m="19880">speaker</span>
  <span m="20240">today.</span> <span m="21510">Andy</span> <span m="22640">has</span>
  <span m="23270">a</span> <span m="23360">very</span> <span m="23720">unique</span>
  <span m="24350">background.</span> <span m="25250">He's</span> <span m="25730">trained</span>
  <span m="26480">both</span> <span m="26750">as</span> <span m="26870">a</span> <span
  m="26960">computer</span> <span m="27260">scientist</span> <span m="28220">and</span>
  <span m="28550">as</span> <span m="28700">a</span> <span m="28760">clinician.</span>
  <span m="29030">His</span> <span m="29300">specialty</span> <span m="29610">is</span>
  <span m="29920">in</span> <span m="30080">pathology.</span> <span m="31490">When</span>
  <span m="31700">he</span> <span m="31820">was</span> <span m="32180">a</span> <span
  m="32360">student</span> <span m="33140">at</span> <span m="33350">Stanford,</span>
  <span m="34860">his</span> <span m="35390">thesis</span> <span m="35990">was</span>
  <span m="36350">on</span> <span m="37040">how</span> <span m="37160">one</span>
  <span m="37310">could</span> <span m="37460">use</span> <span m="37580">machine</span>
  <span m="37850">learning</span> <span m="38150">algorithms</span> <span m="39200">to</span>
  <span m="39350">really</span> <span m="39920">understand</span> <span m="41060">a</span>
  <span m="41300">pathology</span> <span m="41920">data</span> <span m="42190">set,</span>
  <span m="42600">at</span> <span m="42750">the</span> <span m="42830">time,</span>
  <span m="43730">using</span> <span m="44330">more</span> <span m="44510">traditional</span>
  <span m="44960">regression-style</span> <span m="45710">approaches</span> <span
  m="47180">to</span> <span m="47630">understanding</span> <span m="48140">what</span>
  <span m="48480">the</span> <span m="48610">field</span> <span m="49010">is</span>
  <span m="49220">now</span> <span m="49430">called</span> <span m="49700">computational</span>
  <span m="50210">pathology.</span> <span m="51260">But</span> <span m="51410">his</span>
  <span m="51620">work</span> <span m="51800">was</span> <span m="51950">really</span>
  <span m="52310">at</span> <span m="52370">the</span> <span m="52460">forefront</span>
  <span m="52820">of</span> <span m="52880">his</span> <span m="53060">field.</span></p><p><span
  m="53780">Since</span> <span m="54140">then,</span> <span m="54370">he's</span>
  <span m="54530">come</span> <span m="54800">to</span> <span m="55220">Boston,</span>
  <span m="55940">where</span> <span m="56390">he</span> <span m="56780">was</span>
  <span m="57900">an</span> <span m="58250">attending</span> <span m="58970">and</span>
  <span m="59150">faculty</span> <span m="60110">at</span> <span m="60500">Beth</span>
  <span m="60710">Israel</span> <span m="60890">Deaconess</span> <span m="61280">Medical</span>
  <span m="61580">Center.</span> <span m="62480">In</span> <span m="62600">the</span>
  <span m="62660">recent</span> <span m="62960">couple</span> <span m="63230">of</span>
  <span m="63320">years,</span> <span m="63770">he's</span> <span m="64010">been</span>
  <span m="64160">running</span> <span m="64610">a</span> <span m="64730">company</span>
  <span m="65269">called</span> <span m="65660">PathAI,</span> <span m="67160">which</span>
  <span m="67430">is,</span> <span m="68480">in</span> <span m="68960">my</span> <span
  m="69290">opinion,</span> <span m="69960">one</span> <span m="70040">of</span> <span
  m="70100">the</span> <span m="70190">most</span> <span m="70580">exciting</span>
  <span m="71090">companies</span> <span m="71960">of</span> <span m="72140">AI</span>
  <span m="72440">in</span> <span m="72520">medicine.</span> <span m="73670">And</span>
  <span m="74260">he</span> <span m="74440">is</span> <span m="74540">my</span> <span
  m="74660">favorite</span> <span m="75020">invited</span> <span m="75380">speaker--</span></p><p><span
  m="75920">ANDY BECK:</span> <span m="75985">He</span> <span m="76050">says</span>
  <span m="76115">that</span> <span m="76180">to</span> <span m="76245">everyone.</span></p><p><span
  m="76310">PROFESSOR:</span> <span m="76430">--every</span> <span m="76550">time</span>
  <span m="76710">I</span> <span m="77160">get</span> <span m="77270">an</span> <span
  m="77410">opportunity to</span> <span m="77620">invite</span> <span m="77870">someone</span>
  <span m="78370">to</span> <span m="78870">speak.</span> <span m="79870">And</span>
  <span m="80370">I</span> <span m="80580">think</span> <span m="81340">you'll be</span>
  <span m="81440">really</span> <span m="81620">interested</span> <span m="81770">in</span>
  <span m="81870">what</span> <span m="81960">he</span> <span m="82030">has</span>
  <span m="82130">to</span> <span m="82220">say.</span></p><p><span m="82770">ANDY
  BECK:</span> <span m="82925">Great.</span> <span m="83080">Well,</span> <span m="83210">thank</span>
  <span m="83480">you</span> <span m="83540">so</span> <span m="83720">much.</span>
  <span m="84060">Thanks</span> <span m="84230">for</span> <span m="84350">having</span>
  <span m="84680">me.</span> <span m="85550">Yeah,</span> <span m="85710">I'm</span>
  <span m="85790">really</span> <span m="85940">excited</span> <span m="86390">to</span>
  <span m="86840">talk</span> <span m="87170">in</span> <span m="87290">this</span>
  <span m="87440">course.</span> <span m="88310">It</span> <span m="88430">is</span>
  <span m="88550">a</span> <span m="88610">super</span> <span m="88850">exciting</span>
  <span m="89180">time</span> <span m="90350">for</span> <span m="90710">machine</span>
  <span m="91010">learning</span> <span m="91230">in</span> <span m="91290">pathology</span>
  <span m="92585">And</span> <span m="93020">if</span> <span m="93080">you</span>
  <span m="93140">have</span> <span m="93230">any</span> <span m="93320">questions</span>
  <span m="93710">throughout,</span> <span m="94220">please</span> <span m="94550">feel</span>
  <span m="94700">free</span> <span m="94790">to</span> <span m="94880">ask.</span></p><p><span
  m="98530">And</span> <span m="99060">so</span> <span m="99300">for</span> <span
  m="99450">some</span> <span m="99600">background</span> <span m="100020">on what</span>
  <span m="100140">pathology</span> <span m="100740">is--</span> <span m="102430">it's</span>
  <span m="102820">so</span> <span m="103070">like,</span> <span m="103230">if</span>
  <span m="103320">you're</span> <span m="103410">a</span> <span m="103440">patient.</span>
  <span m="103860">You</span> <span m="103950">go</span> <span m="104040">to</span>
  <span m="104130">the</span> <span m="104250">doctor,</span> <span m="105810">and</span>
  <span m="106380">AI</span> <span m="106740">could</span> <span m="106890">apply</span>
  <span m="107850">in</span> <span m="108000">any</span> <span m="108360">aspect</span>
  <span m="108990">of</span> <span m="109140">this</span> <span m="109320">whole</span>
  <span m="109530">trajectory,</span> <span m="110430">and</span> <span m="110550">I'll</span>
  <span m="110610">kind</span> <span m="110760">of</span> <span m="110820">talk</span>
  <span m="111000">about</span> <span m="111210">specifically in</span> <span m="111600">pathology.</span></p><p><span
  m="112140">So</span> <span m="112260">you</span> <span m="112320">go</span> <span
  m="112380">to</span> <span m="112470">the</span> <span m="112530">doctor.</span>
  <span m="113130">They</span> <span m="113280">take</span> <span m="113460">a</span>
  <span m="113520">bunch</span> <span m="113670">of</span> <span m="113760">data</span>
  <span m="114000">from</span> <span m="114240">you.</span> <span m="114660">You</span>
  <span m="114750">talk</span> <span m="115020">to</span> <span m="115110">them.</span>
  <span m="115540">They</span> <span m="116040">get</span> <span m="116250">signs</span>
  <span m="116550">and</span> <span m="116640">symptoms.</span> <span m="118260">Typically,</span>
  <span m="118770">if</span> <span m="118860">they're</span> <span m="119010">at</span>
  <span m="119130">all</span> <span m="119400">concerned,</span> <span m="120590">and</span>
  <span m="120900">it</span> <span m="120960">could</span> <span m="121140">be</span>
  <span m="121230">something</span> <span m="121560">that's</span> <span m="122010">a</span>
  <span m="122070">structural</span> <span m="122790">alteration</span> <span m="123360">that's</span>
  <span m="123510">not</span> <span m="123750">accessible</span> <span m="124320">just</span>
  <span m="124530">through</span> <span m="124680">taking</span> <span m="124960">blood
  work,</span> <span m="125580">say,</span> <span m="125910">like</span> <span m="126210">a</span>
  <span m="126540">cancer,</span> <span m="127270">which</span> <span m="127320">is</span>
  <span m="127410">one</span> <span m="127530">of</span> <span m="127590">the</span>
  <span m="127650">biggest</span> <span m="127920">things,</span> <span m="128190">they'll</span>
  <span m="128310">send</span> <span m="128490">you</span> <span m="128550">to</span>
  <span m="128610">radiology</span> <span m="129270">where</span> <span m="129389">they</span>
  <span m="129509">want</span> <span m="129660">to--</span> <span m="130139">the</span>
  <span m="130310">radiology</span> <span m="130800">is</span> <span m="130889">the</span>
  <span m="130949">best</span> <span m="131220">way</span> <span m="131340">for</span>
  <span m="131430">acquiring</span> <span m="131760">data</span> <span m="132120">to</span>
  <span m="132270">look</span> <span m="132540">for</span> <span m="132780">big</span>
  <span m="133110">structural</span> <span m="133650">changes.</span></p><p><span
  m="134400">So</span> <span m="134520">you</span> <span m="134610">can't</span> <span
  m="134850">see</span> <span m="135090">single</span> <span m="135420">cells</span>
  <span m="136140">in</span> <span m="136290">radiology.</span> <span m="136830">But</span>
  <span m="136920">you</span> <span m="136980">can</span> <span m="137160">see</span>
  <span m="137930">inside</span> <span m="138690">the</span> <span m="138780">body</span>
  <span m="139200">and</span> <span m="139290">see</span> <span m="139500">some</span>
  <span m="139680">large</span> <span m="139980">things</span> <span m="140160">that</span>
  <span m="140250">are</span> <span m="140340">changing</span> <span m="140790">to</span>
  <span m="140910">make</span> <span m="141090">evaluations</span> <span m="141900">for,</span>
  <span m="142230">like,</span> <span m="142350">you</span> <span m="142440">have</span>
  <span m="142560">a</span> <span m="142590">cough,</span> <span m="143280">like</span>
  <span m="143400">are</span> <span m="143490">you</span> <span m="143610">looking</span>
  <span m="143880">at</span> <span m="144405">lung</span> <span m="144720">cancer,</span>
  <span m="145410">or</span> <span m="145440">are</span> <span m="145560">you</span>
  <span m="145650">looking</span> <span m="145890">at</span> <span m="145980">pneumonia?</span></p><p><span
  m="147200">And</span> <span m="147330">radiology</span> <span m="147900">only</span>
  <span m="148140">takes</span> <span m="148350">you</span> <span m="148440">so</span>
  <span m="148620">far.</span> <span m="149010">And</span> <span m="149130">people</span>
  <span m="149370">are</span> <span m="149430">super</span> <span m="149670">excited</span>
  <span m="150030">about</span> <span m="150210">applying</span> <span m="151290">AI</span>
  <span m="151950">to</span> <span m="152100">radiology,</span> <span m="153030">but</span>
  <span m="153150">I</span> <span m="153210">think</span> <span m="153420">one</span>
  <span m="153660">thing</span> <span m="153810">they</span> <span m="153930">often</span>
  <span m="154260">forget</span> <span m="155100">is</span> <span m="155310">these</span>
  <span m="155460">images</span> <span m="156240">are</span> <span m="156690">not</span>
  <span m="156930">very</span> <span m="157170">data-rich</span> <span m="157800">compared</span>
  <span m="158280">to</span> <span m="159540">the</span> <span m="160080">core</span>
  <span m="160590">data</span> <span m="160920">types.</span> <span m="161460">I</span>
  <span m="161490">mean,</span> <span m="161610">this</span> <span m="161730">is</span>
  <span m="161850">my</span> <span m="162000">bias</span> <span m="162360">from</span>
  <span m="162510">pathology,</span> <span m="163340">but</span> <span m="163470">radiology</span>
  <span m="163980">gets</span> <span m="164190">you</span> <span m="164250">some</span>
  <span m="164520">part</span> <span m="164730">of</span> <span m="164790">the</span>
  <span m="164880">way,</span> <span m="165090">where</span> <span m="165210">you</span>
  <span m="165300">can</span> <span m="165420">sort</span> <span m="165600">of</span>
  <span m="165690">triage</span> <span m="166140">normal</span> <span m="166440">stuff.</span></p><p><span
  m="166890">And</span> <span m="167010">the</span> <span m="167070">radiologist</span>
  <span m="167580">will</span> <span m="167770">have</span> <span m="167970">some</span>
  <span m="168150">impression</span> <span m="168630">of</span> <span m="168720">what</span>
  <span m="168870">they're</span> <span m="168960">looking</span> <span m="169260">at.</span>
  <span m="169410">And</span> <span m="169500">often,</span> <span m="169710">that's</span>
  <span m="169860">the</span> <span m="169950">bottom</span> <span m="170250">line</span>
  <span m="170370">in</span> <span m="170460">the</span> <span m="170520">radiology</span>
  <span m="170940">report</span> <span m="171210">is</span> <span m="171530">impression--</span>
  <span m="172350">concerning</span> <span m="172890">for</span> <span m="173040">cancer,</span>
  <span m="173430">or</span> <span m="173550">impression--</span> <span m="174030">likely</span>
  <span m="174330">benign</span> <span m="174720">but</span> <span m="175200">not</span>
  <span m="175410">sure,</span> <span m="175770">or</span> <span m="176010">impression--</span>
  <span m="176820">totally</span> <span m="177180">benign.</span> <span m="178020">And</span>
  <span m="178140">that</span> <span m="178270">will</span> <span m="178340">also</span>
  <span m="178650">guide</span> <span m="178890">subsequent</span> <span m="179280">decisions.</span>
  <span m="179740">But</span> <span m="179840">if</span> <span m="179940">there's
  some</span> <span m="180060">concern</span> <span m="180450">that</span> <span m="180540">something</span>
  <span m="180720">serious</span> <span m="180990">is</span> <span m="181080">going</span>
  <span m="181290">on,</span> <span m="181410">the</span> <span m="181470">patient</span>
  <span m="181770">undergoes</span> <span m="182040">a</span> <span m="182070">pretty</span>
  <span m="182250">serious</span> <span m="183240">procedure,</span> <span m="183750">which</span>
  <span m="183900">is</span> <span m="184010">a</span> <span m="184050">tissue</span>
  <span m="184350">biopsy.</span></p><p><span m="185130">So</span> <span m="185280">pathology</span>
  <span m="186900">requires</span> <span m="187540">tissue</span> <span m="188010">to</span>
  <span m="188220">do</span> <span m="188940">what</span> <span m="189090">I'm</span>
  <span m="189150">going</span> <span m="189270">to</span> <span m="189330">talk</span>
  <span m="189510">about,</span> <span m="189730">which</span> <span m="189750">is</span>
  <span m="189810">surgical</span> <span m="190290">pathology</span> <span m="190920">that</span>
  <span m="191040">requires</span> <span m="191500">tissue</span> <span m="191640">specimen.</span>
  <span m="192010">There's</span> <span m="192150">also</span> <span m="192360">blood-based</span>
  <span m="192780">things.</span> <span m="193290">But</span> <span m="193470">then</span>
  <span m="193650">this</span> <span m="193890">is</span> <span m="194010">the</span>
  <span m="194100">diagnosis</span> <span m="194730">where</span> <span m="195860">you're</span>
  <span m="195960">trying</span> <span m="196290">to</span> <span m="196380">say</span>
  <span m="196560">is</span> <span m="196650">this</span> <span m="196770">cancer?</span>
  <span m="197100">Is</span> <span m="197220">this</span> <span m="197340">not</span>
  <span m="197490">cancer?</span> <span m="198300">And</span> <span m="198390">that</span>
  <span m="198600">report</span> <span m="198960">by</span> <span m="199140">itself</span>
  <span m="199620">can</span> <span m="199830">really</span> <span m="200070">guide</span>
  <span m="200580">subsequent</span> <span m="201150">decisions,</span> <span m="201660">which</span>
  <span m="201780">could</span> <span m="201900">be</span> <span m="201990">no</span>
  <span m="202200">further</span> <span m="202470">treatment</span> <span m="202860">or</span>
  <span m="203040">a</span> <span m="203700">big</span> <span m="203970">surgery</span>
  <span m="204450">or</span> <span m="204520">a</span> <span m="204540">big</span>
  <span m="205140">decision</span> <span m="205500">about</span> <span m="205650">chemotherapy</span>
  <span m="206400">and</span> <span m="206520">radiotherapy.</span></p><p><span m="207360">So</span>
  <span m="207480">this</span> <span m="207630">is</span> <span m="207750">one</span>
  <span m="207990">area</span> <span m="208350">where</span> <span m="208500">you</span>
  <span m="208620">really</span> <span m="208830">want to</span> <span m="208950">incorporate</span>
  <span m="209400">data</span> <span m="209760">in</span> <span m="209850">the</span>
  <span m="209910">most</span> <span m="210090">effective</span> <span m="210480">way</span>
  <span m="211260">to</span> <span m="211410">reduce</span> <span m="211740">errors,</span>
  <span m="212160">to</span> <span m="212220">increase</span> <span m="212430">standardization,</span>
  <span m="213330">and</span> <span m="213420">to</span> <span m="213510">really</span>
  <span m="213720">inform</span> <span m="214410">the</span> <span m="214530">best</span>
  <span m="214830">treatment</span> <span m="215130">decision</span> <span m="215490">for</span>
  <span m="215580">each</span> <span m="215760">patient</span> <span m="216180">based</span>
  <span m="216510">on</span> <span m="216600">the</span> <span m="216660">characteristics</span>
  <span m="217830">of</span> <span m="217980">their</span> <span m="218130">disease.</span></p><p><span
  m="219480">And</span> <span m="219600">the</span> <span m="219690">one</span> <span
  m="219870">thing</span> <span m="220020">about</span> <span m="220200">pathology</span>
  <span m="220680">that's</span> <span m="220890">pretty</span> <span m="221280">interesting</span>
  <span m="221880">is</span> <span m="222060">it's</span> <span m="222210">super</span>
  <span m="222690">visual.</span> <span m="223470">And</span> <span m="224460">this</span>
  <span m="224640">is</span> <span m="224760">just</span> <span m="225180">a</span>
  <span m="225240">kind</span> <span m="225450">of</span> <span m="225540">random</span>
  <span m="225930">sampling</span> <span m="226380">of</span> <span m="226500">some</span>
  <span m="226680">of</span> <span m="226770">the</span> <span m="226860">types</span>
  <span m="227340">of</span> <span m="227730">different</span> <span m="228150">imagery</span>
  <span m="228630">that</span> <span m="228750">pathologists</span> <span m="229230">are</span>
  <span m="229320">looking</span> <span m="229530">at</span> <span m="229590">every</span>
  <span m="229760">day.</span> <span m="229930">I think</span> <span m="230040">this
  is</span> <span m="230400">one</span> <span m="230640">thing</span> <span m="230760">that</span>
  <span m="230910">draws</span> <span m="231300">people</span> <span m="231900">to</span>
  <span m="232050">this</span> <span m="232170">specialty</span> <span m="232770">is</span>
  <span m="233675">a saying</span> <span m="234090">in</span> <span m="234180">radiology,</span>
  <span m="234730">you're</span> <span m="234810">sort</span> <span m="234960">of</span>
  <span m="235050">looking</span> <span m="235380">at</span> <span m="235500">an</span>
  <span m="235590">impression</span> <span m="236100">of</span> <span m="236220">what</span>
  <span m="236400">might</span> <span m="236730">be</span> <span m="236880">happening</span>
  <span m="237330">based</span> <span m="237690">on</span> <span m="237960">sending</span>
  <span m="240270">different</span> <span m="240630">types</span> <span m="241200">of</span>
  <span m="241500">images</span> <span m="242010">and</span> <span m="242100">acquiring</span>
  <span m="242490">the</span> <span m="242580">data</span> <span m="243000">and</span>
  <span m="243120">sort</span> <span m="243300">of</span> <span m="243360">trying</span>
  <span m="243570">to</span> <span m="243690">estimate</span> <span m="244050">what's</span>
  <span m="244200">going</span> <span m="244410">on.</span></p><p><span m="244730">Whereas
  here,</span> <span m="244890">you're</span> <span m="245010">actually</span> <span
  m="245490">staining</span> <span m="246420">pieces</span> <span m="246750">of</span>
  <span m="246810">tissue</span> <span m="247380">and</span> <span m="247500">looking</span>
  <span m="247740">by</span> <span m="248090">eye</span> <span m="248560">at</span>
  <span m="248820">actual</span> <span m="249720">individual</span> <span m="250200">cells.</span>
  <span m="250720">You</span> <span m="250780">can</span> <span m="250860">look</span>
  <span m="250980">within</span> <span m="251250">cells.</span> <span m="251700">You</span>
  <span m="251790">can</span> <span m="251910">look</span> <span m="252030">at</span>
  <span m="252120">how</span> <span m="252270">populations</span> <span m="252840">of</span>
  <span m="252900">cells</span> <span m="253170">are</span> <span m="253230">being</span>
  <span m="253350">organized.</span> <span m="254170">And</span> <span m="254280">for</span>
  <span m="254400">many</span> <span m="254640">diseases,</span> <span m="255090">this</span>
  <span m="255180">still</span> <span m="255360">represents</span> <span m="255840">sort</span>
  <span m="255960">of</span> <span m="256050">the</span> <span m="256110">core</span>
  <span m="256380">data</span> <span m="256680">type</span> <span m="256950">that</span>
  <span m="257100">defines</span> <span m="258120">what's</span> <span m="258420">going</span>
  <span m="258750">on,</span> <span m="259800">and</span> <span m="259920">is</span>
  <span m="260040">this</span> <span m="260490">something</span> <span m="260730">with</span>
  <span m="260820">a</span> <span m="260880">serious</span> <span m="261240">prognosis</span>
  <span m="261750">that</span> <span m="261839">requires,</span> <span m="262410">say,</span>
  <span m="262590">surgery?</span> <span m="263040">Or</span> <span m="263130">is</span>
  <span m="263220">this</span> <span m="263280">something</span> <span m="263620">that's
  totally</span> <span m="263790">benign?</span> <span m="264520">All</span> <span
  m="264570">of</span> <span m="264660">these</span> <span m="264840">are</span> <span
  m="264930">different</span> <span m="265140">aspects</span> <span m="265560">of</span>
  <span m="265650">benign</span> <span m="266160">processes.</span></p><p><span m="266980">And</span>
  <span m="267840">so</span> <span m="268170">just</span> <span m="268380">the</span>
  <span m="268500">normal</span> <span m="268920">human</span> <span m="269160">body</span>
  <span m="269460">creates</span> <span m="269760">all</span> <span m="269880">these</span>
  <span m="270030">different</span> <span m="270240">patterns.</span> <span m="270690">And
  then</span> <span m="270810">there's</span> <span m="270960">a</span> <span m="271020">lot</span>
  <span m="271200">of</span> <span m="271290">patterns</span> <span m="271740">of</span>
  <span m="271980">disease.</span> <span m="272620">And</span> <span m="272720">these</span>
  <span m="272790">are</span> <span m="272850">all</span> <span m="272970">different</span>
  <span m="273540">subtypes</span> <span m="274140">of</span> <span m="274230">disease</span>
  <span m="275420">that</span> <span m="275730">are</span> <span m="275790">all</span>
  <span m="275970">different</span> <span m="276210">morphologies.</span> <span m="277360">So</span>
  <span m="277380">there's</span> <span m="277510">sort</span> <span m="277680">of</span>
  <span m="277740">an</span> <span m="277800">incredible</span> <span m="278490">wealth</span>
  <span m="278970">of</span> <span m="279090">different</span> <span m="279660">visual</span>
  <span m="280140">imagery</span> <span m="280530">that</span> <span m="280680">the</span>
  <span m="280770">pathologist</span> <span m="281220">has</span> <span m="281370">to</span>
  <span m="281430">incorporate</span> <span m="281880">into</span> <span m="282000">their</span>
  <span m="282120">diagnosis.</span></p><p><span m="282670">And</span> <span m="282750">then</span>
  <span m="282840">there's,</span> <span m="283110">on</span> <span m="283230">top</span>
  <span m="283500">of</span> <span m="283620">that,</span> <span m="283800">things</span>
  <span m="283980">like</span> <span m="284100">special</span> <span m="284460">stains</span>
  <span m="284940">that</span> <span m="285030">can</span> <span m="285150">stain</span>
  <span m="285420">for</span> <span m="285540">specific</span> <span m="286620">organisms,</span>
  <span m="287610">for</span> <span m="287910">infectious</span> <span m="288360">disease,</span>
  <span m="288840">or</span> <span m="288960">specific</span> <span m="289410">patterns</span>
  <span m="289740">of</span> <span m="289800">protein</span> <span m="290190">expression,</span>
  <span m="290730">for</span> <span m="290980">subtyping</span> <span m="291810">disease</span>
  <span m="292260">based</span> <span m="292530">on</span> <span m="292590">expression</span>
  <span m="292980">of</span> <span m="293040">drug</span> <span m="293280">targets.</span>
  <span m="294180">And</span> <span m="294300">this</span> <span m="294540">even</span>
  <span m="294750">more</span> <span m="294930">sort of</span> <span m="295260">increases</span>
  <span m="295680">the</span> <span m="295740">complexity</span> <span m="297390">of</span>
  <span m="297540">the</span> <span m="297690">work.</span></p><p><span m="298900">So</span>
  <span m="299070">for</span> <span m="299460">many</span> <span m="299790">years,</span>
  <span m="300300">there's</span> <span m="300480">really</span> <span m="300660">nothing</span>
  <span m="301050">new</span> <span m="301290">about</span> <span m="301500">trying</span>
  <span m="301710">to</span> <span m="301800">apply</span> <span m="302280">AI</span>
  <span m="302880">or</span> <span m="303000">machine</span> <span m="303360">learning</span>
  <span m="303870">or</span> <span m="303960">computation</span> <span m="304620">to</span>
  <span m="304740">this</span> <span m="304950">field.</span> <span m="305230">It's</span>
  <span m="305370">actually</span> <span m="305580">a</span> <span m="305640">very</span>
  <span m="305910">natural</span> <span m="306540">field,</span> <span m="306930">because</span>
  <span m="307410">it's</span> <span m="307560">sort</span> <span m="307770">of</span>
  <span m="307860">laboratory-based.</span> <span m="309090">It's</span> <span m="309240">all</span>
  <span m="309360">about</span> <span m="309540">data</span> <span m="309780">processing.</span>
  <span m="310350">You</span> <span m="310410">take</span> <span m="310600">this</span>
  <span m="310740">input,</span> <span m="311100">things</span> <span m="311340">like</span>
  <span m="311460">images,</span> <span m="311850">and</span> <span m="311940">produces</span>
  <span m="312300">output,</span> <span m="312880">what</span> <span m="313050">a</span>
  <span m="313110">diagnosis</span> <span m="313680">is.</span></p><p><span m="314340">So</span>
  <span m="314520">people</span> <span m="314700">have</span> <span m="314790">really</span>
  <span m="314940">been</span> <span m="315060">trying</span> <span m="315390">this</span>
  <span m="315600">for</span> <span m="316530">40</span> <span m="316830">years</span>
  <span m="317040">or</span> <span m="317100">so</span> <span m="317280">now.</span>
  <span m="317520">This</span> <span m="317640">is</span> <span m="317730">one</span>
  <span m="317910">of</span> <span m="317970">the</span> <span m="318060">very</span>
  <span m="318360">first</span> <span m="318600">studies</span> <span m="319140">that</span>
  <span m="319440">sort</span> <span m="319680">of</span> <span m="319770">just</span>
  <span m="319950">tried</span> <span m="320220">to</span> <span m="320310">see,</span>
  <span m="320680">could</span> <span m="320760">we</span> <span m="321210">train</span>
  <span m="321510">a</span> <span m="321570">computer</span> <span m="322230">to</span>
  <span m="322650">identify</span> <span m="323460">the</span> <span m="323610">size</span>
  <span m="324150">of</span> <span m="324240">cancer</span> <span m="324630">cells</span>
  <span m="325350">through</span> <span m="325590">a</span> <span m="325650">process</span>
  <span m="326040">they</span> <span m="326130">called</span> <span m="326340">morphometry,</span>
  <span m="327000">here</span> <span m="327120">on</span> <span m="327180">the</span>
  <span m="327270">bottom?</span> <span m="327990">And</span> <span m="328080">then</span>
  <span m="328260">could</span> <span m="328410">we</span> <span m="329130">just</span>
  <span m="329400">use</span> <span m="329670">sort</span> <span m="329910">of</span>
  <span m="330840">measurements</span> <span m="331350">about</span> <span m="331500">the</span>
  <span m="331590">size</span> <span m="331890">of</span> <span m="331980">cancer</span>
  <span m="332340">cells</span> <span m="332760">in</span> <span m="332880">a</span>
  <span m="332970">very</span> <span m="333360">simple</span> <span m="333690">model</span>
  <span m="335220">to</span> <span m="335550">predict</span> <span m="336030">outcome?</span></p><p><span
  m="336580">And</span> <span m="336680">in</span> <span m="336780">this</span> <span
  m="336880">study,</span> <span m="337140">they</span> <span m="337320">have</span>
  <span m="337470">a</span> <span m="337530">learning</span> <span m="337920">set</span>
  <span m="338220">that</span> <span m="338340">they're</span> <span m="338460">learning</span>
  <span m="338820">from</span> <span m="339510">and</span> <span m="339630">then</span>
  <span m="339780">a</span> <span m="339840">test</span> <span m="340080">set.</span>
  <span m="340410">And</span> <span m="340500">they</span> <span m="340650">show</span>
  <span m="341210">that</span> <span m="341400">their</span> <span m="341550">system,</span>
  <span m="341940">as</span> <span m="342090">every</span> <span m="342360">paper</span>
  <span m="342630">that</span> <span m="342750">ever</span> <span m="342900">gets</span>
  <span m="343050">published</span> <span m="343350">shows,</span> <span m="344610">does</span>
  <span m="344880">better</span> <span m="345120">than</span> <span m="345320">the
  two</span> <span m="345510">competing</span> <span m="345840">approaches.</span>
  <span m="346450">Although</span> <span m="347190">even</span> <span m="347490">in</span>
  <span m="347580">this</span> <span m="347730">best</span> <span m="347940">case</span>
  <span m="348120">scenario,</span> <span m="348550">there's</span> <span m="348600">significant</span>
  <span m="349200">degradation</span> <span m="350220">from</span> <span m="350430">learning</span>
  <span m="350730">to</span> <span m="350790">test.</span></p><p><span m="351150">So</span>
  <span m="351630">one,</span> <span m="351930">it's</span> <span m="352040">super</span>
  <span m="352320">simple.</span> <span m="352820">It's</span> <span m="352870">using</span>
  <span m="353100">very</span> <span m="353250">simple</span> <span m="353460">methods,</span>
  <span m="353820">and</span> <span m="353910">the</span> <span m="354000">data</span>
  <span m="354220">sets</span> <span m="354480">are</span> <span m="354540">tiny,</span>
  <span m="355670">38</span> <span m="356160">learning</span> <span m="356490">cases,</span>
  <span m="356940">40</span> <span m="357240">test</span> <span m="357510">cases.</span>
  <span m="358190">And</span> <span m="358290">this</span> <span m="358410">is</span>
  <span m="358530">published</span> <span m="358890">in</span> <span m="359160"><i>The</i></span>
  <span m="359250"><i>Lancet,</i></span> <span m="359700">which</span> <span m="359880">is</span>
  <span m="360540">the</span> <span m="360660">leading</span> <span m="361020">biomedical</span>
  <span m="361560">journal</span> <span m="362440">even</span> <span m="362550">today.</span></p><p><span
  m="364230">And</span> <span m="364320">then</span> <span m="364440">people</span>
  <span m="364650">got</span> <span m="364770">excited</span> <span m="365160">about</span>
  <span m="365610">AI</span> <span m="366480">sort</span> <span m="366690">of</span>
  <span m="366750">building</span> <span m="367170">off</span> <span m="367430">of</span>
  <span m="367500">simple</span> <span m="367860">approaches.</span> <span m="368890">And</span>
  <span m="369000">back</span> <span m="369240">in</span> <span m="369330">1990,</span>
  <span m="370650">it</span> <span m="370740">was</span> <span m="370890">thought</span>
  <span m="371190">artificial</span> <span m="371580">neural</span> <span m="371850">nets</span>
  <span m="372090">would</span> <span m="372180">be</span> <span m="372270">super</span>
  <span m="372540">useful</span> <span m="372810">for</span> <span m="372960">quantitative</span>
  <span m="373440">pathology</span> <span m="373920">for</span> <span m="374040">sort</span>
  <span m="374190">of</span> <span m="374280">obvious</span> <span m="374640">reasons.</span>
  <span m="376080">But</span> <span m="376620">at</span> <span m="376740">that</span>
  <span m="376950">time,</span> <span m="377190">there was</span> <span m="377370">really</span>
  <span m="377520">no</span> <span m="377700">way</span> <span m="377820">of</span>
  <span m="377910">digitizing</span> <span m="378540">stuff</span> <span m="378750">at</span>
  <span m="378840">any</span> <span m="378990">sort</span> <span m="379170">of</span>
  <span m="379230">scale,</span> <span m="380150">and</span> <span m="380300">that</span>
  <span m="380420">problem's</span> <span m="380820">only</span> <span m="381060">recently</span>
  <span m="381420">been</span> <span m="381540">solved.</span></p><p><span m="381920">But</span>
  <span m="382050">sort</span> <span m="382200">of</span> <span m="382270">in</span>
  <span m="382370">2000,</span> <span m="382920">people</span> <span m="383160">were</span>
  <span m="383250">first</span> <span m="383520">thinking</span> <span m="383820">about</span>
  <span m="384180">once</span> <span m="384690">the</span> <span m="384780">slides</span>
  <span m="385140">are</span> <span m="385200">digital,</span> <span m="385680">then</span>
  <span m="385830">you</span> <span m="385890">could</span> <span m="386160">apply</span>
  <span m="386430">computational</span> <span m="387030">methods</span> <span m="388050">effectively.</span>
  <span m="389580">But</span> <span m="389760">kind</span> <span m="389930">of</span>
  <span m="390000">nothing</span> <span m="390300">really</span> <span m="390480">changed,</span>
  <span m="391710">and</span> <span m="391830">still,</span> <span m="392130">to</span>
  <span m="392280">a</span> <span m="392340">large</span> <span m="392610">degree,</span>
  <span m="392850">hasn't</span> <span m="393090">changed</span> <span m="393390">for</span>
  <span m="393510">the</span> <span m="393600">predominance</span> <span m="394080">of</span>
  <span m="394140">pathology,</span> <span m="394690">which</span> <span m="394740">I'll</span>
  <span m="394830">talk</span> <span m="395100">about.</span></p><p><span m="397710">But</span>
  <span m="398070">as</span> <span m="398250">was</span> <span m="398400">mentioned</span>
  <span m="398730">earlier,</span> <span m="399220">I</span> <span m="399480">was</span>
  <span m="399660">part</span> <span m="399990">of</span> <span m="400410">one</span>
  <span m="400590">of</span> <span m="400650">the</span> <span m="400710">first</span>
  <span m="400950">studies</span> <span m="401250">to</span> <span m="401340">really</span>
  <span m="401490">take</span> <span m="401670">a</span> <span m="401850">more</span>
  <span m="402030">machine</span> <span m="402390">learning</span> <span m="402630">approach</span>
  <span m="403320">to</span> <span m="403470">this.</span> <span m="403770">And</span>
  <span m="403860">what</span> <span m="403980">we</span> <span m="404070">mean</span>
  <span m="404280">by</span> <span m="404400">machine</span> <span m="404760">learning</span>
  <span m="405060">versus</span> <span m="405390">prior</span> <span m="405630">approaches</span>
  <span m="406470">is</span> <span m="406590">the</span> <span m="406680">idea</span>
  <span m="406860">of</span> <span m="406920">using</span> <span m="407160">data-driven</span>
  <span m="408060">analysis</span> <span m="408930">to</span> <span m="409050">figure</span>
  <span m="409470">out</span> <span m="409680">the</span> <span m="409800">best</span>
  <span m="410070">features.</span></p><p><span m="411030">And</span> <span m="411150">now</span>
  <span m="411330">you</span> <span m="411450">can</span> <span m="411570">do</span>
  <span m="411660">that</span> <span m="411810">in</span> <span m="411930">an even</span>
  <span m="412170">more</span> <span m="412350">explicit</span> <span m="412890">way</span>
  <span m="413280">with</span> <span m="413550">machine</span> <span m="413850">learning,</span>
  <span m="414550">but</span> <span m="414600">there's</span> <span m="414750">sort</span>
  <span m="414870">of</span> <span m="414930">a</span> <span m="414990">progression</span>
  <span m="415500">from</span> <span m="415650">measuring</span> <span m="416070">one</span>
  <span m="416250">or</span> <span m="416340">two</span> <span m="416550">things</span>
  <span m="416910">in</span> <span m="417000">a</span> <span m="417060">very</span>
  <span m="417300">tedious</span> <span m="417750">way</span> <span m="417960">on</span>
  <span m="418080">very</span> <span m="418260">small</span> <span m="418440">data</span>
  <span m="418660">sets</span> <span m="418940">to,</span> <span m="419060">I'd</span>
  <span m="419160">say,</span> <span m="419310">this</span> <span m="419550">way,</span>
  <span m="419730">where we're</span> <span m="419880">using</span> <span m="420210">some</span>
  <span m="420750">traditional</span> <span m="421350">regression-based</span> <span
  m="422190">machine</span> <span m="422520">learning</span> <span m="422850">to</span>
  <span m="423090">measure</span> <span m="423990">larger</span> <span m="424500">numbers</span>
  <span m="424860">of</span> <span m="424920">features.</span> <span m="425370">And</span>
  <span m="425460">then</span> <span m="425550">using</span> <span m="425820">things</span>
  <span m="426030">like</span> <span m="426180">those</span> <span m="426420">associations,</span>
  <span m="427170">those</span> <span m="427410">features</span> <span m="427760">with</span>
  <span m="427800">patient</span> <span m="428100">outcome</span> <span m="428940">to</span>
  <span m="429090">focus</span> <span m="429600">your</span> <span m="429720">analyses</span>
  <span m="430200">on</span> <span m="430290">the</span> <span m="430350">most</span>
  <span m="430530">important</span> <span m="430920">ones.</span></p><p><span m="431700">And</span>
  <span m="432120">the</span> <span m="432450">challenging</span> <span m="432960">machine</span>
  <span m="433290">learning</span> <span m="433560">task</span> <span m="433920">here</span>
  <span m="434370">and</span> <span m="434550">really</span> <span m="434790">one</span>
  <span m="434910">of</span> <span m="434970">the</span> <span m="435030">core</span>
  <span m="435240">tasks</span> <span m="435660">in</span> <span m="435840">pathology</span>
  <span m="436410">is</span> <span m="436620">image</span> <span m="436860">processing.</span>
  <span m="437860">So</span> <span m="437970">how</span> <span m="438090">do</span>
  <span m="438180">we</span> <span m="438300">train</span> <span m="438720">computers</span>
  <span m="439440">to</span> <span m="439530">sort</span> <span m="439680">of</span>
  <span m="439770">have</span> <span m="439980">the</span> <span m="440070">knowledge</span>
  <span m="440850">of</span> <span m="441030">what</span> <span m="441240">is</span>
  <span m="441390">being</span> <span m="441570">looked</span> <span m="441840">at</span>
  <span m="442050">that</span> <span m="442230">any</span> <span m="442440">pathologist</span>
  <span m="442980">would</span> <span m="443070">want</span> <span m="443220">to</span>
  <span m="443280">have?</span> <span m="444000">And</span> <span m="444090">there's</span>
  <span m="444240">a</span> <span m="444300">few</span> <span m="444420">basic</span>
  <span m="444840">things</span> <span m="445110">you'd</span> <span m="445200">want</span>
  <span m="445350">to</span> <span m="445410">train</span> <span m="445620">the</span>
  <span m="445710">computer</span> <span m="446040">to</span> <span m="446160">do,</span>
  <span m="446790">which</span> <span m="446970">is,</span> <span m="447160">for</span>
  <span m="447260">example,</span> <span m="447580">identify</span> <span m="447930">where's</span>
  <span m="448230">the</span> <span m="448290">cancer?</span> <span m="449070">Where's</span>
  <span m="449430">the</span> <span m="449530">stroma?</span> <span m="450150">Where</span>
  <span m="450330">are the</span> <span m="450420">cancer</span> <span m="450720">cells?</span>
  <span m="451260">Where</span> <span m="451530">are</span> <span m="451850">the</span>
  <span m="452170">fibroblasts,</span> <span m="452820">et</span> <span m="453060">cetera?</span></p><p><span
  m="453690">And</span> <span m="453810">then</span> <span m="453930">once</span>
  <span m="454200">you</span> <span m="454290">train</span> <span m="454890">a</span>
  <span m="454950">machine</span> <span m="455280">learning</span> <span m="455520">based</span>
  <span m="455700">system</span> <span m="456420">to</span> <span m="456540">identify</span>
  <span m="456990">those</span> <span m="457230">things,</span> <span m="457620">you</span>
  <span m="457710">can</span> <span m="457830">then</span> <span m="457950">extract</span>
  <span m="458490">lots</span> <span m="458850">of</span> <span m="458940">quantitative</span>
  <span m="459450">phenotypes</span> <span m="460290">out</span> <span m="460410">of</span>
  <span m="460500">the</span> <span m="460590">images.</span> <span m="460980">And</span>
  <span m="461070">this</span> <span m="461220">is</span> <span m="461310">all</span>
  <span m="461430">using</span> <span m="461640">human-engineered</span> <span m="462330">features</span>
  <span m="463110">to</span> <span m="463230">measure</span> <span m="463650">all</span>
  <span m="464010">the</span> <span m="464130">different</span> <span m="464370">characteristics</span>
  <span m="465060">of</span> <span m="465150">what's</span> <span m="465330">going</span>
  <span m="465540">on</span> <span m="465660">in an</span> <span m="465780">image.</span>
  <span m="466540">And</span> <span m="466650">machine</span> <span m="466950">learning</span>
  <span m="467250">is</span> <span m="467340">being</span> <span m="467700">used</span>
  <span m="468000">here</span> <span m="468390">to</span> <span m="468540">create</span>
  <span m="468960">those</span> <span m="469200">features.</span> <span m="469960">And</span>
  <span m="469980">then</span> <span m="470100">we</span> <span m="470190">use</span>
  <span m="470760">other</span> <span m="471000">regression-based</span> <span m="471750">methods</span>
  <span m="472110">to</span> <span m="472230">associate</span> <span m="472740">these</span>
  <span m="472890">features</span> <span m="473310">with</span> <span m="473400">things</span>
  <span m="473550">like</span> <span m="473640">clinical</span> <span m="473940">outcome.</span></p><p><span
  m="474750">And</span> <span m="474960">in</span> <span m="475050">this</span> <span
  m="475230">work,</span> <span m="475440">we</span> <span m="475560">show</span>
  <span m="475810">that</span> <span m="475920">by</span> <span m="476040">taking</span>
  <span m="476310">a</span> <span m="476370">data-driven</span> <span m="476880">approach,</span>
  <span m="477370">sort</span> <span m="477570">of,</span> <span m="477810">you</span>
  <span m="478125">begin</span> <span m="478440">to</span> <span m="478530">focus</span>
  <span m="479010">on</span> <span m="479190">things</span> <span m="479460">like</span>
  <span m="479610">what's</span> <span m="479790">happening</span> <span m="480210">in</span>
  <span m="480330">the</span> <span m="480420">tumor</span> <span m="480660">microenvironment,</span>
  <span m="481770">not</span> <span m="481980">just</span> <span m="482160">in</span>
  <span m="482250">the</span> <span m="482310">tumor</span> <span m="482580">itself?</span>
  <span m="483350">And</span> <span m="483480">it sort</span> <span m="483630">of</span>
  <span m="483720">turned</span> <span m="484050">out,</span> <span m="484890">over</span>
  <span m="485130">the</span> <span m="485190">past</span> <span m="485460">decade,</span>
  <span m="485910">that</span> <span m="486090">understanding</span> <span m="486660">the</span>
  <span m="486750">way</span> <span m="486870">the</span> <span m="486960">tumor</span>
  <span m="487260">interacts</span> <span m="487590">with</span> <span m="487680">the</span>
  <span m="487740">tumor</span> <span m="487890">microenvironment</span> <span m="488580">is</span>
  <span m="488640">sort</span> <span m="488820">of</span> <span m="489000">one</span>
  <span m="489210">of</span> <span m="489270">the</span> <span m="489360">most</span>
  <span m="489660">important</span> <span m="490020">things</span> <span m="490230">to</span>
  <span m="490290">do</span> <span m="490380">in</span> <span m="490470">cancer</span>
  <span m="490950">with</span> <span m="491070">things</span> <span m="491280">like</span>
  <span m="491940">fields</span> <span m="492200">like</span> <span m="492300">immunooncology</span>
  <span m="493260">being</span> <span m="493920">one</span> <span m="494100">of</span>
  <span m="494160">the</span> <span m="494220">biggest</span> <span m="494520">advances</span>
  <span m="494890">in</span> <span m="494940">the</span> <span m="495030">therapy</span>
  <span m="495390">of</span> <span m="495480">cancer,</span> <span m="495840">where
  you're</span> <span m="495960">essentially</span> <span m="496290">just</span> <span
  m="496500">regulating</span> <span m="497010">how</span> <span m="497250">tumor</span>
  <span m="497520">cells</span> <span m="499110">interact</span> <span m="499680">with</span>
  <span m="499800">the</span> <span m="499890">cells</span> <span m="500190">around</span>
  <span m="500520">them.</span></p><p><span m="501120">And</span> <span m="501240">that</span>
  <span m="501480">sort</span> <span m="501690">of</span> <span m="501780">data</span>
  <span m="502140">is</span> <span m="502290">entirely</span> <span m="503010">inaccessible</span>
  <span m="503820">using</span> <span m="504060">traditional</span> <span m="504540">pathology</span>
  <span m="504960">approaches</span> <span m="505380">and</span> <span m="505470">really</span>
  <span m="505650">required</span> <span m="506100">a</span> <span m="506130">machine</span>
  <span m="506430">learning</span> <span m="506700">approach</span> <span m="507450">to</span>
  <span m="508320">extract</span> <span m="508770">a</span> <span m="508800">bunch</span>
  <span m="509010">of</span> <span m="509070">features</span> <span m="509610">and</span>
  <span m="509730">sort</span> <span m="509880">of</span> <span m="509940">let</span>
  <span m="510090">the</span> <span m="510180">data</span> <span m="510480">speak</span>
  <span m="510720">for</span> <span m="510810">itself</span> <span m="511560">in</span>
  <span m="511650">terms</span> <span m="511860">of</span> <span m="511920">which</span>
  <span m="512070">of</span> <span m="512130">those</span> <span m="512309">features</span>
  <span m="512640">is</span> <span m="512760">most</span> <span m="513000">important</span>
  <span m="513929">for</span> <span m="514230">survival.</span></p><p><span m="515679">And</span>
  <span m="515850">in</span> <span m="515909">this</span> <span m="516059">study,</span>
  <span m="516360">we</span> <span m="516480">showed</span> <span m="516809">that</span>
  <span m="517200">these</span> <span m="517440">things</span> <span m="517820">are</span>
  <span m="517919">associated</span> <span m="518309">with</span> <span m="518400">survival.</span>
  <span m="518970">I</span> <span m="519030">don't</span> <span m="519150">know</span>
  <span m="519210">if</span> <span m="519299">you</span> <span m="519360">guys</span>
  <span m="519570">do</span> <span m="519690">a</span> <span m="519750">lot</span>
  <span m="519870">of</span> <span m="519960">Kaplan-Meier</span> <span m="520590">plots</span>
  <span m="521250">in</span> <span m="521429">here.</span></p><p><span m="521880">PROFESSOR:</span>
  <span m="521950">They</span> <span m="522020">saw</span> <span m="522090">it</span>
  <span m="522210">once,</span> <span m="522669">but</span> <span m="522990">taking</span>
  <span m="523289">us</span> <span m="523409">through it</span> <span m="523570">slowly</span>
  <span m="523919">is</span> <span m="524070">never</span> <span m="524320">a</span>
  <span m="524390">bad</span> <span m="524570">idea.</span></p><p><span m="524890">ANDY
  BECK:</span> <span m="525050">Yeah,</span> <span m="525210">so</span> <span m="525390">these</span>
  <span m="525690">are--</span> <span m="525810">I</span> <span m="525900">feel</span>
  <span m="526080">there's</span> <span m="526350">one</span> <span m="526620">type</span>
  <span m="526860">of</span> <span m="526950">plot</span> <span m="527370">to</span>
  <span m="527520">know</span> <span m="528280">for</span> <span m="528450">most</span>
  <span m="528780">of</span> <span m="528840">biomedical</span> <span m="529320">research,</span>
  <span m="529720">and</span> <span m="529860">it's probably</span> <span m="530130">this</span>
  <span m="530310">one.</span> <span m="530790">And</span> <span m="530910">it's</span>
  <span m="531030">extremely</span> <span m="531840">simple.</span> <span m="533020">So</span>
  <span m="533580">it's</span> <span m="533760">really</span> <span m="534030">just</span>
  <span m="534180">an</span> <span m="534300">empirical</span> <span m="536010">distribution</span>
  <span m="536640">of</span> <span m="536700">how</span> <span m="536880">patients</span>
  <span m="537390">are</span> <span m="537750">doing</span> <span m="538140">over</span>
  <span m="538440">time.</span></p><p><span m="539350">So</span> <span m="539400">the</span>
  <span m="539520">x-axis</span> <span m="540180">is</span> <span m="540390">time.</span>
  <span m="541290">And</span> <span m="541500">here,</span> <span m="542010">the</span>
  <span m="542190">goal</span> <span m="542640">is</span> <span m="542820">to</span>
  <span m="542940">build</span> <span m="543330">a</span> <span m="543360">prognostic</span>
  <span m="544080">model.</span> <span m="544380">I</span> <span m="544460">wish</span>
  <span m="544580">I</span> <span m="544620">had</span> <span m="544710">a</span>
  <span m="544770">predictive</span> <span m="545160">one</span> <span m="545310">in</span>
  <span m="545400">here,</span> <span m="545650">but</span> <span m="545750">we</span>
  <span m="545850">can</span> <span m="545950">talk</span> <span m="545960">about
  what</span> <span m="546110">that</span> <span m="546200">would</span> <span m="546300">look</span>
  <span m="546450">like.</span> <span m="547020">But</span> <span m="547200">a</span>
  <span m="547260">prognostic</span> <span m="547830">model,</span> <span m="548460">any</span>
  <span m="548700">sort</span> <span m="548850">of</span> <span m="548910">prognostic</span>
  <span m="549450">test</span> <span m="549840">in</span> <span m="549990">any</span>
  <span m="550260">disease</span> <span m="550620">in</span> <span m="550710">medicine</span>
  <span m="551430">is</span> <span m="551610">to</span> <span m="551700">try</span>
  <span m="551880">to</span> <span m="551970">create</span> <span m="552270">subgroups</span>
  <span m="552870">that</span> <span m="552990">show</span> <span m="553140">different</span>
  <span m="553470">survival</span> <span m="553890">outcomes.</span></p><p><span m="554670">And</span>
  <span m="554790">then</span> <span m="554880">by</span> <span m="555030">implication,</span>
  <span m="555660">they</span> <span m="555780">may</span> <span m="555960">benefit</span>
  <span m="556320">from</span> <span m="556470">different</span> <span m="556710">therapies.</span>
  <span m="557220">They</span> <span m="557340">may</span> <span m="557520">not.</span>
  <span m="558030">That</span> <span m="558180">doesn't</span> <span m="558420">answer</span>
  <span m="558660">that</span> <span m="558780">question,</span> <span m="559170">but</span>
  <span m="559290">it</span> <span m="559380">just</span> <span m="559530">tells</span>
  <span m="559860">you</span> <span m="559980">if</span> <span m="560070">you</span>
  <span m="560160">want</span> <span m="560280">to</span> <span m="560430">make</span>
  <span m="560670">an</span> <span m="560760">estimate</span> <span m="561270">for</span>
  <span m="561780">how</span> <span m="561990">a</span> <span m="562050">patient's</span>
  <span m="562390">going</span> <span m="562490">to</span> <span m="562570">be</span>
  <span m="562650">doing</span> <span m="562860">in</span> <span m="562950">five</span>
  <span m="563250">years,</span> <span m="564240">and</span> <span m="564390">you</span>
  <span m="564510">can</span> <span m="564660">sub-classify</span> <span m="565350">them</span>
  <span m="565470">into</span> <span m="565620">two</span> <span m="565830">groups,</span>
  <span m="566350">this</span> <span m="566400">is</span> <span m="566520">a</span>
  <span m="566580">way</span> <span m="566670">to</span> <span m="566760">visualize
  it.</span> <span m="567150">You</span> <span m="567210">don't</span> <span m="567390">need</span>
  <span m="567630">two</span> <span m="567810">groups.</span> <span m="568140">You</span>
  <span m="568200">could</span> <span m="568320">do</span> <span m="568410">this</span>
  <span m="568530">with</span> <span m="568650">even</span> <span m="568830">one</span>
  <span m="569010">group,</span> <span m="569460">but</span> <span m="569640">it's</span>
  <span m="569760">frequently</span> <span m="570300">used</span> <span m="570450">to</span>
  <span m="570540">show</span> <span m="570750">differences</span> <span m="571380">between</span>
  <span m="571680">two</span> <span m="571860">groups.</span></p><p><span m="572730">So</span>
  <span m="573420">you'll</span> <span m="573620">see</span> <span m="573810">here,</span>
  <span m="573960">there's</span> <span m="574110">a</span> <span m="574140">black</span>
  <span m="574440">line</span> <span m="574860">and</span> <span m="575130">a</span>
  <span m="575220">red</span> <span m="575400">line.</span> <span m="576460">And</span>
  <span m="576750">these</span> <span m="576990">are</span> <span m="577080">groups</span>
  <span m="577350">of</span> <span m="577440">patients</span> <span m="577890">where</span>
  <span m="578160">a</span> <span m="578250">model</span> <span m="579720">trained</span>
  <span m="580230">not</span> <span m="580440">on</span> <span m="580530">these</span>
  <span m="580680">cases</span> <span m="581160">was</span> <span m="581370">trained</span>
  <span m="581700">to</span> <span m="581970">separate</span> <span m="582540">high-risk</span>
  <span m="583080">patients</span> <span m="583470">from</span> <span m="583620">low-risk</span>
  <span m="584010">patients.</span></p><p><span m="584850">And</span> <span m="584970">the</span>
  <span m="585030">way</span> <span m="585180">we</span> <span m="585270">did</span>
  <span m="585420">that</span> <span m="585690">was</span> <span m="585930">we</span>
  <span m="586020">did</span> <span m="586200">logistic</span> <span m="586680">regression</span>
  <span m="587370">on</span> <span m="587490">a</span> <span m="587550">different</span>
  <span m="587880">data</span> <span m="588130">set,</span> <span m="588870">sort</span>
  <span m="589110">of</span> <span m="589200">trying</span> <span m="589410">to</span>
  <span m="589470">classify</span> <span m="590130">patients</span> <span m="590520">alive</span>
  <span m="590850">at</span> <span m="590910">five</span> <span m="591210">years</span>
  <span m="591480">following</span> <span m="591720">diagnosis</span> <span m="592260">versus</span>
  <span m="592560">patients</span> <span m="592980">deceased,</span> <span m="593400">five</span>
  <span m="593610">years</span> <span m="593730">diagnosis.</span></p><p><span m="594510">We</span>
  <span m="594600">build</span> <span m="594790">a</span> <span m="594840">model.</span>
  <span m="595200">We</span> <span m="595320">fix</span> <span m="595590">the</span>
  <span m="595680">model.</span> <span m="596310">Then</span> <span m="596430">we</span>
  <span m="596490">apply</span> <span m="596760">it</span> <span m="596850">to</span>
  <span m="596940">this</span> <span m="597090">data</span> <span m="597280">set</span>
  <span m="597480">of</span> <span m="597570">about</span> <span m="597820">250</span>
  <span m="598260">cases.</span> <span m="600280">And</span> <span m="600300">then</span>
  <span m="600450">we</span> <span m="600540">just</span> <span m="600750">ask,</span>
  <span m="601300">did</span> <span m="601410">we</span> <span m="601530">actually</span>
  <span m="601890">effectively</span> <span m="602430">create</span> <span m="602790">two</span>
  <span m="603060">different</span> <span m="603720">groups</span> <span m="603990">of</span>
  <span m="604050">patients</span> <span m="604800">whose</span> <span m="605130">survival</span>
  <span m="605670">distribution</span> <span m="607110">is</span> <span m="607290">significantly</span>
  <span m="607860">different?</span></p><p><span m="608770">So</span> <span m="608850">what</span>
  <span m="608940">this</span> <span m="609090">p-value</span> <span m="609510">is</span>
  <span m="609660">telling</span> <span m="609960">you</span> <span m="610050">is</span>
  <span m="610170">the</span> <span m="610260">probability</span> <span m="611520">that</span>
  <span m="611640">these</span> <span m="611820">two</span> <span m="612000">curves</span>
  <span m="612450">come</span> <span m="612690">from</span> <span m="612870">the</span>
  <span m="612960">same</span> <span m="613230">underlying</span> <span m="613650">distribution</span>
  <span m="614250">or</span> <span m="614370">that</span> <span m="614490">there's</span>
  <span m="614640">no</span> <span m="614850">difference</span> <span m="615360">between</span>
  <span m="615660">these</span> <span m="615810">two</span> <span m="615960">curves</span>
  <span m="616740">across</span> <span m="617730">all</span> <span m="617970">of</span>
  <span m="618060">the</span> <span m="618150">time</span> <span m="618390">points.</span>
  <span m="619720">And</span> <span m="619820">what</span> <span m="619830">we</span>
  <span m="619950">see</span> <span m="620100">here</span> <span m="620250">is</span>
  <span m="620370">there</span> <span m="620670">seems</span> <span m="620940">to</span>
  <span m="621030">be</span> <span m="621120">a</span> <span m="621180">difference</span>
  <span m="621630">between</span> <span m="621990">the</span> <span m="622110">black</span>
  <span m="622380">line</span> <span m="622680">versus</span> <span m="623040">the</span>
  <span m="623160">red</span> <span m="623310">line,</span> <span m="623610">where,</span>
  <span m="624180">say,</span> <span m="624600">10</span> <span m="624900">years,</span>
  <span m="626736">the</span> <span m="627180">probability</span> <span m="627780">of</span>
  <span m="627870">survival</span> <span m="628470">is</span> <span m="628650">about</span>
  <span m="628890">80%</span> <span m="629580">in</span> <span m="629670">the</span>
  <span m="629760">low-risk</span> <span m="629920">group</span> <span m="630390">and</span>
  <span m="630480">more</span> <span m="630630">like</span> <span m="630930">60%</span>
  <span m="631620">in</span> <span m="631710">the</span> <span m="631770">high-risk</span>
  <span m="632070">group.</span></p><p><span m="632310">And</span> <span m="632460">overall,</span>
  <span m="633210">the</span> <span m="633300">p-value's</span> <span m="634410">very</span>
  <span m="634680">small</span> <span m="635160">for</span> <span m="635580">there</span>
  <span m="635730">being</span> <span m="635880">a</span> <span m="635950">difference</span>
  <span m="636210">between</span> <span m="636270">those</span> <span m="636390">two</span>
  <span m="636540">curves.</span> <span m="636900">So that's</span> <span m="637050">sort</span>
  <span m="637200">of</span> <span m="637260">like</span> <span m="637380">what</span>
  <span m="637500">a</span> <span m="637530">successful</span> <span m="638580">type</span>
  <span m="639280">Kaplan-Meier</span> <span m="639930">plot</span> <span m="640200">would</span>
  <span m="640350">look</span> <span m="640530">like</span> <span m="640740">if</span>
  <span m="640830">you're</span> <span m="640920">trying</span> <span m="641190">to</span>
  <span m="641280">create</span> <span m="641640">a</span> <span m="641700">model</span>
  <span m="642360">that</span> <span m="642540">separates</span> <span m="643050">patients</span>
  <span m="643440">into</span> <span m="643590">groups</span> <span m="643860">with</span>
  <span m="644010">different</span> <span m="644400">survival</span> <span m="644790">distributions</span></p><p><span
  m="645840">And</span> <span m="645930">then</span> <span m="646050">it's</span>
  <span m="646200">always</span> <span m="646440">important</span> <span m="646800">for</span>
  <span m="646890">these</span> <span m="647070">types</span> <span m="647280">of</span>
  <span m="647370">things</span> <span m="647670">to</span> <span m="647730">try</span>
  <span m="647910">them</span> <span m="648020">on</span> <span m="648120">multiple</span>
  <span m="648510">data</span> <span m="648730">sets.</span> <span m="649030">And</span>
  <span m="649140">here</span> <span m="649320">we</span> <span m="649410">show</span>
  <span m="649860">the</span> <span m="649950">same</span> <span m="650190">model</span>
  <span m="650580">applied</span> <span m="650850">to a</span> <span m="650940">different</span>
  <span m="651150">data</span> <span m="651320">set</span> <span m="651510">showed</span>
  <span m="652530">pretty</span> <span m="652800">similar</span> <span m="653250">overall</span>
  <span m="654330">effectiveness</span> <span m="654990">at</span> <span m="655140">stratifying</span>
  <span m="655700">patients</span> <span m="656040">into</span> <span m="656190">two</span>
  <span m="656340">groups.</span></p><p><span m="657820">So</span> <span m="657900">why</span>
  <span m="658050">do</span> <span m="658110">you</span> <span m="658170">think</span>
  <span m="658530">doing</span> <span m="658860">this</span> <span m="659220">might</span>
  <span m="659610">be</span> <span m="659760">useful?</span> <span m="661320">I</span>
  <span m="661410">guess,</span> <span m="661830">yeah,</span> <span m="662010">anyone?</span>
  <span m="664960">Because</span> <span m="665160">there's</span> <span m="665370">actually,</span>
  <span m="665760">I</span> <span m="665850">think</span> <span m="666030">this</span>
  <span m="666360">type</span> <span m="666600">of</span> <span m="666690">curve</span>
  <span m="666960">is</span> <span m="667080">often</span> <span m="667320">confused</span>
  <span m="667800">with</span> <span m="667950">one</span> <span m="668130">that</span>
  <span m="668250">actually</span> <span m="668520">is</span> <span m="668700">extremely</span>
  <span m="669240">useful,</span> <span m="670270">which</span> <span m="670380">I</span>
  <span m="670500">would</span> <span m="670620">say--</span> <span m="670910">yeah?</span></p><p><span
  m="671130">PROFESSOR:</span> <span m="671240">Why</span> <span m="671350">don't</span>
  <span m="671460">you</span> <span m="671570">wait?</span></p><p><span m="672010">ANDY
  BECK:</span> <span m="672155">Sure.</span></p><p><span m="674320">PROFESSOR:</span>
  <span m="674375">Don't</span> <span m="674430">be</span> <span m="674500">shy.</span>
  <span m="678500">You can call</span> <span m="678750">them.</span></p><p><span m="680080">ANDY
  BECK:</span> <span m="680110">All</span> <span m="680140">right.</span></p><p><span
  m="681270">AUDIENCE:</span> <span m="681470">Probably</span> <span m="682315">you</span>
  <span m="682680">can you use</span> <span m="682980">this to</span> <span m="683850">start
  off</span> <span m="684890">when</span> <span m="686510">the</span> <span m="686710">patient's</span>
  <span m="687120">of</span> <span m="687330">high-risk</span> <span m="687760">and</span>
  <span m="688160">probably at</span> <span m="688600">five</span> <span m="688730">years,</span>
  <span m="689040">if the patient</span> <span m="689370">has high-risk,</span> <span
  m="689850">probably</span> <span m="690880">do</span> <span m="691320">a</span>
  <span m="691670">follow-up.</span></p><p><span m="693090">ANDY BECK:</span> <span
  m="693245">Right,</span> <span m="693400">exactly.</span> <span m="693990">Yeah,</span>
  <span m="695320">yeah.</span> <span m="695870">So</span> <span m="695990">that would</span>
  <span m="696110">be</span> <span m="696230">a</span> <span m="696290">great</span>
  <span m="696620">use.</span></p><p><span m="697010">PROFESSOR:</span> <span m="697070">Can</span>
  <span m="697130">you</span> <span m="697190">repeat</span> <span m="697340">the</span>
  <span m="697400">question for the</span> <span m="697730">recording?</span></p><p><span
  m="698100">ANDY BECK:</span> <span m="698305">So</span> <span m="698740">it</span>
  <span m="698840">was</span> <span m="698960">saying</span> <span m="699260">like</span>
  <span m="700040">if</span> <span m="700190">you</span> <span m="700280">know</span>
  <span m="700460">someone's</span> <span m="700910">at</span> <span m="701380">a</span>
  <span m="701480">high</span> <span m="701780">risk</span> <span m="702170">of</span>
  <span m="702260">having</span> <span m="702590">an</span> <span m="702680">event</span>
  <span m="703070">prior</span> <span m="703430">to</span> <span m="703490">five</span>
  <span m="703790">years,</span> <span m="704090">an</span> <span m="704180">event</span>
  <span m="704570">is</span> <span m="704720">when</span> <span m="704900">the</span>
  <span m="705020">curve</span> <span m="705290">goes</span> <span m="705500">down.</span>
  <span m="706190">So</span> <span m="706370">definitely,</span> <span m="707000">the</span>
  <span m="707180">red</span> <span m="707600">group</span> <span m="708530">is</span>
  <span m="708770">at</span> <span m="710600">40,</span> <span m="712130">almost</span>
  <span m="712430">double</span> <span m="712970">or</span> <span m="713060">something</span>
  <span m="714560">the</span> <span m="714710">risk</span> <span m="715040">of</span>
  <span m="715100">the</span> <span m="715190">black</span> <span m="715460">group.</span></p><p><span
  m="716150">So</span> <span m="716960">if</span> <span m="717080">you</span> <span
  m="717200">have</span> <span m="717380">certain</span> <span m="717620">interventions</span>
  <span m="718220">you</span> <span m="718310">can</span> <span m="718460">do</span>
  <span m="718940">to</span> <span m="719120">help</span> <span m="719960">prevent</span>
  <span m="720410">these</span> <span m="720650">things,</span> <span m="721340">such</span>
  <span m="721580">as</span> <span m="721730">giving</span> <span m="721940">an</span>
  <span m="721990">additional</span> <span m="722300">treatment</span> <span m="722780">or</span>
  <span m="722900">giving</span> <span m="723470">more</span> <span m="723740">frequent</span>
  <span m="724190">monitoring</span> <span m="724670">for</span> <span m="724820">recurrence.</span>
  <span m="725390">Like</span> <span m="725570">if</span> <span m="725660">you can</span>
  <span m="725780">do</span> <span m="725870">a</span> <span m="725930">follow-up</span>
  <span m="726470">scan</span> <span m="726920">in</span> <span m="727460">a</span>
  <span m="727520">month</span> <span m="727850">versus</span> <span m="728150">six</span>
  <span m="728420">months,</span> <span m="729170">you</span> <span m="729290">could</span>
  <span m="729410">make</span> <span m="729620">that</span> <span m="729770">decision</span>
  <span m="730160">in</span> <span m="730310">a</span> <span m="730370">data-driven</span>
  <span m="730880">way</span> <span m="731090">by</span> <span m="731240">knowing</span>
  <span m="731660">whether</span> <span m="731870">the</span> <span m="731930">patient's</span>
  <span m="732260">on</span> <span m="732350">the</span> <span m="732410">red</span>
  <span m="732590">curve</span> <span m="732810">or</span> <span m="732870">the</span>
  <span m="732950">black</span> <span m="733190">curve.</span></p><p><span m="735230">So</span>
  <span m="735500">yeah,</span> <span m="735710">exactly</span> <span m="736190">right.</span>
  <span m="736370">It</span> <span m="736430">helps</span> <span m="736730">you</span>
  <span m="736790">to</span> <span m="736850">make</span> <span m="737030">therapeutic</span>
  <span m="737450">decisions</span> <span m="737870">when</span> <span m="737990">there's</span>
  <span m="738140">a</span> <span m="738200">bunch</span> <span m="738500">of</span>
  <span m="738620">things</span> <span m="738860">you</span> <span m="738920">can</span>
  <span m="739040">do,</span> <span m="739220">either</span> <span m="739400">give</span>
  <span m="739550">more</span> <span m="739670">aggressive</span> <span m="739970">treatment</span>
  <span m="740360">or</span> <span m="740420">do</span> <span m="740540">more</span>
  <span m="740690">aggressive</span> <span m="741110">monitoring</span> <span m="741590">of</span>
  <span m="741680">disease,</span> <span m="742160">depending</span> <span m="742670">on</span>
  <span m="742970">is</span> <span m="743495">it</span> <span m="743750">aggressive</span>
  <span m="744140">disease</span> <span m="744500">or</span> <span m="744800">a non-aggressive</span>
  <span m="745340">disease.</span></p><p><span m="746190">The</span> <span m="746210">other</span>
  <span m="746390">type</span> <span m="746630">of</span> <span m="746720">curve</span>
  <span m="747080">that</span> <span m="747260">I</span> <span m="747350">think</span>
  <span m="747470">often</span> <span m="747680">gets</span> <span m="747830">confused</span>
  <span m="748160">with</span> <span m="748280">these</span> <span m="748490">that's</span>
  <span m="748640">quite</span> <span m="748880">useful</span> <span m="750530">is</span>
  <span m="750680">one</span> <span m="750890">that</span> <span m="751010">directly</span>
  <span m="751670">tests</span> <span m="752420">that</span> <span m="752720">intervention.</span>
  <span m="754050">So</span> <span m="754190">essentially,</span> <span m="754670">you</span>
  <span m="754820">could</span> <span m="754940">do</span> <span m="755060">a</span>
  <span m="755120">trial</span> <span m="755720">of</span> <span m="756410">the</span>
  <span m="756560">usefulness,</span> <span m="757370">the</span> <span m="757490">clinical</span>
  <span m="757880">utility</span> <span m="758390">of</span> <span m="758450">this</span>
  <span m="758600">algorithm,</span> <span m="759580">where</span> <span m="759770">on</span>
  <span m="759860">the</span> <span m="759950">one</span> <span m="760130">hand,</span>
  <span m="760490">you</span> <span m="760880">make</span> <span m="761090">the</span>
  <span m="761180">prediction</span> <span m="761540">on</span> <span m="761630">everyone</span>
  <span m="762140">and</span> <span m="762260">don't</span> <span m="762410">do</span>
  <span m="762530">anything</span> <span m="762890">differently.</span> <span m="764150">And</span>
  <span m="764300">then</span> <span m="764630">the</span> <span m="764810">other</span>
  <span m="765050">one</span> <span m="765590">is</span> <span m="766220">you</span>
  <span m="766370">make</span> <span m="766580">a</span> <span m="767000">prediction</span>
  <span m="767450">on</span> <span m="767540">the</span> <span m="767600">patients,</span>
  <span m="767990">and</span> <span m="768080">you</span> <span m="768170">actually</span>
  <span m="768440">use</span> <span m="768650">it</span> <span m="768710">to</span>
  <span m="768800">make</span> <span m="768980">a</span> <span m="769010">decision,</span>
  <span m="769490">like</span> <span m="769940">more</span> <span m="770150">frequent</span>
  <span m="770660">treatment</span> <span m="771260">or</span> <span m="772070">more</span>
  <span m="772220">frequent</span> <span m="772540">intervention.</span></p><p><span
  m="773270">And</span> <span m="773390">then</span> <span m="773540">you</span> <span
  m="773630">could</span> <span m="773750">do</span> <span m="773870">a</span> <span
  m="773930">curve,</span> <span m="774950">saying</span> <span m="775580">among</span>
  <span m="775910">the</span> <span m="776000">high-risk</span> <span m="776450">patients,</span>
  <span m="776990">where</span> <span m="777110">we</span> <span m="777230">actually</span>
  <span m="777500">acted</span> <span m="777920">on</span> <span m="778130">it,</span>
  <span m="779120">that's</span> <span m="779450">black.</span> <span m="780020">And</span>
  <span m="780110">if</span> <span m="780200">we</span> <span m="780290">didn't</span>
  <span m="780530">act</span> <span m="780770">on</span> <span m="780950">it,</span>
  <span m="781040">it's</span> <span m="781220">red.</span> <span m="782240">And</span>
  <span m="782390">then,</span> <span m="782750">if</span> <span m="782870">you</span>
  <span m="782960">do</span> <span m="783050">the</span> <span m="783140">experiment</span>
  <span m="783830">in</span> <span m="783950">the</span> <span m="784040">right</span>
  <span m="784190">way,</span> <span m="784640">you</span> <span m="784760">can</span>
  <span m="784880">make</span> <span m="785030">the</span> <span m="785090">inference</span>
  <span m="786440">that</span> <span m="787040">you're</span> <span m="787250">actually</span>
  <span m="788240">preventing</span> <span m="788960">death</span> <span m="789410">by</span>
  <span m="789620">50%</span> <span m="791240">if</span> <span m="791360">the</span>
  <span m="791480">intervention</span> <span m="791990">is</span> <span m="792140">causing</span>
  <span m="792740">black</span> <span m="793040">versus</span> <span m="793340">red.</span></p><p><span
  m="793910">Here,</span> <span m="794090">we're</span> <span m="794180">not</span>
  <span m="794330">doing</span> <span m="794510">anything</span> <span m="794690">with</span>
  <span m="794780">causality.</span> <span m="795350">We're</span> <span m="795440">just</span>
  <span m="795540">sort</span> <span m="795650">of</span> <span m="795740">observing</span>
  <span m="796340">how</span> <span m="796490">patients</span> <span m="797510">do</span>
  <span m="797720">differently</span> <span m="798140">over</span> <span m="798290">time.</span>
  <span m="798890">But</span> <span m="799100">frequently,</span> <span m="799670">you</span>
  <span m="799760">see</span> <span m="799940">these</span> <span m="800240">as</span>
  <span m="800860">the</span> <span m="801020">figure,</span> <span m="801470">the</span>
  <span m="801590">key</span> <span m="801860">figure</span> <span m="802250">for</span>
  <span m="802370">a</span> <span m="802430">randomized</span> <span m="802850">control</span>
  <span m="803150">trial,</span> <span m="803990">where</span> <span m="805550">the</span>
  <span m="805670">only</span> <span m="805850">thing</span> <span m="806030">different</span>
  <span m="806270">between the</span> <span m="806720">groups</span> <span m="806930">of</span>
  <span m="806990">patients</span> <span m="807350">is</span> <span m="807560">the</span>
  <span m="807680">intervention.</span> <span m="808740">And</span> <span m="808790">that</span>
  <span m="809000">really</span> <span m="809360">lets you</span> <span m="809600">make</span>
  <span m="809750">a</span> <span m="809780">powerful</span> <span m="810230">inference</span>
  <span m="810830">that</span> <span m="810980">changes</span> <span m="811430">what</span>
  <span m="811580">care</span> <span m="811850">should</span> <span m="812060">be.</span></p><p><span
  m="812510">This</span> <span m="812750">one,</span> <span m="812900">you're</span>
  <span m="813000">just</span> <span m="813140">like,</span> <span m="813420">OK,</span>
  <span m="813720">maybe</span> <span m="813890">we</span> <span m="813950">should</span>
  <span m="814070">do</span> <span m="814130">something</span> <span m="814340">differently,</span>
  <span m="814800">but</span> <span m="814820">not</span> <span m="814970">really</span>
  <span m="815120">sure,</span> <span m="815600">but</span> <span m="815720">it</span>
  <span m="815780">makes</span> <span m="816500">intuitive</span> <span m="816920">sense.</span>
  <span m="817740">But</span> <span m="817790">if</span> <span m="817880">you</span>
  <span m="817940">actually</span> <span m="818180">have</span> <span m="818270">something</span>
  <span m="818450">from</span> <span m="818600">a</span> <span m="818630">randomized</span>
  <span m="818950">clinical</span> <span m="819170">trial</span> <span m="819620">or</span>
  <span m="819710">something</span> <span m="820040">else</span> <span m="820220">that</span>
  <span m="820310">allows</span> <span m="820550">you</span> <span m="820610">to</span>
  <span m="820730">infer</span> <span m="821030">causality,</span> <span m="821900">this</span>
  <span m="822140">is</span> <span m="822665">the</span> <span m="823040">most</span>
  <span m="823310">important</span> <span m="823670">figure.</span></p><p><span m="825380">And</span>
  <span m="825410">you</span> <span m="825500">can</span> <span m="825590">actually</span>
  <span m="825830">infer</span> <span m="826370">how</span> <span m="826490">many</span>
  <span m="827120">lives</span> <span m="827510">are</span> <span m="827600">being</span>
  <span m="827780">saved</span> <span m="828200">or</span> <span m="828290">things</span>
  <span m="828560">by</span> <span m="828770">doing</span> <span m="829130">something.</span>
  <span m="829790">But</span> <span m="829940">this</span> <span m="830120">one's</span>
  <span m="830300">not</span> <span m="830510">about</span> <span m="830750">intervention.</span>
  <span m="831320">It's</span> <span m="831410">just</span> <span m="831590">about</span>
  <span m="831740">sort</span> <span m="831860">of</span> <span m="831950">observing</span>
  <span m="833090">how</span> <span m="833270">patients</span> <span m="833600">do</span>
  <span m="833690">over</span> <span m="833840">time.</span></p><p><span m="836130">So</span>
  <span m="836270">that</span> <span m="836420">was</span> <span m="836870">some</span>
  <span m="837170">of</span> <span m="837290">the</span> <span m="837410">work</span>
  <span m="837920">from</span> <span m="838570">eight</span> <span m="838700">years</span>
  <span m="839000">ago,</span> <span m="839750">and</span> <span m="839900">none</span>
  <span m="840110">of</span> <span m="840170">this</span> <span m="841130">has</span>
  <span m="841310">really</span> <span m="841490">changed</span> <span m="841820">in</span>
  <span m="841910">practice.</span> <span m="842510">Everyone is</span> <span m="842720">still</span>
  <span m="842870">using</span> <span m="843080">glass</span> <span m="843290">slides</span>
  <span m="843510">and</span> <span m="843590">microscopes</span> <span m="844250">in</span>
  <span m="844430">the</span> <span m="844520">clinic.</span> <span m="845030">Research</span>
  <span m="845560">is</span> <span m="845900">a</span> <span m="845960">totally</span>
  <span m="846200">different</span> <span m="846440">story.</span> <span m="847290">But</span>
  <span m="847370">still,</span> <span m="847670">99%</span> <span m="848300">of</span>
  <span m="848360">clinic</span> <span m="850100">is</span> <span m="850280">using</span>
  <span m="850640">these</span> <span m="850790">old-fashioned</span> <span m="851240">technologies--</span>
  <span m="851870">microscopes</span> <span m="852500">from</span> <span m="853100">technology</span>
  <span m="853850">breakthroughs</span> <span m="854350">in the mid-1800s,</span>
  <span m="855290">staining</span> <span m="855830">breakthroughs</span> <span m="856460">in</span>
  <span m="856760">the</span> <span m="856880">late</span> <span m="857150">1800s.</span>
  <span m="858020">The</span> <span m="858140">H</span> <span m="858400">and E</span>
  <span m="858530">stain</span> <span m="858950">is</span> <span m="859100">the</span>
  <span m="859370">key</span> <span m="859610">stain.</span></p><p><span m="860480">So</span>
  <span m="861170">aspects</span> <span m="861650">of</span> <span m="861710">pathology</span>
  <span m="862310">haven't</span> <span m="862520">moved</span> <span m="862790">forward
  at</span> <span m="862940">all,</span> <span m="863600">and</span> <span m="863720">this</span>
  <span m="863870">has</span> <span m="864110">pretty</span> <span m="864650">significant</span>
  <span m="865460">consequences.</span> <span m="866300">And</span> <span m="866450">here's</span>
  <span m="866630">just</span> <span m="866780">a</span> <span m="866840">couple</span>
  <span m="867550">of</span> <span m="867680">types</span> <span m="868040">of</span>
  <span m="868130">figures</span> <span m="868610">that</span> <span m="868760">really</span>
  <span m="869480">allow</span> <span m="869720">you</span> <span m="869780">to</span>
  <span m="869870">see</span> <span m="870020">the</span> <span m="870170">primary</span>
  <span m="870650">data</span> <span m="871010">for</span> <span m="871160">what</span>
  <span m="871280">a</span> <span m="871310">problem</span> <span m="871790">interobserver</span>
  <span m="872660">variability</span> <span m="873410">really</span> <span m="873740">is</span>
  <span m="873920">in</span> <span m="873980">clinical</span> <span m="874280">practice.</span>
  <span m="875250">And</span> <span m="875270">this</span> <span m="875420">is</span>
  <span m="875540">just</span> <span m="875720">another,</span> <span m="876140">I</span>
  <span m="876230">think,</span> <span m="876380">really</span> <span m="876620">nice,</span>
  <span m="877010">empirical</span> <span m="878060">way</span> <span m="878420">of</span>
  <span m="878540">viewing</span> <span m="878900">raw</span> <span m="879110">data,</span>
  <span m="880160">where</span> <span m="881090">there</span> <span m="881260">is</span>
  <span m="881360">a</span> <span m="881570">ground</span> <span m="881960">truth</span>
  <span m="882230">consensus</span> <span m="883070">of</span> <span m="883220">experts,</span>
  <span m="884060">who</span> <span m="884180">sort</span> <span m="884390">of</span>
  <span m="884480">decided</span> <span m="884960">what</span> <span m="885140">all</span>
  <span m="885320">these</span> <span m="885470">70</span> <span m="886130">or</span>
  <span m="886220">so</span> <span m="886430">cases</span> <span m="886910">were,</span>
  <span m="887510">through</span> <span m="888100">experts</span> <span m="888800">always</span>
  <span m="889010">knowing</span> <span m="889190">the</span> <span m="889250">right</span>
  <span m="889430">answer.</span></p><p><span m="890210">And</span> <span m="890570">for</span>
  <span m="890780">all</span> <span m="890990">of</span> <span m="891080">these</span>
  <span m="891230">70,</span> <span m="891710">called</span> <span m="891980">them</span>
  <span m="892160">all</span> <span m="892490">the</span> <span m="892640">category</span>
  <span m="893000">of</span> <span m="893090">atypia,</span> <span m="893820">which</span>
  <span m="893930">here</span> <span m="894080">is</span> <span m="894200">indicated</span>
  <span m="894530">in</span> <span m="894650">yellow.</span> <span m="895530">And</span>
  <span m="895550">then</span> <span m="895670">they</span> <span m="895790">took</span>
  <span m="896090">all</span> <span m="896240">of</span> <span m="896300">these</span>
  <span m="896450">70</span> <span m="896810">cases</span> <span m="897350">that</span>
  <span m="897440">the</span> <span m="897560">experts</span> <span m="897980">that</span>
  <span m="898070">are</span> <span m="898160">atypia</span> <span m="898740">and</span>
  <span m="899030">sent</span> <span m="899330">them</span> <span m="899450">to</span>
  <span m="899840">hundreds</span> <span m="900230">of</span> <span m="900320">pathologists</span>
  <span m="901040">across</span> <span m="901520">the</span> <span m="901610">country</span>
  <span m="902540">and</span> <span m="902660">for</span> <span m="902780">each</span>
  <span m="902960">one,</span> <span m="903290">just</span> <span m="903890">plotted</span>
  <span m="904400">the</span> <span m="904490">distribution</span> <span m="905150">of</span>
  <span m="905240">different</span> <span m="905480">diagnoses</span> <span m="905960">they</span>
  <span m="906080">were</span> <span m="906170">receiving.</span></p><p><span m="907040">And</span>
  <span m="907340">quite</span> <span m="907730">strikingly--</span> <span m="908420">and</span>
  <span m="908510">this</span> <span m="908630">was</span> <span m="908720">published</span>
  <span m="909140">in</span> <span m="909230"><i>JAMA,</i></span> <span m="909500">a</span>
  <span m="909770">great</span> <span m="910130">journal,</span> <span m="910520">about</span>
  <span m="910910">four</span> <span m="911150">years</span> <span m="911360">ago</span>
  <span m="911510">now--</span> <span m="912200">they</span> <span m="912350">show</span>
  <span m="912500">this</span> <span m="912620">incredible</span> <span m="913010">distribution</span>
  <span m="914150">of</span> <span m="914270">different</span> <span m="914600">diagnoses</span>
  <span m="915170">among</span> <span m="915440">each</span> <span m="915620">case.</span>
  <span m="916500">So</span> <span m="916520">this</span> <span m="916670">is</span>
  <span m="917090">really</span> <span m="917600">why</span> <span m="917820">you</span>
  <span m="917900">might</span> <span m="918050">want</span> <span m="918170">a</span>
  <span m="918210">computational</span> <span m="918740">approach</span> <span m="919020">is</span>
  <span m="919460">there</span> <span m="919550">should</span> <span m="919700">be</span>
  <span m="919790">the</span> <span m="919850">same</span> <span m="920060">color.</span>
  <span m="920570">This</span> <span m="920690">should</span> <span m="920810">just</span>
  <span m="920930">be</span> <span m="921050">one</span> <span m="921230">big</span>
  <span m="921380">color</span> <span m="921800">or</span> <span m="921890">maybe</span>
  <span m="922190">a</span> <span m="922250">few</span> <span m="922490">outliers,</span>
  <span m="922880">but</span> <span m="923240">for</span> <span m="923330">almost</span>
  <span m="923540">any</span> <span m="923720">case,</span> <span m="924020">there's</span>
  <span m="924200">a</span> <span m="924590">significant</span> <span m="925190">proportion</span>
  <span m="925670">of</span> <span m="925770">people</span> <span m="925880">calling</span>
  <span m="926150">it</span> <span m="926240">normal,</span> <span m="926630">which</span>
  <span m="926810">is</span> <span m="927140">yellow--</span> <span m="927860">or</span>
  <span m="927950">sorry,</span> <span m="928160">tan,</span> <span m="928950">then</span>
  <span m="929120">atypical,</span> <span m="929570">which</span> <span m="929750">is</span>
  <span m="929960">yellow,</span> <span m="930350">and</span> <span m="930440">then</span>
  <span m="930680">actually</span> <span m="930980">cancer,</span> <span m="931560">which</span>
  <span m="931610">is</span> <span m="931730">orange</span> <span m="931970">or</span>
  <span m="932030">red.</span></p><p><span m="933170">PROFESSOR:</span> <span m="933215">What</span>
  <span m="933260">does</span> <span m="933410">atypical</span> <span m="933980">mean?</span></p><p><span
  m="935010">ANDY BECK:</span> <span m="935090">Yeah,</span> <span m="935170">so</span>
  <span m="935360">atypical</span> <span m="935930">is</span> <span m="936140">this</span>
  <span m="936320">border</span> <span m="936770">area</span> <span m="937100">between</span>
  <span m="937850">totally</span> <span m="938330">normal</span> <span m="938840">and</span>
  <span m="938990">cancer,</span> <span m="939740">where</span> <span m="940100">the</span>
  <span m="940220">pathologist</span> <span m="940790">is</span> <span m="940880">saying</span>
  <span m="941990">it's--</span> <span m="942500">which</span> <span m="942710">is</span>
  <span m="942800">actually</span> <span m="943100">the</span> <span m="943220">most</span>
  <span m="943520">important</span> <span m="944940">diagnosis</span> <span m="945770">because</span>
  <span m="945950">totally</span> <span m="946220">normal</span> <span m="946490">you</span>
  <span m="946550">do</span> <span m="946640">nothing.</span> <span m="947000">Cancer--</span>
  <span m="947810">there's</span> <span m="947990">well-described</span> <span m="948740">protocols</span>
  <span m="949220">for</span> <span m="949340">what</span> <span m="949460">to</span>
  <span m="949550">do.</span></p><p><span m="950350">Atypia,</span> <span m="950970">they</span>
  <span m="951110">often</span> <span m="951410">overtreat.</span> <span m="952070">And</span>
  <span m="952190">that's</span> <span m="952340">sort</span> <span m="952490">of</span>
  <span m="952550">the</span> <span m="952610">bias</span> <span m="953030">in</span>
  <span m="953120">medicine</span> <span m="953660">is</span> <span m="955100">always</span>
  <span m="955370">assume</span> <span m="955610">the</span> <span m="955700">worst</span>
  <span m="956030">when you</span> <span m="956120">get</span> <span m="956210">a</span>
  <span m="956240">certain</span> <span m="956420">diagnosis</span> <span m="956840">back.</span>
  <span m="957080">So</span> <span m="957250">atypia</span> <span m="957740">has</span>
  <span m="958460">nuclear</span> <span m="958850">features</span> <span m="959390">of</span>
  <span m="959510">cancer</span> <span m="960020">but</span> <span m="960170">doesn't</span>
  <span m="960410">fully.</span> <span m="961120">You</span> <span m="961220">know,</span>
  <span m="961280">maybe you</span> <span m="961460">get</span> <span m="961610">7</span>
  <span m="961910">of</span> <span m="961970">the</span> <span m="962060">10</span>
  <span m="962270">criteria</span> <span m="962900">or</span> <span m="963020">three</span>
  <span m="963200">of</span> <span m="963260">the</span> <span m="963320">five</span>
  <span m="963530">criteria.</span> <span m="965160">And</span> <span m="965240">it</span>
  <span m="965300">has</span> <span m="965510">to</span> <span m="965630">do</span>
  <span m="965840">with</span> <span m="966050">sort</span> <span m="966230">of</span>
  <span m="966470">nuclei</span> <span m="967130">looking</span> <span m="967580">a</span>
  <span m="967640">little</span> <span m="967850">bigger</span> <span m="968240">and</span>
  <span m="968360">a</span> <span m="968390">little</span> <span m="968600">weirder</span>
  <span m="969230">than</span> <span m="969440">expected</span> <span m="970010">but</span>
  <span m="970310">not</span> <span m="970550">enough</span> <span m="971430">where</span>
  <span m="971570">the</span> <span m="971630">pathologist</span> <span m="972080">feels</span>
  <span m="972290">comfortable</span> <span m="972710">calling</span> <span m="972920">it</span>
  <span m="972980">cancer.</span></p><p><span m="973730">And</span> <span m="973820">that's</span>
  <span m="974000">part</span> <span m="974210">of</span> <span m="974270">the</span>
  <span m="974330">reason</span> <span m="974660">that</span> <span m="974780">that</span>
  <span m="975020">shows</span> <span m="975590">almost</span> <span m="975860">a</span>
  <span m="975920">coin</span> <span m="976220">flip.</span> <span m="977540">Of</span>
  <span m="978020">the</span> <span m="978140">ones</span> <span m="978380">the</span>
  <span m="978500">experts</span> <span m="978890">called</span> <span m="979130">atypia,</span>
  <span m="979520">only</span> <span m="980420">48%</span> <span m="981620">was</span>
  <span m="981830">agreed</span> <span m="982130">with</span> <span m="982290">in</span>
  <span m="982340">the</span> <span m="982430">community.</span></p><p><span m="983240">The</span>
  <span m="983330">other</span> <span m="983480">interesting</span> <span m="983780">thing</span>
  <span m="983960">the</span> <span m="984020">study</span> <span m="984350">showed</span>
  <span m="984650">was</span> <span m="985070">intraobserver</span> <span m="986090">variability</span>
  <span m="986660">is</span> <span m="986780">just</span> <span m="986960">as</span>
  <span m="987080">big</span> <span m="987230">of</span> <span m="987320">an</span>
  <span m="987380">issue</span> <span m="987650">as</span> <span m="987800">interobserver.</span>
  <span m="989000">So</span> <span m="989150">a</span> <span m="989210">person</span>
  <span m="989600">disagrees</span> <span m="990140">with</span> <span m="990230">themselves</span>
  <span m="992390">after</span> <span m="992930">an</span> <span m="993050">eight</span>
  <span m="993170">month</span> <span m="993410">washout</span> <span m="993800">period</span>
  <span m="994340">pretty</span> <span m="994580">much</span> <span m="994790">as</span>
  <span m="994910">often</span> <span m="995240">as</span> <span m="995420">they</span>
  <span m="995795">disagree</span> <span m="996380">with</span> <span m="996530">others.</span>
  <span m="997340">So</span> <span m="997880">another</span> <span m="1000280">reason</span>
  <span m="1000640">why</span> <span m="1000760">computational</span> <span m="1001300">approaches</span>
  <span m="1001690">would</span> <span m="1001870">be</span> <span m="1001990">valuable</span>
  <span m="1002530">and</span> <span m="1002650">why</span> <span m="1002830">this</span>
  <span m="1003010">really</span> <span m="1003490">is</span> <span m="1003760">a</span>
  <span m="1003790">problem.</span> <span m="1004050">And</span> <span m="1004310">this</span>
  <span m="1004450">is</span> <span m="1004570">in</span> <span m="1004660">breast</span>
  <span m="1004900">biopsies.</span></p><p><span m="1005290">The</span> <span m="1005380">same</span>
  <span m="1005590">research</span> <span m="1005920">group</span> <span m="1006100">showed</span>
  <span m="1006820">quite</span> <span m="1007120">similar</span> <span m="1007420">results.</span>
  <span m="1007900">This</span> <span m="1008080">was</span> <span m="1008230">in</span>
  <span m="1008380"><i>British</i></span> <span m="1008800"><i>Medical</i></span>
  <span m="1009190"><i>Journal</i></span> <span m="1010230">in</span> <span m="1010420">skin</span>
  <span m="1010660">biopsies,</span> <span m="1011450">which</span> <span m="1011530">is</span>
  <span m="1011620">another</span> <span m="1011920">super</span> <span m="1012250">important</span>
  <span m="1012610">area,</span> <span m="1013030">where,</span> <span m="1013280">again</span>
  <span m="1013450">they</span> <span m="1013540">have</span> <span m="1013660">the</span>
  <span m="1013720">same</span> <span m="1013990">type</span> <span m="1014170">of</span>
  <span m="1014230">visualization</span> <span m="1014830">of</span> <span m="1014920">data.</span>
  <span m="1015880">They</span> <span m="1016090">have</span> <span m="1017110">five</span>
  <span m="1017560">different</span> <span m="1017980">classes</span> <span m="1018490">of</span>
  <span m="1018580">severity</span> <span m="1019390">of</span> <span m="1019690">skin</span>
  <span m="1019990">lesions,</span> <span m="1020470">ranging</span> <span m="1020830">from</span>
  <span m="1020980">a</span> <span m="1021010">totally</span> <span m="1021400">normal</span>
  <span m="1021760">benign</span> <span m="1022090">nevus,</span> <span m="1022450">like</span>
  <span m="1022600">I'm</span> <span m="1022690">sure</span> <span m="1023440">many</span>
  <span m="1023710">of</span> <span m="1023800">us</span> <span m="1023920">have</span>
  <span m="1024069">on</span> <span m="1024130">our</span> <span m="1024220">skin</span>
  <span m="1024579">to</span> <span m="1025030">a</span> <span m="1025089">melanoma,</span>
  <span m="1025690">which</span> <span m="1025839">is</span> <span m="1025930">a</span>
  <span m="1025990">serious,</span> <span m="1027339">malignant</span> <span m="1027849">cancer</span>
  <span m="1028359">that</span> <span m="1028480">needs</span> <span m="1028690">to</span>
  <span m="1028750">be</span> <span m="1028839">treated</span> <span m="1029319">as</span>
  <span m="1029410">soon</span> <span m="1029589">as</span> <span m="1029680">possible.</span></p><p><span
  m="1031569">And</span> <span m="1031720">here,</span> <span m="1032380">the</span>
  <span m="1032560">white</span> <span m="1032829">color</span> <span m="1033280">is</span>
  <span m="1033430">totally</span> <span m="1033940">benign.</span> <span m="1034470">The</span>
  <span m="1034780">darker</span> <span m="1035140">blue</span> <span m="1035349">color</span>
  <span m="1035680">is</span> <span m="1035859">melanoma.</span> <span m="1036790">And</span>
  <span m="1036910">again,</span> <span m="1037150">they</span> <span m="1037270">show</span>
  <span m="1037660">lots</span> <span m="1038020">of</span> <span m="1038079">discordance,</span>
  <span m="1038740">pretty</span> <span m="1038920">much</span> <span m="1039160">as</span>
  <span m="1039369">bad</span> <span m="1039670">as</span> <span m="1039819">in</span>
  <span m="1040390">the</span> <span m="1040480">breast</span> <span m="1040720">biopsies.</span>
  <span m="1042790">And</span> <span m="1043060">here</span> <span m="1043270">again,</span>
  <span m="1043480">the</span> <span m="1043599">intraobserver</span> <span m="1044920">variability</span>
  <span m="1045550">with</span> <span m="1045670">an</span> <span m="1045760">eight-month</span>
  <span m="1046270">washout</span> <span m="1046630">period</span> <span m="1046869">was</span>
  <span m="1046990">about</span> <span m="1047260">33%.</span> <span m="1048310">So</span>
  <span m="1048520">people</span> <span m="1048760">disagree</span> <span m="1049090">with</span>
  <span m="1049180">themselves</span> <span m="1049720">one</span> <span m="1049900">out</span>
  <span m="1049990">of</span> <span m="1050080">three</span> <span m="1050230">times.</span></p><p><span
  m="1053210">And</span> <span m="1053380">then</span> <span m="1053500">these</span>
  <span m="1053710">aren't</span> <span m="1054250">totally</span> <span m="1054700">outlier</span>
  <span m="1055090">cases</span> <span m="1055480">or</span> <span m="1055570">one</span>
  <span m="1055840">research</span> <span m="1056200">group.</span> <span m="1056530">The</span>
  <span m="1057280">College</span> <span m="1057640">of</span> <span m="1057730">American</span>
  <span m="1058090">Pathologists</span> <span m="1058660">did</span> <span m="1058750">a</span>
  <span m="1058780">big</span> <span m="1058930">summary</span> <span m="1059380">of</span>
  <span m="1059900">116</span> <span m="1060880">studies</span> <span m="1061330">and</span>
  <span m="1061420">showed</span> <span m="1061630">overall,</span> <span m="1062770">an</span>
  <span m="1062920">18.3%</span> <span m="1064600">median</span> <span m="1065080">discrepancy</span>
  <span m="1065740">rate</span> <span m="1066010">across</span> <span m="1066520">all</span>
  <span m="1066640">the</span> <span m="1066760">studies</span> <span m="1067750">and</span>
  <span m="1067900">a</span> <span m="1067960">6%</span> <span m="1068680">major</span>
  <span m="1069010">discrepancy</span> <span m="1069550">rate,</span> <span m="1069860">which</span>
  <span m="1069880">would</span> <span m="1069970">be</span> <span m="1070210">a</span>
  <span m="1070300">major</span> <span m="1070750">clinical</span> <span m="1071110">decision</span>
  <span m="1071740">is</span> <span m="1072340">the</span> <span m="1072490">wrong</span>
  <span m="1072790">one,</span> <span m="1073120">like</span> <span m="1073420">surgery,</span>
  <span m="1073840">no</span> <span m="1073990">surgery,</span> <span m="1074350">et</span>
  <span m="1074570">cetera.</span> <span m="1075130">And</span> <span m="1075220">those</span>
  <span m="1075390">sort</span> <span m="1075610">of</span> <span m="1075700">in</span>
  <span m="1075880">the</span> <span m="1076000">ballpark</span> <span m="1076420">agree</span>
  <span m="1076720">with</span> <span m="1077080">the</span> <span m="1077200">previously</span>
  <span m="1077590">published</span> <span m="1077890">findings.</span></p><p><span
  m="1080020">So</span> <span m="1081040">a</span> <span m="1081100">lot</span> <span
  m="1081310">of</span> <span m="1081370">reasons</span> <span m="1081670">to</span>
  <span m="1081760">be</span> <span m="1081850">pessimistic</span> <span m="1082640">but</span>
  <span m="1083170">one</span> <span m="1083440">reason</span> <span m="1083650">to</span>
  <span m="1083710">be</span> <span m="1083800">very</span> <span m="1084040">optimistic</span>
  <span m="1084730">is</span> <span m="1084880">the</span> <span m="1085000">one</span>
  <span m="1085210">area</span> <span m="1085990">where</span> <span m="1086190">AI</span>
  <span m="1086650">is not--</span> <span m="1086800">not</span> <span m="1087280">the</span>
  <span m="1087340">one</span> <span m="1087460">area,</span> <span m="1087610">but
  maybe</span> <span m="1087790">one</span> <span m="1087970">of</span> <span m="1088060">two</span>
  <span m="1088240">or</span> <span m="1088300">three</span> <span m="1088510">areas</span>
  <span m="1088810">where</span> <span m="1088910">AI</span> <span m="1089130">is</span>
  <span m="1089230">not</span> <span m="1089380">total</span> <span m="1089620">hype</span>
  <span m="1090280">is</span> <span m="1090520">vision.</span></p><p><span m="1091990">Vision</span>
  <span m="1092380">really</span> <span m="1092800">started</span> <span m="1093190">working</span>
  <span m="1093550">well</span> <span m="1094210">as,</span> <span m="1094390">I</span>
  <span m="1094420">don't</span> <span m="1094540">if</span> <span m="1094630">you've</span>
  <span m="1094690">covered</span> <span m="1094900">in</span> <span m="1094960">this</span>
  <span m="1095080">class</span> <span m="1095460">but with</span> <span m="1095740">deep</span>
  <span m="1095920">convolutional</span> <span m="1096430">neural</span> <span m="1096700">nets</span>
  <span m="1097480">in</span> <span m="1097630">2012.</span> <span m="1098410">And</span>
  <span m="1098560">then</span> <span m="1099220">all</span> <span m="1099370">the</span>
  <span m="1099490">groups</span> <span m="1099850">sort</span> <span m="1100060">of</span>
  <span m="1100120">just</span> <span m="1100300">kept</span> <span m="1100570">getting</span>
  <span m="1100990">incrementally</span> <span m="1101650">better</span> <span m="1102040">year</span>
  <span m="1102280">over</span> <span m="1102520">year.</span> <span m="1103480">And</span>
  <span m="1103600">now</span> <span m="1103810">this</span> <span m="1103990">is</span>
  <span m="1104260">an</span> <span m="1104350">old</span> <span m="1104560">graph</span>
  <span m="1104890">from</span> <span m="1105040">2015,</span> <span m="1105640">but</span>
  <span m="1105760">there's</span> <span m="1105970">been</span> <span m="1106120">a</span>
  <span m="1106450">huge</span> <span m="1106900">development</span> <span m="1107320">of</span>
  <span m="1107410">methods</span> <span m="1107860">even</span> <span m="1108100">since</span>
  <span m="1108280">2015,</span> <span m="1109750">where</span> <span m="1110470">now</span>
  <span m="1110740">I</span> <span m="1110830">think</span> <span m="1110980">we</span>
  <span m="1111070">really</span> <span m="1111250">understand</span> <span m="1111580">the</span>
  <span m="1111640">strengths</span> <span m="1112000">and</span> <span m="1112090">the</span>
  <span m="1112180">weaknesses</span> <span m="1112660">of</span> <span m="1112750">these</span>
  <span m="1112900">approaches.</span></p><p><span m="1113800">And</span> <span m="1113920">pathology</span>
  <span m="1114520">sort</span> <span m="1114730">of</span> <span m="1114910">has</span>
  <span m="1115180">a</span> <span m="1115240">lot</span> <span m="1115540">of</span>
  <span m="1115630">the</span> <span m="1115750">strengths,</span> <span m="1116270">which</span>
  <span m="1116320">is</span> <span m="1116410">super</span> <span m="1116830">well-defined,</span>
  <span m="1118090">very</span> <span m="1118630">focused</span> <span m="1119500">questions.</span>
  <span m="1120340">And</span> <span m="1120550">I</span> <span m="1120610">think</span>
  <span m="1120760">there's</span> <span m="1121060">lots</span> <span m="1121300">of</span>
  <span m="1121360">failures</span> <span m="1122470">whenever</span> <span m="1122740">you</span>
  <span m="1122800">try to do</span> <span m="1122960">anything</span> <span m="1123160">more</span>
  <span m="1123310">general.</span> <span m="1123910">But</span> <span m="1124090">for</span>
  <span m="1124240">the</span> <span m="1124330">types</span> <span m="1124660">of</span>
  <span m="1124750">tasks</span> <span m="1125170">where you</span> <span m="1125330">know</span>
  <span m="1125550">exactly what</span> <span m="1125750">you're</span> <span m="1125860">looking</span>
  <span m="1126130">for</span> <span m="1126790">and</span> <span m="1126910">you</span>
  <span m="1127420">can</span> <span m="1127570">generate</span> <span m="1127840">the</span>
  <span m="1127930">training</span> <span m="1128200">data,</span> <span m="1129360">these</span>
  <span m="1129520">systems</span> <span m="1129850">can</span> <span m="1130000">work</span>
  <span m="1130180">really</span> <span m="1130360">well.</span></p><p><span m="1131660">So</span>
  <span m="1131710">that's</span> <span m="1132730">a</span> <span m="1132820">lot</span>
  <span m="1133030">of</span> <span m="1133120">what</span> <span m="1133240">we're</span>
  <span m="1133570">focused</span> <span m="1133900">on</span> <span m="1133990">at</span>
  <span m="1134275">PathAI</span> <span m="1134560">is</span> <span m="1134650">how</span>
  <span m="1134740">do</span> <span m="1134830">we</span> <span m="1135200">extract</span>
  <span m="1135380">the</span> <span m="1135530">most</span> <span m="1135830">information</span>
  <span m="1136460">out</span> <span m="1136640">of</span> <span m="1136730">pathology</span>
  <span m="1137210">images</span> <span m="1137570">really</span> <span m="1137750">doing</span>
  <span m="1137900">two</span> <span m="1138080">things.</span> <span m="1138480">One</span>
  <span m="1138650">is</span> <span m="1138800">understanding</span> <span m="1139220">what's</span>
  <span m="1139400">inside</span> <span m="1139700">the</span> <span m="1139820">images</span>
  <span m="1140750">and</span> <span m="1141600">the</span> <span m="1141620">second</span>
  <span m="1141920">is</span> <span m="1142010">using</span> <span m="1142220">deep</span>
  <span m="1142430">learning</span> <span m="1142820">to</span> <span m="1142940">sort</span>
  <span m="1143120">of</span> <span m="1143210">directly</span> <span m="1143720">try</span>
  <span m="1143960">to</span> <span m="1144080">infer</span> <span m="1144530">patient</span>
  <span m="1144950">level</span> <span m="1145670">phenotypes</span> <span m="1146240">and</span>
  <span m="1146330">outcomes</span> <span m="1146780">directly</span> <span m="1147110">from</span>
  <span m="1147230">the</span> <span m="1147320">images.</span></p><p><span m="1148750">And</span>
  <span m="1148880">we</span> <span m="1149030">use</span> <span m="1149240">both</span>
  <span m="1149990">traditional</span> <span m="1150500">machine</span> <span m="1150800">learning</span>
  <span m="1151040">models</span> <span m="1151460">for</span> <span m="1151610">certain</span>
  <span m="1151880">things,</span> <span m="1152270">like</span> <span m="1152660">particularly</span>
  <span m="1153200">making</span> <span m="1153440">inference</span> <span m="1153890">at</span>
  <span m="1153950">the</span> <span m="1154010">patient</span> <span m="1154310">level,</span>
  <span m="1154610">where</span> <span m="1154880">n</span> <span m="1155060">is</span>
  <span m="1155210">often</span> <span m="1155420">very</span> <span m="1155600">small.</span>
  <span m="1156290">But</span> <span m="1156500">anything</span> <span m="1156830">that's</span>
  <span m="1157160">directly</span> <span m="1157820">operating</span> <span m="1158210">on</span>
  <span m="1158300">the</span> <span m="1158420">image</span> <span m="1158770">is</span>
  <span m="1158930">almost</span> <span m="1159380">some</span> <span m="1159650">variant</span>
  <span m="1160730">always</span> <span m="1161450">of</span> <span m="1161600">deep</span>
  <span m="1161780">convolutional</span> <span m="1162290">neural</span> <span m="1162530">nets,</span>
  <span m="1162860">which</span> <span m="1163010">really</span> <span m="1163280">are</span>
  <span m="1163730">the</span> <span m="1163820">state</span> <span m="1164090">of</span>
  <span m="1164180">the</span> <span m="1164300">art</span> <span m="1164600">for</span>
  <span m="1165620">image</span> <span m="1165860">processing.</span></p><p><span
  m="1167930">And</span> <span m="1168530">we</span> <span m="1168710">sort</span>
  <span m="1168950">of,</span> <span m="1169370">a</span> <span m="1169430">lot</span>
  <span m="1169670">of</span> <span m="1169760">what</span> <span m="1169880">we</span>
  <span m="1170000">think</span> <span m="1170180">about</span> <span m="1170600">at</span>
  <span m="1170660">PathAI,</span> <span m="1171010">and I</span> <span m="1171170">think</span>
  <span m="1171290">what's</span> <span m="1171440">really</span> <span m="1171620">important</span>
  <span m="1172640">in</span> <span m="1172790">this</span> <span m="1173030">area</span>
  <span m="1173390">of</span> <span m="1173730">ML</span> <span m="1174020">for</span>
  <span m="1174140">medicine</span> <span m="1174530">is</span> <span m="1174650">generating</span>
  <span m="1175100">the</span> <span m="1175160">right</span> <span m="1175280">data</span>
  <span m="1175560">set</span> <span m="1176360">and</span> <span m="1176480">then</span>
  <span m="1176630">using</span> <span m="1177350">things</span> <span m="1177620">like</span>
  <span m="1177770">deep</span> <span m="1177980">learning</span> <span m="1178250">to</span>
  <span m="1178340">optimize</span> <span m="1178950">all</span> <span m="1179190">of</span>
  <span m="1179240">the</span> <span m="1179330">features</span> <span m="1179750">in
  a</span> <span m="1179900">data-driven</span> <span m="1180460">away,</span> <span
  m="1181130">and</span> <span m="1181250">then</span> <span m="1181400">really</span>
  <span m="1181610">thinking</span> <span m="1181880">about</span> <span m="1182060">how</span>
  <span m="1182150">to</span> <span m="1182240">use</span> <span m="1182600">the</span>
  <span m="1182930">outputs</span> <span m="1183350">of</span> <span m="1183410">these</span>
  <span m="1183560">models</span> <span m="1183890">intelligently</span> <span m="1184970">and</span>
  <span m="1185600">really</span> <span m="1185990">validate</span> <span m="1186500">them</span>
  <span m="1186650">in</span> <span m="1186740">a</span> <span m="1186800">robust</span>
  <span m="1187280">way,</span> <span m="1187520">because</span> <span m="1187760">there's</span>
  <span m="1187940">many</span> <span m="1188270">ways</span> <span m="1188450">to</span>
  <span m="1188510">be</span> <span m="1188600">fooled</span> <span m="1188930">by</span>
  <span m="1189770">artefacts</span> <span m="1190600">and</span> <span m="1190730">other</span>
  <span m="1190940">things.</span></p><p><span m="1192570">So</span> <span m="1192690">just</span>
  <span m="1192820">some</span> <span m="1193010">of</span> <span m="1193070">the--</span>
  <span m="1194150">not</span> <span m="1194360">to</span> <span m="1194480">belabor</span>
  <span m="1194930">the</span> <span m="1195020">points,</span> <span m="1195380">but</span>
  <span m="1195500">why</span> <span m="1195710">these</span> <span m="1195920">approaches</span>
  <span m="1196370">are</span> <span m="1197280">really</span> <span m="1197510">valuable</span>
  <span m="1197840">in</span> <span m="1197900">this</span> <span m="1198020">application</span>
  <span m="1198590">is</span> <span m="1198710">it</span> <span m="1198800">allows</span>
  <span m="1199070">you</span> <span m="1199130">to</span> <span m="1199220">exhaustively</span>
  <span m="1199910">analyze</span> <span m="1200300">slides.</span> <span m="1200870">So</span>
  <span m="1201630">a</span> <span m="1201720">pathologist,</span> <span m="1202350">the</span>
  <span m="1202430">reason</span> <span m="1202650">they're</span> <span m="1202700">making</span>
  <span m="1202850">so</span> <span m="1202940">many</span> <span m="1203090">errors</span>
  <span m="1203450">is</span> <span m="1203580">they're</span> <span m="1203690">just</span>
  <span m="1203870">kind</span> <span m="1204020">of</span> <span m="1204110">overwhelmed.</span>
  <span m="1205080">I</span> <span m="1205180">mean,</span> <span m="1205280">there's
  two</span> <span m="1205430">reasons.</span></p><p><span m="1205860">One</span>
  <span m="1206030">is</span> <span m="1206330">humans</span> <span m="1206720">aren't</span>
  <span m="1206870">good</span> <span m="1207050">at</span> <span m="1207140">interpreting</span>
  <span m="1208040">visual</span> <span m="1208370">patterns.</span> <span m="1208880">Actually,
  I</span> <span m="1209070">think</span> <span m="1209190">that's</span> <span m="1209390">not</span>
  <span m="1209630">the</span> <span m="1209780">real</span> <span m="1210110">reason,</span>
  <span m="1210530">because</span> <span m="1210710">humans</span> <span m="1211010">are</span>
  <span m="1211220">pretty</span> <span m="1211490">darn</span> <span m="1211730">good</span>
  <span m="1211880">at</span> <span m="1211970">that.</span> <span m="1212730">And</span>
  <span m="1212780">there</span> <span m="1212930">are</span> <span m="1213140">difficult</span>
  <span m="1213530">things</span> <span m="1213740">where we</span> <span m="1213890">can</span>
  <span m="1213980">disagree,</span> <span m="1214520">but</span> <span m="1215000">when</span>
  <span m="1215150">people</span> <span m="1215420">focus</span> <span m="1215930">on</span>
  <span m="1216050">small</span> <span m="1216500">images,</span> <span m="1217460">frequently</span>
  <span m="1217910">they</span> <span m="1218090">agree.</span> <span m="1218750">But</span>
  <span m="1218930">these</span> <span m="1219110">images</span> <span m="1219410">are</span>
  <span m="1219530">enormous,</span> <span m="1220310">and</span> <span m="1221330">humans</span>
  <span m="1221660">just</span> <span m="1221780">don't</span> <span m="1221900">have</span>
  <span m="1221990">enough</span> <span m="1222140">time</span> <span m="1222470">to</span>
  <span m="1222590">study</span> <span m="1222980">carefully</span> <span m="1223670">every</span>
  <span m="1223970">cell</span> <span m="1224270">on</span> <span m="1224360">every</span>
  <span m="1224540">slide.</span> <span m="1225170">Whereas,</span> <span m="1225560">the</span>
  <span m="1225740">computer,</span> <span m="1226715">in</span> <span m="1227000">a</span>
  <span m="1227030">real</span> <span m="1227240">way,</span> <span m="1227450">can</span>
  <span m="1227600">be</span> <span m="1227720">forced</span> <span m="1228110">to</span>
  <span m="1228260">exhaustively</span> <span m="1229460">analyze</span> <span m="1230000">every</span>
  <span m="1230330">cell</span> <span m="1230810">on</span> <span m="1230960">every</span>
  <span m="1231170">slide,</span> <span m="1231950">and</span> <span m="1232070">that's</span>
  <span m="1232250">just</span> <span m="1232430">a</span> <span m="1232460">huge</span>
  <span m="1232880">difference.</span></p><p><span m="1233940">It's</span> <span m="1234050">quantitative.</span>
  <span m="1234950">I</span> <span m="1235010">mean,</span> <span m="1235130">this</span>
  <span m="1235250">is</span> <span m="1235340">one</span> <span m="1235520">thing</span>
  <span m="1235690">the</span> <span m="1235760">computer</span> <span m="1236060">is</span>
  <span m="1236110">definitely</span> <span m="1236420">better</span> <span m="1236630">at.</span>
  <span m="1236810">It</span> <span m="1237080">can</span> <span m="1237230">compute</span>
  <span m="1237770">huge</span> <span m="1238130">numerators,</span> <span m="1238640">huge</span>
  <span m="1238850">denominators,</span> <span m="1239150">and</span> <span m="1239450">exactly</span>
  <span m="1239900">compute</span> <span m="1240200">proportions.</span> <span m="1241190">Whereas,</span>
  <span m="1241430">when</span> <span m="1241550">a</span> <span m="1241610">person</span>
  <span m="1241780">is</span> <span m="1241940">looking</span> <span m="1242150">at</span>
  <span m="1242210">a</span> <span m="1242240">slide,</span> <span m="1242510">they're</span>
  <span m="1242600">really</span> <span m="1242750">just</span> <span m="1242930">eyeballing</span>
  <span m="1243470">some</span> <span m="1243620">percentage</span> <span m="1244220">based</span>
  <span m="1244460">on</span> <span m="1244550">a</span> <span m="1244610">very</span>
  <span m="1244880">small</span> <span m="1245090">amount</span> <span m="1245240">of</span>
  <span m="1245330">data.</span></p><p><span m="1246050">It's</span> <span m="1246200">super</span>
  <span m="1246500">efficient.</span> <span m="1247110">So</span> <span m="1248120">you</span>
  <span m="1248270">can</span> <span m="1248570">analyze--</span> <span m="1249590">this</span>
  <span m="1250110">whole</span> <span m="1250340">process</span> <span m="1250760">is</span>
  <span m="1250880">massively</span> <span m="1251780">paralyzable,</span> <span m="1252710">so</span>
  <span m="1252830">you</span> <span m="1252950">can</span> <span m="1253460">almost</span>
  <span m="1253760">do</span> <span m="1253910">a</span> <span m="1253970">slide</span>
  <span m="1254300">as</span> <span m="1254420">fast</span> <span m="1254690">as</span>
  <span m="1254810">you</span> <span m="1254900">want</span> <span m="1255110">based</span>
  <span m="1255320">on</span> <span m="1255410">how</span> <span m="1255500">much</span>
  <span m="1256220">you're</span> <span m="1256370">willing</span> <span m="1256610">to</span>
  <span m="1256730">spend</span> <span m="1257090">on</span> <span m="1257240">it.</span></p><p><span
  m="1258140">And</span> <span m="1258560">it</span> <span m="1258650">allows</span>
  <span m="1258950">you</span> <span m="1259010">not</span> <span m="1259160">only</span>
  <span m="1259400">do</span> <span m="1259520">all</span> <span m="1259640">of</span>
  <span m="1259730">of these,</span> <span m="1259940">sort</span> <span m="1260180">of,</span>
  <span m="1260270">automation</span> <span m="1260840">tasks</span> <span m="1261320">exhaustively,</span>
  <span m="1261890">quantitatively,</span> <span m="1262400">and</span> <span m="1262490">efficiently</span>
  <span m="1262980">but</span> <span m="1263000">also</span> <span m="1263270">discover</span>
  <span m="1263840">a</span> <span m="1263870">lot</span> <span m="1264050">of</span>
  <span m="1264110">new</span> <span m="1264230">insights</span> <span m="1264560">from</span>
  <span m="1264680">the</span> <span m="1264770">data,</span> <span m="1265560">which</span>
  <span m="1265610">I</span> <span m="1265640">think</span> <span m="1265760">we</span>
  <span m="1265850">did</span> <span m="1265970">in</span> <span m="1266030">a</span>
  <span m="1266090">very</span> <span m="1267080">early</span> <span m="1267440">way,</span>
  <span m="1267680">back</span> <span m="1268040">eight</span> <span m="1268190">years</span>
  <span m="1268430">ago,</span> <span m="1268640">when we sort of</span> <span m="1268890">had</span>
  <span m="1269020">human-extracted</span> <span m="1269780">features</span> <span
  m="1270620">correlate</span> <span m="1271010">those</span> <span m="1271160">with</span>
  <span m="1271260">outcome.</span> <span m="1271640">But</span> <span m="1271730">now</span>
  <span m="1271910">you</span> <span m="1272000">can</span> <span m="1272150">really</span>
  <span m="1272660">supervise</span> <span m="1273260">the</span> <span m="1273320">whole</span>
  <span m="1273470">process</span> <span m="1273890">with</span> <span m="1274040">machine</span>
  <span m="1274310">learning</span> <span m="1274970">of</span> <span m="1275120">how</span>
  <span m="1275270">you</span> <span m="1275390">go</span> <span m="1275600">from</span>
  <span m="1275960">the</span> <span m="1276050">components</span> <span m="1276530">of</span>
  <span m="1276620">an</span> <span m="1276710">image</span> <span m="1277100">to</span>
  <span m="1277490">patient</span> <span m="1277850">outcomes</span> <span m="1279200">and</span>
  <span m="1279380">learn</span> <span m="1279680">new</span> <span m="1279800">biology</span>
  <span m="1281030">that</span> <span m="1281150">you</span> <span m="1281210">didn't</span>
  <span m="1281450">know</span> <span m="1281600">going</span> <span m="1281870">in.</span></p><p><span
  m="1284330">And</span> <span m="1284900">everyone's</span> <span m="1285200">always</span>
  <span m="1285440">like,</span> <span m="1285720">well,</span> <span m="1285800">are</span>
  <span m="1285890">you</span> <span m="1285950">just</span> <span m="1286070">going</span>
  <span m="1286190">to</span> <span m="1286250">replace</span> <span m="1286610">pathologists?</span>
  <span m="1287420">And</span> <span m="1287630">I</span> <span m="1287690">really</span>
  <span m="1287900">don't</span> <span m="1288140">think</span> <span m="1288350">this</span>
  <span m="1288590">is,</span> <span m="1289650">in</span> <span m="1289790">any</span>
  <span m="1290010">way,</span> <span m="1290210">the</span> <span m="1290330">future.</span>
  <span m="1291080">In</span> <span m="1291170">almost</span> <span m="1291440">every</span>
  <span m="1291830">field</span> <span m="1292350">that's</span> <span m="1292730">sort</span>
  <span m="1292880">of</span> <span m="1292940">like</span> <span m="1294520">where</span>
  <span m="1294710">automation</span> <span m="1295850">is</span> <span m="1296060">becoming</span>
  <span m="1296360">very</span> <span m="1296510">common,</span> <span m="1297800">the</span>
  <span m="1297950">demand</span> <span m="1298550">for</span> <span m="1299060">people</span>
  <span m="1299390">who</span> <span m="1299510">are</span> <span m="1299600">experts</span>
  <span m="1300020">in</span> <span m="1300110">that</span> <span m="1300230">area</span>
  <span m="1300590">is</span> <span m="1300800">increasing.</span></p><p><span m="1301440">And</span>
  <span m="1301550">like</span> <span m="1301760">airplane</span> <span m="1302090">pilots</span>
  <span m="1302480">is</span> <span m="1302600">one</span> <span m="1302720">I</span>
  <span m="1302750">was</span> <span m="1302870">just</span> <span m="1303470">learning</span>
  <span m="1303830">about</span> <span m="1304010">today.</span> <span m="1305090">They</span>
  <span m="1305210">just</span> <span m="1305390">do</span> <span m="1305600">a</span>
  <span m="1305660">completely</span> <span m="1306080">different</span> <span m="1306350">thing</span>
  <span m="1306500">than</span> <span m="1306620">they</span> <span m="1306770">did</span>
  <span m="1307220">20</span> <span m="1307550">years</span> <span m="1307790">ago,</span>
  <span m="1307970">and</span> <span m="1308050">now</span> <span m="1308210">it's</span>
  <span m="1308330">all</span> <span m="1308480">about</span> <span m="1308870">mission</span>
  <span m="1309770">control</span> <span m="1310370">of</span> <span m="1310520">this</span>
  <span m="1310820">big</span> <span m="1311000">system</span> <span m="1311450">and</span>
  <span m="1311960">understanding</span> <span m="1312500">all</span> <span m="1312650">the</span>
  <span m="1312740">flight</span> <span m="1313010">management</span> <span m="1313370">systems</span>
  <span m="1313800">and understanding</span> <span m="1314120">all</span> <span m="1314180">the</span>
  <span m="1314270">data</span> <span m="1314510">they're</span> <span m="1314630">getting.</span>
  <span m="1315420">And</span> <span m="1315520">I</span> <span m="1315620">think
  the</span> <span m="1315710">job</span> <span m="1316040">has</span> <span m="1316190">not</span>
  <span m="1316370">gotten</span> <span m="1316730">necessarily</span> <span m="1317300">simpler,</span>
  <span m="1317900">but</span> <span m="1318050">they're</span> <span m="1318140">much</span>
  <span m="1318350">more</span> <span m="1318440">effective,</span> <span m="1318950">and</span>
  <span m="1319040">they're</span> <span m="1319130">doing</span> <span m="1319340">much</span>
  <span m="1319580">different</span> <span m="1319820">types</span> <span m="1320000">of</span>
  <span m="1320120">work.</span></p><p><span m="1320790">And</span> <span m="1320900">I</span>
  <span m="1320940">do</span> <span m="1321060">think</span> <span m="1321320">the</span>
  <span m="1321410">pathologist</span> <span m="1321830">is</span> <span m="1321920">going</span>
  <span m="1322040">to</span> <span m="1322100">move</span> <span m="1322310">from</span>
  <span m="1322460">sort</span> <span m="1322610">of</span> <span m="1322670">staring</span>
  <span m="1323180">into</span> <span m="1323540">a</span> <span m="1323570">microscope</span>
  <span m="1324170">with</span> <span m="1324350">a</span> <span m="1324500">literally</span>
  <span m="1324980">very</span> <span m="1325220">myopic</span> <span m="1325730">focus</span>
  <span m="1326150">on</span> <span m="1326300">very</span> <span m="1326450">small</span>
  <span m="1326690">things</span> <span m="1327020">to</span> <span m="1328070">being</span>
  <span m="1328310">more</span> <span m="1328490">of</span> <span m="1328580">a</span>
  <span m="1328610">consultant</span> <span m="1329180">with</span> <span m="1329300">physicians,</span>
  <span m="1329900">integrating</span> <span m="1330260">lots</span> <span m="1330410">of</span>
  <span m="1330470">different</span> <span m="1330680">types</span> <span m="1330860">of</span>
  <span m="1330920">data,</span> <span m="1333050">things</span> <span m="1333260">that</span>
  <span m="1333380">AI</span> <span m="1333650">is</span> <span m="1333770">really</span>
  <span m="1333950">bad</span> <span m="1334280">at,</span> <span m="1334460">a</span>
  <span m="1334490">lot</span> <span m="1334640">of</span> <span m="1334730">reasoning</span>
  <span m="1335210">about</span> <span m="1335420">specific</span> <span m="1336140">instances,</span>
  <span m="1338120">and</span> <span m="1338300">then</span> <span m="1338690">providing</span>
  <span m="1339140">that</span> <span m="1339260">guidance</span> <span m="1339650">to</span>
  <span m="1339770">physicians.</span> <span m="1340200">So</span> <span m="1340270">I</span>
  <span m="1340310">think</span> <span m="1340460">the</span> <span m="1340520">job</span>
  <span m="1340820">will</span> <span m="1340910">look</span> <span m="1341090">a</span>
  <span m="1341120">lot</span> <span m="1341300">different,</span> <span m="1341960">but</span>
  <span m="1342200">we</span> <span m="1342620">never</span> <span m="1342830">really</span>
  <span m="1342980">needed</span> <span m="1343220">more</span> <span m="1343640">diagnosticians</span>
  <span m="1344570">in</span> <span m="1344690">the</span> <span m="1344780">future</span>
  <span m="1345485">than</span> <span m="1345800">in</span> <span m="1345890">the</span>
  <span m="1345950">past.</span></p><p><span m="1348420">So</span> <span m="1348590">one</span>
  <span m="1348800">example,</span> <span m="1349280">I</span> <span m="1349310">think</span>
  <span m="1349460">we</span> <span m="1349550">sent</span> <span m="1349730">out</span>
  <span m="1350300">a</span> <span m="1350390">reading</span> <span m="1350690">about</span>
  <span m="1350930">this</span> <span m="1351140">was</span> <span m="1351320">this</span>
  <span m="1351890">concept</span> <span m="1352490">of</span> <span m="1352610">breast</span>
  <span m="1352880">cancer</span> <span m="1353210">metastasis</span> <span m="1353900">is</span>
  <span m="1354020">a</span> <span m="1354080">good</span> <span m="1354260">use</span>
  <span m="1354650">case</span> <span m="1355040">of</span> <span m="1356000">machine</span>
  <span m="1356330">learning.</span> <span m="1356780">And</span> <span m="1356930">this</span>
  <span m="1357050">is</span> <span m="1357170">just</span> <span m="1357440">a</span>
  <span m="1357710">patient</span> <span m="1358100">example.</span> <span m="1358520">So</span>
  <span m="1358880">a</span> <span m="1358940">primary</span> <span m="1360020">mass</span>
  <span m="1360470">is</span> <span m="1360650">discovered.</span></p><p><span m="1361370">So</span>
  <span m="1362780">one</span> <span m="1362990">of</span> <span m="1363050">the</span>
  <span m="1363140">big</span> <span m="1363290">determinants</span> <span m="1363770">of</span>
  <span m="1363830">the</span> <span m="1363890">prognosis</span> <span m="1364460">from</span>
  <span m="1364580">a</span> <span m="1364640">primary</span> <span m="1364970">tumor</span>
  <span m="1365240">is has</span> <span m="1365510">it</span> <span m="1365570">spread</span>
  <span m="1365810">to</span> <span m="1365870">the</span> <span m="1365960">lymph</span>
  <span m="1366140">nodes?</span> <span m="1367160">Because</span> <span m="1367400">that's</span>
  <span m="1367550">one</span> <span m="1367640">of</span> <span m="1367700">the</span>
  <span m="1367790">first</span> <span m="1368240">areas</span> <span m="1368630">that</span>
  <span m="1368750">tumors</span> <span m="1369140">metastasize</span> <span m="1369980">to.</span>
  <span m="1371240">And</span> <span m="1371540">the</span> <span m="1371660">way</span>
  <span m="1371870">to</span> <span m="1371990">diagnose</span> <span m="1372440">whether</span>
  <span m="1373010">tumors</span> <span m="1373340">have</span> <span m="1373430">metastasized</span>
  <span m="1373695">to</span> <span m="1373960">lymph</span> <span m="1374180">nodes</span>
  <span m="1374390">is</span> <span m="1374480">to</span> <span m="1374570">take</span>
  <span m="1374750">a</span> <span m="1374810">biopsy</span> <span m="1375950">and</span>
  <span m="1376040">then</span> <span m="1376130">evaluate</span> <span m="1376610">those</span>
  <span m="1376880">for</span> <span m="1377120">the</span> <span m="1377240">presence</span>
  <span m="1377690">of</span> <span m="1377780">cancer</span> <span m="1378200">where</span>
  <span m="1378350">it</span> <span m="1378410">shouldn't</span> <span m="1378680">be.</span></p><p><span
  m="1380960">And</span> <span m="1381080">this</span> <span m="1381260">is</span>
  <span m="1381380">a</span> <span m="1381440">task</span> <span m="1381890">that's</span>
  <span m="1382230">very</span> <span m="1382610">quantitative</span> <span m="1383360">and</span>
  <span m="1383450">very</span> <span m="1383630">tedious.</span> <span m="1384980">So</span>
  <span m="1386300">the</span> <span m="1386720">International</span> <span m="1387260">Symposium</span>
  <span m="1387770">on</span> <span m="1387860">Biomedical</span> <span m="1388340">Imaging</span>
  <span m="1388700">organized</span> <span m="1389060">this</span> <span m="1389180">challenge</span>
  <span m="1389600">called</span> <span m="1389780">the</span> <span m="1389840">Chameleon</span>
  <span m="1390380">16</span> <span m="1390860">Challenge,</span> <span m="1392090">where</span>
  <span m="1392240">they</span> <span m="1392360">put</span> <span m="1392510">together</span>
  <span m="1393020">almost</span> <span m="1393410">300</span> <span m="1393980">training</span>
  <span m="1394370">slides</span> <span m="1394790">and about</span> <span m="1394910">130</span>
  <span m="1396020">test</span> <span m="1396290">slides.</span> <span m="1396740">And</span>
  <span m="1396860">they</span> <span m="1397280">asked</span> <span m="1397550">a</span>
  <span m="1397580">bunch</span> <span m="1397790">of</span> <span m="1397880">teams</span>
  <span m="1398210">to</span> <span m="1398330">build</span> <span m="1399110">machine</span>
  <span m="1399470">learning</span> <span m="1399740">based</span> <span m="1399950">systems</span>
  <span m="1401750">to</span> <span m="1401990">automate</span> <span m="1402890">the</span>
  <span m="1403010">evaluation</span> <span m="1403580">of</span> <span m="1403640">the</span>
  <span m="1403700">test</span> <span m="1403940">slides,</span> <span m="1404270">both</span>
  <span m="1404510">to</span> <span m="1405170">diagnose</span> <span m="1405740">whether</span>
  <span m="1405950">the</span> <span m="1406010">slide</span> <span m="1406300">contained</span>
  <span m="1406580">cancer</span> <span m="1406940">or</span> <span m="1407000">not,</span>
  <span m="1407270">as</span> <span m="1407420">well</span> <span m="1407570">as</span>
  <span m="1407660">to</span> <span m="1407720">actually</span> <span m="1407930">identify</span>
  <span m="1408350">where</span> <span m="1408560">in</span> <span m="1408620">the</span>
  <span m="1408710">slides</span> <span m="1409490">the</span> <span m="1409580">cancer</span>
  <span m="1409940">was</span> <span m="1410060">located.</span></p><p><span m="1411560">And</span>
  <span m="1411780">kind</span> <span m="1412100">of</span> <span m="1412150">the</span>
  <span m="1412250">big</span> <span m="1412550">machine</span> <span m="1412970">learning</span>
  <span m="1413570">challenge</span> <span m="1414020">here,</span> <span m="1414170">why</span>
  <span m="1414290">you</span> <span m="1414350">can't</span> <span m="1414560">just</span>
  <span m="1415040">throw</span> <span m="1415460">it</span> <span m="1415580">into</span>
  <span m="1416060">a</span> <span m="1417770">off-the-shelf</span> <span m="1418790">or</span>
  <span m="1419850">on</span> <span m="1420050">the</span> <span m="1420170">web</span>
  <span m="1421010">image</span> <span m="1421280">classification</span> <span m="1421970">tool</span>
  <span m="1422620">is</span> <span m="1423260">the</span> <span m="1423410">images</span>
  <span m="1423770">are</span> <span m="1423860">so</span> <span m="1424100">large</span>
  <span m="1424760">that</span> <span m="1425390">it's</span> <span m="1425510">just</span>
  <span m="1425660">not</span> <span m="1426650">feasible</span> <span m="1427220">to</span>
  <span m="1427340">throw</span> <span m="1427790">the</span> <span m="1427880">whole</span>
  <span m="1428120">image</span> <span m="1430430">into</span> <span m="1431690">any</span>
  <span m="1431930">kind</span> <span m="1432170">of</span> <span m="1432260">neural</span>
  <span m="1432530">net.</span> <span m="1433070">Because</span> <span m="1435180">they</span>
  <span m="1435380">can</span> <span m="1435500">be</span> <span m="1435650">between</span>
  <span m="1435950">20,000</span> <span m="1436400">and 200,000</span> <span m="1437150">pixels</span>
  <span m="1437660">on</span> <span m="1437810">a</span> <span m="1437870">side.</span>
  <span m="1438260">So</span> <span m="1438380">they</span> <span m="1438470">have</span>
  <span m="1439490">millions</span> <span m="1441320">of</span> <span m="1441440">pixels.</span></p><p><span
  m="1443840">And</span> <span m="1444890">for</span> <span m="1445100">that,</span>
  <span m="1445610">we</span> <span m="1445730">do</span> <span m="1445850">this</span>
  <span m="1446000">process</span> <span m="1446420">where</span> <span m="1446540">we</span>
  <span m="1446660">start</span> <span m="1446960">with</span> <span m="1447110">a</span>
  <span m="1447170">labeled</span> <span m="1447760">data</span> <span m="1448010">set,</span>
  <span m="1448280">where</span> <span m="1448520">there</span> <span m="1448700">are</span>
  <span m="1448720">these</span> <span m="1448910">very</span> <span m="1449120">large</span>
  <span m="1449660">regions</span> <span m="1450290">labeled</span> <span m="1450710">either</span>
  <span m="1450920">as</span> <span m="1451100">normal</span> <span m="1452060">or</span>
  <span m="1452180">tumor.</span> <span m="1452960">And</span> <span m="1453050">then</span>
  <span m="1453170">we</span> <span m="1453290">build</span> <span m="1453710">procedures,</span>
  <span m="1454400">which</span> <span m="1454550">is</span> <span m="1454640">actually</span>
  <span m="1454970">a</span> <span m="1455060">key</span> <span m="1455330">component</span>
  <span m="1455930">of</span> <span m="1456020">getting</span> <span m="1456230">machine</span>
  <span m="1456470">learning</span> <span m="1456680">to</span> <span m="1456770">work</span>
  <span m="1456950">well,</span> <span m="1457460">of</span> <span m="1457670">sampling</span>
  <span m="1458240">patches</span> <span m="1458780">of</span> <span m="1458870">images</span>
  <span m="1459380">and</span> <span m="1459530">putting</span> <span m="1459890">those</span>
  <span m="1460040">patches</span> <span m="1460550">into</span> <span m="1461330">the</span>
  <span m="1461450">model.</span></p><p><span m="1462110">And</span> <span m="1462230">this</span>
  <span m="1462400">sampling</span> <span m="1462890">procedure</span> <span m="1463250">is</span>
  <span m="1463400">actually</span> <span m="1463760">incredibly</span> <span m="1464690">important</span>
  <span m="1465260">for</span> <span m="1466100">controlling</span> <span m="1466820">the</span>
  <span m="1466910">behavior</span> <span m="1467870">of</span> <span m="1468080">the</span>
  <span m="1468200">system,</span> <span m="1468710">because</span> <span m="1468890">you</span>
  <span m="1468980">could</span> <span m="1469160">sample</span> <span m="1469550">in</span>
  <span m="1469640">all</span> <span m="1469880">different</span> <span m="1470180">ways.</span>
  <span m="1470510">You're</span> <span m="1470600">never</span> <span m="1470780">going</span>
  <span m="1470850">to</span> <span m="1470940">sample</span> <span m="1471230">exhaustively</span>
  <span m="1471830">just</span> <span m="1471980">because</span> <span m="1472370">there's</span>
  <span m="1472580">far</span> <span m="1472790">too</span> <span m="1472970">many</span>
  <span m="1473660">possible</span> <span m="1474230">patches.</span> <span m="1475160">So</span>
  <span m="1475340">thinking</span> <span m="1475730">about</span> <span m="1476120">the</span>
  <span m="1476270">right</span> <span m="1476540">examples</span> <span m="1477110">to</span>
  <span m="1477200">show</span> <span m="1477410">the</span> <span m="1477500">system</span>
  <span m="1477920">has</span> <span m="1478130">an</span> <span m="1478220">enormous</span>
  <span m="1478790">effect</span> <span m="1479660">on</span> <span m="1479870">both</span>
  <span m="1480290">the</span> <span m="1480410">performance</span> <span m="1480950">and</span>
  <span m="1481070">the</span> <span m="1481160">generalizability</span> <span m="1482910">of
  the</span> <span m="1483080">systems</span> <span m="1483410">you're</span> <span
  m="1483500">building.</span> <span m="1483800">And</span> <span m="1483890">some</span>
  <span m="1484070">of</span> <span m="1484130">the,</span> <span m="1484430">sort</span>
  <span m="1484670">of,</span> <span m="1485150">insights</span> <span m="1485570">we</span>
  <span m="1485690">learned</span> <span m="1485900">was</span> <span m="1485990">how</span>
  <span m="1486170">best</span> <span m="1486905">to</span> <span m="1487340">do</span>
  <span m="1487550">the,</span> <span m="1487650">sort</span> <span m="1487820">of,</span>
  <span m="1487910">sampling.</span></p><p><span m="1489290">But</span> <span m="1489560">once</span>
  <span m="1489730">you</span> <span m="1489800">have</span> <span m="1489850">these</span>
  <span m="1489950">samples,</span> <span m="1490550">it's</span> <span m="1490730">all</span>
  <span m="1491120">data</span> <span m="1491420">driven--</span> <span m="1491690">sure.</span></p><p><span
  m="1491990">AUDIENCE:</span> <span m="1492060">Can</span> <span m="1492130">you</span>
  <span m="1492200">talk</span> <span m="1492270">more</span> <span m="1492470">about</span>
  <span m="1492710">the</span> <span m="1492800">sampling</span> <span m="1493160">strategy</span>
  <span m="1493420">schemes?</span></p><p><span m="1494740">ANDY BECK:</span> <span
  m="1494925">Yeah,</span> <span m="1495110">so</span> <span m="1495470">from</span>
  <span m="1495770">a</span> <span m="1495830">high</span> <span m="1496040">level,</span>
  <span m="1498200">you</span> <span m="1498350">want</span> <span m="1498500">to</span>
  <span m="1498560">go</span> <span m="1499520">from</span> <span m="1500630">random</span>
  <span m="1501080">sampling,</span> <span m="1501720">which</span> <span m="1501800">is</span>
  <span m="1501890">a</span> <span m="1501950">reasonable</span> <span m="1502340">thing</span>
  <span m="1502520">to</span> <span m="1502640">do,</span> <span m="1504100">to</span>
  <span m="1504320">more</span> <span m="1504470">intelligent</span> <span m="1504950">sampling,</span>
  <span m="1506000">based</span> <span m="1506450">on</span> <span m="1507530">knowing</span>
  <span m="1508010">what</span> <span m="1508160">the</span> <span m="1508250">computer</span>
  <span m="1508970">needs</span> <span m="1509210">to</span> <span m="1509330">learn</span>
  <span m="1509630">more</span> <span m="1509870">about.</span> <span m="1512220">And</span>
  <span m="1512630">one</span> <span m="1512900">thing</span> <span m="1514070">we've</span>
  <span m="1514460">done</span> <span m="1515010">and--</span> <span m="1515750">so</span>
  <span m="1515910">it's</span> <span m="1515990">sort</span> <span m="1516110">of</span>
  <span m="1516200">like</span> <span m="1516350">figuring--</span> <span m="1516900">so</span>
  <span m="1516920">the</span> <span m="1517010">first</span> <span m="1517280">step</span>
  <span m="1517520">is</span> <span m="1517580">sort</span> <span m="1517820">of</span>
  <span m="1517880">simple.</span> <span m="1519050">You</span> <span m="1519380">can</span>
  <span m="1519500">randomly</span> <span m="1519890">sample.</span></p><p><span m="1521210">But</span>
  <span m="1521420">then</span> <span m="1521600">the</span> <span m="1521690">second</span>
  <span m="1521990">part</span> <span m="1522230">is</span> <span m="1522320">a</span>
  <span m="1522380">little</span> <span m="1522560">harder</span> <span m="1522950">to</span>
  <span m="1523070">figure</span> <span m="1523430">out</span> <span m="1523700">what</span>
  <span m="1523940">examples</span> <span m="1524690">do</span> <span m="1524750">you</span>
  <span m="1524810">want</span> <span m="1524960">to</span> <span m="1525050">enrich</span>
  <span m="1525470">your</span> <span m="1525590">training</span> <span m="1525950">set</span>
  <span m="1526190">for</span> <span m="1526970">to</span> <span m="1527360">make</span>
  <span m="1527540">the</span> <span m="1527640">system</span> <span m="1527990">perform</span>
  <span m="1528320">even</span> <span m="1528500">better?</span> <span m="1529710">And</span>
  <span m="1529850">there's</span> <span m="1530030">different</span> <span m="1530300">things</span>
  <span m="1530450">you</span> <span m="1530510">can</span> <span m="1530600">optimize</span>
  <span m="1530855">for,</span> <span m="1531110">for</span> <span m="1531440">that.</span>
  <span m="1531680">So</span> <span m="1531860">it's</span> <span m="1531950">sort</span>
  <span m="1532130">of</span> <span m="1532220">like</span> <span m="1532550">this</span>
  <span m="1532730">whole</span> <span m="1532970">sampling</span> <span m="1533510">actually</span>
  <span m="1533780">being</span> <span m="1533930">part</span> <span m="1534110">of</span>
  <span m="1534170">the</span> <span m="1534230">machine</span> <span m="1534500">learning</span>
  <span m="1534740">procedure</span> <span m="1536330">is</span> <span m="1536570">quite</span>
  <span m="1537110">useful.</span> <span m="1537740">And</span> <span m="1537890">you're</span>
  <span m="1538040">not</span> <span m="1538190">just</span> <span m="1538340">going</span>
  <span m="1538400">to</span> <span m="1538460">be</span> <span m="1538550">sampling</span>
  <span m="1538910">once.</span> <span m="1539300">You</span> <span m="1539420">could</span>
  <span m="1539690">iterate</span> <span m="1540140">on</span> <span m="1540320">this</span>
  <span m="1540530">and</span> <span m="1540620">keep</span> <span m="1541250">providing</span>
  <span m="1541520">different</span> <span m="1541820">types</span> <span m="1542030">of</span>
  <span m="1542090">samples.</span></p><p><span m="1542610">So</span> <span m="1542690">for</span>
  <span m="1542810">example,</span> <span m="1543840">if</span> <span m="1543920">you</span>
  <span m="1544100">learn</span> <span m="1544580">that</span> <span m="1544700">it's</span>
  <span m="1545030">missing</span> <span m="1546050">certain</span> <span m="1546380">types</span>
  <span m="1546770">of</span> <span m="1547190">errors,</span> <span m="1547880">or</span>
  <span m="1548030">it</span> <span m="1548090">hasn't</span> <span m="1548330">seen</span>
  <span m="1548510">enough</span> <span m="1549110">of</span> <span m="1549230">certain--</span>
  <span m="1549920">there's</span> <span m="1550130">many</span> <span m="1550430">ways</span>
  <span m="1550580">of</span> <span m="1550640">getting</span> <span m="1550820">at</span>
  <span m="1550970">it.</span> <span m="1551060">But</span> <span m="1551470">if</span>
  <span m="1551690">you</span> <span m="1551780">know</span> <span m="1551930">it</span>
  <span m="1551990">hasn't</span> <span m="1552260">seen</span> <span m="1552440">enough</span>
  <span m="1552920">types</span> <span m="1553280">of</span> <span m="1553370">examples</span>
  <span m="1554000">in</span> <span m="1554120">your</span> <span m="1554210">training</span>
  <span m="1554480">set,</span> <span m="1555020">you</span> <span m="1555110">can</span>
  <span m="1555260">over-sample</span> <span m="1555860">for</span> <span m="1556010">that.</span></p><p><span
  m="1556640">Or</span> <span m="1556790">if</span> <span m="1556910">you</span> <span
  m="1557000">see</span> <span m="1557330">you have</span> <span m="1557650">a</span>
  <span m="1557720">confusion</span> <span m="1558110">matrix</span> <span m="1558500">and</span>
  <span m="1558590">you</span> <span m="1558650">see</span> <span m="1558860">it's</span>
  <span m="1559130">failing</span> <span m="1559670">on</span> <span m="1559820">certain</span>
  <span m="1560060">types,</span> <span m="1560450">you</span> <span m="1560570">can</span>
  <span m="1560690">try</span> <span m="1560840">to</span> <span m="1560960">figure</span>
  <span m="1561170">out</span> <span m="1561230">why</span> <span m="1561410">is</span>
  <span m="1561500">it</span> <span m="1561590">failing</span> <span m="1561830">on</span>
  <span m="1561920">those</span> <span m="1562190">and</span> <span m="1562640">alter</span>
  <span m="1562940">the</span> <span m="1563060">sampling</span> <span m="1563450">procedure</span>
  <span m="1563870">to</span> <span m="1563990">enrich</span> <span m="1564230">for</span>
  <span m="1564350">that.</span> <span m="1564950">You</span> <span m="1565070">could</span>
  <span m="1565190">even</span> <span m="1565400">provide</span> <span m="1565880">outputs</span>
  <span m="1566480">to</span> <span m="1566780">humans,</span> <span m="1567740">who</span>
  <span m="1567890">can</span> <span m="1568730">point</span> <span m="1569030">you</span>
  <span m="1569120">to</span> <span m="1569210">the</span> <span m="1569660">areas</span>
  <span m="1570590">where</span> <span m="1570710">it's</span> <span m="1570830">making</span>
  <span m="1571070">mistakes.</span> <span m="1571460">Because</span> <span m="1571640">often</span>
  <span m="1571880">you</span> <span m="1571940">don't</span> <span m="1572090">have</span>
  <span m="1572210">exhaustively</span> <span m="1572720">labeled.</span> <span m="1573860">In</span>
  <span m="1573980">this</span> <span m="1574130">case,</span> <span m="1574410">we</span>
  <span m="1574510">actually</span> <span m="1574580">did</span> <span m="1574710">have</span>
  <span m="1574790">exhaustively</span> <span m="1575270">labeled</span> <span m="1576730">slides.</span>
  <span m="1577220">So</span> <span m="1577640">it</span> <span m="1577730">was</span>
  <span m="1577820">somewhat</span> <span m="1578150">easier.</span></p><p><span m="1578990">But</span>
  <span m="1579140">you</span> <span m="1579200">can</span> <span m="1579320">see</span>
  <span m="1579440">there's</span> <span m="1579620">even</span> <span m="1579800">a</span>
  <span m="1579830">lot</span> <span m="1580010">of</span> <span m="1580100">heterogeneity</span>
  <span m="1580820">within</span> <span m="1581240">the</span> <span m="1581330">different</span>
  <span m="1581630">classes.</span> <span m="1582270">So</span> <span m="1583310">you</span>
  <span m="1583460">might</span> <span m="1583940">do</span> <span m="1584180">some</span>
  <span m="1584360">clever</span> <span m="1584690">tricks</span> <span m="1585290">to</span>
  <span m="1585470">figure</span> <span m="1585830">out</span> <span m="1585950">what</span>
  <span m="1586100">are</span> <span m="1586130">the</span> <span m="1586220">types</span>
  <span m="1586670">of</span> <span m="1586910">the</span> <span m="1587030">red</span>
  <span m="1587270">class that</span> <span m="1587740">it's</span> <span m="1587840">getting</span>
  <span m="1588050">wrong,</span> <span m="1588470">and</span> <span m="1588590">how</span>
  <span m="1588710">am</span> <span m="1588800">I</span> <span m="1588830">going</span>
  <span m="1588950">to</span> <span m="1589010">fix</span> <span m="1589310">that</span>
  <span m="1589550">by</span> <span m="1589730">providing</span> <span m="1590130">it</span>
  <span m="1590240">more</span> <span m="1590360">examples?</span></p><p><span m="1591330">So</span>
  <span m="1591380">I</span> <span m="1591470">think,</span> <span m="1591650">sort</span>
  <span m="1591950">of,</span> <span m="1593210">that's</span> <span m="1593570">one</span>
  <span m="1593690">of</span> <span m="1593750">the</span> <span m="1593870">easier</span>
  <span m="1594380">things</span> <span m="1594650">to</span> <span m="1594740">control.</span>
  <span m="1595490">Rather</span> <span m="1595820">than</span> <span m="1595970">trying</span>
  <span m="1596240">to</span> <span m="1596330">tune</span> <span m="1596690">other</span>
  <span m="1597680">parameters</span> <span m="1598310">within</span> <span m="1598520">these</span>
  <span m="1598670">super</span> <span m="1599090">complicated</span> <span m="1599840">networks,</span>
  <span m="1600890">in</span> <span m="1601040">our</span> <span m="1601130">experience,</span>
  <span m="1601730">just</span> <span m="1602180">playing</span> <span m="1602570">with</span>
  <span m="1602720">the</span> <span m="1602810">training,</span> <span m="1604430">the</span>
  <span m="1604550">sampling</span> <span m="1604940">piece</span> <span m="1605150">of</span>
  <span m="1605240">the</span> <span m="1605300">training,</span> <span m="1605960">it</span>
  <span m="1606020">should</span> <span m="1606200">almost</span> <span m="1606500">just</span>
  <span m="1606620">be</span> <span m="1606740">thought</span> <span m="1606920">of</span>
  <span m="1607010">as</span> <span m="1607100">another</span> <span m="1607370">parameter</span>
  <span m="1607800">to</span> <span m="1607850">optimize</span> <span m="1609170">for</span>
  <span m="1609500">when</span> <span m="1609650">you're</span> <span m="1609740">dealing</span>
  <span m="1610040">with</span> <span m="1610160">a</span> <span m="1610190">problem</span>
  <span m="1610670">where</span> <span m="1611210">you</span> <span m="1611300">have</span>
  <span m="1611450">humongous</span> <span m="1612020">slides</span> <span m="1612470">and</span>
  <span m="1612560">you</span> <span m="1612620">can't</span> <span m="1613040">use</span>
  <span m="1613280">all</span> <span m="1613370">the</span> <span m="1613460">training</span>
  <span m="1613760">data.</span></p><p><span m="1616090">AUDIENCE:</span> <span m="1616150">So</span>
  <span m="1616640">decades</span> <span m="1617150">ago,</span> <span m="1617460">I</span>
  <span m="1617900">met</span> <span m="1618140">some</span> <span m="1618380">pathologists</span>
  <span m="1619250">who</span> <span m="1619510">were</span> <span m="1619660">looking</span>
  <span m="1619900">at</span> <span m="1621140">cervical</span> <span m="1621710">cancer</span>
  <span m="1622190">screening.</span> <span m="1623390">And</span> <span m="1623930">they</span>
  <span m="1624530">thought</span> <span m="1625730">that</span> <span m="1626030">you</span>
  <span m="1626150">could</span> <span m="1626360">detect</span> <span m="1626830">a</span>
  <span m="1626910">gradient</span> <span m="1628130">in</span> <span m="1628310">the</span>
  <span m="1628430">degree</span> <span m="1628880">of</span> <span m="1629070">atypia.</span>
  <span m="1631140">And</span> <span m="1631340">so</span> <span m="1632150">not</span>
  <span m="1632450">at</span> <span m="1632510">training</span> <span m="1633020">time</span>
  <span m="1633320">but</span> <span m="1633500">at</span> <span m="1633590">testing</span>
  <span m="1634100">time,</span> <span m="1634940">what</span> <span m="1635210">they</span>
  <span m="1635360">were</span> <span m="1635510">trying</span> <span m="1635840">to</span>
  <span m="1635990">do</span> <span m="1636230">was</span> <span m="1636470">to</span>
  <span m="1636590">follow</span> <span m="1637010">that</span> <span m="1637250">gradient</span>
  <span m="1637910">in</span> <span m="1638030">order</span> <span m="1638300">to</span>
  <span m="1638480">find</span> <span m="1639790">the</span> <span m="1640250">most</span>
  <span m="1640520">atypical</span> <span m="1642370">part</span> <span m="1642700">of</span>
  <span m="1643100">of the</span> <span m="1644000">image.</span> <span m="1645450">Is</span>
  <span m="1645710">that</span> <span m="1646090">still</span> <span m="1646420">believed</span>
  <span m="1646870">to</span> <span m="1647020">be</span> <span m="1647170">true?</span></p><p><span
  m="1647920">ANDY BECK:</span> <span m="1648085">Yeah.</span> <span m="1648250">That</span>
  <span m="1648400">it's</span> <span m="1648550">a</span> <span m="1648580">continuum?</span>
  <span m="1649890">Yeah,</span> <span m="1650450">definitely.</span></p><p><span
  m="1651380">PROFESSOR:</span> <span m="1651523">You</span> <span m="1651666">mean</span>
  <span m="1651810">within</span> <span m="1652240">a</span> <span m="1652450">sample</span>
  <span m="1654360">and in the slides.</span></p><p><span m="1655240">ANDY BECK:</span>
  <span m="1655307">Yeah,</span> <span m="1656070">I</span> <span m="1656110">mean,</span>
  <span m="1656650">you</span> <span m="1656710">mean</span> <span m="1656860">just</span>
  <span m="1656980">like</span> <span m="1657130">a</span> <span m="1657430">continuum</span>
  <span m="1658060">of</span> <span m="1658180">aggressiveness.</span> <span m="1659050">Yeah,</span>
  <span m="1659470">I</span> <span m="1659590">think</span> <span m="1659770">it</span>
  <span m="1659860">is</span> <span m="1660040">a</span> <span m="1660130">continuum.</span>
  <span m="1660570">I</span> <span m="1660610">mean,</span> <span m="1661390">this</span>
  <span m="1661630">is</span> <span m="1661780">more</span> <span m="1662050">of</span>
  <span m="1662170">a</span> <span m="1662200">binary</span> <span m="1662680">task,</span>
  <span m="1663460">but</span> <span m="1663700">there's</span> <span m="1663880">going</span>
  <span m="1663970">to</span> <span m="1664060">be</span> <span m="1664720">continuums</span>
  <span m="1665590">of</span> <span m="1665770">grade</span> <span m="1666280">within</span>
  <span m="1666640">the</span> <span m="1666730">cancer.</span> <span m="1667720">I</span>
  <span m="1667780">mean,</span> <span m="1667930">that's</span> <span m="1668200">another</span>
  <span m="1668680">level</span> <span m="1669070">of</span> <span m="1669160">adding</span>
  <span m="1669520">on.</span></p><p><span m="1670000">If</span> <span m="1670060">we</span>
  <span m="1670150">wanted</span> <span m="1670270">to</span> <span m="1670360">correlate</span>
  <span m="1670840">this</span> <span m="1671080">with</span> <span m="1671290">outcome,</span>
  <span m="1672130">it</span> <span m="1672250">would</span> <span m="1672340">definitely</span>
  <span m="1672700">be</span> <span m="1672820">valuable</span> <span m="1673450">to</span>
  <span m="1673600">do</span> <span m="1673780">that.</span> <span m="1674380">To</span>
  <span m="1674530">not</span> <span m="1674770">just</span> <span m="1675010">say</span>
  <span m="1675130">quantitate</span> <span m="1675670">the</span> <span m="1675790">bulk</span>
  <span m="1676120">of</span> <span m="1676240">tumor</span> <span m="1676730">but</span>
  <span m="1677290">to</span> <span m="1677710">estimate</span> <span m="1678250">the</span>
  <span m="1678580">malignancy</span> <span m="1679210">of</span> <span m="1679300">every</span>
  <span m="1679600">individual</span> <span m="1680050">nucleus,</span> <span m="1680770">which</span>
  <span m="1680980">we</span> <span m="1681070">can</span> <span m="1681250">do</span>
  <span m="1681430">also.</span> <span m="1682270">So</span> <span m="1682390">you</span>
  <span m="1682450">can</span> <span m="1682570">actually</span> <span m="1682780">classify,</span>
  <span m="1684040">not</span> <span m="1684280">just</span> <span m="1684460">tumor</span>
  <span m="1684730">region</span> <span m="1685180">but</span> <span m="1685420">you
  can classify</span> <span m="1685750">individual</span> <span m="1686140">cells.</span>
  <span m="1686830">And</span> <span m="1686920">you</span> <span m="1686980">can</span>
  <span m="1687070">classify</span> <span m="1687430">them</span> <span m="1687550">based</span>
  <span m="1687880">on</span> <span m="1688060">malignancy.</span> <span m="1689200">And</span>
  <span m="1689350">then</span> <span m="1689470">you</span> <span m="1689590">can</span>
  <span m="1689800">get</span> <span m="1689950">the,</span> <span m="1690040">sort</span>
  <span m="1690220">of,</span> <span m="1690310">gradient</span> <span m="1691480">within</span>
  <span m="1691750">a</span> <span m="1691810">population.</span></p><p><span m="1692500">In</span>
  <span m="1692590">this</span> <span m="1692740">study,</span> <span m="1693070">it</span>
  <span m="1693130">was</span> <span m="1693250">just</span> <span m="1693460">a</span>
  <span m="1693520">region-based,</span> <span m="1694750">not</span> <span m="1694930">a</span>
  <span m="1694990">cell-based,</span> <span m="1696130">but</span> <span m="1696400">you</span>
  <span m="1696520">can</span> <span m="1696640">definitely</span> <span m="1696970">do</span>
  <span m="1697090">that,</span> <span m="1697300">and</span> <span m="1697460">definitely,</span>
  <span m="1698365">it's</span> <span m="1698800">a</span> <span m="1698860">spectrum.</span>
  <span m="1699440">I</span> <span m="1699540">mean,</span> <span m="1699640">it's</span>
  <span m="1699740">kind</span> <span m="1699840">of</span> <span m="1699940">like</span>
  <span m="1700040">the</span> <span m="1700140">atypia</span> <span m="1700360">idea.</span>
  <span m="1701140">Everything</span> <span m="1701440">in</span> <span m="1701500">biology</span>
  <span m="1702040">is</span> <span m="1702760">pretty</span> <span m="1702970">much</span>
  <span m="1703120">on</span> <span m="1703210">a</span> <span m="1703270">spectrum,</span>
  <span m="1703690">like</span> <span m="1703870">from</span> <span m="1704110">normal</span>
  <span m="1704530">to</span> <span m="1705250">atypical</span> <span m="1705910">to</span>
  <span m="1706120">low-grade</span> <span m="1706450">cancer,</span> <span m="1707080">medium-grade</span>
  <span m="1707560">cancer,</span> <span m="1708130">high-grade</span> <span m="1708460">cancer,</span>
  <span m="1709840">and</span> <span m="1710140">these</span> <span m="1710290">sorts</span>
  <span m="1710530">of</span> <span m="1710620">methods</span> <span m="1710980">do</span>
  <span m="1711100">allow</span> <span m="1711370">you</span> <span m="1711895">to</span>
  <span m="1712360">really</span> <span m="1712660">more</span> <span m="1712810">precisely</span>
  <span m="1713590">estimate</span> <span m="1714250">where</span> <span m="1714430">you</span>
  <span m="1714550">are</span> <span m="1714640">on</span> <span m="1714730">that</span>
  <span m="1714850">continuum.</span></p><p><span m="1718690">And</span> <span m="1719220">that's</span>
  <span m="1719490">the</span> <span m="1719640">basic</span> <span m="1720150">approach.</span>
  <span m="1721350">We</span> <span m="1721530">get</span> <span m="1721680">the</span>
  <span m="1721800">big</span> <span m="1722010">whole</span> <span m="1722140">site</span>
  <span m="1722340">images.</span> <span m="1722910">We</span> <span m="1723120">figure</span>
  <span m="1723480">out</span> <span m="1723630">how</span> <span m="1723750">to</span>
  <span m="1723870">sample</span> <span m="1724260">patches</span> <span m="1724800">from</span>
  <span m="1724950">the</span> <span m="1725040">different</span> <span m="1725250">regions</span>
  <span m="1725730">to</span> <span m="1725880">optimize</span> <span m="1726360">performance</span>
  <span m="1726750">of</span> <span m="1726810">the</span> <span m="1726870">model</span>
  <span m="1727590">during</span> <span m="1727830">training</span> <span m="1728130">time.</span>
  <span m="1728370">And</span> <span m="1728500">then during</span> <span m="1728730">testing</span>
  <span m="1729060">time,</span> <span m="1729900">just</span> <span m="1730200">we</span>
  <span m="1730320">take</span> <span m="1730530">a</span> <span m="1730590">whole</span>
  <span m="1730740">big</span> <span m="1730980">whole</span> <span m="1731100">site</span>
  <span m="1731280">image.</span> <span m="1731570">We</span> <span m="1731670">break</span>
  <span m="1731970">it</span> <span m="1732030">into</span> <span m="1732210">millions</span>
  <span m="1732540">of</span> <span m="1732630">little</span> <span m="1732810">patches.</span>
  <span m="1733680">Send</span> <span m="1733980">each</span> <span m="1734130">patch</span>
  <span m="1734910">individually.</span></p><p><span m="1735840">We</span> <span m="1735960">don't</span>
  <span m="1736140">actually--</span> <span m="1736470">you</span> <span m="1736620">could</span>
  <span m="1736890">potentially</span> <span m="1737370">use</span> <span m="1737550">spatial</span>
  <span m="1737940">information</span> <span m="1738480">about</span> <span m="1739200">how</span>
  <span m="1739350">close</span> <span m="1739650">they</span> <span m="1739740">are</span>
  <span m="1739800">to</span> <span m="1739890">each</span> <span m="1740070">other,</span>
  <span m="1740860">which</span> <span m="1741000">would</span> <span m="1741090">make</span>
  <span m="1741240">the</span> <span m="1741300">process</span> <span m="1742050">less</span>
  <span m="1742290">efficient.</span> <span m="1743130">We</span> <span m="1743220">don't</span>
  <span m="1743400">do</span> <span m="1743520">that.</span> <span m="1743700">We</span>
  <span m="1743790">just</span> <span m="1743940">send</span> <span m="1744120">them</span>
  <span m="1744270">in</span> <span m="1744540">individually</span> <span m="1745320">and</span>
  <span m="1745470">then</span> <span m="1746430">visualize</span> <span m="1747060">the</span>
  <span m="1747180">output</span> <span m="1747750">as</span> <span m="1747900">a</span>
  <span m="1747960">heat</span> <span m="1748110">map.</span></p><p><span m="1750960">And</span>
  <span m="1751350">this,</span> <span m="1751620">I</span> <span m="1751710">think,</span>
  <span m="1751950">isn't</span> <span m="1752370">in</span> <span m="1752490">the</span>
  <span m="1752580">reference</span> <span m="1753030">I</span> <span m="1753120">sent</span>
  <span m="1753720">so</span> <span m="1753930">the</span> <span m="1754020">one</span>
  <span m="1754140">I</span> <span m="1754230">sent</span> <span m="1754530">showed</span>
  <span m="1754890">how</span> <span m="1755700">you</span> <span m="1755820">were</span>
  <span m="1755940">able</span> <span m="1756210">to</span> <span m="1756480">combine</span>
  <span m="1757500">the</span> <span m="1758430">estimates</span> <span m="1759060">of</span>
  <span m="1759210">the</span> <span m="1759300">deep</span> <span m="1759510">learning</span>
  <span m="1759750">system</span> <span m="1760140">with</span> <span m="1760860">the</span>
  <span m="1761070">human</span> <span m="1761370">pathologist's</span> <span m="1761910">estimate</span>
  <span m="1762420">to</span> <span m="1762570">make</span> <span m="1762900">the</span>
  <span m="1762990">human</span> <span m="1763170">pathologist's</span> <span m="1763680">error</span>
  <span m="1763930">rate</span> <span m="1764070">go</span> <span m="1764220">down</span>
  <span m="1764400">by</span> <span m="1764690">85%</span> <span m="1765870">and</span>
  <span m="1766020">get</span> <span m="1766230">to</span> <span m="1766980">less</span>
  <span m="1767220">than</span> <span m="1767310">1%.</span></p><p><span m="1768810">And</span>
  <span m="1769080">the</span> <span m="1769290">interesting</span> <span m="1769560">thing</span>
  <span m="1769680">about</span> <span m="1769830">how</span> <span m="1769920">these</span>
  <span m="1770010">systems</span> <span m="1770400">keep</span> <span m="1770550">getting</span>
  <span m="1770730">better</span> <span m="1770880">over</span> <span m="1771030">time</span>
  <span m="1771360">and</span> <span m="1771480">potentially</span> <span m="1771960">they</span>
  <span m="1772110">over-fit</span> <span m="1772590">to</span> <span m="1772750">the</span>
  <span m="1773550">competition</span> <span m="1774150">data</span> <span m="1774390">set--</span>
  <span m="1774640">because</span> <span m="1774880">I think we</span> <span m="1774990">submitted,</span>
  <span m="1775530">maybe,</span> <span m="1775800">three</span> <span m="1776100">times,</span>
  <span m="1776910">which</span> <span m="1777090">isn't</span> <span m="1777240">that</span>
  <span m="1777360">many.</span> <span m="1778020">But</span> <span m="1779400">over</span>
  <span m="1779700">the</span> <span m="1779790">course</span> <span m="1780090">of</span>
  <span m="1780330">six</span> <span m="1780600">months</span> <span m="1780990">after</span>
  <span m="1781200">the</span> <span m="1781290">first</span> <span m="1781500">closing</span>
  <span m="1781890">of the</span> <span m="1781980">competition,</span> <span m="1782700">people</span>
  <span m="1783030">kept</span> <span m="1783330">competing</span> <span m="1783930">and</span>
  <span m="1784020">making</span> <span m="1784290">systems</span> <span m="1784650">better.</span>
  <span m="1785220">And</span> <span m="1785340">actually,</span> <span m="1785580">the</span>
  <span m="1785670">fully</span> <span m="1785940">automated</span> <span m="1786390">system</span>
  <span m="1786720">on</span> <span m="1786810">this</span> <span m="1787060">data</span>
  <span m="1787300">set</span> <span m="1787950">achieved</span> <span m="1788370">an</span>
  <span m="1788460">error</span> <span m="1788640">rate</span> <span m="1788820">of</span>
  <span m="1788910">less</span> <span m="1789150">than</span> <span m="1789300">1%</span>
  <span m="1789840">by</span> <span m="1790290">the</span> <span m="1790350">final</span>
  <span m="1790650">submission</span> <span m="1791100">date,</span> <span m="1792040">which</span>
  <span m="1792150">was</span> <span m="1792270">significantly</span> <span m="1792930">better</span>
  <span m="1793260">than</span> <span m="1793950">both</span> <span m="1794220">the</span>
  <span m="1794310">pathologists</span> <span m="1794780">in</span> <span m="1794850">the</span>
  <span m="1794910">competition,</span> <span m="1795670">which</span> <span m="1795810">is</span>
  <span m="1795930">the</span> <span m="1796080">error</span> <span m="1796310">rate,</span>
  <span m="1796650">I</span> <span m="1796770">believe,</span> <span m="1797070">cited</span>
  <span m="1797490">in</span> <span m="1797730">the</span> <span m="1797880">initial</span>
  <span m="1798360">archive</span> <span m="1798720">paper.</span></p><p><span m="1800220">And</span>
  <span m="1800340">also,</span> <span m="1800670">they</span> <span m="1800790">took</span>
  <span m="1800970">the</span> <span m="1801060">same</span> <span m="1801300">set</span>
  <span m="1801450">of</span> <span m="1801540">slides</span> <span m="1801960">and</span>
  <span m="1802050">sent</span> <span m="1802260">them</span> <span m="1802380">out</span>
  <span m="1802500">to</span> <span m="1802590">pathologists</span> <span m="1803400">operating</span>
  <span m="1803760">in</span> <span m="1803820">clinical</span> <span m="1804120">practice,</span>
  <span m="1805710">where</span> <span m="1805860">they</span> <span m="1805950">had</span>
  <span m="1806100">really</span> <span m="1806370">significantly</span> <span m="1806850">higher</span>
  <span m="1807150">error</span> <span m="1807360">rates,</span> <span m="1808150">mainly</span>
  <span m="1808410">due</span> <span m="1808530">to</span> <span m="1808650">the</span>
  <span m="1808740">fact,</span> <span m="1809110">they were</span> <span m="1809160">more</span>
  <span m="1809340">constrained</span> <span m="1809880">by</span> <span m="1810060">time</span>
  <span m="1810420">limitations</span> <span m="1811650">in</span> <span m="1811800">clinical</span>
  <span m="1812070">practice</span> <span m="1812520">than</span> <span m="1812700">in</span>
  <span m="1812790">the</span> <span m="1812850">competition.</span> <span m="1813840">And</span>
  <span m="1813960">most of the</span> <span m="1814290">errors</span> <span m="1814620">they
  are</span> <span m="1814740">making</span> <span m="1815020">are false</span> <span
  m="1815400">negatives.</span> <span m="1815820">Simply,</span> <span m="1816210">they</span>
  <span m="1816300">don't</span> <span m="1816480">have</span> <span m="1816600">the</span>
  <span m="1816690">time</span> <span m="1816930">to</span> <span m="1817020">focus</span>
  <span m="1817440">on</span> <span m="1817710">small</span> <span m="1818070">regions</span>
  <span m="1818730">of</span> <span m="1818850">metastasis</span> <span m="1819630">amid</span>
  <span m="1819960">these</span> <span m="1820500">humongous</span> <span m="1821340">giga</span>
  <span m="1821610">pixel-size</span> <span m="1823080">slides.</span></p><p><span
  m="1824432">AUDIENCE:</span> <span m="1824651">In</span> <span m="1824870">the</span>
  <span m="1825010">paper,</span> <span m="1825340">you say</span> <span m="1825570">you</span>
  <span m="1825780">combined</span> <span m="1827040">the</span> <span m="1827280">machine</span>
  <span m="1827780">learning</span> <span m="1828065">options</span> <span m="1828350">with</span>
  <span m="1828670">the</span> <span m="1829080">pathologists,</span> <span m="1829870">but</span>
  <span m="1830270">you</span> <span m="1830400">don't really say</span> <span m="1830700">how.</span>
  <span m="1831410">Is that it that</span> <span m="1831700">they</span> <span m="1832090">look</span>
  <span m="1832360">at the</span> <span m="1832630">heat maps,</span> <span m="1833790">or
  is</span> <span m="1834120">it</span> <span m="1834570">just</span> <span m="1835350">sort</span>
  <span m="1835560">of</span> <span m="1835880">combined?</span></p><p><span m="1836820">ANDY
  BECK:</span> <span m="1837000">Yeah,</span> <span m="1837180">no,</span> <span m="1837390">it's</span>
  <span m="1837540">a</span> <span m="1837570">great</span> <span m="1837900">question.</span>
  <span m="1838510">So</span> <span m="1838740">today,</span> <span m="1839340">we</span>
  <span m="1839490">do</span> <span m="1839730">it</span> <span m="1840240">that</span>
  <span m="1840840">way.</span> <span m="1841510">And</span> <span m="1841610">that's</span>
  <span m="1841710">the</span> <span m="1841770">way</span> <span m="1842160">in</span>
  <span m="1842310">clinical</span> <span m="1842610">practice</span> <span m="1843150">we're</span>
  <span m="1843300">building</span> <span m="1843720">it,</span> <span m="1843930">that</span>
  <span m="1844140">the</span> <span m="1844290">pathologists</span> <span m="1844890">will</span>
  <span m="1845070">look</span> <span m="1845310">at</span> <span m="1845370">both</span>
  <span m="1845700">and</span> <span m="1845820">then</span> <span m="1846330">make</span>
  <span m="1846540">a</span> <span m="1846570">diagnosis</span> <span m="1847200">based</span>
  <span m="1847560">on</span> <span m="1847800">incorporating</span> <span m="1848190">both.</span></p><p><span
  m="1848610">For</span> <span m="1848730">the</span> <span m="1848820">competition,</span>
  <span m="1850110">it</span> <span m="1850290">was</span> <span m="1850440">very</span>
  <span m="1850680">simple,</span> <span m="1851040">and</span> <span m="1851160">the</span>
  <span m="1851270">organizers</span> <span m="1851850">actually</span> <span m="1852090">did</span>
  <span m="1852240">it.</span> <span m="1852690">They</span> <span m="1852900">interpreted</span>
  <span m="1853350">them</span> <span m="1853470">independently.</span> <span m="1854650">So</span>
  <span m="1854670">the</span> <span m="1854760">pathologists</span> <span m="1855240">just</span>
  <span m="1855390">looked</span> <span m="1855540">at</span> <span m="1855600">all</span>
  <span m="1855690">the</span> <span m="1855750">slides.</span> <span m="1856230">Our</span>
  <span m="1856320">system</span> <span m="1857010">made</span> <span m="1857130">a</span>
  <span m="1857190">prediction.</span> <span m="1857620">It</span> <span m="1857670">was</span>
  <span m="1857790">literally</span> <span m="1858240">the</span> <span m="1858360">average</span>
  <span m="1858960">of</span> <span m="1859140">the</span> <span m="1859260">probability</span>
  <span m="1860040">that</span> <span m="1860160">that</span> <span m="1860410">slide</span>
  <span m="1860640">contained</span> <span m="1860910">cancer.</span> <span m="1861760">That</span>
  <span m="1861930">became</span> <span m="1862140">the</span> <span m="1862200">final</span>
  <span m="1862440">score,</span> <span m="1862740">and</span> <span m="1862830">then</span>
  <span m="1862920">the</span> <span m="1863010">AUC</span> <span m="1863490">went</span>
  <span m="1863640">to</span> <span m="1863910">99%</span> <span m="1864660">from</span>
  <span m="1865500">whatever</span> <span m="1865770">it</span> <span m="1865830">was,</span>
  <span m="1866100">92%</span> <span m="1867300">by</span> <span m="1867480">combining</span>
  <span m="1868020">these</span> <span m="1868170">two</span> <span m="1868290">scores.</span></p><p><span
  m="1869530">AUDIENCE:</span> <span m="1869600">I</span> <span m="1869670">guess</span>
  <span m="1869740">they make</span> <span m="1870110">uncorrelated</span> <span m="1870530">errors.</span></p><p><span
  m="1870840">ANDY BECK:</span> <span m="1871020">Exactly.</span> <span m="1871560">They're</span>
  <span m="1872400">pretty</span> <span m="1872610">much</span> <span m="1872790">uncorrelated,</span>
  <span m="1873420">particularly</span> <span m="1873900">because</span> <span m="1874140">the</span>
  <span m="1874200">pathologists</span> <span m="1874700">tend</span> <span m="1874860">to</span>
  <span m="1874920">have</span> <span m="1875040">almost</span> <span m="1875370">all</span>
  <span m="1875550">false</span> <span m="1875850">negatives,</span> <span m="1876990">and</span>
  <span m="1878150">the</span> <span m="1878640">deep</span> <span m="1878880">learning</span>
  <span m="1879120">system</span> <span m="1879780">tends</span> <span m="1880050">to</span>
  <span m="1880110">be</span> <span m="1880230">fooled</span> <span m="1880530">by</span>
  <span m="1880710">a</span> <span m="1880770">few</span> <span m="1880950">things,</span>
  <span m="1881250">like</span> <span m="1881460">artefact.</span> <span m="1882090">And</span>
  <span m="1882780">they</span> <span m="1883110">do</span> <span m="1883230">make</span>
  <span m="1883410">uncorrelated</span> <span m="1883950">errors,</span> <span m="1884190">and</span>
  <span m="1884280">that's</span> <span m="1884430">why</span> <span m="1884520">there's</span>
  <span m="1884700">a</span> <span m="1884760">huge</span> <span m="1885000">bump</span>
  <span m="1885210">in</span> <span m="1885270">performance.</span></p><p><span m="1891230">So</span>
  <span m="1891680">I</span> <span m="1891740">kind</span> <span m="1891920">of</span>
  <span m="1892010">made</span> <span m="1892220">a</span> <span m="1892310">reference</span>
  <span m="1892790">to</span> <span m="1892880">this,</span> <span m="1893180">but</span>
  <span m="1893420">any</span> <span m="1893600">of</span> <span m="1893660">these</span>
  <span m="1893810">competition</span> <span m="1894500">data</span> <span m="1894760">sets</span>
  <span m="1895280">are</span> <span m="1895430">relatively</span> <span m="1896180">easy</span>
  <span m="1896570">to</span> <span m="1896720">get</span> <span m="1897110">really</span>
  <span m="1897470">good</span> <span m="1897710">at.</span> <span m="1898430">People</span>
  <span m="1898790">have</span> <span m="1898940">shown</span> <span m="1899390">that</span>
  <span m="1899540">you</span> <span m="1899630">can</span> <span m="1899750">actually</span>
  <span m="1899960">build</span> <span m="1900170">models</span> <span m="1900560">that</span>
  <span m="1900650">just</span> <span m="1900800">predict</span> <span m="1901160">a</span>
  <span m="1901200">data</span> <span m="1901450">set</span> <span m="1902000">using</span>
  <span m="1902240">deep</span> <span m="1902450">learning.</span> <span m="1903080">Like,</span>
  <span m="1903200">deep</span> <span m="1903410">learning</span> <span m="1903680">is</span>
  <span m="1903770">almost</span> <span m="1903980">too</span> <span m="1904190">good</span>
  <span m="1904340">at</span> <span m="1904430">finding</span> <span m="1904790">certain</span>
  <span m="1905870">patterns</span> <span m="1906690">and</span> <span m="1906810">can</span>
  <span m="1906910">find</span> <span m="1907220">artefact.</span> <span m="1908480">So</span>
  <span m="1908610">it's</span> <span m="1908680">just</span> <span m="1908840">a</span>
  <span m="1908870">caveat</span> <span m="1909230">to</span> <span m="1909290">keep</span>
  <span m="1909440">in</span> <span m="1909530">mind.</span></p><p><span m="1909800">We're</span>
  <span m="1909980">doing</span> <span m="1910220">experiments</span> <span m="1910850">on</span>
  <span m="1911480">lots</span> <span m="1911690">of</span> <span m="1911780">real-world</span>
  <span m="1914600">testing</span> <span m="1915230">of</span> <span m="1915320">methods</span>
  <span m="1915710">like</span> <span m="1915860">this</span> <span m="1916040">across</span>
  <span m="1916400">many</span> <span m="1916640">labs</span> <span m="1917050">with</span>
  <span m="1917120">many</span> <span m="1917330">different</span> <span m="1917540">standing</span>
  <span m="1917930">procedures</span> <span m="1918620">and</span> <span m="1918800">tissue</span>
  <span m="1919100">preparation</span> <span m="1919610">procedures,</span> <span
  m="1920220">et</span> <span m="1920320">cetera,</span> <span m="1920990">to</span>
  <span m="1921350">evaluate</span> <span m="1921720">the</span> <span m="1921870">robustness.</span>
  <span m="1922460">But</span> <span m="1922580">that's</span> <span m="1922730">why</span>
  <span m="1923300">competition</span> <span m="1923870">results,</span> <span m="1924260">even</span>
  <span m="1924440">ImageNet</span> <span m="1924980">always</span> <span m="1925250">need</span>
  <span m="1925340">to</span> <span m="1925400">be</span> <span m="1925490">taken</span>
  <span m="1925850">with</span> <span m="1926060">a</span> <span m="1926120">grain</span>
  <span m="1926390">of</span> <span m="1926450">salt.</span></p><p><span m="1929890">And</span>
  <span m="1930000">then</span> <span m="1930510">but</span> <span m="1930810">we</span>
  <span m="1931030">sort</span> <span m="1931290">of</span> <span m="1931350">think</span>
  <span m="1931500">the</span> <span m="1931590">value</span> <span m="1931980">add</span>
  <span m="1932130">of</span> <span m="1932220">this</span> <span m="1932370">is</span>
  <span m="1932490">going</span> <span m="1932570">to</span> <span m="1932670">be</span>
  <span m="1932760">huge.</span> <span m="1933240">I</span> <span m="1933340">mean,</span>
  <span m="1933360">it's</span> <span m="1933510">hard</span> <span m="1933720">to</span>
  <span m="1933840">tell</span> <span m="1934230">because</span> <span m="1934410">it's</span>
  <span m="1934510">such</span> <span m="1934710">a</span> <span m="1934740">big</span>
  <span m="1934890">image,</span> <span m="1935290">but</span> <span m="1935310">this</span>
  <span m="1935430">is</span> <span m="1935550">what</span> <span m="1935640">a</span>
  <span m="1935700">pathologist</span> <span m="1935965">today</span> <span m="1936230">is</span>
  <span m="1936420">looking</span> <span m="1936620">at</span> <span m="1936690">under</span>
  <span m="1936840">a</span> <span m="1936870">microscope,</span> <span m="1938020">and</span>
  <span m="1938040">it's</span> <span m="1938160">very</span> <span m="1938340">hard</span>
  <span m="1938580">to</span> <span m="1938670">see</span> <span m="1938940">anything.</span>
  <span m="1939195">And</span> <span m="1939450">with</span> <span m="1939570">a</span>
  <span m="1939630">very</span> <span m="1940050">simple</span> <span m="1941040">visualization,</span>
  <span m="1942150">just</span> <span m="1942420">of</span> <span m="1942540">the</span>
  <span m="1942690">output</span> <span m="1942960">of</span> <span m="1943020">the</span>
  <span m="1943110">AI</span> <span m="1943410">system</span> <span m="1943800">as</span>
  <span m="1943980">red</span> <span m="1944370">where</span> <span m="1944550">cancer</span>
  <span m="1945060">looks</span> <span m="1945240">like</span> <span m="1945390">it</span>
  <span m="1945450">is.</span> <span m="1946350">It's</span> <span m="1946530">clearly</span>
  <span m="1946980">a</span> <span m="1947070">sort</span> <span m="1947250">of</span>
  <span m="1947430">great</span> <span m="1947730">map</span> <span m="1948150">of</span>
  <span m="1948240">the</span> <span m="1948390">areas</span> <span m="1948720">they</span>
  <span m="1948840">need</span> <span m="1948990">to</span> <span m="1949050">be</span>
  <span m="1949170">sure</span> <span m="1949320">to</span> <span m="1949410">focus</span>
  <span m="1949770">on.</span></p><p><span m="1950580">And</span> <span m="1950700">this</span>
  <span m="1950880">is</span> <span m="1951150">real</span> <span m="1951600">data</span>
  <span m="1951960">from</span> <span m="1952140">this</span> <span m="1952290">example,</span>
  <span m="1952680">where</span> <span m="1952860">this</span> <span m="1953070">bright</span>
  <span m="1953400">red</span> <span m="1953580">area,</span> <span m="1953910">in</span>
  <span m="1954000">fact,</span> <span m="1954240">contains</span> <span m="1954660">this</span>
  <span m="1954840">tiny</span> <span m="1955230">little</span> <span m="1955500">rim</span>
  <span m="1955800">of</span> <span m="1955950">metastatic</span> <span m="1957120">breast</span>
  <span m="1957330">cancer</span> <span m="1957630">cells</span> <span m="1957960">that
  would</span> <span m="1958050">be</span> <span m="1958170">very</span> <span m="1958530">easy</span>
  <span m="1958770">to</span> <span m="1958890">miss</span> <span m="1959400">without</span>
  <span m="1959760">that</span> <span m="1959970">assistant</span> <span m="1960810">sort</span>
  <span m="1961020">of</span> <span m="1961080">just</span> <span m="1961260">pointing</span>
  <span m="1961710">you</span> <span m="1961920">in</span> <span m="1962040">the</span>
  <span m="1962100">right</span> <span m="1962220">place</span> <span m="1962430">to</span>
  <span m="1962520">look</span> <span m="1962730">at,</span> <span m="1963210">because</span>
  <span m="1963480">it's</span> <span m="1963630">a</span> <span m="1963690">tiny</span>
  <span m="1964110">set</span> <span m="1964380">of</span> <span m="1964830">20</span>
  <span m="1965250">cells</span> <span m="1965670">amid</span> <span m="1965910">a</span>
  <span m="1965970">big</span> <span m="1966180">sea</span> <span m="1966480">of</span>
  <span m="1966630">all</span> <span m="1966810">these</span> <span m="1966930">normal</span>
  <span m="1967620">lymphocytes.</span></p><p><span m="1968820">And</span> <span m="1968940">here's</span>
  <span m="1969120">another</span> <span m="1969480">one</span> <span m="1969690">that,</span>
  <span m="1969810">again,</span> <span m="1970080">now</span> <span m="1970230">you</span>
  <span m="1970290">can</span> <span m="1970410">see</span> <span m="1970530">from</span>
  <span m="1970740">low</span> <span m="1970920">power.</span> <span m="1971790">It's</span>
  <span m="1971890">like</span> <span m="1971940">a</span> <span m="1972000">satellite</span>
  <span m="1972510">image</span> <span m="1972750">or</span> <span m="1972810">something,</span>
  <span m="1973080">where</span> <span m="1973170">you</span> <span m="1973260">can</span>
  <span m="1973770">focus</span> <span m="1974240">immediately</span> <span m="1974580">on</span>
  <span m="1974670">this</span> <span m="1974820">little</span> <span m="1974970">red</span>
  <span m="1975150">area,</span> <span m="1976170">that,</span> <span m="1976420">again,</span>
  <span m="1976720">is</span> <span m="1976740">a</span> <span m="1976800">tiny</span>
  <span m="1977160">pocket</span> <span m="1977550">of</span> <span m="1977820">10</span>
  <span m="1978120">cancer</span> <span m="1978540">cells</span> <span m="1978960">amid</span>
  <span m="1979440">hundreds</span> <span m="1979860">of</span> <span m="1979950">thousands</span>
  <span m="1980280">of</span> <span m="1980370">normal</span> <span m="1980640">cells</span>
  <span m="1981350">that</span> <span m="1981550">are</span> <span m="1981600">now</span>
  <span m="1981780">visible</span> <span m="1983920">from</span> <span m="1984250">low</span>
  <span m="1984430">power.</span></p><p><span m="1985750">So</span> <span m="1986200">this</span>
  <span m="1986410">is</span> <span m="1986530">one</span> <span m="1987220">application</span>
  <span m="1988120">we're</span> <span m="1988300">working</span> <span m="1988750">on,</span>
  <span m="1990010">where</span> <span m="1990460">the</span> <span m="1990760">clinical</span>
  <span m="1991150">use</span> <span m="1991390">case</span> <span m="1991720">will</span>
  <span m="1991870">be</span> <span m="1993490">today,</span> <span m="1993940">people</span>
  <span m="1994270">are</span> <span m="1994360">just</span> <span m="1994570">sort</span>
  <span m="1994780">of</span> <span m="1994870">looking</span> <span m="1995230">at</span>
  <span m="1995380">images</span> <span m="1995770">without</span> <span m="1996010">the</span>
  <span m="1996100">assistance</span> <span m="1996520">of</span> <span m="1996610">any</span>
  <span m="1996760">machine</span> <span m="1997060">learning.</span> <span m="1997900">And</span>
  <span m="1998230">they</span> <span m="1998320">just</span> <span m="1998440">have</span>
  <span m="1998560">to</span> <span m="1998650">kind</span> <span m="1998860">of</span>
  <span m="1998920">pick</span> <span m="1999340">a</span> <span m="1999430">number</span>
  <span m="1999790">of</span> <span m="1999940">patches</span> <span m="2000450">to</span>
  <span m="2000570">focus</span> <span m="2000990">on</span> <span m="2001200">with</span>
  <span m="2001350">no</span> <span m="2001560">guidance.</span> <span m="2002490">So</span>
  <span m="2002700">sometimes</span> <span m="2003030">they</span> <span m="2003120">focus</span>
  <span m="2003450">on</span> <span m="2003540">the</span> <span m="2003600">right</span>
  <span m="2003750">patches,</span> <span m="2004140">sometimes</span> <span m="2004470">they</span>
  <span m="2004560">don't,</span> <span m="2004770">but</span> <span m="2004890">clearly</span>
  <span m="2005320">they</span> <span m="2005460">don't</span> <span m="2005610">have</span>
  <span m="2005730">time</span> <span m="2006510">to</span> <span m="2006660">look</span>
  <span m="2006840">at</span> <span m="2006930">all</span> <span m="2007260">of</span>
  <span m="2007350">this</span> <span m="2007590">at</span> <span m="2007680">high</span>
  <span m="2007860">magnification,</span> <span m="2009030">because</span> <span m="2009210">that</span>
  <span m="2009360">would</span> <span m="2009450">take</span> <span m="2009930">an</span>
  <span m="2010050">entire</span> <span m="2010440">day</span> <span m="2010970">if</span>
  <span m="2011090">you</span> <span m="2011150">were</span> <span m="2011220">trying</span>
  <span m="2011430">to</span> <span m="2011520">look</span> <span m="2011730">at</span>
  <span m="2011820">40X</span> <span m="2012420">magnification</span> <span m="2013020">at</span>
  <span m="2013080">the</span> <span m="2013140">whole</span> <span m="2013290">image.</span></p><p><span
  m="2013890">So</span> <span m="2014160">they</span> <span m="2014340">sort</span>
  <span m="2014520">of use</span> <span m="2014760">their</span> <span m="2014850">intuition</span>
  <span m="2015270">to</span> <span m="2015330">focus.</span> <span m="2015810">And</span>
  <span m="2015960">for</span> <span m="2016080">that</span> <span m="2016230">reason,</span>
  <span m="2016470">they</span> <span m="2016560">end</span> <span m="2016680">up,</span>
  <span m="2016920">as</span> <span m="2017070">we've</span> <span m="2017220">seen,</span>
  <span m="2017460">making</span> <span m="2018210">significant</span> <span m="2018780">number</span>
  <span m="2019080">of</span> <span m="2019200">mistakes.</span> <span m="2020010">It's</span>
  <span m="2020220">not</span> <span m="2020400">reproducible,</span> <span m="2021000">because</span>
  <span m="2021180">people</span> <span m="2021420">focus</span> <span m="2021720">on</span>
  <span m="2021810">different</span> <span m="2022050">aspects</span> <span m="2022350">of</span>
  <span m="2022410">the</span> <span m="2022500">image,</span> <span m="2023180">and</span>
  <span m="2023280">it's</span> <span m="2023400">pretty</span> <span m="2023640">slow.</span></p><p><span
  m="2024450">And</span> <span m="2024600">they're</span> <span m="2024720">faced</span>
  <span m="2025010">with</span> <span m="2025110">this</span> <span m="2025230">empty</span>
  <span m="2025500">report.</span> <span m="2026240">So</span> <span m="2026360">they
  have</span> <span m="2026500">to</span> <span m="2026570">actually</span> <span
  m="2026790">summarize</span> <span m="2027480">everything</span> <span m="2027810">they've</span>
  <span m="2027960">looked</span> <span m="2028260">at</span> <span m="2028440">in</span>
  <span m="2028560">a</span> <span m="2028620">report.</span> <span m="2029070">Like,</span>
  <span m="2029250">what's</span> <span m="2029550">the</span> <span m="2029640">diagnosis?</span>
  <span m="2030240">What's</span> <span m="2030480">the</span> <span m="2030570">size?</span></p><p><span
  m="2031560">So</span> <span m="2031890">let's</span> <span m="2032040">say</span>
  <span m="2032130">there's</span> <span m="2032310">cancer</span> <span m="2032670">here</span>
  <span m="2032940">and</span> <span m="2033030">cancer</span> <span m="2033360">here,</span>
  <span m="2033640">they have to</span> <span m="2034110">manually</span> <span m="2034860">add</span>
  <span m="2035220">the</span> <span m="2035340">distances</span> <span m="2036090">of</span>
  <span m="2036180">the</span> <span m="2036240">cancer</span> <span m="2036570">in</span>
  <span m="2036630">those</span> <span m="2036780">two</span> <span m="2036870">regions.</span>
  <span m="2037900">And</span> <span m="2037920">then</span> <span m="2038040">they</span>
  <span m="2038130">have</span> <span m="2038250">to</span> <span m="2039000">put</span>
  <span m="2039240">this</span> <span m="2039510">into</span> <span m="2040110">a</span>
  <span m="2040170">staging</span> <span m="2040650">system</span> <span m="2041460">that</span>
  <span m="2041580">incorporates</span> <span m="2042240">how</span> <span m="2042420">many</span>
  <span m="2042630">areas</span> <span m="2043020">of</span> <span m="2043230">metastasis</span>
  <span m="2043830">there</span> <span m="2043980">are</span> <span m="2044010">and</span>
  <span m="2044100">how</span> <span m="2044220">big</span> <span m="2044400">are</span>
  <span m="2044490">they?</span> <span m="2045050">And</span> <span m="2045330">all</span>
  <span m="2045540">of</span> <span m="2045630">these</span> <span m="2045810">things</span>
  <span m="2046080">are</span> <span m="2046320">pretty</span> <span m="2046530">much</span>
  <span m="2046710">automatable.</span></p><p><span m="2047690">And</span> <span m="2047820">this</span>
  <span m="2047970">is</span> <span m="2048090">the</span> <span m="2048150">kind</span>
  <span m="2048360">of</span> <span m="2048420">thing</span> <span m="2048540">we're</span>
  <span m="2048659">building,</span> <span m="2049020">where</span> <span m="2049139">the</span>
  <span m="2049230">system</span> <span m="2049620">will</span> <span m="2049860">highlight</span>
  <span m="2050670">where</span> <span m="2050820">it</span> <span m="2050909">sees</span>
  <span m="2051090">cancer,</span> <span m="2051630">tell</span> <span m="2051810">the</span>
  <span m="2051900">pathologist</span> <span m="2052350">to</span> <span m="2052440">focus</span>
  <span m="2052800">there.</span> <span m="2053489">And</span> <span m="2053580">then</span>
  <span m="2053730">based</span> <span m="2054150">on</span> <span m="2054449">the</span>
  <span m="2054600">input</span> <span m="2054810">of</span> <span m="2054870">the</span>
  <span m="2055139">AI</span> <span m="2055510">system</span> <span m="2055679">and</span>
  <span m="2055739">the</span> <span m="2055800">input</span> <span m="2056010">of</span>
  <span m="2056070">the</span> <span m="2056130">pathologist</span> <span m="2056639">can</span>
  <span m="2056760">summarize</span> <span m="2057300">all</span> <span m="2057389">of</span>
  <span m="2057480">that</span> <span m="2057630">data,</span> <span m="2058440">quantitative</span>
  <span m="2059370">as</span> <span m="2059489">well</span> <span m="2059760">as</span>
  <span m="2060810">diagnostic</span> <span m="2061620">as</span> <span m="2061770">well</span>
  <span m="2061980">as</span> <span m="2062100">summary</span> <span m="2062520">staging.</span></p><p><span
  m="2063389">Sort</span> <span m="2063659">of</span> <span m="2063750">if the</span>
  <span m="2063960">pathologist</span> <span m="2064500">then</span> <span m="2064710">takes</span>
  <span m="2065010">this</span> <span m="2065190">is</span> <span m="2065550">their</span>
  <span m="2065699">first</span> <span m="2066120">version</span> <span m="2066480">of</span>
  <span m="2066540">the</span> <span m="2066630">report,</span> <span m="2067080">they</span>
  <span m="2067170">can</span> <span m="2067320">edit</span> <span m="2067590">it,</span>
  <span m="2067710">confirm</span> <span m="2068190">it,</span> <span m="2069000">sign</span>
  <span m="2069330">it</span> <span m="2069420">out.</span> <span m="2069719">That</span>
  <span m="2069960">data</span> <span m="2070199">goes</span> <span m="2070380">back</span>
  <span m="2070590">into</span> <span m="2070710">the</span> <span m="2070800">system,</span>
  <span m="2071250">which</span> <span m="2071460">can</span> <span m="2071610">be</span>
  <span m="2071699">used</span> <span m="2071850">for</span> <span m="2071949">more</span>
  <span m="2072120">training</span> <span m="2072449">data</span> <span m="2072690">in</span>
  <span m="2072780">the</span> <span m="2072840">future</span> <span m="2073340">and</span>
  <span m="2073500">the</span> <span m="2073590">case</span> <span m="2073845">is</span>
  <span m="2074460">signed</span> <span m="2074730">out.</span> <span m="2074850">So</span>
  <span m="2074940">it's</span> <span m="2075060">much</span> <span m="2075239">faster,</span>
  <span m="2075820">much</span> <span m="2076020">more</span> <span m="2077130">accurate,</span>
  <span m="2077460">and</span> <span m="2077550">standardized</span> <span m="2078239">once</span>
  <span m="2078630">this</span> <span m="2078870">thing</span> <span m="2079080">is</span>
  <span m="2079230">fully</span> <span m="2079500">developed,</span> <span m="2079920">which</span>
  <span m="2080100">it</span> <span m="2080400">isn't</span> <span m="2080670">yet.</span></p><p><span
  m="2083080">So</span> <span m="2083530">this</span> <span m="2083770">is</span>
  <span m="2083889">a</span> <span m="2083949">great</span> <span m="2084159">application</span>
  <span m="2084760">for</span> <span m="2085100">AI,</span> <span m="2085480">because</span>
  <span m="2086320">you</span> <span m="2086440">really</span> <span m="2086710">do</span>
  <span m="2086949">need--</span> <span m="2087670">you</span> <span m="2087880">actually</span>
  <span m="2088179">do</span> <span m="2088330">have</span> <span m="2088449">a</span>
  <span m="2088480">ton</span> <span m="2088690">of</span> <span m="2088780">data,</span>
  <span m="2089270">so</span> <span m="2089350">you</span> <span m="2089469">need</span>
  <span m="2089679">to</span> <span m="2089770">do</span> <span m="2089889">an</span>
  <span m="2089949">exhaustive</span> <span m="2090400">analysis</span> <span m="2091000">that</span>
  <span m="2091120">has</span> <span m="2091270">a</span> <span m="2091300">lot</span>
  <span m="2091420">of</span> <span m="2091900">value.</span> <span m="2094025">It's</span>
  <span m="2094300">a</span> <span m="2094330">task</span> <span m="2094810">where</span>
  <span m="2094960">the</span> <span m="2095110">local</span> <span m="2095620">image</span>
  <span m="2095980">data</span> <span m="2096310">in</span> <span m="2096460">a</span>
  <span m="2096489">patch,</span> <span m="2097060">which</span> <span m="2097360">is</span>
  <span m="2097480">really</span> <span m="2097720">what</span> <span m="2097870">this</span>
  <span m="2098020">current</span> <span m="2098440">generation</span> <span m="2099010">of</span>
  <span m="2099100">deep</span> <span m="2099340">CNN's</span> <span m="2099700">are</span>
  <span m="2099790">really</span> <span m="2100000">good</span> <span m="2100210">at,</span>
  <span m="2100390">is</span> <span m="2100570">enough.</span></p><p><span m="2101350">So</span>
  <span m="2101530">we're</span> <span m="2101650">looking</span> <span m="2101950">at</span>
  <span m="2102010">things</span> <span m="2102310">at</span> <span m="2102370">the</span>
  <span m="2102460">cellular</span> <span m="2102880">level.</span> <span m="2103600">Radiology</span>
  <span m="2104230">actually</span> <span m="2104470">could</span> <span m="2104620">be</span>
  <span m="2104710">harder,</span> <span m="2105070">because</span> <span m="2105220">you</span>
  <span m="2105340">often</span> <span m="2105640">want</span> <span m="2105790">to</span>
  <span m="2105850">summarize</span> <span m="2106300">over</span> <span m="2106480">larger</span>
  <span m="2106870">areas.</span> <span m="2107320">Here,</span> <span m="2107560">you</span>
  <span m="2107680">really</span> <span m="2108520">often</span> <span m="2108850">have</span>
  <span m="2109120">the</span> <span m="2109450">salient</span> <span m="2110080">information</span>
  <span m="2110800">in</span> <span m="2111280">patches</span> <span m="2111850">that</span>
  <span m="2112120">really</span> <span m="2112420">are</span> <span m="2112480">scalable</span>
  <span m="2113020">in</span> <span m="2113110">current</span> <span m="2113410">ML</span>
  <span m="2113680">systems.</span></p><p><span m="2114820">And</span> <span m="2114940">then</span>
  <span m="2115030">we</span> <span m="2115090">can</span> <span m="2115240">interpret</span>
  <span m="2115630">the</span> <span m="2115750">output</span> <span m="2116030">to</span>
  <span m="2116110">the</span> <span m="2116200">model.</span> <span m="2116560">So</span>
  <span m="2116680">it</span> <span m="2116740">really</span> <span m="2117010">isn't--</span>
  <span m="2117430">even</span> <span m="2117670">though</span> <span m="2117790">the</span>
  <span m="2117910">model</span> <span m="2118180">itself</span> <span m="2118510">is</span>
  <span m="2118720">a</span> <span m="2118750">black</span> <span m="2119050">box,</span>
  <span m="2120470">we</span> <span m="2120490">can</span> <span m="2120640">visualize</span>
  <span m="2121150">the</span> <span m="2121240">output</span> <span m="2121630">on</span>
  <span m="2121780">top</span> <span m="2122080">of</span> <span m="2122200">the</span>
  <span m="2122350">image,</span> <span m="2122740">which</span> <span m="2122980">gives</span>
  <span m="2123250">us</span> <span m="2123370">incredible</span> <span m="2123910">advantage</span>
  <span m="2124390">in</span> <span m="2124450">terms</span> <span m="2124690">of</span>
  <span m="2124750">interpretability</span> <span m="2125910">of</span> <span m="2126040">what</span>
  <span m="2126160">the</span> <span m="2126250">models</span> <span m="2126580">are</span>
  <span m="2126670">doing</span> <span m="2126910">well,</span> <span m="2127210">what</span>
  <span m="2127330">they're</span> <span m="2127420">doing</span> <span m="2127570">poorly</span>
  <span m="2127960">on.</span> <span m="2129010">And</span> <span m="2129130">it's</span>
  <span m="2129280">a</span> <span m="2129340">specialty,</span> <span m="2129880">pathology,</span>
  <span m="2130420">where</span> <span m="2130600">sort</span> <span m="2130810">of</span>
  <span m="2131110">80%</span> <span m="2131320">is not</span> <span m="2131890">good</span>
  <span m="2132040">enough.</span> <span m="2132320">We</span> <span m="2132420">want
  to</span> <span m="2132460">get</span> <span m="2132580">as</span> <span m="2132700">close</span>
  <span m="2132940">to</span> <span m="2133030">100%</span> <span m="2135010">as</span>
  <span m="2135160">possible.</span></p><p><span m="2137640">And</span> <span m="2137660">that's</span>
  <span m="2137870">one</span> <span m="2138140">sort</span> <span m="2138380">of</span>
  <span m="2138530">diagnostic</span> <span m="2139280">application.</span> <span
  m="2139850">The</span> <span m="2139910">last,</span> <span m="2140540">or</span>
  <span m="2140960">one</span> <span m="2141140">of</span> <span m="2141200">the</span>
  <span m="2141260">last</span> <span m="2141440">examples</span> <span m="2141830">I'm</span>
  <span m="2141890">going</span> <span m="2142010">to</span> <span m="2142070">give</span>
  <span m="2142250">has</span> <span m="2142430">to</span> <span m="2142500">do</span>
  <span m="2142550">with</span> <span m="2142670">precision</span> <span m="2143300">immunotherapy,</span>
  <span m="2144020">where</span> <span m="2144140">we're</span> <span m="2144260">not</span>
  <span m="2144410">only</span> <span m="2144590">trying</span> <span m="2144950">to</span>
  <span m="2145640">identify</span> <span m="2146390">what</span> <span m="2146570">the</span>
  <span m="2146660">diagnosis</span> <span m="2147230">is</span> <span m="2147410">but</span>
  <span m="2147590">to actually</span> <span m="2147860">subtype</span> <span m="2148400">patients</span>
  <span m="2149390">to</span> <span m="2149570">predict</span> <span m="2149870">the</span>
  <span m="2149930">right</span> <span m="2150110">treatment.</span> <span m="2151250">And</span>
  <span m="2151370">as</span> <span m="2151490">I</span> <span m="2151790">mentioned</span>
  <span m="2152240">earlier,</span> <span m="2152570">immunotherapy</span> <span m="2152915">is</span>
  <span m="2153260">a</span> <span m="2153350">really</span> <span m="2153830">important</span>
  <span m="2154370">and</span> <span m="2154460">exciting,</span> <span m="2155450">relatively</span>
  <span m="2155960">new</span> <span m="2156260">area</span> <span m="2156470">of</span>
  <span m="2156560">cancer</span> <span m="2156890">therapy,</span> <span m="2157380">which</span>
  <span m="2157400">was</span> <span m="2157520">another</span> <span m="2157850">one</span>
  <span m="2157940">of</span> <span m="2158000">the</span> <span m="2158060">big</span>
  <span m="2158180">advances</span> <span m="2158630">in</span> <span m="2158720">2012.</span></p><p><span
  m="2159770">Around</span> <span m="2159980">the</span> <span m="2160070">same</span>
  <span m="2160280">time</span> <span m="2160620">that</span> <span m="2160970">deep</span>
  <span m="2161180">learning</span> <span m="2161480">came</span> <span m="2161690">out,</span>
  <span m="2162230">the</span> <span m="2162320">first</span> <span m="2162590">studies</span>
  <span m="2163010">came</span> <span m="2163250">out</span> <span m="2163430">showing</span>
  <span m="2164270">that</span> <span m="2164720">targeting</span> <span m="2165320">a</span>
  <span m="2165350">protein</span> <span m="2167315">mostly</span> <span m="2167780">on</span>
  <span m="2167870">tumor</span> <span m="2168110">cells</span> <span m="2168410">but</span>
  <span m="2168530">also</span> <span m="2168680">on</span> <span m="2168770">immune</span>
  <span m="2169010">cells,</span> <span m="2169430">the</span> <span m="2169580">PD-1</span>
  <span m="2170150">or</span> <span m="2170240">the</span> <span m="2170330">PD-L1</span>
  <span m="2170840">protein,</span> <span m="2172010">which</span> <span m="2172280">the</span>
  <span m="2172370">protein's</span> <span m="2172850">job</span> <span m="2173210">when</span>
  <span m="2173360">it's</span> <span m="2173480">on</span> <span m="2173720">is</span>
  <span m="2173810">to</span> <span m="2173930">inhibit</span> <span m="2174320">immune</span>
  <span m="2174560">response.</span></p><p><span m="2175860">But</span> <span m="2175910">in</span>
  <span m="2175970">the</span> <span m="2176060">setting</span> <span m="2176270">of</span>
  <span m="2176360">cancer,</span> <span m="2176840">the</span> <span m="2176960">inhibition</span>
  <span m="2178220">of</span> <span m="2178350">immune</span> <span m="2178550">response</span>
  <span m="2179000">is</span> <span m="2179090">actually</span> <span m="2179420">bad</span>
  <span m="2179720">for</span> <span m="2179840">the</span> <span m="2179900">patient,</span>
  <span m="2180320">because</span> <span m="2180740">the</span> <span m="2180890">immune</span>
  <span m="2181160">system's</span> <span m="2181550">job</span> <span m="2181850">is</span>
  <span m="2181940">to</span> <span m="2182090">really</span> <span m="2182330">try</span>
  <span m="2182540">to</span> <span m="2182660">fight</span> <span m="2182960">off</span>
  <span m="2183140">the</span> <span m="2183230">cancer.</span> <span m="2184230">So</span>
  <span m="2184280">they</span> <span m="2184700">realized</span> <span m="2185120">a</span>
  <span m="2185180">very</span> <span m="2185420">simple</span> <span m="2185720">therapeutic</span>
  <span m="2186140">strategy</span> <span m="2186610">just</span> <span m="2186770">having</span>
  <span m="2186950">an</span> <span m="2187040">antibody</span> <span m="2187640">that</span>
  <span m="2187760">binds</span> <span m="2188240">to</span> <span m="2188330">this</span>
  <span m="2188540">inhibitory</span> <span m="2189200">signal</span> <span m="2190310">can</span>
  <span m="2190580">sort</span> <span m="2190760">of</span> <span m="2190850">unleash</span>
  <span m="2191360">the</span> <span m="2191450">patient's</span> <span m="2191870">own</span>
  <span m="2192020">immune</span> <span m="2192260">system</span> <span m="2192650">to</span>
  <span m="2192770">really</span> <span m="2193190">end</span> <span m="2193340">up</span>
  <span m="2194120">curing</span> <span m="2194780">really</span> <span m="2195110">serious</span>
  <span m="2195470">advanced</span> <span m="2195800">cancers.</span></p><p><span
  m="2196280">And</span> <span m="2196370">that</span> <span m="2196640">image</span>
  <span m="2196940">on</span> <span m="2197030">the</span> <span m="2197120">top</span>
  <span m="2197390">right</span> <span m="2197690">sort</span> <span m="2198050">of</span>
  <span m="2198140">speaks</span> <span m="2198470">to</span> <span m="2198590">that,</span>
  <span m="2199180">where</span> <span m="2199310">this</span> <span m="2199490">patient</span>
  <span m="2200000">had</span> <span m="2200150">a</span> <span m="2200210">very</span>
  <span m="2200480">large</span> <span m="2201890">melanoma.</span> <span m="2203030">And</span>
  <span m="2203150">then</span> <span m="2203300">they</span> <span m="2203420">just</span>
  <span m="2203630">got</span> <span m="2203810">this</span> <span m="2204140">antibody</span>
  <span m="2204740">to</span> <span m="2204860">target,</span> <span m="2205310">to</span>
  <span m="2205430">sort</span> <span m="2205580">of</span> <span m="2206080">invigorate</span>
  <span m="2206630">their</span> <span m="2206720">immune</span> <span m="2206930">system,</span>
  <span m="2207770">and</span> <span m="2207890">then</span> <span m="2208070">the</span>
  <span m="2208340">tumor</span> <span m="2208670">really</span> <span m="2208910">shrunk.</span></p><p><span
  m="2210200">And</span> <span m="2210500">one</span> <span m="2210680">of</span>
  <span m="2210740">the</span> <span m="2210830">big</span> <span m="2211040">biomarkers</span>
  <span m="2211850">for</span> <span m="2212120">assessing</span> <span m="2212600">which</span>
  <span m="2212780">patients</span> <span m="2213170">will</span> <span m="2213260">benefit</span>
  <span m="2213740">from</span> <span m="2213860">these</span> <span m="2214010">therapies</span>
  <span m="2215210">is</span> <span m="2215390">the</span> <span m="2215480">tumor</span>
  <span m="2215810">cell</span> <span m="2216080">or</span> <span m="2216170">the</span>
  <span m="2216260">immune</span> <span m="2216470">cell</span> <span m="2217070">expressing</span>
  <span m="2217820">this</span> <span m="2218000">drug</span> <span m="2218240">target</span>
  <span m="2218630">PD-1</span> <span m="2219350">or</span> <span m="2219470">PD-L1.</span>
  <span m="2220690">And</span> <span m="2220800">the</span> <span m="2220840">one</span>
  <span m="2220970">they</span> <span m="2221060">test</span> <span m="2221420">for</span>
  <span m="2221600">is</span> <span m="2221720">PD-L1,</span> <span m="2222440">which</span>
  <span m="2222590">is</span> <span m="2222710">the</span> <span m="2222800">ligand</span>
  <span m="2223910">for</span> <span m="2224060">the</span> <span m="2224150">PD-1</span>
  <span m="2224570">receptor.</span></p><p><span m="2225990">So</span> <span m="2226130">this</span>
  <span m="2226340">is</span> <span m="2226460">often</span> <span m="2226790">the</span>
  <span m="2226970">key</span> <span m="2227210">piece</span> <span m="2227480">of</span>
  <span m="2227570">data</span> <span m="2227900">used</span> <span m="2228100">to</span>
  <span m="2228170">decide</span> <span m="2228500">who</span> <span m="2228620">gets</span>
  <span m="2228860">these</span> <span m="2229040">therapies.</span> <span m="2229650">And</span>
  <span m="2229750">it</span> <span m="2229850">turns</span> <span m="2230030">out,</span>
  <span m="2230150">pathologists</span> <span m="2230810">are</span> <span m="2230900">pretty</span>
  <span m="2231230">bad</span> <span m="2231620">at</span> <span m="2231710">scoring</span>
  <span m="2232190">this,</span> <span m="2232460">not</span> <span m="2232700">surprisingly,</span>
  <span m="2233490">because</span> <span m="2233570">it's</span> <span m="2233690">very</span>
  <span m="2233870">difficult,</span> <span m="2234145">and</span> <span m="2234420">there's</span>
  <span m="2234470">millions</span> <span m="2234740">of</span> <span m="2234830">cells</span>
  <span m="2236180">potentially</span> <span m="2236660">per</span> <span m="2236840">case.</span>
  <span m="2237870">And</span> <span m="2237890">they</span> <span m="2237980">show</span>
  <span m="2238240">an</span> <span m="2238380">interobserver</span> <span m="2239210">agreement</span>
  <span m="2239720">of</span> <span m="2239780">only</span> <span m="2239990">0.86</span>
  <span m="2240800">for</span> <span m="2240920">scoring</span> <span m="2241190">on</span>
  <span m="2241310">tumor</span> <span m="2241550">cells,</span> <span m="2241950">which</span>
  <span m="2242030">isn't</span> <span m="2242210">bad,</span> <span m="2242840">but</span>
  <span m="2243050">0.2</span> <span m="2243560">for</span> <span m="2243710">scoring</span>
  <span m="2244000">it</span> <span m="2244040">on</span> <span m="2244130">immune</span>
  <span m="2244340">cells,</span> <span m="2245280">which</span> <span m="2245360">is</span>
  <span m="2245450">super</span> <span m="2245780">important.</span></p><p><span m="2247260">So</span>
  <span m="2247310">this</span> <span m="2247490">is</span> <span m="2247570">a</span>
  <span m="2247640">drug</span> <span m="2247910">target.</span> <span m="2248690">We're</span>
  <span m="2248780">trying</span> <span m="2248960">to</span> <span m="2249050">measure</span>
  <span m="2249440">to</span> <span m="2249530">see</span> <span m="2249680">which</span>
  <span m="2249830">patients</span> <span m="2250250">might</span> <span m="2250430">get</span>
  <span m="2250700">this</span> <span m="2250910">life-saving</span> <span m="2252440">therapy,</span>
  <span m="2253460">but</span> <span m="2253610">the</span> <span m="2253700">diagnostic</span>
  <span m="2254330">we</span> <span m="2254450">have</span> <span m="2254660">is</span>
  <span m="2254750">super</span> <span m="2255080">hard</span> <span m="2255320">to</span>
  <span m="2255440">interpret.</span> <span m="2257360">And</span> <span m="2257540">some</span>
  <span m="2257780">studies,</span> <span m="2258170">for</span> <span m="2258260">this</span>
  <span m="2258410">reason,</span> <span m="2258740">have</span> <span m="2258860">shown</span>
  <span m="2259160">sort</span> <span m="2259310">of</span> <span m="2259400">mixed</span>
  <span m="2259700">results</span> <span m="2260270">about</span> <span m="2260690">how</span>
  <span m="2260900">valuable</span> <span m="2261290">it</span> <span m="2261380">is.</span>
  <span m="2261500">In</span> <span m="2261590">some</span> <span m="2261770">cases,</span>
  <span m="2262130">it</span> <span m="2262220">appears</span> <span m="2262490">valuable.</span>
  <span m="2263810">In</span> <span m="2263990">other</span> <span m="2264200">cases,</span>
  <span m="2264500">it</span> <span m="2264590">appears</span> <span m="2264890">it's</span>
  <span m="2265040">not.</span></p><p><span m="2266300">So</span> <span m="2266480">we</span>
  <span m="2266540">want</span> <span m="2266690">to</span> <span m="2266750">see</span>
  <span m="2266990">would</span> <span m="2267470">this</span> <span m="2267650">be</span>
  <span m="2267770">a</span> <span m="2267830">good</span> <span m="2268040">example</span>
  <span m="2268460">of</span> <span m="2268550">where</span> <span m="2268670">we</span>
  <span m="2268760">can</span> <span m="2268880">use</span> <span m="2269540">machine</span>
  <span m="2269900">learning?</span> <span m="2271220">And</span> <span m="2271850">for</span>
  <span m="2272120">this</span> <span m="2272690">type</span> <span m="2272960">of</span>
  <span m="2273050">application,</span> <span m="2274050">this</span> <span m="2274130">is</span>
  <span m="2274280">really</span> <span m="2274520">hard,</span> <span m="2274970">and</span>
  <span m="2275330">we</span> <span m="2275420">want</span> <span m="2275570">to</span>
  <span m="2275630">be</span> <span m="2275750">able</span> <span m="2275870">to</span>
  <span m="2275930">apply</span> <span m="2276290">it</span> <span m="2276380">across</span>
  <span m="2276740">not</span> <span m="2276890">just</span> <span m="2277040">one</span>
  <span m="2277220">cancer</span> <span m="2277640">but</span> <span m="2277850">20</span>
  <span m="2278090">different</span> <span m="2278330">cancers.</span></p><p><span
  m="2279330">So</span> <span m="2279410">we</span> <span m="2279500">built</span>
  <span m="2279720">a</span> <span m="2279800">system</span> <span m="2280400">at</span>
  <span m="2280460">PathAI</span> <span m="2280970">for</span> <span m="2281150">generating</span>
  <span m="2281690">lots</span> <span m="2282080">of</span> <span m="2282170">training</span>
  <span m="2282500">data</span> <span m="2282830">at</span> <span m="2282950">scale.</span>
  <span m="2283910">And</span> <span m="2284000">that's</span> <span m="2284150">something</span>
  <span m="2284420">that</span> <span m="2284510">a</span> <span m="2284570">competition</span>
  <span m="2285200">just</span> <span m="2285800">won't</span> <span m="2286010">get</span>
  <span m="2286250">you.</span> <span m="2286400">Like</span> <span m="2286550">that</span>
  <span m="2286880">competition</span> <span m="2287390">example</span> <span m="2287810">had</span>
  <span m="2288080">300</span> <span m="2288470">slides.</span> <span m="2289550">Once</span>
  <span m="2289790">a</span> <span m="2289850">year,</span> <span m="2290000">they</span>
  <span m="2290150">do</span> <span m="2290330">it.</span> <span m="2290720">But</span>
  <span m="2290870">we</span> <span m="2290960">want</span> <span m="2291030">to</span>
  <span m="2291110">be</span> <span m="2291170">able</span> <span m="2291290">to</span>
  <span m="2291380">build</span> <span m="2291590">these</span> <span m="2291770">models</span>
  <span m="2292580">every</span> <span m="2292910">week</span> <span m="2293180">or</span>
  <span m="2293270">something.</span></p><p><span m="2293660">So</span> <span m="2294170">now,</span>
  <span m="2294380">we</span> <span m="2294470">have</span> <span m="2294650">something</span>
  <span m="2295220">500</span> <span m="2295810">pathologists</span> <span m="2296410">signed</span>
  <span m="2296600">into</span> <span m="2296750">our</span> <span m="2296840">system</span>
  <span m="2297590">that</span> <span m="2297680">we</span> <span m="2297770">can</span>
  <span m="2297920">use</span> <span m="2298160">to</span> <span m="2298280">label</span>
  <span m="2298640">lots</span> <span m="2298910">of</span> <span m="2298970">pathology</span>
  <span m="2299420">data</span> <span m="2299660">for</span> <span m="2299870">us</span>
  <span m="2300720">and</span> <span m="2300890">to</span> <span m="2301010">really</span>
  <span m="2301220">build</span> <span m="2301460">these</span> <span m="2301640">models</span>
  <span m="2302120">quickly</span> <span m="2302600">and</span> <span m="2302780">really</span>
  <span m="2303020">high</span> <span m="2303170">quality.</span> <span m="2303590">So</span>
  <span m="2303710">now</span> <span m="2303830">we</span> <span m="2303890">have</span>
  <span m="2304070">something like</span> <span m="2304280">over</span> <span m="2304730">2</span>
  <span m="2304930">and</span> <span m="2305130">1/2</span> <span m="2305330">million</span>
  <span m="2306380">annotations</span> <span m="2306950">in</span> <span m="2307040">the</span>
  <span m="2307100">system.</span> <span m="2308170">And</span> <span m="2308210">that</span>
  <span m="2308360">allows</span> <span m="2308720">us</span> <span m="2308840">to</span>
  <span m="2308960">build</span> <span m="2309440">tissue</span> <span m="2309830">region</span>
  <span m="2310190">models.</span></p><p><span m="2310670">And</span> <span m="2310760">this</span>
  <span m="2310880">is</span> <span m="2311000">immunohistochemistry</span> <span
  m="2312210">in</span> <span m="2312380">a</span> <span m="2312410">cancer,</span>
  <span m="2313470">where</span> <span m="2313700">we've</span> <span m="2313790">trained</span>
  <span m="2314030">a</span> <span m="2314090">model</span> <span m="2314360">to</span>
  <span m="2314540">identify</span> <span m="2315020">all</span> <span m="2315170">of</span>
  <span m="2315260">the</span> <span m="2315350">cancer</span> <span m="2315680">epithelium</span>
  <span m="2316130">in</span> <span m="2316220">red,</span> <span m="2316520">the</span>
  <span m="2316610">cancer</span> <span m="2317010">stroma</span> <span m="2317270">in</span>
  <span m="2317390">green.</span> <span m="2318420">So</span> <span m="2318470">now</span>
  <span m="2318620">we</span> <span m="2318740">know</span> <span m="2318980">where</span>
  <span m="2319190">the</span> <span m="2319310">protein</span> <span m="2319820">is</span>
  <span m="2319940">being</span> <span m="2320090">expressed,</span> <span m="2321370">in</span>
  <span m="2321470">the</span> <span m="2321560">epithelium</span> <span m="2322010">or</span>
  <span m="2322070">in</span> <span m="2322130">the</span> <span m="2322190">stroma.</span></p><p><span
  m="2323690">And</span> <span m="2323780">then</span> <span m="2323900">we've</span>
  <span m="2324080">also</span> <span m="2324350">trained</span> <span m="2325610">cellular</span>
  <span m="2326120">classification.</span> <span m="2326840">So</span> <span m="2326990">now,</span>
  <span m="2327140">for</span> <span m="2327290">every</span> <span m="2327500">single</span>
  <span m="2327770">cell,</span> <span m="2328220">we</span> <span m="2328310">classify</span>
  <span m="2328760">it</span> <span m="2328820">as</span> <span m="2328940">a</span>
  <span m="2329000">cell</span> <span m="2329240">type.</span> <span m="2329700">Is</span>
  <span m="2329720">it</span> <span m="2329780">a</span> <span m="2329840">cancer</span>
  <span m="2330200">cell</span> <span m="2330620">or</span> <span m="2330750">a</span>
  <span m="2330770">fibroblast</span> <span m="2331490">or</span> <span m="2331580">a
  macrophage</span> <span m="2332660">or a</span> <span m="2332810">lymphocyte?</span>
  <span m="2333410">And</span> <span m="2333530">is</span> <span m="2333650">it</span>
  <span m="2333710">expressing</span> <span m="2334160">the</span> <span m="2334250">protein,</span>
  <span m="2335120">based</span> <span m="2335360">on</span> <span m="2335480">how</span>
  <span m="2335630">brown</span> <span m="2335960">it</span> <span m="2336080">is?</span>
  <span m="2336750">So</span> <span m="2336840">while</span> <span m="2336980">pathologists</span>
  <span m="2337580">will</span> <span m="2337670">try</span> <span m="2337790">to</span>
  <span m="2337910">make</span> <span m="2338060">some</span> <span m="2338300">estimate</span>
  <span m="2338780">across</span> <span m="2339080">the</span> <span m="2339170">whole</span>
  <span m="2339350">slide,</span> <span m="2339870">we</span> <span m="2339970">can</span>
  <span m="2340070">actually</span> <span m="2340160">compute</span> <span m="2340520">for</span>
  <span m="2340670">every</span> <span m="2340910">cell</span> <span m="2341300">and</span>
  <span m="2341390">then</span> <span m="2341510">compute</span> <span m="2341860">exact</span>
  <span m="2342320">statistics</span> <span m="2343040">about</span> <span m="2343220">which</span>
  <span m="2343430">cells</span> <span m="2343760">are</span> <span m="2343790">expressing</span>
  <span m="2344210">this</span> <span m="2344330">protein</span> <span m="2345080">and</span>
  <span m="2345200">which</span> <span m="2345350">patients</span> <span m="2345740">might</span>
  <span m="2345920">be</span> <span m="2346010">the</span> <span m="2346070">best</span>
  <span m="2346760">candidates</span> <span m="2347300">for</span> <span m="2347540">therapy.</span></p><p><span
  m="2353130">And</span> <span m="2353280">then</span> <span m="2353430">the</span>
  <span m="2353490">question</span> <span m="2354000">is,</span> <span m="2355700">can</span>
  <span m="2356640">we</span> <span m="2357990">identify</span> <span m="2358650">additional</span>
  <span m="2359130">things</span> <span m="2359370">beyond</span> <span m="2359760">just</span>
  <span m="2359940">PD-L1</span> <span m="2360810">protein</span> <span m="2361140">expression</span>
  <span m="2361620">that's</span> <span m="2361770">predictive</span> <span m="2362160">of</span>
  <span m="2362250">response</span> <span m="2362640">to</span> <span m="2362760">immunotherapy?</span>
  <span m="2363780">And</span> <span m="2363870">we've</span> <span m="2363990">developed</span>
  <span m="2364320">some</span> <span m="2364470">machine</span> <span m="2364770">learning</span>
  <span m="2365010">approaches</span> <span m="2366420">for</span> <span m="2366600">doing</span>
  <span m="2366960">that.</span></p><p><span m="2369220">And</span> <span m="2369700">part</span>
  <span m="2369940">of</span> <span m="2370030">it's</span> <span m="2370180">doing</span>
  <span m="2370420">things</span> <span m="2370600">like</span> <span m="2370890">quantitating</span>
  <span m="2372010">different</span> <span m="2372340">cells</span> <span m="2372850">and</span>
  <span m="2372970">regions</span> <span m="2373360">on</span> <span m="2373540">H
  and E</span> <span m="2373910">images,</span> <span m="2374320">which</span> <span
  m="2374470">currently</span> <span m="2374800">aren't</span> <span m="2374980">used</span>
  <span m="2375220">at</span> <span m="2375310">all</span> <span m="2375460">in</span>
  <span m="2375580">patient</span> <span m="2375910">subtyping.</span> <span m="2376720">But</span>
  <span m="2376870">we</span> <span m="2376960">can</span> <span m="2377050">do</span>
  <span m="2377110">analyses</span> <span m="2377680">to</span> <span m="2377800">extract</span>
  <span m="2378130">new</span> <span m="2378310">features</span> <span m="2378760">here</span>
  <span m="2378940">and</span> <span m="2379060">to ask,</span> <span m="2379840">even</span>
  <span m="2380110">though</span> <span m="2380260">nothing's</span> <span m="2380590">known</span>
  <span m="2380860">about</span> <span m="2381070">these</span> <span m="2381250">images</span>
  <span m="2381670">and</span> <span m="2382060">immunotherapy</span> <span m="2382660">response,</span>
  <span m="2383500">can</span> <span m="2383650">we</span> <span m="2383740">discover</span>
  <span m="2384880">new</span> <span m="2385090">features</span> <span m="2385570">here?</span></p><p><span
  m="2387360">And</span> <span m="2387490">this</span> <span m="2387610">would</span>
  <span m="2387700">be</span> <span m="2387760">an</span> <span m="2387820">example</span>
  <span m="2388420">routinely</span> <span m="2388990">of</span> <span m="2389110">the</span>
  <span m="2389200">types</span> <span m="2389560">of</span> <span m="2389650">features</span>
  <span m="2390070">we</span> <span m="2390130">can</span> <span m="2390250">quantify</span>
  <span m="2390850">now</span> <span m="2391360">using</span> <span m="2391600">deep</span>
  <span m="2391840">learning</span> <span m="2392320">to</span> <span m="2392470">extract</span>
  <span m="2392920">these</span> <span m="2393130">features</span> <span m="2394290">on</span>
  <span m="2394490">any</span> <span m="2394780">case.</span> <span m="2395290">And</span>
  <span m="2395380">this</span> <span m="2395530">is</span> <span m="2395620">sort</span>
  <span m="2395770">of</span> <span m="2395830">like</span> <span m="2395980">every</span>
  <span m="2396250">sort</span> <span m="2396430">of</span> <span m="2396520">pathologic</span>
  <span m="2397690">characteristic</span> <span m="2398500">you</span> <span m="2398560">can</span>
  <span m="2398680">sort</span> <span m="2398860">of</span> <span m="2398920">imagine.</span>
  <span m="2399610">And</span> <span m="2399730">then</span> <span m="2399850">we</span>
  <span m="2399940">correlate</span> <span m="2400390">these</span> <span m="2400570">with</span>
  <span m="2400660">drug</span> <span m="2400870">response</span> <span m="2401620">and</span>
  <span m="2401710">can</span> <span m="2401830">use</span> <span m="2402070">this</span>
  <span m="2402220">as</span> <span m="2402370">a</span> <span m="2402430">discovery</span>
  <span m="2402970">tool</span> <span m="2403270">for</span> <span m="2403420">identifying</span>
  <span m="2403930">new</span> <span m="2404140">aspects</span> <span m="2404620">of</span>
  <span m="2404680">pathology</span> <span m="2405250">predictive</span> <span m="2405760">of</span>
  <span m="2406150">which</span> <span m="2406360">patients</span> <span m="2406680">will</span>
  <span m="2406740">respond</span> <span m="2407080">best.</span></p><p><span m="2408550">And</span>
  <span m="2408670">then</span> <span m="2408760">we</span> <span m="2408850">can</span>
  <span m="2408970">combine</span> <span m="2409510">these</span> <span m="2409720">features</span>
  <span m="2410110">into</span> <span m="2410290">models.</span> <span m="2410870">This</span>
  <span m="2410920">is</span> <span m="2411010">sort</span> <span m="2411220">of</span>
  <span m="2411310">a</span> <span m="2411370">ridiculous</span> <span m="2411850">example</span>
  <span m="2412300">because</span> <span m="2412510">they're</span> <span m="2412630">so</span>
  <span m="2412780">different.</span> <span m="2413530">But</span> <span m="2413740">this</span>
  <span m="2413950">would</span> <span m="2414070">be</span> <span m="2414190">one</span>
  <span m="2414400">example</span> <span m="2415450">where</span> <span m="2416320">the</span>
  <span m="2416500">output</span> <span m="2416830">of</span> <span m="2416920">the</span>
  <span m="2417010">model,</span> <span m="2417920">and</span> <span m="2418020">this</span>
  <span m="2418060">is</span> <span m="2418180">totally</span> <span m="2418600">fake</span>
  <span m="2418900">data</span> <span m="2419300">but</span> <span m="2419410">I</span>
  <span m="2419470">think</span> <span m="2419590">it's</span> <span m="2419650">just</span>
  <span m="2419990">to</span> <span m="2420080">get</span> <span m="2420160">to</span>
  <span m="2420250">the</span> <span m="2420310">point.</span> <span m="2421270">Is</span>
  <span m="2421630">here,</span> <span m="2421810">the</span> <span m="2421900">color</span>
  <span m="2422320">indicates</span> <span m="2423010">the</span> <span m="2423130">treatment,</span>
  <span m="2423730">where</span> <span m="2423880">green</span> <span m="2424240">would</span>
  <span m="2424360">be</span> <span m="2424480">the</span> <span m="2424570">immunotherapy,</span>
  <span m="2425800">red</span> <span m="2426280">would</span> <span m="2426490">be</span>
  <span m="2426940">the</span> <span m="2428710">traditional</span> <span m="2429250">therapy,</span>
  <span m="2430090">and</span> <span m="2430210">the</span> <span m="2430270">goal</span>
  <span m="2430660">is</span> <span m="2430870">to</span> <span m="2431020">build</span>
  <span m="2431410">a</span> <span m="2431470">model</span> <span m="2431860">to</span>
  <span m="2432010">predict</span> <span m="2432370">which</span> <span m="2432640">patients</span>
  <span m="2433000">actually</span> <span m="2433330">benefit</span> <span m="2433690">from</span>
  <span m="2433840">the</span> <span m="2433900">therapy.</span></p><p><span m="2434750">So</span>
  <span m="2434770">this</span> <span m="2434890">may</span> <span m="2435040">be</span>
  <span m="2435130">an</span> <span m="2435220">easy</span> <span m="2435460">question,</span>
  <span m="2435980">but</span> <span m="2436000">what</span> <span m="2436090">do</span>
  <span m="2436150">you</span> <span m="2436210">think,</span> <span m="2436630">if</span>
  <span m="2436780">the</span> <span m="2436870">model's</span> <span m="2437230">working,</span>
  <span m="2437950">what</span> <span m="2438070">would</span> <span m="2438160">the</span>
  <span m="2438250">title</span> <span m="2438670">of</span> <span m="2438790">the</span>
  <span m="2438850">graph</span> <span m="2439120">on</span> <span m="2439210">the</span>
  <span m="2439270">right</span> <span m="2439510">be</span> <span m="2439720">versus</span>
  <span m="2440050">the</span> <span m="2440110">graph</span> <span m="2440410">on</span>
  <span m="2440560">the</span> <span m="2440620">left</span> <span m="2441750">if</span>
  <span m="2442090">these</span> <span m="2442300">are</span> <span m="2442360">the</span>
  <span m="2442450">ways</span> <span m="2442690">of</span> <span m="2442780">classifying</span>
  <span m="2443530">patients</span> <span m="2443980">with</span> <span m="2444130">our</span>
  <span m="2444220">model,</span> <span m="2445060">and</span> <span m="2445180">the</span>
  <span m="2445240">classifications</span> <span m="2446020">are</span> <span m="2446060">going</span>
  <span m="2446130">to</span> <span m="2446230">be</span> <span m="2446350">responder</span>
  <span m="2447070">class</span> <span m="2447670">or</span> <span m="2447820">non-responder</span>
  <span m="2448540">class?</span> <span m="2450850">And</span> <span m="2451030">the</span>
  <span m="2451120">color</span> <span m="2451600">indicates</span> <span m="2452170">the</span>
  <span m="2452320">drug.</span></p><p><span m="2456450">AUDIENCE:</span> <span m="2456530">The</span>
  <span m="2456610">drug</span> <span m="2457180">works</span> <span m="2457500">or</span>
  <span m="2457973">it doesn't</span> <span m="2458446">work.</span></p><p><span m="2458920">ANDY
  BECK:</span> <span m="2459010">That's</span> <span m="2459280">right</span> <span
  m="2459610">but</span> <span m="2459730">what's</span> <span m="2459970">the</span>
  <span m="2460060">output</span> <span m="2460330">of</span> <span m="2460390">the</span>
  <span m="2460450">model?</span> <span m="2462670">But</span> <span m="2462850">you're</span>
  <span m="2462940">right.</span> <span m="2463150">The</span> <span m="2463300">interpretation</span>
  <span m="2463660">of</span> <span m="2464020">these</span> <span m="2464170">graphs</span>
  <span m="2464480">is</span> <span m="2464620">drug</span> <span m="2464860">works,</span>
  <span m="2465100">drug</span> <span m="2465310">doesn't</span> <span m="2465580">work.</span>
  <span m="2465850">It's</span> <span m="2466000">kind</span> <span m="2466210">of</span>
  <span m="2466300">a</span> <span m="2466360">tricky</span> <span m="2466660">question,</span>
  <span m="2467080">right?</span> <span m="2467920">But</span> <span m="2468520">what</span>
  <span m="2468720">is</span> <span m="2468850">our</span> <span m="2468970">model</span>
  <span m="2469300">trying</span> <span m="2469510">to</span> <span m="2469600">predict?</span></p><p><span
  m="2470620">AUDIENCE:</span> <span m="2470740">Whether</span> <span m="2470860">the</span>
  <span m="2470950">person</span> <span m="2471180">is</span> <span m="2471310">going</span>
  <span m="2471430">to</span> <span m="2471490">die</span> <span m="2471790">or</span>
  <span m="2471850">not?</span> <span m="2472870">It</span> <span m="2472960">looks</span>
  <span m="2473200">like</span> <span m="2473950">likelihood</span> <span m="2474440">of</span>
  <span m="2474610">death</span> <span m="2474940">is</span> <span m="2475210">just</span>
  <span m="2475510">not</span> <span m="2475720">as</span> <span m="2475800">high
  on the</span> <span m="2476250">right.</span></p><p><span m="2477550">ANDY BECK:</span>
  <span m="2477625">I</span> <span m="2477700">think</span> <span m="2477940">the</span>
  <span m="2478090">overall</span> <span m="2478570">likelihood</span> <span m="2479020">is</span>
  <span m="2479140">the</span> <span m="2479230">same</span> <span m="2480070">on</span>
  <span m="2480190">the</span> <span m="2480250">two</span> <span m="2480430">graphs,</span>
  <span m="2480940">right</span> <span m="2481150">versus</span> <span m="2481450">left.</span>
  <span m="2482230">You</span> <span m="2482320">don't</span> <span m="2482440">know</span>
  <span m="2482500">how</span> <span m="2482560">many</span> <span m="2482710">patients</span>
  <span m="2483100">are</span> <span m="2483160">in</span> <span m="2483220">each</span>
  <span m="2483400">arm.</span> <span m="2484060">But</span> <span m="2484180">I</span>
  <span m="2484270">think</span> <span m="2484420">the</span> <span m="2484510">one</span>
  <span m="2484720">piece</span> <span m="2484910">on it--</span> <span m="2485060">so</span>
  <span m="2485200">green</span> <span m="2485590">is</span> <span m="2485770">experimental</span>
  <span m="2486280">treatment.</span> <span m="2486610">Red</span> <span m="2486850">is</span>
  <span m="2486970">conventional</span> <span m="2487480">treatment.</span> <span
  m="2487960">Maybe</span> <span m="2488150">I already</span> <span m="2488290">said</span>
  <span m="2488500">that.</span></p><p><span m="2489070">So</span> <span m="2489640">here,</span>
  <span m="2490490">and</span> <span m="2490630">it's sort</span> <span m="2490840">of</span>
  <span m="2490900">like</span> <span m="2491050">a</span> <span m="2491110">read</span>
  <span m="2491290">my</span> <span m="2491410">mind</span> <span m="2491620">type</span>
  <span m="2491770">question,</span> <span m="2492040">but</span> <span m="2492130">here</span>
  <span m="2492250">the</span> <span m="2492370">output</span> <span m="2492730">of</span>
  <span m="2492790">the</span> <span m="2492880">model</span> <span m="2493360">would</span>
  <span m="2493540">be</span> <span m="2494140">responder</span> <span m="2494860">to</span>
  <span m="2495010">the</span> <span m="2495100">drug</span> <span m="2496210">would</span>
  <span m="2496360">be</span> <span m="2496480">the</span> <span m="2496600">right</span>
  <span m="2497260">class</span> <span m="2497650">of</span> <span m="2497740">patients.</span>
  <span m="2498160">And</span> <span m="2498340">the</span> <span m="2498460">left</span>
  <span m="2498750">class</span> <span m="2499010">of</span> <span m="2499080">patients</span>
  <span m="2499390">would</span> <span m="2499480">be</span> <span m="2499600">non-responder</span>
  <span m="2500410">to</span> <span m="2500530">the</span> <span m="2500620">drug.</span>
  <span m="2501490">So</span> <span m="2501640">you're</span> <span m="2501760">not</span>
  <span m="2501880">actually</span> <span m="2502120">saying</span> <span m="2502480">anything</span>
  <span m="2502750">about</span> <span m="2502990">prognosis,</span> <span m="2503770">but</span>
  <span m="2503920">you're</span> <span m="2504040">saying</span> <span m="2504460">that</span>
  <span m="2505480">I'm</span> <span m="2505660">predicting</span> <span m="2506590">that</span>
  <span m="2506800">if</span> <span m="2506950">you're</span> <span m="2507100">in</span>
  <span m="2507190">the</span> <span m="2507310">right</span> <span m="2508150">population</span>
  <span m="2508990">of</span> <span m="2509080">patients,</span> <span m="2509650">you</span>
  <span m="2509830">will</span> <span m="2509920">benefit</span> <span m="2510340">from</span>
  <span m="2510490">the</span> <span m="2510580">blue</span> <span m="2510790">drug.</span></p><p><span
  m="2512020">And</span> <span m="2512170">then</span> <span m="2512440">you</span>
  <span m="2512560">actually</span> <span m="2512800">see</span> <span m="2513040">that</span>
  <span m="2513370">on</span> <span m="2513520">this</span> <span m="2513670">right</span>
  <span m="2513910">population</span> <span m="2514330">of</span> <span m="2514390">patients,</span>
  <span m="2514810">the</span> <span m="2514930">blue</span> <span m="2515590">drug</span>
  <span m="2515950">does</span> <span m="2516190">really</span> <span m="2516370">well.</span>
  <span m="2517060">And</span> <span m="2517180">then</span> <span m="2517300">the</span>
  <span m="2517390">red</span> <span m="2517600">drug</span> <span m="2518020">are</span>
  <span m="2518335">patients</span> <span m="2518650">who</span> <span m="2519040">we</span>
  <span m="2519220">thought--</span> <span m="2519580">we</span> <span m="2519760">predicted</span>
  <span m="2520080">would benefit</span> <span m="2520310">from</span> <span m="2520450">the</span>
  <span m="2520540">drug,</span> <span m="2520810">but</span> <span m="2520900">because</span>
  <span m="2521170">it's</span> <span m="2521290">an</span> <span m="2521380">experiment,</span>
  <span m="2522430">we</span> <span m="2522580">didn't</span> <span m="2522760">give</span>
  <span m="2522940">them</span> <span m="2523060">the</span> <span m="2523150">right</span>
  <span m="2523330">drug.</span> <span m="2523750">And</span> <span m="2523900">in</span>
  <span m="2523990">fact,</span> <span m="2524260">they</span> <span m="2524380">did</span>
  <span m="2524530">a</span> <span m="2524590">whole</span> <span m="2524740">lot</span>
  <span m="2524920">worse.</span> <span m="2526010">Whereas,</span> <span m="2526420">the</span>
  <span m="2526510">one</span> <span m="2526630">on</span> <span m="2526720">the</span>
  <span m="2526780">left,</span> <span m="2527140">we're</span> <span m="2527230">saying</span>
  <span m="2527440">you</span> <span m="2527500">don't</span> <span m="2527650">benefit</span>
  <span m="2527830">from</span> <span m="2527950">the</span> <span m="2528040">drug,</span>
  <span m="2528500">and</span> <span m="2528580">they</span> <span m="2528700">truly</span>
  <span m="2529000">don't</span> <span m="2529180">benefit</span> <span m="2529480">from</span>
  <span m="2529630">the</span> <span m="2529690">drug.</span></p><p><span m="2530510">So</span>
  <span m="2530530">this</span> <span m="2530710">is</span> <span m="2530810">the</span>
  <span m="2530890">way</span> <span m="2530980">of</span> <span m="2531070">using</span>
  <span m="2531280">an</span> <span m="2531370">output</span> <span m="2531670">of</span>
  <span m="2531790">a</span> <span m="2531850">model</span> <span m="2532330">to</span>
  <span m="2532480">predict</span> <span m="2532780">drug</span> <span m="2533080">response</span>
  <span m="2534460">and</span> <span m="2534580">then</span> <span m="2534760">visualizing</span>
  <span m="2535420">whether</span> <span m="2535600">it</span> <span m="2535660">actually</span>
  <span m="2536170">works.</span> <span m="2536620">And</span> <span m="2536710">it's</span>
  <span m="2536800">kind</span> <span m="2536950">of</span> <span m="2537010">like</span>
  <span m="2537130">the</span> <span m="2537190">example</span> <span m="2537550">I</span>
  <span m="2537610">talked</span> <span m="2537940">about</span> <span m="2538120">before,</span>
  <span m="2538420">but</span> <span m="2538540">here's</span> <span m="2539962">a</span>
  <span m="2540340">real</span> <span m="2540580">version</span> <span m="2541000">of</span>
  <span m="2541150">it.</span> <span m="2541720">And</span> <span m="2541870">you</span>
  <span m="2541960">can</span> <span m="2542110">learn</span> <span m="2542410">this</span>
  <span m="2542590">directly</span> <span m="2543040">using</span> <span m="2543550">machine</span>
  <span m="2543880">learning</span> <span m="2544240">to</span> <span m="2544330">try</span>
  <span m="2544510">to</span> <span m="2544630">say,</span> <span m="2545080">I</span>
  <span m="2545170">want</span> <span m="2545290">to</span> <span m="2545350">find</span>
  <span m="2545560">patients</span> <span m="2545950">who</span> <span m="2546010">actually</span>
  <span m="2546220">benefit</span> <span m="2546640">the</span> <span m="2546700">most</span>
  <span m="2547000">from</span> <span m="2547120">a</span> <span m="2547180">drug.</span></p><p><span
  m="2553660">And</span> <span m="2553840">then</span> <span m="2554740">in</span>
  <span m="2554860">terms</span> <span m="2555190">of</span> <span m="2555310">how</span>
  <span m="2555460">do</span> <span m="2555520">we</span> <span m="2555640">validate</span>
  <span m="2556150">our</span> <span m="2556210">models</span> <span m="2556600">are</span>
  <span m="2556660">correct?</span> <span m="2557290">I</span> <span m="2557410">mean,</span>
  <span m="2557620">we</span> <span m="2557710">have</span> <span m="2557800">two</span>
  <span m="2557980">different</span> <span m="2558220">ways.</span> <span m="2558650">One</span>
  <span m="2558850">is</span> <span m="2559090">do</span> <span m="2559300">stuff</span>
  <span m="2559600">like</span> <span m="2559780">that.</span> <span m="2560130">So</span>
  <span m="2560290">we</span> <span m="2560410">build</span> <span m="2560620">a</span>
  <span m="2560650">model</span> <span m="2560980">that</span> <span m="2561130">says,</span>
  <span m="2561780">respond</span> <span m="2562240">to</span> <span m="2562330">drug,</span>
  <span m="2562630">don't</span> <span m="2562810">respond</span> <span m="2563140">to</span>
  <span m="2563260">a</span> <span m="2563290">drug.</span> <span m="2564580">And</span>
  <span m="2564700">then</span> <span m="2564820">we</span> <span m="2564910">plot</span>
  <span m="2565150">the</span> <span m="2565240">Kaplan-Meier</span> <span m="2565690">curves.</span></p><p><span
  m="2566020">If</span> <span m="2566110">it's</span> <span m="2566260">image</span>
  <span m="2566500">analysis</span> <span m="2567670">stuff,</span> <span m="2569476">we</span>
  <span m="2569860">ask</span> <span m="2570130">pathologists</span> <span m="2570680">to</span>
  <span m="2570760">hand</span> <span m="2571000">label.</span> <span m="2572170">Many</span>
  <span m="2572440">cells,</span> <span m="2572920">and we take</span> <span m="2573100">the</span>
  <span m="2573160">consensus</span> <span m="2573760">of</span> <span m="2573850">pathologists</span>
  <span m="2574540">as</span> <span m="2574720">our</span> <span m="2574810">ground</span>
  <span m="2575050">truth</span> <span m="2576460">and</span> <span m="2576580">go</span>
  <span m="2576730">from</span> <span m="2576940">there.</span></p><p><span m="2581340">AUDIENCE:</span>
  <span m="2581430">The</span> <span m="2581520">way</span> <span m="2581730">you're</span>
  <span m="2581910">presenting</span> <span m="2582460">it,</span> <span m="2583215">it</span>
  <span m="2583510">makes</span> <span m="2583800">it</span> <span m="2583890">sound</span>
  <span m="2584160">like</span> <span m="2584400">all</span> <span m="2584650">the</span>
  <span m="2584870">data</span> <span m="2584970">comes</span> <span m="2585390">from</span>
  <span m="2586115">the</span> <span m="2586480">pathology</span> <span m="2587100">images.</span>
  <span m="2588310">But</span> <span m="2588420">in</span> <span m="2588570">reality,</span>
  <span m="2589623">people</span> <span m="2590076">look at</span> <span m="2590530">single</span>
  <span m="2591040">nucleotide</span> <span m="2591820">polymorphisms</span> <span
  m="2592790">or</span> <span m="2593070">gene</span> <span m="2593380">sequences</span>
  <span m="2594250">or</span> <span m="2595650">all</span> <span m="2595860">kinds</span>
  <span m="2596250">of</span> <span m="2597050">clinical</span> <span m="2597570">data</span>
  <span m="2598530">as</span> <span m="2598710">well.</span> <span m="2599410">So</span>
  <span m="2600000">how</span> <span m="2600390">do</span> <span m="2600600">you</span>
  <span m="2601470">get</span> <span m="2601800">those?</span></p><p><span m="2602770">ANDY
  BECK:</span> <span m="2602803">Yeah,</span> <span m="2602836">I</span> <span m="2602870">mean,</span>
  <span m="2602980">the</span> <span m="2603080">beauty</span> <span m="2603300">of</span>
  <span m="2603360">the</span> <span m="2603480">pathology</span> <span m="2603960">data</span>
  <span m="2604230">is</span> <span m="2604380">it's</span> <span m="2604500">always</span>
  <span m="2604920">available.</span> <span m="2606100">So</span> <span m="2606300">that's</span>
  <span m="2606510">why</span> <span m="2606600">a</span> <span m="2606630">lot</span>
  <span m="2606810">of</span> <span m="2606870">the</span> <span m="2606930">stuff</span>
  <span m="2607170">we</span> <span m="2607290">do</span> <span m="2607470">is</span>
  <span m="2607650">focused</span> <span m="2609060">on</span> <span m="2609270">that,</span>
  <span m="2610170">because</span> <span m="2610800">every</span> <span m="2611040">clinical</span>
  <span m="2611280">trial</span> <span m="2611550">patient</span> <span m="2612810">has</span>
  <span m="2614130">treatment</span> <span m="2614490">data,</span> <span m="2614760">outcome</span>
  <span m="2615060">data,</span> <span m="2615270">and</span> <span m="2615360">pathology</span>
  <span m="2615750">images.</span> <span m="2616080">So</span> <span m="2616260">it's</span>
  <span m="2616380">like,</span> <span m="2617070">we</span> <span m="2617190">can</span>
  <span m="2617310">really</span> <span m="2617460">do</span> <span m="2617580">this</span>
  <span m="2617730">at</span> <span m="2617850">scale</span> <span m="2618240">pretty</span>
  <span m="2618540">fast.</span></p><p><span m="2619830">A</span> <span m="2619890">lot</span>
  <span m="2620100">of</span> <span m="2620160">the</span> <span m="2620280">other</span>
  <span m="2620850">stuff</span> <span m="2621420">is</span> <span m="2621840">things</span>
  <span m="2622050">like</span> <span m="2622140">gene</span> <span m="2622320">expression,</span>
  <span m="2623220">many</span> <span m="2623460">people</span> <span m="2623700">are</span>
  <span m="2623760">collecting</span> <span m="2624180">them.</span> <span m="2625840">And</span>
  <span m="2625920">it's</span> <span m="2626070">important</span> <span m="2626700">to</span>
  <span m="2626940">compare</span> <span m="2627390">these</span> <span m="2627630">to</span>
  <span m="2627720">baselines</span> <span m="2628410">or</span> <span m="2628530">to</span>
  <span m="2628620">integrate</span> <span m="2628980">them.</span> <span m="2629280">I</span>
  <span m="2629340">mean,</span> <span m="2629490">two</span> <span m="2629640">things--</span>
  <span m="2629980">one</span> <span m="2630060">is</span> <span m="2630180">compare</span>
  <span m="2630540">to</span> <span m="2631080">it</span> <span m="2631260">as</span>
  <span m="2631380">a</span> <span m="2631440">baseline.</span> <span m="2632160">What</span>
  <span m="2632460">can</span> <span m="2632580">we</span> <span m="2632700">predict</span>
  <span m="2633340">in</span> <span m="2633550">terms</span> <span m="2633810">of</span>
  <span m="2633870">responder,</span> <span m="2634320">non-responder</span> <span
  m="2634950">using</span> <span m="2635220">just</span> <span m="2635370">the</span>
  <span m="2635430">pathology</span> <span m="2635880">images</span> <span m="2636420">versus</span>
  <span m="2637020">using</span> <span m="2637890">just</span> <span m="2638130">gene</span>
  <span m="2638280">expression</span> <span m="2638700">data</span> <span m="2638940">versus</span>
  <span m="2639330">combining</span> <span m="2639780">them?</span></p><p><span m="2640380">And</span>
  <span m="2640470">that</span> <span m="2640590">would</span> <span m="2640710">just</span>
  <span m="2640890">be</span> <span m="2642520">increasing</span> <span m="2643190">the</span>
  <span m="2643500">input</span> <span m="2643800">feature</span> <span m="2644130">space.</span>
  <span m="2644850">Part</span> <span m="2645090">of</span> <span m="2645150">the</span>
  <span m="2645210">input</span> <span m="2645420">feature</span> <span m="2645690">space</span>
  <span m="2645930">comes</span> <span m="2646120">from</span> <span m="2646240">the</span>
  <span m="2646320">images.</span> <span m="2646710">Part</span> <span m="2646950">of</span>
  <span m="2647040">it</span> <span m="2647100">comes</span> <span m="2647370">from</span>
  <span m="2647970">gene</span> <span m="2648120">expression</span> <span m="2648540">data.</span>
  <span m="2648780">Then</span> <span m="2648930">you use</span> <span m="2649110">machine</span>
  <span m="2649380">learning</span> <span m="2649650">to</span> <span m="2649740">focus</span>
  <span m="2650160">on</span> <span m="2650250">the</span> <span m="2650340">most</span>
  <span m="2650550">important</span> <span m="2650970">characteristics</span> <span
  m="2652170">and</span> <span m="2652290">predict</span> <span m="2653310">outcome.</span></p><p><span
  m="2654120">And</span> <span m="2654240">the</span> <span m="2654330">other</span>
  <span m="2654570">is</span> <span m="2654690">if</span> <span m="2654780">you</span>
  <span m="2654900">want</span> <span m="2655080">to</span> <span m="2655140">sort</span>
  <span m="2655320">of</span> <span m="2655380">prioritize.</span> <span m="2656970">Use</span>
  <span m="2657480">pathology</span> <span m="2657960">as</span> <span m="2658050">a</span>
  <span m="2658110">baseline</span> <span m="2658590">because</span> <span m="2658750">it's
  available</span> <span m="2659040">on</span> <span m="2659160">everyone.</span>
  <span m="2660100">But</span> <span m="2660180">then</span> <span m="2660540">an</span>
  <span m="2660630">adjuvant</span> <span m="2661020">test</span> <span m="2661290">that</span>
  <span m="2661380">costs</span> <span m="2661740">another</span> <span m="2662640">$1,000</span>
  <span m="2663480">and</span> <span m="2663570">might</span> <span m="2663750">take</span>
  <span m="2663990">another</span> <span m="2664290">two</span> <span m="2664470">weeks,</span>
  <span m="2665250">how</span> <span m="2665370">much</span> <span m="2665520">does</span>
  <span m="2665640">that</span> <span m="2665850">add</span> <span m="2666030">to</span>
  <span m="2666120">the</span> <span m="2666210">prediction?</span> <span m="2668370">And</span>
  <span m="2668550">that</span> <span m="2668700">would</span> <span m="2668820">be</span>
  <span m="2668910">another</span> <span m="2669240">way.</span></p><p><span m="2669390">So</span>
  <span m="2669480">I</span> <span m="2669540">think</span> <span m="2669660">it</span>
  <span m="2669750">is</span> <span m="2669900">important,</span> <span m="2670410">but</span>
  <span m="2671130">a</span> <span m="2671190">lot</span> <span m="2671430">of</span>
  <span m="2671550">our</span> <span m="2671850">technology</span> <span m="2672420">to</span>
  <span m="2672520">developing</span> <span m="2672720">our</span> <span m="2672780">platform</span>
  <span m="2673260">is</span> <span m="2673440">focused</span> <span m="2673860">around</span>
  <span m="2674040">how</span> <span m="2674130">do</span> <span m="2674190">we</span>
  <span m="2674280">most</span> <span m="2674490">effectively</span> <span m="2674910">use</span>
  <span m="2675540">pathology</span> <span m="2675810">and</span> <span m="2676080">can</span>
  <span m="2676410">certainly</span> <span m="2676530">add</span> <span m="2676740">in</span>
  <span m="2677970">gene</span> <span m="2678180">expression date.</span> <span m="2678650">I'm</span>
  <span m="2678700">actually</span> <span m="2678870">going to</span> <span m="2678960">talk</span>
  <span m="2679170">about</span> <span m="2679380">that</span> <span m="2679590">next--</span>
  <span m="2680010">one</span> <span m="2680220">way</span> <span m="2680340">of</span>
  <span m="2680430">doing</span> <span m="2680700">it.</span> <span m="2681300">Because</span>
  <span m="2681480">it's</span> <span m="2681600">a</span> <span m="2681660">very</span>
  <span m="2681870">natural</span> <span m="2682290">synergy,</span> <span m="2682740">because</span>
  <span m="2682890">they</span> <span m="2683010">tell</span> <span m="2683190">you</span>
  <span m="2683280">very</span> <span m="2683460">different</span> <span m="2683700">things.</span></p><p><span
  m="2687250">So</span> <span m="2687870">here's</span> <span m="2688080">one</span>
  <span m="2688200">example</span> <span m="2688530">of</span> <span m="2688650">integrating,</span>
  <span m="2689250">just</span> <span m="2689610">kind</span> <span m="2689820">of</span>
  <span m="2689910">relative to</span> <span m="2690200">that</span> <span m="2690300">question,</span>
  <span m="2690600">gene</span> <span m="2690750">expression</span> <span m="2691170">data</span>
  <span m="2691440">with</span> <span m="2691590">image</span> <span m="2691920">data,</span>
  <span m="2692820">where</span> <span m="2693210">the</span> <span m="2693330">cancer</span>
  <span m="2693660">genome</span> <span m="2693990">analysis,</span> <span m="2694320">and</span>
  <span m="2694410">this</span> <span m="2694530">is</span> <span m="2694620">all</span>
  <span m="2694800">public.</span> <span m="2695280">So</span> <span m="2695460">they</span>
  <span m="2695580">have</span> <span m="2695730">pathology</span> <span m="2696270">images,</span>
  <span m="2696840">RNA</span> <span m="2697260">data,</span> <span m="2698380">clinical</span>
  <span m="2698640">outcomes.</span> <span m="2699090">They</span> <span m="2699210">don't
  have</span> <span m="2699330">the</span> <span m="2699420">greatest</span> <span
  m="2699690">treatment</span> <span m="2699990">data,</span> <span m="2700620">but</span>
  <span m="2700710">it's</span> <span m="2700830">a</span> <span m="2700860">great</span>
  <span m="2701070">place</span> <span m="2701280">for</span> <span m="2701400">method</span>
  <span m="2701700">development</span> <span m="2702210">for</span> <span m="2702360">sort</span>
  <span m="2702570">of</span> <span m="2704020">ML</span> <span m="2704510">in</span>
  <span m="2704700">cancer,</span> <span m="2705630">including</span> <span m="2706110">pathology-type</span>
  <span m="2706950">analyses.</span></p><p><span m="2707850">So</span> <span m="2707970">this</span>
  <span m="2708090">is</span> <span m="2708200">a</span> <span m="2708270">case</span>
  <span m="2708510">of</span> <span m="2708600">melanoma.</span> <span m="2709470">We've</span>
  <span m="2709620">trained</span> <span m="2709860">a</span> <span m="2709920">model</span>
  <span m="2710220">to</span> <span m="2710340">identify</span> <span m="2710700">cancer</span>
  <span m="2711240">and</span> <span m="2711370">stroma</span> <span m="2712140">and</span>
  <span m="2712260">all</span> <span m="2712350">the</span> <span m="2712440">different</span>
  <span m="2712680">cells.</span> <span m="2713950">And</span> <span m="2714050">then</span>
  <span m="2714060">we</span> <span m="2714120">extract,</span> <span m="2714780">as</span>
  <span m="2714930">you</span> <span m="2715020">saw,</span> <span m="2715410">sort</span>
  <span m="2715620">of</span> <span m="2715710">hundreds</span> <span m="2716070">of</span>
  <span m="2716130">features.</span> <span m="2716980">And</span> <span m="2717000">then</span>
  <span m="2717090">we</span> <span m="2717180">can</span> <span m="2717330">rank</span>
  <span m="2717630">the</span> <span m="2717750">features</span> <span m="2718290">here</span>
  <span m="2719820">by</span> <span m="2720030">their</span> <span m="2720150">correlation</span>
  <span m="2720810">with</span> <span m="2720930">survival.</span></p><p><span m="2721960">So</span>
  <span m="2721980">now</span> <span m="2722190">we're</span> <span m="2722280">mapping</span>
  <span m="2722730">from</span> <span m="2722940">pathology</span> <span m="2723570">images</span>
  <span m="2724110">to</span> <span m="2724650">outcome</span> <span m="2725070">data</span>
  <span m="2725850">and</span> <span m="2725970">we</span> <span m="2726120">find</span>
  <span m="2726660">just</span> <span m="2726900">in a totally</span> <span m="2727290">data-driven</span>
  <span m="2727740">way</span> <span m="2727890">that</span> <span m="2728040">there's</span>
  <span m="2728370">some</span> <span m="2728640">small</span> <span m="2728910">set</span>
  <span m="2729210">of</span> <span m="2729780">15</span> <span m="2730230">features</span>
  <span m="2730620">or</span> <span m="2730710">so</span> <span m="2730950">highly</span>
  <span m="2731280">associated</span> <span m="2731500">with</span> <span m="2731710">survival.</span>
  <span m="2732270">The</span> <span m="2732360">rest</span> <span m="2732660">aren't.</span>
  <span m="2733510">And</span> <span m="2733650">the</span> <span m="2733770">top</span>
  <span m="2734130">ranking</span> <span m="2734460">one</span> <span m="2734640">is</span>
  <span m="2735105">an</span> <span m="2735390">immune</span> <span m="2735870">cell</span>
  <span m="2736500">feature,</span> <span m="2736920">increased</span> <span m="2737340">area</span>
  <span m="2737550">of stroma</span> <span m="2737910">plasma</span> <span m="2738300">cells</span>
  <span m="2738630">that</span> <span m="2738750">are</span> <span m="2738810">associated
  with</span> <span m="2739230">increased</span> <span m="2739560">survival.</span>
  <span m="2740500">And</span> <span m="2740600">this</span> <span m="2740640">was</span>
  <span m="2740760">an</span> <span m="2740850">analysis</span> <span m="2741360">that</span>
  <span m="2741480">was</span> <span m="2741600">really</span> <span m="2741810">just</span>
  <span m="2741990">linking</span> <span m="2742320">the</span> <span m="2742410">images</span>
  <span m="2742740">with</span> <span m="2742860">outcome.</span></p><p><span m="2743970">And</span>
  <span m="2744090">then</span> <span m="2744510">we</span> <span m="2744660">can</span>
  <span m="2744810">ask,</span> <span m="2745040">well, what</span> <span m="2745250">are</span>
  <span m="2745320">the</span> <span m="2745410">genes</span> <span m="2746370">underlying</span>
  <span m="2747060">this</span> <span m="2747300">pathology?</span> <span m="2748050">So</span>
  <span m="2748230">pathology</span> <span m="2748710">is</span> <span m="2748860">telling</span>
  <span m="2749100">you</span> <span m="2749190">about</span> <span m="2749460">cells</span>
  <span m="2750030">and</span> <span m="2750120">tissues.</span> <span m="2750990">RNAs</span>
  <span m="2751590">are</span> <span m="2751680">telling</span> <span m="2751950">you</span>
  <span m="2752040">about</span> <span m="2752400">the</span> <span m="2752640">actual</span>
  <span m="2752940">transcriptional</span> <span m="2753570">landscape</span> <span
  m="2754110">of</span> <span m="2754200">what's</span> <span m="2754530">going</span>
  <span m="2754860">on</span> <span m="2755040">underneath.</span> <span m="2757180">And</span>
  <span m="2757200">then</span> <span m="2757320">we</span> <span m="2757440">can</span>
  <span m="2757590">rank</span> <span m="2758280">all</span> <span m="2758460">the</span>
  <span m="2758550">genes</span> <span m="2758790">in</span> <span m="2758880">the</span>
  <span m="2758940">genome</span> <span m="2759300">just</span> <span m="2759450">by</span>
  <span m="2759570">their</span> <span m="2759660">correlation</span> <span m="2760320">with</span>
  <span m="2760470">this</span> <span m="2760650">quantitative</span> <span m="2761220">phenotype</span>
  <span m="2761700">we're</span> <span m="2761760">measuring</span> <span m="2762120">on</span>
  <span m="2762210">the</span> <span m="2762270">pathology</span> <span m="2762690">images.</span>
  <span m="2762990">And</span> <span m="2763080">here are</span> <span m="2763260">all</span>
  <span m="2763380">the</span> <span m="2763470">genes,</span> <span m="2763770">ranked</span>
  <span m="2764040">from</span> <span m="2764190">0</span> <span m="2764370">to</span>
  <span m="2764460">20,000.</span> <span m="2765420">And</span> <span m="2765510">again,</span>
  <span m="2765750">we</span> <span m="2765840">see</span> <span m="2766050">a</span>
  <span m="2766110">small</span> <span m="2767190">set</span> <span m="2767550">that</span>
  <span m="2767670">we're</span> <span m="2767760">thresholding</span> <span m="2768400">at</span>
  <span m="2768510">a</span> <span m="2768570">correlation</span> <span m="2769170">of</span>
  <span m="2769530">0.4,</span> <span m="2770970">strongly</span> <span m="2771450">associated</span>
  <span m="2771990">with</span> <span m="2772350">the</span> <span m="2772590">pathologic</span>
  <span m="2773190">phenotype</span> <span m="2773620">we're</span> <span m="2773700">measuring.</span></p><p><span
  m="2774720">And</span> <span m="2774870">then</span> <span m="2775050">we</span>
  <span m="2775200">sort</span> <span m="2775440">of</span> <span m="2775710">discover</span>
  <span m="2776670">these</span> <span m="2776970">sets</span> <span m="2777360">of</span>
  <span m="2777450">genes</span> <span m="2778170">that</span> <span m="2778320">are</span>
  <span m="2778410">known</span> <span m="2778830">to</span> <span m="2778950">be</span>
  <span m="2779070">highly</span> <span m="2779430">enriched</span> <span m="2779880">in</span>
  <span m="2779970">immune</span> <span m="2780240">cell</span> <span m="2780480">genes.</span>
  <span m="2781230">Sort</span> <span m="2781470">of</span> <span m="2781530">which</span>
  <span m="2781710">is</span> <span m="2781770">some</span> <span m="2782010">form</span>
  <span m="2782250">of</span> <span m="2782310">validation</span> <span m="2784050">that</span>
  <span m="2784290">we're</span> <span m="2784410">measuring</span> <span m="2784800">what</span>
  <span m="2784920">we</span> <span m="2785040">think</span> <span m="2785220">we're</span>
  <span m="2785340">measuring,</span> <span m="2785760">but</span> <span m="2785910">also</span>
  <span m="2786300">this</span> <span m="2786510">sets</span> <span m="2786990">of</span>
  <span m="2787140">genes</span> <span m="2787710">are</span> <span m="2788280">potentially</span>
  <span m="2788820">new</span> <span m="2788970">drug</span> <span m="2789210">targets,</span>
  <span m="2789690">new</span> <span m="2789840">diagnostics,</span> <span m="2790570">et</span>
  <span m="2790850">cetera,</span> <span m="2791610">that</span> <span m="2791850">was</span>
  <span m="2792000">uncovered</span> <span m="2792420">by</span> <span m="2792510">going</span>
  <span m="2792720">from</span> <span m="2792870">clinical</span> <span m="2793140">outcomes</span>
  <span m="2793620">to</span> <span m="2793680">pathology</span> <span m="2794100">data</span>
  <span m="2794430">to</span> <span m="2794550">the</span> <span m="2794640">underlying</span>
  <span m="2795090">RNA</span> <span m="2795390">signature.</span></p><p><span m="2799440">And</span>
  <span m="2799590">then</span> <span m="2799740">kind</span> <span m="2799890">of</span>
  <span m="2799950">the</span> <span m="2800040">beauty</span> <span m="2800220">of</span>
  <span m="2800280">the</span> <span m="2800370">approach</span> <span m="2801300">we're</span>
  <span m="2801450">working</span> <span m="2801840">on</span> <span m="2801990">is</span>
  <span m="2802110">it's</span> <span m="2802210">super</span> <span m="2802470">scalable,</span>
  <span m="2803670">and</span> <span m="2804480">in</span> <span m="2804600">theory,</span>
  <span m="2804840">you</span> <span m="2804900">could</span> <span m="2805020">apply</span>
  <span m="2805200">it</span> <span m="2805260">to</span> <span m="2805350">all</span>
  <span m="2805530">of</span> <span m="2805620">TCGA</span> <span m="2806220">or</span>
  <span m="2806280">other</span> <span m="2806460">data</span> <span m="2806730">sets</span>
  <span m="2807000">and</span> <span m="2807090">apply</span> <span m="2807390">it</span>
  <span m="2807450">across</span> <span m="2808590">cancer</span> <span m="2808950">types</span>
  <span m="2809400">and</span> <span m="2810240">do</span> <span m="2810420">things</span>
  <span m="2810630">like</span> <span m="2810810">find--</span> <span m="2811950">automatically</span>
  <span m="2812520">find</span> <span m="2812760">artefacts</span> <span m="2813390">in</span>
  <span m="2813480">all</span> <span m="2813660">of</span> <span m="2813750">the</span>
  <span m="2813810">slides</span> <span m="2817230">and</span> <span m="2817950">kind</span>
  <span m="2818190">of</span> <span m="2818280">do</span> <span m="2818400">this</span>
  <span m="2818940">in</span> <span m="2819120">a</span> <span m="2819150">broad</span>
  <span m="2819435">way.</span> <span m="2819720">And</span> <span m="2819840">then</span>
  <span m="2820890">sort</span> <span m="2821130">of</span> <span m="2821220">the</span>
  <span m="2821310">most</span> <span m="2821640">interesting</span> <span m="2822060">part,</span>
  <span m="2822270">potentially,</span> <span m="2822700">is</span> <span m="2823050">analyzing</span>
  <span m="2823620">the</span> <span m="2823740">outputs</span> <span m="2824220">of</span>
  <span m="2824340">the</span> <span m="2824400">models</span> <span m="2824850">and</span>
  <span m="2824940">how</span> <span m="2825030">they</span> <span m="2825150">correlate</span>
  <span m="2825570">with</span> <span m="2825690">things</span> <span m="2825870">like</span>
  <span m="2825990">drug</span> <span m="2826200">response</span> <span m="2827010">or</span>
  <span m="2827100">underlying</span> <span m="2827460">molecular</span> <span m="2827850">profiles.</span></p><p><span
  m="2830100">And</span> <span m="2830220">this</span> <span m="2830400">is</span>
  <span m="2830520">really</span> <span m="2830670">the</span> <span m="2830760">process</span>
  <span m="2831210">we're</span> <span m="2831450">working</span> <span m="2831810">on,</span>
  <span m="2831930">is</span> <span m="2832050">how</span> <span m="2832140">do</span>
  <span m="2832200">we</span> <span m="2832290">go</span> <span m="2832440">from</span>
  <span m="2832620">images</span> <span m="2833100">to</span> <span m="2833610">new</span>
  <span m="2833820">ways</span> <span m="2834060">of</span> <span m="2834150">measuring</span>
  <span m="2834930">disease</span> <span m="2835290">pathology?</span> <span m="2836810">And</span>
  <span m="2836940">kind</span> <span m="2837090">of</span> <span m="2837180">in</span>
  <span m="2837270">summary,</span> <span m="2837930">a</span> <span m="2837990">lot</span>
  <span m="2838350">of</span> <span m="2838440">the</span> <span m="2838560">technology</span>
  <span m="2839070">development that</span> <span m="2839430">I</span> <span m="2839490">think</span>
  <span m="2839610">is</span> <span m="2839730">most</span> <span m="2840000">important</span>
  <span m="2840540">today</span> <span m="2841080">for</span> <span m="2841230">getting</span>
  <span m="2841470">ML</span> <span m="2841770">to</span> <span m="2841860">work</span>
  <span m="2842160">really</span> <span m="2842490">well</span> <span m="2842700">in</span>
  <span m="2842820">the</span> <span m="2842910">real</span> <span m="2843150">world</span>
  <span m="2843810">for</span> <span m="2843990">applications</span> <span m="2844500">in</span>
  <span m="2844590">medicine</span> <span m="2845490">is</span> <span m="2845700">a</span>
  <span m="2845760">lot</span> <span m="2846240">about</span> <span m="2846450">being</span>
  <span m="2846660">super</span> <span m="2847350">thoughtful</span> <span m="2847860">about</span>
  <span m="2848070">building</span> <span m="2848370">the</span> <span m="2848460">right</span>
  <span m="2848640">training</span> <span m="2849010">data</span> <span m="2849260">set.</span>
  <span m="2849900">And</span> <span m="2850050">how</span> <span m="2850170">do</span>
  <span m="2850220">you</span> <span m="2850310">do</span> <span m="2850410">that</span>
  <span m="2850530">in</span> <span m="2850620">a</span> <span m="2850680">scalable</span>
  <span m="2851370">way</span> <span m="2851670">and</span> <span m="2851790">even</span>
  <span m="2852040">in a</span> <span m="2852090">way</span> <span m="2852210">that</span>
  <span m="2852300">incorporates</span> <span m="2852960">machine</span> <span m="2853290">learning?</span></p><p><span
  m="2853770">Which</span> <span m="2853950">is</span> <span m="2854040">kind</span>
  <span m="2854220">of</span> <span m="2854280">what</span> <span m="2854410">I</span>
  <span m="2854540">was talking about</span> <span m="2854670">before--</span> <span
  m="2855030">intelligently</span> <span m="2855630">picking</span> <span m="2855900">patches.</span>
  <span m="2856410">But</span> <span m="2856830">that</span> <span m="2856960">sort</span>
  <span m="2857100">of</span> <span m="2857190">concept</span> <span m="2857700">applies</span>
  <span m="2858120">everywhere.</span> <span m="2859180">So</span> <span m="2859200">I</span>
  <span m="2859260">think</span> <span m="2859440">there's</span> <span m="2859740">almost</span>
  <span m="2860070">more</span> <span m="2860340">room</span> <span m="2860610">for</span>
  <span m="2860730">innovation</span> <span m="2861360">on</span> <span m="2861540">the</span>
  <span m="2862020">defining</span> <span m="2862560">the</span> <span m="2862650">training</span>
  <span m="2863010">data</span> <span m="2863300">set</span> <span m="2863760">side</span>
  <span m="2864210">than</span> <span m="2864390">on</span> <span m="2864540">the</span>
  <span m="2865200">predictive</span> <span m="2865710">modeling</span> <span m="2866190">side,</span>
  <span m="2866960">and</span> <span m="2867090">then</span> <span m="2867210">putting</span>
  <span m="2867450">the</span> <span m="2867510">two</span> <span m="2867630">together</span>
  <span m="2868050">is</span> <span m="2868230">incredibly</span> <span m="2868710">important.</span></p><p><span
  m="2870730">And</span> <span m="2870900">for</span> <span m="2870990">the</span>
  <span m="2871080">kind</span> <span m="2871320">of</span> <span m="2871380">work</span>
  <span m="2871560">we're</span> <span m="2871710">doing,</span> <span m="2871920">there's</span>
  <span m="2872100">already</span> <span m="2872370">such</span> <span m="2872640">great</span>
  <span m="2872850">advances</span> <span m="2873510">in</span> <span m="2873900">image</span>
  <span m="2874140">processing.</span> <span m="2874620">A</span> <span m="2874680">lot</span>
  <span m="2874920">of</span> <span m="2874980">it's</span> <span m="2875130">about</span>
  <span m="2875790">engineering</span> <span m="2876330">and</span> <span m="2876420">scalability,</span>
  <span m="2877230">as</span> <span m="2877720">well</span> <span m="2877870">as</span>
  <span m="2877960">rigorous</span> <span m="2878290">validation.</span> <span m="2879220">And</span>
  <span m="2879310">then</span> <span m="2879430">how</span> <span m="2879550">do</span>
  <span m="2879640">we</span> <span m="2879730">connect</span> <span m="2880150">it</span>
  <span m="2880240">with</span> <span m="2880690">underlying</span> <span m="2881050">molecular</span>
  <span m="2881470">data</span> <span m="2881830">as</span> <span m="2881980">well</span>
  <span m="2882100">as</span> <span m="2882190">clinical</span> <span m="2882490">outcome</span>
  <span m="2882790">data?</span> <span m="2883720">Versus</span> <span m="2884950">trying</span>
  <span m="2885310">to</span> <span m="2885400">solve</span> <span m="2885880">a</span>
  <span m="2885940">lot</span> <span m="2886120">of</span> <span m="2886180">the</span>
  <span m="2886270">core</span> <span m="2887230">vision</span> <span m="2887590">tasks,</span>
  <span m="2888100">which</span> <span m="2888850">there's</span> <span m="2889060">already</span>
  <span m="2889270">just</span> <span m="2889420">been</span> <span m="2889510">incredible</span>
  <span m="2889930">progress</span> <span m="2890320">over</span> <span m="2890440">the</span>
  <span m="2890530">past</span> <span m="2890710">couple</span> <span m="2890920">of</span>
  <span m="2890980">years.</span></p><p><span m="2891900">And</span> <span m="2892000">in</span>
  <span m="2892090">terms</span> <span m="2892330">of</span> <span m="2892420">in</span>
  <span m="2892540">our</span> <span m="2892750">world,</span> <span m="2893590">things</span>
  <span m="2893920">we</span> <span m="2894010">think</span> <span m="2894190">a</span>
  <span m="2894250">lot</span> <span m="2894460">about,</span> <span m="2894700">not</span>
  <span m="2894910">just</span> <span m="2895180">the</span> <span m="2895270">technology</span>
  <span m="2895960">and</span> <span m="2896070">putting</span> <span m="2896330">together</span>
  <span m="2896620">our data</span> <span m="2896980">sets</span> <span m="2897160">but</span>
  <span m="2897250">also,</span> <span m="2897490">how</span> <span m="2897580">do</span>
  <span m="2897640">we</span> <span m="2897760">work</span> <span m="2897970">with</span>
  <span m="2898090">regulators?</span> <span m="2898850">How</span> <span m="2898950">do</span>
  <span m="2899050">we</span> <span m="2899150">make</span> <span m="2899250">strong</span>
  <span m="2899980">business</span> <span m="2900340">cases</span> <span m="2900730">for</span>
  <span m="2900850">partners</span> <span m="2901210">working</span> <span m="2901570">with</span>
  <span m="2901720">to</span> <span m="2901780">actually</span> <span m="2902080">change</span>
  <span m="2902380">what</span> <span m="2902500">they're</span> <span m="2902620">doing</span>
  <span m="2903340">to</span> <span m="2903490">incorporate</span> <span m="2904000">some</span>
  <span m="2904090">of</span> <span m="2904150">these</span> <span m="2904300">new</span>
  <span m="2904420">approaches</span> <span m="2905230">that will</span> <span m="2905430">really</span>
  <span m="2905680">bring</span> <span m="2905920">benefits</span> <span m="2906340">to</span>
  <span m="2906430">patients</span> <span m="2906850">around</span> <span m="2907030">quality</span>
  <span m="2908470">and</span> <span m="2908590">accuracy</span> <span m="2909040">in</span>
  <span m="2909100">their</span> <span m="2909190">diagnosis?</span></p><p><span m="2911340">So</span>
  <span m="2911480">in</span> <span m="2911690">summary--</span> <span m="2912280">I</span>
  <span m="2912380">know</span> <span m="2912410">you have to</span> <span m="2912650">go
  in</span> <span m="2912770">four</span> <span m="2913070">minutes--</span> <span
  m="2914540">this</span> <span m="2914750">has</span> <span m="2914870">been</span>
  <span m="2915020">a</span> <span m="2915190">longstanding</span> <span m="2915950">problem.</span>
  <span m="2916580">There's</span> <span m="2916790">nothing</span> <span m="2917150">new</span>
  <span m="2917390">about</span> <span m="2917570">trying</span> <span m="2917780">to</span>
  <span m="2917840">apply</span> <span m="2918600">AI</span> <span m="2919070">to</span>
  <span m="2919520">diagnostics</span> <span m="2920360">or</span> <span m="2920450">to</span>
  <span m="2920690">vision</span> <span m="2921020">tasks,</span> <span m="2921500">but</span>
  <span m="2921650">there</span> <span m="2921800">are</span> <span m="2921980">some</span>
  <span m="2922190">really</span> <span m="2922520">big</span> <span m="2922820">differences</span>
  <span m="2923810">in</span> <span m="2923960">the</span> <span m="2924020">past</span>
  <span m="2924350">five</span> <span m="2924620">years</span> <span m="2924920">that,</span>
  <span m="2925010">even</span> <span m="2925190">in</span> <span m="2925280">my</span>
  <span m="2925910">short</span> <span m="2926210">career,</span> <span m="2926600">I've</span>
  <span m="2926750">seen</span> <span m="2927410">a</span> <span m="2927470">sea</span>
  <span m="2927740">change</span> <span m="2928250">in</span> <span m="2928400">this</span>
  <span m="2928580">field.</span></p><p><span m="2929480">One</span> <span m="2929810">is</span>
  <span m="2929960">availability</span> <span m="2930440">of</span> <span m="2930530">digital</span>
  <span m="2930860">data--</span> <span m="2931250">it's</span> <span m="2931400">now</span>
  <span m="2931640">much</span> <span m="2932060">cheaper</span> <span m="2932540">to</span>
  <span m="2932690">generate</span> <span m="2933140">lots</span> <span m="2933380">of</span>
  <span m="2933470">images</span> <span m="2933830">at</span> <span m="2933920">scale.</span>
  <span m="2935450">But</span> <span m="2935690">even</span> <span m="2935960">more</span>
  <span m="2936260">important,</span> <span m="2936650">I</span> <span m="2936710">think,</span>
  <span m="2936860">are</span> <span m="2936950">the</span> <span m="2937010">last</span>
  <span m="2937340">two,</span> <span m="2937970">which</span> <span m="2938150">is</span>
  <span m="2938270">access</span> <span m="2938630">to</span> <span m="2938720">large-scale</span>
  <span m="2939230">computing</span> <span m="2939620">resources</span> <span m="2940220">is</span>
  <span m="2940640">a</span> <span m="2940700">game-changer</span> <span m="2941900">for</span>
  <span m="2942380">anyone</span> <span m="2943070">with</span> <span m="2943250">access</span>
  <span m="2943790">to</span> <span m="2944240">cloud</span> <span m="2944510">computing</span>
  <span m="2945020">or</span> <span m="2945200">large</span> <span m="2945590">computing</span>
  <span m="2945920">resources.</span> <span m="2946790">Just,</span> <span m="2947000">we</span>
  <span m="2947120">all</span> <span m="2947270">have</span> <span m="2947420">access</span>
  <span m="2947900">to</span> <span m="2948070">a</span> <span m="2948110">sort</span>
  <span m="2948260">of</span> <span m="2948380">arbitrary</span> <span m="2949220">compute</span>
  <span m="2949640">today,</span> <span m="2950090">and 10</span> <span m="2950330">years</span>
  <span m="2950570">ago,</span> <span m="2951620">that</span> <span m="2951800">was</span>
  <span m="2951920">a</span> <span m="2951980">huge</span> <span m="2952370">limitation</span>
  <span m="2952645">in</span> <span m="2952920">this</span> <span m="2953060">field.</span>
  <span m="2953780">As</span> <span m="2953900">well</span> <span m="2954080">as</span>
  <span m="2954200">these</span> <span m="2954350">really</span> <span m="2954590">major</span>
  <span m="2954920">algorithmic</span> <span m="2955430">advances,</span> <span m="2955880">particularly</span>
  <span m="2956360">deep</span> <span m="2956540">CNN's</span> <span m="2957010">revision.</span></p><p><span
  m="2959090">And,</span> <span m="2959720">in</span> <span m="2959840">general,</span>
  <span m="2960460">AI</span> <span m="2960620">works</span> <span m="2960860">extremely</span>
  <span m="2961310">well</span> <span m="2961700">when</span> <span m="2962150">problems</span>
  <span m="2962660">can</span> <span m="2962810">be</span> <span m="2962930">defined</span>
  <span m="2963560">to</span> <span m="2963800">get</span> <span m="2964130">the</span>
  <span m="2964280">right</span> <span m="2964580">type</span> <span m="2964790">of</span>
  <span m="2964880">training</span> <span m="2965180">data,</span> <span m="2966080">access,</span>
  <span m="2966680">large-scale</span> <span m="2967250">computing,</span> <span m="2968280">as</span>
  <span m="2968330">well</span> <span m="2968510">as</span> <span m="2968720">implement</span>
  <span m="2969110">things</span> <span m="2969380">like</span> <span m="2969530">deep</span>
  <span m="2969710">CNNs</span> <span m="2970070">that</span> <span m="2970190">work</span>
  <span m="2970350">really</span> <span m="2970550">well.</span> <span m="2971300">And</span>
  <span m="2971480">it</span> <span m="2971570">sort</span> <span m="2971720">of</span>
  <span m="2971810">fails</span> <span m="2972170">everywhere</span> <span m="2972500">else,</span>
  <span m="2972890">which</span> <span m="2973070">is</span> <span m="2973190">probably</span>
  <span m="2973700">98%</span> <span m="2974090">of</span> <span m="2974330">things.</span>
  <span m="2974770">But</span> <span m="2975200">if</span> <span m="2975350">you</span>
  <span m="2975440">can</span> <span m="2976010">create</span> <span m="2976310">a</span>
  <span m="2976370">problem</span> <span m="2976790">where</span> <span m="2976880">the</span>
  <span m="2977000">algorithms</span> <span m="2977390">actually</span> <span m="2977660">work,</span>
  <span m="2978140">you</span> <span m="2978260">can</span> <span m="2978560">have</span>
  <span m="2978740">lots</span> <span m="2978950">of</span> <span m="2979010">data</span>
  <span m="2979220">to</span> <span m="2979340">train</span> <span m="2979610">on,</span>
  <span m="2980960">they</span> <span m="2981080">can</span> <span m="2981200">succeed</span>
  <span m="2981860">really</span> <span m="2982100">well.</span></p><p><span m="2983330">And</span>
  <span m="2983450">this</span> <span m="2983960">sort</span> <span m="2984230">of</span>
  <span m="2984320">vision-based</span> <span m="2985550">AI-powered</span> <span
  m="2985970">pathology</span> <span m="2986420">is</span> <span m="2986540">broadly</span>
  <span m="2986810">applicable</span> <span m="2987320">across,</span> <span m="2987830">really,</span>
  <span m="2988100">all</span> <span m="2988310">image-based</span> <span m="2988760">tasks</span>
  <span m="2989060">and</span> <span m="2989150">pathology.</span> <span m="2989660">It</span>
  <span m="2989720">does</span> <span m="2989900">enable</span> <span m="2990200">integration</span>
  <span m="2990740">with</span> <span m="2990920">things</span> <span m="2991160">like</span>
  <span m="2992060">omics</span> <span m="2992630">data--</span> <span m="2992900">genomics,</span>
  <span m="2993350">transcriptonics,</span> <span m="2994010">SNP</span> <span m="2994340">data,</span>
  <span m="2994630">et</span> <span m="2994880">cetera.</span> <span m="2997010">And</span>
  <span m="2997340">in</span> <span m="2997430">the</span> <span m="2997730">near</span>
  <span m="2998000">future,</span> <span m="2998330">we</span> <span m="2998450">think</span>
  <span m="2998630">this</span> <span m="2998810">will</span> <span m="2998900">be</span>
  <span m="2998960">incorporated</span> <span m="2999500">into</span> <span m="2999620">clinical</span>
  <span m="2999950">practice.</span> <span m="3000520">And</span> <span m="3000790">even</span>
  <span m="3001030">today,</span> <span m="3001360">it's</span> <span m="3001540">really</span>
  <span m="3001780">central</span> <span m="3002170">to</span> <span m="3002290">a</span>
  <span m="3002320">lot</span> <span m="3002470">of</span> <span m="3002560">research</span>
  <span m="3002950">efforts.</span></p><p><span m="3005360">And</span> <span m="3005570">I
  just</span> <span m="3005840">want to end on</span> <span m="3005950">a</span> <span
  m="3006010">quote</span> <span m="3006310">from</span> <span m="3006610">1987,</span>
  <span m="3007480">where</span> <span m="3007570">in</span> <span m="3007690">the</span>
  <span m="3007780">future,</span> <span m="3008320">AI</span> <span m="3008620">can</span>
  <span m="3008770">be</span> <span m="3008860">expected</span> <span m="3009220">to</span>
  <span m="3009260">become</span> <span m="3009400">staples</span> <span m="3009850">of</span>
  <span m="3009910">pathology</span> <span m="3010390">practice.</span> <span m="3012070">And</span>
  <span m="3012250">I</span> <span m="3012340">think</span> <span m="3012550">we're</span>
  <span m="3012790">much,</span> <span m="3013220">much</span> <span m="3013330">closer</span>
  <span m="3014971">than</span> <span m="3015370">30</span> <span m="3015640">years</span>
  <span m="3015910">ago.</span></p><p><span m="3017500">And</span> <span m="3017590">I</span>
  <span m="3017650">want</span> <span m="3017770">to</span> <span m="3017830">thank</span>
  <span m="3018220">everyone</span> <span m="3018460">at</span> <span m="3018570">PathAI,</span>
  <span m="3018930">as</span> <span m="3019060">well</span> <span m="3019160">as</span>
  <span m="3019270">Hunter,</span> <span m="3019600">who</span> <span m="3019720">really</span>
  <span m="3019900">helped</span> <span m="3020170">put</span> <span m="3020290">together</span>
  <span m="3020500">a</span> <span m="3020530">lot</span> <span m="3020650">of</span>
  <span m="3020720">these</span> <span m="3020800">slides.</span> <span m="3021310">And</span>
  <span m="3021970">we</span> <span m="3022060">do</span> <span m="3022150">have</span>
  <span m="3022240">lots</span> <span m="3022450">of</span> <span m="3022510">opportunities</span>
  <span m="3023140">for</span> <span m="3023890">machine</span> <span m="3024160">learning</span>
  <span m="3024430">engineers,</span> <span m="3025000">software</span> <span m="3025240">engineers,</span>
  <span m="3025970">et</span> <span m="3026200">cetera,</span> <span m="3026470">at
  PathAI.</span> <span m="3026940">So</span> <span m="3027130">certainly</span> <span
  m="3027790">reach</span> <span m="3028090">out</span> <span m="3029080">if</span>
  <span m="3029230">you're</span> <span m="3029320">interested</span> <span m="3029560">in
  learning</span> <span m="3029770">more.</span> <span m="3030520">And</span> <span
  m="3030760">I'm</span> <span m="3030850">happy</span> <span m="3031150">to</span>
  <span m="3031450">take</span> <span m="3031660">any</span> <span m="3031810">questions,</span>
  <span m="3032200">if</span> <span m="3032260">we</span> <span m="3032310">have</span>
  <span m="3032410">time.</span> <span m="3032990">So</span> <span m="3033280">thank</span>
  <span m="3033520">you.</span></p><p><span m="3035035">[APPLAUSE]</span></p><p>&nbsp;</p><p><span
  m="3040150">AUDIENCE:</span> <span m="3040235">Yes,</span> <span m="3040320">I</span>
  <span m="3040380">think</span> <span m="3040570">generally</span> <span m="3041010">very</span>
  <span m="3041250">aggressive</span> <span m="3041860">events.</span> <span m="3042760">I</span>
  <span m="3042860">was</span> <span m="3042930">wondering</span> <span m="3043950">how</span>
  <span m="3044390">close</span> <span m="3044720">is</span> <span m="3044870">this</span>
  <span m="3045200">to</span> <span m="3045660">clinical</span> <span m="3046110">practice?</span>
  <span m="3046640">Is there</span> <span m="3046925">FDA</span> <span m="3047740">or--</span></p><p><span
  m="3048180">ANDY BECK:</span> <span m="3048315">Yeah,</span> <span m="3049610">so</span>
  <span m="3051150">I</span> <span m="3051210">mean,</span> <span m="3051420">actual</span>
  <span m="3051780">clinical</span> <span m="3052170">practice,</span> <span m="3052590">probably</span>
  <span m="3053900">2020,</span> <span m="3054750">like</span> <span m="3055140">early,</span>
  <span m="3055500">mid-2020.</span> <span m="3057890">But</span> <span m="3058680">I</span>
  <span m="3058740">mean,</span> <span m="3058860">today,</span> <span m="3059310">it's</span>
  <span m="3059460">very</span> <span m="3059790">active</span> <span m="3060120">in</span>
  <span m="3060300">clinical</span> <span m="3060750">research,</span> <span m="3061450">so</span>
  <span m="3061680">like</span> <span m="3061860">clinical</span> <span m="3062130">trials,</span>
  <span m="3063320">et</span> <span m="3063400">cetera,</span> <span m="3063690">that</span>
  <span m="3063810">do</span> <span m="3063900">involve</span> <span m="3064230">patients,</span>
  <span m="3064740">but</span> <span m="3064860">it's</span> <span m="3065070">in</span>
  <span m="3065520">a</span> <span m="3065970">much</span> <span m="3066240">more</span>
  <span m="3066420">well-defined</span> <span m="3066990">setting.</span> <span m="3067740">But</span>
  <span m="3068070">the</span> <span m="3068160">first</span> <span m="3068670">clinical</span>
  <span m="3069210">use</span> <span m="3069420">cases,</span> <span m="3069770">at</span>
  <span m="3069840">least</span> <span m="3070050">of</span> <span m="3070230">the</span>
  <span m="3070380">types</span> <span m="3070680">of</span> <span m="3070740">stuff</span>
  <span m="3071010">we're</span> <span m="3071130">building,</span> <span m="3072000">will</span>
  <span m="3072270">be,</span> <span m="3072570">I</span> <span m="3072690">think,</span>
  <span m="3072870">about</span> <span m="3073140">a</span> <span m="3073200">year</span>
  <span m="3073470">from</span> <span m="3073680">now.</span></p><p><span m="3074350">And</span>
  <span m="3074490">I</span> <span m="3074550">think</span> <span m="3074670">it will</span>
  <span m="3074760">start</span> <span m="3075030">small</span> <span m="3075330">and</span>
  <span m="3075420">then</span> <span m="3075540">get</span> <span m="3075720">progressively</span>
  <span m="3076290">bigger.</span> <span m="3076680">So</span> <span m="3076770">I</span>
  <span m="3076860">don't</span> <span m="3076980">think</span> <span m="3077100">it's</span>
  <span m="3077220">going</span> <span m="3077300">to</span> <span m="3077400">be</span>
  <span m="3077880">everything</span> <span m="3078270">all</span> <span m="3078390">at</span>
  <span m="3078450">once</span> <span m="3078720">transforms</span> <span m="3079770">in</span>
  <span m="3079920">the</span> <span m="3079980">clinic,</span> <span m="3080460">but</span>
  <span m="3080640">I</span> <span m="3080700">do</span> <span m="3080850">think</span>
  <span m="3081090">we'll</span> <span m="3081210">start</span> <span m="3081570">seeing</span>
  <span m="3081720">the</span> <span m="3081810">first</span> <span m="3082050">applications</span>
  <span m="3082740">out.</span> <span m="3083970">And</span> <span m="3084120">they</span>
  <span m="3084240">will</span> <span m="3084420">go--</span> <span m="3084700">some</span>
  <span m="3084810">of</span> <span m="3084870">them</span> <span m="3084990">will</span>
  <span m="3085080">go</span> <span m="3085200">through</span> <span m="3085320">the</span>
  <span m="3085410">FDA,</span> <span m="3085830">and</span> <span m="3085950">there'll</span>
  <span m="3086100">be</span> <span m="3086220">some</span> <span m="3086490">laboratory-developed</span>
  <span m="3087240">tests.</span> <span m="3087450">Ours</span> <span m="3087690">will</span>
  <span m="3087780">go</span> <span m="3087930">through</span> <span m="3088050">the</span>
  <span m="3088140">FDA,</span> <span m="3089310">but</span> <span m="3089550">labs</span>
  <span m="3089970">themselves</span> <span m="3090450">can</span> <span m="3090600">actually</span>
  <span m="3091470">validate</span> <span m="3091950">tools</span> <span m="3092400">themselves.</span>
  <span m="3093870">And</span> <span m="3093990">that's</span> <span m="3094140">another</span>
  <span m="3094410">path.</span></p><p><span m="3095700">AUDIENCE:</span> <span m="3095940">Thanks.</span></p><p><span
  m="3096180">ANDY BECK:</span> <span m="3096315">Sure.</span></p><p><span m="3106698">PROFESSOR:</span>
  <span m="3106820">So</span> <span m="3109640">have</span> <span m="3109780">you</span>
  <span m="3109870">been</span> <span m="3110200">using</span> <span m="3110890">observational</span>
  <span m="3111460">data</span> <span m="3111690">sets?</span> <span m="3111880">You</span>
  <span m="3111940">gave</span> <span m="3112120">one</span> <span m="3112240">example</span>
  <span m="3112660">where</span> <span m="3112810">you</span> <span m="3112930">tried</span>
  <span m="3113230">to</span> <span m="3114880">use</span> <span m="3115960">data</span>
  <span m="3116200">from</span> <span m="3116350">a</span> <span m="3116410">randomized</span>
  <span m="3116830">controlled</span> <span m="3117190">trial,</span> <span m="3117900">or</span>
  <span m="3117970">both</span> <span m="3118150">trials,</span> <span m="3118540">you
  used</span> <span m="3118660">different</span> <span m="3119090">randomized</span>
  <span m="3119370">control trials</span> <span m="3119750">for</span> <span m="3120130">different</span>
  <span m="3120460">efficacies</span> <span m="3120900">of</span> <span m="3121060">each
  event.</span></p><p><span m="3123820">The next</span> <span m="3124150">major</span>
  <span m="3124420">segment</span> <span m="3124690">of</span> <span m="3124960">this
  course,</span> <span m="3125560">starting</span> <span m="3126070">in</span> <span
  m="3126190">about</span> <span m="3126550">two</span> <span m="3126790">weeks,</span>
  <span m="3127180">will</span> <span m="3127330">be</span> <span m="3127540">about</span>
  <span m="3127840">causal</span> <span m="3128170">inference from</span> <span m="3128500">observational</span>
  <span m="3129100">data.</span> <span m="3130060">I'm</span> <span m="3130210">wondering</span>
  <span m="3130670">if</span> <span m="3130920">that</span> <span m="3131150">is</span>
  <span m="3131330">something</span> <span m="3132120">PathAI</span> <span m="3132510">has
  gotten</span> <span m="3132860">into</span> <span m="3133150">yet?</span> <span
  m="3134300">And</span> <span m="3134800">if</span> <span m="3135070">so,</span>
  <span m="3135340">what</span> <span m="3135490">has</span> <span m="3135610">your</span>
  <span m="3135730">finding</span> <span m="3136150">been</span> <span m="3136390">so</span>
  <span m="3136540">far?</span></p><p><span m="3137410">ANDY BECK:</span> <span m="3137582">So</span>
  <span m="3138100">we</span> <span m="3138310">have</span> <span m="3138550">focused</span>
  <span m="3139030">a</span> <span m="3139090">lot</span> <span m="3139480">on</span>
  <span m="3139600">randomized</span> <span m="3140020">controlled</span> <span m="3140320">trial</span>
  <span m="3140650">data</span> <span m="3141880">and</span> <span m="3142060">have</span>
  <span m="3143110">developed</span> <span m="3143680">methods</span> <span m="3144160">around</span>
  <span m="3144520">that,</span> <span m="3144700">which</span> <span m="3144910">sort</span>
  <span m="3145150">of</span> <span m="3145300">simplifies</span> <span m="3145960">the</span>
  <span m="3146080">problem</span> <span m="3146650">and</span> <span m="3147130">allows</span>
  <span m="3147490">us</span> <span m="3147610">to</span> <span m="3147730">do,</span>
  <span m="3148180">I</span> <span m="3148240">think,</span> <span m="3148390">pretty</span>
  <span m="3148600">clever</span> <span m="3148960">things</span> <span m="3149350">around</span>
  <span m="3150460">how</span> <span m="3150640">to</span> <span m="3150760">generate</span>
  <span m="3151120">those</span> <span m="3151300">types</span> <span m="3151540">of</span>
  <span m="3151600">graphs</span> <span m="3151990">I</span> <span m="3152050">was</span>
  <span m="3152170">showing,</span> <span m="3153330">where</span> <span m="3153640">you</span>
  <span m="3153790">truly</span> <span m="3154180">can</span> <span m="3154390">infer</span>
  <span m="3155260">the</span> <span m="3155410">treatment</span> <span m="3155950">is</span>
  <span m="3156070">having</span> <span m="3156340">an</span> <span m="3156430">effect.</span></p><p><span
  m="3158620">And</span> <span m="3158740">we've</span> <span m="3158950">done</span>
  <span m="3159220">far</span> <span m="3159580">less.</span> <span m="3159910">I'm</span>
  <span m="3160030">super</span> <span m="3160330">interested</span> <span m="3160900">in</span>
  <span m="3161020">that.</span> <span m="3161230">I'd</span> <span m="3161350">say</span>
  <span m="3161470">the</span> <span m="3161590">advantages</span> <span m="3162040">of</span>
  <span m="3162130">RCTs</span> <span m="3162850">are</span> <span m="3162940">people</span>
  <span m="3163190">are</span> <span m="3163210">already</span> <span m="3163480">investing</span>
  <span m="3163960">hugely</span> <span m="3164440">in</span> <span m="3164560">building</span>
  <span m="3165070">these</span> <span m="3165250">very</span> <span m="3165580">well-curated</span>
  <span m="3166300">data</span> <span m="3166590">sets</span> <span m="3167200">that</span>
  <span m="3167350">include</span> <span m="3168550">images,</span> <span m="3169270">molecular</span>
  <span m="3169750">data,</span> <span m="3170020">when</span> <span m="3170140">available,</span>
  <span m="3170590">treatment,</span> <span m="3171070">and</span> <span m="3171220">outcome.</span>
  <span m="3172170">And</span> <span m="3172300">it's</span> <span m="3172420">just</span>
  <span m="3172780">that's</span> <span m="3173080">there,</span> <span m="3173590">because</span>
  <span m="3173770">they've</span> <span m="3173980">invested</span> <span m="3174490">in</span>
  <span m="3174640">the</span> <span m="3174730">clinical</span> <span m="3175000">trial.</span>
  <span m="3175300">They've</span> <span m="3175480">invested</span> <span m="3175745">in</span>
  <span m="3176010">generating</span> <span m="3176200">that</span> <span m="3176290">data</span>
  <span m="3176470">set.</span></p><p><span m="3177130">To</span> <span m="3177250">me,</span>
  <span m="3177370">the</span> <span m="3177460">big</span> <span m="3177610">challenge</span>
  <span m="3177870">in</span> <span m="3177940">observational</span> <span m="3178630">stuff,</span>
  <span m="3179110">there's</span> <span m="3179290">a</span> <span m="3179350">few</span>
  <span m="3179990">but</span> <span m="3180150">I'd</span> <span m="3180260">be</span>
  <span m="3180430">interested in</span> <span m="3180700">what</span> <span m="3180850">you</span>
  <span m="3180910">guys</span> <span m="3181150">are</span> <span m="3181210">doing</span>
  <span m="3182320">and</span> <span m="3182500">learn</span> <span m="3182710">about</span>
  <span m="3182950">it,</span> <span m="3183400">is</span> <span m="3183760">getting</span>
  <span m="3184120">the</span> <span m="3184210">data</span> <span m="3184540">is</span>
  <span m="3184660">not</span> <span m="3184870">easy,</span> <span m="3185230">right?</span>
  <span m="3186310">The</span> <span m="3187060">outcome</span> <span m="3187450">data</span>
  <span m="3187870">is</span> <span m="3188050">not--</span> <span m="3189400">linking</span>
  <span m="3189730">the</span> <span m="3189790">pathology</span> <span m="3190360">images</span>
  <span m="3190780">with</span> <span m="3190990">the</span> <span m="3191110">outcome</span>
  <span m="3191410">data</span> <span m="3191710">even</span> <span m="3192020">is,</span>
  <span m="3192220">actually,</span> <span m="3192560">in</span> <span m="3192580">my</span>
  <span m="3192710">opinion,</span> <span m="3192940">harder</span> <span m="3193450">in</span>
  <span m="3193630">observational</span> <span m="3194410">way than</span> <span m="3194580">in</span>
  <span m="3194690">RCT.</span> <span m="3195490">Because</span> <span m="3195640">they're</span>
  <span m="3195730">actually</span> <span m="3195970">doing</span> <span m="3196420">it</span>
  <span m="3196490">and</span> <span m="3196550">paying</span> <span m="3196810">for
  it</span> <span m="3196990">and</span> <span m="3197080">collecting it</span> <span
  m="3197510">in</span> <span m="3197660">RCTs.</span></p><p><span m="3198790">No</span>
  <span m="3199000">one's</span> <span m="3199210">really</span> <span m="3199420">done</span>
  <span m="3199570">a</span> <span m="3199630">very</span> <span m="3199810">good</span>
  <span m="3199930">job</span> <span m="3200290">of--</span> <span m="3201270">TCGA</span>
  <span m="3201940">would</span> <span m="3202090">be</span> <span m="3202180">a</span>
  <span m="3202240">good</span> <span m="3202390">place</span> <span m="3202600">to</span>
  <span m="3202720">play</span> <span m="3203020">around</span> <span m="3203380">with</span>
  <span m="3203530">because</span> <span m="3203710">that</span> <span m="3203920">is</span>
  <span m="3204040">observational</span> <span m="3204700">data.</span> <span m="3206320">And</span>
  <span m="3206440">we</span> <span m="3206590">want</span> <span m="3206740">to</span>
  <span m="3206950">also, we</span> <span m="3207330">generally</span> <span m="3207700">want</span>
  <span m="3207820">to</span> <span m="3207880">focus</span> <span m="3208210">on</span>
  <span m="3208330">actionable</span> <span m="3209290">decisions.</span> <span m="3209860">And</span>
  <span m="3209940">RCT</span> <span m="3210450">is</span> <span m="3210520">sort</span>
  <span m="3210670">of</span> <span m="3210730">perfectly</span> <span m="3211150">set</span>
  <span m="3211430">up</span> <span m="3211540">for</span> <span m="3211690">that.</span>
  <span m="3212050">Do</span> <span m="3212230">I</span> <span m="3212320">give</span>
  <span m="3212530">drug</span> <span m="3212950">X</span> <span m="3213310">or</span>
  <span m="3213460">not?</span></p><p><span m="3215500">So</span> <span m="3215740">I</span>
  <span m="3215800">think</span> <span m="3215950">if</span> <span m="3216010">you</span>
  <span m="3216100">put</span> <span m="3216310">together</span> <span m="3216550">the</span>
  <span m="3216640">right</span> <span m="3216850">data</span> <span m="3217030">set</span>
  <span m="3217420">and</span> <span m="3217510">somehow</span> <span m="3217810">make</span>
  <span m="3218080">the</span> <span m="3218170">results</span> <span m="3218590">actionable,</span>
  <span m="3220220">it</span> <span m="3220320">could</span> <span m="3220420">be</span>
  <span m="3220810">really,</span> <span m="3221240">really</span> <span m="3221350">useful,</span>
  <span m="3221770">because</span> <span m="3221920">there</span> <span m="3222010">is</span>
  <span m="3222160">a</span> <span m="3222190">lot</span> <span m="3222340">of</span>
  <span m="3222400">data.</span> <span m="3222700">But</span> <span m="3222910">I</span>
  <span m="3223060">think</span> <span m="3223300">just</span> <span m="3223510">collecting</span>
  <span m="3224710">the</span> <span m="3224890">outcomes</span> <span m="3225400">and</span>
  <span m="3225520">linking</span> <span m="3225760">them</span> <span m="3225850">with</span>
  <span m="3225940">images</span> <span m="3226300">is</span> <span m="3226420">actually</span>
  <span m="3226660">quite</span> <span m="3226900">hard.</span> <span m="3227260">And</span>
  <span m="3227470">ironically,</span> <span m="3228140">I</span> <span m="3228190">think</span>
  <span m="3228310">it's</span> <span m="3228400">harder</span> <span m="3228820">for</span>
  <span m="3229000">observational</span> <span m="3229690">than</span> <span m="3229900">for</span>
  <span m="3231510">randomized</span> <span m="3231800">control</span> <span m="3232090">trials,</span>
  <span m="3232390">where</span> <span m="3232500">they're already</span> <span m="3232600">collecting</span>
  <span m="3232990">it.</span></p><p><span m="3233290">I</span> <span m="3233350">guess</span>
  <span m="3233530">one</span> <span m="3233710">example</span> <span m="3234070">would</span>
  <span m="3234160">be</span> <span m="3234370">the</span> <span m="3234460">Nurses'</span>
  <span m="3234730">Health</span> <span m="3234880">Study</span> <span m="3235210">or</span>
  <span m="3235270">these</span> <span m="3235450">big</span> <span m="3235660">epidemiology</span>
  <span m="3236440">cohorts,</span> <span m="3238060">potentially.</span> <span m="3238600">They</span>
  <span m="3238750">are</span> <span m="3238840">collecting</span> <span m="3239260">that</span>
  <span m="3239380">data</span> <span m="3239770">and</span> <span m="3240280">organizing</span>
  <span m="3240850">it.</span> <span m="3241240">But</span> <span m="3241360">what</span>
  <span m="3241480">were</span> <span m="3241600">you</span> <span m="3241690">thinking</span>
  <span m="3241990">about?</span> <span m="3242140">Do</span> <span m="3242200">you
  have</span> <span m="3242360">anything</span> <span m="3242620">with</span> <span
  m="3242710">pathology</span> <span m="3243220">in</span> <span m="3243310">mind</span>
  <span m="3243580">for</span> <span m="3244090">causal</span> <span m="3244450">inference</span>
  <span m="3244810">from</span> <span m="3244960">observational</span> <span m="3245530">data?</span></p><p><span
  m="3245770">PROFESSOR:</span> <span m="3245995">Well,</span> <span m="3246220">I</span>
  <span m="3246310">think,</span> <span m="3246580">the example</span> <span m="3246990">you</span>
  <span m="3247480">gave,</span> <span m="3247710">like</span> <span m="3247900">Nurses'</span>
  <span m="3248500">Health</span> <span m="3248680">Study</span> <span m="3249280">or</span>
  <span m="3249610">the Framingham</span> <span m="3250300">study,</span> <span m="3251000">where</span>
  <span m="3251630">you're</span> <span m="3251860">tracking</span> <span m="3252220">patients</span>
  <span m="3252590">across</span> <span m="3252850">time.</span> <span m="3253510">They're</span>
  <span m="3253720">getting</span> <span m="3254050">different</span> <span m="3254380">interventions</span>
  <span m="3255160">across</span> <span m="3255680">time.</span> <span m="3256700">And</span>
  <span m="3257080">because</span> <span m="3257770">of</span> <span m="3257920">the</span>
  <span m="3258010">way</span> <span m="3258190">the</span> <span m="3258250">study</span>
  <span m="3258490">was</span> <span m="3258580">designed,</span> <span m="3258940">in</span>
  <span m="3259030">fact,</span> <span m="3259370">there are</span> <span m="3259480">even</span>
  <span m="3259870">good</span> <span m="3260160">outcomes</span> <span m="3260420">for</span>
  <span m="3260680">patients</span> <span m="3261220">across</span> <span m="3261590">times.</span>
  <span m="3262040">So that</span> <span m="3262250">problem</span> <span m="3262620">in
  the profession</span> <span m="3262990">doesn't</span> <span m="3263260">happen</span>
  <span m="3263620">there.</span></p><p><span m="3264960">But</span> <span m="3265210">then</span>
  <span m="3265610">suppose</span> <span m="3265840">you were</span> <span m="3266070">to
  take it from a</span> <span m="3266470">biobank</span> <span m="3267910">and</span>
  <span m="3268360">do</span> <span m="3268580">pathologies?</span> <span m="3268860">You're
  now</span> <span m="3269140">getting</span> <span m="3269340">the</span> <span m="3269530">samples.</span>
  <span m="3271450">Then,</span> <span m="3272080">you</span> <span m="3272230">can</span>
  <span m="3272410">ask</span> <span m="3272690">about,</span> <span m="3273310">well,</span>
  <span m="3273500">what</span> <span m="3273540">is</span> <span m="3273640">the</span>
  <span m="3273760">effect</span> <span m="3274060">of</span> <span m="3274150">different</span>
  <span m="3274480">interventions</span> <span m="3274750">or</span> <span m="3275020">treatment</span>
  <span m="3275650">plans</span> <span m="3276100">on</span> <span m="3276520">outcomes?</span>
  <span m="3277740">The</span> <span m="3277870">challenge,</span> <span m="3278170">of</span>
  <span m="3278470">course,</span> <span m="3278710">drawing</span> <span m="3279070">inferences</span>
  <span m="3279610">there</span> <span m="3279820">is</span> <span m="3280000">that</span>
  <span m="3280270">there was</span> <span m="3280670">bias</span> <span m="3280925">in
  terms</span> <span m="3281180">of who</span> <span m="3281616">got</span> <span
  m="3282052">what treatments.</span> <span m="3283510">That's</span> <span m="3283780">where</span>
  <span m="3284080">the</span> <span m="3284170">techniques</span> <span m="3284530">that
  we</span> <span m="3284770">talk about in</span> <span m="3284980">class</span>
  <span m="3285445">would</span> <span m="3285910">become</span> <span m="3286180">very</span>
  <span m="3286626">important.</span> <span m="3288790">I just say,</span> <span m="3289160">I</span>
  <span m="3289420">appreciate</span> <span m="3289870">the</span> <span m="3289960">challenges</span>
  <span m="3290400">that you</span> <span m="3290470">mentioned.</span></p><p><span
  m="3291070">ANDY BECK:</span> <span m="3291130">I</span> <span m="3291190">think</span>
  <span m="3291310">it's</span> <span m="3291430">incredibly</span> <span m="3292060">powerful.</span>
  <span m="3292670">I</span> <span m="3292690">think</span> <span m="3292840">the</span>
  <span m="3292900">other</span> <span m="3293200">issue</span> <span m="3293620">I</span>
  <span m="3293710">just</span> <span m="3293890">think</span> <span m="3294100">about</span>
  <span m="3294370">is</span> <span m="3294910">that</span> <span m="3295030">treatments</span>
  <span m="3295510">change</span> <span m="3295900">so</span> <span m="3296050">quickly</span>
  <span m="3296410">over</span> <span m="3296590">time.</span> <span m="3297040">So</span>
  <span m="3297220">you</span> <span m="3297310">don't</span> <span m="3297430">want</span>
  <span m="3297550">to</span> <span m="3297610">be</span> <span m="3297700">like</span>
  <span m="3297850">overfitting</span> <span m="3298290">to</span> <span m="3298390">the</span>
  <span m="3298480">past.</span> <span m="3301360">But</span> <span m="3301660">I</span>
  <span m="3301780">think</span> <span m="3301930">there's</span> <span m="3302050">certain</span>
  <span m="3302260">cases</span> <span m="3302620">where</span> <span m="3302770">the</span>
  <span m="3303100">therapeutic</span> <span m="3303520">decisions</span> <span m="3303940">today</span>
  <span m="3304180">are</span> <span m="3304360">similar</span> <span m="3304720">to</span>
  <span m="3304810">what</span> <span m="3304930">they</span> <span m="3305020">were</span>
  <span m="3305110">in</span> <span m="3305170">the</span> <span m="3305260">past.</span>
  <span m="3305560">There</span> <span m="3305680">are</span> <span m="3305710">other</span>
  <span m="3305890">areas,</span> <span m="3306640">like</span> <span m="3306850">immunooncology,</span>
  <span m="3307690">where</span> <span m="3308410">there's</span> <span m="3308620">just</span>
  <span m="3308770">no</span> <span m="3308980">history</span> <span m="3309400">to</span>
  <span m="3309490">learn</span> <span m="3309730">from.</span> <span m="3310570">So</span>
  <span m="3310660">I</span> <span m="3310690">think</span> <span m="3310810">it</span>
  <span m="3310870">depends</span> <span m="3311260">on</span> <span m="3311440">the--</span></p><p><span
  m="3312490">PROFESSOR:</span> <span m="3312533">All</span> <span m="3312576">right,</span>
  <span m="3312885">then</span> <span m="3313150">with</span> <span m="3313310">that,</span>
  <span m="3313570">let's thank</span> <span m="3313950">Andy</span> <span m="3314250">Beck.</span></p><p><span
  m="3314850">[APPLAUSE]</span></p><p><span m="3315150">ANDY BECK:</span> <span m="3315250">Thank</span>
  <span m="3315350">you.</span></p>
type: course
uid: 657574bd0575b7aa68db5dfea1969336

---
None