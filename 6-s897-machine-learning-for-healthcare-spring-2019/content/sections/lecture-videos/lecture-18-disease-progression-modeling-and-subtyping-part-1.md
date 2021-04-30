---
about_this_resource_text: '<p>Prof. Sontag discusses aspects of disease progression
  modeling, including staging, subtyping, and multi-task and unsupervised learning.
  The goals are to determine the patient&rsquo;s place in the disease trajectory and
  how treatment may affect progression.</p> <p>Speaker: David Sontag</p>             <p><a
  href="./resolveuid/e09af5308ddd08566747347ad6a2fab5">Lecture 18: Disease Progression
  &amp; Subtyping, Part 1 slides (PDF - 1.6MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: yYWyLZrdRRI
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: Video-YouTube-Stream
  type: Video
  uid: 0fa880e82467a592088da6fcf974659a
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/yYWyLZrdRRI/default.jpg
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: 11fd1315a58e44eaf2b22d371b3b5a82
- id: 3Play-3PlayYouTubeid-MP4
  media_location: yYWyLZrdRRI
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: de4a44d302e928144af9a999a0871edd
- id: yYWyLZrdRRI.srt
  parent_uid: 77923ed984040ad58785a8ce650bca64
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-18-disease-progression-modeling-and-subtyping-part-1/yYWyLZrdRRI.srt
  title: 3play caption file
  type: null
  uid: 6f46bde4dbc9e0ecc1ba8b970e07f999
- id: yYWyLZrdRRI.pdf
  parent_uid: 77923ed984040ad58785a8ce650bca64
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-18-disease-progression-modeling-and-subtyping-part-1/yYWyLZrdRRI.pdf
  title: 3play pdf file
  type: null
  uid: 6f9bae3ca11e314645f4c97c10fd4bbd
- id: Caption-3Play YouTube id-SRT
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: 0e0fed658d1e2df778afa9b0a0d707e2
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: 5e6bd43e830b6f4eda58e597ccfc8008
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec18_300k.mp4
  parent_uid: 77923ed984040ad58785a8ce650bca64
  title: Video-Internet Archive-MP4
  type: Video
  uid: 2e4b8a16c3f400901885467d8f3f393d
inline_embed_id: 76879431lecture18diseaseprogressionmodelingandsubtypingpart178729505
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-18-disease-progression-modeling-and-subtyping-part-1
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-18-disease-progression-modeling-and-subtyping-part-1
template_type: Tabbed
title: 'Lecture 18: Disease Progression Modeling and Subtyping, Part 1'
transcript: <p><span m="15340">DAVID SONTAG:</span> <span m="15415">So</span> <span
  m="15490">we're</span> <span m="15580">done</span> <span m="15760">with</span> <span
  m="15880">our</span> <span m="15970">segment</span> <span m="16630">on</span> <span
  m="17020">causal</span> <span m="17410">inference</span> <span m="17980">and</span>
  <span m="18460">reinforcement</span> <span m="19000">learning.</span> <span m="20320">And</span>
  <span m="20560">for the</span> <span m="20690">next</span> <span m="20950">week,</span>
  <span m="21670">today</span> <span m="22030">and</span> <span m="22150">Tuesday's</span>
  <span m="22510">lecture,</span> <span m="23210">we'll</span> <span m="23230">be</span>
  <span m="23320">talking</span> <span m="23710">about</span> <span m="23890">disease</span>
  <span m="24160">progression</span> <span m="24520">modeling</span> <span m="24850">and</span>
  <span m="24940">disease</span> <span m="25120">subtyping.</span> <span m="26740">This</span>
  <span m="26950">is,</span> <span m="27310">from</span> <span m="27460">my</span>
  <span m="27580">perspective,</span> <span m="28040">a</span> <span m="28140">really</span>
  <span m="28180">exciting</span> <span m="28510">field.</span></p><p><span m="29530">It's</span>
  <span m="29770">one</span> <span m="30040">which</span> <span m="30430">has</span>
  <span m="30880">really</span> <span m="31180">a</span> <span m="31240">richness</span>
  <span m="31750">of</span> <span m="31870">literature</span> <span m="32270">going</span>
  <span m="32500">back</span> <span m="32770">to</span> <span m="32890">somewhat</span>
  <span m="33550">simple</span> <span m="33880">approaches</span> <span m="34480">from</span>
  <span m="35290">a</span> <span m="35320">couple</span> <span m="35560">of</span>
  <span m="35620">decades</span> <span m="35980">ago</span> <span m="37060">up</span>
  <span m="37240">to</span> <span m="37690">some</span> <span m="38050">really</span>
  <span m="38470">state</span> <span m="38740">of</span> <span m="38800">the</span>
  <span m="38860">art</span> <span m="39130">methods,</span> <span m="40250">including</span>
  <span m="40540">one</span> <span m="40780">which</span> <span m="40990">is</span>
  <span m="41290">in</span> <span m="41410">one</span> <span m="41560">of</span> <span
  m="41650">your</span> <span m="41740">readings</span> <span m="42130">for</span>
  <span m="42220">today's</span> <span m="42520">lecture.</span> <span m="43900">And</span>
  <span m="44020">I</span> <span m="44080">could</span> <span m="44290">spent</span>
  <span m="44890">a</span> <span m="44980">few</span> <span m="45190">weeks</span>
  <span m="45580">just</span> <span m="45760">talking</span> <span m="46000">about</span>
  <span m="46150">this</span> <span m="46300">topic.</span> <span m="47260">But</span>
  <span m="47410">instead,</span> <span m="48220">since</span> <span m="48340">we</span>
  <span m="48460">have</span> <span m="48610">a lot to</span> <span m="48790">cover
  in</span> <span m="49090">this</span> <span m="49240">course,</span> <span m="50110">what</span>
  <span m="50230">I'll</span> <span m="50320">do</span> <span m="50560">today</span>
  <span m="51100">is</span> <span m="51340">give</span> <span m="51520">you</span>
  <span m="51850">a</span> <span m="52150">high-level</span> <span m="52690">overview</span>
  <span m="53380">of</span> <span m="55210">one</span> <span m="55450">approach</span>
  <span m="55910">to</span> <span m="55950">try</span> <span m="56080">to</span> <span
  m="56170">think</span> <span m="56380">through</span> <span m="56470">these</span>
  <span m="56620">questions.</span></p><p><span m="57710">The</span> <span m="57810">methods</span>
  <span m="58030">in</span> <span m="58120">today's</span> <span m="58420">lecture</span>
  <span m="58690">will</span> <span m="58780">be</span> <span m="58870">somewhat</span>
  <span m="59140">simple.</span> <span m="59860">They're</span> <span m="60010">meant</span>
  <span m="60250">to</span> <span m="60430">illustrate</span> <span m="60850">how</span>
  <span m="61150">simple</span> <span m="61420">methods</span> <span m="61750">can</span>
  <span m="61930">go</span> <span m="62080">a</span> <span m="62110">long</span> <span
  m="62380">way.</span> <span m="63220">And</span> <span m="63550">they're</span>
  <span m="63700">meant</span> <span m="64120">to</span> <span m="64450">illustrate,</span>
  <span m="64870">also,</span> <span m="65440">how</span> <span m="65710">one</span>
  <span m="65920">could</span> <span m="66610">learn</span> <span m="66900">something</span>
  <span m="67300">really</span> <span m="67570">significant</span> <span m="68200">about</span>
  <span m="68860">clinical</span> <span m="69220">outcomes</span> <span m="69820">and</span>
  <span m="69940">about</span> <span m="70240">predicting</span> <span m="70660">these</span>
  <span m="70810">progression</span> <span m="71380">from</span> <span m="71650">these</span>
  <span m="71770">simple</span> <span m="72040">methods.</span> <span m="73000">And</span>
  <span m="73090">then</span> <span m="73510">in</span> <span m="74020">Tuesday's</span>
  <span m="74440">lecture,</span> <span m="74950">I'll</span> <span m="76210">ramp</span>
  <span m="76480">it</span> <span m="76540">up</span> <span m="76660">quite</span>
  <span m="76840">a</span> <span m="76900">bit.</span> <span m="77170">And</span>
  <span m="77260">I'll</span> <span m="77320">talk</span> <span m="77530">about</span>
  <span m="78190">several</span> <span m="78460">more</span> <span m="78610">elaborate</span>
  <span m="78940">approaches</span> <span m="79360">towards</span> <span m="79570">this</span>
  <span m="79690">problem,</span> <span m="79930">which</span> <span m="80080">tackle</span>
  <span m="80440">some</span> <span m="80560">more</span> <span m="80710">substantial</span>
  <span m="81160">problems</span> <span m="81550">that</span> <span m="81640">we'll</span>
  <span m="81790">really</span> <span m="81970">elucidate</span> <span m="82340">at</span>
  <span m="82450">the</span> <span m="82510">end</span> <span m="82630">of</span>
  <span m="82690">today's</span> <span m="82930">lecture.</span></p><p><span m="87120">So</span>
  <span m="87140">there's</span> <span m="87350">three</span> <span m="88085">types</span>
  <span m="88520">of</span> <span m="88580">questions</span> <span m="88940">that</span>
  <span m="89030">we</span> <span m="89150">hope</span> <span m="89390">to</span>
  <span m="89540">answer</span> <span m="89990">when</span> <span m="90200">studying</span>
  <span m="90530">disease</span> <span m="90830">progression</span> <span m="91160">modeling.</span>
  <span m="93450">At</span> <span m="93560">a</span> <span m="93590">high</span> <span
  m="93740">level,</span> <span m="94320">I</span> <span m="94420">want</span> <span
  m="94520">you</span> <span m="94620">to</span> <span m="94720">think</span> <span
  m="94730">about</span> <span m="95060">this</span> <span m="95270">type</span> <span
  m="95420">of</span> <span m="95480">picture</span> <span m="95720">and</span> <span
  m="95810">have</span> <span m="95960">this</span> <span m="96110">in</span> <span
  m="96170">the</span> <span m="96220">back</span> <span m="96410">of</span> <span
  m="96470">your</span> <span m="96590">head</span> <span m="96890">throughout</span>
  <span m="98510">today</span> <span m="98840">and</span> <span m="98930">Tuesday's</span>
  <span m="99260">lecture.</span> <span m="101150">What</span> <span m="101300">you're</span>
  <span m="101390">seeing</span> <span m="101660">here</span> <span m="101900">is</span>
  <span m="101960">a</span> <span m="102020">single</span> <span m="102350">patient's</span>
  <span m="102770">disease</span> <span m="103070">trajectory</span> <span m="103520">across</span>
  <span m="103790">time.</span> <span m="105110">On</span> <span m="105240">the</span>
  <span m="105290">x-axis</span> <span m="106130">is</span> <span m="106700">time.</span>
  <span m="107180">On</span> <span m="107270">the</span> <span m="107330">y-axis</span>
  <span m="108260">is</span> <span m="108560">some</span> <span m="108890">measure</span>
  <span m="109310">of</span> <span m="109400">disease</span> <span m="109700">burden.</span></p><p><span
  m="110880">So</span> <span m="110930">for</span> <span m="110990">example,</span>
  <span m="111540">you</span> <span m="111640">could</span> <span m="111650">think</span>
  <span m="111830">about</span> <span m="112160">that</span> <span m="112460">y-axis</span>
  <span m="113150">as</span> <span m="113210">summarizing</span> <span m="114320">the</span>
  <span m="114380">amount</span> <span m="114650">of</span> <span m="114740">symptoms</span>
  <span m="115280">that a</span> <span m="115490">patient</span> <span m="115770">is</span>
  <span m="115890">reporting</span> <span m="116490">or</span> <span m="120250">the</span>
  <span m="120560">amount</span> <span m="120740">of</span> <span m="120830">pain</span>
  <span m="121040">medication</span> <span m="121520">that</span> <span m="121640">they're</span>
  <span m="121760">taking,</span> <span m="122870">or</span> <span m="123290">some</span>
  <span m="123590">measure</span> <span m="124070">of</span> <span m="124550">what's</span>
  <span m="124850">going</span> <span m="125000">on</span> <span m="125090">with</span>
  <span m="125240">them.</span> <span m="126680">And</span> <span m="127700">initially,</span>
  <span m="129080">that</span> <span m="129289">disease</span> <span m="129590">burden</span>
  <span m="129830">might</span> <span m="129979">be</span> <span m="130100">somewhat</span>
  <span m="130400">low,</span> <span m="130669">and</span> <span m="130759">maybe</span>
  <span m="131120">even</span> <span m="131510">the</span> <span m="131630">patient's</span>
  <span m="132020">in</span> <span m="132140">an</span> <span m="132260">undiagnosed</span>
  <span m="132950">disease</span> <span m="133190">state</span> <span m="133430">at</span>
  <span m="133520">that</span> <span m="133700">time.</span> <span m="135590">As</span>
  <span m="135890">the</span> <span m="136010">symptoms</span> <span m="136520">get</span>
  <span m="136790">worse</span> <span m="137090">and</span> <span m="137180">worse,</span>
  <span m="137750">at</span> <span m="137840">some</span> <span m="138020">point</span>
  <span m="138230">the</span> <span m="138290">patient</span> <span m="138560">might</span>
  <span m="138680">be</span> <span m="138830">diagnosed.</span> <span m="139175">And</span>
  <span m="139520">that's</span> <span m="139640">what</span> <span m="139730">I'm</span>
  <span m="139790">illustrating</span> <span m="140240">by</span> <span m="140420">this</span>
  <span m="140960">gray</span> <span m="141230">curve.</span> <span m="141500">This</span>
  <span m="141650">is</span> <span m="141740">the</span> <span m="141830">point</span>
  <span m="142040">in</span> <span m="142100">time</span> <span m="142410">which</span>
  <span m="143070">the</span> <span m="143150">patient</span> <span m="143450">is</span>
  <span m="143540">diagnosed</span> <span m="144020">with</span> <span m="144120">their</span>
  <span m="144200">disease.</span></p><p><span m="146360">At</span> <span m="146480">the</span>
  <span m="146540">time</span> <span m="146720">of</span> <span m="146780">diagnosis,</span>
  <span m="147590">a</span> <span m="147650">variety</span> <span m="147950">of</span>
  <span m="148010">things</span> <span m="148220">might</span> <span m="148400">happen.</span>
  <span m="149420">The</span> <span m="149480">patient</span> <span m="149840">might</span>
  <span m="150140">begin</span> <span m="150530">treatment.</span> <span m="151190">And</span>
  <span m="151280">that</span> <span m="151400">treatment</span> <span m="151970">might,</span>
  <span m="152300">for</span> <span m="152450">example,</span> <span m="152870">start</span>
  <span m="153170">to</span> <span m="154010">influence</span> <span m="154520">the</span>
  <span m="154640">disease</span> <span m="154910">burden.</span> <span m="155450">And</span>
  <span m="155540">you</span> <span m="155600">might</span> <span m="155780">see</span>
  <span m="155930">a</span> <span m="155990">drop</span> <span m="156320">in</span>
  <span m="156440">disease</span> <span m="156680">burden</span> <span m="156980">initially.</span></p><p><span
  m="158120">This</span> <span m="158300">is</span> <span m="158420">a</span> <span
  m="158480">cancer.</span> <span m="159860">Unfortunately,</span> <span m="160490">often</span>
  <span m="162020">we'll</span> <span m="162170">see</span> <span m="162440">recurrences</span>
  <span m="162980">of</span> <span m="163040">the</span> <span m="163130">cancer.</span>
  <span m="163920">And</span> <span m="163940">that</span> <span m="164060">might</span>
  <span m="164240">manifest</span> <span m="164870">by</span> <span m="165665">a</span>
  <span m="165980">uphill</span> <span m="166610">peak</span> <span m="166850">again,</span>
  <span m="168650">where</span> <span m="168900">it</span> <span m="168970">is</span>
  <span m="169100">burden</span> <span m="169340">grows.</span> <span m="170660">And</span>
  <span m="171230">once</span> <span m="171440">you</span> <span m="171500">start</span>
  <span m="171720">second-line</span> <span m="172100">treatment,</span> <span m="172700">that</span>
  <span m="172880">might</span> <span m="173180">succeed</span> <span m="173540">in</span>
  <span m="173750">lowering</span> <span m="174080">it</span> <span m="174170">again</span>
  <span m="174470">and</span> <span m="174560">so</span> <span m="174740">on.</span>
  <span m="174990">And</span> <span m="175090">this</span> <span m="175490">might</span>
  <span m="175670">be</span> <span m="175760">a</span> <span m="175820">cycle</span>
  <span m="176180">that</span> <span m="176270">repeats</span> <span m="176600">over</span>
  <span m="176780">and</span> <span m="176870">over</span> <span m="177020">again.</span></p><p><span
  m="178130">For</span> <span m="178310">other</span> <span m="178460">diseases</span>
  <span m="180800">for</span> <span m="180980">which</span> <span m="181160">have</span>
  <span m="181340">no</span> <span m="181550">cure,</span> <span m="181910">for</span>
  <span m="182060">example,</span> <span m="182480">but</span> <span m="182630">which</span>
  <span m="182810">are</span> <span m="182900">managed</span> <span m="183410">on</span>
  <span m="183500">a</span> <span m="183590">day-to-day</span> <span m="184040">basis--</span>
  <span m="184520">and we'll</span> <span m="184640">talk</span> <span m="184820">about</span>
  <span m="184940">some</span> <span m="185090">of</span> <span m="185150">those--</span>
  <span m="185870">you</span> <span m="185960">might</span> <span m="186110">see,</span>
  <span m="187100">even</span> <span m="187310">on</span> <span m="187400">a</span>
  <span m="187460">day-by-day</span> <span m="188450">basis,</span> <span m="189230">fluctuations.</span>
  <span m="190310">Or</span> <span m="190430">you</span> <span m="190490">might</span>
  <span m="190670">see</span> <span m="191240">nothing</span> <span m="191570">happening</span>
  <span m="191960">for</span> <span m="192110">a</span> <span m="192140">while.</span>
  <span m="192680">And</span> <span m="192800">then,</span> <span m="193250">for</span>
  <span m="193340">example,</span> <span m="193640">in</span> <span m="193730">autoimmune</span>
  <span m="194090">diseases,</span> <span m="194470">you'll</span> <span m="194570">see</span>
  <span m="194720">these</span> <span m="194870">flare-ups</span> <span m="195830">where
  the</span> <span m="195960">disease</span> <span m="196250">burden</span> <span
  m="196550">grows</span> <span m="196880">a</span> <span m="196940">lot,</span> <span
  m="197690">then</span> <span m="197840">comes</span> <span m="198080">down</span>
  <span m="198290">again.</span> <span m="198530">It's</span> <span m="198650">really</span>
  <span m="199040">inexplicable</span> <span m="199730">why</span> <span m="200000">that</span>
  <span m="200150">happens.</span></p><p><span m="202350">So</span> <span m="202640">the</span>
  <span m="202730">types</span> <span m="202960">of</span> <span m="203030">questions</span>
  <span m="203360">that</span> <span m="203450">we'd</span> <span m="203600">like</span>
  <span m="203750">to</span> <span m="203840">really</span> <span m="204020">understand</span>
  <span m="204560">here</span> <span m="205130">are,</span> <span m="205670">first,</span>
  <span m="208220">where</span> <span m="208490">is</span> <span m="208610">the</span>
  <span m="208670">patient</span> <span m="209000">in</span> <span m="209090">their</span>
  <span m="209180">disease</span> <span m="209480">trajectory?</span> <span m="209930">So</span>
  <span m="210080">a</span> <span m="210110">patient</span> <span m="210410">comes</span>
  <span m="210740">in</span> <span m="210860">today.</span> <span m="213290">And</span>
  <span m="213860">they</span> <span m="214010">might</span> <span m="214190">be</span>
  <span m="214700">diagnosed</span> <span m="215750">today</span> <span m="216140">because</span>
  <span m="216740">of</span> <span m="217550">symptoms</span> <span m="217970">somehow</span>
  <span m="218330">crossing</span> <span m="219810">some</span> <span m="220280">threshold</span>
  <span m="220890">and</span> <span m="220910">them</span> <span m="221060">coming</span>
  <span m="221300">into</span> <span m="221450">the</span> <span m="221540">doctor's</span>
  <span m="221870">office.</span> <span m="222900">But</span> <span m="223070">they</span>
  <span m="223220">could</span> <span m="223400">be</span> <span m="223520">sort</span>
  <span m="223700">of</span> <span m="223850">anywhere</span> <span m="224420">in</span>
  <span m="224510">this</span> <span m="224660">disease</span> <span m="225020">trajectory</span>
  <span m="225910">at</span> <span m="226060">the</span> <span m="226130">time</span>
  <span m="226340">of</span> <span m="226430">diagnosis.</span></p><p><span m="228510">And</span>
  <span m="229430">a</span> <span m="229490">key</span> <span m="229670">question</span>
  <span m="230090">is,</span> <span m="230210">can</span> <span m="230360">we</span>
  <span m="230450">stage</span> <span m="231080">patients</span> <span m="231590">to</span>
  <span m="231680">understand,</span> <span m="233340">for</span> <span m="233390">example,</span>
  <span m="234450">things</span> <span m="234680">like,</span> <span m="234860">how</span>
  <span m="235010">long</span> <span m="235250">are</span> <span m="235310">they</span>
  <span m="235430">likely</span> <span m="235670">to</span> <span m="235760">live</span>
  <span m="236810">based</span> <span m="237200">on</span> <span m="237470">what's</span>
  <span m="237710">currently</span> <span m="238040">going</span> <span m="238220">on</span>
  <span m="238310">with</span> <span m="238460">them?</span> <span m="240060">A</span>
  <span m="240160">second</span> <span m="240290">question</span> <span m="240770">is,</span>
  <span m="241310">when</span> <span m="241520">will</span> <span m="241630">the</span>
  <span m="241700">disease</span> <span m="242000">progress?</span> <span m="243710">So</span>
  <span m="244580">if</span> <span m="244700">you</span> <span m="244760">have</span>
  <span m="244850">a</span> <span m="244910">patient</span> <span m="245150">with</span>
  <span m="245240">kidney</span> <span m="245510">disease,</span> <span m="246510">you</span>
  <span m="246610">might</span> <span m="246620">want</span> <span m="246740">to</span>
  <span m="246800">know</span> <span m="246920">something</span> <span m="247220">about,</span>
  <span m="247640">when</span> <span m="247910">will</span> <span m="248000">this</span>
  <span m="248150">patient</span> <span m="248420">kidney</span> <span m="248660">disease</span>
  <span m="250598">need</span> <span m="251855">a</span> <span m="252320">transplant?</span></p><p><span
  m="255440">Another</span> <span m="255740">question</span> <span m="256250">is,</span>
  <span m="256640">how</span> <span m="256810">will</span> <span m="256870">treatment</span>
  <span m="257240">effect</span> <span m="257480">that</span> <span m="257570">disease</span>
  <span m="257810">progression?</span> <span m="258940">That</span> <span m="259130">I'm</span>
  <span m="259250">sort</span> <span m="259399">of</span> <span m="259490">hinting</span>
  <span m="259850">at</span> <span m="260000">here,</span> <span m="260329">when</span>
  <span m="260480">I'm</span> <span m="260600">showing</span> <span m="263126">these</span>
  <span m="263570">valleys</span> <span m="265120">that</span> <span m="265320">we</span>
  <span m="265430">conjecture</span> <span m="265850">to</span> <span m="265910">be</span>
  <span m="266000">affected</span> <span m="266390">by</span> <span m="266510">treatment.</span>
  <span m="267630">But</span> <span m="268580">one</span> <span m="269030">often</span>
  <span m="269300">wants</span> <span m="269480">to</span> <span m="269540">ask</span>
  <span m="269750">counterfactual</span> <span m="270350">questions</span> <span m="270800">like,</span>
  <span m="270950">what</span> <span m="271070">would</span> <span m="271160">happen</span>
  <span m="271430">to</span> <span m="271490">this</span> <span m="271640">patient's</span>
  <span m="272000">disease</span> <span m="272330">progression</span> <span m="272870">if</span>
  <span m="272990">you</span> <span m="273080">did</span> <span m="273400">one</span>
  <span m="273650">treatment</span> <span m="274070">therapy</span> <span m="274490">versus</span>
  <span m="274730">another</span> <span m="274940">treatment</span> <span m="275180">therapy?</span></p><p><span
  m="277230">So</span> <span m="277250">the</span> <span m="277310">example</span>
  <span m="277730">that</span> <span m="277850">I'm</span> <span m="278210">mentioning</span>
  <span m="278630">here</span> <span m="278780">in</span> <span m="278840">this</span>
  <span m="278930">slide</span> <span m="279890">is</span> <span m="280310">a</span>
  <span m="280640">rare</span> <span m="280850">blood</span> <span m="281090">cancer</span>
  <span m="281720">named</span> <span m="282290">multiple</span> <span m="282620">myeloma.</span>
  <span m="285200">It's</span> <span m="285890">rare.</span> <span m="286460">And</span>
  <span m="286640">so</span> <span m="287330">you</span> <span m="287600">often</span>
  <span m="287870">won't</span> <span m="288080">find</span> <span m="288350">data</span>
  <span m="288560">sets</span> <span m="288800">with</span> <span m="288980">that</span>
  <span m="289130">many</span> <span m="289310">patients</span> <span m="289670">in</span>
  <span m="289730">them.</span> <span m="290640">So</span> <span m="290660">for</span>
  <span m="290750">example,</span> <span m="291330">this</span> <span m="291440">data</span>
  <span m="291600">set</span> <span m="291800">which</span> <span m="291980">I'm</span>
  <span m="292070">listening</span> <span m="292310">in</span> <span m="292370">the</span>
  <span m="292430">very</span> <span m="292580">bottom</span> <span m="292850">here</span>
  <span m="293060">from</span> <span m="293180">the</span> <span m="293240">Multiple</span>
  <span m="293420">Myeloma</span> <span m="293660">Research</span> <span m="293900">Foundation</span>
  <span m="294200">CoMMpass</span> <span m="294560">study</span> <span m="295370">has</span>
  <span m="295550">roughly</span> <span m="295790">1,000</span> <span m="296210">patients.</span></p><p><span
  m="296720">And</span> <span m="297050">it's</span> <span m="297170">a</span> <span
  m="297200">publicly</span> <span m="297590">available</span> <span m="297800">data
  set.</span> <span m="298090">Any of</span> <span m="298330">you</span> <span m="298460">can</span>
  <span m="298640">download</span> <span m="299000">it</span> <span m="299060">today.</span>
  <span m="299840">And</span> <span m="299930">you</span> <span m="299990">could</span>
  <span m="300080">study</span> <span m="300350">questions</span> <span m="300740">like</span>
  <span m="300890">this</span> <span m="301220">about</span> <span m="301460">disease</span>
  <span m="301700">progression.</span> <span m="302150">Because</span> <span m="302450">you</span>
  <span m="302540">can</span> <span m="303080">look</span> <span m="303260">at</span>
  <span m="303380">laboratory</span> <span m="303860">tests</span> <span m="304130">across</span>
  <span m="304460">time.</span> <span m="304850">You</span> <span m="305180">could</span>
  <span m="305300">look</span> <span m="305480">at</span> <span m="305930">when</span>
  <span m="306140">symptoms</span> <span m="306560">start</span> <span m="306830">to</span>
  <span m="306950">rise.</span> <span m="307530">You</span> <span m="307550">have</span>
  <span m="307670">information</span> <span m="308120">about</span> <span m="308240">what</span>
  <span m="308400">treatments</span> <span m="308700">a</span> <span m="308810">patient</span>
  <span m="309110">is</span> <span m="309200">on.</span> <span m="309390">And</span>
  <span m="309480">you</span> <span m="309540">have</span> <span m="309650">outcomes,</span>
  <span m="310160">like</span> <span m="310370">death.</span></p><p><span m="315540">So</span>
  <span m="315960">for</span> <span m="316140">multiple</span> <span m="316410">myeloma,</span>
  <span m="317880">today's</span> <span m="318210">standard</span> <span m="318870">for</span>
  <span m="319020">how</span> <span m="319200">one</span> <span m="319410">would</span>
  <span m="319560">attempt</span> <span m="319830">to</span> <span m="319920">stage</span>
  <span m="320370">a</span> <span m="320400">patient</span> <span m="320820">looks</span>
  <span m="321000">a</span> <span m="321030">little</span> <span m="321180">bit</span>
  <span m="321330">like</span> <span m="321480">this.</span> <span m="323970">Here</span>
  <span m="324210">I'm</span> <span m="324300">showing</span> <span m="324510">you</span>
  <span m="324600">two</span> <span m="324750">different</span> <span m="324990">staging</span>
  <span m="325350">systems.</span> <span m="326100">On</span> <span m="326190">the</span>
  <span m="326280">left</span> <span m="326610">is</span> <span m="326760">a</span>
  <span m="326820">Durie-Salmon</span> <span m="327900">Staging</span> <span m="328230">System,</span>
  <span m="329310">which</span> <span m="329490">is</span> <span m="329580">a</span>
  <span m="329640">bit</span> <span m="329790">older.</span> <span m="330240">On</span>
  <span m="330330">the</span> <span m="330420">right</span> <span m="330750">is</span>
  <span m="330840">what's</span> <span m="330960">called</span> <span m="331140">the</span>
  <span m="331260">Revised</span> <span m="331890">International</span> <span m="332460">Staging</span>
  <span m="332790">System.</span></p><p><span m="334560">A</span> <span m="334620">patient</span>
  <span m="334920">walks</span> <span m="335220">into</span> <span m="335470">their</span>
  <span m="336240">oncologist's</span> <span m="336720">office</span> <span m="337140">newly</span>
  <span m="337440">diagnosed</span> <span m="337830">with</span> <span m="337900">multiple</span>
  <span m="338160">myeloma.</span> <span m="339090">And</span> <span m="339210">after</span>
  <span m="339450">doing</span> <span m="339780">a</span> <span m="339840">series</span>
  <span m="340200">of</span> <span m="340290">blood</span> <span m="340530">tests,</span>
  <span m="341910">looking</span> <span m="342300">at</span> <span m="342420">quantities</span>
  <span m="342840">such</span> <span m="343080">as</span> <span m="343230">their</span>
  <span m="343410">hemoglobin</span> <span m="343950">rates,</span> <span m="344450">amount</span>
  <span m="344640">of</span> <span m="344700">calcium</span> <span m="345450">in</span>
  <span m="345600">the</span> <span m="345660">blood,</span> <span m="346750">also</span>
  <span m="347160">doing,</span> <span m="347520">let's</span> <span m="347650">say,</span>
  <span m="348000">a</span> <span m="348180">biopsy</span> <span m="348700">of</span>
  <span m="348740">the</span> <span m="348810">patient's</span> <span m="349470">bone</span>
  <span m="349740">marrow</span> <span m="350460">to</span> <span m="350880">measure</span>
  <span m="351930">amounts</span> <span m="352290">of</span> <span m="352650">different</span>
  <span m="353340">kinds</span> <span m="353640">of</span> <span m="353760">immunoglobulins,</span>
  <span m="355350">doing</span> <span m="356220">gene</span> <span m="357060">expression</span>
  <span m="357690">assays</span> <span m="358530">to</span> <span m="358650">understand</span>
  <span m="360960">various</span> <span m="361380">different</span> <span m="361770">genetic</span>
  <span m="362130">abnormalities,</span> <span m="363330">that</span> <span m="363510">data</span>
  <span m="363780">will</span> <span m="363870">then</span> <span m="364020">feed</span>
  <span m="364350">into</span> <span m="364740">a</span> <span m="364800">staging</span>
  <span m="365130">system</span> <span m="365430">like</span> <span m="365610">this.</span></p><p><span
  m="366540">So</span> <span m="366780">in</span> <span m="366870">the</span> <span
  m="366960">Durie-Salmon</span> <span m="367500">Staging</span> <span m="367860">System,</span>
  <span m="369450">a</span> <span m="369510">patient</span> <span m="369930">who</span>
  <span m="370040">is</span> <span m="370140">in</span> <span m="370230">stage</span>
  <span m="370620">one</span> <span m="371970">is</span> <span m="372540">found</span>
  <span m="372870">to</span> <span m="372960">have</span> <span m="373530">a</span>
  <span m="374340">very</span> <span m="374700">low</span> <span m="375180">M-component</span>
  <span m="375930">production</span> <span m="376350">rate.</span> <span m="376590">So</span>
  <span m="376710">that's</span> <span m="376950">what</span> <span m="377070">I'm</span>
  <span m="377160">showing</span> <span m="377400">over</span> <span m="377550">here.</span>
  <span m="378620">And</span> <span m="378750">that</span> <span m="378900">really</span>
  <span m="379080">corresponds</span> <span m="379680">to</span> <span m="379800">the</span>
  <span m="379890">amount</span> <span m="380370">of</span> <span m="381270">disease</span>
  <span m="381600">activity</span> <span m="382170">as</span> <span m="382380">measured</span>
  <span m="382740">by</span> <span m="383180">their</span> <span m="383620">immunoglobulins.</span>
  <span m="384860">And</span> <span m="384960">since</span> <span m="385060">this</span>
  <span m="385160">is</span> <span m="385200">a</span> <span m="385320">blood</span>
  <span m="385620">cancer,</span> <span m="387150">that's</span> <span m="387450">a</span>
  <span m="387480">very</span> <span m="387750">good</span> <span m="387870">marker</span>
  <span m="388320">of</span> <span m="388410">what's</span> <span m="388580">going
  on</span> <span m="388740">with</span> <span m="388860">the</span> <span m="388920">patient.</span></p><p><span
  m="391980">So</span> <span m="392350">at sort of</span> <span m="392500">this</span>
  <span m="392670">middle</span> <span m="392940">stage,</span> <span m="393490">which</span>
  <span m="393570">is</span> <span m="393660">called</span> <span m="393900">neither</span>
  <span m="394260">stage</span> <span m="394500">one</span> <span m="394710">nor</span>
  <span m="394860">stage</span> <span m="395160">three,</span> <span m="396030">is</span>
  <span m="396180">characterized</span> <span m="396930">by,</span> <span m="400980">in</span>
  <span m="401070">this</span> <span m="401250">case--</span> <span m="404570">well,</span>
  <span m="404700">I'm</span> <span m="404820">not</span> <span m="404920">going</span>
  <span m="404980">to</span> <span m="405030">talk</span> <span m="405190">with</span>
  <span m="405300">that.</span> <span m="405570">If</span> <span m="405660">you</span>
  <span m="405720">go</span> <span m="405810">to</span> <span m="405900">stage</span>
  <span m="406200">three</span> <span m="406590">for</span> <span m="406740">here,</span>
  <span m="409020">you</span> <span m="409170">see</span> <span m="409290">that</span>
  <span m="409650">the</span> <span m="409800">M-component</span> <span m="410280">levels</span>
  <span m="410550">are</span> <span m="410610">much</span> <span m="410820">higher.</span>
  <span m="411730">If</span> <span m="411750">you</span> <span m="411810">look</span>
  <span m="411990">at</span> <span m="412080">X-ray</span> <span m="412470">studies</span>
  <span m="413040">of</span> <span m="413130">the</span> <span m="413220">patient's</span>
  <span m="413520">bones,</span> <span m="413910">you'll</span> <span m="414030">see</span>
  <span m="414240">that</span> <span m="414420">there</span> <span m="414720">are</span>
  <span m="414990">lytic</span> <span m="415410">bone</span> <span m="415740">lesions,</span>
  <span m="416700">which</span> <span m="416880">are</span> <span m="416940">caused</span>
  <span m="417330">by</span> <span m="417480">the</span> <span m="417540">disease</span>
  <span m="417780">and</span> <span m="417870">really</span> <span m="418090">represent</span>
  <span m="418510">an</span> <span m="418620">advanced</span> <span m="419070">status</span>
  <span m="419520">of</span> <span m="419580">the</span> <span m="419670">disease.</span>
  <span m="421150">And</span> <span m="421410">if</span> <span m="421560">you</span>
  <span m="421650">were</span> <span m="421710">to</span> <span m="421800">measure</span>
  <span m="422160">for</span> <span m="422280">the</span> <span m="422340">patient's</span>
  <span m="422730">urine</span> <span m="423540">the</span> <span m="423600">amount</span>
  <span m="423840">of</span> <span m="423940">light-chain</span> <span m="424440">production,</span>
  <span m="424860">you</span> <span m="424950">see</span> <span m="425070">that</span>
  <span m="425220">it</span> <span m="425320">has</span> <span m="425430">much</span>
  <span m="425670">larger</span> <span m="425970">values</span> <span m="426330">as</span>
  <span m="426420">well.</span></p><p><span m="428440">Now,</span> <span m="429450">this</span>
  <span m="429750">is</span> <span m="429870">an</span> <span m="429990">older</span>
  <span m="430290">staging</span> <span m="430650">system.</span> <span m="431370">In</span>
  <span m="431460">the</span> <span m="431550">middle,</span> <span m="431820">now</span>
  <span m="432000">I'm</span> <span m="432090">showing</span> <span m="432300">you</span>
  <span m="432360">a</span> <span m="432390">newer</span> <span m="432630">staging</span>
  <span m="432930">system,</span> <span m="433200">which</span> <span m="433380">is</span>
  <span m="433470">both</span> <span m="433710">dramatically</span> <span m="434160">simpler</span>
  <span m="434520">and</span> <span m="434700">involves</span> <span m="435150">some</span>
  <span m="435570">newer</span> <span m="435990">components.</span> <span m="437070">So</span>
  <span m="437430">for</span> <span m="437550">example,</span> <span m="438420">in</span>
  <span m="438540">stage</span> <span m="438870">one,</span> <span m="439260">it</span>
  <span m="439470">looks</span> <span m="439740">at</span> <span m="439800">just</span>
  <span m="440040">four</span> <span m="440340">quantities.</span> <span m="441870">First</span>
  <span m="442260">it</span> <span m="442320">looks</span> <span m="442560">at</span>
  <span m="442650">the</span> <span m="442740">patient's</span> <span m="443160">albumin</span>
  <span m="443730">and</span> <span m="443940">beta-2</span> <span m="444330">microglobulin</span>
  <span m="444990">levels.</span> <span m="445480">Those</span> <span m="445620">are</span>
  <span m="446070">biomarkers</span> <span m="446610">that</span> <span m="446670">can</span>
  <span m="446760">be</span> <span m="446820">easily</span> <span m="447120">measured</span>
  <span m="447420">from</span> <span m="447600">the</span> <span m="447660">blood.</span>
  <span m="449310">And</span> <span m="450120">it</span> <span m="450270">says</span>
  <span m="450690">no</span> <span m="451200">high-risk</span> <span m="451920">cytogenetics.</span>
  <span m="452790">So</span> <span m="452940">now</span> <span m="453150">we're</span>
  <span m="453270">starting</span> <span m="453510">to</span> <span m="453600">bring</span>
  <span m="453780">in</span> <span m="453870">genetic</span> <span m="454380">quantities</span>
  <span m="454890">in</span> <span m="454980">terms</span> <span m="455190">of</span>
  <span m="455250">quantifying</span> <span m="455880">risk</span> <span m="456120">levels.</span></p><p><span
  m="457260">Stage</span> <span m="457650">three</span> <span m="458520">is</span>
  <span m="460500">characterized</span> <span m="461010">by</span> <span m="461340">significantly</span>
  <span m="462030">higher</span> <span m="462330">beta-2</span> <span m="462710">microglobulin</span>
  <span m="463290">levels,</span> <span m="464580">translocations</span> <span m="465570">corresponding</span>
  <span m="465990">to</span> <span m="466050">particular</span> <span m="466410">high-risk</span>
  <span m="466760">types</span> <span m="466890">of</span> <span m="466980">genetics.</span>
  <span m="468180">This</span> <span m="468360">will</span> <span m="468450">not</span>
  <span m="468660">be</span> <span m="468750">the</span> <span m="468810">focus</span>
  <span m="469170">of</span> <span m="469230">the</span> <span m="469290">next</span>
  <span m="469500">two</span> <span m="469600">lectures,</span> <span m="470040">but</span>
  <span m="470250">Pete</span> <span m="470520">is</span> <span m="470640">going</span>
  <span m="470820">to</span> <span m="470910">go</span> <span m="471060">much</span>
  <span m="471330">more</span> <span m="471510">detail</span> <span m="471960">in</span>
  <span m="472090">two</span> <span m="472260">genetic</span> <span m="472680">aspects</span>
  <span m="473190">of</span> <span m="473460">precision</span> <span m="473820">medicine</span>
  <span m="475000">in</span> <span m="475320">a</span> <span m="475380">week</span>
  <span m="475560">and</span> <span m="475650">a</span> <span m="475680">half</span>
  <span m="475890">now.</span> <span m="479340">And</span> <span m="479740">in</span>
  <span m="479850">this</span> <span m="480060">way,</span> <span m="480720">each</span>
  <span m="480930">one</span> <span m="481080">of</span> <span m="481170">these</span>
  <span m="481590">stages</span> <span m="482370">represents</span> <span m="482850">something</span>
  <span m="484791">about</span> <span m="485730">the</span> <span m="486150">belief</span>
  <span m="486600">of</span> <span m="486780">how</span> <span m="487020">far</span>
  <span m="487200">along</span> <span m="487410">the</span> <span m="487470">patient</span>
  <span m="487830">is</span> <span m="488640">and</span> <span m="489540">is</span>
  <span m="489720">really</span> <span m="490350">strongly</span> <span m="490860">used</span>
  <span m="491130">to</span> <span m="491250">guide</span> <span m="492000">treatment</span>
  <span m="492860">therapy.</span> <span m="493230">So</span> <span m="493320">for</span>
  <span m="493410">example,</span> <span m="494280">patient</span> <span m="494670">is</span>
  <span m="494760">in</span> <span m="494850">stage</span> <span m="495210">one,</span>
  <span m="495860">an</span> <span m="495960">oncologist</span> <span m="496380">might</span>
  <span m="496530">decide</span> <span m="496860">we're</span> <span m="496950">not</span>
  <span m="497100">going</span> <span m="497280">to</span> <span m="497370">treat</span>
  <span m="497550">this</span> <span m="497700">patient</span> <span m="498000">today.</span></p><p><span
  m="503140">So</span> <span m="504100">a</span> <span m="504160">different</span>
  <span m="504430">type</span> <span m="504610">of</span> <span m="504670">question,</span>
  <span m="505930">whereas</span> <span m="506290">you</span> <span m="506410">could</span>
  <span m="506500">think</span> <span m="506650">about</span> <span m="506800">this</span>
  <span m="507070">as</span> <span m="507190">being</span> <span m="507520">one</span>
  <span m="508000">of</span> <span m="509260">characterizing</span> <span m="510010">on</span>
  <span m="510190">a</span> <span m="510340">patient-specific</span> <span m="511900">level--</span>
  <span m="512890">one</span> <span m="513159">patient</span> <span m="513490">walks</span>
  <span m="513820">in.</span> <span m="514059">We</span> <span m="514179">want</span>
  <span m="514299">to</span> <span m="514360">stage</span> <span m="514690">that</span>
  <span m="514840">specific</span> <span m="515470">patient.</span> <span m="516240">And</span>
  <span m="516370">we're</span> <span m="516460">going</span> <span m="516610">to</span>
  <span m="516730">look</span> <span m="516940">at</span> <span m="517059">some</span>
  <span m="517510">long-term</span> <span m="517990">outcomes</span> <span m="519070">and</span>
  <span m="519190">look</span> <span m="519370">at</span> <span m="519600">the</span>
  <span m="519659">correlation</span> <span m="520100">between</span> <span m="520240">stage</span>
  <span m="520590">and</span> <span m="520690">long-term</span> <span m="520990">outcomes.</span>
  <span m="522230">A</span> <span m="522340">very</span> <span m="522580">different</span>
  <span m="522820">question</span> <span m="523210">is</span> <span m="523480">a</span>
  <span m="523600">descriptive-type</span> <span m="524500">question.</span> <span
  m="526000">Can</span> <span m="526120">we</span> <span m="526240">say</span> <span
  m="526540">what</span> <span m="526810">will</span> <span m="526940">the</span>
  <span m="527050">typical</span> <span m="527590">trajectory</span> <span m="528640">of</span>
  <span m="528760">this</span> <span m="528940">disease</span> <span m="529300">look</span>
  <span m="529480">like?</span></p><p><span m="532340">So</span> <span m="533030">for</span>
  <span m="533150">example,</span> <span m="533810">we'll</span> <span m="533930">talk</span>
  <span m="534200">about</span> <span m="534380">Parkinson's</span> <span m="534890">disease</span>
  <span m="535190">for</span> <span m="535250">the</span> <span m="535310">next</span>
  <span m="535520">couple</span> <span m="535700">of</span> <span m="535790">minutes.</span>
  <span m="536180">Parkinson's</span> <span m="536720">disease</span> <span m="537230">is</span>
  <span m="537440">a</span> <span m="537500">progressive</span> <span m="538910">nervous</span>
  <span m="539210">system</span> <span m="539540">disorder.</span> <span m="540530">It's</span>
  <span m="540650">a</span> <span m="540680">very</span> <span m="540920">common</span>
  <span m="541310">one,</span> <span m="541490">as</span> <span m="541640">opposed</span>
  <span m="541880">to</span> <span m="541970">multiple</span> <span m="542210">myeloma.</span>
  <span m="542630">Parkinson's</span> <span m="543140">affects</span> <span m="544040">over</span>
  <span m="544310">1</span> <span m="544520">in</span> <span m="544590">100</span>
  <span m="545090">people,</span> <span m="545930">age</span> <span m="547050">60</span>
  <span m="547370">and</span> <span m="547520">above.</span> <span m="548990">And</span>
  <span m="550160">like</span> <span m="550430">multiple</span> <span m="550640">myeloma,</span>
  <span m="550940">there</span> <span m="551020">is</span> <span m="551150">also</span>
  <span m="551720">disease</span> <span m="552380">registries</span> <span m="553280">that</span>
  <span m="553580">are</span> <span m="553700">publicly</span> <span m="554060">available</span>
  <span m="554390">and</span> <span m="554480">that</span> <span m="554990">you could</span>
  <span m="555270">use to</span> <span m="555450">study</span> <span m="556130">Parkinson's.</span></p><p><span
  m="560150">Now,</span> <span m="560480">various</span> <span m="560750">researchers</span>
  <span m="561140">have</span> <span m="561320">used</span> <span m="561590">those</span>
  <span m="561770">data</span> <span m="561920">sets</span> <span m="562130">in</span>
  <span m="562220">the</span> <span m="562280">past.</span> <span m="562700">And</span>
  <span m="562820">they've</span> <span m="563000">created</span> <span m="564140">something
  that</span> <span m="564440">looks</span> <span m="564650">a</span> <span m="564710">little</span>
  <span m="564860">bit</span> <span m="564980">like</span> <span m="565190">this</span>
  <span m="565880">to</span> <span m="566000">try</span> <span m="566180">to</span>
  <span m="566270">characterize,</span> <span m="566930">at</span> <span m="567050">now</span>
  <span m="567230">a</span> <span m="567290">population</span> <span m="568100">level,</span>
  <span m="568400">what</span> <span m="568580">it</span> <span m="568670">means</span>
  <span m="569150">for</span> <span m="569270">a</span> <span m="569300">patient</span>
  <span m="569630">to</span> <span m="569720">progress</span> <span m="570200">through</span>
  <span m="570380">their</span> <span m="570470">disease.</span> <span m="573310">So</span>
  <span m="573490">on</span> <span m="573550">the</span> <span m="573850">x-axis,</span>
  <span m="574330">again,</span> <span m="574600">I</span> <span m="574690">have</span>
  <span m="574990">time</span> <span m="575380">now.</span> <span m="576160">On</span>
  <span m="576520">the</span> <span m="576580">y-axis,</span> <span m="577270">again,</span>
  <span m="577920">it</span> <span m="578050">denotes</span> <span m="578420">some</span>
  <span m="578650">level</span> <span m="579160">of</span> <span m="579580">disease</span>
  <span m="580130">disability.</span> <span m="581930">But</span> <span m="581950">what</span>
  <span m="582040">we're</span> <span m="582160">showing</span> <span m="582490">here</span>
  <span m="582790">now</span> <span m="583210">are</span> <span m="583600">symptoms</span>
  <span m="584200">that</span> <span m="584320">might</span> <span m="584530">arise</span>
  <span m="584860">at</span> <span m="584920">different</span> <span m="585190">parts</span>
  <span m="585430">of</span> <span m="585490">the</span> <span m="585580">disease</span>
  <span m="585790">stage.</span></p><p><span m="587080">So</span> <span m="588280">very</span>
  <span m="588640">early</span> <span m="589090">in</span> <span m="589210">Parkinson's,</span>
  <span m="589780">you</span> <span m="589840">might</span> <span m="589990">have</span>
  <span m="590200">some</span> <span m="590410">sleep</span> <span m="590680">behavior</span>
  <span m="591070">disorders,</span> <span m="591570">some</span> <span m="591760">depression,</span>
  <span m="592480">maybe</span> <span m="592690">constipation,</span> <span m="593410">anxiety.</span>
  <span m="594910">As</span> <span m="595300">the</span> <span m="595600">disease</span>
  <span m="596080">gets</span> <span m="596320">further</span> <span m="596590">and</span>
  <span m="596680">further</span> <span m="597010">along,</span> <span m="597430">you'll</span>
  <span m="597580">see</span> <span m="597730">symptoms</span> <span m="598240">such</span>
  <span m="598600">as</span> <span m="598840">mild</span> <span m="599110">cognitive</span>
  <span m="599560">impairment,</span> <span m="601270">increased</span> <span m="601690">pain.</span>
  <span m="602740">As</span> <span m="603040">the</span> <span m="603130">disease</span>
  <span m="603430">goes</span> <span m="603640">further</span> <span m="604480">on,</span>
  <span m="604930">you'll</span> <span m="605110">see</span> <span m="605560">things</span>
  <span m="605830">like</span> <span m="606010">dementia</span> <span m="606850">and</span>
  <span m="607690">an</span> <span m="608020">increasing</span> <span m="608650">amount</span>
  <span m="608980">of</span> <span m="609070">psychotic</span> <span m="609550">symptoms.</span></p><p><span
  m="612920">And</span> <span m="613180">information</span> <span m="613600">like</span>
  <span m="613750">this</span> <span m="613930">can</span> <span m="614050">be</span>
  <span m="614110">extremely</span> <span m="614590">valuable</span> <span m="615010">for</span>
  <span m="615130">a</span> <span m="615160">patient</span> <span m="615790">who</span>
  <span m="616210">is</span> <span m="616390">newly</span> <span m="616660">diagnosed</span>
  <span m="617020">with</span> <span m="617110">a</span> <span m="617170">disease.</span>
  <span m="617770">They</span> <span m="617890">might</span> <span m="618040">want</span>
  <span m="618250">to</span> <span m="618340">make</span> <span m="618580">life</span>
  <span m="618850">decisions</span> <span m="619360">like,</span> <span m="620470">should</span>
  <span m="620680">they</span> <span m="620800">buy</span> <span m="621010">this</span>
  <span m="621190">home?</span> <span m="621910">Should</span> <span m="622180">they</span>
  <span m="622840">stick</span> <span m="623260">with</span> <span m="623410">their</span>
  <span m="623500">current</span> <span m="623830">job?</span> <span m="625090">Can</span>
  <span m="625390">they</span> <span m="625480">have</span> <span m="625660">a</span>
  <span m="625720">baby?</span> <span m="627340">And</span> <span m="627970">all</span>
  <span m="628180">of</span> <span m="628270">these</span> <span m="628480">questions</span>
  <span m="629020">might</span> <span m="629320">really</span> <span m="629800">be</span>
  <span m="629950">impact--</span> <span m="630360">the</span> <span m="630430">answer</span>
  <span m="630680">to</span> <span m="630760">those</span> <span m="630910">questions</span>
  <span m="631240">might</span> <span m="631360">be</span> <span m="631430">really</span>
  <span m="631630">impacted</span> <span m="632140">by</span> <span m="632290">what</span>
  <span m="632470">this</span> <span m="632620">patient</span> <span m="632980">could</span>
  <span m="633190">expect</span> <span m="633880">their</span> <span m="634090">life</span>
  <span m="634330">to</span> <span m="634450">be</span> <span m="634600">like</span>
  <span m="634900">over</span> <span m="635020">the</span> <span m="635080">next</span>
  <span m="635620">couple</span> <span m="635860">of</span> <span m="635950">years,</span>
  <span m="636310">over</span> <span m="636400">the</span> <span m="636460">next</span>
  <span m="636700">10</span> <span m="636910">years</span> <span m="637150">or the</span>
  <span m="637210">next</span> <span m="637390">20</span> <span m="637660">years.</span>
  <span m="638940">And</span> <span m="639040">so</span> <span m="639140">if</span>
  <span m="639240">one</span> <span m="639310">could</span> <span m="639430">characterize</span>
  <span m="640090">really</span> <span m="640300">well</span> <span m="640600">what</span>
  <span m="640870">the</span> <span m="640990">disease</span> <span m="641590">trajectory</span>
  <span m="642190">might</span> <span m="642400">look</span> <span m="642670">like,</span>
  <span m="643330">it will</span> <span m="643450">be</span> <span m="643570">incredibly</span>
  <span m="644140">valuable</span> <span m="644590">for</span> <span m="644740">guiding</span>
  <span m="645550">those</span> <span m="646480">life</span> <span m="646750">decisions.</span></p><p><span
  m="648280">But</span> <span m="648430">the</span> <span m="648490">challenge</span>
  <span m="648970">is</span> <span m="649180">that--</span> <span m="650140">this</span>
  <span m="650350">is</span> <span m="650440">for</span> <span m="650560">Parkinson's.</span>
  <span m="651100">And</span> <span m="651190">Parkinson's</span> <span m="651640">is</span>
  <span m="651760">reasonably</span> <span m="652240">well</span> <span m="652360">understood.</span>
  <span m="653600">There</span> <span m="653680">are</span> <span m="653740">a</span>
  <span m="653770">large</span> <span m="654220">number</span> <span m="654520">of</span>
  <span m="654610">diseases</span> <span m="655210">that</span> <span m="655390">are</span>
  <span m="655480">much</span> <span m="655750">more</span> <span m="656290">rare,</span>
  <span m="657250">where</span> <span m="658270">any</span> <span m="658480">one</span>
  <span m="658720">clinician</span> <span m="659140">might</span> <span m="659350">see</span>
  <span m="659560">a</span> <span m="659620">very</span> <span m="659800">small</span>
  <span m="660160">number</span> <span m="660400">of</span> <span m="660460">patients</span>
  <span m="660910">in</span> <span m="660970">their</span> <span m="661090">clinic.</span>
  <span m="662110">And</span> <span m="662620">figuring</span> <span m="663010">out,</span>
  <span m="663220">really,</span> <span m="664180">how</span> <span m="664360">do</span>
  <span m="664420">we</span> <span m="664540">combine</span> <span m="665320">the</span>
  <span m="665470">symptoms</span> <span m="666160">that</span> <span m="666280">are</span>
  <span m="666370">seen</span> <span m="666670">in</span> <span m="666760">a</span>
  <span m="666820">very</span> <span m="667090">noisy</span> <span m="667510">fashion</span>
  <span m="667930">for</span> <span m="668200">a</span> <span m="668470">small</span>
  <span m="668650">number</span> <span m="668830">of</span> <span m="668890">patients,</span>
  <span m="669730">how</span> <span m="669880">to</span> <span m="669970">bring</span>
  <span m="670150">that</span> <span m="670270">together</span> <span m="670630">to</span>
  <span m="670810">a</span> <span m="670870">coherent</span> <span m="671320">picture</span>
  <span m="671560">like</span> <span m="671740">this</span> <span m="671920">is</span>
  <span m="672040">actually</span> <span m="672310">very,</span> <span m="672620">very</span>
  <span m="672700">challenging.</span> <span m="674090">And</span> <span m="674190">that's</span>
  <span m="674320">where</span> <span m="674470">some</span> <span m="674620">of</span>
  <span m="674680">the</span> <span m="674740">techniques</span> <span m="675130">we'll</span>
  <span m="675220">be</span> <span m="675310">talking</span> <span m="675640">about</span>
  <span m="676480">in</span> <span m="676900">Tuesday's</span> <span m="677350">lecture,</span>
  <span m="677830">which</span> <span m="678010">talks</span> <span m="678280">about</span>
  <span m="678520">how</span> <span m="678730">do</span> <span m="678820">we</span>
  <span m="678970">infer</span> <span m="679330">disease</span> <span m="679600">stages,</span>
  <span m="680530">how</span> <span m="680680">do</span> <span m="680800">we</span>
  <span m="680870">automatically</span> <span m="681220">align</span> <span m="681610">patients</span>
  <span m="682060">across</span> <span m="682450">time,</span> <span m="683230">and</span>
  <span m="683320">how</span> <span m="683450">do</span> <span m="683530">we</span>
  <span m="683620">use</span> <span m="683920">very</span> <span m="684130">noisy</span>
  <span m="684460">data</span> <span m="684730">to</span> <span m="684880">do</span>
  <span m="685030">that,</span> <span m="685240">will</span> <span m="685360">be</span>
  <span m="685480">particularly</span> <span m="685960">valuable.</span></p><p><span
  m="688440">But I</span> <span m="688510">want</span> <span m="688630">to</span>
  <span m="688690">emphasize</span> <span m="689080">one</span> <span m="689260">last</span>
  <span m="689470">point</span> <span m="689710">regarding</span> <span m="690130">this</span>
  <span m="690370">descriptive</span> <span m="691000">question.</span> <span m="691870">This</span>
  <span m="692050">is</span> <span m="692170">not</span> <span m="692470">about</span>
  <span m="692740">prediction.</span> <span m="693340">This</span> <span m="693520">is</span>
  <span m="693580">about</span> <span m="693790">understanding,</span> <span m="696190">whereas</span>
  <span m="696520">the</span> <span m="696580">previous</span> <span m="697270">slide</span>
  <span m="697840">was</span> <span m="698380">about</span> <span m="698590">prognosis,</span>
  <span m="699440">which</span> <span m="699490">is</span> <span m="699580">very</span>
  <span m="699730">much</span> <span m="699910">a</span> <span m="699940">prediction-like</span>
  <span m="700960">question.</span></p><p><span m="702880">Now,</span> <span m="703450">a</span>
  <span m="703870">different</span> <span m="704170">type</span> <span m="704560">of</span>
  <span m="704920">understanding</span> <span m="705880">question</span> <span m="708600">is</span>
  <span m="708750">that</span> <span m="709050">of</span> <span m="709530">disease</span>
  <span m="709830">subtyping.</span> <span m="711480">Here,</span> <span m="711780">again,</span>
  <span m="712260">you</span> <span m="712350">might</span> <span m="712500">be</span>
  <span m="712590">interested</span> <span m="713220">in</span> <span m="714240">identifying,</span>
  <span m="716460">for</span> <span m="716880">a</span> <span m="716940">single</span>
  <span m="717360">patient,</span> <span m="718860">are</span> <span m="718980">they</span>
  <span m="719100">likely</span> <span m="719490">to</span> <span m="719640">progress</span>
  <span m="720150">quickly</span> <span m="720810">through</span> <span m="720960">their</span>
  <span m="721080">disease?</span> <span m="721440">Are</span> <span m="721530">they</span>
  <span m="721620">likely</span> <span m="721770">to</span> <span m="721950">progress</span>
  <span m="722280">slowly</span> <span m="722820">through</span> <span m="722970">their</span>
  <span m="723090">disease?</span> <span m="723560">Are</span> <span m="723570">they</span>
  <span m="723690">likely</span> <span m="723960">to</span> <span m="724020">respond</span>
  <span m="724830">to</span> <span m="725400">treatment?</span> <span m="725810">Are</span>
  <span m="725880">they</span> <span m="726000">not</span> <span m="726270">likely</span>
  <span m="726510">to</span> <span m="726570">respond</span> <span m="726990">to</span>
  <span m="727110">treatment?</span></p><p><span m="728100">But</span> <span m="728190">we'd</span>
  <span m="728310">like</span> <span m="728470">to be able to</span> <span m="728730">characterize</span>
  <span m="729420">that</span> <span m="729540">heterogeneity</span> <span m="731250">across</span>
  <span m="731730">the</span> <span m="731820">whole</span> <span m="731940">population</span>
  <span m="732540">and</span> <span m="732630">summarize</span> <span m="733320">it</span>
  <span m="733440">into</span> <span m="733740">a</span> <span m="733800">small</span>
  <span m="734250">number</span> <span m="734520">of</span> <span m="734610">subtypes.</span>
  <span m="736020">And</span> <span m="736200">you</span> <span m="736260">might</span>
  <span m="736410">think</span> <span m="736620">about</span> <span m="736800">this</span>
  <span m="736950">as</span> <span m="737070">redefining</span> <span m="737730">disease</span>
  <span m="738030">altogether.</span> <span m="739230">So</span> <span m="739380">today,</span>
  <span m="740310">we</span> <span m="740430">might</span> <span m="740610">say</span>
  <span m="740940">patients</span> <span m="741930">who</span> <span m="742110">have</span>
  <span m="742710">a</span> <span m="742830">particular</span> <span m="744270">blood</span>
  <span m="744750">abnormality,</span> <span m="745560">we</span> <span m="745680">will</span>
  <span m="745780">say</span> <span m="746040">are</span> <span m="746130">multiple</span>
  <span m="746490">myeloma</span> <span m="746850">patients.</span> <span m="747940">But</span>
  <span m="748920">as</span> <span m="749100">we</span> <span m="749220">learn</span>
  <span m="749460">more</span> <span m="749640">and</span> <span m="749730">more</span>
  <span m="749850">about</span> <span m="750030">cancer,</span> <span m="750510">we</span>
  <span m="750750">increasingly</span> <span m="751350">understand</span> <span m="752010">that,</span>
  <span m="752130">in</span> <span m="752220">fact,</span> <span m="753390">every</span>
  <span m="753690">patient's</span> <span m="754050">cancer</span> <span m="754500">is</span>
  <span m="754620">very</span> <span m="754800">unique.</span></p><p><span m="756120">And</span>
  <span m="756210">so</span> <span m="757110">over</span> <span m="757350">time,</span>
  <span m="758010">we're</span> <span m="758190">going</span> <span m="758460">to</span>
  <span m="758610">be</span> <span m="759030">subdividing</span> <span m="760110">diseases,</span>
  <span m="760710">and</span> <span m="760830">in</span> <span m="760920">other</span>
  <span m="761100">cases</span> <span m="761430">combining</span> <span m="762060">things</span>
  <span m="762240">that</span> <span m="762330">we</span> <span m="762420">thought</span>
  <span m="762630">were</span> <span m="763010">different</span> <span m="763350">diseases,</span>
  <span m="763890">into</span> <span m="764160">new</span> <span m="764400">disease</span>
  <span m="764700">categories.</span> <span m="766090">And</span> <span m="766170">in</span>
  <span m="766260">doing</span> <span m="766620">so</span> <span m="767820">it</span>
  <span m="767950">will</span> <span m="768080">allow</span> <span m="768270">us</span>
  <span m="768510">to</span> <span m="769560">better</span> <span m="769860">take</span>
  <span m="770070">care</span> <span m="770280">of</span> <span m="770340">patients</span>
  <span m="771895">by,</span> <span m="772320">first</span> <span m="772530">of</span>
  <span m="772590">all,</span> <span m="772680">coming</span> <span m="772840">up</span>
  <span m="772920">with</span> <span m="773070">guidelines</span> <span m="773700">that</span>
  <span m="773820">are</span> <span m="773880">specific</span> <span m="774570">to</span>
  <span m="774840">each</span> <span m="775050">of</span> <span m="775140">these</span>
  <span m="775380">disease</span> <span m="775710">subtypes.</span> <span m="777450">And</span>
  <span m="779120">it</span> <span m="779330">will</span> <span m="779430">allow</span>
  <span m="779700">us</span> <span m="779820">to</span> <span m="780000">make</span>
  <span m="780450">better</span> <span m="780750">predictions</span> <span m="781980">based</span>
  <span m="782280">on</span> <span m="782370">these</span> <span m="782520">guidelines.</span>
  <span m="782880">So</span> <span m="782970">we</span> <span m="783060">can</span>
  <span m="783180">say</span> <span m="783450">a</span> <span m="783510">patient</span>
  <span m="784050">like</span> <span m="784350">this,</span> <span m="784725">in</span>
  <span m="785100">subtype</span> <span m="785580">A,</span> <span m="785880">is</span>
  <span m="786030">likely</span> <span m="786330">to</span> <span m="786420">have</span>
  <span m="786600">the</span> <span m="786690">following</span> <span m="787050">disease</span>
  <span m="787290">progression.</span> <span m="788100">A</span> <span m="788160">patient</span>
  <span m="788430">like</span> <span m="788610">this,</span> <span m="788910">in</span>
  <span m="789000">subtype</span> <span m="789420">B,</span> <span m="789780">is</span>
  <span m="789930">likely</span> <span m="790200">to</span> <span m="790260">have</span>
  <span m="790410">a</span> <span m="790470">different</span> <span m="790740">disease</span>
  <span m="790950">progression</span> <span m="791550">or</span> <span m="791670">be
  a</span> <span m="791790">responder</span> <span m="792240">or a</span> <span m="792360">non-responder.</span></p><p><span
  m="794940">So</span> <span m="795060">here's</span> <span m="795270">an</span> <span
  m="795330">example</span> <span m="796020">of</span> <span m="796530">such</span>
  <span m="797010">a</span> <span m="797790">characterization.</span> <span m="798940">This</span>
  <span m="799020">is</span> <span m="799110">still</span> <span m="799440">sticking</span>
  <span m="799800">with</span> <span m="799920">the</span> <span m="799980">Parkinson's</span>
  <span m="800520">example.</span> <span m="802830">This</span> <span m="803040">is</span>
  <span m="803160">a</span> <span m="803220">paper</span> <span m="804620">from</span>
  <span m="805080">a</span> <span m="805530">neuropsychiatry</span> <span m="807720">journal.</span>
  <span m="808710">And</span> <span m="808830">it</span> <span m="808920">uses</span>
  <span m="809190">a</span> <span m="809250">clustering-like</span> <span m="809880">algorithm,</span>
  <span m="810230">and</span> <span m="810290">we'll</span> <span m="810390">see</span>
  <span m="810720">many</span> <span m="810930">more</span> <span m="811080">examples</span>
  <span m="811500">of</span> <span m="811560">that</span> <span m="811710">in</span>
  <span m="811800">today's</span> <span m="812040">lecture,</span> <span m="812940">to</span>
  <span m="813210">characterize</span> <span m="814140">patients</span> <span m="814560">into,</span>
  <span m="815310">to</span> <span m="815850">group</span> <span m="816120">patients</span>
  <span m="816510">into,</span> <span m="816660">four</span> <span m="816930">different</span>
  <span m="817230">clusters.</span> <span m="819220">So</span> <span m="819240">let</span>
  <span m="819360">me</span> <span m="819510">walk</span> <span m="819840">you</span>
  <span m="819930">through</span> <span m="820170">this</span> <span m="820350">figure</span>
  <span m="820610">so</span> <span m="820700">you</span> <span m="820770">see</span>
  <span m="820950">how</span> <span m="821040">to</span> <span m="821100">interpret</span>
  <span m="821460">it.</span></p><p><span m="824250">Parkinson's</span> <span m="824760">patients</span>
  <span m="825120">can</span> <span m="825240">be</span> <span m="825300">measured</span>
  <span m="825660">in</span> <span m="825750">terms</span> <span m="826170">of</span>
  <span m="826890">a</span> <span m="826950">few</span> <span m="827130">different</span>
  <span m="827490">axes.</span> <span m="828210">You</span> <span m="828330">could</span>
  <span m="828450">look</span> <span m="828660">at</span> <span m="828780">their</span>
  <span m="828960">motor</span> <span m="829290">progression.</span> <span m="830010">So</span>
  <span m="830490">that</span> <span m="830730">is</span> <span m="830850">shown</span>
  <span m="831150">here</span> <span m="831600">in</span> <span m="831720">the</span>
  <span m="831780">innermost</span> <span m="832290">circle.</span> <span m="833070">And</span>
  <span m="833190">you</span> <span m="833250">see</span> <span m="833400">that</span>
  <span m="833520">patients</span> <span m="834030">in</span> <span m="834360">Cluster</span>
  <span m="834810">2</span> <span m="835560">seem</span> <span m="835770">to</span>
  <span m="835860">have</span> <span m="836550">intermediate-level</span> <span m="837360">motor</span>
  <span m="837630">progression.</span> <span m="838140">Patients</span> <span m="838500">in</span>
  <span m="838570">Cluster</span> <span m="838890">1</span> <span m="839160">have</span>
  <span m="839310">very</span> <span m="839640">fast</span> <span m="840060">motor</span>
  <span m="840300">progression,</span> <span m="840900">means</span> <span m="841140">that</span>
  <span m="841230">their</span> <span m="841350">motor</span> <span m="841680">symptoms</span>
  <span m="842310">get</span> <span m="842550">increasingly</span> <span m="843450">worse</span>
  <span m="844680">very</span> <span m="845130">quickly</span> <span m="845730">over</span>
  <span m="845940">time.</span></p><p><span m="849190">One</span> <span m="849300">could</span>
  <span m="849420">also</span> <span m="849630">look</span> <span m="849900">at</span>
  <span m="850050">the</span> <span m="850110">response</span> <span m="850740">of</span>
  <span m="850830">patients</span> <span m="851310">to</span> <span m="851790">one</span>
  <span m="852000">of</span> <span m="852060">the</span> <span m="852150">drugs,</span>
  <span m="852540">such</span> <span m="852900">as</span> <span m="853170">levodopa</span>
  <span m="854010">that's</span> <span m="854220">used</span> <span m="854490">to</span>
  <span m="854580">treat</span> <span m="854790">patients.</span> <span m="855870">Patients</span>
  <span m="856250">in</span> <span m="856320">Cluster</span> <span m="856680">1</span>
  <span m="856980">are</span> <span m="857040">characterized</span> <span m="857550">by</span>
  <span m="857700">having</span> <span m="857880">a</span> <span m="857940">very</span>
  <span m="858180">poor</span> <span m="858420">response</span> <span m="858870">to</span>
  <span m="858930">that</span> <span m="859110">drug.</span> <span m="859800">Patients</span>
  <span m="860220">in</span> <span m="860280">Cluster</span> <span m="860640">3</span>
  <span m="861660">are</span> <span m="861780">characterized</span> <span m="862380">as</span>
  <span m="862500">having</span> <span m="862980">intermediate,</span> <span m="863580">patients
  in</span> <span m="863940">Cluster</span> <span m="864300">2</span> <span m="864600">as</span>
  <span m="864720">having</span> <span m="865290">good</span> <span m="866040">response</span>
  <span m="866430">to</span> <span m="866520">that</span> <span m="866670">drug.</span></p><p><span
  m="868440">Similarly</span> <span m="868860">one</span> <span m="869070">could</span>
  <span m="869220">look</span> <span m="869490">at</span> <span m="869970">baseline</span>
  <span m="870510">motor</span> <span m="870810">symptoms.</span> <span m="871470">So</span>
  <span m="871680">at</span> <span m="871800">the</span> <span m="871890">time</span>
  <span m="872130">the</span> <span m="872220">patient</span> <span m="873420">is</span>
  <span m="873660">diagnosed</span> <span m="874320">or</span> <span m="874410">comes</span>
  <span m="874620">into</span> <span m="874800">the</span> <span m="874890">clinic</span>
  <span m="875130">for</span> <span m="875220">the</span> <span m="875280">first</span>
  <span m="875430">time</span> <span m="875580">to</span> <span m="875640">manage</span>
  <span m="875850">their</span> <span m="875940">disease,</span> <span m="876720">you</span>
  <span m="876810">can</span> <span m="876930">look</span> <span m="877080">at</span>
  <span m="877620">what</span> <span m="877830">types</span> <span m="878370">of</span>
  <span m="878550">motor-like</span> <span m="879360">symptoms</span> <span m="879780">do</span>
  <span m="879840">they</span> <span m="879990">have.</span> <span m="880360">And</span>
  <span m="880460">again,</span> <span m="880690">you</span> <span m="880710">see</span>
  <span m="880890">different</span> <span m="881790">heterogeneous</span> <span m="883050">aspects</span>
  <span m="883500">to</span> <span m="883590">these</span> <span m="883770">different</span>
  <span m="884010">clusters.</span> <span m="885280">So</span> <span m="885300">this</span>
  <span m="885480">is</span> <span m="885570">one</span> <span m="886050">means--</span>
  <span m="886470">this</span> <span m="886650">is</span> <span m="886710">a</span>
  <span m="886740">very</span> <span m="887070">concrete</span> <span m="887460">way,</span>
  <span m="887730">of what</span> <span m="887880">I</span> <span m="887940">mean</span>
  <span m="888150">by</span> <span m="888300">trying</span> <span m="888510">to</span>
  <span m="888600">subtype</span> <span m="889080">patients.</span></p><p><span m="892390">So</span>
  <span m="893290">we'll</span> <span m="893440">begin</span> <span m="893770">our</span>
  <span m="893860">journey</span> <span m="894250">through</span> <span m="894400">disease</span>
  <span m="894640">progression</span> <span m="895030">modeling</span> <span m="895840">by</span>
  <span m="895990">starting</span> <span m="896350">out</span> <span m="896500">with</span>
  <span m="896680">that</span> <span m="896830">first</span> <span m="897190">question</span>
  <span m="897910">of</span> <span m="898270">prognosis.</span> <span m="901880">And</span>
  <span m="902030">prognosis,</span> <span m="902630">from</span> <span m="902780">my</span>
  <span m="902960">perspective,</span> <span m="903560">is</span> <span m="903740">really</span>
  <span m="904010">a</span> <span m="904130">supervised</span> <span m="904910">machine-learning</span>
  <span m="905480">problem.</span> <span m="908340">So</span> <span m="911140">we</span>
  <span m="911230">can</span> <span m="911380">think</span> <span m="911560">about</span>
  <span m="912040">prognosis</span> <span m="912820">from</span> <span m="913000">the</span>
  <span m="913060">following</span> <span m="913420">perspective.</span></p><p><span
  m="919200">Patient</span> <span m="919530">walks</span> <span m="919890">in</span>
  <span m="920550">at</span> <span m="920670">time</span> <span m="921060">zero.</span>
  <span m="924810">And</span> <span m="925140">you</span> <span m="925230">want</span>
  <span m="925410">to</span> <span m="925500">know</span> <span m="925680">something</span>
  <span m="926160">about</span> <span m="926550">what</span> <span m="926880">will</span>
  <span m="927090">that</span> <span m="927270">patient's</span> <span m="927750">disease</span>
  <span m="928380">status</span> <span m="928920">be</span> <span m="929130">like</span>
  <span m="929490">over</span> <span m="929730">time.</span> <span m="930820">So</span>
  <span m="930900">for</span> <span m="930990">example,</span> <span m="931510">you</span>
  <span m="931610">could</span> <span m="931650">ask,</span> <span m="932790">at</span>
  <span m="933270">six</span> <span m="933720">months,</span> <span m="936940">what</span>
  <span m="937180">is</span> <span m="937300">their</span> <span m="937420">disease</span>
  <span m="937660">status?</span> <span m="938180">And</span> <span m="938470">for</span>
  <span m="938620">this</span> <span m="938800">patient,</span> <span m="939320">it</span>
  <span m="939420">might</span> <span m="939460">be,</span> <span m="939880">let's</span>
  <span m="940060">say,</span> <span m="940870">6</span> <span m="941260">out</span>
  <span m="941380">of</span> <span m="941500">10.</span> <span m="942160">And</span>
  <span m="942610">where</span> <span m="942880">these</span> <span m="943030">numbers</span>
  <span m="943330">are</span> <span m="943390">coming</span> <span m="943630">from</span>
  <span m="943810">will</span> <span m="943900">become</span> <span m="944140">clear</span>
  <span m="944380">in</span> <span m="944470">a</span> <span m="944500">few</span>
  <span m="944650">minutes.</span></p><p><span m="946870">12</span> <span m="947350">months</span>
  <span m="948730">down</span> <span m="948970">the</span> <span m="949060">line,</span>
  <span m="949510">their</span> <span m="949690">disease</span> <span m="949960">status</span>
  <span m="950380">might</span> <span m="950620">be</span> <span m="952360">7</span>
  <span m="952720">out</span> <span m="952810">of</span> <span m="952930">10.</span>
  <span m="954890">18</span> <span m="955350">months,</span> <span m="957660">it</span>
  <span m="957760">might</span> <span m="957970">be</span> <span m="958810">9</span>
  <span m="959230">out</span> <span m="959350">of</span> <span m="959470">10.</span>
  <span m="960910">And</span> <span m="961390">the</span> <span m="961510">goal</span>
  <span m="961870">that</span> <span m="962020">we're</span> <span m="962110">going</span>
  <span m="962290">to</span> <span m="962380">try</span> <span m="962500">to</span>
  <span m="962620">tackle</span> <span m="963100">for</span> <span m="963220">the</span>
  <span m="963310">first</span> <span m="963640">half</span> <span m="963820">of</span>
  <span m="963990">today's</span> <span m="964180">lecture</span> <span m="965170">is</span>
  <span m="965290">this</span> <span m="965440">question</span> <span m="965920">of,</span>
  <span m="966040">how</span> <span m="966220">do</span> <span m="966310">we</span>
  <span m="966430">take</span> <span m="966790">the</span> <span m="966910">data,</span>
  <span m="968170">what</span> <span m="968260">I'll</span> <span m="968350">call</span>
  <span m="968560">the</span> <span m="968710">x</span> <span m="969060">vector,</span>
  <span m="969880">available</span> <span m="970510">for</span> <span m="970660">the</span>
  <span m="970750">patient</span> <span m="971230">at</span> <span m="971380">baseline</span>
  <span m="972580">and</span> <span m="972700">predict</span> <span m="973960">what</span>
  <span m="974260">will</span> <span m="974470">be</span> <span m="974770">these</span>
  <span m="975100">values</span> <span m="976600">at</span> <span m="976990">different</span>
  <span m="977350">time</span> <span m="977650">points?</span></p><p><span m="980020">So</span>
  <span m="980170">you</span> <span m="980260">could</span> <span m="980350">think</span>
  <span m="980590">about</span> <span m="980770">that</span> <span m="980950">as</span>
  <span m="981030">actually</span> <span m="981220">drawing</span> <span m="981850">out</span>
  <span m="982090">this</span> <span m="982300">curve</span> <span m="982600">that</span>
  <span m="982720">I</span> <span m="982810">showed</span> <span m="983050">you</span>
  <span m="983140">earlier.</span> <span m="984700">So</span> <span m="985840">what</span>
  <span m="986050">we</span> <span m="986140">want</span> <span m="986260">to</span>
  <span m="986320">do</span> <span m="986470">is</span> <span m="986590">take</span>
  <span m="986890">the</span> <span m="987370">initial</span> <span m="987910">information</span>
  <span m="988240">we</span> <span m="988330">have</span> <span m="988450">about</span>
  <span m="988600">the</span> <span m="988690">patient</span> <span m="989560">and</span>
  <span m="989710">say,</span> <span m="990220">oh,</span> <span m="990460">the</span>
  <span m="990550">patient's</span> <span m="991180">disease</span> <span m="991510">status,</span>
  <span m="992860">or</span> <span m="992950">their</span> <span m="993070">disease</span>
  <span m="993370">burden,</span> <span m="993850">over</span> <span m="994060">time</span>
  <span m="994360">is</span> <span m="994450">going</span> <span m="994570">to</span>
  <span m="994630">look</span> <span m="994780">a</span> <span m="994840">little</span>
  <span m="994960">bit</span> <span m="995080">like</span> <span m="995200">this.</span>
  <span m="995680">And</span> <span m="995790">for</span> <span m="995920">a</span>
  <span m="995950">different</span> <span m="996250">patient,</span> <span m="996580">based</span>
  <span m="996760">on</span> <span m="996850">their</span> <span m="997000">initial</span>
  <span m="997330">covariance,</span> <span m="997780">you</span> <span m="997840">might</span>
  <span m="998020">say</span> <span m="998230">that</span> <span m="998640">their</span>
  <span m="998830">disease</span> <span m="999100">burden</span> <span m="999340">might</span>
  <span m="999550">look</span> <span m="999760">like</span> <span m="999970">that.</span></p><p><span
  m="1002430">So</span> <span m="1002580">we</span> <span m="1002670">want</span>
  <span m="1002790">to</span> <span m="1002850">be</span> <span m="1002910">able</span>
  <span m="1003030">to</span> <span m="1003090">predict</span> <span m="1003660">these</span>
  <span m="1003900">curves</span> <span m="1004530">in</span> <span m="1004620">this--</span>
  <span m="1005370">for</span> <span m="1005710">this</span> <span m="1005850">presentation,</span>
  <span m="1006400">there</span> <span m="1006480">are</span> <span m="1006570">going</span>
  <span m="1006780">to</span> <span m="1006870">actually</span> <span m="1007110">be</span>
  <span m="1007560">sort</span> <span m="1007710">of</span> <span m="1007770">discrete</span>
  <span m="1008220">time</span> <span m="1008490">points.</span> <span m="1009180">We</span>
  <span m="1009300">want</span> <span m="1009420">to be able to</span> <span m="1009590">predict</span>
  <span m="1010080">that</span> <span m="1010380">curve</span> <span m="1011280">from</span>
  <span m="1011640">the</span> <span m="1011730">baseline</span> <span m="1012240">information</span>
  <span m="1012660">we</span> <span m="1012750">have</span> <span m="1012900">available.</span>
  <span m="1013890">And</span> <span m="1014120">that</span> <span m="1014220">will</span>
  <span m="1014310">give</span> <span m="1014430">us</span> <span m="1014490">some</span>
  <span m="1014760">idea</span> <span m="1015645">of</span> <span m="1016080">how</span>
  <span m="1016320">this</span> <span m="1016440">patient's</span> <span m="1016770">going</span>
  <span m="1016890">to</span> <span m="1016950">progress</span> <span m="1017280">through</span>
  <span m="1017460">their</span> <span m="1017580">disease.</span></p><p><span m="1019810">So</span>
  <span m="1020130">in</span> <span m="1020250">this</span> <span m="1020430">case</span>
  <span m="1020640">study,</span> <span m="1020980">we're</span> <span m="1021080">going</span>
  <span m="1021120">to</span> <span m="1021210">look</span> <span m="1021330">at</span>
  <span m="1021450">Alzheimer's</span> <span m="1021930">disease.</span> <span m="1023220">Here</span>
  <span m="1023460">I'm</span> <span m="1023550">showing</span> <span m="1023910">you</span>
  <span m="1024480">two</span> <span m="1024720">brains,</span> <span m="1025410">a</span>
  <span m="1026099">healthy</span> <span m="1026609">brain</span> <span m="1027150">and</span>
  <span m="1027450">a</span> <span m="1027630">diseased</span> <span m="1028180">brain,</span>
  <span m="1028619">to</span> <span m="1028740">really</span> <span m="1028920">emphasize</span>
  <span m="1029579">how</span> <span m="1030690">the</span> <span m="1030810">brain</span>
  <span m="1031079">suffers</span> <span m="1032819">under</span> <span m="1033030">Alzheimer's</span>
  <span m="1033390">disease.</span> <span m="1034890">We're</span> <span m="1034980">going</span>
  <span m="1035130">to</span> <span m="1035220">characterize</span> <span m="1035970">the</span>
  <span m="1036060">patient's</span> <span m="1037109">disease</span> <span m="1037470">status</span>
  <span m="1038640">by</span> <span m="1039119">a</span> <span m="1039240">score.</span>
  <span m="1039960">And</span> <span m="1040260">one</span> <span m="1040470">example</span>
  <span m="1040859">of</span> <span m="1040950">such a</span> <span m="1041069">score</span>
  <span m="1041880">is</span> <span m="1042060">shown</span> <span m="1042359">here.</span>
  <span m="1042730">It's</span> <span m="1042810">called</span> <span m="1043020">the</span>
  <span m="1043140">Mini</span> <span m="1043440">Mental</span> <span m="1043950">State</span>
  <span m="1044280">Examination,</span> <span m="1045300">summarized</span> <span
  m="1045810">by</span> <span m="1045960">the</span> <span m="1046109">acronym</span>
  <span m="1046569">MMSE.</span> <span m="1047940">And</span> <span m="1048030">it's</span>
  <span m="1048119">going</span> <span m="1048190">to</span> <span m="1048270">look</span>
  <span m="1048390">as</span> <span m="1048540">follows.</span></p><p><span m="1050220">For</span>
  <span m="1050430">each</span> <span m="1050640">of</span> <span m="1050730">a</span>
  <span m="1051000">number</span> <span m="1051330">of</span> <span m="1051420">different</span>
  <span m="1051750">cognitive</span> <span m="1052560">questions,</span> <span m="1055060">a</span>
  <span m="1055290">test</span> <span m="1055650">is</span> <span m="1055770">going</span>
  <span m="1055920">to</span> <span m="1055980">be</span> <span m="1056040">performed,</span>
  <span m="1057640">which--</span> <span m="1058540">for</span> <span m="1058560">example,</span>
  <span m="1059400">in</span> <span m="1059520">the</span> <span m="1059580">middle,</span>
  <span m="1059940">what</span> <span m="1060090">it</span> <span m="1060150">says
  is</span> <span m="1060360">registration.</span> <span m="1061370">The</span> <span
  m="1061500">examiner</span> <span m="1062010">might</span> <span m="1062760">name</span>
  <span m="1063060">three</span> <span m="1063330">objects</span> <span m="1063750">like</span>
  <span m="1064080">apple,</span> <span m="1064530">table,</span> <span m="1065580">penny,</span>
  <span m="1066450">and</span> <span m="1066540">then</span> <span m="1066660">ask</span>
  <span m="1066900">the</span> <span m="1066990">patient</span> <span m="1067290">to</span>
  <span m="1067380">repeat</span> <span m="1069030">those</span> <span m="1069360">three</span>
  <span m="1069570">objects.</span> <span m="1072130">All</span> <span m="1072340">of
  us</span> <span m="1072520">should</span> <span m="1072640">be</span> <span m="1072730">able</span>
  <span m="1073720">to</span> <span m="1073870">remember</span> <span m="1074770">a</span>
  <span m="1074830">sequence</span> <span m="1075250">of</span> <span m="1075370">three</span>
  <span m="1075580">things</span> <span m="1075910">so</span> <span m="1076060">that</span>
  <span m="1076180">when</span> <span m="1076330">we</span> <span m="1076480">finish</span>
  <span m="1076780">the</span> <span m="1076870">sequence,</span> <span m="1077410">you</span>
  <span m="1077530">should</span> <span m="1077680">be</span> <span m="1077740">able</span>
  <span m="1077860">to</span> <span m="1077900">remember</span> <span m="1078130">what</span>
  <span m="1078220">the</span> <span m="1078310">first</span> <span m="1078550">thing</span>
  <span m="1078670">in</span> <span m="1078730">the</span> <span m="1078820">sequence</span>
  <span m="1079180">was.</span> <span m="1080950">We</span> <span m="1081130">shouldn't</span>
  <span m="1081370">have</span> <span m="1081520">a</span> <span m="1081550">problem</span>
  <span m="1081760">with</span> <span m="1081880">that.</span> <span m="1082160">But</span>
  <span m="1082240">as</span> <span m="1082390">patients</span> <span m="1082780">get</span>
  <span m="1082930">increasingly</span> <span m="1083920">worse</span> <span m="1084210">in</span>
  <span m="1084340">their</span> <span m="1084460">Alzheimer's</span> <span m="1084850">disease,</span>
  <span m="1085120">that</span> <span m="1085330">task</span> <span m="1085720">becomes</span>
  <span m="1085990">very</span> <span m="1086170">challenging.</span></p><p><span
  m="1087350">And</span> <span m="1087450">so</span> <span m="1087550">you</span>
  <span m="1087650">might</span> <span m="1087750">give</span> <span m="1089080">1.4</span>
  <span m="1090400">correct</span> <span m="1092100">for</span> <span m="1092290">each</span>
  <span m="1092470">correct.</span> <span m="1092950">And so</span> <span m="1093070">if</span>
  <span m="1093130">the</span> <span m="1093190">patient</span> <span m="1093460">gets</span>
  <span m="1093640">all</span> <span m="1093820">three,</span> <span m="1094300">if</span>
  <span m="1094450">they</span> <span m="1094570">repeat</span> <span m="1094960">all</span>
  <span m="1095080">three</span> <span m="1095320">of</span> <span m="1095410">them,</span>
  <span m="1095650">then</span> <span m="1095770">they</span> <span m="1095860">get</span>
  <span m="1095980">three</span> <span m="1096160">points.</span> <span m="1096490">If</span>
  <span m="1096610">they</span> <span m="1096940">can't</span> <span m="1097180">remember</span>
  <span m="1097480">any</span> <span m="1097630">of</span> <span m="1097690">them,</span>
  <span m="1097920">zero</span> <span m="1098140">points.</span></p><p><span m="1101290">Then</span>
  <span m="1101500">you</span> <span m="1101590">might</span> <span m="1101770">continue.</span>
  <span m="1102460">You</span> <span m="1102520">might</span> <span m="1102910">ask</span>
  <span m="1103270">something</span> <span m="1103660">else</span> <span m="1103900">like</span>
  <span m="1104140">subtract</span> <span m="1104680">7</span> <span m="1104980">from</span>
  <span m="1105150">100,</span> <span m="1105520">then</span> <span m="1105670">repeat</span>
  <span m="1106150">some</span> <span m="1106360">results,</span> <span m="1107000">so</span>
  <span m="1107110">some</span> <span m="1107290">sort</span> <span m="1107440">of</span>
  <span m="1107500">mathematical</span> <span m="1108070">question.</span> <span m="1109060">Then</span>
  <span m="1109180">you</span> <span m="1109270">might</span> <span m="1109420">return</span>
  <span m="1109840">back</span> <span m="1110080">to</span> <span m="1110170">that</span>
  <span m="1110350">original</span> <span m="1110800">three</span> <span m="1111130">objects</span>
  <span m="1111580">you</span> <span m="1111640">asked</span> <span m="1111850">about</span>
  <span m="1112000">originally.</span> <span m="1112550">Now</span> <span m="1112660">it's</span>
  <span m="1112780">been,</span> <span m="1113530">let's</span> <span m="1113710">say,</span>
  <span m="1113830">a</span> <span m="1113890">minute</span> <span m="1114190">later.</span>
  <span m="1114490">And</span> <span m="1114580">you</span> <span m="1114670">say,</span>
  <span m="1114820">what</span> <span m="1115030">were</span> <span m="1115180">those</span>
  <span m="1115420">three</span> <span m="1115600">objects</span> <span m="1115930">I</span>
  <span m="1115990">mentioned</span> <span m="1116290">earlier?</span> <span m="1116940">And</span>
  <span m="1117120">this</span> <span m="1117250">is</span> <span m="1117310">trying</span>
  <span m="1117550">to</span> <span m="1117640">get</span> <span m="1117790">at</span>
  <span m="1117880">a</span> <span m="1117940">little</span> <span m="1118090">bit</span>
  <span m="1118360">longer-term</span> <span m="1119080">memory</span> <span m="1121130">and</span>
  <span m="1121450">so</span> <span m="1121690">on.</span></p><p><span m="1121930">And</span>
  <span m="1122260">one</span> <span m="1122500">will</span> <span m="1122620">then</span>
  <span m="1123490">add</span> <span m="1123820">up</span> <span m="1124270">the</span>
  <span m="1124690">number</span> <span m="1124960">of</span> <span m="1125020">points</span>
  <span m="1125350">associated</span> <span m="1125620">with</span> <span m="1125740">each</span>
  <span m="1125860">of</span> <span m="1125920">these</span> <span m="1126100">responses</span>
  <span m="1126730">and</span> <span m="1126820">get</span> <span m="1126940">a</span>
  <span m="1127000">total</span> <span m="1127360">score.</span> <span m="1128610">Here</span>
  <span m="1128910">it's out</span> <span m="1129010">of</span> <span m="1129070">30</span>
  <span m="1129370">points.</span> <span m="1130410">If</span> <span m="1130510">you</span>
  <span m="1130600">divide</span> <span m="1130870">by</span> <span m="1131020">3,</span>
  <span m="1131320">you</span> <span m="1131410">get</span> <span m="1131530">the</span>
  <span m="1131620">story I</span> <span m="1131950">give</span> <span m="1132130">you</span>
  <span m="1132220">here.</span></p><p><span m="1133000">So</span> <span m="1133690">these</span>
  <span m="1133990">are</span> <span m="1134350">the</span> <span m="1134500">scores</span>
  <span m="1135190">that</span> <span m="1135340">I'm</span> <span m="1135430">talking</span>
  <span m="1135700">about</span> <span m="1136660">for</span> <span m="1136960">Alzheimer's</span>
  <span m="1137470">disease.</span> <span m="1137890">They're</span> <span m="1138040">often</span>
  <span m="1138310">characterized</span> <span m="1140200">by</span> <span m="1140350">scores</span>
  <span m="1140730">to</span> <span m="1141040">questionnaires.</span> <span m="1141640">But</span>
  <span m="1141760">of</span> <span m="1141850">course,</span> <span m="1142210">if</span>
  <span m="1142360">you</span> <span m="1142510">had</span> <span m="1142660">done</span>
  <span m="1142870">something</span> <span m="1143110">like</span> <span m="1143290">brain</span>
  <span m="1143680">imaging,</span> <span m="1144640">the</span> <span m="1144970">disease</span>
  <span m="1145270">status</span> <span m="1145660">might,</span> <span m="1146470">for</span>
  <span m="1146620">example,</span> <span m="1147100">be</span> <span m="1147340">inferred</span>
  <span m="1147760">automatically</span> <span m="1148270">from</span> <span m="1148540">brain</span>
  <span m="1148780">imaging.</span> <span m="1149690">If</span> <span m="1149770">you</span>
  <span m="1149890">had</span> <span m="1150100">a</span> <span m="1150190">smartphone</span>
  <span m="1150820">device,</span> <span m="1151570">which</span> <span m="1151790">patients</span>
  <span m="1152170">are</span> <span m="1152230">carrying</span> <span m="1153160">around</span>
  <span m="1153430">with</span> <span m="1153610">them,</span> <span m="1154420">and</span>
  <span m="1154690">which</span> <span m="1154900">is</span> <span m="1155980">looking</span>
  <span m="1156370">at</span> <span m="1156490">mobile</span> <span m="1156820">activity,</span>
  <span m="1157360">you</span> <span m="1157450">might</span> <span m="1157570">be</span>
  <span m="1157630">able</span> <span m="1157750">to</span> <span m="1157870">automatically</span>
  <span m="1158410">infer</span> <span m="1158710">their</span> <span m="1158860">current</span>
  <span m="1159190">disease</span> <span m="1159460">status</span> <span m="1159880">from</span>
  <span m="1160150">that</span> <span m="1160330">smartphone.</span> <span m="1161900">You</span>
  <span m="1162000">might</span> <span m="1162010">be able to</span> <span m="1162190">infer</span>
  <span m="1162560">it</span> <span m="1162670">from</span> <span m="1163000">their</span>
  <span m="1163240">typing</span> <span m="1163660">patterns.</span> <span m="1164200">You</span>
  <span m="1164260">might</span> <span m="1164380">be able</span> <span m="1164500">to</span>
  <span m="1164710">infer</span> <span m="1164890">it</span> <span m="1165010">from</span>
  <span m="1165220">their</span> <span m="1165370">email</span> <span m="1165670">or</span>
  <span m="1165760">Facebook</span> <span m="1166150">habits.</span></p><p><span m="1166730">And</span>
  <span m="1166810">so</span> <span m="1167530">I'm</span> <span m="1167620">just</span>
  <span m="1167740">trying</span> <span m="1167890">to</span> <span m="1167950">point</span>
  <span m="1168160">out,</span> <span m="1168280">there</span> <span m="1168380">are</span>
  <span m="1168400">a</span> <span m="1168430">lot</span> <span m="1168700">of</span>
  <span m="1168760">different</span> <span m="1169000">ways</span> <span m="1169210">to</span>
  <span m="1169270">try</span> <span m="1169420">to</span> <span m="1169540">get</span>
  <span m="1169750">this</span> <span m="1169960">number</span> <span m="1170470">of</span>
  <span m="1170710">how</span> <span m="1170920">the</span> <span m="1171010">patient</span>
  <span m="1171400">might</span> <span m="1171580">be</span> <span m="1171700">doing</span>
  <span m="1172630">at</span> <span m="1172780">any</span> <span m="1172930">one</span>
  <span m="1173140">point</span> <span m="1173260">in</span> <span m="1173320">time.</span>
  <span m="1173950">Each</span> <span m="1174100">of</span> <span m="1174160">those</span>
  <span m="1174340">an</span> <span m="1174430">interesting</span> <span m="1174760">question.</span>
  <span m="1175150">For</span> <span m="1175300">now,</span> <span m="1175450">we're</span>
  <span m="1175530">just</span> <span m="1175660">going</span> <span m="1175700">to</span>
  <span m="1175760">assume</span> <span m="1176020">it's</span> <span m="1176170">known.</span>
  <span m="1177700">So</span> <span m="1178450">retrospectively,</span> <span m="1179950">you've</span>
  <span m="1180160">gathered</span> <span m="1180580">this</span> <span m="1180760">data</span>
  <span m="1181720">for</span> <span m="1181870">patients,</span> <span m="1182770">which</span>
  <span m="1182950">is</span> <span m="1183070">now</span> <span m="1183250">longitudinal</span>
  <span m="1183880">in</span> <span m="1184020">nature.</span> <span m="1184640">You</span>
  <span m="1184660">have</span> <span m="1184840">some</span> <span m="1184990">baseline</span>
  <span m="1185350">information.</span> <span m="1185950">And</span> <span m="1186070">you</span>
  <span m="1186190">know</span> <span m="1186820">how</span> <span m="1187060">the</span>
  <span m="1187120">patient</span> <span m="1187420">is</span> <span m="1187540">doing</span>
  <span m="1188250">over</span> <span m="1188500">different</span> <span m="1188800">six-month</span>
  <span m="1189250">intervals.</span> <span m="1190180">And</span> <span m="1190270">we'd</span>
  <span m="1190420">then</span> <span m="1190570">like</span> <span m="1190720">to</span>
  <span m="1190810">be</span> <span m="1190870">able</span> <span m="1190990">to</span>
  <span m="1191080">predict</span> <span m="1191500">to</span> <span m="1191620">those</span>
  <span m="1191860">things.</span></p><p><span m="1193240">Now,</span> <span m="1197400">if</span>
  <span m="1197610">this</span> <span m="1197850">were--</span> <span m="1201390">we</span>
  <span m="1201510">can</span> <span m="1201600">now</span> <span m="1201750">go</span>
  <span m="1201900">back</span> <span m="1202140">in</span> <span m="1202230">time</span>
  <span m="1202620">to</span> <span m="1202980">lecture</span> <span m="1203370">three</span>
  <span m="1204360">and</span> <span m="1204480">ask,</span> <span m="1204850">well,</span>
  <span m="1205200">how</span> <span m="1205500">could</span> <span m="1205680">we</span>
  <span m="1205800">predict</span> <span m="1206160">these</span> <span m="1206370">different</span>
  <span m="1206610">things?</span> <span m="1207023">So</span> <span m="1208110">what</span>
  <span m="1208230">are</span> <span m="1208290">some</span> <span m="1208440">approaches</span>
  <span m="1209190">that</span> <span m="1209580">you</span> <span m="1209640">might</span>
  <span m="1209790">try?</span> <span m="1217300">Why don't</span> <span m="1217460">you</span>
  <span m="1217550">talk</span> <span m="1217760">to</span> <span m="1217820">your</span>
  <span m="1217910">neighbor</span> <span m="1219440">for</span> <span m="1219560">a</span>
  <span m="1219590">second,</span> <span m="1220690">and</span> <span m="1221030">then</span>
  <span m="1221120">I'll</span> <span m="1221180">call</span> <span m="1221390">on</span>
  <span m="1221450">a</span> <span m="1221480">random</span> <span m="1221750">person.</span></p><p><span
  m="1223416">[SIDE CONVERSATION]</span></p><p>&nbsp;</p><p><span m="1226720">OK.</span>
  <span m="1227480">That's</span> <span m="1227780">enough.</span> <span m="1229100">My</span>
  <span m="1229220">question</span> <span m="1229550">was</span> <span m="1230260">sufficiently</span>
  <span m="1230890">under-defined</span> <span m="1231890">that</span> <span m="1232145">if</span>
  <span m="1232400">you</span> <span m="1232490">talk</span> <span m="1232730">longer,</span>
  <span m="1233270">who</span> <span m="1233360">knows</span> <span m="1233510">what</span>
  <span m="1233600">you'll</span> <span m="1233680">be</span> <span m="1233750">talking</span>
  <span m="1233960">about.</span> <span m="1237410">Over</span> <span m="1237800">here,</span>
  <span m="1239690">the</span> <span m="1239810">two</span> <span m="1240050">of</span>
  <span m="1240110">you--</span> <span m="1240520">the</span> <span m="1240620">person</span>
  <span m="1240840">with</span> <span m="1240930">the</span> <span m="1240980">computer.</span>
  <span m="1241280">Yeah.</span> <span m="1242360">How</span> <span m="1242480">would</span>
  <span m="1242570">you</span> <span m="1242630">tackle</span> <span m="1242870">this</span>
  <span m="1242990">problem?</span></p><p><span m="1245204">AUDIENCE:</span> <span
  m="1245439">Me?</span> <span m="1245675">OK.</span></p><p><span m="1247559">DAVID
  SONTAG:</span> <span m="1247676">No,</span> <span m="1247793">no,</span> <span m="1247910">no.</span>
  <span m="1248030">Over</span> <span m="1248180">here,</span> <span m="1248370">yeah.</span>
  <span m="1248490">Yeah, you.</span></p><p><span m="1252530">AUDIENCE:</span> <span
  m="1252680">I</span> <span m="1252830">would</span> <span m="1253000">just</span>
  <span m="1253280">take,</span> <span m="1254199">I</span> <span m="1254688">guess,</span>
  <span m="1255177">previous</span> <span m="1255666">data,</span> <span m="1257133">and
  then--</span> <span m="1260556">yeah, I guess,</span> <span m="1261045">any</span>
  <span m="1261534">previous</span> <span m="1262023">data with</span> <span m="1263001">records</span>
  <span m="1263490">of</span> <span m="1265935">disease</span> <span m="1266424">progression</span>
  <span m="1266913">over</span> <span m="1267891">that time</span> <span m="1268380">span,</span>
  <span m="1268869">and then</span> <span m="1270336">treated</span> <span m="1270825">[INAUDIBLE].</span></p><p><span
  m="1272320">DAVID SONTAG:</span> <span m="1272425">But</span> <span m="1272840">just</span>
  <span m="1273050">to</span> <span m="1273140">understand,</span> <span m="1273590">would</span>
  <span m="1273770">you</span> <span m="1274220">learn</span> <span m="1274880">five</span>
  <span m="1275270">different</span> <span m="1275750">models?</span> <span m="1277800">So</span>
  <span m="1278070">our</span> <span m="1278360">goal</span> <span m="1278660">is</span>
  <span m="1278750">to</span> <span m="1278870">get</span> <span m="1279110">these--</span>
  <span m="1279850">here</span> <span m="1280220">I'm</span> <span m="1280310">showing</span>
  <span m="1280490">you</span> <span m="1280580">three,</span> <span m="1280850">but</span>
  <span m="1280940">it</span> <span m="1281000">might</span> <span m="1281090">be</span>
  <span m="1281180">five</span> <span m="1281660">different</span> <span m="1282020">numbers</span>
  <span m="1282390">at</span> <span m="1282430">different</span> <span m="1282680">time</span>
  <span m="1282890">points.</span> <span m="1283820">Would</span> <span m="1284010">you</span>
  <span m="1284120">learn</span> <span m="1284450">one</span> <span m="1284690">model</span>
  <span m="1284960">to</span> <span m="1285080">predict</span> <span m="1285470">what</span>
  <span m="1285650">it</span> <span m="1285710">would</span> <span m="1285800">be</span>
  <span m="1285890">at</span> <span m="1285950">six</span> <span m="1286190">months,</span>
  <span m="1286430">another to</span> <span m="1286700">predict</span> <span m="1287000">what</span>
  <span m="1287120">would</span> <span m="1287210">be</span> <span m="1287300">a</span>
  <span m="1287380">12</span> <span m="1287630">months?</span> <span m="1289550">Would</span>
  <span m="1289700">you</span> <span m="1289760">learn</span> <span m="1289910">a</span>
  <span m="1289970">single</span> <span m="1290240">model?</span></p><p><span m="1294830">Other</span>
  <span m="1295010">ideas?</span> <span m="1296640">Somewhere</span> <span m="1297200">over
  in</span> <span m="1297440">this</span> <span m="1297560">part</span> <span m="1297710">of</span>
  <span m="1297770">the</span> <span m="1297830">room.</span> <span m="1299620">Yeah.</span>
  <span m="1299730">You.</span></p><p><span m="1301970">AUDIENCE:</span> <span m="1302194">[INAUDIBLE]</span></p><p><span
  m="1303770">DAVID SONTAG:</span> <span m="1303840">Yeah.</span> <span m="1304350">Sure.</span></p><p><span
  m="1307560">AUDIENCE:</span> <span m="1307807">[INAUDIBLE]</span></p><p>&nbsp;</p><p><span
  m="1318960">DAVID SONTAG:</span> <span m="1319107">So</span> <span m="1319550">use</span>
  <span m="1319790">a</span> <span m="1319910">multi-task</span> <span m="1320550">learning</span>
  <span m="1320820">approach,</span> <span m="1321840">where you</span> <span m="1321960">try</span>
  <span m="1322120">to</span> <span m="1322200">learn</span> <span m="1322380">all</span>
  <span m="1322560">five</span> <span m="1322770">at</span> <span m="1322830">that</span>
  <span m="1322940">time</span> <span m="1323490">and</span> <span m="1323670">use
  what?</span> <span m="1323940">What</span> <span m="1324250">was the</span> <span
  m="1324420">other</span> <span m="1324600">thing?</span></p><p><span m="1325780">AUDIENCE:</span>
  <span m="1325941">So</span> <span m="1326102">you</span> <span m="1326265">can</span>
  <span m="1326750">learn</span> <span m="1327235">to</span> <span m="1328205">use
  these</span> <span m="1328690">datas</span> <span m="1329175">in</span> <span m="1329660">six</span>
  <span m="1330145">months</span> <span m="1330630">and also</span> <span m="1331115">use</span>
  <span m="1331600">that</span> <span m="1332570">as</span> <span m="1333540">your</span>
  <span m="1334995">baseline</span> <span m="1335965">[INAUDIBLE].</span></p><p><span
  m="1337420">DAVID SONTAG:</span> <span m="1337675">Oh,</span> <span m="1337930">that's</span>
  <span m="1338140">a</span> <span m="1338200">really</span> <span m="1338380">interesting</span>
  <span m="1338710">idea.</span> <span m="1339160">OK.</span> <span m="1341330">So</span>
  <span m="1341500">the</span> <span m="1341590">suggestion</span> <span m="1342130">was--</span>
  <span m="1343420">so</span> <span m="1343780">there</span> <span m="1343900">are</span>
  <span m="1343930">two</span> <span m="1344110">different</span> <span m="1344350">suggestions,</span>
  <span m="1344790">actually.</span> <span m="1346180">The</span> <span m="1346300">first</span>
  <span m="1346540">suggestion</span> <span m="1346990">was</span> <span m="1348640">do</span>
  <span m="1348940">a</span> <span m="1349000">multi-task</span> <span m="1349630">learning</span>
  <span m="1349930">approach,</span> <span m="1350320">where</span> <span m="1350470">you</span>
  <span m="1350530">attempt</span> <span m="1350740">to</span> <span m="1350800">learn--</span>
  <span m="1351160">instead</span> <span m="1351400">of</span> <span m="1351460">five</span>
  <span m="1351850">different</span> <span m="1352210">and</span> <span m="1352300">sort
  of</span> <span m="1352450">independent</span> <span m="1352900">models,</span>
  <span m="1354550">try</span> <span m="1354760">to</span> <span m="1354850">learn</span>
  <span m="1355120">them</span> <span m="1355270">jointly</span> <span m="1355600">together.</span>
  <span m="1356170">And</span> <span m="1356635">in</span> <span m="1357100">a</span>
  <span m="1357160">second,</span> <span m="1357490">we'll</span> <span m="1357610">talk</span>
  <span m="1357850">about</span> <span m="1358570">why</span> <span m="1358920">it</span>
  <span m="1359010">might</span> <span m="1359170">make</span> <span m="1359290">sense</span>
  <span m="1359470">to</span> <span m="1359560">do</span> <span m="1359650">that.</span></p><p><span
  m="1360250">The</span> <span m="1360340">different</span> <span m="1360850">thought</span>
  <span m="1361180">was,</span> <span m="1362170">well,</span> <span m="1362830">is</span>
  <span m="1362920">this</span> <span m="1363070">really</span> <span m="1363280">the</span>
  <span m="1363370">question</span> <span m="1363640">you</span> <span m="1363730">want</span>
  <span m="1363850">to</span> <span m="1363940">solve?</span> <span m="1365050">For</span>
  <span m="1365170">example,</span> <span m="1369250">you</span> <span m="1369400">might</span>
  <span m="1369670">imagine</span> <span m="1371110">settings</span> <span m="1371680">where</span>
  <span m="1372850">you</span> <span m="1373090">have</span> <span m="1374100">the</span>
  <span m="1374170">patient</span> <span m="1374530">not</span> <span m="1374800">at</span>
  <span m="1374920">time</span> <span m="1375170">zero</span> <span m="1375520">but</span>
  <span m="1375670">actually</span> <span m="1376000">at</span> <span m="1376150">six</span>
  <span m="1376450">months.</span> <span m="1377140">And</span> <span m="1377230">you</span>
  <span m="1377320">might</span> <span m="1377500">want</span> <span m="1377680">to</span>
  <span m="1377740">know</span> <span m="1377980">what's</span> <span m="1378160">going</span>
  <span m="1378280">to</span> <span m="1378340">happen</span> <span m="1378550">to</span>
  <span m="1378640">them</span> <span m="1378760">in</span> <span m="1378820">the</span>
  <span m="1378910">future.</span> <span m="1379430">And</span> <span m="1379530">so</span>
  <span m="1379540">you</span> <span m="1379600">shouldn't</span> <span m="1379840">just</span>
  <span m="1380140">use</span> <span m="1380290">the</span> <span m="1380380">baseline</span>
  <span m="1380710">information.</span> <span m="1381070">You</span> <span m="1381140">should</span>
  <span m="1381280">recondition</span> <span m="1381700">on</span> <span m="1381790">the</span>
  <span m="1381850">data</span> <span m="1382090">you</span> <span m="1382150">have</span>
  <span m="1382330">available</span> <span m="1382670">for</span> <span m="1382780">time.</span></p><p><span
  m="1384250">And</span> <span m="1384340">a</span> <span m="1384400">different</span>
  <span m="1384700">way</span> <span m="1384880">of</span> <span m="1384970">thinking</span>
  <span m="1385270">through</span> <span m="1385420">that</span> <span m="1385720">is</span>
  <span m="1385870">you</span> <span m="1385960">could</span> <span m="1386050">imagine</span>
  <span m="1386350">learning</span> <span m="1386590">a</span> <span m="1386620">Markov</span>
  <span m="1387040">model,</span> <span m="1387900">where</span> <span m="1388030">you</span>
  <span m="1388120">learn</span> <span m="1388330">something</span> <span m="1388660">about</span>
  <span m="1390160">the</span> <span m="1390490">joint</span> <span m="1391030">distribution</span>
  <span m="1391990">of</span> <span m="1392230">the</span> <span m="1392350">disease</span>
  <span m="1392650">stage</span> <span m="1393430">over</span> <span m="1393700">time.</span>
  <span m="1394690">And</span> <span m="1394780">then</span> <span m="1394900">you</span>
  <span m="1394990">could,</span> <span m="1395110">for</span> <span m="1395230">example,</span>
  <span m="1395840">even</span> <span m="1396010">if</span> <span m="1396160">you</span>
  <span m="1396250">only</span> <span m="1396430">had</span> <span m="1396550">baseline</span>
  <span m="1396970">information</span> <span m="1397360">available,</span> <span m="1397690">you</span>
  <span m="1397810">could</span> <span m="1397930">attempt</span> <span m="1398290">to</span>
  <span m="1398920">marginalize</span> <span m="1399760">over</span> <span m="1399980">the</span>
  <span m="1400060">intermediate</span> <span m="1400570">values</span> <span m="1400930">that</span>
  <span m="1401050">are</span> <span m="1401110">unobserved</span> <span m="1401740">to</span>
  <span m="1401890">infer</span> <span m="1402190">what</span> <span m="1402400">the</span>
  <span m="1402670">later</span> <span m="1402940">values</span> <span m="1403240">might</span>
  <span m="1403450">be.</span> <span m="1406300">Now,</span> <span m="1406720">that</span>
  <span m="1406930">Markov</span> <span m="1407320">model</span> <span m="1407560">approach,</span>
  <span m="1407950">although</span> <span m="1408190">we</span> <span m="1408310">will</span>
  <span m="1408460">talk</span> <span m="1408700">about</span> <span m="1408910">it</span>
  <span m="1408970">extensively</span> <span m="1410210">in</span> <span m="1410350">the</span>
  <span m="1410440">next</span> <span m="1410860">week</span> <span m="1411130">or</span>
  <span m="1411190">so,</span> <span m="1412480">it's</span> <span m="1412630">actually</span>
  <span m="1412870">not</span> <span m="1413110">a</span> <span m="1413170">very</span>
  <span m="1413410">good</span> <span m="1413530">approach</span> <span m="1413800">for</span>
  <span m="1413890">this</span> <span m="1414040">problem.</span> <span m="1415210">And</span>
  <span m="1415300">the</span> <span m="1415390">reason</span> <span m="1415690">why</span>
  <span m="1415930">is</span> <span m="1416050">because</span> <span m="1417130">it</span>
  <span m="1417250">increases</span> <span m="1418300">the</span> <span m="1418420">complexity.</span></p><p><span
  m="1419290">So</span> <span m="1419680">when</span> <span m="1419920">you</span>
  <span m="1420610">are</span> <span m="1420790">learn--</span> <span m="1421180">in
  essence</span> <span m="1422230">if</span> <span m="1422350">you</span> <span m="1422440">wanted</span>
  <span m="1422650">to</span> <span m="1422770">predict</span> <span m="1423100">what's</span>
  <span m="1423280">going on</span> <span m="1423530">at</span> <span m="1423640">18</span>
  <span m="1424000">months,</span> <span m="1424950">and</span> <span m="1425020">if,</span>
  <span m="1425260">as</span> <span m="1425410">an</span> <span m="1425530">intermediate</span>
  <span m="1426040">step</span> <span m="1426310">to</span> <span m="1426400">predict</span>
  <span m="1426760">what</span> <span m="1426880">goes</span> <span m="1427060">on
  at</span> <span m="1427180">18</span> <span m="1427480">months,</span> <span m="1427750">you</span>
  <span m="1427840">have</span> <span m="1427960">to</span> <span m="1428050">predict</span>
  <span m="1428500">what's</span> <span m="1428680">going</span> <span m="1428800">to</span>
  <span m="1428890">go</span> <span m="1429010">on</span> <span m="1429160">at</span>
  <span m="1429340">12</span> <span m="1429550">months,</span> <span m="1430000">and</span>
  <span m="1430120">then</span> <span m="1430240">the</span> <span m="1430300">likelihood</span>
  <span m="1430720">of</span> <span m="1430810">transitioning</span> <span m="1432040">from</span>
  <span m="1432250">12</span> <span m="1432520">months</span> <span m="1432710">to</span>
  <span m="1432770">18</span> <span m="1433030">months,</span> <span m="1434040">then</span>
  <span m="1434590">you</span> <span m="1434680">might</span> <span m="1434830">incur</span>
  <span m="1435250">error</span> <span m="1435700">in</span> <span m="1435790">trying</span>
  <span m="1436030">to</span> <span m="1436090">predict</span> <span m="1436750">what's</span>
  <span m="1436960">going</span> <span m="1437110">on</span> <span m="1437200">at</span>
  <span m="1437260">12</span> <span m="1437530">months.</span> <span m="1438480">And</span>
  <span m="1438580">that</span> <span m="1438730">error is</span> <span m="1439150">then</span>
  <span m="1439270">going</span> <span m="1439390">to</span> <span m="1439690">propagate</span>
  <span m="1440200">as</span> <span m="1440320">you</span> <span m="1440410">attempt</span>
  <span m="1440680">to</span> <span m="1441610">think</span> <span m="1441880">about</span>
  <span m="1442030">the</span> <span m="1442120">transition</span> <span m="1442630">from</span>
  <span m="1442810">12</span> <span m="1443020">months</span> <span m="1443290">to</span>
  <span m="1443410">18</span> <span m="1443680">months.</span> <span m="1444430">And</span>
  <span m="1444650">that</span> <span m="1444730">propagation</span> <span m="1445360">of</span>
  <span m="1445450">error,</span> <span m="1445780">particularly</span> <span m="1446290">when</span>
  <span m="1446440">you</span> <span m="1446500">don't</span> <span m="1446650">have</span>
  <span m="1446860">much</span> <span m="1447100">data,</span> <span m="1447430">is</span>
  <span m="1447550">going</span> <span m="1447760">to</span> <span m="1447850">really</span>
  <span m="1448270">hurt</span> <span m="1448510">the</span> <span m="1448730">[INAUDIBLE]</span>
  <span m="1448940">of your</span> <span m="1449170">machine</span> <span m="1449440">learning</span>
  <span m="1449680">algorithm.</span></p><p><span m="1451430">So</span> <span m="1451510">the</span>
  <span m="1451600">method</span> <span m="1451900">I'll</span> <span m="1451990">be</span>
  <span m="1452080">talking</span> <span m="1452380">about</span> <span m="1452530">today</span>
  <span m="1452830">is,</span> <span m="1452950">in</span> <span m="1453010">fact,</span>
  <span m="1453280">going to</span> <span m="1453380">be</span> <span m="1453880">what</span>
  <span m="1454240">I</span> <span m="1454350">view</span> <span m="1454500">as</span>
  <span m="1454540">the</span> <span m="1454630">simplest</span> <span m="1455140">possible</span>
  <span m="1455560">approach</span> <span m="1455950">to</span> <span m="1456070">this</span>
  <span m="1456220">problem.</span> <span m="1457270">And</span> <span m="1457390">it's</span>
  <span m="1457480">going</span> <span m="1457600">to</span> <span m="1457660">be</span>
  <span m="1457750">direct</span> <span m="1458140">prediction</span> <span m="1458530">approach.</span>
  <span m="1458960">So</span> <span m="1459060">we're</span> <span m="1459280">directly</span>
  <span m="1459850">going</span> <span m="1460120">to</span> <span m="1460360">predict</span>
  <span m="1461500">each</span> <span m="1461740">of</span> <span m="1461800">the</span>
  <span m="1461890">different</span> <span m="1462190">time</span> <span m="1462460">points</span>
  <span m="1462820">independently.</span> <span m="1464470">But</span> <span m="1464740">we</span>
  <span m="1464890">will</span> <span m="1465100">tie</span> <span m="1465400">together</span>
  <span m="1465730">the</span> <span m="1465820">parameters</span> <span m="1466360">of</span>
  <span m="1466420">the</span> <span m="1466480">model,</span> <span m="1466750">as</span>
  <span m="1466870">was</span> <span m="1466930">suggested,</span> <span m="1467500">using</span>
  <span m="1467770">a</span> <span m="1467810">multi-task</span> <span m="1468430">learning</span>
  <span m="1468700">approach.</span></p><p><span m="1471480">And</span> <span m="1471580">the</span>
  <span m="1471640">reason</span> <span m="1471940">why</span> <span m="1472060">we're</span>
  <span m="1472180">going</span> <span m="1472330">to</span> <span m="1472450">want</span>
  <span m="1472630">to</span> <span m="1472750">use</span> <span m="1472890">a</span>
  <span m="1472960">multi-task</span> <span m="1473470">learning</span> <span m="1473680">approach</span>
  <span m="1473990">is</span> <span m="1474040">because</span> <span m="1474340">of</span>
  <span m="1474430">data</span> <span m="1474670">sparsity.</span> <span m="1476980">So</span>
  <span m="1477490">imagine</span> <span m="1477910">the</span> <span m="1478000">following</span>
  <span m="1478330">situation.</span> <span m="1480470">Imagine</span> <span m="1482305">that</span>
  <span m="1482740">we</span> <span m="1482920">had</span> <span m="1483190">just</span>
  <span m="1483400">binary</span> <span m="1483850">indicators</span> <span m="1484390">here.</span>
  <span m="1484720">So</span> <span m="1487090">let's</span> <span m="1487240">say</span>
  <span m="1487750">patient</span> <span m="1490330">is</span> <span m="1490480">OK,</span>
  <span m="1491110">or</span> <span m="1491230">they're</span> <span m="1491380">not</span>
  <span m="1491610">OK.</span> <span m="1492730">So</span> <span m="1492850">the</span>
  <span m="1492910">data</span> <span m="1493120">might</span> <span m="1493240">look</span>
  <span m="1493390">like</span> <span m="1493570">this--</span> <span m="1494290">0,</span>
  <span m="1495130">0,</span> <span m="1495820">1.</span></p><p><span m="1498130">Then</span>
  <span m="1498280">the</span> <span m="1498370">data</span> <span m="1498580">set</span>
  <span m="1498860">you</span> <span m="1498960">might</span> <span m="1498970">have</span>
  <span m="1499840">might</span> <span m="1500080">look</span> <span m="1500230">a</span>
  <span m="1500290">little</span> <span m="1500440">bit</span> <span m="1500530">like</span>
  <span m="1500680">this.</span> <span m="1501050">So</span> <span m="1501280">now</span>
  <span m="1501400">I'm</span> <span m="1501460">going</span> <span m="1501580">to</span>
  <span m="1502030">show</span> <span m="1502270">you</span> <span m="1502420">the</span>
  <span m="1502570">data.</span> <span m="1503500">And</span> <span m="1507580">one</span>
  <span m="1507790">row is</span> <span m="1508060">one</span> <span m="1508210">patient.</span>
  <span m="1509140">Different</span> <span m="1509560">columns</span> <span m="1509950">are</span>
  <span m="1510010">different</span> <span m="1510250">time</span> <span m="1510460">points.</span>
  <span m="1511850">So</span> <span m="1511930">the</span> <span m="1512020">first</span>
  <span m="1512230">patient,</span> <span m="1512620">as</span> <span m="1512740">I</span>
  <span m="1512830">showed</span> <span m="1513040">you</span> <span m="1513100">before,</span>
  <span m="1513470">is</span> <span m="1513520">0,</span> <span m="1513800">0,</span>
  <span m="1514030">1.</span> <span m="1514480">Second</span> <span m="1514810">patient</span>
  <span m="1515140">might</span> <span m="1515380">be</span> <span m="1521970">0,</span>
  <span m="1524980">0,</span> <span m="1525700">1,</span> <span m="1526090">0.</span>
  <span m="1526870">Third</span> <span m="1527110">patient</span> <span m="1527470">might</span>
  <span m="1527680">be</span> <span m="1528640">1,</span> <span m="1533140">1, 1,</span>
  <span m="1533640">1.</span> <span m="1534795">Next</span> <span m="1535180">patient</span>
  <span m="1535450">might</span> <span m="1535630">be</span> <span m="1536200">0,</span>
  <span m="1536920">1,</span> <span m="1537365">1,</span> <span m="1537810">1.</span></p><p><span
  m="1538990">So</span> <span m="1539200">if</span> <span m="1539290">you</span> <span
  m="1539350">look</span> <span m="1539500">at</span> <span m="1539590">the</span>
  <span m="1539650">first</span> <span m="1540100">time</span> <span m="1540370">point</span>
  <span m="1540700">here,</span> <span m="1541390">you'll</span> <span m="1541570">notice</span>
  <span m="1541990">that</span> <span m="1542710">you</span> <span m="1542830">have</span>
  <span m="1543000">a</span> <span m="1543040">really</span> <span m="1543310">imbalanced</span>
  <span m="1543760">data</span> <span m="1544000">set.</span> <span m="1544300">There's</span>
  <span m="1544480">only</span> <span m="1544690">a</span> <span m="1544750">single</span>
  <span m="1545260">1</span> <span m="1545680">in</span> <span m="1545800">that</span>
  <span m="1545950">first</span> <span m="1546220">time</span> <span m="1546430">point.</span>
  <span m="1548260">If</span> <span m="1548350">you</span> <span m="1548410">look</span>
  <span m="1548500">at</span> <span m="1548580">the</span> <span m="1548950">second</span>
  <span m="1549190">time</span> <span m="1549400">point,</span> <span m="1549610">there</span>
  <span m="1549730">are</span> <span m="1549790">two.</span> <span m="1550530">It's</span>
  <span m="1550880">more</span> <span m="1550970">of</span> <span m="1551010">a</span>
  <span m="1551140">balanced</span> <span m="1551390">data</span> <span m="1551560">set.</span>
  <span m="1551860">And then</span> <span m="1552000">in</span> <span m="1552250">the</span>
  <span m="1552310">third</span> <span m="1552490">time</span> <span m="1552700">point,</span>
  <span m="1552940">again,</span> <span m="1553180">you're</span> <span m="1553300">sort</span>
  <span m="1553450">of</span> <span m="1553510">back</span> <span m="1553780">into</span>
  <span m="1553960">that</span> <span m="1554080">imbalanced</span> <span m="1554470">setting.</span>
  <span m="1556300">What</span> <span m="1556450">that</span> <span m="1556600">means</span>
  <span m="1557140">is</span> <span m="1557350">that</span> <span m="1557530">if</span>
  <span m="1557650">you</span> <span m="1557740">were</span> <span m="1557800">to</span>
  <span m="1557890">try</span> <span m="1558100">to</span> <span m="1558220">learn</span>
  <span m="1558550">from</span> <span m="1558760">just</span> <span m="1558970">one</span>
  <span m="1559120">of</span> <span m="1559180">these</span> <span m="1559360">time</span>
  <span m="1559540">points</span> <span m="1559870">by</span> <span m="1560050">itself,</span>
  <span m="1562480">particularly</span> <span m="1562930">in the</span> <span m="1562990">setting</span>
  <span m="1563230">where</span> <span m="1563320">you</span> <span m="1563410">don't</span>
  <span m="1563590">have</span> <span m="1563740">that</span> <span m="1563920">many</span>
  <span m="1564130">data</span> <span m="1564340">points</span> <span m="1564640">alone,</span>
  <span m="1565150">that</span> <span m="1565780">data</span> <span m="1566110">sparsity</span>
  <span m="1566680">and</span> <span m="1566770">in</span> <span m="1566890">outcome</span>
  <span m="1567250">label</span> <span m="1567670">is</span> <span m="1567820">going</span>
  <span m="1568000">to</span> <span m="1568090">really</span> <span m="1568600">hurt</span>
  <span m="1568840">you.</span> <span m="1569270">It's</span> <span m="1569290">going</span>
  <span m="1569470">to be</span> <span m="1569690">very</span> <span m="1570100">hard</span>
  <span m="1570370">to</span> <span m="1570490">learn</span> <span m="1570730">any</span>
  <span m="1570940">interesting</span> <span m="1571330">signal</span> <span m="1571660">just</span>
  <span m="1571810">from</span> <span m="1571930">that</span> <span m="1572080">time</span>
  <span m="1572290">point</span> <span m="1572500">alone.</span></p><p><span m="1575180">The</span>
  <span m="1575280">second</span> <span m="1575440">problem</span> <span m="1575740">is</span>
  <span m="1575860">that</span> <span m="1575980">the</span> <span m="1576200">label</span>
  <span m="1576430">is</span> <span m="1576520">also</span> <span m="1576700">very</span>
  <span m="1576910">noisy.</span> <span m="1577490">So</span> <span m="1577510">not</span>
  <span m="1577720">only</span> <span m="1577960">might</span> <span m="1578200">you</span>
  <span m="1578290">have</span> <span m="1578560">lots</span> <span m="1578800">of</span>
  <span m="1578890">imbalance,</span> <span m="1579550">but</span> <span m="1579820">there</span>
  <span m="1580150">might</span> <span m="1580390">be</span> <span m="1580990">noise</span>
  <span m="1581440">in</span> <span m="1581540">the</span> <span m="1581590">actual</span>
  <span m="1581890">characterizations.</span> <span m="1582580">Like</span> <span
  m="1582760">for</span> <span m="1583120">this</span> <span m="1583300">patient,</span>
  <span m="1586900">maybe</span> <span m="1587140">with</span> <span m="1587230">some</span>
  <span m="1587410">probability,</span> <span m="1587920">you</span> <span m="1588040">would</span>
  <span m="1588220">calculate</span> <span m="1588700">1, 1, 1,</span> <span m="1589100">1.</span>
  <span m="1589500">With some</span> <span m="1589900">other</span> <span m="1590050">probability,</span>
  <span m="1590380">you</span> <span m="1590680">would</span> <span m="1590920">observe</span>
  <span m="1591270">0,</span> <span m="1591550">1, 1,</span> <span m="1591880">1.</span></p><p><span
  m="1592480">And it</span> <span m="1592600">might</span> <span m="1592780">correspond</span>
  <span m="1593470">to</span> <span m="1593890">some</span> <span m="1594190">threshold</span>
  <span m="1594880">in</span> <span m="1595000">that</span> <span m="1595120">score</span>
  <span m="1595420">I</span> <span m="1595510">showed</span> <span m="1595690">you</span>
  <span m="1595780">earlier.</span> <span m="1596530">And</span> <span m="1596650">just</span>
  <span m="1596830">by</span> <span m="1596980">chance,</span> <span m="1597370">a</span>
  <span m="1597430">patient,</span> <span m="1598360">on</span> <span m="1598510">some</span>
  <span m="1598720">day,</span> <span m="1599110">passes</span> <span m="1599530">the</span>
  <span m="1599620">threshold.</span> <span m="1600130">On</span> <span m="1600250">the</span>
  <span m="1600340">next</span> <span m="1600550">day,</span> <span m="1600640">they</span>
  <span m="1600760">might</span> <span m="1600910">not</span> <span m="1601120">pass</span>
  <span m="1601360">that</span> <span m="1601510">threshold.</span> <span m="1603020">So</span>
  <span m="1603040">there</span> <span m="1603160">might</span> <span m="1603280">be</span>
  <span m="1603370">a</span> <span m="1603400">lot</span> <span m="1603580">of</span>
  <span m="1603670">noise</span> <span m="1604090">in</span> <span m="1604180">the</span>
  <span m="1604270">particular</span> <span m="1605050">labels</span> <span m="1605560">at</span>
  <span m="1605650">any</span> <span m="1605830">one</span> <span m="1606010">time</span>
  <span m="1606310">point.</span> <span m="1608050">And</span> <span m="1608320">you</span>
  <span m="1608410">wouldn't</span> <span m="1608680">want</span> <span m="1609280">that</span>
  <span m="1609460">noise</span> <span m="1609760">to</span> <span m="1609850">really</span>
  <span m="1610060">dramatically</span> <span m="1610510">affect</span> <span m="1610840">your</span>
  <span m="1610930">learning</span> <span m="1611260">algorithm</span> <span m="1611800">based</span>
  <span m="1612310">on</span> <span m="1612490">some,</span> <span m="1612780">let's</span>
  <span m="1612920">say,</span> <span m="1613060">prior</span> <span m="1613450">belief</span>
  <span m="1613810">that</span> <span m="1613930">we</span> <span m="1614050">might</span>
  <span m="1614200">have</span> <span m="1614500">that</span> <span m="1614650">there</span>
  <span m="1614770">might</span> <span m="1614920">be</span> <span m="1615040">some</span>
  <span m="1615180">amount</span> <span m="1615310">of</span> <span m="1615370">smoothness</span>
  <span m="1616060">in</span> <span m="1616180">this</span> <span m="1616300">process</span>
  <span m="1616690">across</span> <span m="1617020">time.</span></p><p><span m="1619725">And</span>
  <span m="1620220">the</span> <span m="1620280">final</span> <span m="1620640">problem</span>
  <span m="1621120">is</span> <span m="1621270">that</span> <span m="1621360">there</span>
  <span m="1621480">might</span> <span m="1621630">be</span> <span m="1621720">censoring.</span>
  <span m="1623770">So</span> <span m="1624110">the</span> <span m="1624180">actual</span>
  <span m="1624540">data</span> <span m="1624780">might</span> <span m="1624960">look</span>
  <span m="1625140">like</span> <span m="1625350">this.</span> <span m="1630820">For</span>
  <span m="1631480">much</span> <span m="1631660">later</span> <span m="1631930">time</span>
  <span m="1632180">points,</span> <span m="1632440">we</span> <span m="1632530">might</span>
  <span m="1632710">have</span> <span m="1632830">many</span> <span m="1633040">fewer</span>
  <span m="1633340">observations.</span> <span m="1634550">And</span> <span m="1634570">so</span>
  <span m="1634930">if</span> <span m="1635050">you</span> <span m="1635140">were</span>
  <span m="1635230">to</span> <span m="1635380">just</span> <span m="1635920">use</span>
  <span m="1636880">those</span> <span m="1637120">later</span> <span m="1637390">time</span>
  <span m="1637690">points</span> <span m="1637930">to</span> <span m="1638020">learn</span>
  <span m="1638200">your</span> <span m="1638290">predictive</span> <span m="1638680">model,</span>
  <span m="1639010">you</span> <span m="1639100">just</span> <span m="1639250">might</span>
  <span m="1639400">not</span> <span m="1639550">have</span> <span m="1639700">enough</span>
  <span m="1639940">data.</span> <span m="1641300">So</span> <span m="1641400">those</span>
  <span m="1641500">are</span> <span m="1641590">all</span> <span m="1641770">different</span>
  <span m="1642070">challenges</span> <span m="1642430">that</span> <span m="1642520">we're</span>
  <span m="1642610">going</span> <span m="1642790">to</span> <span m="1642850">attempt</span>
  <span m="1643090">to</span> <span m="1643150">solve</span> <span m="1643540">using</span>
  <span m="1643990">a</span> <span m="1644620">multi-task</span> <span m="1645250">learning</span>
  <span m="1645490">approach.</span></p><p><span m="1646390">Now,</span> <span m="1646570">to</span>
  <span m="1646630">put</span> <span m="1646750">some</span> <span m="1646840">numbers</span>
  <span m="1647200">to</span> <span m="1647290">these</span> <span m="1647480">things,</span>
  <span m="1648710">we</span> <span m="1648730">have</span> <span m="1648940">these</span>
  <span m="1649630">four</span> <span m="1649810">different</span> <span m="1650200">time</span>
  <span m="1650470">points.</span> <span m="1651070">We're</span> <span m="1651190">going</span>
  <span m="1651290">to</span> <span m="1651400">have</span> <span m="1651730">648</span>
  <span m="1652660">patients</span> <span m="1653290">at</span> <span m="1653530">the</span>
  <span m="1653620">six-month</span> <span m="1654100">time</span> <span m="1654340">interval.</span>
  <span m="1655350">And</span> <span m="1655630">at</span> <span m="1655900">the</span>
  <span m="1656560">four-year</span> <span m="1656980">time</span> <span m="1657160">interval,</span>
  <span m="1657430">there will</span> <span m="1657550">only</span> <span m="1657770">be</span>
  <span m="1657880">87</span> <span m="1658330">patients</span> <span m="1658750">due</span>
  <span m="1658930">to</span> <span m="1659020">patients</span> <span m="1659830">dropping</span>
  <span m="1660220">out</span> <span m="1660790">of</span> <span m="1661150">the</span>
  <span m="1661270">study.</span></p><p><span m="1665600">So</span> <span m="1665860">the</span>
  <span m="1665980">key</span> <span m="1666130">idea</span> <span m="1666460">here</span>
  <span m="1666670">will</span> <span m="1666790">be,</span> <span m="1666940">rather</span>
  <span m="1667150">than</span> <span m="1667270">learning</span> <span m="1668290">these</span>
  <span m="1669760">five</span> <span m="1670210">independent</span> <span m="1670780">models,</span>
  <span m="1671110">we're</span> <span m="1671200">going</span> <span m="1671290">to</span>
  <span m="1671380">try</span> <span m="1671530">to</span> <span m="1671740">jointly</span>
  <span m="1672310">learn</span> <span m="1672610">the</span> <span m="1672700">parameters</span>
  <span m="1673150">corresponding</span> <span m="1673540">to</span> <span m="1673600">those</span>
  <span m="1673750">models.</span> <span m="1675430">And</span> <span m="1675820">the</span>
  <span m="1676000">intuitions</span> <span m="1676480">that</span> <span m="1676570">we're</span>
  <span m="1676660">going</span> <span m="1676810">to</span> <span m="1676900">try</span>
  <span m="1677080">to</span> <span m="1677170">incorporate</span> <span m="1677650">in</span>
  <span m="1677770">doing</span> <span m="1678040">so</span> <span m="1678820">are</span>
  <span m="1678970">that</span> <span m="1679120">there</span> <span m="1679240">might</span>
  <span m="1679420">be</span> <span m="1679540">some</span> <span m="1679840">features</span>
  <span m="1680530">that</span> <span m="1680830">are</span> <span m="1681100">useful</span>
  <span m="1681700">across</span> <span m="1682120">these</span> <span m="1682330">five</span>
  <span m="1682570">different</span> <span m="1682870">prediction</span> <span m="1683230">tasks.</span>
  <span m="1684190">And</span> <span m="1684490">so</span> <span m="1684640">I'm</span>
  <span m="1684760">using</span> <span m="1685090">the</span> <span m="1685180">example</span>
  <span m="1685570">of</span> <span m="1685630">biomarkers</span> <span m="1686320">here</span>
  <span m="1686530">as</span> <span m="1686650">a</span> <span m="1686710">feature.</span>
  <span m="1687010">Think</span> <span m="1687190">of</span> <span m="1687250">that</span>
  <span m="1687370">like</span> <span m="1687550">a</span> <span m="1687610">laboratory</span>
  <span m="1688030">test</span> <span m="1688240">result,</span> <span m="1688780">for</span>
  <span m="1688870">example,</span> <span m="1689140">or</span> <span m="1689440">an</span>
  <span m="1689530">answer</span> <span m="1689830">to</span> <span m="1689920">a</span>
  <span m="1689980">question</span> <span m="1691000">that's</span> <span m="1691180">available</span>
  <span m="1691510">baseline.</span></p><p><span m="1692720">And</span> <span m="1692820">so</span>
  <span m="1693340">one</span> <span m="1693580">approach</span> <span m="1693880">to</span>
  <span m="1693970">learning</span> <span m="1694300">is</span> <span m="1694390">to</span>
  <span m="1694480">say,</span> <span m="1694630">OK,</span> <span m="1694990">let's</span>
  <span m="1695200">regularize</span> <span m="1696070">the</span> <span m="1696160">learning</span>
  <span m="1696520">of</span> <span m="1696610">these</span> <span m="1696730">different</span>
  <span m="1697030">models</span> <span m="1697570">to</span> <span m="1697750">encourage</span>
  <span m="1698260">them</span> <span m="1698560">to</span> <span m="1698740">choose</span>
  <span m="1699100">a</span> <span m="1699160">common</span> <span m="1699520">set</span>
  <span m="1699790">of</span> <span m="1699940">predictive</span> <span m="1700390">features</span>
  <span m="1700780">or</span> <span m="1700840">biomarkers.</span> <span m="1702460">But</span>
  <span m="1702550">we</span> <span m="1702670">also</span> <span m="1702880">want</span>
  <span m="1703030">to</span> <span m="1703090">allow</span> <span m="1703270">some</span>
  <span m="1703480">amount</span> <span m="1703630">of</span> <span m="1703690">flexibility.</span>
  <span m="1704410">For</span> <span m="1704530">example,</span> <span m="1705590">we</span>
  <span m="1705610">might</span> <span m="1705760">want</span> <span m="1705940">to</span>
  <span m="1706000">say</span> <span m="1706360">that,</span> <span m="1706780">well,</span>
  <span m="1706990">at</span> <span m="1707050">any</span> <span m="1707230">one</span>
  <span m="1707410">time</span> <span m="1707650">point,</span> <span m="1707890">there</span>
  <span m="1708010">might</span> <span m="1708220">be</span> <span m="1708490">couple</span>
  <span m="1708830">of</span> <span m="1708920">new</span> <span m="1709310">biomarkers</span>
  <span m="1709900">that</span> <span m="1710020">are</span> <span m="1710080">relevant</span>
  <span m="1710530">for</span> <span m="1710680">predicting</span> <span m="1711040">that</span>
  <span m="1711160">time</span> <span m="1711370">point.</span> <span m="1713910">And</span>
  <span m="1714250">there</span> <span m="1714340">might</span> <span m="1714490">be</span>
  <span m="1714580">some</span> <span m="1714760">small</span> <span m="1715090">amounts</span>
  <span m="1715330">of</span> <span m="1715390">changes</span> <span m="1715840">across</span>
  <span m="1716170">time.</span></p><p><span m="1717740">So</span> <span m="1718210">what</span>
  <span m="1718390">I'll</span> <span m="1718480">do</span> <span m="1718630">right</span>
  <span m="1718810">now</span> <span m="1719080">is</span> <span m="1719200">I'll</span>
  <span m="1719260">introduce</span> <span m="1719710">to</span> <span m="1719830">you</span>
  <span m="1720970">the</span> <span m="1721120">simplest</span> <span m="1721630">way</span>
  <span m="1721780">to</span> <span m="1721870">think</span> <span m="1722140">through</span>
  <span m="1722350">multi-task</span> <span m="1723010">learning,</span> <span m="1724630">which--</span>
  <span m="1725230">I</span> <span m="1725380">will</span> <span m="1725500">focus</span>
  <span m="1725860">specifically</span> <span m="1726520">on</span> <span m="1726910">a</span>
  <span m="1727000">linear</span> <span m="1727390">model</span> <span m="1727660">setting.</span>
  <span m="1729040">And</span> <span m="1729160">then</span> <span m="1729250">I'll</span>
  <span m="1729370">show</span> <span m="1729610">you</span> <span m="1729790">how</span>
  <span m="1730240">we</span> <span m="1730390">can</span> <span m="1731530">slightly</span>
  <span m="1732010">modify</span> <span m="1732520">this</span> <span m="1732670">simple</span>
  <span m="1733000">approach</span> <span m="1733390">to</span> <span m="1733510">capture</span>
  <span m="1733990">those</span> <span m="1734230">criteria</span> <span m="1734770">that</span>
  <span m="1734890">I</span> <span m="1734980">have</span> <span m="1735130">over</span>
  <span m="1735310">there.</span></p><p><span m="1741610">So</span> <span m="1742180">let's</span>
  <span m="1742360">talk</span> <span m="1742510">about</span> <span m="1742630">a</span>
  <span m="1742690">linear</span> <span m="1742930">model.</span> <span m="1743180">And
  let's</span> <span m="1743290">talk</span> <span m="1743440">about</span> <span
  m="1743560">regression.</span> <span m="1744130">Because</span> <span m="1744340">here,</span>
  <span m="1745080">in</span> <span m="1745150">the</span> <span m="1745210">example</span>
  <span m="1745480">I</span> <span m="1745540">showed</span> <span m="1745720">you</span>
  <span m="1745780">earlier,</span> <span m="1746120">we were</span> <span m="1746220">trying</span>
  <span m="1746280">to</span> <span m="1746340">pick</span> <span m="1746440">the</span>
  <span m="1746765">score</span> <span m="1747090">that's</span> <span m="1747260">a</span>
  <span m="1747370">continuous</span> <span m="1747760">value</span> <span m="1747980">number.</span>
  <span m="1748300">We</span> <span m="1748390">want</span> <span m="1748540">to</span>
  <span m="1748600">try</span> <span m="1748690">to</span> <span m="1748780">predict</span>
  <span m="1749080">it.</span> <span m="1749140">And</span> <span m="1749230">we</span>
  <span m="1749320">might</span> <span m="1749470">care</span> <span m="1749650">about</span>
  <span m="1749770">minimizing</span> <span m="1750340">some</span> <span m="1750670">loss</span>
  <span m="1750940">function.</span></p><p><span m="1752810">So</span> <span m="1753400">if</span>
  <span m="1753490">you</span> <span m="1753580">were</span> <span m="1753630">to</span>
  <span m="1753700">try</span> <span m="1753970">to</span> <span m="1754930">minimize</span>
  <span m="1755710">a</span> <span m="1756100">squared</span> <span m="1756730">loss,</span>
  <span m="1758000">imagine</span> <span m="1758320">a</span> <span m="1758350">scenario</span>
  <span m="1758770">where</span> <span m="1758920">you</span> <span m="1759070">had</span>
  <span m="1759340">two</span> <span m="1759730">different</span> <span m="1760240">prediction</span>
  <span m="1760660">problems.</span> <span m="1761410">So</span> <span m="1762250">this</span>
  <span m="1762460">might</span> <span m="1762700">be</span> <span m="1762960">time</span>
  <span m="1763240">point</span> <span m="1764980">0,</span> <span m="1765850">and</span>
  <span m="1765940">this</span> <span m="1766090">might</span> <span m="1766270">be</span>
  <span m="1766390">time</span> <span m="1766750">point</span> <span m="1767170">12,</span>
  <span m="1769630">for</span> <span m="1769780">six</span> <span m="1770020">months</span>
  <span m="1770210">and</span> <span m="1770290">12</span> <span m="1770500">months.</span>
  <span m="1771280">You</span> <span m="1771340">can</span> <span m="1771430">start</span>
  <span m="1771670">by</span> <span m="1771790">summing</span> <span m="1772240">over</span>
  <span m="1772810">the</span> <span m="1772930">patients,</span> <span m="1775930">looking</span>
  <span m="1776350">at</span> <span m="1776830">your</span> <span m="1777280">mean</span>
  <span m="1777580">squared</span> <span m="1778000">error</span> <span m="1778420">at</span>
  <span m="1778660">predicting</span> <span m="1779380">what</span> <span m="1779560">I'll</span>
  <span m="1779680">say</span> <span m="1780010">is</span> <span m="1782110">the</span>
  <span m="1782800">six-month</span> <span m="1783850">outcome</span> <span m="1784330">label</span>
  <span m="1786480">by</span> <span m="1786940">some</span> <span m="1787300">linear</span>
  <span m="1787660">function,</span> <span m="1788300">which,</span> <span m="1788380">I'm</span>
  <span m="1788530">going</span> <span m="1788680">to</span> <span m="1788710">have
  it</span> <span m="1788930">as</span> <span m="1790450">subscript</span> <span m="1790960">6</span>
  <span m="1791350">to</span> <span m="1791440">denote</span> <span m="1791740">that</span>
  <span m="1791890">this</span> <span m="1792070">is</span> <span m="1792280">a</span>
  <span m="1792880">linear</span> <span m="1793210">model</span> <span m="1793600">for</span>
  <span m="1794200">predicting</span> <span m="1794650">the</span> <span m="1794920">six-month</span>
  <span m="1795460">time</span> <span m="1795730">point</span> <span m="1796150">value,</span>
  <span m="1797670">dot-producted</span> <span m="1798520">with</span> <span m="1798790">your</span>
  <span m="1798910">baseline</span> <span m="1799450">features.</span></p><p><span
  m="1801670">And</span> <span m="1801820">similarly,</span> <span m="1802540">your</span>
  <span m="1802720">loss</span> <span m="1802960">function</span> <span m="1803380">for</span>
  <span m="1803650">predicting,</span> <span m="1804070">this</span> <span m="1804220">one</span>
  <span m="1804340">is</span> <span m="1804400">going</span> <span m="1804500">be</span>
  <span m="1804580">the</span> <span m="1804640">same.</span> <span m="1805160">But</span>
  <span m="1805180">now</span> <span m="1805330">you'll</span> <span m="1805480">be</span>
  <span m="1805570">predicting</span> <span m="1805990">the</span> <span m="1806380">y12</span>
  <span m="1807370">label.</span> <span m="1810550">And</span> <span m="1810670">we're</span>
  <span m="1810760">going</span> <span m="1810970">to</span> <span m="1811120">have</span>
  <span m="1811270">a</span> <span m="1811330">different</span> <span m="1811690">weight</span>
  <span m="1811900">vector</span> <span m="1812560">for</span> <span m="1812770">predicting</span>
  <span m="1813250">that.</span> <span m="1816670">Notice</span> <span m="1817000">that</span>
  <span m="1817210">x</span> <span m="1817450">is</span> <span m="1817570">the</span>
  <span m="1817660">same.</span> <span m="1817990">Because</span> <span m="1818320">I'm</span>
  <span m="1818440">assuming</span> <span m="1818950">in</span> <span m="1819340">everything</span>
  <span m="1819730">I'm</span> <span m="1819820">telling</span> <span m="1820060">you</span>
  <span m="1820150">here</span> <span m="1820480">that</span> <span m="1820660">we're</span>
  <span m="1820750">going</span> <span m="1820870">to</span> <span m="1820930">be</span>
  <span m="1821020">predicting</span> <span m="1821440">from</span> <span m="1821710">baseline</span>
  <span m="1822250">data</span> <span m="1822490">alone.</span></p><p><span m="1825530">Now,</span>
  <span m="1826690">a</span> <span m="1826750">typical</span> <span m="1827140">approach</span>
  <span m="1827410">and</span> <span m="1827490">try</span> <span m="1827620">to</span>
  <span m="1827710">regularize</span> <span m="1828220">in</span> <span m="1828280">this</span>
  <span m="1828370">setting</span> <span m="1828670">might</span> <span m="1828820">be,</span>
  <span m="1829120">let's</span> <span m="1829270">say,</span> <span m="1829420">to</span>
  <span m="1829540">do</span> <span m="1829700">L2</span> <span m="1829960">regularization.</span>
  <span m="1830650">So</span> <span m="1830800">you</span> <span m="1830860">might</span>
  <span m="1831040">say,</span> <span m="1831340">I'm</span> <span m="1831460">going</span>
  <span m="1831640">to</span> <span m="1831760">add</span> <span m="1832030">onto</span>
  <span m="1832330">this</span> <span m="1832840">some</span> <span m="1833350">lambda</span>
  <span m="1835600">times</span> <span m="1837370">the</span> <span m="1837520">weight</span>
  <span m="1837730">vector</span> <span m="1838540">6</span> <span m="1839860">squared.</span>
  <span m="1841050">Maybe--</span> <span m="1842620">same</span> <span m="1842890">thing</span>
  <span m="1843070">over</span> <span m="1843220">here.</span></p><p><span m="1852030">So</span>
  <span m="1852140">the</span> <span m="1852260">way</span> <span m="1852410">that</span>
  <span m="1852530">I</span> <span m="1852800">set</span> <span m="1853130">this</span>
  <span m="1853310">up</span> <span m="1853430">for</span> <span m="1853550">you</span>
  <span m="1853640">so</span> <span m="1853820">far,</span> <span m="1854120">right</span>
  <span m="1854300">now,</span> <span m="1854600">is</span> <span m="1854810">two</span>
  <span m="1855050">different</span> <span m="1855320">independent</span> <span m="1855740">prediction</span>
  <span m="1856100">problems.</span> <span m="1857670">The</span> <span m="1857690">next</span>
  <span m="1857900">step</span> <span m="1858110">is</span> <span m="1858200">to</span>
  <span m="1858290">talk</span> <span m="1858500">about</span> <span m="1858680">how</span>
  <span m="1858860">we</span> <span m="1858950">could</span> <span m="1859070">try</span>
  <span m="1859190">to</span> <span m="1859280">tie</span> <span m="1859520">these</span>
  <span m="1859700">together.</span> <span m="1861060">So</span> <span m="1861680">any</span>
  <span m="1861890">idea,</span> <span m="1863516">for</span> <span m="1863960">those</span>
  <span m="1864170">of</span> <span m="1864260">you</span> <span m="1864320">who</span>
  <span m="1864410">have</span> <span m="1864530">not</span> <span m="1864770">specifically</span>
  <span m="1865520">studied</span> <span m="1865820">multi-task</span> <span m="1866270">learning</span>
  <span m="1866560">in</span> <span m="1866630">class?</span> <span m="1867480">So</span>
  <span m="1867530">for</span> <span m="1867680">those</span> <span m="1867830">of</span>
  <span m="1867890">you</span> <span m="1868040">who</span> <span m="1868160">did,</span>
  <span m="1868750">don't</span> <span m="1868940">answer.</span> <span m="1869540">For</span>
  <span m="1869630">everyone</span> <span m="1869960">else,</span> <span m="1872330">what</span>
  <span m="1872540">are</span> <span m="1872600">some</span> <span m="1872780">ways</span>
  <span m="1872990">that</span> <span m="1873080">you</span> <span m="1873140">might</span>
  <span m="1873260">try</span> <span m="1873350">to</span> <span m="1873470">tie</span>
  <span m="1873830">these</span> <span m="1874010">two</span> <span m="1874160">prediction</span>
  <span m="1874520">problems</span> <span m="1874880">together?</span> <span m="1882950">Yeah.</span></p><p><span
  m="1884420">AUDIENCE:</span> <span m="1884540">Maybe</span> <span m="1884660">you</span>
  <span m="1884750">could</span> <span m="1884900">share</span> <span m="1885430">certain</span>
  <span m="1885960">weight</span> <span m="1886130">parameters,</span> <span m="1886580">so
  if</span> <span m="1886930">you've</span> <span m="1887040">got</span> <span m="1887180">a</span>
  <span m="1887240">common</span> <span m="1887520">set</span> <span m="1887880">of</span>
  <span m="1888060">biomarkers.</span></p><p><span m="1889740">DAVID SONTAG:</span>
  <span m="1889815">So</span> <span m="1889890">maybe</span> <span m="1890050">you</span>
  <span m="1890100">could</span> <span m="1890190">share</span> <span m="1890520">some</span>
  <span m="1890760">weight</span> <span m="1890970">parameters.</span> <span m="1891285">Well,</span>
  <span m="1891600">I</span> <span m="1891660">mean,</span> <span m="1891750">the</span>
  <span m="1891810">simplest</span> <span m="1892200">way</span> <span m="1892290">to</span>
  <span m="1892380">tie</span> <span m="1892500">them</span> <span m="1892620">together</span>
  <span m="1892920">is</span> <span m="1893040">just</span> <span m="1893250">to</span>
  <span m="1893370">say,</span> <span m="1895530">we're</span> <span m="1895650">going</span>
  <span m="1895920">to--</span> <span m="1897625">so</span> <span m="1897930">you</span>
  <span m="1897990">might</span> <span m="1898170">say,</span> <span m="1898590">let's</span>
  <span m="1898770">first</span> <span m="1898980">of</span> <span m="1899070">all</span>
  <span m="1899160">add</span> <span m="1899430">these</span> <span m="1899610">two</span>
  <span m="1899730">objective</span> <span m="1900060">functions</span> <span m="1900420">together.</span>
  <span m="1902820">And</span> <span m="1902970">now</span> <span m="1903120">we're</span>
  <span m="1903270">going</span> <span m="1903540">to</span> <span m="1903930">minimize--</span>
  <span m="1904830">instead</span> <span m="1905310">of</span> <span m="1905880">minimizing</span>
  <span m="1908550">just--</span> <span m="1910260">now</span> <span m="1910440">we're</span>
  <span m="1910530">going</span> <span m="1910650">to</span> <span m="1910710">minimize</span>
  <span m="1911130">over</span> <span m="1911540">the</span> <span m="1911640">two</span>
  <span m="1911890">weight</span> <span m="1912090">vectors</span> <span m="1912810">jointly.</span></p><p><span
  m="1917280">So</span> <span m="1917400">now</span> <span m="1917520">we</span> <span
  m="1917610">have</span> <span m="1917730">a</span> <span m="1917790">single</span>
  <span m="1918150">optimization</span> <span m="1918750">problem.</span> <span m="1919110">All</span>
  <span m="1919290">I've</span> <span m="1919380">done</span> <span m="1919560">is</span>
  <span m="1920040">I've</span> <span m="1920400">now--</span> <span m="1920670">we're</span>
  <span m="1920820">optimizing.</span> <span m="1921390">We're</span> <span m="1921510">minimizing</span>
  <span m="1922230">this</span> <span m="1922450">joint</span> <span m="1922740">objective</span>
  <span m="1923100">where</span> <span m="1923190">I'm</span> <span m="1923340">summing</span>
  <span m="1923850">this</span> <span m="1924030">objective</span> <span m="1924660">with</span>
  <span m="1924960">this</span> <span m="1925110">objective.</span> <span m="1926880">We're</span>
  <span m="1927030">minimizing</span> <span m="1927510">it</span> <span m="1927570">with
  respect</span> <span m="1927855">to</span> <span m="1928140">now</span> <span m="1928410">two</span>
  <span m="1928710">different</span> <span m="1928980">weight</span> <span m="1929160">vectors.</span>
  <span m="1929940">And</span> <span m="1930090">the</span> <span m="1930150">simplest</span>
  <span m="1930480">thing</span> <span m="1930630">to</span> <span m="1930720">do</span>
  <span m="1930810">what</span> <span m="1930930">you</span> <span m="1930990">just</span>
  <span m="1931170">described</span> <span m="1931560">might</span> <span m="1931710">be</span>
  <span m="1931800">to</span> <span m="1931920">say,</span> <span m="1932340">let's</span>
  <span m="1932640">let</span> <span m="1933540">W6</span> <span m="1935070">equal</span>
  <span m="1935610">to</span> <span m="1935790">W12.</span></p><p><span m="1939020">So</span>
  <span m="1939240">you</span> <span m="1939300">might</span> <span m="1939450">just</span>
  <span m="1939660">add</span> <span m="1940050">in</span> <span m="1940320">this</span>
  <span m="1940890">equality</span> <span m="1941490">constraint</span> <span m="1942060">saying</span>
  <span m="1942510">that</span> <span m="1943170">these</span> <span m="1943590">two</span>
  <span m="1943830">weight</span> <span m="1944040">vectors</span> <span m="1944430">should</span>
  <span m="1944610">be</span> <span m="1944880">identical.</span> <span m="1946570">What</span>
  <span m="1946800">would</span> <span m="1946920">be</span> <span m="1947040">wrong</span>
  <span m="1947340">with</span> <span m="1947550">that?</span> <span m="1948180">Someone</span>
  <span m="1948450">else,</span> <span m="1949020">what</span> <span m="1949170">would</span>
  <span m="1949260">be</span> <span m="1949410">wrong</span> <span m="1949710">with--</span>
  <span m="1950090">and</span> <span m="1950130">I</span> <span m="1950190">know</span>
  <span m="1950340">that</span> <span m="1950460">wasn't</span> <span m="1950700">precisely</span>
  <span m="1950990">your</span> <span m="1951060">suggestion.</span> <span m="1951420">So
  don't</span> <span m="1951756">worry.</span></p><p><span m="1952092">AUDIENCE:</span>
  <span m="1952159">I</span> <span m="1952226">have</span> <span m="1952293">a</span>
  <span m="1952360">question.</span></p><p><span m="1952430">DAVID SONTAG:</span>
  <span m="1952525">Yeah.</span> <span m="1952620">What's</span> <span m="1952740">your</span>
  <span m="1952800">question?</span></p><p><span m="1953040">AUDIENCE:</span> <span
  m="1953220">Is</span> <span m="1953400">x--</span> <span m="1953900">are</span>
  <span m="1954230">those</span> <span m="1954630">also</span> <span m="1955000">different?</span></p><p><span
  m="1955920">DAVID SONTAG:</span> <span m="1956040">Sorry.</span> <span m="1956160">Yeah.</span>
  <span m="1956370">I'm</span> <span m="1956430">missing</span> <span m="1956670">some</span>
  <span m="1956850">subscripts,</span> <span m="1957320">right.</span> <span m="1958000">So</span>
  <span m="1961770">I'll</span> <span m="1961830">put</span> <span m="1961950">this</span>
  <span m="1962070">in</span> <span m="1962170">superscript.</span> <span m="1963400">And</span>
  <span m="1963570">I'll</span> <span m="1963630">put</span> <span m="1963810">subscript</span>
  <span m="1964500">i,</span> <span m="1965010">subscript</span> <span m="1965640">i.</span>
  <span m="1971260">And</span> <span m="1972040">it</span> <span m="1972460">doesn't</span>
  <span m="1972700">matter</span> <span m="1974830">for</span> <span m="1975010">the</span>
  <span m="1975160">purpose</span> <span m="1975490">of</span> <span m="1975550">this</span>
  <span m="1975760">presentation</span> <span m="1976460">whether</span> <span m="1976660">these</span>
  <span m="1976810">are</span> <span m="1976870">the</span> <span m="1976990">same</span>
  <span m="1977230">individuals</span> <span m="1977620">or</span> <span m="1977680">different</span>
  <span m="1977890">individuals</span> <span m="1979735">across</span> <span m="1981040">these</span>
  <span m="1981190">two</span> <span m="1981280">problems.</span> <span m="1981820">You</span>
  <span m="1981910">can</span> <span m="1982030">imagine</span> <span m="1982270">they're</span>
  <span m="1982360">the</span> <span m="1982450">same</span> <span m="1982660">individual.</span></p><p><span
  m="1984620">So</span> <span m="1985120">you</span> <span m="1985240">might</span>
  <span m="1985390">imagine</span> <span m="1985690">that</span> <span m="1985870">there</span>
  <span m="1986170">are</span> <span m="1986680">n</span> <span m="1987010">individuals</span>
  <span m="1987460">in</span> <span m="1987550">the</span> <span m="1987640">data</span>
  <span m="1987970">set.</span> <span m="1989020">And</span> <span m="1989140">we're</span>
  <span m="1989230">summing</span> <span m="1989590">over</span> <span m="1989860">the</span>
  <span m="1989950">same</span> <span m="1990300">n</span> <span m="1990490">people</span>
  <span m="1990850">for</span> <span m="1991000">both</span> <span m="1991190">of</span>
  <span m="1991230">these</span> <span m="1991350">sums,</span> <span m="1991960">just</span>
  <span m="1992140">looking</span> <span m="1992350">at</span> <span m="1992440">different</span>
  <span m="1992860">outcomes</span> <span m="1993460">for</span> <span m="1993520">each</span>
  <span m="1993640">of</span> <span m="1993700">them.</span> <span m="1993910">This</span>
  <span m="1994120">is</span> <span m="1994270">the</span> <span m="1994420">six-month</span>
  <span m="1995170">outcome.</span> <span m="1995720">This</span> <span m="1995770">is</span>
  <span m="1995860">the</span> <span m="1996100">12-month</span> <span m="1996640">outcome.</span>
  <span m="1997820">Is</span> <span m="1997930">that</span> <span m="1998020">clear?</span></p><p><span
  m="2000040">All right.</span> <span m="2000210">So</span> <span m="2000330">the</span>
  <span m="2000420">simplest</span> <span m="2000780">thing</span> <span m="2000870">to</span>
  <span m="2000990">do</span> <span m="2001110">would</span> <span m="2001200">be</span>
  <span m="2001290">just</span> <span m="2001500">to</span> <span m="2001630">not--</span>
  <span m="2001800">now</span> <span m="2001950">that</span> <span m="2002040">we</span>
  <span m="2002130">have</span> <span m="2002250">a</span> <span m="2002310">joint</span>
  <span m="2002580">optimization</span> <span m="2003060">problem,</span> <span m="2003870">we</span>
  <span m="2003990">could</span> <span m="2004200">constrain</span> <span m="2004740">the</span>
  <span m="2004830">two</span> <span m="2005010">weight</span> <span m="2005130">vectors</span>
  <span m="2005520">to</span> <span m="2005580">be</span> <span m="2005670">identical.</span>
  <span m="2007440">But</span> <span m="2007560">of</span> <span m="2007620">course,</span>
  <span m="2007800">this</span> <span m="2007920">is</span> <span m="2007980">a</span>
  <span m="2008010">bit</span> <span m="2008130">of</span> <span m="2008190">an</span>
  <span m="2008280">overkill.</span> <span m="2008700">This</span> <span m="2008850">is</span>
  <span m="2008940">like</span> <span m="2009120">saying</span> <span m="2009420">that</span>
  <span m="2012162">you're</span> <span m="2012600">going</span> <span m="2012930">to</span>
  <span m="2014370">just</span> <span m="2014610">learn</span> <span m="2014850">a</span>
  <span m="2014910">single</span> <span m="2015240">prediction</span> <span m="2015630">problem,</span>
  <span m="2016140">where</span> <span m="2016290">you</span> <span m="2016410">sort</span>
  <span m="2016590">of</span> <span m="2016740">ignore</span> <span m="2017700">the</span>
  <span m="2018000">difference</span> <span m="2018450">between</span> <span m="2018870">six</span>
  <span m="2019140">months</span> <span m="2019320">and</span> <span m="2019410">12</span>
  <span m="2019590">months</span> <span m="2019800">and</span> <span m="2019890">just</span>
  <span m="2020040">try</span> <span m="2020160">to</span> <span m="2020280">predict--</span>
  <span m="2021720">you</span> <span m="2021820">put</span> <span m="2021990">those</span>
  <span m="2022200">under</span> <span m="2022410">there</span> <span m="2022560">and</span>
  <span m="2022650">just</span> <span m="2022770">predict them</span> <span m="2023100">both</span>
  <span m="2023310">together.</span> <span m="2024140">So</span> <span m="2024150">you</span>
  <span m="2024360">had</span> <span m="2024450">another</span> <span m="2024690">suggestion,</span>
  <span m="2024990">it</span> <span m="2025110">sounded</span> <span m="2025290">like.</span></p><p><span
  m="2026000">AUDIENCE:</span> <span m="2026090">Oh,</span> <span m="2026180">no.</span>
  <span m="2026580">You</span> <span m="2026760">had</span> <span m="2027020">just</span>
  <span m="2027250">asked</span> <span m="2027660">why</span> <span m="2027840">that</span>
  <span m="2027960">was</span> <span m="2028140">not it.</span></p><p><span m="2028360">DAVID
  SONTAG:</span> <span m="2028500">Oh,</span> <span m="2028640">OK.</span> <span m="2029040">And</span>
  <span m="2029130">I</span> <span m="2029250">answered</span> <span m="2029480">that.</span>
  <span m="2029650">Sorry.</span> <span m="2030900">What</span> <span m="2031080">could
  we</span> <span m="2031170">do</span> <span m="2031230">differently?</span> <span
  m="2031600">Yeah,</span> <span m="2031750">you.</span></p><p><span m="2032970">AUDIENCE:</span>
  <span m="2033056">You</span> <span m="2033142">could</span> <span m="2033230">maybe</span>
  <span m="2033710">try to</span> <span m="2034190">minimize</span> <span m="2034670">the</span>
  <span m="2035150">difference</span> <span m="2035620">between</span> <span m="2035915">the
  two.</span> <span m="2036210">So</span> <span m="2037200">I'm</span> <span m="2037340">not</span>
  <span m="2037530">saying</span> <span m="2037800">that they</span> <span m="2038090">need
  to</span> <span m="2038400">be the</span> <span m="2038460">same.</span> <span m="2039030">But</span>
  <span m="2040110">the</span> <span m="2040200">chances</span> <span m="2040640">that
  they're</span> <span m="2040830">going to be</span> <span m="2041050">super,</span>
  <span m="2041405">super</span> <span m="2041760">different</span> <span m="2042398">isn't
  really</span> <span m="2042886">high.</span></p><p><span m="2044840">DAVID SONTAG:</span>
  <span m="2044945">That's</span> <span m="2045050">a very</span> <span m="2045170">interesting</span>
  <span m="2045470">idea.</span> <span m="2045750">So</span> <span m="2045800">we</span>
  <span m="2045890">don't</span> <span m="2046070">want</span> <span m="2046250">them</span>
  <span m="2046370">to</span> <span m="2046460">be</span> <span m="2046520">the</span>
  <span m="2046610">same.</span> <span m="2046880">But</span> <span m="2047150">I</span>
  <span m="2047270">might</span> <span m="2047450">want</span> <span m="2047630">them</span>
  <span m="2047780">to</span> <span m="2047930">be</span> <span m="2048199">approximately</span>
  <span m="2049159">the</span> <span m="2049280">same,</span> <span m="2049639">right?</span></p><p><span
  m="2050390">AUDIENCE:</span> <span m="2050615">Yeah.</span></p><p><span m="2050840">DAVID
  SONTAG:</span> <span m="2050900">And</span> <span m="2050960">what's</span> <span
  m="2051380">one</span> <span m="2051590">way</span> <span m="2051800">to</span>
  <span m="2051920">try</span> <span m="2052070">to</span> <span m="2052190">measure</span>
  <span m="2052730">how</span> <span m="2053060">different</span> <span m="2053570">these</span>
  <span m="2053780">two</span> <span m="2053989">are?</span></p><p><span m="2055429">AUDIENCE:</span>
  <span m="2055634">Subtract</span> <span m="2055839">them.</span></p><p><span m="2056250">DAVID
  SONTAG:</span> <span m="2056392">Subtract</span> <span m="2056820">them,</span>
  <span m="2057540">and</span> <span m="2057690">then</span> <span m="2058260">do</span>
  <span m="2058469">what?</span> <span m="2059899">So</span> <span m="2060179">these</span>
  <span m="2060389">are</span> <span m="2060480">vectors.</span> <span m="2061000">So
  you--</span></p><p><span m="2061230">AUDIENCE:</span> <span m="2061335">Absolute</span>
  <span m="2061440">value.</span></p><p><span m="2062760">DAVID SONTAG:</span> <span
  m="2062965">So</span> <span m="2063960">it's</span> <span m="2064650">not</span>
  <span m="2064860">absolute</span> <span m="2065159">value</span> <span m="2065420">of</span>
  <span m="2065469">a</span> <span m="2065520">vector.</span> <span m="2065900">What</span>
  <span m="2066030">can</span> <span m="2066150">you</span> <span m="2066210">do</span>
  <span m="2066330">to</span> <span m="2066449">turn</span> <span m="2066679">a</span>
  <span m="2066719">vector</span> <span m="2067020">into</span> <span m="2067170">a</span>
  <span m="2067230">single</span> <span m="2067500">number?</span></p><p><span m="2068275">AUDIENCE:</span>
  <span m="2068433">Take</span> <span m="2068591">the</span> <span m="2068750">norm</span>
  <span m="2069225">[INAUDIBLE].</span></p><p><span m="2070179">DAVID SONTAG:</span>
  <span m="2070234">Take</span> <span m="2070290">a</span> <span m="2070350">norm</span>
  <span m="2070620">of</span> <span m="2070710">it.</span> <span m="2070800">Yeah.</span>
  <span m="2071489">I</span> <span m="2071520">think</span> <span m="2071730">what</span>
  <span m="2071820">you</span> <span m="2071880">meant.</span> <span m="2073080">So</span>
  <span m="2073380">we</span> <span m="2073469">might</span> <span m="2073590">take</span>
  <span m="2073739">the</span> <span m="2073830">norm</span> <span m="2074010">of</span>
  <span m="2074070">it.</span> <span m="2074159">What</span> <span m="2074300">norm</span>
  <span m="2074520">should</span> <span m="2074639">we</span> <span m="2074730">take?</span></p><p><span
  m="2075536">AUDIENCE:</span> <span m="2075774">L2?</span></p><p><span m="2076489">DAVID
  SONTAG:</span> <span m="2076589">Maybe the</span> <span m="2076690">L2</span> <span
  m="2076980">norm.</span> <span m="2077969">OK.</span> <span m="2079500">And</span>
  <span m="2079920">we</span> <span m="2080040">might</span> <span m="2080250">say</span>
  <span m="2080489">we</span> <span m="2080639">want</span> <span m="2080880">that.</span>
  <span m="2081690">So</span> <span m="2081929">if</span> <span m="2082080">we</span>
  <span m="2082199">said</span> <span m="2082350">that</span> <span m="2082469">this</span>
  <span m="2082600">was</span> <span m="2082710">equal</span> <span m="2082980">to</span>
  <span m="2083460">0,</span> <span m="2084630">then,</span> <span m="2084780">of</span>
  <span m="2084870">course,</span> <span m="2085080">that's</span> <span m="2085230">saying</span>
  <span m="2085440">that</span> <span m="2085530">they</span> <span m="2085590">have</span>
  <span m="2085739">to</span> <span m="2085830">be</span> <span m="2085920">the</span>
  <span m="2085980">same.</span></p><p><span m="2087210">But</span> <span m="2087389">we</span>
  <span m="2087480">could</span> <span m="2087630">say</span> <span m="2087900">that</span>
  <span m="2088050">this</span> <span m="2088320">is,</span> <span m="2088650">let's</span>
  <span m="2088830">say,</span> <span m="2089400">bounded</span> <span m="2090090">by</span>
  <span m="2090659">some</span> <span m="2091679">epsilon.</span> <span m="2092600">And</span>
  <span m="2092699">epsilon</span> <span m="2093060">now</span> <span m="2093210">is</span>
  <span m="2093300">a</span> <span m="2093360">parameter</span> <span m="2093750">we</span>
  <span m="2093870">get</span> <span m="2093989">to</span> <span m="2094080">choose.</span>
  <span m="2095150">And</span> <span m="2095250">that</span> <span m="2095370">would</span>
  <span m="2095520">then</span> <span m="2095670">say,</span> <span m="2095820">oh,</span>
  <span m="2096179">OK,</span> <span m="2096540">we've</span> <span m="2096690">now</span>
  <span m="2096900">tied</span> <span m="2097470">together</span> <span m="2097980">these</span>
  <span m="2098190">two</span> <span m="2098400">optimization</span> <span m="2099060">problems.</span>
  <span m="2100650">And</span> <span m="2101340">we</span> <span m="2102560">want</span>
  <span m="2102780">to</span> <span m="2102870">encourage</span> <span m="2103500">that</span>
  <span m="2103860">the</span> <span m="2104010">two</span> <span m="2104280">weight</span>
  <span m="2104490">vectors</span> <span m="2104910">are</span> <span m="2105030">not</span>
  <span m="2105270">that</span> <span m="2105450">far</span> <span m="2105630">from</span>
  <span m="2105780">each</span> <span m="2105900">other.</span> <span m="2107556">Yep?</span></p><p><span
  m="2108540">AUDIENCE:</span> <span m="2108595">You</span> <span m="2108650">represent</span>
  <span m="2109070">each</span> <span m="2109250">weight</span> <span m="2109370">vector</span>
  <span m="2109730">as--</span> <span m="2110930">have</span> <span m="2111250">it</span>
  <span m="2111390">just</span> <span m="2112030">be</span> <span m="2112250">duplicated</span>
  <span m="2113090">and</span> <span m="2113320">force</span> <span m="2113690">the</span>
  <span m="2113780">first</span> <span m="2114470">place</span> <span m="2114800">to</span>
  <span m="2114860">be</span> <span m="2115010">the</span> <span m="2115100">same</span>
  <span m="2115490">and</span> <span m="2115990">the second ones</span> <span m="2116490">to
  be</span> <span m="2117490">different.</span></p><p><span m="2118900">DAVID SONTAG:</span>
  <span m="2118975">You're</span> <span m="2119050">suggesting</span> <span m="2119530">a</span>
  <span m="2119590">slightly</span> <span m="2119890">different</span> <span m="2120160">way</span>
  <span m="2120310">to</span> <span m="2120760">parameterize</span> <span m="2121660">this</span>
  <span m="2121960">by</span> <span m="2122110">saying</span> <span m="2122410">that</span>
  <span m="2122560">W12</span> <span m="2123700">is</span> <span m="2123880">equal</span>
  <span m="2124240">to</span> <span m="2124510">W6</span> <span m="2125320">plus</span>
  <span m="2125920">some</span> <span m="2126790">delta</span> <span m="2127260">function,</span>
  <span m="2127700">some</span> <span m="2127900">delta</span> <span m="2128500">difference.</span>
  <span m="2128840">Is</span> <span m="2129080">that</span> <span m="2129230">you're</span>
  <span m="2129350">suggesting?</span></p><p><span m="2129970">AUDIENCE:</span> <span
  m="2130105">No,</span> <span m="2130240">that</span> <span m="2130870">you</span>
  <span m="2131050">have</span> <span m="2131230">your--</span> <span m="2131440">say</span>
  <span m="2131860">it's</span> <span m="2132340">n-dimensional,</span> <span m="2133000">like</span>
  <span m="2133360">each vector is</span> <span m="2133780">n-dimensional.</span>
  <span m="2134090">But</span> <span m="2134400">now</span> <span m="2134620">it's</span>
  <span m="2134740">going</span> <span m="2134860">to</span> <span m="2134920">be</span>
  <span m="2135370">2n-dimensional.</span> <span m="2136330">And</span> <span m="2136470">you</span>
  <span m="2136570">force</span> <span m="2136850">the</span> <span m="2136950">first</span>
  <span m="2137290">n</span> <span m="2137585">dimensions</span> <span m="2137880">to</span>
  <span m="2137950">be</span> <span m="2138070">the</span> <span m="2138160">same</span>
  <span m="2138490">on</span> <span m="2138580">the</span> <span m="2138640">weight</span>
  <span m="2138790">vector.</span> <span m="2139260">And</span> <span m="2139680">then</span>
  <span m="2140080">the</span> <span m="2140480">others,</span> <span m="2140880">you--</span></p><p><span
  m="2141280">DAVID SONTAG:</span> <span m="2141336">Now,</span> <span m="2141392">that's</span>
  <span m="2141450">a really</span> <span m="2141760">interesting</span> <span m="2142090">idea.</span>
  <span m="2143620">I'll</span> <span m="2144040">return</span> <span m="2144430">to</span>
  <span m="2144520">that</span> <span m="2144640">point</span> <span m="2144820">in</span>
  <span m="2144880">just</span> <span m="2145060">a</span> <span m="2145090">second.</span>
  <span m="2145930">Thanks.</span></p><p><span m="2147370">Before</span> <span m="2147710">I</span>
  <span m="2147770">return</span> <span m="2148030">to</span> <span m="2148090">that</span>
  <span m="2148210">point,</span> <span m="2148390">I</span> <span m="2148450">just</span>
  <span m="2148570">want</span> <span m="2148810">to</span> <span m="2149440">point</span>
  <span m="2149770">out</span> <span m="2150160">this</span> <span m="2150340">isn't</span>
  <span m="2150580">the</span> <span m="2150640">most</span> <span m="2150900">immediate</span>
  <span m="2151210">think</span> <span m="2151420">optimize.</span> <span m="2152350">Because</span>
  <span m="2152530">this</span> <span m="2152650">is</span> <span m="2152770">now
  a</span> <span m="2152950">constrained</span> <span m="2153400">optimization</span>
  <span m="2153880">problem.</span> <span m="2154700">What's</span> <span m="2154990">our</span>
  <span m="2155230">favorite</span> <span m="2155770">algorithm</span> <span m="2156220">for</span>
  <span m="2156610">convex</span> <span m="2157090">optimization</span> <span m="2157610">in</span>
  <span m="2157690">machine</span> <span m="2157930">learning,</span> <span m="2158170">and</span>
  <span m="2158290">non-convex</span> <span m="2158740">optimization?</span> <span
  m="2159550">Everyone</span> <span m="2159790">say it</span> <span m="2159910">out</span>
  <span m="2160000">loud.</span></p><p><span m="2160240">AUDIENCE:</span> <span m="2160455">Stochastic</span>
  <span m="2161100">gradient</span> <span m="2161530">descent.</span></p><p><span
  m="2163250">DAVID SONTAG:</span> <span m="2163500">TAs</span> <span m="2163750">are</span>
  <span m="2163810">not</span> <span m="2163960">supposed</span> <span m="2164230">to</span>
  <span m="2164440">answer.</span></p><p><span m="2165295">AUDIENCE:</span> <span
  m="2165527">Just</span> <span m="2165760">muttering.</span></p><p><span m="2167620">DAVID
  SONTAG:</span> <span m="2167785">Neither</span> <span m="2167950">are</span> <span
  m="2168040">faculty.</span> <span m="2170880">But</span> <span m="2170950">I</span>
  <span m="2171040">think</span> <span m="2171190">I</span> <span m="2171250">heard</span>
  <span m="2171400">enough</span> <span m="2171610">of</span> <span m="2171700">you</span>
  <span m="2171820">say</span> <span m="2172030">stochastic</span> <span m="2172540">gradient</span>
  <span m="2172870">descent.</span> <span m="2173260">Yes.</span> <span m="2173470">Good.</span>
  <span m="2174070">That's</span> <span m="2174220">what</span> <span m="2174310">I</span>
  <span m="2174340">was</span> <span m="2174430">expecting.</span></p><p><span m="2175670">And</span>
  <span m="2176350">well,</span> <span m="2176680">you</span> <span m="2176800">could</span>
  <span m="2177010">do</span> <span m="2177160">projected</span> <span m="2178330">gradient</span>
  <span m="2178750">descent.</span> <span m="2179460">But</span> <span m="2179650">it's</span>
  <span m="2179740">much</span> <span m="2179920">easier</span> <span m="2180160">to</span>
  <span m="2180250">just</span> <span m="2180520">get</span> <span m="2180670">rid</span>
  <span m="2180820">of</span> <span m="2180880">this.</span> <span m="2181190">And</span>
  <span m="2181290">so</span> <span m="2181300">what</span> <span m="2181390">we're</span>
  <span m="2181480">going</span> <span m="2181660">to</span> <span m="2181780">do</span>
  <span m="2181900">is</span> <span m="2181960">we're</span> <span m="2182050">just</span>
  <span m="2182170">going</span> <span m="2182240">to</span> <span m="2182320">put</span>
  <span m="2182470">this</span> <span m="2182590">into</span> <span m="2182770">the</span>
  <span m="2182830">objective</span> <span m="2183190">function.</span> <span m="2184510">And</span>
  <span m="2185470">one</span> <span m="2185710">way</span> <span m="2185830">to</span>
  <span m="2185950">do</span> <span m="2186100">that--</span> <span m="2186370">so</span>
  <span m="2187840">one</span> <span m="2188950">motivation</span> <span m="2189490">would</span>
  <span m="2189580">be</span> <span m="2189650">to</span> <span m="2189690">say</span>
  <span m="2189850">we're</span> <span m="2189940">going to</span> <span m="2190030">take</span>
  <span m="2190200">the</span> <span m="2190330">Lagrangian</span> <span m="2190900">of</span>
  <span m="2190960">this</span> <span m="2191140">inequality.</span> <span m="2192380">And</span>
  <span m="2192460">then</span> <span m="2192610">that'll</span> <span m="2192850">bring</span>
  <span m="2193060">this</span> <span m="2193240">into</span> <span m="2193390">the</span>
  <span m="2193450">objective.</span></p><p><span m="2194030">But</span> <span m="2194200">you</span>
  <span m="2194290">know</span> <span m="2194410">what?</span> <span m="2194590">Screw</span>
  <span m="2194830">that</span> <span m="2194980">motivation.</span> <span m="2195630">Let's</span>
  <span m="2195670">just</span> <span m="2195840">erase</span> <span m="2196120">this.</span>
  <span m="2198640">And</span> <span m="2199180">I'll</span> <span m="2199450">just</span>
  <span m="2200140">say</span> <span m="2201040">plus</span> <span m="2202360">something</span>
  <span m="2202720">else.</span> <span m="2203150">So</span> <span m="2203260">I'll</span>
  <span m="2203350">call</span> <span m="2203530">that</span> <span m="2204370">lambda</span>
  <span m="2204730">1,</span> <span m="2205150">some</span> <span m="2205420">other</span>
  <span m="2205870">hyper-parameter,</span> <span m="2207130">times</span> <span m="2208450">now</span>
  <span m="2209380">W12</span> <span m="2212140">minus</span> <span m="2212830">W6</span>
  <span m="2214810">squared.</span></p><p><span m="2217090">Now</span> <span m="2217240">let's</span>
  <span m="2217360">look</span> <span m="2217510">to</span> <span m="2217570">see</span>
  <span m="2217720">what</span> <span m="2217840">happens.</span> <span m="2218260">If</span>
  <span m="2218380">we</span> <span m="2218440">were</span> <span m="2218530">to</span>
  <span m="2218620">push</span> <span m="2218920">this</span> <span m="2219100">lambda</span>
  <span m="2219430">2</span> <span m="2219730">to</span> <span m="2220030">infinity,</span>
  <span m="2221870">remember</span> <span m="2222100">we're</span> <span m="2222250">minimizing</span>
  <span m="2223150">this</span> <span m="2223280">objective</span> <span m="2223720">function.</span>
  <span m="2224660">So if</span> <span m="2224800">lambda</span> <span m="2225130">2</span>
  <span m="2225310">is</span> <span m="2225460">pushed</span> <span m="2225690">to</span>
  <span m="2225760">infinity,</span> <span m="2229390">what</span> <span m="2229870">is</span>
  <span m="2230110">the</span> <span m="2230200">solution</span> <span m="2230740">of</span>
  <span m="2230860">W12</span> <span m="2231700">with</span> <span m="2231910">respect</span>
  <span m="2232300">to</span> <span m="2232480">W6?</span> <span m="2233500">Everyone</span>
  <span m="2233800">say it</span> <span m="2233920">out</span> <span m="2234010">loud.</span></p><p><span
  m="2234640">AUDIENCE:</span> <span m="2234830">0.</span></p><p><span m="2236140">DAVID
  SONTAG:</span> <span m="2236170">I</span> <span m="2236200">said</span> <span m="2236320">&quot;with</span>
  <span m="2236440">respect</span> <span m="2236700">to.&quot;</span> <span m="2236860">So</span>
  <span m="2237370">there,</span> <span m="2237550">1</span> <span m="2237730">minus</span>
  <span m="2237960">other</span> <span m="2238130">is</span> <span m="2238200">0.</span>
  <span m="2239080">Yes.</span> <span m="2239340">Good.</span></p><p><span m="2240060">All</span>
  <span m="2240260">right.</span> <span m="2240430">So</span> <span m="2240730">it
  would</span> <span m="2241060">be</span> <span m="2241180">forcing</span> <span
  m="2241660">them</span> <span m="2242050">that</span> <span m="2242500">they</span>
  <span m="2242710">be</span> <span m="2242860">the</span> <span m="2242950">same.</span>
  <span m="2244100">And</span> <span m="2244120">of</span> <span m="2244210">course,</span>
  <span m="2244450">if</span> <span m="2244540">lambda</span> <span m="2244810">2</span>
  <span m="2245020">is</span> <span m="2245080">smaller,</span> <span m="2245590">then
  it's</span> <span m="2245840">saying</span> <span m="2246190">we're</span> <span
  m="2246280">going</span> <span m="2246360">to</span> <span m="2246430">allow</span>
  <span m="2246640">some</span> <span m="2246790">flexibility.</span> <span m="2247270">They</span>
  <span m="2247330">don't</span> <span m="2247450">have</span> <span m="2247570">to</span>
  <span m="2247660">be</span> <span m="2247720">the</span> <span m="2247810">same.</span>
  <span m="2248220">But</span> <span m="2248230">we're</span> <span m="2248320">going</span>
  <span m="2248440">to</span> <span m="2248500">penalize</span> <span m="2248950">their</span>
  <span m="2249060">difference</span> <span m="2249400">by</span> <span m="2249520">the</span>
  <span m="2249620">squared</span> <span m="2250480">difference</span> <span m="2250810">in</span>
  <span m="2250870">their</span> <span m="2250960">norms.</span></p><p><span m="2256240">So</span>
  <span m="2256420">this</span> <span m="2256600">is</span> <span m="2256720">good.</span>
  <span m="2257020">And</span> <span m="2257500">so</span> <span m="2257650">you</span>
  <span m="2258010">raised</span> <span m="2258220">a</span> <span m="2258250">really</span>
  <span m="2258400">interesting</span> <span m="2258700">question,</span> <span m="2260500">which</span>
  <span m="2260970">I'll</span> <span m="2261100">talk</span> <span m="2261340">about</span>
  <span m="2261520">now,</span> <span m="2262370">which</span> <span m="2262420">is,</span>
  <span m="2262510">well,</span> <span m="2262630">maybe</span> <span m="2262900">you</span>
  <span m="2262960">don't</span> <span m="2263110">want</span> <span m="2263230">to</span>
  <span m="2263290">enforce</span> <span m="2263650">all</span> <span m="2263860">of</span>
  <span m="2263920">the</span> <span m="2264010">dimensions</span> <span m="2264490">to</span>
  <span m="2264580">be</span> <span m="2264670">the</span> <span m="2264730">same.</span>
  <span m="2265100">Maybe</span> <span m="2265210">that's</span> <span m="2265420">too</span>
  <span m="2265600">much.</span> <span m="2266410">So</span> <span m="2267640">one</span>
  <span m="2268240">thing</span> <span m="2268510">one</span> <span m="2268720">could</span>
  <span m="2269050">imagine</span> <span m="2269380">doing</span> <span m="2269770">is</span>
  <span m="2269860">saying,</span> <span m="2270980">we're</span> <span m="2271030">going</span>
  <span m="2271240">to</span> <span m="2271330">only</span> <span m="2271600">enforce</span>
  <span m="2272080">this</span> <span m="2272410">constraint</span> <span m="2273710">for--</span>
  <span m="2274380">[INAUDIBLE]</span> <span m="2274960">we're</span> <span m="2275050">only</span>
  <span m="2275110">going</span> <span m="2275200">to</span> <span m="2275380">put</span>
  <span m="2275470">this</span> <span m="2275620">penalty</span> <span m="2275980">in</span>
  <span m="2276160">for,</span> <span m="2276340">let's</span> <span m="2276520">say,</span>
  <span m="2278900">dimensions--</span> <span m="2283730">trying</span> <span m="2283940">to</span>
  <span m="2284090">think</span> <span m="2284230">the</span> <span m="2284290">right</span>
  <span m="2284440">notation</span> <span m="2284890">for</span> <span m="2285010">this.</span>
  <span m="2285490">I</span> <span m="2285520">think</span> <span m="2285670">I'll</span>
  <span m="2285760">use</span> <span m="2286180">this</span> <span m="2286360">notation.</span>
  <span m="2286655">Let's see</span> <span m="2286950">if</span> <span m="2287080">you</span>
  <span m="2287170">guys</span> <span m="2287350">like</span> <span m="2287530">this.</span></p><p><span
  m="2298350">Let's</span> <span m="2298450">see</span> <span m="2298580">if</span>
  <span m="2298630">this</span> <span m="2298750">notation</span> <span m="2299050">makes</span>
  <span m="2299200">sense</span> <span m="2299410">for</span> <span m="2299530">you.</span>
  <span m="2299750">What</span> <span m="2299770">I'm</span> <span m="2299860">saying</span>
  <span m="2300130">is</span> <span m="2300220">I'm</span> <span m="2300280">going</span>
  <span m="2300390">to</span> <span m="2300460">take</span> <span m="2300940">the--</span>
  <span m="2301660">d</span> <span m="2301960">is the</span> <span m="2302070">dimension.</span>
  <span m="2303090">I'm</span> <span m="2303220">going</span> <span m="2303340">to</span>
  <span m="2303400">take</span> <span m="2303730">the</span> <span m="2304120">first</span>
  <span m="2304510">half</span> <span m="2304950">of</span> <span m="2305050">the</span>
  <span m="2305140">dimensions</span> <span m="2305860">to</span> <span m="2306040">the</span>
  <span m="2306160">end.</span> <span m="2307480">I'm</span> <span m="2307500">going
  to</span> <span m="2307600">take</span> <span m="2307780">that</span> <span m="2307990">vector</span>
  <span m="2308530">and</span> <span m="2308650">I'll</span> <span m="2308710">penalize</span>
  <span m="2309250">that.</span> <span m="2312640">So</span> <span m="2312990">it's</span>
  <span m="2313240">ignoring</span> <span m="2313630">the</span> <span m="2313720">first</span>
  <span m="2313990">half</span> <span m="2314170">of</span> <span m="2314230">the</span>
  <span m="2314290">dimensions.</span></p><p><span m="2315240">And so</span> <span
  m="2315400">what</span> <span m="2315530">that's</span> <span m="2315640">saying</span>
  <span m="2315940">is,</span> <span m="2316090">well,</span> <span m="2317460">we're</span>
  <span m="2317860">going</span> <span m="2318040">to</span> <span m="2318130">share</span>
  <span m="2318610">parameters</span> <span m="2319390">for</span> <span m="2319630">some</span>
  <span m="2320020">of</span> <span m="2320140">this</span> <span m="2320290">weight</span>
  <span m="2320470">vector.</span> <span m="2320990">But</span> <span m="2321090">we're</span>
  <span m="2321190">not</span> <span m="2321250">going</span> <span m="2321430">to</span>
  <span m="2321550">worry</span> <span m="2321790">about--</span> <span m="2322090">we're</span>
  <span m="2322180">going</span> <span m="2322260">to</span> <span m="2322330">let</span>
  <span m="2322450">them</span> <span m="2322840">be</span> <span m="2322990">completely</span>
  <span m="2323290">dependent</span> <span m="2323590">of</span> <span m="2323650">each</span>
  <span m="2323770">other</span> <span m="2323920">for</span> <span m="2324010">the</span>
  <span m="2324070">rest.</span> <span m="2324580">That's</span> <span m="2324970">an</span>
  <span m="2325060">example of</span> <span m="2325450">what</span> <span m="2325540">you're</span>
  <span m="2325630">suggesting.</span></p><p><span m="2326860">So</span> <span m="2326980">this</span>
  <span m="2327160">is</span> <span m="2327310">all</span> <span m="2327520">great</span>
  <span m="2327790">and</span> <span m="2327880">dandy</span> <span m="2328210">for</span>
  <span m="2328510">the</span> <span m="2328600">case</span> <span m="2328930">of</span>
  <span m="2329050">just</span> <span m="2329290">two</span> <span m="2329500">time</span>
  <span m="2329770">points.</span> <span m="2330130">But</span> <span m="2330390">what</span>
  <span m="2330780">do</span> <span m="2330850">we</span> <span m="2331000">do</span>
  <span m="2331330">if then</span> <span m="2331480">we</span> <span m="2331600">have</span>
  <span m="2331690">five</span> <span m="2332020">time</span> <span m="2332290">points?</span>
  <span m="2337770">Yeah?</span></p><p><span m="2338320">AUDIENCE:</span> <span m="2338485">There's</span>
  <span m="2338650">some</span> <span m="2338850">percentage</span> <span m="2339510">of</span>
  <span m="2339660">shared</span> <span m="2340620">entries</span> <span m="2341010">in</span>
  <span m="2341130">that</span> <span m="2341610">vector.</span> <span m="2342750">So</span>
  <span m="2342960">instead</span> <span m="2343260">of</span> <span m="2343320">saying</span>
  <span m="2343890">these</span> <span m="2344280">have</span> <span m="2344430">to</span>
  <span m="2344520">be in</span> <span m="2344670">common,</span> <span m="2345030">you</span>
  <span m="2345120">say,</span> <span m="2345690">treat</span> <span m="2345990">all</span>
  <span m="2346200">of</span> <span m="2346290">them</span> <span m="2346972">[INAUDIBLE].</span></p><p><span
  m="2352640">DAVID SONTAG:</span> <span m="2352755">I</span> <span m="2352870">think</span>
  <span m="2353080">you</span> <span m="2353140">have</span> <span m="2353230">the</span>
  <span m="2353290">right</span> <span m="2353410">intuition.</span> <span m="2353900">But
  I</span> <span m="2354040">don't</span> <span m="2354310">really</span> <span m="2354580">know</span>
  <span m="2354700">how</span> <span m="2354760">to</span> <span m="2354880">formalize</span>
  <span m="2355600">that</span> <span m="2356320">just</span> <span m="2356530">from</span>
  <span m="2356680">your</span> <span m="2356770">verbal</span> <span m="2357100">description.</span>
  <span m="2359320">What</span> <span m="2359500">would</span> <span m="2359590">be</span>
  <span m="2359680">the</span> <span m="2359770">simplest</span> <span m="2360190">thing</span>
  <span m="2360340">you</span> <span m="2360400">might</span> <span m="2360490">think</span>
  <span m="2360670">of?</span> <span m="2360910">I</span> <span m="2361330">gave</span>
  <span m="2361660">you</span> <span m="2361750">an</span> <span m="2361810">example</span>
  <span m="2362320">of</span> <span m="2362410">how</span> <span m="2362560">to</span>
  <span m="2362680">do,</span> <span m="2363900">in</span> <span m="2364000">some</span>
  <span m="2364180">sense,</span> <span m="2364570">pairwise</span> <span m="2365560">similarity.</span>
  <span m="2366250">Could</span> <span m="2366460">you</span> <span m="2366550">just</span>
  <span m="2366730">easily</span> <span m="2367060">extend</span> <span m="2367420">that</span>
  <span m="2367750">if</span> <span m="2367870">you</span> <span m="2367990">have</span>
  <span m="2368140">more</span> <span m="2368350">than</span> <span m="2368470">two</span>
  <span m="2368650">things?</span> <span m="2369680">You</span> <span m="2369770">have</span>
  <span m="2369910">idea?</span> <span m="2370710">Nope?</span></p><p><span m="2371210">AUDIENCE:</span>
  <span m="2371385">[INAUDIBLE]</span></p><p><span m="2371910">DAVID SONTAG:</span>
  <span m="2371995">Yeah.</span></p><p><span m="2372375">AUDIENCE:</span> <span m="2372522">And</span>
  <span m="2372670">then</span> <span m="2372830">I'd</span> <span m="2373060">get</span>
  <span m="2373390">y1's</span> <span m="2374250">similar</span> <span m="2374570">to
  y2,</span> <span m="2375290">and</span> <span m="2375700">y2</span> <span m="2376110">[INAUDIBLE]</span>
  <span m="2377165">y3.</span> <span m="2377920">And so</span> <span m="2378410">I
  might</span> <span m="2378720">just--</span></p><p><span m="2379460">DAVID SONTAG:</span>
  <span m="2379590">So</span> <span m="2379720">you</span> <span m="2379780">might</span>
  <span m="2379930">say</span> <span m="2380110">w1</span> <span m="2380590">is</span>
  <span m="2380630">similar to</span> <span m="2380930">w2.</span> <span m="2381380">w2</span>
  <span m="2381650">is</span> <span m="2381850">similar to</span> <span m="2382120">w3.</span>
  <span m="2382600">w3</span> <span m="2382810">is</span> <span m="2382990">similar
  to</span> <span m="2383260">w4</span> <span m="2383830">and</span> <span m="2383950">so</span>
  <span m="2384130">on.</span> <span m="2384530">Yeah.</span> <span m="2384730">I</span>
  <span m="2384790">like</span> <span m="2384940">that</span> <span m="2385060">idea.</span></p><p><span
  m="2387390">I'm</span> <span m="2387490">going</span> <span m="2387520">to</span>
  <span m="2387580">generalize</span> <span m="2387980">that</span> <span m="2388090">just</span>
  <span m="2388270">a</span> <span m="2388330">little</span> <span m="2388510">bit.</span>
  <span m="2389470">So</span> <span m="2389620">I'm</span> <span m="2389680">going</span>
  <span m="2389800">to</span> <span m="2389860">start</span> <span m="2390070">thinking</span>
  <span m="2390370">now</span> <span m="2390550">about</span> <span m="2390760">graphs.</span>
  <span m="2392800">And</span> <span m="2394330">we're</span> <span m="2394450">going</span>
  <span m="2394570">to now</span> <span m="2394690">define</span> <span m="2395380">a</span>
  <span m="2395440">very</span> <span m="2395680">simple</span> <span m="2396790">abstraction</span>
  <span m="2397720">to</span> <span m="2397870">talk</span> <span m="2398110">about</span>
  <span m="2398410">multi-task</span> <span m="2399010">learning.</span> <span m="2400300">I'm</span>
  <span m="2400420">going</span> <span m="2400540">to</span> <span m="2400600">have</span>
  <span m="2400840">a</span> <span m="2400930">graph</span> <span m="2401710">where</span>
  <span m="2402250">I</span> <span m="2402400">have</span> <span m="2402880">one</span>
  <span m="2403270">node</span> <span m="2403570">for</span> <span m="2403720">every</span>
  <span m="2403960">task</span> <span m="2404770">and</span> <span m="2404890">an</span>
  <span m="2405070">edge</span> <span m="2405520">between</span> <span m="2406300">tasks,</span>
  <span m="2406990">between</span> <span m="2407320">nodes,</span> <span m="2408190">if</span>
  <span m="2408580">those</span> <span m="2409000">two</span> <span m="2409270">tasks,</span>
  <span m="2410020">we</span> <span m="2410170">want</span> <span m="2410380">to</span>
  <span m="2410530">encourage</span> <span m="2411370">their</span> <span m="2411520">weights</span>
  <span m="2411820">to</span> <span m="2411910">be</span> <span m="2412000">similar</span>
  <span m="2412270">to</span> <span m="2412360">another.</span></p><p><span m="2413710">So</span>
  <span m="2416680">what</span> <span m="2416860">are</span> <span m="2416920">our</span>
  <span m="2417010">tasks</span> <span m="2417520">here?</span> <span m="2417820">W6,</span>
  <span m="2418930">W12.</span> <span m="2420190">So</span> <span m="2420460">in</span>
  <span m="2420540">what you're</span> <span m="2420970">suggesting,</span> <span
  m="2422260">you</span> <span m="2422380">would</span> <span m="2422800">have</span>
  <span m="2423010">the</span> <span m="2423100">following</span> <span m="2423490">graph.</span>
  <span m="2424390">W6</span> <span m="2425800">goes</span> <span m="2426130">to</span>
  <span m="2426430">W12</span> <span m="2428830">goes</span> <span m="2429220">to</span>
  <span m="2429850">W24</span> <span m="2432730">goes</span> <span m="2433000">to</span>
  <span m="2433360">W36</span> <span m="2435910">goes</span> <span m="2436220">to</span>
  <span m="2436380">W48.</span></p><p><span m="2442300">Now,</span> <span m="2442540">the</span>
  <span m="2442630">way</span> <span m="2442750">that</span> <span m="2442840">we're</span>
  <span m="2442930">going</span> <span m="2443010">to</span> <span m="2443110">transform</span>
  <span m="2443680">a</span> <span m="2443740">graph</span> <span m="2444280">into</span>
  <span m="2444490">an</span> <span m="2444550">optimization</span> <span m="2445120">problem</span>
  <span m="2445420">is</span> <span m="2445540">going</span> <span m="2445610">to</span>
  <span m="2445690">be</span> <span m="2445780">as</span> <span m="2445960">follows.</span>
  <span m="2447830">I'm</span> <span m="2447850">going</span> <span m="2447970">to</span>
  <span m="2448270">now</span> <span m="2448510">suppose</span> <span m="2449050">that</span>
  <span m="2449290">I'm</span> <span m="2449350">going</span> <span m="2449470">to</span>
  <span m="2449560">let--</span> <span m="2452020">I'm going to</span> <span m="2452240">define</span>
  <span m="2452620">a</span> <span m="2452680">graph</span> <span m="2454490">on</span>
  <span m="2454710">V comma</span> <span m="2455080">E.</span> <span m="2456700">V,</span>
  <span m="2457180">in</span> <span m="2457270">this</span> <span m="2457450">case,</span>
  <span m="2457870">is going to</span> <span m="2457990">be</span> <span m="2458440">the</span>
  <span m="2458540">set</span> <span m="2459810">6,</span> <span m="2460712">12,</span>
  <span m="2462065">24,</span> <span m="2462970">and</span> <span m="2463120">so</span>
  <span m="2463390">on.</span></p><p><span m="2464590">And</span> <span m="2464740">I'll</span>
  <span m="2464800">denote</span> <span m="2465220">edges</span> <span m="2465760">by</span>
  <span m="2467740">s</span> <span m="2468070">comma</span> <span m="2468550">t.</span>
  <span m="2469510">And</span> <span m="2469760">E</span> <span m="2470200">is</span>
  <span m="2470320">going</span> <span m="2470400">to</span> <span m="2470500">refer</span>
  <span m="2470800">to</span> <span m="2470980">a</span> <span m="2471040">particular</span>
  <span m="2472330">two</span> <span m="2472570">tasks.</span> <span m="2473210">So</span>
  <span m="2473260">for</span> <span m="2473350">example,</span> <span m="2473740">the</span>
  <span m="2473830">task</span> <span m="2474340">of</span> <span m="2474520">six,</span>
  <span m="2474790">predicting</span> <span m="2475160">at</span> <span m="2475200">six</span>
  <span m="2475420">months,</span> <span m="2475600">and</span> <span m="2475720">the</span>
  <span m="2475830">task</span> <span m="2476140">of</span> <span m="2476200">predicting</span>
  <span m="2476530">at</span> <span m="2476620">12</span> <span m="2476890">months.</span></p><p><span
  m="2479080">Then</span> <span m="2479260">what</span> <span m="2479380">we'll</span>
  <span m="2479470">do</span> <span m="2480340">is</span> <span m="2480490">we'll</span>
  <span m="2480610">say</span> <span m="2480760">that</span> <span m="2480880">the</span>
  <span m="2480970">new</span> <span m="2481150">optimization</span> <span m="2481750">problem</span>
  <span m="2482080">is</span> <span m="2482200">going</span> <span m="2482440">to</span>
  <span m="2482590">be</span> <span m="2485500">a</span> <span m="2485590">sum</span>
  <span m="2487090">over</span> <span m="2487780">all of</span> <span m="2488230">the</span>
  <span m="2488380">tasks</span> <span m="2492030">of</span> <span m="2492660">the</span>
  <span m="2493260">loss</span> <span m="2493710">function</span> <span m="2495030">for</span>
  <span m="2495270">that</span> <span m="2495480">task.</span> <span m="2496330">So</span>
  <span m="2496770">I'm</span> <span m="2496830">going</span> <span m="2496940">to</span>
  <span m="2497010">ignore</span> <span m="2497280">what</span> <span m="2497460">is.</span>
  <span m="2497640">I'm</span> <span m="2497700">just</span> <span m="2497820">going</span>
  <span m="2497900">to</span> <span m="2497970">simply</span> <span m="2498200">write--</span>
  <span m="2498810">over</span> <span m="2498990">there,</span> <span m="2499260">I</span>
  <span m="2499350">have</span> <span m="2499530">two</span> <span m="2499740">different</span>
  <span m="2499980">loss</span> <span m="2500160">functions</span> <span m="2500580">for</span>
  <span m="2500670">two</span> <span m="2500820">different</span> <span m="2501030">tasks.</span>
  <span m="2501450">I'm</span> <span m="2501540">just</span> <span m="2501690">going</span>
  <span m="2501750">to</span> <span m="2501810">add</span> <span m="2502230">those</span>
  <span m="2502440">together.</span> <span m="2502830">I'm</span> <span m="2502920">just</span>
  <span m="2503040">going</span> <span m="2503100">to</span> <span m="2503160">leave</span>
  <span m="2503310">that</span> <span m="2503560">in</span> <span m="2503670">this</span>
  <span m="2503820">abstract</span> <span m="2504270">form.</span></p><p><span m="2505640">And</span>
  <span m="2505770">then</span> <span m="2505920">I'm</span> <span m="2506010">going</span>
  <span m="2506250">to</span> <span m="2506340">now</span> <span m="2507120">sum</span>
  <span m="2508080">over</span> <span m="2508980">the</span> <span m="2509250">edges</span>
  <span m="2510090">s</span> <span m="2510360">comma</span> <span m="2510830">t</span>
  <span m="2511350">in</span> <span m="2512330">E</span> <span m="2512820">in</span>
  <span m="2512940">this</span> <span m="2513120">graph</span> <span m="2513600">that</span>
  <span m="2513750">I've</span> <span m="2513840">just</span> <span m="2514020">defined</span>
  <span m="2515640">of</span> <span m="2518130">Ws</span> <span m="2519870">minus</span>
  <span m="2520620">Wt</span> <span m="2522570">squared.</span> <span m="2527150">So</span>
  <span m="2530490">in</span> <span m="2530870">the</span> <span m="2530960">example</span>
  <span m="2531410">that</span> <span m="2531530">I</span> <span m="2531590">go</span>
  <span m="2531680">over</span> <span m="2531890">there</span> <span m="2532310">in</span>
  <span m="2532430">the</span> <span m="2532520">very</span> <span m="2532730">top,</span>
  <span m="2533300">there</span> <span m="2533410">were</span> <span m="2533450">only</span>
  <span m="2533630">two</span> <span m="2533870">tasks,</span> <span m="2534500">W6</span>
  <span m="2535010">and</span> <span m="2535100">W12.</span> <span m="2536480">And
  we</span> <span m="2536570">had</span> <span m="2536690">an</span> <span m="2536750">edge</span>
  <span m="2536960">between</span> <span m="2537290">them.</span> <span m="2537440">And</span>
  <span m="2537530">we</span> <span m="2537650">penalized</span> <span m="2538060">it</span>
  <span m="2538160">exactly</span> <span m="2538550">in</span> <span m="2538610">that</span>
  <span m="2538730">way.</span></p><p><span m="2541130">But</span> <span m="2543410">in</span>
  <span m="2543560">the</span> <span m="2543680">general</span> <span m="2544070">case,</span>
  <span m="2544610">one</span> <span m="2544820">could</span> <span m="2544940">imagine</span>
  <span m="2545900">many</span> <span m="2546200">different</span> <span m="2546440">solutions.</span>
  <span m="2547010">For</span> <span m="2547100">example,</span> <span m="2548150">you</span>
  <span m="2548270">could</span> <span m="2548420">imagine</span> <span m="2548780">a</span>
  <span m="2548840">solution</span> <span m="2549290">where</span> <span m="2549410">you</span>
  <span m="2549530">have</span> <span m="2551000">a</span> <span m="2551090">complete</span>
  <span m="2551510">graph.</span> <span m="2552710">So</span> <span m="2552910">you</span>
  <span m="2552990">may</span> <span m="2553120">have</span> <span m="2553250">four</span>
  <span m="2553520">time</span> <span m="2553790">points.</span> <span m="2554280">And</span>
  <span m="2554300">you</span> <span m="2554390">might</span> <span m="2555290">penalize</span>
  <span m="2556220">every</span> <span m="2557180">pair</span> <span m="2557450">of</span>
  <span m="2557570">them</span> <span m="2557900">to</span> <span m="2558020">be</span>
  <span m="2558140">similar</span> <span m="2558380">to</span> <span m="2558440">one</span>
  <span m="2558560">another.</span> <span m="2560390">Or,</span> <span m="2560930">as</span>
  <span m="2561110">was</span> <span m="2561230">just</span> <span m="2561380">suggested,</span>
  <span m="2561770">you</span> <span m="2561830">might</span> <span m="2561980">think</span>
  <span m="2562160">that</span> <span m="2562250">there</span> <span m="2562340">might</span>
  <span m="2562490">be</span> <span m="2562670">some</span> <span m="2563180">ordering</span>
  <span m="2563810">of</span> <span m="2563960">the</span> <span m="2564050">tasks.</span>
  <span m="2564740">And</span> <span m="2565070">you</span> <span m="2565130">might</span>
  <span m="2565310">say</span> <span m="2565670">that</span> <span m="2566450">you</span>
  <span m="2566600">want</span> <span m="2567110">that--</span> <span m="2568590">instead</span>
  <span m="2568760">of</span> <span m="2568910">a</span> <span m="2569000">complete</span>
  <span m="2569390">graph,</span> <span m="2569900">you're</span> <span m="2570050">going</span>
  <span m="2570260">to</span> <span m="2570380">just</span> <span m="2570620">have</span>
  <span m="2571610">a</span> <span m="2572510">chain</span> <span m="2572840">graph,</span>
  <span m="2573710">where,</span> <span m="2574480">with</span> <span m="2574690">respect</span>
  <span m="2574940">to</span> <span m="2574990">that</span> <span m="2575150">ordering,</span>
  <span m="2575570">you</span> <span m="2575660">want</span> <span m="2575840">every</span>
  <span m="2576050">pair</span> <span m="2576320">of</span> <span m="2576410">them</span>
  <span m="2576530">along</span> <span m="2576740">the</span> <span m="2576830">ordering</span>
  <span m="2577190">to</span> <span m="2577310">be</span> <span m="2577520">close</span>
  <span m="2577850">to</span> <span m="2577910">each</span> <span m="2578060">other.</span></p><p><span
  m="2581240">And</span> <span m="2581690">in</span> <span m="2581750">fact,</span>
  <span m="2582030">I</span> <span m="2582130">think</span> <span m="2582140">that's</span>
  <span m="2582290">probably</span> <span m="2582560">the</span> <span m="2582650">most</span>
  <span m="2582890">reasonable</span> <span m="2583340">thing</span> <span m="2583520">to</span>
  <span m="2583640">do</span> <span m="2583820">in</span> <span m="2583920">a</span>
  <span m="2584000">setting</span> <span m="2584270">of</span> <span m="2584350">disease</span>
  <span m="2584570">progression</span> <span m="2584960">modeling.</span> <span m="2585380">Because,</span>
  <span m="2585890">in</span> <span m="2585980">fact,</span> <span m="2586280">we</span>
  <span m="2586400">have</span> <span m="2586670">some</span> <span m="2586910">smoothness</span>
  <span m="2587570">type</span> <span m="2587750">prior</span> <span m="2588050">in</span>
  <span m="2588140">our</span> <span m="2588260">head</span> <span m="2589280">about</span>
  <span m="2589670">these</span> <span m="2590180">values.</span> <span m="2591240">The</span>
  <span m="2591610">values</span> <span m="2591840">should</span> <span m="2591980">be</span>
  <span m="2592070">similar</span> <span m="2592340">to</span> <span m="2592400">one</span>
  <span m="2592520">another</span> <span m="2594650">when</span> <span m="2594740">they're</span>
  <span m="2594830">very</span> <span m="2595010">close</span> <span m="2595280">time</span>
  <span m="2595520">points.</span></p><p><span m="2598630">I</span> <span m="2598710">just</span>
  <span m="2598830">want</span> <span m="2598950">to</span> <span m="2599010">mention</span>
  <span m="2599250">one</span> <span m="2599430">other</span> <span m="2599610">thing,</span>
  <span m="2600130">which</span> <span m="2600240">is</span> <span m="2600390">that</span>
  <span m="2600570">from</span> <span m="2600780">an</span> <span m="2600870">optimization</span>
  <span m="2601470">perspective,</span> <span m="2602220">if</span> <span m="2602430">this</span>
  <span m="2602640">is</span> <span m="2602760">what</span> <span m="2602910">you</span>
  <span m="2603030">had</span> <span m="2603180">wanted</span> <span m="2603450">to</span>
  <span m="2603600">do,</span> <span m="2603980">there</span> <span m="2604090">is</span>
  <span m="2604200">a</span> <span m="2604260">much</span> <span m="2604440">cleaner</span>
  <span m="2604800">way</span> <span m="2604980">of</span> <span m="2605070">doing</span>
  <span m="2605400">it.</span> <span m="2606690">And</span> <span m="2606810">that's</span>
  <span m="2607020">to</span> <span m="2607830">introduce</span> <span m="2608250">a</span>
  <span m="2608340">dummy</span> <span m="2608730">node.</span> <span m="2609150">I</span>
  <span m="2609240">wish</span> <span m="2609420">I</span> <span m="2609450">had</span>
  <span m="2609570">more</span> <span m="2609690">colors.</span> <span m="2611370">So</span>
  <span m="2614130">one</span> <span m="2614400">could</span> <span m="2614910">instead</span>
  <span m="2615570">introduce</span> <span m="2618336">a</span> <span m="2618750">new</span>
  <span m="2619110">weight</span> <span m="2619350">vector.</span> <span m="2619920">I'll</span>
  <span m="2620010">call</span> <span m="2620280">it</span> <span m="2620680">W.</span>
  <span m="2621590">I'll</span> <span m="2621690">just</span> <span m="2621810">call</span>
  <span m="2621960">it</span> <span m="2622100">W</span> <span m="2624390">with</span>
  <span m="2624600">no</span> <span m="2624780">subscript.</span> <span m="2626640">And</span>
  <span m="2627030">I'm</span> <span m="2627210">going</span> <span m="2627450">to</span>
  <span m="2627570">say</span> <span m="2627960">that</span> <span m="2628260">every</span>
  <span m="2628620">other</span> <span m="2628950">task</span> <span m="2630930">is</span>
  <span m="2631080">going</span> <span m="2631350">to</span> <span m="2631500">be</span>
  <span m="2631680">connected</span> <span m="2632130">to</span> <span m="2632310">it</span>
  <span m="2632550">in</span> <span m="2632680">that</span> <span m="2632860">star.</span></p><p><span
  m="2634420">So</span> <span m="2634530">here</span> <span m="2634740">we've</span>
  <span m="2634890">introduced</span> <span m="2635400">a</span> <span m="2635460">dummy</span>
  <span m="2635820">task.</span> <span m="2637275">And</span> <span m="2637650">we're</span>
  <span m="2637740">connecting</span> <span m="2638100">every</span> <span m="2638280">other</span>
  <span m="2638430">task</span> <span m="2638730">to</span> <span m="2638910">it.</span>
  <span m="2639540">And</span> <span m="2639660">then,</span> <span m="2640260">now</span>
  <span m="2640470">you'd</span> <span m="2640680">have</span> <span m="2641100">a</span>
  <span m="2641160">linear</span> <span m="2641580">number</span> <span m="2642795">of</span>
  <span m="2643200">these</span> <span m="2643380">regularization</span> <span m="2643890">terms</span>
  <span m="2644250">in</span> <span m="2644340">the</span> <span m="2644430">number</span>
  <span m="2644670">of</span> <span m="2644760">tasks.</span> <span m="2645960">But</span>
  <span m="2646110">yet</span> <span m="2646290">you are</span> <span m="2646410">not</span>
  <span m="2646560">making</span> <span m="2646800">any</span> <span m="2646950">assumption</span>
  <span m="2647370">that</span> <span m="2647460">there</span> <span m="2647550">exists</span>
  <span m="2647820">some</span> <span m="2648030">ordering</span> <span m="2649050">between</span>
  <span m="2649350">them</span> <span m="2649440">in</span> <span m="2649500">the</span>
  <span m="2649560">task.</span> <span m="2650060">Yep?</span></p><p><span m="2651000">AUDIENCE:</span>
  <span m="2651195">Do</span> <span m="2651390">you--</span></p><p><span m="2652530">DAVID
  SONTAG:</span> <span m="2652585">And</span> <span m="2653340">W</span> <span m="2653740">is</span>
  <span m="2654140">never</span> <span m="2654440">used</span> <span m="2654800">for</span>
  <span m="2654950">prediction</span> <span m="2655370">ever.</span> <span m="2655760">It's</span>
  <span m="2655970">used</span> <span m="2656210">during</span> <span m="2656450">optimization.</span></p><p><span
  m="2657830">AUDIENCE:</span> <span m="2657956">Why</span> <span m="2658082">do</span>
  <span m="2658210">you</span> <span m="2658310">need</span> <span m="2658610">a</span>
  <span m="2658810">W0</span> <span m="2659180">instead of</span> <span m="2659570">just
  doing it</span> <span m="2659920">based on</span> <span m="2660361">like W1?</span></p><p><span
  m="2662570">DAVID SONTAG:</span> <span m="2662735">Well,</span> <span m="2662900">if</span>
  <span m="2662990">you</span> <span m="2663080">do</span> <span m="2663170">it</span>
  <span m="2663230">based</span> <span m="2663440">on</span> <span m="2663530">W1,</span>
  <span m="2665990">then</span> <span m="2666200">it's</span> <span m="2666290">basically</span>
  <span m="2666590">saying</span> <span m="2666740">that</span> <span m="2666830">W1</span>
  <span m="2667340">is</span> <span m="2667430">special</span> <span m="2667850">in</span>
  <span m="2667970">some</span> <span m="2668150">way.</span> <span m="2668930">And</span>
  <span m="2669080">so</span> <span m="2669170">everything</span> <span m="2669540">sort</span>
  <span m="2669740">of</span> <span m="2669830">pulled</span> <span m="2670130">towards</span>
  <span m="2670640">it,</span> <span m="2671120">whereas</span> <span m="2671510">it's</span>
  <span m="2671630">not</span> <span m="2671870">clear</span> <span m="2672140">that</span>
  <span m="2672290">that's</span> <span m="2672560">actually</span> <span m="2673070">the</span>
  <span m="2673190">right</span> <span m="2673550">thing</span> <span m="2673790">to</span>
  <span m="2673910">do.</span> <span m="2674820">So</span> <span m="2674920">you'll</span>
  <span m="2674930">get</span> <span m="2675050">different</span> <span m="2675290">answers.</span>
  <span m="2676610">And</span> <span m="2676940">I'd</span> <span m="2677060">leave</span>
  <span m="2677240">that</span> <span m="2677360">as</span> <span m="2677420">an</span>
  <span m="2677480">exercise</span> <span m="2677900">for you to</span> <span m="2678020">try</span>
  <span m="2678170">to</span> <span m="2678260">derive.</span></p><p><span m="2681890">So</span>
  <span m="2682490">this</span> <span m="2682670">is</span> <span m="2682760">the</span>
  <span m="2682880">general</span> <span m="2683180">idea</span> <span m="2683720">for</span>
  <span m="2684215">how</span> <span m="2684470">one</span> <span m="2684680">could</span>
  <span m="2684830">do</span> <span m="2684950">multi-task</span> <span m="2685490">learning</span>
  <span m="2686030">using</span> <span m="2686330">linear</span> <span m="2686570">models.</span>
  <span m="2687920">And</span> <span m="2688290">I'll</span> <span m="2688620">also
  leave it</span> <span m="2688710">as an</span> <span m="2688970">exercise</span>
  <span m="2689255">for you</span> <span m="2689540">to</span> <span m="2689630">think</span>
  <span m="2689870">through</span> <span m="2690110">how</span> <span m="2690230">you</span>
  <span m="2690290">could</span> <span m="2690410">take</span> <span m="2690590">the</span>
  <span m="2690680">same</span> <span m="2690950">idea</span> <span m="2691610">and</span>
  <span m="2692090">now</span> <span m="2692360">apply</span> <span m="2692720">it</span>
  <span m="2692900">to,</span> <span m="2693180">for</span> <span m="2693200">example,</span>
  <span m="2693740">deep</span> <span m="2693920">neural</span> <span m="2694040">networks.</span>
  <span m="2695700">And</span> <span m="2696170">you</span> <span m="2696260">can</span>
  <span m="2696410">believe</span> <span m="2696590">me</span> <span m="2696710">that</span>
  <span m="2696830">these</span> <span m="2696950">ideas</span> <span m="2697280">do</span>
  <span m="2697430">generalize</span> <span m="2698260">in</span> <span m="2698630">the</span>
  <span m="2698690">ways</span> <span m="2698870">that</span> <span m="2698960">you
  would</span> <span m="2699050">expect</span> <span m="2699350">them</span> <span
  m="2699500">to</span> <span m="2699590">do.</span></p><p><span m="2701780">And</span>
  <span m="2701990">it's</span> <span m="2702110">a</span> <span m="2702140">very</span>
  <span m="2702410">powerful</span> <span m="2702800">concept.</span> <span m="2703620">And</span>
  <span m="2703820">so</span> <span m="2704420">whenever</span> <span m="2705140">you</span>
  <span m="2705440">are</span> <span m="2705950">tasked</span> <span m="2706340">with--</span>
  <span m="2706900">when you</span> <span m="2707060">tackle</span> <span m="2707330">problems</span>
  <span m="2707630">like</span> <span m="2707780">this,</span> <span m="2709430">and</span>
  <span m="2709700">you're</span> <span m="2709850">in</span> <span m="2709970">settings</span>
  <span m="2711380">where</span> <span m="2711740">a</span> <span m="2711800">linear</span>
  <span m="2712100">model</span> <span m="2712370">might</span> <span m="2712910">do</span>
  <span m="2713150">well,</span> <span m="2716060">before</span> <span m="2716360">you</span>
  <span m="2716510">believe</span> <span m="2718130">that</span> <span m="2718400">someone's</span>
  <span m="2718820">results</span> <span m="2719330">using</span> <span m="2719600">a</span>
  <span m="2719660">very</span> <span m="2719960">complicated</span> <span m="2720680">approach</span>
  <span m="2722990">is</span> <span m="2723680">interesting,</span> <span m="2724460">you</span>
  <span m="2724580">should</span> <span m="2724760">ask,</span> <span m="2725340">well,</span>
  <span m="2725490">what</span> <span m="2725570">about</span> <span m="2725840">the</span>
  <span m="2726320">simplest</span> <span m="2726890">possible</span> <span m="2727250">multi-task</span>
  <span m="2727790">learning</span> <span m="2728150">approach?</span></p><p><span
  m="2731300">So</span> <span m="2732950">we</span> <span m="2733070">already</span>
  <span m="2733280">talked</span> <span m="2733550">about</span> <span m="2733730">one</span>
  <span m="2733970">way</span> <span m="2734150">to</span> <span m="2734270">try</span>
  <span m="2734630">to</span> <span m="2735290">make</span> <span m="2735680">the</span>
  <span m="2735860">regularization</span> <span m="2736550">a</span> <span m="2736610">bit</span>
  <span m="2736790">more</span> <span m="2736940">interesting.</span> <span m="2737540">For</span>
  <span m="2737660">example,</span> <span m="2740510">we</span> <span m="2740600">could</span>
  <span m="2740720">attempt</span> <span m="2740990">to</span> <span m="2741200">regularize</span>
  <span m="2742010">only</span> <span m="2742340">some</span> <span m="2742730">of</span>
  <span m="2742910">the</span> <span m="2743840">features'</span> <span m="2744320">values</span>
  <span m="2744830">to</span> <span m="2744950">be</span> <span m="2745070">similar</span>
  <span m="2745340">to</span> <span m="2745440">another.</span> <span m="2746870">In</span>
  <span m="2747020">this</span> <span m="2747170">paper,</span> <span m="2747750">which</span>
  <span m="2747830">was</span> <span m="2748160">tackling</span> <span m="2748730">this</span>
  <span m="2749060">disease</span> <span m="2749360">progression</span> <span m="2749720">modeling</span>
  <span m="2749990">problem</span> <span m="2750260">for</span> <span m="2750410">Alzheimer's,</span>
  <span m="2752270">they</span> <span m="2752420">developed</span> <span m="2752840">a</span>
  <span m="2752900">slightly</span> <span m="2753410">more</span> <span m="2753650">complicated</span>
  <span m="2754280">approach,</span> <span m="2754790">but</span> <span m="2754970">not</span>
  <span m="2755330">too</span> <span m="2755480">much</span> <span m="2755630">more</span>
  <span m="2755750">complicated,</span> <span m="2757110">which</span> <span m="2757220">they</span>
  <span m="2757340">call</span> <span m="2757640">the</span> <span m="2757790">convex</span>
  <span m="2758470">fused</span> <span m="2758780">sparse</span> <span m="2759290">group</span>
  <span m="2759500">lasso.</span></p><p><span m="2761310">And</span> <span m="2761690">it</span>
  <span m="2761750">does</span> <span m="2761990">the</span> <span m="2762120">same</span>
  <span m="2762650">idea</span> <span m="2762950">that</span> <span m="2763100">I</span>
  <span m="2763250">gave</span> <span m="2763520">here,</span> <span m="2764390">where</span>
  <span m="2765050">you're</span> <span m="2765200">going</span> <span m="2765470">to</span>
  <span m="2765590">now</span> <span m="2765830">learn</span> <span m="2766370">a</span>
  <span m="2766550">matrix</span> <span m="2767250">W.</span> <span m="2767690">And</span>
  <span m="2767810">that</span> <span m="2767930">matrix</span> <span m="2768350">W</span>
  <span m="2769010">is</span> <span m="2769280">precisely</span> <span m="2769970">the</span>
  <span m="2770060">same</span> <span m="2770330">notion.</span> <span m="2770720">You</span>
  <span m="2770810">have</span> <span m="2770960">a</span> <span m="2770990">different</span>
  <span m="2771290">weight</span> <span m="2771560">vector</span> <span m="2771860">per</span>
  <span m="2772010">task.</span> <span m="2772490">You</span> <span m="2772550">just</span>
  <span m="2772700">stack</span> <span m="2773090">them</span> <span m="2773270">all</span>
  <span m="2773450">up</span> <span m="2773630">into</span> <span m="2773870">a</span>
  <span m="2773900">matrix.</span></p><p><span m="2777430">L</span> <span m="2777750">of</span>
  <span m="2777880">W,</span> <span m="2778430">that's</span> <span m="2778700">just</span>
  <span m="2779240">what</span> <span m="2779390">I</span> <span m="2779450">mean</span>
  <span m="2779660">by</span> <span m="2779810">the</span> <span m="2779900">sum</span>
  <span m="2780230">of</span> <span m="2780350">the</span> <span m="2780440">loss</span>
  <span m="2780680">functions.</span> <span m="2781340">That's</span> <span m="2781470">the</span>
  <span m="2781540">same</span> <span m="2781820">thing.</span> <span m="2783710">The</span>
  <span m="2783830">first</span> <span m="2784340">term</span> <span m="2784850">in</span>
  <span m="2785090">the</span> <span m="2785480">optimization</span> <span m="2786080">problem,</span>
  <span m="2786800">lambda</span> <span m="2787100">1</span> <span m="2787370">times</span>
  <span m="2787790">the</span> <span m="2787910">L1</span> <span m="2788360">norm</span>
  <span m="2788660">of</span> <span m="2788780">W,</span> <span m="2789110">is</span>
  <span m="2789170">simply</span> <span m="2789440">saying--</span> <span m="2790250">it's</span>
  <span m="2790370">exactly</span> <span m="2790790">like</span> <span m="2792630">the</span>
  <span m="2792710">sparsity</span> <span m="2793160">penalty</span> <span m="2793460">that</span>
  <span m="2793550">we</span> <span m="2793640">typically</span> <span m="2794000">see</span>
  <span m="2794210">when</span> <span m="2794330">we're</span> <span m="2794450">doing</span>
  <span m="2796150">regression.</span> <span m="2797480">So</span> <span m="2797700">it's</span>
  <span m="2797760">simply</span> <span m="2797960">saying</span> <span m="2798290">that</span>
  <span m="2798440">we're</span> <span m="2798560">going</span> <span m="2798740">to</span>
  <span m="2798830">encourage</span> <span m="2799460">the</span> <span m="2799610">weights</span>
  <span m="2800120">across</span> <span m="2800480">all of</span> <span m="2800810">the</span>
  <span m="2800930">tasks</span> <span m="2801440">to</span> <span m="2801590">be</span>
  <span m="2802020">as</span> <span m="2802280">small</span> <span m="2802610">as</span>
  <span m="2802700">possible.</span> <span m="2803510">And</span> <span m="2803630">because</span>
  <span m="2803900">it's</span> <span m="2804020">an</span> <span m="2804140">L1</span>
  <span m="2804560">penalty,</span> <span m="2805130">it adds</span> <span m="2805370">the</span>
  <span m="2805520">effect</span> <span m="2805940">of</span> <span m="2806030">actually</span>
  <span m="2806330">trying</span> <span m="2806570">to</span> <span m="2806630">encourage</span>
  <span m="2807080">sparsity.</span> <span m="2807230">So</span> <span m="2807590">it's</span>
  <span m="2807680">going</span> <span m="2807800">to</span> <span m="2807860">push</span>
  <span m="2808040">things</span> <span m="2808250">to</span> <span m="2808340">zero</span>
  <span m="2808640">wherever</span> <span m="2808910">possible.</span></p><p><span
  m="2810930">The</span> <span m="2811220">second</span> <span m="2811820">term</span>
  <span m="2812300">in</span> <span m="2812420">this</span> <span m="2812600">optimization</span>
  <span m="2813260">problem,</span> <span m="2815160">this</span> <span m="2816230">lambda</span>
  <span m="2816560">2</span> <span m="2816980">RW</span> <span m="2817610">squared,</span>
  <span m="2824710">is</span> <span m="2825340">also</span> <span m="2825850">a</span>
  <span m="2825910">sparsely</span> <span m="2826500">penalty.</span> <span m="2827320">But</span>
  <span m="2827470">it's</span> <span m="2827590">now</span> <span m="2827830">pre-multiplying</span>
  <span m="2828670">the</span> <span m="2828760">W</span> <span m="2829030">by</span>
  <span m="2829180">this</span> <span m="2829450">R</span> <span m="2829660">matrix.</span>
  <span m="2830890">This</span> <span m="2831070">R</span> <span m="2831250">matrix,</span>
  <span m="2832030">in</span> <span m="2832150">this</span> <span m="2832360">example,</span>
  <span m="2832840">is</span> <span m="2832960">shown</span> <span m="2833230">by</span>
  <span m="2833380">this.</span> <span m="2834586">And</span> <span m="2834980">this</span>
  <span m="2835030">is</span> <span m="2835150">just</span> <span m="2836320">one</span>
  <span m="2836650">way</span> <span m="2836950">to</span> <span m="2837310">implement</span>
  <span m="2837880">precisely</span> <span m="2838450">this</span> <span m="2838660">idea</span>
  <span m="2839290">that</span> <span m="2839410">I</span> <span m="2839500">had</span>
  <span m="2839680">on</span> <span m="2839770">the</span> <span m="2839860">board</span>
  <span m="2840160">here.</span></p><p><span m="2841180">So</span> <span m="2841860">what
  this</span> <span m="2842110">R</span> <span m="2842200">matrix</span> <span m="2842590">is</span>
  <span m="2842680">going</span> <span m="2842780">to</span> <span m="2842860">say</span>
  <span m="2843190">it</span> <span m="2843270">is it's</span> <span m="2843370">going</span>
  <span m="2843490">to</span> <span m="2843550">say</span> <span m="2843700">for--</span>
  <span m="2844690">it's</span> <span m="2844840">going</span> <span m="2844960">to</span>
  <span m="2845020">have</span> <span m="2845590">one--</span> <span m="2848230">you</span>
  <span m="2848320">can</span> <span m="2848440">have</span> <span m="2848530">as</span>
  <span m="2848650">many</span> <span m="2848890">rows</span> <span m="2849280">as</span>
  <span m="2849400">you</span> <span m="2849520">have</span> <span m="2849820">edges.</span>
  <span m="2851150">And</span> <span m="2851170">you're</span> <span m="2851290">going</span>
  <span m="2851470">to</span> <span m="2851560">have--</span> <span m="2851920">for</span>
  <span m="2852280">the</span> <span m="2852550">corresponding</span> <span m="2853300">task</span>
  <span m="2853720">which</span> <span m="2853870">is</span> <span m="2854020">S,</span>
  <span m="2854350">you</span> <span m="2854470">have</span> <span m="2854590">a</span>
  <span m="2854840">1.</span> <span m="2855390">For</span> <span m="2855540">the</span>
  <span m="2855610">corresponding</span> <span m="2856030">task</span> <span m="2856330">which</span>
  <span m="2856480">is</span> <span m="2856600">T,</span> <span m="2856820">you</span>
  <span m="2856930">have</span> <span m="2857070">a</span> <span m="2857110">minus</span>
  <span m="2857500">1.</span></p><p><span m="2858430">And</span> <span m="2858550">then</span>
  <span m="2859120">if</span> <span m="2859240">you</span> <span m="2859360">multiply</span>
  <span m="2860980">this</span> <span m="2861640">R</span> <span m="2861850">matrix</span>
  <span m="2862420">by</span> <span m="2863260">W</span> <span m="2863590">transpose,</span>
  <span m="2865150">what</span> <span m="2865360">you</span> <span m="2865450">get</span>
  <span m="2865840">is</span> <span m="2866050">precisely</span> <span m="2868510">these</span>
  <span m="2868930">types</span> <span m="2869230">of</span> <span m="2869380">pair-wise</span>
  <span m="2869830">comparisons</span> <span m="2870370">out,</span> <span m="2871060">the</span>
  <span m="2871150">only</span> <span m="2871360">difference</span> <span m="2871720">being</span>
  <span m="2871960">that</span> <span m="2872080">here,</span> <span m="2873610">instead</span>
  <span m="2873970">of</span> <span m="2874090">using</span> <span m="2875740">a</span>
  <span m="2876190">L2</span> <span m="2876760">norm,</span> <span m="2877330">they</span>
  <span m="2877460">penalized</span> <span m="2878110">using</span> <span m="2878590">an</span>
  <span m="2878860">L1</span> <span m="2879340">norm.</span> <span m="2881950">So</span>
  <span m="2882070">that's</span> <span m="2882310">what</span> <span m="2882520">that</span>
  <span m="2883060">second</span> <span m="2883420">term</span> <span m="2883780">is,</span>
  <span m="2884020">lambda</span> <span m="2884380">2</span> <span m="2884950">RW</span>
  <span m="2886560">transposed.</span> <span m="2887590">It's</span> <span m="2887710">simply</span>
  <span m="2887980">an</span> <span m="2888040">implementation</span> <span m="2888760">of</span>
  <span m="2888820">precisely</span> <span m="2889300">this</span> <span m="2889510">idea.</span></p><p><span
  m="2891120">And</span> <span m="2891250">that</span> <span m="2891400">final</span>
  <span m="2891760">term</span> <span m="2892570">is</span> <span m="2892990">just</span>
  <span m="2893650">a</span> <span m="2893710">group</span> <span m="2893980">lasso</span>
  <span m="2894250">penalty.</span> <span m="2894580">It's</span> <span m="2895150">nothing</span>
  <span m="2895420">really</span> <span m="2895570">interesting</span> <span m="2895900">happening</span>
  <span m="2896320">there.</span> <span m="2897480">I</span> <span m="2897610">just</span>
  <span m="2897730">want</span> <span m="2897850">to</span> <span m="2897910">comment--</span>
  <span m="2898600">I had</span> <span m="2898750">forgotten</span> <span m="2899050">to</span>
  <span m="2899110">mention</span> <span m="2899380">this.</span> <span m="2900280">The</span>
  <span m="2900430">loss</span> <span m="2900790">term</span> <span m="2901810">is</span>
  <span m="2902230">going</span> <span m="2902470">to</span> <span m="2902590">be</span>
  <span m="2903280">precisely</span> <span m="2904180">a</span> <span m="2904450">squared</span>
  <span m="2905020">loss.</span> <span m="2905530">This</span> <span m="2905860">F</span>
  <span m="2906130">refers</span> <span m="2906520">to</span> <span m="2906640">a</span>
  <span m="2906670">Frobenius</span> <span m="2907390">norm,</span> <span m="2907810">because</span>
  <span m="2910660">we've</span> <span m="2910810">just</span> <span m="2910930">stacked</span>
  <span m="2911230">together</span> <span m="2911620">all</span> <span m="2911750">of</span>
  <span m="2911800">the</span> <span m="2911860">different</span> <span m="2912100">tasks</span>
  <span m="2913270">into</span> <span m="2913540">one.</span></p><p><span m="2914830">And</span>
  <span m="2914980">the</span> <span m="2915130">only</span> <span m="2915460">interesting</span>
  <span m="2915910">thing</span> <span m="2916090">that's</span> <span m="2916240">happening</span>
  <span m="2916630">here</span> <span m="2916990">is</span> <span m="2917170">this</span>
  <span m="2917530">S,</span> <span m="2920230">which</span> <span m="2920380">we're</span>
  <span m="2920500">doing</span> <span m="2920680">an</span> <span m="2920770">element-wise</span>
  <span m="2921880">multiplication.</span> <span m="2923030">What</span> <span m="2923200">that</span>
  <span m="2923350">S</span> <span m="2923670">is</span> <span m="2923830">is</span>
  <span m="2923890">simply</span> <span m="2924190">a</span> <span m="2924250">masking</span>
  <span m="2924640">function.</span> <span m="2925030">It's</span> <span m="2925120">saying,</span>
  <span m="2925540">if</span> <span m="2925720">we</span> <span m="2925840">don't</span>
  <span m="2926170">observe</span> <span m="2927450">a</span> <span m="2927580">value</span>
  <span m="2928030">at</span> <span m="2928100">some</span> <span m="2928330">time</span>
  <span m="2928570">point,</span> <span m="2928870">like,</span> <span m="2929410">for</span>
  <span m="2929500">example,</span> <span m="2930140">if</span> <span m="2930160">either</span>
  <span m="2930520">this</span> <span m="2930700">is</span> <span m="2930820">unknown</span>
  <span m="2931390">or</span> <span m="2931540">censored,</span> <span m="2932530">then</span>
  <span m="2932680">we're</span> <span m="2932800">just</span> <span m="2932980">going</span>
  <span m="2933160">to</span> <span m="2933250">zero</span> <span m="2933730">it</span>
  <span m="2933820">out.</span> <span m="2934180">So</span> <span m="2934930">there</span>
  <span m="2935290">will</span> <span m="2935470">not</span> <span m="2935710">be</span>
  <span m="2935860">any</span> <span m="2936070">loss</span> <span m="2936640">for</span>
  <span m="2936820">that</span> <span m="2937090">particular</span> <span m="2937810">element.</span>
  <span m="2938860">So</span> <span m="2938950">that</span> <span m="2939040">S</span>
  <span m="2939280">is</span> <span m="2939340">just</span> <span m="2939530">the</span>
  <span m="2939640">mask</span> <span m="2940240">which</span> <span m="2940420">allows</span>
  <span m="2940750">you</span> <span m="2940840">to</span> <span m="2941140">account</span>
  <span m="2941470">for</span> <span m="2941560">the</span> <span m="2941650">fact</span>
  <span m="2941830">that</span> <span m="2941920">you</span> <span m="2941980">might</span>
  <span m="2942100">have</span> <span m="2942220">some</span> <span m="2942430">missing</span>
  <span m="2942760">data.</span></p><p><span m="2946540">So</span> <span m="2947130">this</span>
  <span m="2947340">is</span> <span m="2947400">the</span> <span m="2947460">approach</span>
  <span m="2947760">used</span> <span m="2947970">in</span> <span m="2948060">that</span>
  <span m="2948150">KDD</span> <span m="2948510">paper</span> <span m="2948800">from</span>
  <span m="2948870">2012.</span> <span m="2950250">And</span> <span m="2950970">returning</span>
  <span m="2951370">now</span> <span m="2951420">to</span> <span m="2951480">the</span>
  <span m="2951570">Alzheimer's</span> <span m="2952050">example,</span> <span m="2953460">they</span>
  <span m="2953610">used</span> <span m="2953880">a</span> <span m="2954150">pretty</span>
  <span m="2954390">simple</span> <span m="2954720">feature</span> <span m="2954990">set</span>
  <span m="2955320">with</span> <span m="2955790">370</span> <span m="2956490">features.</span>
  <span m="2958110">The</span> <span m="2958230">first</span> <span m="2958500">set</span>
  <span m="2958650">of</span> <span m="2958710">features</span> <span m="2959130">were</span>
  <span m="2959250">derived</span> <span m="2959640">from</span> <span m="2960540">MRI</span>
  <span m="2961050">scans</span> <span m="2961530">of</span> <span m="2961590">the</span>
  <span m="2961680">patient's</span> <span m="2962040">brain.</span> <span m="2963120">In</span>
  <span m="2963210">this</span> <span m="2963390">case,</span> <span m="2963850">they</span>
  <span m="2963930">just</span> <span m="2964650">derived</span> <span m="2965040">some</span>
  <span m="2965940">pre-established</span> <span m="2967020">features</span> <span
  m="2967530">that</span> <span m="2967650">characterize</span> <span m="2969170">the</span>
  <span m="2969250">amount</span> <span m="2969450">of</span> <span m="2969600">white</span>
  <span m="2969900">matter</span> <span m="2971200">and</span> <span m="2971250">so</span>
  <span m="2971460">on.</span> <span m="2972430">That</span> <span m="2972540">includes</span>
  <span m="2972990">some</span> <span m="2973320">genetic</span> <span m="2973650">information,</span>
  <span m="2974640">a</span> <span m="2974700">bunch</span> <span m="2974910">of</span>
  <span m="2975120">cognitive</span> <span m="2975570">scores.</span></p><p><span
  m="2976110">So</span> <span m="2976500">MMSE</span> <span m="2977280">was</span>
  <span m="2977550">one</span> <span m="2977760">example</span> <span m="2978240">of</span>
  <span m="2978330">an</span> <span m="2978510">input</span> <span m="2979020">to</span>
  <span m="2979230">this</span> <span m="2979440">model,</span> <span m="2980820">at</span>
  <span m="2981210">baseline</span> <span m="2981750">is</span> <span m="2981870">critical.</span>
  <span m="2982570">So</span> <span m="2982970">there</span> <span m="2983070">are</span>
  <span m="2983100">a</span> <span m="2983130">number</span> <span m="2983310">of</span>
  <span m="2983400">different</span> <span m="2983730">types</span> <span m="2984060">of</span>
  <span m="2984480">cognitive</span> <span m="2984870">scores</span> <span m="2985290">that</span>
  <span m="2985380">were</span> <span m="2985470">collected</span> <span m="2985860">at</span>
  <span m="2985950">baseline,</span> <span m="2986390">and</span> <span m="2986490">each</span>
  <span m="2986700">one</span> <span m="2986820">of</span> <span m="2986880">those</span>
  <span m="2987090">makes</span> <span m="2987300">up</span> <span m="2987420">some</span>
  <span m="2987600">feature,</span> <span m="2988440">and</span> <span m="2988530">then</span>
  <span m="2988680">a</span> <span m="2988710">number</span> <span m="2989040">of</span>
  <span m="2989160">laboratory</span> <span m="2989740">tests,</span> <span m="2990630">which</span>
  <span m="2990810">I'm</span> <span m="2990900">just</span> <span m="2991080">noting</span>
  <span m="2991410">as</span> <span m="2991500">random</span> <span m="2991740">numbers</span>
  <span m="2992040">here.</span> <span m="2992250">But</span> <span m="2993210">they</span>
  <span m="2993330">have</span> <span m="2993480">some</span> <span m="2993660">significance.</span></p><p><span
  m="2997320">Now,</span> <span m="2998160">one</span> <span m="2998280">of</span>
  <span m="2998340">the</span> <span m="2998400">most</span> <span m="2998550">interesting</span>
  <span m="2998910">things</span> <span m="2999150">about</span> <span m="2999330">the</span>
  <span m="2999390">results</span> <span m="2999900">is</span> <span m="3000020">if</span>
  <span m="3000140">you</span> <span m="3000230">compare</span> <span m="3001220">the</span>
  <span m="3001670">predictive</span> <span m="3002210">performance</span> <span m="3003440">of</span>
  <span m="3004220">the</span> <span m="3004580">multi-task</span> <span m="3005300">approach</span>
  <span m="3005720">to</span> <span m="3006290">the</span> <span m="3007010">independent</span>
  <span m="3007640">regressor</span> <span m="3008180">approach.</span> <span m="3009810">So</span>
  <span m="3009860">here</span> <span m="3010250">we're</span> <span m="3010400">showing</span>
  <span m="3010790">two</span> <span m="3011030">different</span> <span m="3011390">measures</span>
  <span m="3011690">of</span> <span m="3011750">performance.</span> <span m="3012900">The</span>
  <span m="3012920">first</span> <span m="3013130">one</span> <span m="3013310">is</span>
  <span m="3013370">some</span> <span m="3013610">normalized</span> <span m="3014300">mean</span>
  <span m="3014540">squared</span> <span m="3014870">error.</span> <span m="3015260">And</span>
  <span m="3015350">we</span> <span m="3015410">want</span> <span m="3015620">that</span>
  <span m="3015980">to</span> <span m="3016130">be</span> <span m="3016280">as</span>
  <span m="3016460">low</span> <span m="3016730">as</span> <span m="3016880">possible.</span>
  <span m="3017910">And</span> <span m="3018010">the</span> <span m="3018110">second</span>
  <span m="3018240">one</span> <span m="3018590">is</span> <span m="3019400">R,</span>
  <span m="3019820">as</span> <span m="3020000">in</span> <span m="3020120">R</span>
  <span m="3020330">squared.</span> <span m="3021230">And</span> <span m="3021350">you</span>
  <span m="3021410">want</span> <span m="3021590">that</span> <span m="3021740">to</span>
  <span m="3021860">be</span> <span m="3021980">as</span> <span m="3022220">high</span>
  <span m="3022460">as</span> <span m="3022550">possible.</span> <span m="3023160">So</span>
  <span m="3023330">one</span> <span m="3023720">would</span> <span m="3023870">be</span>
  <span m="3023990">perfect</span> <span m="3024470">prediction.</span></p><p><span
  m="3026210">On</span> <span m="3027320">this</span> <span m="3027530">first</span>
  <span m="3027830">column</span> <span m="3028160">here,</span> <span m="3028550">it's</span>
  <span m="3028790">showing</span> <span m="3029210">the</span> <span m="3029330">results</span>
  <span m="3029930">of</span> <span m="3030200">just</span> <span m="3030410">using</span>
  <span m="3030650">independent</span> <span m="3031280">regressors--</span> <span
  m="3031820">so</span> <span m="3032540">if</span> <span m="3032780">instead</span>
  <span m="3033140">of</span> <span m="3033290">tying</span> <span m="3033620">them</span>
  <span m="3033740">together</span> <span m="3034220">with</span> <span m="3034400">that</span>
  <span m="3034560">R</span> <span m="3034760">matrix,</span> <span m="3035210">you</span>
  <span m="3035300">had</span> <span m="3035510">R</span> <span m="3035720">equal</span>
  <span m="3036140">to</span> <span m="3036410">0,</span> <span m="3036710">for</span>
  <span m="3036800">example.</span> <span m="3039500">And</span> <span m="3039650">then</span>
  <span m="3040430">in</span> <span m="3040820">each</span> <span m="3041060">of</span>
  <span m="3041180">the</span> <span m="3041300">subsequent</span> <span m="3041840">columns,</span>
  <span m="3042590">it</span> <span m="3042740">shows</span> <span m="3043580">now</span>
  <span m="3044270">learning</span> <span m="3046271">with</span> <span m="3047120">this</span>
  <span m="3047420">objective</span> <span m="3047870">function,</span> <span m="3050000">where</span>
  <span m="3050780">we</span> <span m="3050960">are</span> <span m="3051050">pumping</span>
  <span m="3051680">up</span> <span m="3051980">increasingly</span> <span m="3052730">high</span>
  <span m="3053630">this</span> <span m="3053930">lambda</span> <span m="3054500">2</span>
  <span m="3054800">coefficient.</span> <span m="3055550">So</span> <span m="3055730">it's</span>
  <span m="3055820">going</span> <span m="3056060">to</span> <span m="3056180">be</span>
  <span m="3057770">asking</span> <span m="3058160">for</span> <span m="3058340">more</span>
  <span m="3058810">and</span> <span m="3058910">more</span> <span m="3059150">similarity</span>
  <span m="3059810">across</span> <span m="3060140">the</span> <span m="3060230">tasks.</span></p><p><span
  m="3062030">So</span> <span m="3062210">you</span> <span m="3062300">see</span>
  <span m="3062450">that</span> <span m="3062600">even</span> <span m="3062870">with</span>
  <span m="3063080">a</span> <span m="3063140">moderate</span> <span m="3063560">value</span>
  <span m="3063890">of</span> <span m="3063980">lambda</span> <span m="3064310">2,</span>
  <span m="3065180">you</span> <span m="3065270">start</span> <span m="3065540">to</span>
  <span m="3065600">get</span> <span m="3065750">improvements</span> <span m="3066410">between</span>
  <span m="3067010">this</span> <span m="3067220">multi-task</span> <span m="3067760">learning</span>
  <span m="3068000">approach</span> <span m="3068510">and</span> <span m="3069020">the</span>
  <span m="3069180">independent</span> <span m="3069750">regressors.</span> <span
  m="3071780">So</span> <span m="3073610">the</span> <span m="3073910">average</span>
  <span m="3074690">R</span> <span m="3074840">squared,</span> <span m="3075140">for</span>
  <span m="3075230">example,</span> <span m="3075590">goes</span> <span m="3075780">from</span>
  <span m="3075920">0.69</span> <span m="3077210">up</span> <span m="3077360">to</span>
  <span m="3077840">0.77.</span> <span m="3079130">And</span> <span m="3079220">you</span>
  <span m="3079310">notice</span> <span m="3079580">how</span> <span m="3079670">we</span>
  <span m="3079790">have</span> <span m="3080240">95%</span> <span m="3080870">confidence</span>
  <span m="3081320">intervals</span> <span m="3081710">here</span> <span m="3081860">as</span>
  <span m="3082040">well.</span> <span m="3082910">And</span> <span m="3083030">it</span>
  <span m="3083100">seems</span> <span m="3083330">to</span> <span m="3083390">be</span>
  <span m="3083480">significant.</span> <span m="3085250">As</span> <span m="3085490">you</span>
  <span m="3085640">pump</span> <span m="3086000">that</span> <span m="3086240">lambda</span>
  <span m="3086570">value</span> <span m="3086900">larger,</span> <span m="3088160">although</span>
  <span m="3088370">I</span> <span m="3088430">won't</span> <span m="3088670">comment</span>
  <span m="3089000">about</span> <span m="3089150">the</span> <span m="3089250">statistical</span>
  <span m="3089630">significance</span> <span m="3090260">between</span> <span m="3090650">these</span>
  <span m="3090800">columns,</span> <span m="3091280">we</span> <span m="3091370">do</span>
  <span m="3091520">see</span> <span m="3091730">a</span> <span m="3091790">trend,</span>
  <span m="3092430">which</span> <span m="3092540">is</span> <span m="3092690">that</span>
  <span m="3093585">performance</span> <span m="3094010">gets</span> <span m="3094190">increasingly</span>
  <span m="3094640">better</span> <span m="3095060">as</span> <span m="3095270">you</span>
  <span m="3095390">encourage</span> <span m="3095810">them</span> <span m="3095990">to</span>
  <span m="3096080">be</span> <span m="3096170">closer</span> <span m="3096510">and</span>
  <span m="3096610">closer</span> <span m="3096800">together.</span></p><p><span m="3102660">So</span>
  <span m="3104810">I</span> <span m="3104870">don't</span> <span m="3104990">think</span>
  <span m="3105170">I</span> <span m="3105200">want</span> <span m="3105320">to</span>
  <span m="3105380">mention</span> <span m="3105680">anything</span> <span m="3106100">else</span>
  <span m="3106340">about</span> <span m="3106700">this</span> <span m="3106940">result.</span>
  <span m="3107255">Is</span> <span m="3107570">there a</span> <span m="3107740">question?</span></p><p><span
  m="3108140">AUDIENCE:</span> <span m="3108225">Is</span> <span m="3108310">this</span>
  <span m="3108830">like a</span> <span m="3109250">holdout</span> <span m="3109520">set?</span></p><p><span
  m="3109910">DAVID SONTAG:</span> <span m="3110105">Ah,</span> <span m="3110300">thank</span>
  <span m="3110570">you.</span> <span m="3110870">Yes.</span> <span m="3111140">So</span>
  <span m="3111290">this</span> <span m="3111470">is</span> <span m="3111590">on</span>
  <span m="3111710">a</span> <span m="3111770">holdout</span> <span m="3112020">set.</span>
  <span m="3112730">Thank</span> <span m="3112940">you.</span> <span m="3113750">And</span>
  <span m="3113840">that</span> <span m="3114040">also</span> <span m="3114200">reminded</span>
  <span m="3114530">me of</span> <span m="3114630">one</span> <span m="3114770">other</span>
  <span m="3114890">thing</span> <span m="3115070">I</span> <span m="3115100">wanted</span>
  <span m="3115250">to</span> <span m="3115310">mention,</span> <span m="3116160">which</span>
  <span m="3116270">is</span> <span m="3116450">critical</span> <span m="3116930">to</span>
  <span m="3117050">this</span> <span m="3117170">story,</span> <span m="3117990">which</span>
  <span m="3118040">is</span> <span m="3118130">that</span> <span m="3118250">you</span>
  <span m="3118370">see</span> <span m="3118580">these</span> <span m="3118670">results</span>
  <span m="3119120">because</span> <span m="3119360">there's</span> <span m="3119510">not</span>
  <span m="3119660">much</span> <span m="3119870">data.</span></p><p><span m="3121340">If</span>
  <span m="3121580">you</span> <span m="3121730">had</span> <span m="3122090">a</span>
  <span m="3122150">really</span> <span m="3122450">large</span> <span m="3122750">training</span>
  <span m="3123050">set,</span> <span m="3123320">you</span> <span m="3123470">would</span>
  <span m="3123590">see</span> <span m="3123800">no</span> <span m="3124010">difference</span>
  <span m="3124370">between</span> <span m="3124700">these</span> <span m="3124820">columns.</span>
  <span m="3125840">Or,</span> <span m="3126050">in</span> <span m="3126110">fact,</span>
  <span m="3126440">if</span> <span m="3126680">you</span> <span m="3126770">had</span>
  <span m="3126860">a</span> <span m="3126920">really</span> <span m="3127220">data</span>
  <span m="3127430">set,</span> <span m="3128180">these</span> <span m="3128450">results</span>
  <span m="3128780">would</span> <span m="3128930">be</span> <span m="3129020">worse.</span>
  <span m="3129470">As</span> <span m="3129620">you</span> <span m="3129710">pump</span>
  <span m="3129920">lambda</span> <span m="3130640">higher,</span> <span m="3131150">the</span>
  <span m="3131270">results</span> <span m="3131570">will</span> <span m="3131660">get</span>
  <span m="3131810">worse.</span> <span m="3132620">Because</span> <span m="3133340">allowing</span>
  <span m="3133730">flexibility</span> <span m="3134690">among</span> <span m="3134960">the</span>
  <span m="3135020">different</span> <span m="3135230">tasks</span> <span m="3135650">is</span>
  <span m="3135860">actually</span> <span m="3136130">a</span> <span m="3136190">better</span>
  <span m="3136490">thing</span> <span m="3136790">if</span> <span m="3136910">you</span>
  <span m="3137000">have</span> <span m="3137120">enough</span> <span m="3137360">data</span>
  <span m="3137570">for</span> <span m="3137690">each</span> <span m="3137840">task.</span>
  <span m="3138930">So</span> <span m="3139010">this</span> <span m="3139250">is</span>
  <span m="3139460">particularly</span> <span m="3140000">valuable</span> <span m="3140420">in</span>
  <span m="3140510">the</span> <span m="3140600">data-poor</span> <span m="3141380">regime.</span></p><p><span
  m="3146620">When it</span> <span m="3146800">goes</span> <span m="3147010">to</span>
  <span m="3147100">try</span> <span m="3147220">to</span> <span m="3147310">analyze</span>
  <span m="3147590">the</span> <span m="3147630">results</span> <span m="3147910">in</span>
  <span m="3147970">terms</span> <span m="3148180">of</span> <span m="3148240">looking</span>
  <span m="3148810">at</span> <span m="3149770">the</span> <span m="3149890">feature</span>
  <span m="3150250">importances</span> <span m="3151210">as</span> <span m="3151360">a</span>
  <span m="3151420">function</span> <span m="3151810">of</span> <span m="3151930">time,</span>
  <span m="3153980">so</span> <span m="3154780">one</span> <span m="3155320">row</span>
  <span m="3155710">here</span> <span m="3156040">corresponds</span> <span m="3156700">to</span>
  <span m="3156940">the</span> <span m="3157090">weight</span> <span m="3157420">vector</span>
  <span m="3157810">for</span> <span m="3158050">that</span> <span m="3158380">time</span>
  <span m="3158680">point's</span> <span m="3159100">predictor.</span> <span m="3160690">And</span>
  <span m="3162070">so</span> <span m="3162520">here</span> <span m="3162830">we're</span>
  <span m="3162930">just</span> <span m="3162970">looking</span> <span m="3163180">at</span>
  <span m="3163270">four</span> <span m="3163540">of</span> <span m="3163630">the</span>
  <span m="3163690">time</span> <span m="3163880">points,</span> <span m="3164110">four
  of</span> <span m="3164330">the</span> <span m="3164410">five</span> <span m="3164680">time</span>
  <span m="3164890">points.</span> <span m="3165880">And</span> <span m="3166480">the</span>
  <span m="3166960">columns</span> <span m="3167560">correspond</span> <span m="3167980">to</span>
  <span m="3168130">different</span> <span m="3168430">features</span> <span m="3168970">that</span>
  <span m="3169090">were</span> <span m="3169180">used</span> <span m="3169540">in</span>
  <span m="3169630">the</span> <span m="3169720">predictions.</span> <span m="3171160">And</span>
  <span m="3171340">the</span> <span m="3171430">colors</span> <span m="3172030">correspond</span>
  <span m="3172630">to</span> <span m="3173260">how</span> <span m="3173560">important</span>
  <span m="3174250">that</span> <span m="3174490">feature</span> <span m="3174910">is</span>
  <span m="3175330">to</span> <span m="3175480">the</span> <span m="3175570">prediction.</span>
  <span m="3176410">You</span> <span m="3176560">could</span> <span m="3176680">imagine</span>
  <span m="3177010">that</span> <span m="3177220">being</span> <span m="3178240">something</span>
  <span m="3178600">like</span> <span m="3179335">the</span> <span m="3179710">norm</span>
  <span m="3180280">of</span> <span m="3180430">the</span> <span m="3180520">corresponding</span>
  <span m="3180970">weight</span> <span m="3181210">in</span> <span m="3181270">the</span>
  <span m="3181360">linear</span> <span m="3181600">model,</span> <span m="3183670">or</span>
  <span m="3183850">a</span> <span m="3183880">normalized</span> <span m="3184360">version</span>
  <span m="3184660">of</span> <span m="3184720">that.</span></p><p><span m="3185650">What</span>
  <span m="3185800">you</span> <span m="3185890">see</span> <span m="3186100">are</span>
  <span m="3186190">some</span> <span m="3186370">interesting</span> <span m="3186700">things.</span>
  <span m="3186970">First,</span> <span m="3187240">there</span> <span m="3187350">are</span>
  <span m="3187420">some</span> <span m="3187870">features,</span> <span m="3189850">such</span>
  <span m="3190060">as</span> <span m="3190210">these,</span> <span m="3191110">where</span>
  <span m="3191500">they're</span> <span m="3191680">important</span> <span m="3192160">at</span>
  <span m="3192280">all</span> <span m="3192460">different</span> <span m="3192760">time</span>
  <span m="3193000">points.</span> <span m="3194290">That</span> <span m="3194440">might</span>
  <span m="3194620">be</span> <span m="3194740">expected.</span> <span m="3195950">But</span>
  <span m="3196090">then</span> <span m="3196360">there</span> <span m="3196510">also</span>
  <span m="3196840">might</span> <span m="3197020">be</span> <span m="3197920">some</span>
  <span m="3198310">features</span> <span m="3198670">that</span> <span m="3198760">are</span>
  <span m="3198850">really</span> <span m="3199060">important</span> <span m="3199450">for</span>
  <span m="3199570">predicting</span> <span m="3199900">what's</span> <span m="3200020">going</span>
  <span m="3200140">to</span> <span m="3200200">happen</span> <span m="3200620">right</span>
  <span m="3200920">away</span> <span m="3201990">but</span> <span m="3202240">are</span>
  <span m="3202300">really</span> <span m="3202600">not</span> <span m="3202810">important</span>
  <span m="3203350">to</span> <span m="3203500">predicting</span> <span m="3204070">longer-term</span>
  <span m="3204700">outcomes.</span> <span m="3205500">And you</span> <span m="3205570">start</span>
  <span m="3205810">to</span> <span m="3205900">see</span> <span m="3206650">things</span>
  <span m="3206890">like</span> <span m="3207070">that</span> <span m="3207250">over</span>
  <span m="3207400">here,</span> <span m="3207790">where</span> <span m="3207940">you</span>
  <span m="3208000">see</span> <span m="3208210">that,</span> <span m="3208510">for</span>
  <span m="3208660">example,</span> <span m="3210580">these</span> <span m="3210850">features</span>
  <span m="3211870">are</span> <span m="3212050">not</span> <span m="3212290">at</span>
  <span m="3212410">all</span> <span m="3212590">important</span> <span m="3213100">for</span>
  <span m="3213280">predicting</span> <span m="3214300">in the</span> <span m="3214390">36th</span>
  <span m="3215590">time</span> <span m="3215890">point</span> <span m="3216550">but</span>
  <span m="3216690">were</span> <span m="3216880">useful</span> <span m="3217360">for</span>
  <span m="3217510">the</span> <span m="3217600">earlier</span> <span m="3217900">time</span>
  <span m="3218170">points.</span></p><p><span m="3224350">So</span> <span m="3224420">from</span>
  <span m="3224570">here,</span> <span m="3224720">now</span> <span m="3224840">we're</span>
  <span m="3224930">going</span> <span m="3225080">to</span> <span m="3225140">start</span>
  <span m="3225350">changing</span> <span m="3225710">gears</span> <span m="3225950">a</span>
  <span m="3225980">little</span> <span m="3226130">bit.</span> <span m="3226370">What</span>
  <span m="3226520">I</span> <span m="3226610">just</span> <span m="3226790">gave</span>
  <span m="3227000">you</span> <span m="3227120">is</span> <span m="3227240">an</span>
  <span m="3227300">example</span> <span m="3228050">of</span> <span m="3228260">a</span>
  <span m="3228350">supervised</span> <span m="3229040">approach.</span> <span m="3229770">Is</span>
  <span m="3229850">there</span> <span m="3229950">a</span> <span m="3230030">question?</span></p><p><span
  m="3230960">AUDIENCE:</span> <span m="3231140">Yes.</span> <span m="3231920">If</span>
  <span m="3232160">a</span> <span m="3232460">faculty</span> <span m="3232710">member</span>
  <span m="3233090">may ask</span> <span m="3233445">this</span> <span m="3233800">question.</span></p><p><span
  m="3235340">DAVID SONTAG:</span> <span m="3235505">Yes.</span> <span m="3236670">I'll</span>
  <span m="3236940">permit it</span> <span m="3237235">today.</span></p><p><span m="3237956">AUDIENCE:</span>
  <span m="3238098">Thank</span> <span m="3238240">you.</span> <span m="3239660">So</span>
  <span m="3240800">it's</span> <span m="3240980">really</span> <span m="3241250">two</span>
  <span m="3241490">questions.</span> <span m="3242190">But</span> <span m="3242920">I</span>
  <span m="3243080">like</span> <span m="3243380">the</span> <span m="3243580">linear</span>
  <span m="3243830">model,</span> <span m="3245050">the</span> <span m="3245290">one</span>
  <span m="3245760">where</span> <span m="3246230">Fred</span> <span m="3246500">suggested,</span>
  <span m="3247350">better</span> <span m="3247740">than</span> <span m="3247820">the</span>
  <span m="3248560">fully</span> <span m="3248920">coupled</span> <span m="3249270">model.</span>
  <span m="3250440">Because</span> <span m="3250950">it</span> <span m="3251070">seems</span>
  <span m="3251550">more</span> <span m="3251890">intuitively</span> <span m="3252820">plausible</span>
  <span m="3253380">to--</span></p><p><span m="3254100">DAVID SONTAG:</span> <span
  m="3254220">And</span> <span m="3254340">indeed,</span> <span m="3254700">it's</span>
  <span m="3254850">the</span> <span m="3254970">linear</span> <span m="3255270">model</span>
  <span m="3255610">which</span> <span m="3255660">is</span> <span m="3255780">used</span>
  <span m="3255990">in</span> <span m="3256050">this</span> <span m="3256200">paper.</span></p><p><span
  m="3256895">AUDIENCE:</span> <span m="3257092">Ah,</span> <span m="3257450">OK.</span></p><p><span
  m="3257980">DAVID SONTAG:</span> <span m="3258070">Yes.</span> <span m="3258360">Because</span>
  <span m="3258570">you</span> <span m="3258660">noticed</span> <span m="3258930">how</span>
  <span m="3259020">that</span> <span m="3259200">R</span> <span m="3260400">was</span>
  <span m="3260730">sort</span> <span m="3260910">of</span> <span m="3260970">diagonal</span>
  <span m="3262480">in--</span></p><p><span m="3263590">AUDIENCE:</span> <span m="3263720">So</span>
  <span m="3263850">it's--</span> <span m="3264120">OK.</span> <span m="3266415">The</span>
  <span m="3266820">other</span> <span m="3267090">observation</span> <span m="3268020">is</span>
  <span m="3268260">that,</span> <span m="3268810">in</span> <span m="3269060">particular</span>
  <span m="3269490">in</span> <span m="3269670">Alzheimer's,</span> <span m="3271120">given</span>
  <span m="3271250">our</span> <span m="3271380">current</span> <span m="3272050">state</span>
  <span m="3273980">of</span> <span m="3274660">inability</span> <span m="3275360">to</span>
  <span m="3275520">treat</span> <span m="3275880">it,</span> <span m="3276345">it</span>
  <span m="3276690">never</span> <span m="3277020">gets</span> <span m="3277290">better.</span>
  <span m="3278360">And</span> <span m="3278920">yet</span> <span m="3279210">that's</span>
  <span m="3279480">not</span> <span m="3280205">constrained</span> <span m="3282025">in</span>
  <span m="3282480">the</span> <span m="3282600">model.</span> <span m="3283420">And</span>
  <span m="3283860">I</span> <span m="3284060">wonder</span> <span m="3284350">if
  it</span> <span m="3284630">would</span> <span m="3284800">help</span> <span m="3285180">to</span>
  <span m="3285410">know</span> <span m="3285760">that.</span></p><p><span m="3286726">DAVID
  SONTAG:</span> <span m="3286968">I</span> <span m="3287210">think</span> <span m="3287300">that's</span>
  <span m="3287390">a</span> <span m="3287450">really</span> <span m="3287600">interesting</span>
  <span m="3287930">point.</span> <span m="3294170">So</span> <span m="3294350">what</span>
  <span m="3294500">Pete's</span> <span m="3294710">suggesting</span> <span m="3294965">is
  that</span> <span m="3295220">you</span> <span m="3295310">could</span> <span m="3295400">think</span>
  <span m="3295580">about</span> <span m="3295820">this</span> <span m="3296210">as--</span>
  <span m="3297530">you could</span> <span m="3297720">think</span> <span m="3297860">about</span>
  <span m="3298070">putting</span> <span m="3298310">an</span> <span m="3298400">additional</span>
  <span m="3298760">constraint</span> <span m="3299360">in,</span> <span m="3302810">which</span>
  <span m="3303080">is</span> <span m="3303350">that</span> <span m="3309299">you
  can</span> <span m="3309790">imagine</span> <span m="3310120">saying</span> <span
  m="3319280">that</span> <span m="3323240">we</span> <span m="3323600">know</span>
  <span m="3324320">that,</span> <span m="3324550">let's</span> <span m="3324740">say,</span>
  <span m="3325900">yi6</span> <span m="3332660">is</span> <span m="3333530">typically</span>
  <span m="3334130">less</span> <span m="3334640">than</span> <span m="3335630">yi12,</span>
  <span m="3337730">which</span> <span m="3337910">is</span> <span m="3338000">typically</span>
  <span m="3338420">less</span> <span m="3338770">than</span> <span m="3339350">yi24</span>
  <span m="3342230">and</span> <span m="3342320">so</span> <span m="3342560">on.</span>
  <span m="3344850">And</span> <span m="3346400">if</span> <span m="3346760">we</span>
  <span m="3346940">were</span> <span m="3347090">able</span> <span m="3347270">to</span>
  <span m="3347420">do</span> <span m="3347510">perfect</span> <span m="3347900">prediction,</span>
  <span m="3348530">meaning</span> <span m="3349070">if</span> <span m="3349310">it</span>
  <span m="3349400">were</span> <span m="3349580">the</span> <span m="3349700">case</span>
  <span m="3350210">that</span> <span m="3352385">your</span> <span m="3352790">predicted</span>
  <span m="3353880">y's</span> <span m="3354530">are</span> <span m="3354740">equal</span>
  <span m="3355100">to</span> <span m="3355250">your</span> <span m="3355430">true</span>
  <span m="3355810">y's,</span> <span m="3356070">then</span> <span m="3356230">you</span>
  <span m="3356330">should</span> <span m="3356510">also</span> <span m="3356900">have</span>
  <span m="3357320">that</span> <span m="3358790">W6</span> <span m="3361961">dot</span>
  <span m="3363230">xi</span> <span m="3365570">is</span> <span m="3365750">less</span>
  <span m="3366110">than</span> <span m="3367260">W12</span> <span m="3369750">dot</span>
  <span m="3370640">xi,</span> <span m="3372120">which</span> <span m="3372410">should</span>
  <span m="3372590">be</span> <span m="3372710">less</span> <span m="3372950">than</span>
  <span m="3374000">W24</span> <span m="3377870">dot</span> <span m="3378680">xi.</span></p><p><span
  m="3382300">And</span> <span m="3382450">so</span> <span m="3382630">one</span>
  <span m="3382810">could</span> <span m="3382960">imagine</span> <span m="3383260">now</span>
  <span m="3383410">introducing</span> <span m="3384130">these</span> <span m="3384490">as</span>
  <span m="3384640">new</span> <span m="3384880">constraints</span> <span m="3385900">in</span>
  <span m="3386050">your</span> <span m="3386170">learning</span> <span m="3386470">problem.</span>
  <span m="3386860">In</span> <span m="3386950">some</span> <span m="3387160">sense,</span>
  <span m="3387490">what</span> <span m="3387640">it's</span> <span m="3387730">saying</span>
  <span m="3388120">is,</span> <span m="3388640">well,</span> <span m="3388840">we</span>
  <span m="3388960">may</span> <span m="3389110">not</span> <span m="3389350">care</span>
  <span m="3390370">that</span> <span m="3390700">much</span> <span m="3391780">if</span>
  <span m="3391930">we</span> <span m="3392080">get</span> <span m="3392290">some</span>
  <span m="3392680">errors</span> <span m="3393400">in</span> <span m="3393700">the</span>
  <span m="3394150">predictions,</span> <span m="3395440">but we</span> <span m="3395590">want</span>
  <span m="3395830">to</span> <span m="3395890">make</span> <span m="3396040">sure</span>
  <span m="3396250">that</span> <span m="3396400">at</span> <span m="3396490">least</span>
  <span m="3396790">we're</span> <span m="3396940">able</span> <span m="3397150">to</span>
  <span m="3397240">sort</span> <span m="3398200">the</span> <span m="3398290">patients</span>
  <span m="3398770">correctly,</span> <span m="3399760">a</span> <span m="3400150">given</span>
  <span m="3400450">patient</span> <span m="3401800">correctly.</span> <span m="3402840">So</span>
  <span m="3402970">we</span> <span m="3403060">want</span> <span m="3403240">to</span>
  <span m="3403360">ensure</span> <span m="3403660">at</span> <span m="3403750">least</span>
  <span m="3403930">some</span> <span m="3404440">monotonicity</span> <span m="3405430">in</span>
  <span m="3405610">these</span> <span m="3405880">values.</span></p><p><span m="3407160">And</span>
  <span m="3407290">one</span> <span m="3407440">could</span> <span m="3407560">easily</span>
  <span m="3407860">try</span> <span m="3408010">to</span> <span m="3408130">translate</span>
  <span m="3408910">these</span> <span m="3409180">types</span> <span m="3409540">of</span>
  <span m="3410050">constraints</span> <span m="3410710">into</span> <span m="3411160">a</span>
  <span m="3411220">modification</span> <span m="3411850">to</span> <span m="3411940">your</span>
  <span m="3412060">learning</span> <span m="3412510">algorithm.</span> <span m="3413410">For</span>
  <span m="3413530">example,</span> <span m="3414080">if</span> <span m="3414100">you</span>
  <span m="3414190">took</span> <span m="3414400">any</span> <span m="3414580">pair</span>
  <span m="3414910">of</span> <span m="3415030">these--</span> <span m="3415540">let's</span>
  <span m="3415750">say,</span> <span m="3416170">I'll</span> <span m="3416260">take</span>
  <span m="3416620">these</span> <span m="3417190">two</span> <span m="3417580">together.</span>
  <span m="3419980">One</span> <span m="3420250">could</span> <span m="3420520">introduce</span>
  <span m="3420940">something</span> <span m="3421270">like</span> <span m="3421450">a</span>
  <span m="3421510">hinge</span> <span m="3421820">loss,</span> <span m="3422600">where</span>
  <span m="3422710">you</span> <span m="3422830">say</span> <span m="3423130">you</span>
  <span m="3423280">want</span> <span m="3423760">that--</span> <span m="3425680">you're</span>
  <span m="3425800">going</span> <span m="3425920">to</span> <span m="3426370">add</span>
  <span m="3426610">a</span> <span m="3426670">new</span> <span m="3426820">objective</span>
  <span m="3427240">function,</span> <span m="3427700">which</span> <span m="3427780">says</span>
  <span m="3428020">something</span> <span m="3428410">like,</span> <span m="3429190">you're</span>
  <span m="3429310">going</span> <span m="3429420">to</span> <span m="3429490">penalize</span>
  <span m="3430360">the</span> <span m="3430540">max</span> <span m="3431950">of</span>
  <span m="3433300">0</span> <span m="3434260">and</span> <span m="3435970">1</span>
  <span m="3436270">minus--</span> <span m="3437230">and</span> <span m="3437320">I'm</span>
  <span m="3437380">going</span> <span m="3437500">to</span> <span m="3437560">screw</span>
  <span m="3437890">up</span> <span m="3438070">this</span> <span m="3438430">order.</span>
  <span m="3438950">But</span> <span m="3438990">it will be</span> <span m="3439090">something</span>
  <span m="3439450">like</span> <span m="3440870">W--</span> <span m="3444160">so</span>
  <span m="3444770">I'll</span> <span m="3445150">derive</span> <span m="3445450">it</span>
  <span m="3445510">correctly.</span></p><p><span m="3446245">So</span> <span m="3446530">this</span>
  <span m="3446680">would</span> <span m="3446770">be</span> <span m="3447490">W12</span>
  <span m="3448630">minus</span> <span m="3449260">W24</span> <span m="3453910">dot</span>
  <span m="3454150">product</span> <span m="3454660">with</span> <span m="3455080">xi,</span>
  <span m="3456060">we</span> <span m="3456200">want</span> <span m="3456490">to</span>
  <span m="3456670">be</span> <span m="3457210">less</span> <span m="3457540">than</span>
  <span m="3458170">0.</span> <span m="3461550">And</span> <span m="3461740">so</span>
  <span m="3461830">you</span> <span m="3461890">could</span> <span m="3462040">look</span>
  <span m="3462220">at</span> <span m="3463010">how</span> <span m="3463360">far</span>
  <span m="3463630">from</span> <span m="3463810">0</span> <span m="3464140">is</span>
  <span m="3464350">it.</span> <span m="3465280">So</span> <span m="3465400">you</span>
  <span m="3465460">could</span> <span m="3465580">look</span> <span m="3465820">at</span>
  <span m="3466405">W12--</span> <span m="3470827">do,</span> <span m="3471270">do,</span>
  <span m="3471595">do.</span> <span m="3473330">You</span> <span m="3473450">might</span>
  <span m="3473600">imagine</span> <span m="3473930">a</span> <span m="3473960">loss</span>
  <span m="3474200">function</span> <span m="3474470">which</span> <span m="3474590">says,</span>
  <span m="3475020">OK,</span> <span m="3477050">if</span> <span m="3477530">it's</span>
  <span m="3477920">greater</span> <span m="3478280">than</span> <span m="3478460">0,</span>
  <span m="3478760">then</span> <span m="3478910">you</span> <span m="3478970">have</span>
  <span m="3479150">problem.</span> <span m="3479810">And</span> <span m="3479930">we</span>
  <span m="3480020">might</span> <span m="3480170">penalize</span> <span m="3480620">it</span>
  <span m="3480800">at,</span> <span m="3481070">let's</span> <span m="3481280">say,</span>
  <span m="3482460">a</span> <span m="3482540">linear</span> <span m="3482900">penalty</span>
  <span m="3483660">however</span> <span m="3483920">greater</span> <span m="3484220">than</span>
  <span m="3484340">0</span> <span m="3484670">it</span> <span m="3484760">is.</span></p><p><span
  m="3485210">And if</span> <span m="3485390">it's</span> <span m="3485570">less</span>
  <span m="3485780">than</span> <span m="3485870">0,</span> <span m="3486210">you</span>
  <span m="3486290">don't</span> <span m="3486440">penalties</span> <span m="3486770">at</span>
  <span m="3486860">all.</span> <span m="3487140">So</span> <span m="3487250">you</span>
  <span m="3487340">say</span> <span m="3487490">something</span> <span m="3487760">like</span>
  <span m="3487940">this,</span> <span m="3488870">max</span> <span m="3489320">of</span>
  <span m="3490670">W12</span> <span m="3491540">minus</span> <span m="3491990">W24</span>
  <span m="3493810">dot</span> <span m="3494150">product</span> <span m="3494510">xi.</span>
  <span m="3495320">And you</span> <span m="3495530">might</span> <span m="3495710">add</span>
  <span m="3495920">something</span> <span m="3496190">like</span> <span m="3496340">this
  to</span> <span m="3496640">your</span> <span m="3496760">learning</span> <span
  m="3497000">objective.</span> <span m="3497740">That</span> <span m="3497900">would</span>
  <span m="3497980">try</span> <span m="3498110">to</span> <span m="3498230">encourage--</span>
  <span m="3499070">that</span> <span m="3499190">would</span> <span m="3499280">penalize</span>
  <span m="3499790">violations</span> <span m="3500390">of</span> <span m="3500480">this</span>
  <span m="3500870">constraint</span> <span m="3502130">using</span> <span m="3502370">a</span>
  <span m="3502430">hinge</span> <span m="3502670">loss-type</span> <span m="3503270">loss</span>
  <span m="3503510">function.</span> <span m="3504710">So</span> <span m="3504800">that</span>
  <span m="3504920">would</span> <span m="3505040">be</span> <span m="3505130">one</span>
  <span m="3505370">approach</span> <span m="3505670">to</span> <span m="3505760">try</span>
  <span m="3505910">to</span> <span m="3506000">put</span> <span m="3506180">such</span>
  <span m="3506960">constraints</span> <span m="3507440">into</span> <span m="3507560">your</span>
  <span m="3507650">learning</span> <span m="3507890">objective.</span></p><p><span
  m="3508970">A</span> <span m="3509060">very</span> <span m="3509240">different</span>
  <span m="3509510">approach</span> <span m="3509810">would</span> <span m="3509900">be</span>
  <span m="3509990">to</span> <span m="3510050">think</span> <span m="3510290">about</span>
  <span m="3510470">it</span> <span m="3511850">as</span> <span m="3512240">a</span>
  <span m="3512360">structured</span> <span m="3512900">prediction</span> <span m="3513290">problem,</span>
  <span m="3514550">where</span> <span m="3515120">instead</span> <span m="3515420">of</span>
  <span m="3515480">trying</span> <span m="3515660">to</span> <span m="3515840">say</span>
  <span m="3516020">that</span> <span m="3516140">you're</span> <span m="3516230">going</span>
  <span m="3516310">to</span> <span m="3516380">be</span> <span m="3516440">predicting</span>
  <span m="3517760">a</span> <span m="3517850">given</span> <span m="3518300">time</span>
  <span m="3518600">point</span> <span m="3518840">by</span> <span m="3518990">itself,</span>
  <span m="3519410">you</span> <span m="3519470">want</span> <span m="3519590">to</span>
  <span m="3519650">predict</span> <span m="3520010">the</span> <span m="3520160">vector</span>
  <span m="3520640">of</span> <span m="3520760">time</span> <span m="3521030">points.</span>
  <span m="3524170">And</span> <span m="3524430">there's a</span> <span m="3524510">whole</span>
  <span m="3524690">field</span> <span m="3525080">of</span> <span m="3525500">what's</span>
  <span m="3525680">called</span> <span m="3525860">structured</span> <span m="3526400">prediction,</span>
  <span m="3527000">which</span> <span m="3527240">would</span> <span m="3527480">allow</span>
  <span m="3527780">one</span> <span m="3528050">to</span> <span m="3528670">formalize</span>
  <span m="3530210">objective</span> <span m="3530630">functions</span> <span m="3531110">that</span>
  <span m="3531260">might</span> <span m="3531500">encourage,</span> <span m="3531980">for</span>
  <span m="3532040">example,</span> <span m="3532400">smoothness</span> <span m="3533210">in</span>
  <span m="3533390">predictions</span> <span m="3534020">across</span> <span m="3534410">time</span>
  <span m="3536930">that</span> <span m="3537240">one</span> <span m="3537530">could</span>
  <span m="3537650">take</span> <span m="3537770">advantage</span> <span m="3538130">of.</span>
  <span m="3538330">But</span> <span m="3538550">I'm</span> <span m="3538610">not</span>
  <span m="3538730">going</span> <span m="3538830">to</span> <span m="3538910">go</span>
  <span m="3539000">more</span> <span m="3539150">into</span> <span m="3539300">that</span>
  <span m="3539420">for</span> <span m="3539540">reasons</span> <span m="3539780">of</span>
  <span m="3539870">time.</span></p><p><span m="3545180">Hold</span> <span m="3545560">any</span>
  <span m="3545710">more</span> <span m="3545860">questions</span> <span m="3546310">to</span>
  <span m="3546400">the end</span> <span m="3546580">of the lecture.</span> <span
  m="3547000">Because I</span> <span m="3547030">want</span> <span m="3547150">to</span>
  <span m="3547210">make</span> <span m="3547330">sure</span> <span m="3547450">I</span>
  <span m="3547540">get</span> <span m="3547720">through</span> <span m="3547840">this</span>
  <span m="3548230">last</span> <span m="3548530">piece.</span></p><p><span m="3552210">So</span>
  <span m="3552390">what</span> <span m="3552510">we've</span> <span m="3552690">talked</span>
  <span m="3552900">about</span> <span m="3553080">so</span> <span m="3553230">far</span>
  <span m="3553770">is</span> <span m="3554130">a</span> <span m="3554310">supervised</span>
  <span m="3555240">learning</span> <span m="3555540">approach</span> <span m="3557520">to</span>
  <span m="3557970">trying</span> <span m="3558450">to</span> <span m="3559650">predict</span>
  <span m="3560070">what's</span> <span m="3560250">going</span> <span m="3560370">to</span>
  <span m="3560460">happen</span> <span m="3560700">to</span> <span m="3560790">a</span>
  <span m="3560820">patient</span> <span m="3561930">given</span> <span m="3562230">what</span>
  <span m="3562350">you</span> <span m="3562470">know</span> <span m="3562620">at</span>
  <span m="3562740">baseline.</span> <span m="3565050">But</span> <span m="3566400">I'm</span>
  <span m="3566520">now</span> <span m="3566670">going</span> <span m="3566790">to</span>
  <span m="3566880">talk</span> <span m="3567090">about</span> <span m="3567720">a</span>
  <span m="3567780">very</span> <span m="3568050">different</span> <span m="3568590">style</span>
  <span m="3568920">of</span> <span m="3569040">thought,</span> <span m="3569370">which</span>
  <span m="3569580">is</span> <span m="3569760">using</span> <span m="3570060">an</span>
  <span m="3570180">unsupervised</span> <span m="3570810">learning</span> <span m="3571020">approach</span>
  <span m="3571320">to</span> <span m="3571410">this.</span> <span m="3571830">And</span>
  <span m="3571940">there are</span> <span m="3572030">going</span> <span m="3572090">to</span>
  <span m="3572170">be</span> <span m="3572250">two</span> <span m="3572700">goals</span>
  <span m="3573300">of</span> <span m="3573420">doing</span> <span m="3573810">unsupervised</span>
  <span m="3574350">learning</span> <span m="3574620">for</span> <span m="3574740">tackling</span>
  <span m="3575130">this</span> <span m="3575220">problem.</span></p><p><span m="3576450">The</span>
  <span m="3576540">first</span> <span m="3576840">goal</span> <span m="3578070">is</span>
  <span m="3578400">that</span> <span m="3578580">of</span> <span m="3578730">discovery,</span>
  <span m="3579480">which</span> <span m="3579630">I</span> <span m="3579690">mentioned</span>
  <span m="3579990">at</span> <span m="3580050">the</span> <span m="3580110">very</span>
  <span m="3580290">beginning</span> <span m="3580710">of</span> <span m="3580800">today's</span>
  <span m="3581010">lecture.</span> <span m="3582110">We</span> <span m="3582220">might</span>
  <span m="3582450">not</span> <span m="3582690">just</span> <span m="3583050">be</span>
  <span m="3583170">interested</span> <span m="3583560">in</span> <span m="3583650">prediction.</span>
  <span m="3584190">We</span> <span m="3584310">might</span> <span m="3584460">also</span>
  <span m="3584700">be</span> <span m="3584790">interested</span> <span m="3585090">in</span>
  <span m="3585180">understanding</span> <span m="3585690">something,</span> <span
  m="3586140">getting</span> <span m="3586410">some</span> <span m="3586530">new</span>
  <span m="3586680">insights</span> <span m="3587250">about</span> <span m="3587490">the</span>
  <span m="3587580">disease,</span> <span m="3588060">like</span> <span m="3588450">discovering</span>
  <span m="3588930">that</span> <span m="3589020">there</span> <span m="3589140">might</span>
  <span m="3589320">be</span> <span m="3589470">some</span> <span m="3589710">subtypes</span>
  <span m="3590340">of</span> <span m="3590430">the</span> <span m="3590520">disease.</span></p><p><span
  m="3592320">And</span> <span m="3592440">those</span> <span m="3592590">subtypes</span>
  <span m="3593160">might</span> <span m="3593310">be</span> <span m="3593370">useful,</span>
  <span m="3593890">for</span> <span m="3593940">example,</span> <span m="3595240">to</span>
  <span m="3595440">help</span> <span m="3595740">design</span> <span m="3596130">new</span>
  <span m="3596280">clinical</span> <span m="3596610">trials.</span> <span m="3597180">Like</span>
  <span m="3597360">maybe</span> <span m="3597750">you</span> <span m="3597900">want</span>
  <span m="3598140">to</span> <span m="3598260">say,</span> <span m="3598560">OK,</span>
  <span m="3600120">we</span> <span m="3600270">conjecture</span> <span m="3600900">that</span>
  <span m="3601050">patients</span> <span m="3601470">in</span> <span m="3601590">this</span>
  <span m="3602100">subtype</span> <span m="3602490">are</span> <span m="3602550">likely</span>
  <span m="3602880">to</span> <span m="3602970">respond</span> <span m="3603390">best</span>
  <span m="3603570">to</span> <span m="3603660">treatment.</span> <span m="3604150">So</span>
  <span m="3604170">we're</span> <span m="3604290">only</span> <span m="3604500">going</span>
  <span m="3604590">to</span> <span m="3604680">run</span> <span m="3604770">the</span>
  <span m="3604830">clinical</span> <span m="3605100">trial</span> <span m="3605270">for</span>
  <span m="3605400">patients</span> <span m="3605730">in</span> <span m="3605820">this</span>
  <span m="3605900">subtype,</span> <span m="3606330">not</span> <span m="3606570">in
  the</span> <span m="3606630">other</span> <span m="3606810">one.</span></p><p><span
  m="3607890">It</span> <span m="3607980">might</span> <span m="3608190">be</span>
  <span m="3608310">useful,</span> <span m="3608940">also,</span> <span m="3609420">to</span>
  <span m="3609570">try</span> <span m="3609900">to</span> <span m="3610800">better</span>
  <span m="3611505">understand</span> <span m="3611970">the</span> <span m="3612040">disease</span>
  <span m="3612300">mechanism.</span> <span m="3612900">So</span> <span m="3613440">if</span>
  <span m="3613590">you</span> <span m="3613680">find</span> <span m="3615630">that</span>
  <span m="3616080">there</span> <span m="3616290">are</span> <span m="3616500">some</span>
  <span m="3616920">people</span> <span m="3617580">who</span> <span m="3617760">seem</span>
  <span m="3618060">to</span> <span m="3618270">progress</span> <span m="3618750">very</span>
  <span m="3619050">quickly</span> <span m="3619530">through</span> <span m="3619650">their</span>
  <span m="3619800">disease</span> <span m="3620220">and</span> <span m="3620310">other</span>
  <span m="3620460">people</span> <span m="3620640">who</span> <span m="3620760">seem</span>
  <span m="3620910">to</span> <span m="3621000">progress</span> <span m="3621380">very</span>
  <span m="3621600">slowly,</span> <span m="3622590">you</span> <span m="3622680">might</span>
  <span m="3622890">then</span> <span m="3623070">go</span> <span m="3623280">back</span>
  <span m="3623730">and</span> <span m="3623850">do</span> <span m="3624030">new</span>
  <span m="3624240">biological</span> <span m="3624870">assays</span> <span m="3625590">on</span>
  <span m="3626100">them</span> <span m="3626700">to</span> <span m="3626760">try</span>
  <span m="3626880">to</span> <span m="3626940">understand</span> <span m="3627210">what</span>
  <span m="3627330">differentiates</span> <span m="3628230">those</span> <span m="3628470">two</span>
  <span m="3628770">clusters.</span> <span m="3629760">So</span> <span m="3629880">the</span>
  <span m="3629970">two</span> <span m="3630210">clusters</span> <span m="3630510">are</span>
  <span m="3630600">differentiated</span> <span m="3631020">in</span> <span m="3631110">terms</span>
  <span m="3631320">of</span> <span m="3631380">their</span> <span m="3632160">phenotype,</span>
  <span m="3632860">but you</span> <span m="3632970">want</span> <span m="3633090">to</span>
  <span m="3633150">go</span> <span m="3633270">back</span> <span m="3633570">and</span>
  <span m="3633660">ask,</span> <span m="3633930">well,</span> <span m="3634020">what</span>
  <span m="3634140">is</span> <span m="3634230">different</span> <span m="3634560">about</span>
  <span m="3634680">their</span> <span m="3634770">genotype</span> <span m="3635310">that</span>
  <span m="3635400">differentiates</span> <span m="3636000">them?</span></p><p><span
  m="3637890">And</span> <span m="3638190">it</span> <span m="3638250">might</span>
  <span m="3638430">also</span> <span m="3638640">be</span> <span m="3638760">useful</span>
  <span m="3639120">to</span> <span m="3639240">have</span> <span m="3639420">a</span>
  <span m="3639480">very</span> <span m="3639690">concise</span> <span m="3640110">description</span>
  <span m="3640680">of</span> <span m="3640770">what</span> <span m="3640920">differentiates</span>
  <span m="3641670">patients</span> <span m="3642510">in</span> <span m="3642630">order</span>
  <span m="3642780">to</span> <span m="3642900">actually</span> <span m="3643260">have</span>
  <span m="3643830">policies</span> <span m="3644460">that</span> <span m="3644580">you</span>
  <span m="3644670">can</span> <span m="3644790">implement.</span> <span m="3645550">So</span>
  <span m="3646350">rather</span> <span m="3646530">than</span> <span m="3646650">having</span>
  <span m="3647400">what</span> <span m="3647580">might</span> <span m="3647760">be</span>
  <span m="3647850">a</span> <span m="3647910">very</span> <span m="3648120">complicated</span>
  <span m="3649260">linear</span> <span m="3649710">model,</span> <span m="3650760">or</span>
  <span m="3650880">even</span> <span m="3651060">non-linear</span> <span m="3651510">model,</span>
  <span m="3651780">for</span> <span m="3651930">predicting</span> <span m="3652770">future</span>
  <span m="3653070">disease</span> <span m="3653310">progression,</span> <span m="3653880">it</span>
  <span m="3654170">would</span> <span m="3654280">be</span> <span m="3654360">much</span>
  <span m="3654600">easier</span> <span m="3654900">if</span> <span m="3654990">you</span>
  <span m="3655070">could</span> <span m="3655130">just</span> <span m="3655260">say,</span>
  <span m="3656590">OK,</span> <span m="3657420">for</span> <span m="3657870">patients</span>
  <span m="3659010">who</span> <span m="3659490">have</span> <span m="3659910">this</span>
  <span m="3660270">biomarker</span> <span m="3660960">abnormal,</span> <span m="3661950">they're</span>
  <span m="3662220">likely</span> <span m="3662640">to</span> <span m="3662730">have</span>
  <span m="3663240">very</span> <span m="3663510">fast</span> <span m="3663840">disease</span>
  <span m="3664080">progression.</span> <span m="3664860">Patients</span> <span m="3665160">who</span>
  <span m="3665230">are</span> <span m="3665290">likely</span> <span m="3665490">have</span>
  <span m="3665610">this</span> <span m="3665790">other</span> <span m="3666030">biomarker</span>
  <span m="3667470">abnormal,</span> <span m="3667920">they're</span> <span m="3668000">likely</span>
  <span m="3668120">to</span> <span m="3668190">have</span> <span m="3668310">a</span>
  <span m="3668370">slow</span> <span m="3668610">disease</span> <span m="3668880">progression.</span></p><p><span
  m="3670080">And</span> <span m="3670470">so</span> <span m="3670560">we'd</span>
  <span m="3670680">like</span> <span m="3670830">to</span> <span m="3670950">be</span>
  <span m="3671040">able</span> <span m="3672225">to</span> <span m="3672660">do</span>
  <span m="3672780">that.</span> <span m="3673350">That's</span> <span m="3673530">what</span>
  <span m="3673620">I</span> <span m="3673650">mean</span> <span m="3673770">by</span>
  <span m="3673890">discovering</span> <span m="3674240">disease</span> <span m="3674430">subtypes.</span>
  <span m="3675150">But</span> <span m="3675300">there's</span> <span m="3675390">actually</span>
  <span m="3675600">a</span> <span m="3675620">second</span> <span m="3676080">goal</span>
  <span m="3676440">as</span> <span m="3676590">well,</span> <span m="3677310">which--</span>
  <span m="3677480">remember,</span> <span m="3678180">think</span> <span m="3678450">back</span>
  <span m="3678780">to</span> <span m="3678900">that</span> <span m="3679050">original</span>
  <span m="3680700">motivation</span> <span m="3681300">I</span> <span m="3681360">mentioned</span>
  <span m="3681720">earlier</span> <span m="3682110">of</span> <span m="3682290">having</span>
  <span m="3682620">very</span> <span m="3682980">little</span> <span m="3683250">data.</span></p><p><span
  m="3684240">If you</span> <span m="3684360">have</span> <span m="3684570">very</span>
  <span m="3684870">little</span> <span m="3685170">data,</span> <span m="3685680">which</span>
  <span m="3685890">is</span> <span m="3686040">unfortunately</span> <span m="3686610">the</span>
  <span m="3686720">setting</span> <span m="3687000">that</span> <span m="3687120">we're</span>
  <span m="3687210">almost</span> <span m="3687540">always</span> <span m="3687960">in</span>
  <span m="3688080">when</span> <span m="3688200">doing</span> <span m="3688350">machine</span>
  <span m="3688590">learning</span> <span m="3688770">in</span> <span m="3688860">health</span>
  <span m="3689070">care,</span> <span m="3690250">then</span> <span m="3690420">you</span>
  <span m="3690510">can</span> <span m="3690660">overfit</span> <span m="3691230">really</span>
  <span m="3691560">easily</span> <span m="3692190">to</span> <span m="3692970">your</span>
  <span m="3693180">data</span> <span m="3693630">when</span> <span m="3694110">just</span>
  <span m="3694440">using</span> <span m="3694770">it</span> <span m="3694950">strictly</span>
  <span m="3695550">within</span> <span m="3695790">a</span> <span m="3695910">discriminative</span>
  <span m="3696690">learning</span> <span m="3697020">framework.</span></p><p><span
  m="3699100">And</span> <span m="3699200">so</span> <span m="3699300">if</span> <span
  m="3699420">one</span> <span m="3699660">were</span> <span m="3699750">to</span>
  <span m="3699870">now</span> <span m="3700020">change</span> <span m="3700440">your</span>
  <span m="3700620">optimization</span> <span m="3701340">problem</span> <span m="3701640">altogether</span>
  <span m="3702210">to</span> <span m="3702330">start</span> <span m="3702570">to</span>
  <span m="3702660">bring</span> <span m="3703020">in</span> <span m="3703140">an</span>
  <span m="3703380">unsupervised</span> <span m="3704250">loss</span> <span m="3704580">function,</span>
  <span m="3706080">then</span> <span m="3706500">one</span> <span m="3706800">can</span>
  <span m="3706980">hope</span> <span m="3707280">to</span> <span m="3707970">get</span>
  <span m="3708240">much</span> <span m="3708600">more</span> <span m="3708960">out</span>
  <span m="3709170">of</span> <span m="3709260">the</span> <span m="3709320">limited</span>
  <span m="3709620">data</span> <span m="3709800">you</span> <span m="3709920">have</span>
  <span m="3710370">and</span> <span m="3710520">save</span> <span m="3710940">the</span>
  <span m="3711060">labels,</span> <span m="3711630">which</span> <span m="3711810">you</span>
  <span m="3711900">might</span> <span m="3712080">overfit</span> <span m="3712530">on</span>
  <span m="3712680">very</span> <span m="3712860">easily,</span> <span m="3713280">for</span>
  <span m="3713490">the</span> <span m="3713580">very</span> <span m="3713880">last</span>
  <span m="3714180">step</span> <span m="3714420">of</span> <span m="3714540">your</span>
  <span m="3714630">learning</span> <span m="3714900">algorithm.</span> <span m="3715920">And</span>
  <span m="3716010">that's</span> <span m="3716160">exactly</span> <span m="3716520">what</span>
  <span m="3716640">we'll</span> <span m="3716760">do</span> <span m="3717000">in</span>
  <span m="3717300">this</span> <span m="3717450">segment</span> <span m="3717840">of</span>
  <span m="3717900">the</span> <span m="3717990">lecture.</span></p><p><span m="3720010">So</span>
  <span m="3720570">for</span> <span m="3720720">today,</span> <span m="3721090">we're</span>
  <span m="3721190">going</span> <span m="3721260">to</span> <span m="3721320">think</span>
  <span m="3721500">about</span> <span m="3721650">the</span> <span m="3721740">simplest</span>
  <span m="3722280">possible</span> <span m="3722670">unsupervised</span> <span m="3723180">learning</span>
  <span m="3723480">algorithm.</span> <span m="3724700">And</span> <span m="3724800">because</span>
  <span m="3726180">the</span> <span m="3726330">official</span> <span m="3726690">prerequisite</span>
  <span m="3727140">for</span> <span m="3727260">this</span> <span m="3727410">course</span>
  <span m="3727680">was</span> <span m="3727800">6036,</span> <span m="3729060">and</span>
  <span m="3729150">because</span> <span m="3729960">clustering</span> <span m="3730470">was</span>
  <span m="3730620">not</span> <span m="3730770">discussed</span> <span m="3731190">in</span>
  <span m="3731310">6036,</span> <span m="3732180">I'll</span> <span m="3732270">spend</span>
  <span m="3732480">just</span> <span m="3732660">two</span> <span m="3732870">minutes</span>
  <span m="3734130">talking</span> <span m="3734430">about</span> <span m="3734550">clustering</span>
  <span m="3735390">using</span> <span m="3735630">the</span> <span m="3735690">simplest</span>
  <span m="3736080">algorithm</span> <span m="3736380">called</span> <span m="3736620">K-means,</span>
  <span m="3737070">which</span> <span m="3737250">I</span> <span m="3737310">hope</span>
  <span m="3737640">almost</span> <span m="3737940">all</span> <span m="3738120">of</span>
  <span m="3738210">you</span> <span m="3738300">know.</span> <span m="3738880">But</span>
  <span m="3739050">this</span> <span m="3739170">will</span> <span m="3739260">just</span>
  <span m="3739440">be</span> <span m="3739580">a</span> <span m="3739620">simple</span>
  <span m="3739890">reminder.</span></p><p><span m="3742530">How</span> <span m="3742650">many</span>
  <span m="3742830">clusters</span> <span m="3743370">are</span> <span m="3743490">there</span>
  <span m="3744020">in</span> <span m="3745400">in this</span> <span m="3745770">figure</span>
  <span m="3746010">that</span> <span m="3746130">I'm</span> <span m="3746220">showing</span>
  <span m="3746400">over</span> <span m="3746550">here?</span> <span m="3749060">Let's</span>
  <span m="3749280">raise</span> <span m="3749440">some</span> <span m="3749610">hands.</span>
  <span m="3750270">One</span> <span m="3750510">cluster?</span> <span m="3751380">Two</span>
  <span m="3751560">clusters?</span> <span m="3752600">Three</span> <span m="3752760">clusters?</span>
  <span m="3753660">Four</span> <span m="3753870">clusters?</span> <span m="3754920">Five</span>
  <span m="3755190">clusters?</span> <span m="3756240">OK.</span></p><p><span m="3758280">And</span>
  <span m="3758760">are</span> <span m="3759570">these</span> <span m="3759780">red</span>
  <span m="3759960">points</span> <span m="3760320">more</span> <span m="3760500">or</span>
  <span m="3760530">less</span> <span m="3760710">showing</span> <span m="3761010">where</span>
  <span m="3761130">those</span> <span m="3761280">five</span> <span m="3761460">clusters</span>
  <span m="3761790">are?</span> <span m="3762700">No.</span> <span m="3763466">No,</span>
  <span m="3763812">they're not.</span> <span m="3764160">So</span> <span m="3764220">rather</span>
  <span m="3764880">there's</span> <span m="3765030">a</span> <span m="3765090">cluster</span>
  <span m="3765360">here.</span> <span m="3765600">There's a</span> <span m="3765750">cluster</span>
  <span m="3765990">here,</span> <span m="3766350">there,</span> <span m="3766590">there,</span>
  <span m="3766790">there.</span></p><p><span m="3768280">All right.</span> <span
  m="3768450">So</span> <span m="3768570">you</span> <span m="3768930">were</span>
  <span m="3769590">you</span> <span m="3769710">are</span> <span m="3769800">able</span>
  <span m="3769950">to</span> <span m="3770040">do</span> <span m="3770100">this</span>
  <span m="3770250">really</span> <span m="3770430">well,</span> <span m="3771150">as</span>
  <span m="3771300">humans,</span> <span m="3771930">looking</span> <span m="3772200">at</span>
  <span m="3772290">two</span> <span m="3772440">dimensional</span> <span m="3772890">data.</span>
  <span m="3774030">The</span> <span m="3774090">goal</span> <span m="3774390">of</span>
  <span m="3774780">algorithms</span> <span m="3775170">like</span> <span m="3775300">K-means</span>
  <span m="3775830">is</span> <span m="3775950">to</span> <span m="3776100">show</span>
  <span m="3776340">how</span> <span m="3776460">one</span> <span m="3776640">could</span>
  <span m="3776790">do</span> <span m="3776880">that</span> <span m="3777840">automatically</span>
  <span m="3778680">for</span> <span m="3778860">high-dimensional</span> <span m="3779550">data.</span>
  <span m="3780390">And the</span> <span m="3780610">K-means</span> <span m="3781020">algorithm</span>
  <span m="3781350">is</span> <span m="3781440">very</span> <span m="3781620">simple.</span>
  <span m="3781950">It works</span> <span m="3782160">as</span> <span m="3782280">follows.</span></p><p><span
  m="3782700">You</span> <span m="3782850">hypothesize</span> <span m="3783420">a</span>
  <span m="3783450">number</span> <span m="3783640">of</span> <span m="3783690">clusters.</span>
  <span m="3784330">So</span> <span m="3784440">here</span> <span m="3784650">we</span>
  <span m="3784740">have</span> <span m="3784800">hypothesized</span> <span m="3785400">five</span>
  <span m="3785700">clusters.</span> <span m="3786810">You're</span> <span m="3786900">going</span>
  <span m="3787110">to</span> <span m="3787380">randomly</span> <span m="3788010">initialize</span>
  <span m="3788550">those</span> <span m="3788730">cluster</span> <span m="3789030">centers,</span>
  <span m="3789450">which</span> <span m="3789570">I'm</span> <span m="3789700">denoting</span>
  <span m="3790080">by</span> <span m="3790230">those</span> <span m="3790410">red</span>
  <span m="3790650">points</span> <span m="3791010">shown</span> <span m="3791280">here.</span>
  <span m="3792510">Then</span> <span m="3792660">in</span> <span m="3792750">the</span>
  <span m="3792810">first</span> <span m="3793110">stage</span> <span m="3793380">of</span>
  <span m="3793440">the</span> <span m="3793530">K-means</span> <span m="3793890">algorithm,</span>
  <span m="3794670">you're</span> <span m="3794790">going</span> <span m="3794970">to</span>
  <span m="3795060">assign</span> <span m="3795690">every</span> <span m="3795930">data</span>
  <span m="3796200">point</span> <span m="3796560">to</span> <span m="3796650">the</span>
  <span m="3796740">closest</span> <span m="3797250">cluster</span> <span m="3797640">center.</span></p><p><span
  m="3798540">And</span> <span m="3798630">that's</span> <span m="3798810">going</span>
  <span m="3799050">to</span> <span m="3799170">induce</span> <span m="3799830">a</span>
  <span m="3800100">Voronoi</span> <span m="3800670">diagram</span> <span m="3803040">where</span>
  <span m="3803460">every</span> <span m="3803850">point</span> <span m="3804240">within</span>
  <span m="3804720">this</span> <span m="3805230">Voronoi</span> <span m="3805770">cell</span>
  <span m="3806250">is</span> <span m="3806460">closer</span> <span m="3807120">to</span>
  <span m="3807360">this</span> <span m="3807630">red</span> <span m="3807810">point</span>
  <span m="3808170">than</span> <span m="3808380">to</span> <span m="3808500">any</span>
  <span m="3808710">other</span> <span m="3809090">red</span> <span m="3809280">point.</span>
  <span m="3810570">And</span> <span m="3810660">so</span> <span m="3810780">every</span>
  <span m="3811170">data</span> <span m="3811500">point</span> <span m="3811800">in</span>
  <span m="3811980">this</span> <span m="3812160">Voronoi</span> <span m="3812490">cell</span>
  <span m="3812790">will</span> <span m="3812940">then</span> <span m="3813150">be</span>
  <span m="3813270">assigned</span> <span m="3814140">to</span> <span m="3814260">this</span>
  <span m="3814440">data</span> <span m="3814650">point.</span> <span m="3815220">Every</span>
  <span m="3815460">data</span> <span m="3815640">point</span> <span m="3815990">in</span>
  <span m="3816090">this</span> <span m="3816330">Voronoi</span> <span m="3816630">cell</span>
  <span m="3816880">will</span> <span m="3816990">be</span> <span m="3817110">assigned</span>
  <span m="3817410">to</span> <span m="3817500">that</span> <span m="3817740">data</span>
  <span m="3818010">point</span> <span m="3818380">and</span> <span m="3818400">so</span>
  <span m="3818640">on.</span></p><p><span m="3819880">So</span> <span m="3819960">we're</span>
  <span m="3820050">going</span> <span m="3820120">to</span> <span m="3820200">now</span>
  <span m="3820590">assign</span> <span m="3821250">all</span> <span m="3821430">data</span>
  <span m="3821700">points</span> <span m="3822000">to</span> <span m="3822120">the</span>
  <span m="3822240">closest</span> <span m="3822630">cluster</span> <span m="3822960">center.</span>
  <span m="3823770">And</span> <span m="3823860">then</span> <span m="3823980">we're</span>
  <span m="3824100">just</span> <span m="3824250">going</span> <span m="3824460">to</span>
  <span m="3824790">average</span> <span m="3825510">all</span> <span m="3825660">the</span>
  <span m="3825750">data</span> <span m="3825960">points</span> <span m="3826200">assigned</span>
  <span m="3826440">to</span> <span m="3826500">some</span> <span m="3826650">cluster</span>
  <span m="3826950">center</span> <span m="3827310">to</span> <span m="3827460">get</span>
  <span m="3827610">the</span> <span m="3827700">new</span> <span m="3828030">cluster</span>
  <span m="3828360">center.</span> <span m="3829200">And</span> <span m="3829320">you</span>
  <span m="3829380">repeat.</span> <span m="3830890">And</span> <span m="3831000">you're</span>
  <span m="3831090">going</span> <span m="3831200">to</span> <span m="3831270">stop</span>
  <span m="3831540">this</span> <span m="3831710">procedure</span> <span m="3832080">when</span>
  <span m="3832710">no</span> <span m="3832950">point</span> <span m="3833220">in</span>
  <span m="3833280">time</span> <span m="3833460">is</span> <span m="3833550">changed.</span></p><p><span
  m="3834420">So let's</span> <span m="3834570">look</span> <span m="3834720">at</span>
  <span m="3834780">a</span> <span m="3834810">simple</span> <span m="3835050">example.</span>
  <span m="3836040">Here</span> <span m="3836250">we're</span> <span m="3836340">using</span>
  <span m="3836640">K</span> <span m="3836970">equals</span> <span m="3837150">2.</span>
  <span m="3837460">We</span> <span m="3837650">just</span> <span m="3838080">decided</span>
  <span m="3838650">there</span> <span m="3838770">are</span> <span m="3838800">only</span>
  <span m="3839040">two</span> <span m="3839220">clusters.</span> <span m="3840210">We've</span>
  <span m="3840390">initialized</span> <span m="3841080">the</span> <span m="3841200">two</span>
  <span m="3841320">clusters</span> <span m="3841710">shown</span> <span m="3841980">here,</span>
  <span m="3842700">the</span> <span m="3842820">two</span> <span m="3842970">cluster</span>
  <span m="3843240">centers,</span> <span m="3843600">as</span> <span m="3844200">this</span>
  <span m="3844380">red</span> <span m="3844620">cluster</span> <span m="3844920">center</span>
  <span m="3845140">and</span> <span m="3845220">this</span> <span m="3845370">blue</span>
  <span m="3845520">cluster</span> <span m="3845820">center.</span> <span m="3846480">Notice</span>
  <span m="3846810">that</span> <span m="3846960">they're</span> <span m="3847110">nowhere</span>
  <span m="3847560">near</span> <span m="3847860">the</span> <span m="3847980">data.</span>
  <span m="3848640">We've</span> <span m="3848780">just</span> <span m="3849120">randomly</span>
  <span m="3849570">chosen.</span> <span m="3850050">They're</span> <span m="3850090">nowhere</span>
  <span m="3850360">near</span> <span m="3850540">the</span> <span m="3850610">data.</span>
  <span m="3850840">It's</span> <span m="3850930">actually</span> <span m="3851170">pretty</span>
  <span m="3851350">bad</span> <span m="3851530">initialization.</span></p><p><span
  m="3852700">The</span> <span m="3852790">first</span> <span m="3853060">step</span>
  <span m="3853270">is</span> <span m="3853390">going</span> <span m="3853540">to</span>
  <span m="3853630">assign</span> <span m="3854170">data</span> <span m="3854440">points</span>
  <span m="3856120">to</span> <span m="3856510">their</span> <span m="3856690">closest</span>
  <span m="3857560">cluster</span> <span m="3857920">center.</span> <span m="3859030">So</span>
  <span m="3859230">I want</span> <span m="3859380">everyone</span> <span m="3859470">to</span>
  <span m="3859720">say</span> <span m="3859930">out</span> <span m="3860080">loud</span>
  <span m="3860500">either</span> <span m="3860800">red</span> <span m="3861070">or</span>
  <span m="3861250">green,</span> <span m="3862060">to</span> <span m="3862360">which</span>
  <span m="3862540">cluster</span> <span m="3862840">center</span> <span m="3863080">it's</span>
  <span m="3863200">going</span> <span m="3863380">to</span> <span m="3863470">point</span>
  <span m="3863770">to,</span> <span m="3864400">what</span> <span m="3864550">it
  is</span> <span m="3864700">going</span> <span m="3864880">to</span> <span m="3864940">be</span>
  <span m="3865000">assigned</span> <span m="3865300">to</span> <span m="3865480">this</span>
  <span m="3865600">step.</span></p><p><span m="3867438">[INTERPOSING VOICES]</span></p><p><span
  m="3869918">AUDIENCE:</span> <span m="3870166">Red.</span> <span m="3871406">Blue.</span>
  <span m="3872720">Blue.</span></p><p><span m="3873086">DAVID SONTAG:</span> <span
  m="3873208">All</span> <span m="3873330">right.</span> <span m="3873452">Good.</span>
  <span m="3873820">We</span> <span m="3873910">get</span> <span m="3874000">it.</span></p><p><span
  m="3876930">So</span> <span m="3877120">that's</span> <span m="3877330">the</span>
  <span m="3877420">first</span> <span m="3877690">assignment.</span> <span m="3879160">Now</span>
  <span m="3879460">we're</span> <span m="3879550">going</span> <span m="3879730">to</span>
  <span m="3879970">average</span> <span m="3880640">the</span> <span m="3880690">data</span>
  <span m="3880930">points</span> <span m="3881380">that</span> <span m="3881740">are</span>
  <span m="3882730">assigned</span> <span m="3883360">to</span> <span m="3883480">that</span>
  <span m="3883630">red</span> <span m="3884200">cluster</span> <span m="3884500">center.</span>
  <span m="3884860">So</span> <span m="3885010">we're</span> <span m="3885100">going</span>
  <span m="3885220">to</span> <span m="3885310">average</span> <span m="3885820">all</span>
  <span m="3885880">the</span> <span m="3885970">red</span> <span m="3886150">points.</span>
  <span m="3888100">And</span> <span m="3888280">the</span> <span m="3888370">new</span>
  <span m="3888850">red</span> <span m="3889180">cluster</span> <span m="3889480">center</span>
  <span m="3889780">will</span> <span m="3889930">be</span> <span m="3890770">over</span>
  <span m="3890950">here,</span> <span m="3891070">right?</span></p><p><span m="3892146">AUDIENCE:</span>
  <span m="3892360">No.</span></p><p><span m="3893002">DAVID SONTAG:</span> <span
  m="3893216">Oh,</span> <span m="3893430">over</span> <span m="3893860">there?</span>
  <span m="3895750">Over</span> <span m="3895860">here?</span></p><p><span m="3896010">AUDIENCE:</span>
  <span m="3896226">Yes.</span></p><p><span m="3896876">DAVID SONTAG:</span> <span
  m="3897020">OK.</span> <span m="3897164">Good.</span> <span m="3897310">And</span>
  <span m="3897430">the</span> <span m="3897520">blue</span> <span m="3897970">cluster</span>
  <span m="3898270">center</span> <span m="3898780">will</span> <span m="3898990">be</span>
  <span m="3899140">somewhere</span> <span m="3899440">over</span> <span m="3899590">here,</span>
  <span m="3900000">right?</span></p><p><span m="3900140">AUDIENCE:</span> <span m="3900342">Yes.</span></p><p><span
  m="3900950">DAVID SONTAG:</span> <span m="3901045">OK.</span> <span m="3901540">Good.</span>
  <span m="3901970">So</span> <span m="3902070">that's</span> <span m="3902170">the</span>
  <span m="3902260">next</span> <span m="3902500">step.</span> <span m="3905280">And</span>
  <span m="3905680">then</span> <span m="3905800">you</span> <span m="3905890">repeat.</span>
  <span m="3906830">So</span> <span m="3906880">now,</span> <span m="3907150">again,</span>
  <span m="3907410">you</span> <span m="3907510">assign</span> <span m="3907780">every</span>
  <span m="3907960">data</span> <span m="3908110">point</span> <span m="3908290">to</span>
  <span m="3908410">its</span> <span m="3908530">closest</span> <span m="3908800">cluster</span>
  <span m="3909130">center.</span> <span m="3909790">By</span> <span m="3909970">the</span>
  <span m="3910030">way,</span> <span m="3910180">the</span> <span m="3910240">reason</span>
  <span m="3910600">why</span> <span m="3910720">you're</span> <span m="3910840">seeing</span>
  <span m="3911170">what</span> <span m="3911290">looks</span> <span m="3911560">like</span>
  <span m="3911800">a</span> <span m="3911860">linear</span> <span m="3912280">hyperplane</span>
  <span m="3912790">here</span> <span m="3912970">is</span> <span m="3913090">because</span>
  <span m="3913360">there</span> <span m="3913450">are</span> <span m="3913510">exactly</span>
  <span m="3913990">two</span> <span m="3914380">cluster</span> <span m="3914740">centers.</span></p><p><span
  m="3918610">And</span> <span m="3918760">then</span> <span m="3918880">you</span>
  <span m="3918970">repeat.</span> <span m="3919450">Blah,</span> <span m="3919830">blah,</span>
  <span m="3919930">blah.</span> <span m="3920410">And</span> <span m="3920650">you're</span>
  <span m="3920770">done.</span> <span m="3921980">So</span> <span m="3922510">in</span>
  <span m="3922630">fact,</span> <span m="3922870">I</span> <span m="3922930">think</span>
  <span m="3924030">I've</span> <span m="3924190">just</span> <span m="3924340">shown</span>
  <span m="3924520">you</span> <span m="3924590">the</span> <span m="3924670">convergence</span>
  <span m="3925420">point.</span></p><p><span m="3926330">So</span> <span m="3926430">that's</span>
  <span m="3926530">the</span> <span m="3926620">K-means</span> <span m="3927010">algorithm.</span>
  <span m="3927560">It's</span> <span m="3927800">an</span> <span m="3928030">extremely</span>
  <span m="3928660">simple</span> <span m="3929020">algorithm.</span> <span m="3930320">And</span>
  <span m="3931000">what</span> <span m="3931180">I'm</span> <span m="3931300">going</span>
  <span m="3931450">to</span> <span m="3931540">show</span> <span m="3931780">you</span>
  <span m="3931930">for</span> <span m="3932080">the</span> <span m="3932140">next</span>
  <span m="3932410">10</span> <span m="3932620">minutes</span> <span m="3932890">of</span>
  <span m="3932980">lecture</span> <span m="3933490">is</span> <span m="3933700">how</span>
  <span m="3933820">one</span> <span m="3934000">could</span> <span m="3934150">use</span>
  <span m="3934420">this</span> <span m="3934630">very</span> <span m="3934900">simple</span>
  <span m="3935230">clustering</span> <span m="3935710">algorithm</span> <span m="3936400">to</span>
  <span m="3936550">better</span> <span m="3936910">understand</span> <span m="3937840">asthma.</span></p><p><span
  m="3939850">So</span> <span m="3940210">asthma</span> <span m="3940720">is</span>
  <span m="3940780">something</span> <span m="3941020">that</span> <span m="3941140">really</span>
  <span m="3941320">affects</span> <span m="3941590">a</span> <span m="3941620">large</span>
  <span m="3941860">number</span> <span m="3942100">of</span> <span m="3942220">individuals.</span>
  <span m="3944260">It's</span> <span m="3944680">characterized</span> <span m="3945220">by</span>
  <span m="3945640">having</span> <span m="3947200">difficulties</span> <span m="3947830">breathing.</span>
  <span m="3949000">It's</span> <span m="3949150">often</span> <span m="3949480">managed</span>
  <span m="3949900">by</span> <span m="3950080">inhalers,</span> <span m="3950890">although,</span>
  <span m="3951700">as</span> <span m="3951970">asthma</span> <span m="3952390">gets</span>
  <span m="3952690">more</span> <span m="3952900">and</span> <span m="3952990">more</span>
  <span m="3953140">severe,</span> <span m="3953680">you</span> <span m="3953830">need</span>
  <span m="3954040">more</span> <span m="3954310">and</span> <span m="3954400">more</span>
  <span m="3954610">complex</span> <span m="3955180">management</span> <span m="3955690">schemes.</span></p><p><span
  m="3957850">And</span> <span m="3958180">it's</span> <span m="3958360">been</span>
  <span m="3958480">found</span> <span m="3958870">that</span> <span m="3959050">5%</span>
  <span m="3959290">to</span> <span m="3959380">10%</span> <span m="3959770">of</span>
  <span m="3959830">people</span> <span m="3960340">who</span> <span m="3960490">have</span>
  <span m="3960910">severe</span> <span m="3961300">asthma</span> <span m="3962110">remain</span>
  <span m="3962560">poorly</span> <span m="3963100">controlled</span> <span m="3963610">despite</span>
  <span m="3964390">using</span> <span m="3965230">the</span> <span m="3965650">largest</span>
  <span m="3967960">tolerable</span> <span m="3970780">inhaled</span> <span m="3971260">therapy.</span>
  <span m="3971980">And</span> <span m="3972100">so</span> <span m="3972550">a</span>
  <span m="3972610">really</span> <span m="3973150">big</span> <span m="3973390">question</span>
  <span m="3973870">that</span> <span m="3974050">the</span> <span m="3974140">pharmaceutical</span>
  <span m="3975100">community</span> <span m="3975550">is</span> <span m="3975730">extremely</span>
  <span m="3976420">interested</span> <span m="3976840">in</span> <span m="3977560">is,</span>
  <span m="3977860">how</span> <span m="3978190">do</span> <span m="3978280">we</span>
  <span m="3978400">come</span> <span m="3978610">up</span> <span m="3978700">with</span>
  <span m="3978880">better</span> <span m="3979150">therapies</span> <span m="3979540">for</span>
  <span m="3979630">asthma?</span> <span m="3979960">There's</span> <span m="3980110">a</span>
  <span m="3980170">lot</span> <span m="3980530">of</span> <span m="3980620">money</span>
  <span m="3980950">in</span> <span m="3981040">that</span> <span m="3981160">problem.</span></p><p><span
  m="3982450">I</span> <span m="3982600">first</span> <span m="3982840">learned</span>
  <span m="3983080">about</span> <span m="3983260">this</span> <span m="3983410">problem</span>
  <span m="3983680">when</span> <span m="3983800">a</span> <span m="3983860">pharmaceutical</span>
  <span m="3984310">company</span> <span m="3984580">came</span> <span m="3984790">to</span>
  <span m="3984880">me</span> <span m="3985060">when</span> <span m="3985150">I</span>
  <span m="3985180">was</span> <span m="3985270">a</span> <span m="3985300">professor</span>
  <span m="3985540">at</span> <span m="3985600">NYU</span> <span m="3986020">and</span>
  <span m="3986110">asked</span> <span m="3986320">me,</span> <span m="3986440">could</span>
  <span m="3986560">they</span> <span m="3986650">work</span> <span m="3986860">with</span>
  <span m="3986980">me</span> <span m="3987070">on</span> <span m="3987160">this</span>
  <span m="3987280">problem?</span> <span m="3988000">I</span> <span m="3988090">said</span>
  <span m="3988240">no</span> <span m="3988390">at</span> <span m="3988450">the</span>
  <span m="3988510">time.</span> <span m="3988780">But</span> <span m="3988900">I</span>
  <span m="3988990">still</span> <span m="3989140">find</span> <span m="3989290">it</span>
  <span m="3989410">interesting.</span></p><p><span m="3990720">[CHUCKLING]</span></p><p>&nbsp;</p><p><span
  m="3994150">And</span> <span m="3994540">at</span> <span m="3994720">that</span>
  <span m="3994870">time,</span> <span m="3995170">the</span> <span m="3995260">company</span>
  <span m="3995590">pointed</span> <span m="3995950">me</span> <span m="3997190">to</span>
  <span m="3997660">this</span> <span m="3997810">paper,</span> <span m="3998240">which</span>
  <span m="3998320">I'll</span> <span m="3998440">tell</span> <span m="3998590">you</span>
  <span m="3998650">about</span> <span m="3998800">in</span> <span m="3998860">a</span>
  <span m="3998890">second.</span> <span m="4002560">But</span> <span m="4002640">before</span>
  <span m="4003000">I</span> <span m="4003090">get</span> <span m="4003270">there,</span>
  <span m="4003620">I want</span> <span m="4003970">to</span> <span m="4004110">point</span>
  <span m="4004410">out</span> <span m="4004560">what</span> <span m="4004710">are</span>
  <span m="4004800">some</span> <span m="4004990">of</span> <span m="4005040">the</span>
  <span m="4005130">big</span> <span m="4005490">picture</span> <span m="4005850">questions</span>
  <span m="4006390">that</span> <span m="4006780">everyone's</span> <span m="4007170">interested</span>
  <span m="4007530">in</span> <span m="4007710">when</span> <span m="4007830">it</span>
  <span m="4007890">comes</span> <span m="4008040">to</span> <span m="4008130">asthma.</span>
  <span m="4009690">The</span> <span m="4009810">first</span> <span m="4010080">one</span>
  <span m="4010200">is</span> <span m="4010260">to really</span> <span m="4010380">understand</span>
  <span m="4011340">what</span> <span m="4011700">is</span> <span m="4011910">it</span>
  <span m="4012390">about</span> <span m="4012720">either</span> <span m="4013020">genetic</span>
  <span m="4013530">or</span> <span m="4013590">environmental</span> <span m="4014040">factors</span>
  <span m="4014730">that</span> <span m="4014910">underlie</span> <span m="4015420">different</span>
  <span m="4015780">subtypes</span> <span m="4016260">of</span> <span m="4016350">asthma.</span>
  <span m="4017090">It's</span> <span m="4017220">observed</span> <span m="4017610">that</span>
  <span m="4017760">people</span> <span m="4018060">respond</span> <span m="4018420">differently</span>
  <span m="4018760">the</span> <span m="4018840">therapy.</span> <span m="4019180">It
  is</span> <span m="4019350">observed</span> <span m="4019710">that</span> <span
  m="4019800">some</span> <span m="4019950">people</span> <span m="4020190">aren't</span>
  <span m="4020430">even</span> <span m="4020610">controlled</span> <span m="4021030">with</span>
  <span m="4021210">therapy.</span> <span m="4021630">Why</span> <span m="4022020">is</span>
  <span m="4022170">that?</span></p><p><span m="4025200">Third,</span> <span m="4026370">what</span>
  <span m="4026730">are</span> <span m="4027810">biomarkers,</span> <span m="4028380">what</span>
  <span m="4028500">are</span> <span m="4028530">ways</span> <span m="4028740">to</span>
  <span m="4028830">predict</span> <span m="4029760">who's</span> <span m="4030030">going</span>
  <span m="4030210">to</span> <span m="4030270">respond</span> <span m="4030600">or</span>
  <span m="4030660">not</span> <span m="4030810">respond</span> <span m="4031120">to
  any one</span> <span m="4031410">therapy?</span> <span m="4033090">And</span> <span
  m="4034050">can</span> <span m="4034170">we</span> <span m="4034230">get</span>
  <span m="4034380">better</span> <span m="4034560">mechanistic</span> <span m="4035100">understanding</span>
  <span m="4035970">of</span> <span m="4036240">these</span> <span m="4036450">different</span>
  <span m="4036690">subtypes?</span> <span m="4038290">And</span> <span m="4038390">so</span>
  <span m="4039870">this</span> <span m="4040080">was</span> <span m="4040260">a</span>
  <span m="4040440">long-standing</span> <span m="4041070">question.</span> <span
  m="4042840">And</span> <span m="4043680">in</span> <span m="4043800">this</span>
  <span m="4043980">paper</span> <span m="4045000">from</span> <span m="4045840">the</span>
  <span m="4045950"><i>American</i></span> <span m="4046180"><i>Journal</i></span>
  <span m="4046280"><i>of</i></span> <span m="4046380"><i>Respiratory</i></span> <span
  m="4046840"><i>Critical</i></span> <span m="4047160"><i>Care</i></span> <span m="4047460"><i>Medicine,</i></span>
  <span m="4047910">which,</span> <span m="4048390">by</span> <span m="4048540">the</span>
  <span m="4048630">way,</span> <span m="4048750">has</span> <span m="4048900">a</span>
  <span m="4048930">huge</span> <span m="4049170">number</span> <span m="4049320">of</span>
  <span m="4049380">citations</span> <span m="4049890">now--</span> <span m="4050160">it's</span>
  <span m="4050430">sort</span> <span m="4050640">of</span> <span m="4050730">a</span>
  <span m="4050820">prototypical</span> <span m="4051510">example</span> <span m="4051960">of</span>
  <span m="4052050">subtyping.</span> <span m="4052980">That's</span> <span m="4053130">why</span>
  <span m="4053220">I'm</span> <span m="4053310">going</span> <span m="4053520">through</span>
  <span m="4053670">it.</span> <span m="4055440">They</span> <span m="4056250">started</span>
  <span m="4056610">to</span> <span m="4056700">answer</span> <span m="4057000">that</span>
  <span m="4057120">question</span> <span m="4057480">using</span> <span m="4058370">a</span>
  <span m="4058440">data-driven</span> <span m="4058950">approach</span> <span m="4059250">for</span>
  <span m="4059430">asthma.</span></p><p><span m="4060390">And</span> <span m="4060480">what</span>
  <span m="4060600">I'm</span> <span m="4060690">showing</span> <span m="4060990">you</span>
  <span m="4061080">here</span> <span m="4061380">is</span> <span m="4061530">the</span>
  <span m="4061620">punch</span> <span m="4061850">line.</span> <span m="4062130">This</span>
  <span m="4062280">is</span> <span m="4062400">that</span> <span m="4063000">main</span>
  <span m="4063360">result,</span> <span m="4063840">the</span> <span m="4063930">main</span>
  <span m="4064170">figure</span> <span m="4064500">over</span> <span m="4064590">the</span>
  <span m="4064680">paper.</span> <span m="4065670">They've</span> <span m="4065850">characterized</span>
  <span m="4068070">asthma</span> <span m="4068670">in</span> <span m="4068790">terms</span>
  <span m="4069210">of</span> <span m="4070050">five</span> <span m="4070470">different</span>
  <span m="4072300">subtypes,</span> <span m="4072900">really</span> <span m="4074220">three</span>
  <span m="4075390">type.</span> <span m="4076980">One</span> <span m="4077220">type,</span>
  <span m="4077600">which</span> <span m="4077630">I'll show</span> <span m="4077790">over</span>
  <span m="4078030">here,</span> <span m="4078340">was</span> <span m="4078450">sort</span>
  <span m="4078600">of</span> <span m="4078660">inflammation</span> <span m="4079230">predominant;</span>
  <span m="4080160">one</span> <span m="4080400">type</span> <span m="4080670">over</span>
  <span m="4080820">there,</span> <span m="4081190">which</span> <span m="4081240">is</span>
  <span m="4081330">called</span> <span m="4081600">early</span> <span m="4081900">symptom</span>
  <span m="4083180">predominant;</span> <span m="4085140">and</span> <span m="4085620">another</span>
  <span m="4085890">here,</span> <span m="4086030">which</span> <span m="4086140">is</span>
  <span m="4086220">sort</span> <span m="4086340">of</span> <span m="4086400">concordant</span>
  <span m="4086910">disease.</span> <span m="4089410">And</span> <span m="4089760">what</span>
  <span m="4089880">I'll</span> <span m="4090000">do</span> <span m="4090210">over</span>
  <span m="4090300">the</span> <span m="4090390">next</span> <span m="4090600">few</span>
  <span m="4090750">minutes</span> <span m="4091050">is</span> <span m="4091170">walk</span>
  <span m="4091440">you</span> <span m="4091620">through</span> <span m="4091860">how</span>
  <span m="4092010">they</span> <span m="4092130">came</span> <span m="4092400">up</span>
  <span m="4092520">with</span> <span m="4092640">these</span> <span m="4092790">different</span>
  <span m="4093690">clusters.</span></p><p><span m="4095740">So</span> <span m="4095970">they</span>
  <span m="4096090">used</span> <span m="4096359">three</span> <span m="4096689">different</span>
  <span m="4097000">data</span> <span m="4097370">sets.</span> <span m="4099180">These</span>
  <span m="4099359">data</span> <span m="4099510">sets</span> <span m="4099750">consisted</span>
  <span m="4100200">of</span> <span m="4100410">patients</span> <span m="4101550">who</span>
  <span m="4102870">had</span> <span m="4103140">asthma</span> <span m="4103649">and</span>
  <span m="4103890">already</span> <span m="4104160">had</span> <span m="4104520">at</span>
  <span m="4104640">least</span> <span m="4104910">one</span> <span m="4105359">recent</span>
  <span m="4105689">therapy</span> <span m="4106080">for</span> <span m="4106260">asthma.</span>
  <span m="4107580">They're</span> <span m="4107760">all</span> <span m="4107970">nonsmokers.</span>
  <span m="4109109">But</span> <span m="4109319">they</span> <span m="4109439">were</span>
  <span m="4109590">managed</span> <span m="4110200">in--</span> <span m="4111640">they're</span>
  <span m="4111810">three</span> <span m="4112229">disjoint</span> <span m="4113399">set</span>
  <span m="4113520">of</span> <span m="4113569">patients</span> <span m="4113970">coming</span>
  <span m="4114240">from</span> <span m="4114390">three</span> <span m="4114660">different</span>
  <span m="4115170">populations.</span> <span m="4116560">The</span> <span m="4116580">first</span>
  <span m="4116880">group</span> <span m="4117060">of</span> <span m="4117120">patients</span>
  <span m="4117990">were</span> <span m="4118170">recruited</span> <span m="4118680">from</span>
  <span m="4119370">primary</span> <span m="4119910">care</span> <span m="4120180">practices</span>
  <span m="4120750">in</span> <span m="4120810">the</span> <span m="4120870">United</span>
  <span m="4121140">Kingdom.</span></p><p><span m="4122140">All</span> <span m="4122210">right.</span>
  <span m="4122370">So</span> <span m="4122490">if</span> <span m="4122580">you're</span>
  <span m="4123090">a</span> <span m="4123149">patient</span> <span m="4123929">with</span>
  <span m="4124319">asthma,</span> <span m="4126120">and</span> <span m="4126210">your</span>
  <span m="4126330">asthma is</span> <span m="4126720">being</span> <span m="4126870">managed</span>
  <span m="4127260">by</span> <span m="4127410">your</span> <span m="4127529">primary</span>
  <span m="4127890">care</span> <span m="4128130">doctor,</span> <span m="4129479">then</span>
  <span m="4129630">it's</span> <span m="4129779">probably</span> <span m="4130170">not</span>
  <span m="4130410">too</span> <span m="4130620">bad.</span> <span m="4132300">But</span>
  <span m="4132479">if</span> <span m="4132540">your</span> <span m="4132609">asthma,</span>
  <span m="4132880">on</span> <span m="4133000">the other</span> <span m="4133260">hand,</span>
  <span m="4133470">were</span> <span m="4133590">being</span> <span m="4133770">managed</span>
  <span m="4134460">at</span> <span m="4134729">a</span> <span m="4134850">refractory</span>
  <span m="4135569">asthma</span> <span m="4136050">clinic,</span> <span m="4136590">which</span>
  <span m="4136800">is</span> <span m="4136890">designed</span> <span m="4137220">specifically</span>
  <span m="4138060">for</span> <span m="4138210">helping</span> <span m="4138479">patients</span>
  <span m="4138779">manage</span> <span m="4139109">asthma,</span> <span m="4139410">then</span>
  <span m="4139529">your</span> <span m="4139620">asthma</span> <span m="4139899">is</span>
  <span m="4139979">probably</span> <span m="4140470">a</span> <span m="4140490">bit</span>
  <span m="4140640">more</span> <span m="4140790">severe.</span> <span m="4141550">And</span>
  <span m="4141660">that</span> <span m="4141720">second</span> <span m="4142109">group</span>
  <span m="4142290">of</span> <span m="4142350">patients,</span> <span m="4142859">187</span>
  <span m="4143790">patients,</span> <span m="4144120">were</span> <span m="4144240">from</span>
  <span m="4144420">that</span> <span m="4144569">second</span> <span m="4145529">cohort</span>
  <span m="4145979">of</span> <span m="4146850">patients</span> <span m="4147149">managed</span>
  <span m="4147950">out</span> <span m="4148120">of an</span> <span m="4148260">asthma</span>
  <span m="4148620">clinic.</span></p><p><span m="4149939">The</span> <span m="4150060">third</span>
  <span m="4150420">data</span> <span m="4150700">set</span> <span m="4151080">is</span>
  <span m="4151229">much</span> <span m="4151470">smaller,</span> <span m="4151859">only</span>
  <span m="4152069">68</span> <span m="4152580">patients.</span> <span m="4153720">But</span>
  <span m="4153840">it's</span> <span m="4153990">very</span> <span m="4154380">unique</span>
  <span m="4154740">because</span> <span m="4154979">it</span> <span m="4155250">is</span>
  <span m="4156330">coming</span> <span m="4156660">from</span> <span m="4156899">a</span>
  <span m="4157040">12-month</span> <span m="4157649">study,</span> <span m="4158970">where</span>
  <span m="4159450">it</span> <span m="4159569">was</span> <span m="4159660">a</span>
  <span m="4159720">clinical</span> <span m="4160140">trial,</span> <span m="4161100">and</span>
  <span m="4161729">there</span> <span m="4162060">were</span> <span m="4162540">two</span>
  <span m="4162840">different</span> <span m="4163170">types</span> <span m="4163410">of</span>
  <span m="4163500">treatments</span> <span m="4164189">applied</span> <span m="4166050">given</span>
  <span m="4167220">to</span> <span m="4167689">these</span> <span m="4167840">patients.</span>
  <span m="4168979">And</span> <span m="4169100">it</span> <span m="4169160">was</span>
  <span m="4169250">a</span> <span m="4169310">randomized</span> <span m="4169729">control</span>
  <span m="4170060">trial.</span> <span m="4170420">So the</span> <span m="4170490">patients</span>
  <span m="4170899">were</span> <span m="4171080">randomized</span> <span m="4171620">into</span>
  <span m="4171859">each</span> <span m="4172040">of</span> <span m="4172100">the</span>
  <span m="4172189">two</span> <span m="4172670">arms</span> <span m="4173210">of</span>
  <span m="4173330">the</span> <span m="4173420">study.</span></p><p><span m="4176649">I'll</span>
  <span m="4176770">describe</span> <span m="4177220">to</span> <span m="4177340">you</span>
  <span m="4177399">what</span> <span m="4177520">the</span> <span m="4177609">features</span>
  <span m="4178149">are</span> <span m="4178450">on</span> <span m="4178569">just</span>
  <span m="4178779">the</span> <span m="4178870">next</span> <span m="4179140">slide.</span>
  <span m="4179560">But</span> <span m="4179670">first</span> <span m="4179920">I</span>
  <span m="4179950">want</span> <span m="4180069">to</span> <span m="4180130">tell</span>
  <span m="4180310">you</span> <span m="4180399">about</span> <span m="4180550">how</span>
  <span m="4180819">their</span> <span m="4180960">pre-processes</span> <span m="4181800">to</span>
  <span m="4181990">use</span> <span m="4182229">within</span> <span m="4182470">the</span>
  <span m="4182529">K-means</span> <span m="4183010">algorithm.</span> <span m="4184899">Continuous-valued</span>
  <span m="4186460">features</span> <span m="4187120">where</span> <span m="4187500">z-scored</span>
  <span m="4188319">in</span> <span m="4188439">order</span> <span m="4188560">to</span>
  <span m="4188740">normalize</span> <span m="4189460">their</span> <span m="4189609">ranges.</span>
  <span m="4190930">And</span> <span m="4191470">categorical</span> <span m="4192130">variables</span>
  <span m="4192550">were</span> <span m="4192850">represented</span> <span m="4193359">just</span>
  <span m="4193600">by</span> <span m="4193880">a</span> <span m="4194290">one-hot</span>
  <span m="4194710">encoding.</span></p><p><span m="4197740">Some</span> <span m="4197950">of</span>
  <span m="4198010">the</span> <span m="4198070">continuous</span> <span m="4198580">variables</span>
  <span m="4199270">were</span> <span m="4199550">furthermore</span> <span m="4202720">transformed</span>
  <span m="4203530">prior</span> <span m="4203920">to</span> <span m="4204070">clustering</span>
  <span m="4204670">by</span> <span m="4204790">taking</span> <span m="4205120">the</span>
  <span m="4205240">logarithm</span> <span m="4205870">of</span> <span m="4205930">the</span>
  <span m="4206020">features.</span> <span m="4207160">And</span> <span m="4207280">that's</span>
  <span m="4207400">something</span> <span m="4207580">that</span> <span m="4207670">can</span>
  <span m="4207760">be</span> <span m="4207850">very</span> <span m="4208210">useful</span>
  <span m="4208840">when</span> <span m="4209290">doing</span> <span m="4209530">something</span>
  <span m="4209830">like</span> <span m="4210250">K-means.</span> <span m="4211480">Because</span>
  <span m="4213250">it</span> <span m="4213670">can,</span> <span m="4213910">in</span>
  <span m="4213970">essence,</span> <span m="4214270">allow</span> <span m="4214600">for</span>
  <span m="4214840">that</span> <span m="4215020">Euclidean</span> <span m="4215650">distance</span>
  <span m="4216010">function,</span> <span m="4216370">which</span> <span m="4216490">is</span>
  <span m="4216610">using</span> <span m="4216910">K-means,</span> <span m="4217300">to</span>
  <span m="4217390">be</span> <span m="4217510">more</span> <span m="4217690">meaningful</span>
  <span m="4220120">by</span> <span m="4220270">capturing</span> <span m="4220750">more</span>
  <span m="4220900">of</span> <span m="4220990">a</span> <span m="4221030">dynamic</span>
  <span m="4221440">range</span> <span m="4221830">of</span> <span m="4221920">the</span>
  <span m="4222010">feature.</span></p><p><span m="4223960">So</span> <span m="4224110">these</span>
  <span m="4224320">were</span> <span m="4224410">the</span> <span m="4224530">features</span>
  <span m="4225100">that</span> <span m="4225250">went</span> <span m="4225460">into</span>
  <span m="4225700">the</span> <span m="4225790">clustering</span> <span m="4226270">algorithm.</span>
  <span m="4228960">And</span> <span m="4229300">there</span> <span m="4229430">are</span>
  <span m="4229480">very,</span> <span m="4229910">very</span> <span m="4230050">few,</span>
  <span m="4232270">so</span> <span m="4232540">roughly</span> <span m="4232960">20,</span>
  <span m="4233470">30</span> <span m="4233740">features.</span> <span m="4235330">They</span>
  <span m="4235480">range</span> <span m="4235840">from</span> <span m="4236140">the</span>
  <span m="4236200">patient's</span> <span m="4236560">gender</span> <span m="4237040">and</span>
  <span m="4237220">age</span> <span m="4237910">to</span> <span m="4238480">their</span>
  <span m="4238630">body</span> <span m="4238900">mass</span> <span m="4239170">index,</span>
  <span m="4240450">to</span> <span m="4240760">measures</span> <span m="4241480">of</span>
  <span m="4241780">their</span> <span m="4242020">function,</span> <span m="4244970">to</span>
  <span m="4245200">biomarkers</span> <span m="4246160">such</span> <span m="4246430">as</span>
  <span m="4246610">eosinophil</span> <span m="4247420">count</span> <span m="4247870">that</span>
  <span m="4248020">could</span> <span m="4248110">be</span> <span m="4248200">measured</span>
  <span m="4249160">from the</span> <span m="4249430">patient's</span> <span m="4249700">sputum,</span>
  <span m="4253270">and</span> <span m="4253720">more.</span> <span m="4254080">And</span>
  <span m="4254200">there</span> <span m="4254330">a</span> <span m="4254380">couple</span>
  <span m="4254560">of</span> <span m="4254650">other</span> <span m="4254800">features</span>
  <span m="4255100">that</span> <span m="4255190">I'll</span> <span m="4256020">show</span>
  <span m="4256390">you</span> <span m="4256450">later</span> <span m="4256690">as</span>
  <span m="4256810">well.</span> <span m="4257750">And</span> <span m="4257830">you</span>
  <span m="4257890">could</span> <span m="4258010">look</span> <span m="4258130">to</span>
  <span m="4258250">see</span> <span m="4259240">how</span> <span m="4259420">did</span>
  <span m="4259540">these</span> <span m="4259780">quantities,</span> <span m="4260950">how</span>
  <span m="4261040">did</span> <span m="4261130">these</span> <span m="4261220">populations,</span>
  <span m="4261730">differ.</span></p><p><span m="4262510">So</span> <span m="4262780">on</span>
  <span m="4262930">this</span> <span m="4263080">column,</span> <span m="4263510">you</span>
  <span m="4263530">see</span> <span m="4264010">the</span> <span m="4264220">primary</span>
  <span m="4264640">care</span> <span m="4264940">population.</span> <span m="4265540">You</span>
  <span m="4265600">look</span> <span m="4265780">at</span> <span m="4265930">all</span>
  <span m="4266080">of</span> <span m="4266140">these</span> <span m="4266290">features</span>
  <span m="4266620">in</span> <span m="4266710">that</span> <span m="4266860">population.</span>
  <span m="4267760">You</span> <span m="4267910">see</span> <span m="4268090">that</span>
  <span m="4268910">in</span> <span m="4269060">the</span> <span m="4269140">primary</span>
  <span m="4269830">care</span> <span m="4270040">population,</span> <span m="4274645">the</span>
  <span m="4274930">individuals</span> <span m="4276520">are--</span> <span m="4276970">on</span>
  <span m="4277150">average,</span> <span m="4278260">54%</span> <span m="4280000">percent</span>
  <span m="4280300">of</span> <span m="4280360">them</span> <span m="4282010">are</span>
  <span m="4282490">female.</span> <span m="4283470">In</span> <span m="4283660">the</span>
  <span m="4283750">secondary</span> <span m="4284170">care</span> <span m="4284500">population,</span>
  <span m="4285100">65%</span> <span m="4285790">of</span> <span m="4285850">them</span>
  <span m="4285970">are</span> <span m="4286030">female.</span> <span m="4287740">You</span>
  <span m="4287830">notice</span> <span m="4288130">that</span> <span m="4288250">things</span>
  <span m="4288550">like--</span> <span m="4288820">if</span> <span m="4288880">you</span>
  <span m="4288970">look</span> <span m="4289120">at</span> <span m="4289310">to</span>
  <span m="4289720">some</span> <span m="4289930">measures</span> <span m="4291535">of</span>
  <span m="4292030">lung</span> <span m="4292423">function,</span> <span m="4293210">it's</span>
  <span m="4293290">significantly</span> <span m="4293920">worse</span> <span m="4294340">in</span>
  <span m="4294460">that</span> <span m="4294670">secondary</span> <span m="4295240">care</span>
  <span m="4296290">population,</span> <span m="4296890">as</span> <span m="4297070">one</span>
  <span m="4297220">would</span> <span m="4297340">expect.</span> <span m="4297670">Because</span>
  <span m="4297970">these</span> <span m="4298120">are</span> <span m="4300310">patients</span>
  <span m="4300610">with</span> <span m="4300700">more</span> <span m="4300820">severe</span>
  <span m="4301090">asthma.</span></p><p><span m="4302830">So</span> <span m="4303100">next,</span>
  <span m="4303370">after</span> <span m="4303550">doing</span> <span m="4303790">K-means</span>
  <span m="4304210">clustering,</span> <span m="4306040">these</span> <span m="4306430">are</span>
  <span m="4306640">the</span> <span m="4306730">three</span> <span m="4307030">clusters</span>
  <span m="4307510">that</span> <span m="4307600">result.</span> <span m="4308030">And</span>
  <span m="4308100">now</span> <span m="4308260">I'm</span> <span m="4308380">showing</span>
  <span m="4308680">you</span> <span m="4308770">the</span> <span m="4308860">full</span>
  <span m="4309070">set</span> <span m="4309250">of</span> <span m="4309310">features.</span>
  <span m="4313640">So</span> <span m="4315010">let</span> <span m="4315160">me</span>
  <span m="4315280">first</span> <span m="4315520">tell</span> <span m="4315670">you</span>
  <span m="4315760">how</span> <span m="4315850">to</span> <span m="4315940">read</span>
  <span m="4316180">this.</span> <span m="4317650">This</span> <span m="4317890">is</span>
  <span m="4318250">clusters</span> <span m="4318940">found</span> <span m="4319390">in</span>
  <span m="4319510">the</span> <span m="4319600">primary</span> <span m="4320200">care</span>
  <span m="4320470">population.</span> <span m="4321700">This</span> <span m="4321940">column</span>
  <span m="4322330">here</span> <span m="4322690">is</span> <span m="4322870">just</span>
  <span m="4323260">the</span> <span m="4323560">average</span> <span m="4324250">values</span>
  <span m="4324820">of</span> <span m="4324910">those</span> <span m="4325090">features</span>
  <span m="4325450">across</span> <span m="4325750">the</span> <span m="4325870">full</span>
  <span m="4326260">population.</span></p><p><span m="4327520">And</span> <span m="4327610">then</span>
  <span m="4327730">for</span> <span m="4327940">each</span> <span m="4328330">one</span>
  <span m="4328660">of</span> <span m="4328870">these</span> <span m="4329170">three</span>
  <span m="4329590">clusters,</span> <span m="4330770">I'm</span> <span m="4330820">showing</span>
  <span m="4331120">you</span> <span m="4331180">the</span> <span m="4331300">average</span>
  <span m="4331840">value</span> <span m="4332440">of</span> <span m="4332620">the</span>
  <span m="4332800">corresponding</span> <span m="4333370">feature</span> <span m="4333760">in</span>
  <span m="4333940">just</span> <span m="4334270">that</span> <span m="4334450">cluster.</span>
  <span m="4336560">And</span> <span m="4337030">in</span> <span m="4337120">essence,</span>
  <span m="4338650">that's</span> <span m="4339010">exactly</span> <span m="4339430">the</span>
  <span m="4339520">same</span> <span m="4339880">as</span> <span m="4340090">those</span>
  <span m="4340300">red</span> <span m="4340510">points</span> <span m="4340840">I</span>
  <span m="4340870">was</span> <span m="4340960">showing</span> <span m="4341200">you</span>
  <span m="4341290">when</span> <span m="4341380">I</span> <span m="4341440">describe</span>
  <span m="4341770">to you</span> <span m="4341860">K-means</span> <span m="4342340">clustering.</span>
  <span m="4342940">It's</span> <span m="4343120">the</span> <span m="4343240">cluster</span>
  <span m="4343600">center.</span> <span m="4345550">And</span> <span m="4345670">one</span>
  <span m="4345820">could</span> <span m="4345950">also</span> <span m="4346180">look</span>
  <span m="4346420">at</span> <span m="4346510">the</span> <span m="4346630">standard</span>
  <span m="4346960">deviation</span> <span m="4348100">of</span> <span m="4348550">how</span>
  <span m="4348850">much</span> <span m="4350470">variance</span> <span m="4351100">there</span>
  <span m="4351310">is</span> <span m="4351610">along</span> <span m="4351880">that</span>
  <span m="4352030">feature</span> <span m="4352360">in</span> <span m="4352480">that</span>
  <span m="4352600">cluster.</span> <span m="4353050">And</span> <span m="4353140">that's</span>
  <span m="4353290">what</span> <span m="4353380">the</span> <span m="4353440">numbers</span>
  <span m="4353740">in</span> <span m="4353860">parentheses</span> <span m="4354430">are</span>
  <span m="4354490">telling</span> <span m="4354850">you.</span></p><p><span m="4358600">So</span>
  <span m="4359340">the</span> <span m="4359430">first</span> <span m="4359700">thing</span>
  <span m="4359850">to</span> <span m="4359970">note</span> <span m="4360480">is</span>
  <span m="4360660">that</span> <span m="4361380">in</span> <span m="4361710">Cluster</span>
  <span m="4362130">1,</span> <span m="4363350">which</span> <span m="4363930">the</span>
  <span m="4364260">authors</span> <span m="4364710">of</span> <span m="4364770">the</span>
  <span m="4364860">study</span> <span m="4365460">named</span> <span m="4366330">Early</span>
  <span m="4366630">Onset</span> <span m="4367950">Atopic</span> <span m="4368640">Asthma,</span>
  <span m="4369970">these</span> <span m="4370050">are</span> <span m="4370140">very</span>
  <span m="4370680">young</span> <span m="4371010">patients,</span> <span m="4371760">average</span>
  <span m="4372360">of</span> <span m="4372570">14,</span> <span m="4373530">15</span>
  <span m="4374010">years</span> <span m="4374280">old,</span> <span m="4375180">as</span>
  <span m="4375330">opposed</span> <span m="4375600">to</span> <span m="4375660">Cluster</span>
  <span m="4375990">2,</span> <span m="4376320">where</span> <span m="4376440">the</span>
  <span m="4376530">average</span> <span m="4376890">age</span> <span m="4377070">was</span>
  <span m="4377220">35</span> <span m="4377850">years</span> <span m="4378060">old--</span>
  <span m="4378240">so</span> <span m="4378360">a</span> <span m="4378390">dramatic</span>
  <span m="4378810">difference</span> <span m="4379200">there.</span> <span m="4381180">Moreover,</span>
  <span m="4381780">we</span> <span m="4381900">see</span> <span m="4382020">that</span>
  <span m="4382170">these</span> <span m="4382350">are</span> <span m="4382440">patients</span>
  <span m="4383130">who</span> <span m="4384210">have</span> <span m="4385950">actually</span>
  <span m="4387360">been</span> <span m="4387690">to</span> <span m="4387810">the</span>
  <span m="4387900">hospital</span> <span m="4388470">recently.</span> <span m="4390390">So</span>
  <span m="4390990">most</span> <span m="4391350">of</span> <span m="4391410">these</span>
  <span m="4391560">patients</span> <span m="4391980">have</span> <span m="4392190">been</span>
  <span m="4392310">to</span> <span m="4392400">the</span> <span m="4392460">hospital.</span>
  <span m="4393120">On</span> <span m="4393300">average,</span> <span m="4393630">these</span>
  <span m="4393720">patients</span> <span m="4393990">have</span> <span m="4394080">been</span>
  <span m="4394170">to</span> <span m="4394260">hospital</span> <span m="4394710">at</span>
  <span m="4394920">least</span> <span m="4395190">once</span> <span m="4395730">recently.</span></p><p><span
  m="4397650">And</span> <span m="4398310">furthermore,</span> <span m="4398760">they've</span>
  <span m="4398910">had</span> <span m="4399120">severe</span> <span m="4399480">asthma</span>
  <span m="4399810">exacerbations</span> <span m="4401010">in</span> <span m="4401100">the</span>
  <span m="4401190">past</span> <span m="4401520">12</span> <span m="4401760">months,</span>
  <span m="4402120">at</span> <span m="4402210">least,</span> <span m="4403110">on</span>
  <span m="4403260">average,</span> <span m="4403590">twice</span> <span m="4404100">per</span>
  <span m="4404280">patient.</span> <span m="4405870">And</span> <span m="4405960">those</span>
  <span m="4406110">are</span> <span m="4406170">very</span> <span m="4406440">large</span>
  <span m="4406710">numbers</span> <span m="4407130">relative</span> <span m="4407460">to</span>
  <span m="4407520">what</span> <span m="4407670">you</span> <span m="4407790">see</span>
  <span m="4408210">in</span> <span m="4408300">these</span> <span m="4408450">other</span>
  <span m="4408630">clusters.</span> <span m="4409200">So</span> <span m="4409320">that's</span>
  <span m="4409500">really</span> <span m="4410280">describing</span> <span m="4411630">something</span>
  <span m="4411910">that's</span> <span m="4412050">very</span> <span m="4412320">unusual</span>
  <span m="4412890">about</span> <span m="4413190">these</span> <span m="4413370">very</span>
  <span m="4413580">young</span> <span m="4413940">patients</span> <span m="4414510">with</span>
  <span m="4414780">pretty</span> <span m="4415020">severe</span> <span m="4415590">asthma.</span>
  <span m="4416760">Yep?</span></p><p><span m="4417429">AUDIENCE:</span> <span m="4417592">What</span>
  <span m="4417755">is</span> <span m="4417918">the p-value</span> <span m="4418407">[INAUDIBLE]?</span></p><p><span
  m="4421830">DAVID SONTAG:</span> <span m="4421995">Yeah.</span> <span m="4422160">I</span>
  <span m="4422220">think</span> <span m="4422400">the</span> <span m="4422490">p-value--</span>
  <span m="4423090">I</span> <span m="4423420">don't</span> <span m="4423570">know</span>
  <span m="4423720">if</span> <span m="4423840">this</span> <span m="4424020">is</span>
  <span m="4424140">a</span> <span m="4424170">pair-wise</span> <span m="4424620">comparison.</span>
  <span m="4425220">I</span> <span m="4425280">don't</span> <span m="4425400">remember</span>
  <span m="4425730">off</span> <span m="4425790">the top of</span> <span m="4425970">my</span>
  <span m="4426120">head.</span> <span m="4426300">But</span> <span m="4426450">it's</span>
  <span m="4426750">really</span> <span m="4426900">looking</span> <span m="4427110">at</span>
  <span m="4427170">the</span> <span m="4427230">difference</span> <span m="4427650">between,</span>
  <span m="4430440">let's</span> <span m="4430620">say--</span> <span m="4432420">I</span>
  <span m="4432630">don't</span> <span m="4432780">know</span> <span m="4432900">which</span>
  <span m="4433110">of</span> <span m="4433200">these</span> <span m="4433320">cl--</span>
  <span m="4434420">I</span> <span m="4434920">don't</span> <span m="4435060">know</span>
  <span m="4435150">if</span> <span m="4435210">it's</span> <span m="4435350">comparing</span>
  <span m="4435680">two</span> <span m="4435840">of</span> <span m="4436020">them</span>
  <span m="4436140">or</span> <span m="4436200">not.</span> <span m="4436370">But
  let's</span> <span m="4436530">say,</span> <span m="4436920">for</span> <span m="4437010">example,</span>
  <span m="4437490">it might be</span> <span m="4437720">looking</span> <span m="4437830">at</span>
  <span m="4437910">the</span> <span m="4438000">difference</span> <span m="4438270">between</span>
  <span m="4438840">this</span> <span m="4439140">and</span> <span m="4439260">that.</span>
  <span m="4440370">But</span> <span m="4440580">I'm</span> <span m="4440700">just</span>
  <span m="4440820">hypothesizing.</span> <span m="4441360">I</span> <span m="4441460">don't</span>
  <span m="4441540">remember.</span></p><p><span m="4444630">Cluster</span> <span
  m="4445010">2,</span> <span m="4445260">one</span> <span m="4445370">other</span>
  <span m="4445560">hand,</span> <span m="4446890">was</span> <span m="4447090">predominately</span>
  <span m="4447870">female.</span> <span m="4448380">So</span> <span m="4448680">81%</span>
  <span m="4449925">of</span> <span m="4450210">the</span> <span m="4450300">patients</span>
  <span m="4450630">were</span> <span m="4450750">female</span> <span m="4451080">there.</span>
  <span m="4452160">And</span> <span m="4452520">they</span> <span m="4452700">were</span>
  <span m="4453390">largely</span> <span m="4453990">overweight.</span> <span m="4454530">So</span>
  <span m="4454680">their</span> <span m="4454890">average</span> <span m="4455220">body</span>
  <span m="4455400">mass</span> <span m="4455580">index</span> <span m="4456000">was</span>
  <span m="4456320">36,</span> <span m="4457080">as</span> <span m="4457260">opposed</span>
  <span m="4457620">to</span> <span m="4457890">the</span> <span m="4458160">other</span>
  <span m="4458430">two</span> <span m="4458580">clusters,</span> <span m="4458970">where</span>
  <span m="4459070">the</span> <span m="4459150">average</span> <span m="4459450">body</span>
  <span m="4459630">mass</span> <span m="4459780">index</span> <span m="4460080">was</span>
  <span m="4460200">26.</span> <span m="4464220">And</span> <span m="4464430">Cluster</span>
  <span m="4464790">3</span> <span m="4466620">consisted</span> <span m="4467340">of</span>
  <span m="4468120">patients</span> <span m="4469110">who</span> <span m="4470490">really</span>
  <span m="4470940">have</span> <span m="4471120">not</span> <span m="4471600">had</span>
  <span m="4472020">that</span> <span m="4472290">severe</span> <span m="4472680">asthma.</span>
  <span m="4473280">So</span> <span m="4474150">the</span> <span m="4474630">average</span>
  <span m="4474990">number</span> <span m="4475170">of</span> <span m="4475230">previous</span>
  <span m="4475530">hospital</span> <span m="4475860">admissions</span> <span m="4476250">and</span>
  <span m="4477930">asthma</span> <span m="4478290">exacerbations</span> <span m="4479040">was</span>
  <span m="4479250">dramatically</span> <span m="4479700">smaller</span> <span m="4480030">than</span>
  <span m="4480210">in the</span> <span m="4480290">other</span> <span m="4480480">two</span>
  <span m="4480660">clusters.</span></p><p><span m="4482100">So</span> <span m="4482980">this</span>
  <span m="4483360">is</span> <span m="4483450">the</span> <span m="4483540">result</span>
  <span m="4483900">of</span> <span m="4483960">the</span> <span m="4484050">finding.</span>
  <span m="4485270">And</span> <span m="4485370">then</span> <span m="4485490">you</span>
  <span m="4485550">might</span> <span m="4485700">ask,</span> <span m="4486180">well,</span>
  <span m="4486960">how</span> <span m="4487140">does</span> <span m="4487260">that</span>
  <span m="4487380">generalize</span> <span m="4487740">to</span> <span m="4487800">the</span>
  <span m="4487860">other</span> <span m="4488160">two</span> <span m="4488340">populations?</span>
  <span m="4489460">So</span> <span m="4490230">they</span> <span m="4490350">then</span>
  <span m="4490500">went</span> <span m="4490680">to</span> <span m="4490770">the</span>
  <span m="4490860">secondary</span> <span m="4491460">care</span> <span m="4491910">population.</span>
  <span m="4493050">And</span> <span m="4493590">they</span> <span m="4493770">reran</span>
  <span m="4494280">the</span> <span m="4494340">clustering</span> <span m="4494840">algorithm</span>
  <span m="4495120">from</span> <span m="4495330">scratch.</span> <span m="4496530">And</span>
  <span m="4496890">this</span> <span m="4497040">is</span> <span m="4497130">a</span>
  <span m="4497160">completely</span> <span m="4497550">disjoint</span> <span m="4497940">set</span>
  <span m="4498090">of</span> <span m="4498150">patients.</span></p><p><span m="4498700">And</span>
  <span m="4498720">what</span> <span m="4498810">they</span> <span m="4498930">found,</span>
  <span m="4499530">what</span> <span m="4499680">they</span> <span m="4499800">got</span>
  <span m="4500010">out,</span> <span m="4500460">is</span> <span m="4500640">that</span>
  <span m="4500890">the</span> <span m="4501000">first</span> <span m="4501300">two</span>
  <span m="4501480">clusters</span> <span m="4502380">exactly</span> <span m="4502920">resembled</span>
  <span m="4503340">Clusters</span> <span m="4503760">1</span> <span m="4503970">and</span>
  <span m="4504060">2</span> <span m="4504390">from</span> <span m="4504600">the</span>
  <span m="4504690">previous</span> <span m="4505080">study</span> <span m="4506250">on</span>
  <span m="4506400">the</span> <span m="4506490">primary</span> <span m="4506790">care</span>
  <span m="4506970">population.</span> <span m="4507960">But</span> <span m="4508080">because</span>
  <span m="4508500">this</span> <span m="4508710">is</span> <span m="4509580">a</span>
  <span m="4509640">different</span> <span m="4510000">population</span> <span m="4510450">with</span>
  <span m="4510600">much</span> <span m="4510780">more</span> <span m="4510900">severe</span>
  <span m="4511230">patients,</span> <span m="4512130">that</span> <span m="4512370">third</span>
  <span m="4512820">cluster</span> <span m="4513270">earlier</span> <span m="4514140">of</span>
  <span m="4514680">benign</span> <span m="4515190">asthma</span> <span m="4515520">doesn't</span>
  <span m="4515820">show</span> <span m="4516090">up</span> <span m="4516270">in</span>
  <span m="4516330">this</span> <span m="4516480">new</span> <span m="4516600">population.</span>
  <span m="4517530">And</span> <span m="4517650">there</span> <span m="4517770">are</span>
  <span m="4517830">two</span> <span m="4518100">new</span> <span m="4518370">clusters</span>
  <span m="4518880">that</span> <span m="4519000">show</span> <span m="4519210">up</span>
  <span m="4519360">in</span> <span m="4519450">this new</span> <span m="4519780">population.</span></p><p><span
  m="4522400">So</span> <span m="4522750">the</span> <span m="4522840">fact</span>
  <span m="4523140">that</span> <span m="4523230">those</span> <span m="4523440">first</span>
  <span m="4523710">two</span> <span m="4523890">clusters</span> <span m="4524520">were</span>
  <span m="4524670">consistent</span> <span m="4525360">across</span> <span m="4525690">two</span>
  <span m="4525960">very</span> <span m="4526200">different</span> <span m="4526440">populations</span>
  <span m="4527010">gave</span> <span m="4527250">the</span> <span m="4527340">authors</span>
  <span m="4527670">confidence</span> <span m="4528180">that</span> <span m="4528300">there</span>
  <span m="4528420">might</span> <span m="4528600">be</span> <span m="4528690">something</span>
  <span m="4528990">real</span> <span m="4529290">here.</span> <span m="4530160">And</span>
  <span m="4530250">then</span> <span m="4530340">they</span> <span m="4530460">went</span>
  <span m="4530670">and they</span> <span m="4530800">explored</span> <span m="4531240">that</span>
  <span m="4531390">third</span> <span m="4531840">population,</span> <span m="4532410">where</span>
  <span m="4532500">they</span> <span m="4532590">had</span> <span m="4532710">longitudinal</span>
  <span m="4533400">data.</span> <span m="4534900">And</span> <span m="4534990">that</span>
  <span m="4535110">third</span> <span m="4535290">population</span> <span m="4535680">they</span>
  <span m="4535770">were</span> <span m="4535860">then</span> <span m="4536220">using</span>
  <span m="4536610">to</span> <span m="4536730">ask,</span> <span m="4537870">does</span>
  <span m="4538140">it</span> <span m="4538290">not--</span> <span m="4538620">so</span>
  <span m="4538770">up</span> <span m="4538920">until</span> <span m="4539160">now,</span>
  <span m="4539440">we've</span> <span m="4539520">only</span> <span m="4539790">used</span>
  <span m="4540000">baseline</span> <span m="4540480">information.</span></p><p><span
  m="4541550">But</span> <span m="4541680">now</span> <span m="4541830">we're</span>
  <span m="4541920">going</span> <span m="4542030">to</span> <span m="4542130">ask</span>
  <span m="4542340">the</span> <span m="4542430">following</span> <span m="4542730">question.</span>
  <span m="4543370">If</span> <span m="4543450">we</span> <span m="4543570">took</span>
  <span m="4543870">the</span> <span m="4543990">baseline</span> <span m="4545010">data</span>
  <span m="4547090">from</span> <span m="4547530">those</span> <span m="4547680">68</span>
  <span m="4548160">patients</span> <span m="4549060">and</span> <span m="4549200">we
  were</span> <span m="4549270">to</span> <span m="4549420">separate</span> <span
  m="4549870">them</span> <span m="4551556">into</span> <span m="4552260">three</span>
  <span m="4552630">different</span> <span m="4552960">clusters</span> <span m="4553890">based</span>
  <span m="4554370">on</span> <span m="4554550">the</span> <span m="4554670">characterizations</span>
  <span m="4555600">found</span> <span m="4555990">in</span> <span m="4556050">the</span>
  <span m="4556140">other</span> <span m="4556410">two</span> <span m="4556620">data</span>
  <span m="4556910">sets,</span> <span m="4558120">and</span> <span m="4558240">then</span>
  <span m="4558360">if</span> <span m="4558450">we were to</span> <span m="4558630">look</span>
  <span m="4558810">at</span> <span m="4558930">long-term</span> <span m="4559680">outcomes</span>
  <span m="4560250">for</span> <span m="4560370">each</span> <span m="4560520">cluster,</span>
  <span m="4561540">would</span> <span m="4561840">they</span> <span m="4562020">be</span>
  <span m="4562170">different</span> <span m="4562650">across</span> <span m="4562950">the</span>
  <span m="4563040">clusters?</span> <span m="4564010">And</span> <span m="4564150">in</span>
  <span m="4564210">particular,</span> <span m="4565150">here</span> <span m="4565560">we</span>
  <span m="4565890">actually</span> <span m="4566310">looked</span> <span m="4566580">at</span>
  <span m="4566700">not</span> <span m="4566940">just</span> <span m="4567360">predicting</span>
  <span m="4567880">a</span> <span m="4567960">progression,</span> <span m="4568410">but
  we're</span> <span m="4568640">also</span> <span m="4568710">looking</span> <span
  m="4568890">at</span> <span m="4568950">prediction--</span> <span m="4569820">we're</span>
  <span m="4569970">looking</span> <span m="4570180">at</span> <span m="4570270">differences</span>
  <span m="4570690">in</span> <span m="4570780">treatment</span> <span m="4571170">response.</span>
  <span m="4572190">Because</span> <span m="4572460">this</span> <span m="4572640">was</span>
  <span m="4572790">a</span> <span m="4572850">randomized-control</span> <span m="4573570">trial.</span></p><p><span
  m="4574610">And</span> <span m="4574710">so</span> <span m="4574810">there are</span>
  <span m="4574910">going</span> <span m="4575030">to</span> <span m="4575140">be</span>
  <span m="4575190">two</span> <span m="4575510">arms</span> <span m="4575880">here,</span>
  <span m="4576480">what's</span> <span m="4576660">called</span> <span m="4576840">the</span>
  <span m="4576930">clinical</span> <span m="4577500">arm,</span> <span m="4577950">which</span>
  <span m="4578220">is</span> <span m="4578490">the</span> <span m="4578730">standard</span>
  <span m="4579330">clinical</span> <span m="4579660">care,</span> <span m="4580420">and
  what's</span> <span m="4580580">called</span> <span m="4580760">the</span> <span
  m="4580860">sputum</span> <span m="4581340">arm,</span> <span m="4582000">which</span>
  <span m="4583260">consists</span> <span m="4583800">of</span> <span m="4583890">doing</span>
  <span m="4584100">regular</span> <span m="4584430">monitoring</span> <span m="4585150">of</span>
  <span m="4585270">the airway</span> <span m="4585840">inflammation,</span> <span
  m="4587010">and</span> <span m="4587130">then</span> <span m="4587460">tight</span>
  <span m="4587760">trading</span> <span m="4588090">steroid</span> <span m="4588480">therapy</span>
  <span m="4588990">in</span> <span m="4589080">order</span> <span m="4589200">to</span>
  <span m="4589320">maintain</span> <span m="4589860">normal</span> <span m="4590690">eosinophil</span>
  <span m="4591540">counts.</span> <span m="4592710">And</span> <span m="4593100">so</span>
  <span m="4593685">this</span> <span m="4594120">is</span> <span m="4594180">comparing</span>
  <span m="4594480">two</span> <span m="4594630">different</span> <span m="4594900">treatment</span>
  <span m="4595290">strategies.</span> <span m="4596550">And</span> <span m="4596640">the</span>
  <span m="4596700">question</span> <span m="4597120">is,</span> <span m="4598210">do</span>
  <span m="4598350">these</span> <span m="4598530">two</span> <span m="4598680">treatment</span>
  <span m="4598950">strategies</span> <span m="4599520">result</span> <span m="4600180">in</span>
  <span m="4601080">differential</span> <span m="4601680">outcomes?</span></p><p><span
  m="4603460">So</span> <span m="4603510">when</span> <span m="4603660">the</span>
  <span m="4603720">clinical</span> <span m="4604050">trial</span> <span m="4604350">was</span>
  <span m="4604500">originally</span> <span m="4605040">performed</span> <span m="4605880">and</span>
  <span m="4606000">they</span> <span m="4606120">computed</span> <span m="4606600">the</span>
  <span m="4606780">average</span> <span m="4607380">treatment</span> <span m="4607770">effect,</span>
  <span m="4608250">which,</span> <span m="4608460">by</span> <span m="4608610">the</span>
  <span m="4608670">way,</span> <span m="4608820">because</span> <span m="4609330">the</span>
  <span m="4609400">RCT</span> <span m="4610020">was</span> <span m="4610140">particularly</span>
  <span m="4610680">simple--</span> <span m="4611140">you</span> <span m="4611240">just</span>
  <span m="4611370">averaged</span> <span m="4611940">outcomes</span> <span m="4612420">across</span>
  <span m="4612660">the</span> <span m="4612720">two</span> <span m="4612930">arms--</span>
  <span m="4614370">they</span> <span m="4614520">found</span> <span m="4614850">that</span>
  <span m="4614970">there</span> <span m="4615060">was</span> <span m="4615210">no</span>
  <span m="4615540">difference</span> <span m="4616590">across</span> <span m="4616890">the</span>
  <span m="4616950">two</span> <span m="4617160">arms.</span> <span m="4617560">So</span>
  <span m="4617580">there</span> <span m="4617670">was</span> <span m="4617790">no</span>
  <span m="4617970">difference</span> <span m="4618330">in</span> <span m="4618390">outcomes</span>
  <span m="4618960">across</span> <span m="4619260">the</span> <span m="4619350">two</span>
  <span m="4619500">different</span> <span m="4619740">therapies.</span></p><p><span
  m="4621240">Now</span> <span m="4621480">what</span> <span m="4621600">these</span>
  <span m="4621750">authors</span> <span m="4622020">are</span> <span m="4622050">going</span>
  <span m="4622200">to</span> <span m="4622260">do</span> <span m="4622410">is</span>
  <span m="4622500">they're</span> <span m="4622590">going</span> <span m="4622740">to</span>
  <span m="4622830">rerun</span> <span m="4623310">the</span> <span m="4623410">study.</span>
  <span m="4625890">And</span> <span m="4626190">they're</span> <span m="4626310">going</span>
  <span m="4626520">to</span> <span m="4626700">now,</span> <span m="4627240">instead</span>
  <span m="4627570">of</span> <span m="4627750">just</span> <span m="4628080">looking</span>
  <span m="4628500">at</span> <span m="4628620">the</span> <span m="4628740">average</span>
  <span m="4629000">treatment</span> <span m="4629250">effect</span> <span m="4629790">for</span>
  <span m="4629910">the</span> <span m="4630000">whole</span> <span m="4630240">population,</span>
  <span m="4631350">they're</span> <span m="4631470">going</span> <span m="4631740">to</span>
  <span m="4632070">use--</span> <span m="4632680">they're</span> <span m="4632730">going</span>
  <span m="4632850">to</span> <span m="4632910">look</span> <span m="4633030">at</span>
  <span m="4633120">the</span> <span m="4633210">average</span> <span m="4633490">treatment</span>
  <span m="4635130">each</span> <span m="4635370">of</span> <span m="4635430">the</span>
  <span m="4635520">clusters</span> <span m="4636090">by</span> <span m="4636330">themselves.</span>
  <span m="4638280">And</span> <span m="4638370">the</span> <span m="4638460">hope</span>
  <span m="4638760">there</span> <span m="4639150">is</span> <span m="4639360">that</span>
  <span m="4639510">one</span> <span m="4639720">might</span> <span m="4639870">be</span>
  <span m="4639960">able</span> <span m="4640140">to</span> <span m="4640770">see</span>
  <span m="4641100">now</span> <span m="4641370">a</span> <span m="4641430">difference,</span>
  <span m="4641940">maybe</span> <span m="4642230">that</span> <span m="4642400">there</span>
  <span m="4642600">was</span> <span m="4642750">heterogeneous</span> <span m="4643035">treatment</span>
  <span m="4643550">response</span> <span m="4644040">and</span> <span m="4644130">sometimes</span>
  <span m="4644570">that</span> <span m="4644640">therapy</span> <span m="4645000">worked</span>
  <span m="4645210">for</span> <span m="4645300">some</span> <span m="4645480">people</span>
  <span m="4645720">and not</span> <span m="4645870">for</span> <span m="4646020">others.</span></p><p><span
  m="4648760">And</span> <span m="4648810">these</span> <span m="4648970">were</span>
  <span m="4649070">the</span> <span m="4649140">results.</span> <span m="4649950">So</span>
  <span m="4650030">indeed,</span> <span m="4650780">across</span> <span m="4651140">these</span>
  <span m="4651350">three</span> <span m="4651530">clusters,</span> <span m="4652490">we</span>
  <span m="4652670">see</span> <span m="4652940">actually</span> <span m="4653540">a</span>
  <span m="4653600">very</span> <span m="4654110">big</span> <span m="4654350">difference.</span>
  <span m="4655170">So</span> <span m="4656690">if</span> <span m="4656810">you</span>
  <span m="4656870">look</span> <span m="4657020">here,</span> <span m="4657330">for</span>
  <span m="4657430">example,</span> <span m="4657780">the</span> <span m="4657880">number</span>
  <span m="4658100">of</span> <span m="4658220">commenced</span> <span m="4658970">on</span>
  <span m="4659450">oral</span> <span m="4659750">corticosteroids,</span> <span m="4660780">which</span>
  <span m="4660990">is</span> <span m="4661100">a</span> <span m="4661190">measure</span>
  <span m="4663950">of</span> <span m="4664330">an</span> <span m="4664550">outcome--</span>
  <span m="4665180">so</span> <span m="4665920">you</span> <span m="4666020">might</span>
  <span m="4666170">want</span> <span m="4666350">this to--</span> <span m="4666580">I</span>
  <span m="4666650">can't</span> <span m="4666860">remember,</span> <span m="4666980">small</span>
  <span m="4667250">or</span> <span m="4667340">large.</span> <span m="4667910">But</span>
  <span m="4668060">there was</span> <span m="4668210">a</span> <span m="4668270">big</span>
  <span m="4668450">difference</span> <span m="4668780">between</span> <span m="4669080">these</span>
  <span m="4669260">two</span> <span m="4669410">clusters.</span> <span m="4670850">And</span>
  <span m="4670970">this</span> <span m="4671180">cluster,</span> <span m="4673740">the</span>
  <span m="4674090">number</span> <span m="4674510">commenced</span> <span m="4675770">under</span>
  <span m="4676220">the</span> <span m="4676370">first</span> <span m="4676730">arm</span>
  <span m="4676940">is</span> <span m="4677090">two;</span> <span m="4677970">in</span>
  <span m="4678230">this</span> <span m="4678380">other</span> <span m="4678560">cluster</span>
  <span m="4678890">for</span> <span m="4679010">patients</span> <span m="4679370">who</span>
  <span m="4679460">got</span> <span m="4679610">the</span> <span m="4679670">second</span>
  <span m="4680090">arm,</span> <span m="4680450">nine;</span> <span m="4681160">and</span>
  <span m="4681290">exactly</span> <span m="4682010">the</span> <span m="4682130">opposite</span>
  <span m="4683135">for</span> <span m="4683540">this</span> <span m="4683750">third</span>
  <span m="4684020">cluster.</span> <span m="4685230">The</span> <span m="4685330">first</span>
  <span m="4685550">cluster,</span> <span m="4685940">by</span> <span m="4686030">the</span>
  <span m="4686120">way,</span> <span m="4686300">had</span> <span m="4686450">only</span>
  <span m="4686630">three</span> <span m="4686840">patients</span> <span m="4687200">in</span>
  <span m="4687290">it.</span> <span m="4687410">So</span> <span m="4687470">I'm</span>
  <span m="4687530">not</span> <span m="4687620">going</span> <span m="4687740">to</span>
  <span m="4687800">make</span> <span m="4687950">any</span> <span m="4688070">comment</span>
  <span m="4688400">about</span> <span m="4688610">it.</span></p><p><span m="4690410">Now,</span>
  <span m="4690830">since</span> <span m="4691130">these</span> <span m="4691330">go</span>
  <span m="4691510">in</span> <span m="4691640">completely</span> <span m="4692480">opposite</span>
  <span m="4692960">directions,</span> <span m="4693690">it's</span> <span m="4693710">not</span>
  <span m="4693920">surprising</span> <span m="4694790">that</span> <span m="4694940">the</span>
  <span m="4695060">average</span> <span m="4695420">treatment</span> <span m="4695660">effect</span>
  <span m="4695900">across</span> <span m="4696140">the</span> <span m="4696230">whole</span>
  <span m="4696410">population</span> <span m="4696980">was</span> <span m="4697550">zero.</span>
  <span m="4698750">But</span> <span m="4698840">what</span> <span m="4698930">we're</span>
  <span m="4699050">seeing</span> <span m="4699380">now</span> <span m="4699620">is</span>
  <span m="4699770">that,</span> <span m="4700050">in</span> <span m="4700150">fact,</span>
  <span m="4700410">there</span> <span m="4700510">is</span> <span m="4700550">a</span>
  <span m="4700610">difference.</span> <span m="4701240">And</span> <span m="4701330">so</span>
  <span m="4701510">it's</span> <span m="4701990">possible</span> <span m="4702440">that</span>
  <span m="4703010">the</span> <span m="4703100">therapy</span> <span m="4703580">is</span>
  <span m="4703730">actually</span> <span m="4704090">effective</span> <span m="4704720">but</span>
  <span m="4704870">just</span> <span m="4705140">for</span> <span m="4705350">a</span>
  <span m="4705410">smaller</span> <span m="4705950">number</span> <span m="4706250">of</span>
  <span m="4706310">people.</span></p><p><span m="4707720">Now,</span> <span m="4707840">this</span>
  <span m="4708020">study</span> <span m="4708260">would've</span> <span m="4708420">never</span>
  <span m="4708680">been</span> <span m="4708860">possible</span> <span m="4710750">had</span>
  <span m="4711080">we</span> <span m="4711230">not</span> <span m="4711590">done</span>
  <span m="4711890">this</span> <span m="4712070">clustering</span> <span m="4712610">beforehand.</span>
  <span m="4713570">Because</span> <span m="4713870">it</span> <span m="4713930">has</span>
  <span m="4714110">so</span> <span m="4714440">few</span> <span m="4714620">patients,</span>
  <span m="4715040">only</span> <span m="4715220">68</span> <span m="4715640">patients.</span>
  <span m="4716360">If</span> <span m="4716510">you</span> <span m="4716600">attempted</span>
  <span m="4716990">to</span> <span m="4717170">both</span> <span m="4717500">search</span>
  <span m="4717980">for</span> <span m="4718370">the</span> <span m="4718510">clustering</span>
  <span m="4719090">at</span> <span m="4719180">the</span> <span m="4719240">same</span>
  <span m="4719540">time</span> <span m="4719870">as,</span> <span m="4720220">let's
  say,</span> <span m="4720470">find</span> <span m="4720740">clusters</span> <span
  m="4721250">to</span> <span m="4721400">differentiate</span> <span m="4722090">outcomes,</span>
  <span m="4723455">you</span> <span m="4723920">would</span> <span m="4724040">overfit</span>
  <span m="4724490">the</span> <span m="4724580">data</span> <span m="4724910">very</span>
  <span m="4725150">quickly.</span> <span m="4726210">So</span> <span m="4726290">it's</span>
  <span m="4726380">precisely</span> <span m="4726800">because</span> <span m="4727190">we</span>
  <span m="4727310">did</span> <span m="4727400">this</span> <span m="4727520">unsupervised</span>
  <span m="4728120">sub-typing</span> <span m="4728690">first,</span> <span m="4729620">and</span>
  <span m="4729710">then</span> <span m="4729890">use</span> <span m="4730240">the</span>
  <span m="4730370">labels</span> <span m="4731210">not</span> <span m="4731510">for</span>
  <span m="4731780">searching</span> <span m="4732290">for</span> <span m="4732410">the</span>
  <span m="4732470">subtypes</span> <span m="4732910">but</span> <span m="4733000">only</span>
  <span m="4733160">for</span> <span m="4733300">evaluating</span> <span m="4733700">the</span>
  <span m="4733760">subtypes,</span> <span m="4734450">that</span> <span m="4734670">we're</span>
  <span m="4734840">actually</span> <span m="4735080">able</span> <span m="4735260">to</span>
  <span m="4735320">do</span> <span m="4735410">something</span> <span m="4735620">interesting</span>
  <span m="4736010">here.</span></p><p><span m="4737200">So in</span> <span m="4737450">summary,</span>
  <span m="4737850">in today's</span> <span m="4738130">lecture,</span> <span m="4738340">I</span>
  <span m="4738440">talked</span> <span m="4738650">about</span> <span m="4738800">two</span>
  <span m="4738980">different</span> <span m="4739190">approaches,</span> <span m="4739730">a</span>
  <span m="4739790">supervised</span> <span m="4740360">approach</span> <span m="4740780">for</span>
  <span m="4740870">predicting</span> <span m="4741230">future</span> <span m="4741500">disease</span>
  <span m="4741710">status</span> <span m="4742140">and an</span> <span m="4742570">unsupervised</span>
  <span m="4743060">approach.</span> <span m="4744350">And</span> <span m="4744980">there</span>
  <span m="4745130">were</span> <span m="4745460">a</span> <span m="4745520">few</span>
  <span m="4745850">major</span> <span m="4746150">limitations</span> <span m="4746780">that</span>
  <span m="4746900">I</span> <span m="4746960">want to</span> <span m="4747080">emphasize</span>
  <span m="4747620">that</span> <span m="4747710">we'll</span> <span m="4747830">return</span>
  <span m="4748100">to</span> <span m="4748370">in</span> <span m="4748520">the</span>
  <span m="4748610">next</span> <span m="4748820">lecture</span> <span m="4749150">and</span>
  <span m="4749240">try</span> <span m="4749420">to</span> <span m="4749540">address.</span>
  <span m="4751100">The</span> <span m="4751160">first</span> <span m="4751430">major</span>
  <span m="4751670">limitation</span> <span m="4752180">is</span> <span m="4752240">that</span>
  <span m="4752360">none</span> <span m="4752510">of</span> <span m="4752570">these</span>
  <span m="4752720">approaches</span> <span m="4753140">differentiated</span> <span
  m="4753680">between</span> <span m="4754010">disease</span> <span m="4754340">stage</span>
  <span m="4755210">and</span> <span m="4755390">subtype.</span></p><p><span m="4757310">In</span>
  <span m="4757490">both</span> <span m="4759518">of</span> <span m="4759920">the</span>
  <span m="4760040">two</span> <span m="4760220">approaches,</span> <span m="4761150">we</span>
  <span m="4761270">assumed</span> <span m="4761870">that</span> <span m="4762050">there</span>
  <span m="4762140">were</span> <span m="4762240">some</span> <span m="4762410">amount</span>
  <span m="4762620">of</span> <span m="4762710">alignment</span> <span m="4763340">of</span>
  <span m="4763430">patients</span> <span m="4763810">at</span> <span m="4763910">baseline.</span>
  <span m="4764610">For</span> <span m="4764630">example,</span> <span m="4766380">here</span>
  <span m="4767030">we</span> <span m="4767120">assume</span> <span m="4767450">that</span>
  <span m="4767570">the</span> <span m="4767660">patients</span> <span m="4768080">at</span>
  <span m="4768200">time</span> <span m="4768550">zero</span> <span m="4768920">were</span>
  <span m="4769100">somewhat</span> <span m="4769400">similar</span> <span m="4769700">to</span>
  <span m="4769760">another.</span> <span m="4770130">For</span> <span m="4770230">example,</span>
  <span m="4770550">they</span> <span m="4770650">might</span> <span m="4770690">have</span>
  <span m="4770780">been</span> <span m="4771020">newly</span> <span m="4771440">diagnosed</span>
  <span m="4771860">with</span> <span m="4771980">Alzheimer's</span> <span m="4772490">at</span>
  <span m="4772610">that</span> <span m="4772760">point</span> <span m="4772890">in</span>
  <span m="4773000">time.</span></p><p><span m="4774350">But</span> <span m="4774560">often</span>
  <span m="4774980">we</span> <span m="4775130">have</span> <span m="4775250">a</span>
  <span m="4775310">data</span> <span m="4775510">set</span> <span m="4775730">where</span>
  <span m="4775850">we</span> <span m="4775940">have</span> <span m="4776180">no</span>
  <span m="4776390">natural</span> <span m="4776930">alignment</span> <span m="4777470">of</span>
  <span m="4777560">patients</span> <span m="4777980">in</span> <span m="4778070">terms</span>
  <span m="4778280">of</span> <span m="4778340">disease</span> <span m="4779450">stage.</span>
  <span m="4780780">And</span> <span m="4780980">if</span> <span m="4781070">we</span>
  <span m="4781160">attempted</span> <span m="4781490">to</span> <span m="4781580">do</span>
  <span m="4781700">some</span> <span m="4781850">type</span> <span m="4782030">of</span>
  <span m="4782090">clustering</span> <span m="4782660">like</span> <span m="4782870">I</span>
  <span m="4782930">did</span> <span m="4783080">in</span> <span m="4783140">this</span>
  <span m="4783290">last</span> <span m="4783560">example,</span> <span m="4784400">what</span>
  <span m="4784580">you</span> <span m="4784700">would</span> <span m="4784880">get</span>
  <span m="4785240">out,</span> <span m="4785660">naively,</span> <span m="4786380">would</span>
  <span m="4786560">be</span> <span m="4787160">one</span> <span m="4787490">cluster</span>
  <span m="4787940">for</span> <span m="4788150">disease</span> <span m="4788510">stage.</span>
  <span m="4789830">So</span> <span m="4789980">patients</span> <span m="4790340">who</span>
  <span m="4790420">are</span> <span m="4790460">very</span> <span m="4790700">early</span>
  <span m="4791040">in their</span> <span m="4791150">disease</span> <span m="4791360">stage</span>
  <span m="4791720">might</span> <span m="4791900">look</span> <span m="4792020">very</span>
  <span m="4792200">different from</span> <span m="4792470">patients</span> <span
  m="4792740">who are</span> <span m="4792880">late</span> <span m="4793070">in</span>
  <span m="4793160">their</span> <span m="4793280">disease</span> <span m="4793490">stage.</span>
  <span m="4795350">And it will</span> <span m="4795590">completely</span> <span m="4796010">conflate</span>
  <span m="4796640">disease</span> <span m="4796970">stage</span> <span m="4797480">from</span>
  <span m="4797630">disease</span> <span m="4797900">subtype,</span> <span m="4798410">which</span>
  <span m="4798590">is</span> <span m="4798680">what</span> <span m="4798830">you</span>
  <span m="4798920">might</span> <span m="4799070">actually</span> <span m="4799370">want</span>
  <span m="4799550">to</span> <span m="4799610">discover.</span></p><p><span m="4801650">The</span>
  <span m="4801740">second</span> <span m="4802430">limitation</span> <span m="4802970">of</span>
  <span m="4803030">these</span> <span m="4803090">approaches</span> <span m="4803570">is</span>
  <span m="4803690">that</span> <span m="4803780">they</span> <span m="4803900">only</span>
  <span m="4804080">used</span> <span m="4804320">one</span> <span m="4804590">time</span>
  <span m="4804920">point</span> <span m="4805220">per</span> <span m="4805370">patient,</span>
  <span m="4806150">whereas</span> <span m="4806390">in</span> <span m="4806480">reality,</span>
  <span m="4808200">such</span> <span m="4808370">as</span> <span m="4808490">you</span>
  <span m="4808700">saw</span> <span m="4808970">here,</span> <span m="4809330">we</span>
  <span m="4809480">might</span> <span m="4809630">have</span> <span m="4809750">multiple</span>
  <span m="4810170">time</span> <span m="4810470">points.</span> <span m="4810740">And</span>
  <span m="4810830">we</span> <span m="4810890">might</span> <span m="4811100">want</span>
  <span m="4811280">to,</span> <span m="4811470">for</span> <span m="4811570">example,</span>
  <span m="4811960">do</span> <span m="4812030">clustering</span> <span m="4812540">using</span>
  <span m="4812810">multiple</span> <span m="4813110">time</span> <span m="4813320">points.</span>
  <span m="4813890">Or</span> <span m="4814020">we</span> <span m="4814100">might</span>
  <span m="4814370">want</span> <span m="4814580">to</span> <span m="4814640">use</span>
  <span m="4814850">multiple</span> <span m="4815180">time</span> <span m="4815450">points</span>
  <span m="4815840">to</span> <span m="4816020">understand</span> <span m="4816350">something</span>
  <span m="4816590">about</span> <span m="4816770">disease</span> <span m="4817010">progression.</span></p><p><span
  m="4819740">The</span> <span m="4819830">third</span> <span m="4820100">limitation</span>
  <span m="4820700">is</span> <span m="4820820">that</span> <span m="4821420">they</span>
  <span m="4821600">assume</span> <span m="4821920">that</span> <span m="4822010">there</span>
  <span m="4822100">is</span> <span m="4822170">a</span> <span m="4822230">single</span>
  <span m="4822590">factor,</span> <span m="4823070">let's</span> <span m="4823250">say</span>
  <span m="4823400">disease</span> <span m="4823640">subtype,</span> <span m="4824150">that</span>
  <span m="4824270">explained</span> <span m="4824750">all</span> <span m="4825050">variation</span>
  <span m="4825740">in</span> <span m="4825810">the</span> <span m="4825860">patients.</span>
  <span m="4826490">In</span> <span m="4826610">fact,</span> <span m="4826980">there</span>
  <span m="4827000">might</span> <span m="4827120">be</span> <span m="4827240">other</span>
  <span m="4827600">factors,</span> <span m="4828140">patient-specific</span> <span
  m="4828830">factors,</span> <span m="4829310">that</span> <span m="4829430">one</span>
  <span m="4829580">would</span> <span m="4829670">like</span> <span m="4829820">to</span>
  <span m="4830000">use</span> <span m="4830450">in</span> <span m="4830600">your</span>
  <span m="4830720">noise</span> <span m="4830990">model.</span> <span m="4831960">When
  you</span> <span m="4832040">use</span> <span m="4832210">an</span> <span m="4832590">algorithm</span>
  <span m="4833000">like</span> <span m="4833120">K-means</span> <span m="4833660">for</span>
  <span m="4833780">clustering,</span> <span m="4834300">it</span> <span m="4834710">presents</span>
  <span m="4835130">no</span> <span m="4835430">opportunity</span> <span m="4836060">for</span>
  <span m="4836180">doing</span> <span m="4836420">that,</span> <span m="4836570">because</span>
  <span m="4836870">it</span> <span m="4836930">has</span> <span m="4837080">such</span>
  <span m="4837260">a</span> <span m="4837320">naive</span> <span m="4837650">distance</span>
  <span m="4838070">function.</span></p><p><span m="4839150">And</span> <span m="4839270">so</span>
  <span m="4839450">in</span> <span m="4839510">next</span> <span m="4839780">week's</span>
  <span m="4839990">lecture,</span> <span m="4840420">we're</span> <span m="4840440">going</span>
  <span m="4840650">to</span> <span m="4840740">move</span> <span m="4841040">in to</span>
  <span m="4841220">start</span> <span m="4841430">talking</span> <span m="4841670">a</span>
  <span m="4841730">probabilistic</span> <span m="4842390">modeling</span> <span m="4842840">approaches</span>
  <span m="4843290">to</span> <span m="4843470">these</span> <span m="4843710">problems,</span>
  <span m="4844580">which</span> <span m="4844790">will</span> <span m="4844880">give</span>
  <span m="4845180">us</span> <span m="4845330">a</span> <span m="4845390">very</span>
  <span m="4845780">natural</span> <span m="4846200">way</span> <span m="4846680">of</span>
  <span m="4846890">characterizing</span> <span m="4847760">variation</span> <span
  m="4848240">along</span> <span m="4848480">other</span> <span m="4848660">axes.</span>
  <span m="4850010">And</span> <span m="4850130">finally,</span> <span m="4850610">a</span>
  <span m="4850700">natural</span> <span m="4851000">question you</span> <span m="4851300">should</span>
  <span m="4851450">ask</span> <span m="4851720">is,</span> <span m="4851870">does</span>
  <span m="4851960">it</span> <span m="4852020">have</span> <span m="4852290">to</span>
  <span m="4852380">be</span> <span m="4852680">unsupervised</span> <span m="4853340">or</span>
  <span m="4853400">supervised?</span> <span m="4853970">Or</span> <span m="4854060">is</span>
  <span m="4854120">there</span> <span m="4854270">a</span> <span m="4854300">way</span>
  <span m="4854420">to</span> <span m="4854540">combine</span> <span m="4854900">those</span>
  <span m="4855010">two</span> <span m="4855120">approaches.</span></p><p><span m="4855750">All</span>
  <span m="4856130">right.</span> <span m="4856220">We'll</span> <span m="4856340">get</span>
  <span m="4856460">back</span> <span m="4856580">to</span> <span m="4856690">that</span>
  <span m="4856790">on Tuesday.</span> <span m="4857190">That's all.</span></p>
type: course
uid: 77923ed984040ad58785a8ce650bca64

---
None