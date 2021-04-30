---
about_this_resource_text: '<p>Prof. Szolovits explains differential diagnosis, the
  distinguishing of a condition from others with similar features. He covers models
  of diagnostic reasoning: flow charts, card selection, naive Bayes, bipartite graphs,
  QMR DT, and reinforcement learning.</p> <p>Speaker: Peter Szolovits</p>             <p><a
  href="./resolveuid/e50b5bb5bb192ba6b6d995af8aad0597">Lecture 11: Machine Learning
  for Differential Diagnosis slides (PDF - 1.8MB)</a></p>'
course_id: 6-s897-machine-learning-for-healthcare-spring-2019
embedded_media:
- id: Video-YouTube-Stream
  media_location: VuKOW8d4KHw
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: Video-YouTube-Stream
  type: Video
  uid: bac9651d538ef9e1ae47c5942e3b1fe1
- id: Thumbnail-YouTube-JPG
  media_location: https://img.youtube.com/vi/VuKOW8d4KHw/default.jpg
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: Thumbnail-YouTube-JPG
  type: Thumbnail
  uid: af452b3333aa3d319a09a61c26d70f4a
- id: 3Play-3PlayYouTubeid-MP4
  media_location: VuKOW8d4KHw
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: 3Play-3Play YouTube id
  type: 3Play
  uid: baa396d1227b71aee1226dda3b8812d3
- id: VuKOW8d4KHw.srt
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-11-differential-diagnosis/VuKOW8d4KHw.srt
  title: 3play caption file
  type: null
  uid: 5870c03cef6d72d39c9592b392cebc0b
- id: VuKOW8d4KHw.pdf
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-11-differential-diagnosis/VuKOW8d4KHw.pdf
  title: 3play pdf file
  type: null
  uid: 8d422297e311ad166f86725339d03ebe
- id: Caption-3Play YouTube id-SRT
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: Caption-3Play YouTube id-SRT-English - US
  type: Caption
  uid: cca59569bece0a5259d7b478a3f6a6dd
- id: Transcript-3Play YouTube id-PDF
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: Transcript-3Play YouTube id-PDF-English - US
  type: Transcript
  uid: ea97376dc962b504cb7d67def4267134
- id: Video-InternetArchive-MP4
  media_location: https://archive.org/download/MIT6.S897S19/MIT6_S897S19_lec11_300k.mp4
  parent_uid: 7c1732890f7067b5e9d525f49e2010e5
  title: Video-Internet Archive-MP4
  type: Video
  uid: 388d3f119ca9ed9abd17691aa33acb8b
inline_embed_id: 45873018lecture11differentialdiagnosis6462050
layout: video
order_index: null
parent_uid: d85bdff15f958ff33b789712195880fb
related_resources_text: ''
short_url: lecture-11-differential-diagnosis
technical_location: https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-s897-machine-learning-for-healthcare-spring-2019/lecture-videos/lecture-11-differential-diagnosis
template_type: Tabbed
title: 'Lecture 11: Differential Diagnosis'
transcript: <p><span m="15730">PETER SZOLOVITS:</span> <span m="15920">OK.</span>
  <span m="16840">Today's</span> <span m="17260">topic</span> <span m="17710">is</span>
  <span m="17890">differential</span> <span m="18760">diagnosis.</span> <span m="20810">And</span>
  <span m="21250">so</span> <span m="21490">I'm</span> <span m="21640">just</span>
  <span m="21850">quoting</span> <span m="22300">Wikipedia</span> <span m="22990">here.</span>
  <span m="23230">Diagnosis</span> <span m="24070">is</span> <span m="24220">the</span>
  <span m="24370">identification</span> <span m="26020">of</span> <span m="26170">the</span>
  <span m="26290">nature</span> <span m="26770">and</span> <span m="26920">cause</span>
  <span m="27340">of</span> <span m="27460">a</span> <span m="27520">certain</span>
  <span m="27910">phenomenon.</span> <span m="29230">And</span> <span m="29410">differential</span>
  <span m="30070">diagnosis</span> <span m="31090">is</span> <span m="31450">the</span>
  <span m="31630">distinguishing</span> <span m="33070">of</span> <span m="33250">a</span>
  <span m="33370">particular</span> <span m="34090">disease</span> <span m="34630">or</span>
  <span m="34750">condition</span> <span m="35800">from</span> <span m="36130">others</span>
  <span m="36550">that</span> <span m="36730">present</span> <span m="37210">similar</span>
  <span m="37690">clinical</span> <span m="38170">features.</span></p><p><span m="39490">So</span>
  <span m="40030">doctors</span> <span m="40600">typically</span> <span m="41140">talk</span>
  <span m="41470">about</span> <span m="41770">differential</span> <span m="42370">diagnosis</span>
  <span m="43720">when</span> <span m="43960">they're</span> <span m="44170">faced</span>
  <span m="44650">with</span> <span m="44900">a</span> <span m="44980">patient</span>
  <span m="46090">and</span> <span m="46390">they</span> <span m="46600">make</span>
  <span m="46930">list</span> <span m="47440">of</span> <span m="47770">what</span>
  <span m="48010">are</span> <span m="48130">the</span> <span m="48280">things</span>
  <span m="48670">that</span> <span m="49090">might</span> <span m="49510">be</span>
  <span m="49720">wrong</span> <span m="50050">with</span> <span m="50260">this</span>
  <span m="50440">patient.</span> <span m="51650">And</span> <span m="51700">then</span>
  <span m="51910">they</span> <span m="52060">go</span> <span m="52270">through</span>
  <span m="52510">the</span> <span m="52630">process</span> <span m="53200">of</span>
  <span m="53320">trying</span> <span m="53590">to</span> <span m="53710">figure</span>
  <span m="54070">out</span> <span m="54670">which</span> <span m="54910">one</span>
  <span m="55120">it</span> <span m="55270">actually</span> <span m="55780">is.</span>
  <span m="56560">So</span> <span m="56740">that's</span> <span m="56980">what</span>
  <span m="57160">we're</span> <span m="57310">going</span> <span m="57460">to</span>
  <span m="57520">focus</span> <span m="58000">on</span> <span m="58150">today.</span></p><p><span
  m="59900">Now,</span> <span m="60250">just</span> <span m="60520">to</span> <span
  m="60640">scare</span> <span m="61030">you,</span> <span m="62290">here's</span>
  <span m="62830">a</span> <span m="63070">lovely</span> <span m="64420">model</span>
  <span m="65530">of</span> <span m="66520">human</span> <span m="66880">circulatory</span>
  <span m="67750">physiology.</span> <span m="69400">So</span> <span m="69640">this</span>
  <span m="69970">is</span> <span m="70270">from</span> <span m="70690">Guyton's</span>
  <span m="71680">textbook</span> <span m="72280">of</span> <span m="73300">cardiology.</span>
  <span m="75700">And</span> <span m="77470">I'm</span> <span m="77800">not</span>
  <span m="77950">going</span> <span m="78100">to</span> <span m="78160">hold</span>
  <span m="78430">you</span> <span m="78550">responsible</span> <span m="79390">for</span>
  <span m="79930">all</span> <span m="80170">of</span> <span m="80350">the</span>
  <span m="80710">details</span> <span m="81760">of</span> <span m="81910">this</span>
  <span m="82150">model,</span> <span m="83470">but</span> <span m="83710">it's</span>
  <span m="83890">interesting,</span> <span m="84520">because</span> <span m="85090">this</span>
  <span m="85510">is,</span> <span m="86410">at</span> <span m="86590">least</span>
  <span m="87130">as</span> <span m="87400">of</span> <span m="87610">maybe</span>
  <span m="87970">20</span> <span m="88330">years</span> <span m="88660">ago,</span>
  <span m="89020">the</span> <span m="89170">state</span> <span m="89500">of</span>
  <span m="89620">the</span> <span m="89800">art</span> <span m="90640">of</span>
  <span m="90820">how</span> <span m="91120">people</span> <span m="91570">understood</span>
  <span m="92200">what</span> <span m="92410">happens</span> <span m="92890">in</span>
  <span m="93010">the</span> <span m="93100">circulatory</span> <span m="93880">system.</span>
  <span m="95120">And</span> <span m="95200">it</span> <span m="95320">has</span>
  <span m="95590">various</span> <span m="96790">control</span> <span m="97510">inputs</span>
  <span m="98590">that</span> <span m="98890">determine</span> <span m="99520">things</span>
  <span m="99910">like</span> <span m="101260">how</span> <span m="101590">your</span>
  <span m="102190">hormone</span> <span m="102700">levels</span> <span m="103240">change</span>
  <span m="104200">various</span> <span m="104710">aspects</span> <span m="105310">of</span>
  <span m="105430">the</span> <span m="105730">cardiovascular</span> <span m="106690">system</span>
  <span m="107800">and</span> <span m="108100">how</span> <span m="108490">the</span>
  <span m="109060">interactions</span> <span m="110020">between</span> <span m="110440">different</span>
  <span m="110800">components</span> <span m="112060">of</span> <span m="112210">the</span>
  <span m="113200">cardiovascular</span> <span m="114130">system</span> <span m="115060">affect</span>
  <span m="115480">each</span> <span m="115720">other.</span></p><p><span m="117220">And</span>
  <span m="117400">so</span> <span m="117610">in</span> <span m="117730">principle,</span>
  <span m="119150">if</span> <span m="119290">I</span> <span m="119440">could</span>
  <span m="119650">tune</span> <span m="120190">this</span> <span m="120490">model</span>
  <span m="121000">to</span> <span m="121240">me,</span> <span m="122620">then</span>
  <span m="123010">I</span> <span m="123190">could</span> <span m="123430">make</span>
  <span m="123790">all</span> <span m="123940">kinds</span> <span m="124300">of</span>
  <span m="124780">pretty</span> <span m="125020">good</span> <span m="125200">predictions</span>
  <span m="126100">that</span> <span m="126340">say</span> <span m="127300">if</span>
  <span m="127570">I</span> <span m="128320">increase</span> <span m="128860">my</span>
  <span m="129160">systemic</span> <span m="129759">vascular</span> <span m="130300">resistance,</span>
  <span m="131560">then</span> <span m="131920">here's</span> <span m="132340">what's</span>
  <span m="132640">going</span> <span m="132760">to</span> <span m="132880">happen</span>
  <span m="133510">as</span> <span m="133840">the</span> <span m="133930">rest</span>
  <span m="134230">of</span> <span m="134320">the</span> <span m="134470">system</span>
  <span m="134920">adjusts.</span> <span m="136570">And</span> <span m="136960">if</span>
  <span m="137290">I</span> <span m="137800">get</span> <span m="138040">a</span>
  <span m="138100">blockage</span> <span m="139000">in</span> <span m="139150">a</span>
  <span m="139210">coronary</span> <span m="139840">artery,</span> <span m="140590">then</span>
  <span m="140980">here's</span> <span m="141370">what's</span> <span m="141610">going</span>
  <span m="141750">to</span> <span m="141850">happen</span> <span m="142750">to</span>
  <span m="142900">my</span> <span m="143110">cardiac</span> <span m="143710">output</span>
  <span m="144340">and</span> <span m="145060">various</span> <span m="145570">other</span>
  <span m="145810">things.</span></p><p><span m="147080">So</span> <span m="147220">this</span>
  <span m="147450">would</span> <span m="147550">be</span> <span m="147700">terrific.</span>
  <span m="148610">And</span> <span m="148720">if</span> <span m="148930">we</span>
  <span m="149110">had</span> <span m="149470">this</span> <span m="149740">kind</span>
  <span m="150070">of</span> <span m="150160">model</span> <span m="151120">for</span>
  <span m="151930">not</span> <span m="152170">just</span> <span m="152410">the</span>
  <span m="152530">cardiovascular</span> <span m="153460">system,</span> <span m="154010">but</span>
  <span m="154090">the</span> <span m="154240">entire</span> <span m="154690">body,</span>
  <span m="155860">then</span> <span m="156130">we'd</span> <span m="156310">say,</span>
  <span m="156610">OK,</span> <span m="156970">we've</span> <span m="157210">solved</span>
  <span m="157600">medicine.</span> <span m="159550">Well,</span> <span m="160030">we</span>
  <span m="160210">don't</span> <span m="160480">have</span> <span m="160720">this</span>
  <span m="160960">kind</span> <span m="161230">of</span> <span m="161320">model</span>
  <span m="162460">for</span> <span m="163030">most</span> <span m="163300">systems.</span>
  <span m="164500">And</span> <span m="164680">also,</span> <span m="165070">there's</span>
  <span m="165340">this</span> <span m="165580">minor</span> <span m="165970">problem</span>
  <span m="167230">that</span> <span m="168850">if</span> <span m="169060">I</span>
  <span m="169210">give</span> <span m="169450">you</span> <span m="169570">this</span>
  <span m="169810">model</span> <span m="170260">and</span> <span m="170380">say,</span>
  <span m="170680">&quot;How</span> <span m="170890">does</span> <span m="171100">this</span>
  <span m="171310">relate</span> <span m="172210">to</span> <span m="172420">a</span>
  <span m="172570">particular</span> <span m="173230">patient?&quot;,</span> <span
  m="175030">how</span> <span m="175210">would</span> <span m="175390">you</span>
  <span m="175510">figure</span> <span m="175840">that</span> <span m="176080">out?</span>
  <span m="177250">This</span> <span m="177520">has</span> <span m="177760">hundreds</span>
  <span m="178240">of</span> <span m="178360">differential</span> <span m="178990">equations</span>
  <span m="179740">that</span> <span m="179920">are</span> <span m="180040">being</span>
  <span m="180340">represented</span> <span m="181000">by</span> <span m="181210">this</span>
  <span m="181420">diagram.</span> <span m="182590">And</span> <span m="182770">they</span>
  <span m="182920">have</span> <span m="183160">many</span> <span m="183520">hundreds</span>
  <span m="184030">of</span> <span m="184150">parameters.</span></p><p><span m="185830">And</span>
  <span m="186010">so</span> <span m="187810">we</span> <span m="187990">were</span>
  <span m="188140">joking</span> <span m="188710">when</span> <span m="188950">we</span>
  <span m="189100">started</span> <span m="189550">working</span> <span m="190450">with</span>
  <span m="190780">this</span> <span m="190990">model</span> <span m="191920">that</span>
  <span m="192190">you'd</span> <span m="192490">really</span> <span m="192850">have</span>
  <span m="193090">to</span> <span m="193180">kill</span> <span m="193480">the</span>
  <span m="193600">patient</span> <span m="194230">in</span> <span m="194470">order</span>
  <span m="194800">to</span> <span m="195550">do</span> <span m="195820">enough</span>
  <span m="196210">measurements</span> <span m="197380">to</span> <span m="197530">be</span>
  <span m="197740">able</span> <span m="198610">to</span> <span m="199880">tune</span>
  <span m="200320">this</span> <span m="200590">model</span> <span m="201070">to</span>
  <span m="201280">their</span> <span m="201520">particular</span> <span m="202150">physiology.</span>
  <span m="203620">And</span> <span m="203770">of</span> <span m="203890">course,</span>
  <span m="204190">that's</span> <span m="204430">probably</span> <span m="204790">not</span>
  <span m="205240">a</span> <span m="205360">good</span> <span m="205720">practical</span>
  <span m="206560">approach.</span></p><p><span m="208030">We're</span> <span m="208240">getting</span>
  <span m="208570">a</span> <span m="208630">little</span> <span m="208930">better</span>
  <span m="209350">by</span> <span m="209620">developing</span> <span m="210700">more</span>
  <span m="211030">non-invasive</span> <span m="211990">ways</span> <span m="212920">of</span>
  <span m="213130">measuring</span> <span m="213670">these</span> <span m="213940">things.</span>
  <span m="216520">But</span> <span m="216910">that's</span> <span m="217210">moving</span>
  <span m="217630">along</span> <span m="217960">very</span> <span m="218200">slowly.</span>
  <span m="218830">And</span> <span m="219070">I</span> <span m="219190">don't</span>
  <span m="219400">expect</span> <span m="220390">that</span> <span m="221110">I</span>
  <span m="221470">or</span> <span m="221740">maybe</span> <span m="222130">even</span>
  <span m="222460">any</span> <span m="222700">of</span> <span m="222850">you</span>
  <span m="223030">will</span> <span m="223270">live</span> <span m="223540">long</span>
  <span m="223840">enough</span> <span m="224680">that</span> <span m="225250">sort</span>
  <span m="225520">of</span> <span m="225640">this</span> <span m="226240">approach</span>
  <span m="226780">to</span> <span m="227050">doing</span> <span m="227620">medical</span>
  <span m="228070">reasoning</span> <span m="228610">and</span> <span m="228730">medical</span>
  <span m="229150">diagnosis</span> <span m="230410">is</span> <span m="230590">actually</span>
  <span m="231040">going</span> <span m="231310">to</span> <span m="231430">happen.</span></p><p><span
  m="234110">So</span> <span m="235390">what</span> <span m="235750">we're</span>
  <span m="235870">going</span> <span m="236020">to</span> <span m="236110">look</span>
  <span m="236350">at</span> <span m="236530">today</span> <span m="237670">is</span>
  <span m="238810">what</span> <span m="240280">simpler</span> <span m="240880">models</span>
  <span m="241480">are</span> <span m="241690">there</span> <span m="242260">for</span>
  <span m="242590">diagnostic</span> <span m="243340">reasoning.</span> <span m="244660">And</span>
  <span m="245020">I'm</span> <span m="245230">going</span> <span m="245350">to</span>
  <span m="246370">take</span> <span m="246670">the</span> <span m="246790">liberty</span>
  <span m="247300">of</span> <span m="247510">inflicting</span> <span m="248260">a</span>
  <span m="248320">bit</span> <span m="248500">of</span> <span m="248620">history</span>
  <span m="249070">on</span> <span m="249280">you,</span> <span m="250480">because</span>
  <span m="251230">I</span> <span m="251320">think</span> <span m="251590">it's</span>
  <span m="251770">interesting</span> <span m="252370">where</span> <span m="252970">a</span>
  <span m="253060">lot</span> <span m="253300">of</span> <span m="253420">these</span>
  <span m="253660">ideas</span> <span m="254110">came</span> <span m="254410">from.</span></p><p><span
  m="256168">So the first idea was to</span> <span m="257140">build</span> <span m="257560">flowcharts.</span>
  <span m="260540">Oh,</span> <span m="260720">and</span> <span m="260839">by</span>
  <span m="261050">the</span> <span m="261140">way,</span> <span m="263070">the</span>
  <span m="263620">signs</span> <span m="264140">and</span> <span m="264290">symptoms,</span>
  <span m="265810">I've</span> <span m="266000">forgotten</span> <span m="266630">if</span>
  <span m="266780">we've</span> <span m="266990">talked</span> <span m="267320">about</span>
  <span m="267620">that</span> <span m="267860">in</span> <span m="267980">the</span>
  <span m="268070">class.</span> <span m="269120">So</span> <span m="269660">a</span>
  <span m="269750">sign</span> <span m="270230">is</span> <span m="270380">something</span>
  <span m="270860">that</span> <span m="271610">a</span> <span m="271670">doctor</span>
  <span m="272120">sees,</span> <span m="273680">and</span> <span m="274070">a</span>
  <span m="274370">symptom</span> <span m="274940">is</span> <span m="275060">something</span>
  <span m="275480">that</span> <span m="275660">the</span> <span m="275780">patient</span>
  <span m="276260">experiences.</span> <span m="277980">So</span> <span m="278150">a</span>
  <span m="278200">sign</span> <span m="278630">is</span> <span m="278900">objective.</span>
  <span m="279750">It's</span> <span m="279800">something</span> <span m="280220">that</span>
  <span m="280370">can</span> <span m="280580">be</span> <span m="280700">told</span>
  <span m="281090">outside</span> <span m="281750">your</span> <span m="281900">body.</span>
  <span m="282950">A</span> <span m="283010">symptom</span> <span m="283580">is</span>
  <span m="283730">something</span> <span m="284180">that</span> <span m="284390">you</span>
  <span m="284600">feel.</span> <span m="285950">So</span> <span m="286160">if</span>
  <span m="286400">you're</span> <span m="286580">feeling</span> <span m="287060">dizzy,</span>
  <span m="288170">then</span> <span m="288710">that's</span> <span m="289070">a</span>
  <span m="289130">symptom,</span> <span m="289730">because</span> <span m="290930">it's</span>
  <span m="291140">not</span> <span m="291380">obvious</span> <span m="291920">to</span>
  <span m="292040">somebody</span> <span m="292520">outside</span> <span m="293090">you</span>
  <span m="293840">that</span> <span m="294080">you're</span> <span m="294260">dizzy,</span>
  <span m="294740">or</span> <span m="294950">that</span> <span m="295190">you</span>
  <span m="295310">have</span> <span m="295490">a</span> <span m="295550">pain,</span>
  <span m="295970">or</span> <span m="296390">such</span> <span m="296720">things.</span></p><p><span
  m="298640">Normally,</span> <span m="299150">we</span> <span m="299300">talk</span>
  <span m="299600">about</span> <span m="299900">manifestations</span> <span m="301040">or</span>
  <span m="301190">findings,</span> <span m="301970">which</span> <span m="302270">is</span>
  <span m="302810">sort</span> <span m="303050">of</span> <span m="303170">a</span>
  <span m="303230">super</span> <span m="303620">category</span> <span m="304340">of</span>
  <span m="304550">all</span> <span m="304760">the</span> <span m="304880">things</span>
  <span m="305270">that</span> <span m="305450">are</span> <span m="306290">determinable</span>
  <span m="307220">about</span> <span m="307490">a</span> <span m="307550">patient.</span>
  <span m="309590">So</span> <span m="309800">we'll</span> <span m="309980">talk</span>
  <span m="310280">about</span> <span m="311060">flowcharts,</span> <span m="313580">models</span>
  <span m="314060">based</span> <span m="314390">on</span> <span m="314540">associations</span>
  <span m="315500">between</span> <span m="316490">diseases</span> <span m="317180">and</span>
  <span m="317300">these</span> <span m="317510">manifestations.</span> <span m="319400">Then</span>
  <span m="319640">there</span> <span m="319710">are</span> <span m="319820">some</span>
  <span m="320090">issues</span> <span m="320510">about</span> <span m="320840">whether</span>
  <span m="321170">you're</span> <span m="321350">trying</span> <span m="321680">to</span>
  <span m="321800">diagnose</span> <span m="322460">a</span> <span m="322490">single</span>
  <span m="322940">disease</span> <span m="323960">or</span> <span m="324140">a</span>
  <span m="324200">multiplicity</span> <span m="325040">of</span> <span m="325190">diseases,</span>
  <span m="325850">which</span> <span m="326090">makes</span> <span m="326420">the</span>
  <span m="326510">models</span> <span m="326960">much</span> <span m="327200">more</span>
  <span m="327380">complicated</span> <span m="329330">whether</span> <span m="329750">you're</span>
  <span m="329960">trying</span> <span m="330320">to</span> <span m="330470">do</span>
  <span m="330710">probabilistic</span> <span m="331610">diagnosis</span> <span m="332540">or</span>
  <span m="332720">definitive</span> <span m="333440">or</span> <span m="333590">categorical.</span>
  <span m="335600">And</span> <span m="335750">then</span> <span m="335960">we'll</span>
  <span m="336140">talk</span> <span m="336470">about</span> <span m="336770">some</span>
  <span m="337160">utility</span> <span m="337760">theoretic</span> <span m="338360">methods.</span>
  <span m="339440">And</span> <span m="339590">I'll</span> <span m="339740">just</span>
  <span m="340010">mention</span> <span m="340520">some</span> <span m="340790">rule-based</span>
  <span m="341390">and</span> <span m="341510">pattern-matching</span> <span m="343040">kinds</span>
  <span m="343400">of</span> <span m="343520">approaches.</span></p><p><span m="345030">So</span>
  <span m="345110">this</span> <span m="345350">is</span> <span m="345500">kind</span>
  <span m="345740">of</span> <span m="345800">cute.</span> <span m="347660">This</span>
  <span m="347990">is</span> <span m="348200">from</span> <span m="348530">1973.</span>
  <span m="350540">And</span> <span m="350990">if</span> <span m="351290">you</span>
  <span m="351860">were</span> <span m="352130">a</span> <span m="352190">woman</span>
  <span m="352610">and</span> <span m="352760">walked</span> <span m="353180">into</span>
  <span m="353780">the</span> <span m="354160">MIT</span> <span m="354680">Health</span>
  <span m="354920">Center</span> <span m="356240">and</span> <span m="356480">complained</span>
  <span m="357290">of</span> <span m="357770">potentially</span> <span m="358460">a</span>
  <span m="358520">urinary</span> <span m="359060">tract</span> <span m="359420">infection,</span>
  <span m="360860">they</span> <span m="361070">would</span> <span m="361430">take</span>
  <span m="361790">out</span> <span m="362210">this</span> <span m="362510">sheet</span>
  <span m="362780">of</span> <span m="362900">paper,</span> <span m="364070">which</span>
  <span m="364310">was</span> <span m="364460">nicely</span> <span m="364910">color-coded,</span>
  <span m="365720">and</span> <span m="365870">they</span> <span m="365990">would</span>
  <span m="366170">check</span> <span m="366470">a</span> <span m="366560">bunch</span>
  <span m="366830">of</span> <span m="366890">boxes.</span> <span m="368120">And</span>
  <span m="369080">if</span> <span m="369320">you</span> <span m="369500">hit</span>
  <span m="369710">a</span> <span m="369770">red</span> <span m="370100">box,</span>
  <span m="370670">that</span> <span m="371390">represented</span> <span m="372140">a</span>
  <span m="372200">conclusion.</span> <span m="373080">And</span> <span m="373460">otherwise,</span>
  <span m="374210">it</span> <span m="374660">gave</span> <span m="374930">you</span>
  <span m="375080">suggestions</span> <span m="375950">about</span> <span m="376670">what</span>
  <span m="376880">further</span> <span m="377270">tests</span> <span m="377690">to</span>
  <span m="377840">do.</span></p><p><span m="378590">And</span> <span m="378710">this</span>
  <span m="378890">was</span> <span m="379100">essentially</span> <span m="379670">a</span>
  <span m="379730">triage</span> <span m="380270">instrument.</span> <span m="381320">It</span>
  <span m="381500">said,</span> <span m="382490">does</span> <span m="382850">this</span>
  <span m="383090">woman</span> <span m="383420">have</span> <span m="383690">a</span>
  <span m="383750">problem</span> <span m="384800">that</span> <span m="385040">requires</span>
  <span m="385760">immediate</span> <span m="386300">attention?</span> <span m="386960">And</span>
  <span m="387080">so</span> <span m="387320">we</span> <span m="387470">should</span>
  <span m="388220">either</span> <span m="389510">call</span> <span m="389840">an</span>
  <span m="389960">ambulance</span> <span m="390560">and</span> <span m="390680">take</span>
  <span m="390920">them</span> <span m="391130">to</span> <span m="391290">a</span>
  <span m="391340">hospital,</span> <span m="392480">or</span> <span m="392720">is</span>
  <span m="392890">it</span> <span m="393020">something</span> <span m="393680">where</span>
  <span m="395810">we</span> <span m="396020">can</span> <span m="396200">just</span>
  <span m="396410">tell</span> <span m="396590">them</span> <span m="396710">to</span>
  <span m="396830">come</span> <span m="397070">back</span> <span m="397340">the</span>
  <span m="397460">next</span> <span m="397760">day</span> <span m="397970">and</span>
  <span m="398090">see</span> <span m="398330">a</span> <span m="398420">doctor,</span>
  <span m="399560">or</span> <span m="399770">is</span> <span m="399970">it</span>
  <span m="400070">in</span> <span m="400220">fact</span> <span m="400640">some</span>
  <span m="400940">self-limited</span> <span m="401660">thing</span> <span m="402020">where</span>
  <span m="402200">we</span> <span m="402350">say,</span> <span m="403430">take</span>
  <span m="403730">two</span> <span m="403970">aspirin,</span> <span m="404480">and</span>
  <span m="404630">it'll</span> <span m="404870">go</span> <span m="405080">away.</span>
  <span m="406170">So</span> <span m="406280">that</span> <span m="406520">was</span>
  <span m="406760">the</span> <span m="407420">attempt</span> <span m="407870">here.</span></p><p><span
  m="408860">Now,</span> <span m="409190">interestingly,</span> <span m="410070">if</span>
  <span m="410090">you</span> <span m="410210">look</span> <span m="410420">at</span>
  <span m="410540">the</span> <span m="410660">history</span> <span m="411110">of</span>
  <span m="411230">this</span> <span m="411410">project</span> <span m="411950">between</span>
  <span m="412370">the</span> <span m="412490">Beth</span> <span m="412760">Israel</span>
  <span m="413120">Hospital</span> <span m="414170">and</span> <span m="414440">Lincoln</span>
  <span m="414770">Laboratories,</span> <span m="416000">it</span> <span m="416180">started</span>
  <span m="416720">off</span> <span m="417170">as</span> <span m="417470">a</span>
  <span m="417530">computer</span> <span m="418010">aid.</span> <span m="419060">So</span>
  <span m="419270">they</span> <span m="419810">were</span> <span m="419990">building</span>
  <span m="420500">a</span> <span m="420590">computer</span> <span m="421070">system</span>
  <span m="422420">that</span> <span m="422720">was</span> <span m="422870">supposed</span>
  <span m="423320">to</span> <span m="423440">do</span> <span m="423650">this.</span>
  <span m="425040">And</span> <span m="425210">then</span> <span m="425450">in--</span>
  <span m="425930">but</span> <span m="426290">you</span> <span m="426440">can</span>
  <span m="426620">imagine,</span> <span m="427160">in</span> <span m="427280">the</span>
  <span m="427370">late</span> <span m="427640">1960s,</span> <span m="429180">early</span>
  <span m="429350">1970s,</span> <span m="430370">computers</span> <span m="431000">were</span>
  <span m="431210">pretty</span> <span m="431510">clunky.</span> <span m="433970">PCs</span>
  <span m="434540">hadn't</span> <span m="434840">been</span> <span m="435080">invented</span>
  <span m="435530">yet.</span> <span m="435900">So</span> <span m="436040">this</span>
  <span m="436280">was</span> <span m="436460">like</span> <span m="436730">mainframe</span>
  <span m="437840">kinds</span> <span m="438170">of</span> <span m="438290">operations.</span>
  <span m="439110">It</span> <span m="439190">was</span> <span m="440000">very</span>
  <span m="440300">hard</span> <span m="440540">to</span> <span m="440720">use.</span>
  <span m="441680">And</span> <span m="441830">so</span> <span m="442070">they</span>
  <span m="442250">said,</span> <span m="442520">well,</span> <span m="443270">this</span>
  <span m="443540">is</span> <span m="443720">a</span> <span m="443780">small</span>
  <span m="444230">enough</span> <span m="444500">program</span> <span m="445610">that</span>
  <span m="445850">we</span> <span m="446000">can</span> <span m="446210">reduce</span>
  <span m="446750">it</span> <span m="446900">to</span> <span m="447140">about</span>
  <span m="447530">20</span> <span m="448010">flow</span> <span m="448340">sheets--</span>
  <span m="448870">20</span> <span m="449210">sheets</span> <span m="449630">like</span>
  <span m="449930">this,</span> <span m="451340">which</span> <span m="451670">they</span>
  <span m="451910">proceeded</span> <span m="452630">to</span> <span m="452780">print</span>
  <span m="453170">up.</span></p><p><span m="454100">And</span> <span m="454310">I</span>
  <span m="454490">was</span> <span m="454730">amused,</span> <span m="455300">because</span>
  <span m="455960">in</span> <span m="456260">the--</span> <span m="457040">around</span>
  <span m="457430">1980,</span> <span m="458960">I</span> <span m="459080">was</span>
  <span m="459320">working</span> <span m="459740">in</span> <span m="459860">my</span>
  <span m="460070">office</span> <span m="460460">one</span> <span m="460670">night.</span>
  <span m="460930">And</span> <span m="461090">I</span> <span m="461180">got</span>
  <span m="461410">this</span> <span m="461530">splitting</span> <span m="462170">headache.</span>
  <span m="463130">And</span> <span m="463250">I</span> <span m="463370">went</span>
  <span m="463610">over</span> <span m="463850">to</span> <span m="464040">MIT</span>
  <span m="464410">medical.</span> <span m="465530">And</span> <span m="465770">sure</span>
  <span m="466040">enough,</span> <span m="466310">the</span> <span m="466460">nurse</span>
  <span m="466820">pulled</span> <span m="467210">out</span> <span m="467960">one</span>
  <span m="468170">of</span> <span m="468290">these</span> <span m="468530">sheets</span>
  <span m="469040">for</span> <span m="469400">headaches</span> <span m="470480">and</span>
  <span m="470720">went</span> <span m="470990">through</span> <span m="471290">it</span>
  <span m="471500">with</span> <span m="471800">me</span> <span m="472010">and</span>
  <span m="472160">decided</span> <span m="472760">that</span> <span m="473420">a</span>
  <span m="473480">couple</span> <span m="473810">of</span> <span m="473870">Tylenols</span>
  <span m="474470">should</span> <span m="474710">fix</span> <span m="475040">me.</span>
  <span m="476420">But</span> <span m="477020">it</span> <span m="477110">was</span>
  <span m="477260">interesting.</span> <span m="477770">So</span> <span m="477950">this</span>
  <span m="478190">was</span> <span m="478400">really</span> <span m="478730">in</span>
  <span m="478850">use</span> <span m="479180">for</span> <span m="479450">a</span>
  <span m="479510">while.</span></p><p><span m="480740">Now,</span> <span m="481100">the</span>
  <span m="481280">difficulty</span> <span m="482360">with</span> <span m="483290">approaches</span>
  <span m="483920">like</span> <span m="484190">this,</span> <span m="484640">of</span>
  <span m="484850">which</span> <span m="485180">there</span> <span m="485390">have</span>
  <span m="485540">been</span> <span m="485780">many,</span> <span m="486150">many,</span>
  <span m="486450">many</span> <span m="486800">in</span> <span m="486980">the</span>
  <span m="487070">medical</span> <span m="487490">world,</span> <span m="488510">is</span>
  <span m="488720">that</span> <span m="489340">they're</span> <span m="489590">very</span>
  <span m="489860">fragile.</span> <span m="491180">They're</span> <span m="491450">very</span>
  <span m="491720">specific.</span> <span m="493620">They</span> <span m="493820">don't</span>
  <span m="494420">take</span> <span m="494780">account</span> <span m="495410">of</span>
  <span m="495860">unusual</span> <span m="496490">cases.</span> <span m="498410">And</span>
  <span m="498860">there's</span> <span m="499190">a</span> <span m="499250">lot</span>
  <span m="499490">of</span> <span m="499610">effort</span> <span m="500180">in</span>
  <span m="500810">coming</span> <span m="501140">to</span> <span m="501290">consensus</span>
  <span m="502100">to</span> <span m="502250">build</span> <span m="502520">these</span>
  <span m="502790">things.</span> <span m="503730">And</span> <span m="503780">then</span>
  <span m="503990">they're</span> <span m="504140">not</span> <span m="504410">necessarily</span>
  <span m="505040">useful</span> <span m="505550">for</span> <span m="505790">a</span>
  <span m="505850">long</span> <span m="506120">time.</span></p><p><span m="507080">So</span>
  <span m="507410">MIT</span> <span m="507860">actually</span> <span m="508670">stopped</span>
  <span m="509090">using</span> <span m="509540">them</span> <span m="510290">shortly</span>
  <span m="510800">after</span> <span m="511160">my</span> <span m="511370">headache</span>
  <span m="511760">experience.</span> <span m="513530">But</span> <span m="514039">if</span>
  <span m="514250">you</span> <span m="514400">go</span> <span m="515090">over</span>
  <span m="515360">to</span> <span m="515539">a</span> <span m="515600">hospital</span>
  <span m="516350">and</span> <span m="516530">you</span> <span m="516710">look</span>
  <span m="516980">on</span> <span m="517130">the</span> <span m="517220">bookshelf</span>
  <span m="518059">of</span> <span m="519690">a</span> <span m="519799">junior</span>
  <span m="520190">doctor,</span> <span m="521900">you</span> <span m="522080">will</span>
  <span m="522230">still</span> <span m="522559">find</span> <span m="522919">manuals</span>
  <span m="524090">that</span> <span m="524330">look</span> <span m="524600">kind</span>
  <span m="524870">of</span> <span m="524930">like</span> <span m="525230">this</span>
  <span m="525740">that</span> <span m="525980">say,</span> <span m="527210">how</span>
  <span m="527390">do</span> <span m="527750">we</span> <span m="527960">deal</span>
  <span m="528230">with</span> <span m="528470">tropical</span> <span m="529040">diseases?</span>
  <span m="530960">So</span> <span m="531200">you</span> <span m="531350">ask</span>
  <span m="531650">a</span> <span m="531710">bunch</span> <span m="531980">of</span>
  <span m="532040">questions,</span> <span m="532730">and</span> <span m="532850">then</span>
  <span m="533450">depending</span> <span m="533990">on</span> <span m="534170">the</span>
  <span m="534260">branching</span> <span m="534740">logic</span> <span m="535250">of</span>
  <span m="535370">the</span> <span m="535540">flowchart,</span> <span m="536990">it'll</span>
  <span m="537290">tell</span> <span m="537560">you</span> <span m="537710">whether</span>
  <span m="538100">this</span> <span m="538340">is</span> <span m="538400">serious</span>
  <span m="539060">or</span> <span m="539150">not.</span></p><p><span m="540000">And</span>
  <span m="540020">the</span> <span m="540140">reason</span> <span m="540530">is</span>
  <span m="540770">because</span> <span m="541190">if</span> <span m="541340">you</span>
  <span m="541490">do</span> <span m="541640">your</span> <span m="541820">medical</span>
  <span m="542240">training</span> <span m="542690">in</span> <span m="542780">Boston,</span>
  <span m="543740">you're</span> <span m="543890">not</span> <span m="544070">going</span>
  <span m="544220">to</span> <span m="544280">see</span> <span m="544580">very</span>
  <span m="544880">many</span> <span m="545510">tropical</span> <span m="546080">diseases.</span>
  <span m="546800">And</span> <span m="546920">so</span> <span m="547130">you</span>
  <span m="547250">don't</span> <span m="547520">have</span> <span m="548840">a</span>
  <span m="548900">base</span> <span m="549230">of</span> <span m="549350">experience</span>
  <span m="550220">on</span> <span m="550430">the</span> <span m="550520">basis</span>
  <span m="551000">of</span> <span m="551120">which</span> <span m="551450">you</span>
  <span m="551570">can</span> <span m="551780">learn</span> <span m="552740">and</span>
  <span m="552980">become</span> <span m="553370">an</span> <span m="553490">expert</span>
  <span m="553940">at</span> <span m="554000">doing</span> <span m="554420">it.</span>
  <span m="554630">And</span> <span m="554780">so</span> <span m="554990">they</span>
  <span m="555170">use</span> <span m="555470">this</span> <span m="555800">as</span>
  <span m="555980">a</span> <span m="556040">kind</span> <span m="556310">of</span>
  <span m="556430">cheat</span> <span m="556690">sheet.</span></p><p><span m="560070">I</span>
  <span m="560190">mentioned</span> <span m="560640">that</span> <span m="561000">the</span>
  <span m="561240">association</span> <span m="562110">between</span> <span m="563190">diseases</span>
  <span m="564200">and</span> <span m="564420">symptoms</span> <span m="565830">is</span>
  <span m="566100">another</span> <span m="566790">important</span> <span m="567390">way</span>
  <span m="567600">of</span> <span m="568110">doing</span> <span m="568440">diagnosis.</span>
  <span m="569850">And</span> <span m="570120">I</span> <span m="570270">swear</span>
  <span m="570570">to</span> <span m="570690">you,</span> <span m="570810">there</span>
  <span m="571050">was</span> <span m="571380">a</span> <span m="571440">paper</span>
  <span m="572130">in</span> <span m="572370">the</span> <span m="572460">1960s,</span>
  <span m="574210">I</span> <span m="574310">think,</span> <span m="575100">that</span>
  <span m="575310">actually</span> <span m="575790">proposed</span> <span m="576390">this.</span>
  <span m="577200">So</span> <span m="577710">if</span> <span m="577920">any</span>
  <span m="578130">of</span> <span m="578280">you</span> <span m="578460">have</span>
  <span m="578580">hung</span> <span m="578850">around</span> <span m="579300">ancient</span>
  <span m="579750">libraries,</span> <span m="581790">libraries</span> <span m="582480">used</span>
  <span m="582750">to</span> <span m="582870">have</span> <span m="583110">card</span>
  <span m="583410">catalogs</span> <span m="584640">that</span> <span m="584910">were</span>
  <span m="585090">physical</span> <span m="585630">pieces</span> <span m="586080">of</span>
  <span m="586170">paper,</span> <span m="587070">cardboard.</span> <span m="588780">And</span>
  <span m="589260">one</span> <span m="589530">of</span> <span m="589650">the</span>
  <span m="589770">things</span> <span m="590130">they</span> <span m="590310">did</span>
  <span m="590550">with</span> <span m="590820">these</span> <span m="591660">was</span>
  <span m="593040">each</span> <span m="594720">card</span> <span m="595170">would</span>
  <span m="595380">be</span> <span m="595560">a</span> <span m="595650">book.</span></p><p><span
  m="597270">And</span> <span m="597480">then</span> <span m="598200">around</span>
  <span m="598590">the</span> <span m="598770">edges</span> <span m="599310">were</span>
  <span m="599550">a</span> <span m="599580">bunch</span> <span m="599910">of</span>
  <span m="600030">holes,</span> <span m="601330">and</span> <span m="601500">depending</span>
  <span m="602220">on</span> <span m="602490">categorizations</span> <span m="603720">of</span>
  <span m="603870">the</span> <span m="603990">book</span> <span m="604770">along</span>
  <span m="605130">various</span> <span m="605580">dimensions,</span> <span m="606930">like</span>
  <span m="607260">its</span> <span m="607710">Dewey</span> <span m="608010">decimal</span>
  <span m="608490">number,</span> <span m="609000">or</span> <span m="609810">the</span>
  <span m="610020">top</span> <span m="610350">digits</span> <span m="610890">of</span>
  <span m="611040">its</span> <span m="612270">Library</span> <span m="612780">of</span>
  <span m="612900">Congress</span> <span m="613380">number</span> <span m="613770">or</span>
  <span m="613950">something,</span> <span m="614940">they</span> <span m="615120">would</span>
  <span m="615330">punch</span> <span m="615780">out</span> <span m="616320">holes</span>
  <span m="617220">in</span> <span m="617400">the</span> <span m="617490">borders.</span>
  <span m="619030">And</span> <span m="619110">this</span> <span m="619410">allowed</span>
  <span m="619830">you</span> <span m="620010">to</span> <span m="620220">do</span>
  <span m="620690">a</span> <span m="620780">kind</span> <span m="621090">of</span>
  <span m="621480">easy</span> <span m="621840">sorting</span> <span m="622710">of</span>
  <span m="622890">these</span> <span m="623160">books.</span></p><p><span m="624130">So</span>
  <span m="624450">if</span> <span m="624780">you've</span> <span m="624930">got</span>
  <span m="625170">a</span> <span m="625230">bunch</span> <span m="625530">of</span>
  <span m="625620">cards</span> <span m="626100">together</span> <span m="627060">when</span>
  <span m="627270">people</span> <span m="627630">were</span> <span m="627810">returning</span>
  <span m="628410">their</span> <span m="628590">books</span> <span m="629100">and</span>
  <span m="629220">you</span> <span m="629370">pulled</span> <span m="630020">a</span>
  <span m="630060">bunch</span> <span m="630360">of</span> <span m="630420">cards.</span>
  <span m="631440">And</span> <span m="631620">you</span> <span m="631740">wanted</span>
  <span m="632010">to</span> <span m="632160">find</span> <span m="632610">all</span>
  <span m="632850">the</span> <span m="632970">math</span> <span m="633330">books.</span>
  <span m="634320">So</span> <span m="634500">what</span> <span m="634740">you</span>
  <span m="634830">would</span> <span m="634980">do</span> <span m="635220">is</span>
  <span m="635400">you'd</span> <span m="635610">stick</span> <span m="636000">a</span>
  <span m="636090">needle</span> <span m="637050">through</span> <span m="637440">the</span>
  <span m="637590">hole</span> <span m="638040">that</span> <span m="638310">represented</span>
  <span m="639030">math</span> <span m="639360">books,</span> <span m="640260">and</span>
  <span m="640380">then</span> <span m="640560">you</span> <span m="640710">shake</span>
  <span m="641100">the</span> <span m="641220">pile,</span> <span m="642300">and</span>
  <span m="642810">all</span> <span m="642990">the</span> <span m="643110">math</span>
  <span m="643410">books</span> <span m="643770">would</span> <span m="643950">fall</span>
  <span m="644310">out</span> <span m="644670">because</span> <span m="645120">they</span>
  <span m="645270">had</span> <span m="645720">punched.</span></p><p><span m="646890">So</span>
  <span m="647100">somebody</span> <span m="647610">seriously</span> <span m="648300">proposed</span>
  <span m="648870">this</span> <span m="649230">as</span> <span m="649410">a</span>
  <span m="649470">diagnostic</span> <span m="650250">algorithm.</span> <span m="652120">And</span>
  <span m="652530">in</span> <span m="652680">fact,</span> <span m="653760">implemented</span>
  <span m="654390">it.</span> <span m="654660">And</span> <span m="654870">was</span>
  <span m="655710">trying</span> <span m="656100">to</span> <span m="657780">even</span>
  <span m="658080">make</span> <span m="658320">money</span> <span m="658650">on</span>
  <span m="658860">it.</span> <span m="659010">I</span> <span m="659130">think</span>
  <span m="659370">this</span> <span m="659580">was</span> <span m="659820">an</span>
  <span m="659940">attempt</span> <span m="660360">at</span> <span m="660480">a</span>
  <span m="660570">commercial</span> <span m="661110">venture,</span> <span m="662940">where</span>
  <span m="663240">they</span> <span m="663390">were</span> <span m="663570">going</span>
  <span m="663840">to</span> <span m="663990">provide</span> <span m="664470">doctors</span>
  <span m="665580">with</span> <span m="665910">these</span> <span m="666150">library</span>
  <span m="666690">cards</span> <span m="667230">that</span> <span m="667440">represented</span>
  <span m="668100">diseases.</span> <span m="669390">And</span> <span m="669570">the</span>
  <span m="669690">holes</span> <span m="670140">now</span> <span m="670440">represented</span>
  <span m="671220">not</span> <span m="671490">mathematics</span> <span m="672390">versus</span>
  <span m="673290">literature,</span> <span m="673920">but</span> <span m="674160">they</span>
  <span m="674340">represented</span> <span m="675570">shortness</span> <span m="676170">of</span>
  <span m="676290">breath</span> <span m="676770">versus</span> <span m="677370">pain</span>
  <span m="677700">in</span> <span m="677850">the</span> <span m="677940">left</span>
  <span m="678300">ankle</span> <span m="678750">versus</span> <span m="679350">whatever.</span>
  <span m="680490">And</span> <span m="680700">again,</span> <span m="681090">as</span>
  <span m="681300">people</span> <span m="681660">came</span> <span m="681960">in</span>
  <span m="682170">and</span> <span m="682350">complained</span> <span m="682980">about</span>
  <span m="683250">some</span> <span m="683520">condition,</span> <span m="684540">you'd</span>
  <span m="684720">stick</span> <span m="685080">a</span> <span m="685140">needle</span>
  <span m="685500">through</span> <span m="685830">that</span> <span m="686070">condition</span>
  <span m="686700">and</span> <span m="686820">you'd</span> <span m="687020">shake,</span>
  <span m="687820">and</span> <span m="688020">up</span> <span m="688200">would</span>
  <span m="688380">come</span> <span m="688650">the</span> <span m="688770">cards</span>
  <span m="689280">that</span> <span m="690570">had</span> <span m="690780">that</span>
  <span m="691050">condition</span> <span m="691590">in</span> <span m="691710">common.</span></p><p><span
  m="693000">So</span> <span m="693360">one</span> <span m="693600">of</span> <span
  m="693720">the</span> <span m="693870">obvious</span> <span m="694350">problems</span>
  <span m="694890">with</span> <span m="695100">this</span> <span m="695310">approach</span>
  <span m="697500">is</span> <span m="697770">that</span> <span m="698190">if</span>
  <span m="698700">you</span> <span m="698850">had</span> <span m="699000">two</span>
  <span m="699240">things</span> <span m="699600">wrong</span> <span m="699870">with</span>
  <span m="700110">you,</span> <span m="701850">then</span> <span m="702150">you</span>
  <span m="702270">would</span> <span m="702450">wind</span> <span m="702750">up</span>
  <span m="702900">with</span> <span m="703080">no</span> <span m="703320">cards</span>
  <span m="703890">very</span> <span m="704190">quickly,</span> <span m="705390">because</span>
  <span m="707520">nothing</span> <span m="707970">would</span> <span m="708090">fall</span>
  <span m="708480">out</span> <span m="708660">of</span> <span m="708780">the</span>
  <span m="708900">pile.</span> <span m="709980">So</span> <span m="710220">this</span>
  <span m="710430">didn't</span> <span m="710700">go</span> <span m="710940">anywhere.</span></p><p><span
  m="711350">But</span> <span m="711810">interestingly,</span> <span m="713190">even</span>
  <span m="713820">in</span> <span m="714120">the</span> <span m="714840">late</span>
  <span m="715200">1980s,</span> <span m="716890">I</span> <span m="716910">remember</span>
  <span m="717870">being</span> <span m="718260">asked</span> <span m="718650">by</span>
  <span m="718890">the</span> <span m="720210">board</span> <span m="720480">of</span>
  <span m="720570">directors</span> <span m="721140">of</span> <span m="721260">the</span>
  <span m="721380"><i>New</i></span> <span m="721560"><i>England</i></span> <span
  m="721800"><i>Journal</i></span> <span m="722130"><i>of</i></span> <span m="722220"><i>Medicine</i></span>
  <span m="722700">to</span> <span m="722850">come</span> <span m="723150">to</span>
  <span m="723360">a</span> <span m="723420">meeting</span> <span m="724560">where</span>
  <span m="724800">they</span> <span m="725010">had</span> <span m="725250">gotten</span>
  <span m="725670">a</span> <span m="725760">pitch</span> <span m="726210">from</span>
  <span m="726480">somebody</span> <span m="727500">who</span> <span m="727650">was</span>
  <span m="727950">proposing</span> <span m="728700">essentially</span> <span m="729390">exactly</span>
  <span m="729990">this</span> <span m="730230">diagnostic</span> <span m="730920">model,</span>
  <span m="731730">except</span> <span m="732180">implemented</span> <span m="732810">in</span>
  <span m="732960">a</span> <span m="733020">computer</span> <span m="733600">now</span>
  <span m="734100">and</span> <span m="734280">not</span> <span m="734730">in</span>
  <span m="736020">these</span> <span m="736200">library</span> <span m="736680">cards.</span>
  <span m="737670">And</span> <span m="737910">they</span> <span m="738060">wanted</span>
  <span m="738390">to</span> <span m="738540">know</span> <span m="738810">whether</span>
  <span m="739230">this</span> <span m="739470">was</span> <span m="739650">something</span>
  <span m="740070">that</span> <span m="740250">they</span> <span m="740400">ought</span>
  <span m="740550">to</span> <span m="740610">get</span> <span m="740850">behind</span>
  <span m="741390">and</span> <span m="741540">invest</span> <span m="742020">in.</span>
  <span m="742740">And</span> <span m="742950">I</span> <span m="743250">and</span>
  <span m="743400">a</span> <span m="743460">bunch</span> <span m="743730">of</span>
  <span m="743820">my</span> <span m="744000">colleagues</span> <span m="744600">assured</span>
  <span m="744990">them</span> <span m="745230">that</span> <span m="745410">this</span>
  <span m="745650">was</span> <span m="745830">probably</span> <span m="746190">not</span>
  <span m="746460">a</span> <span m="746520">great</span> <span m="746820">idea</span>
  <span m="747870">and they</span> <span m="748020">should</span> <span m="748260">stay</span>
  <span m="748530">away</span> <span m="748800">from</span> <span m="749070">it,</span>
  <span m="749320">which</span> <span m="749490">they</span> <span m="749670">did.</span></p><p><span
  m="752940">Well,</span> <span m="753360">a</span> <span m="753420">more</span> <span
  m="753660">sophisticated</span> <span m="754560">model</span> <span m="755250">is</span>
  <span m="755430">something</span> <span m="755850">like</span> <span m="756120">a</span>
  <span m="756180">Naive</span> <span m="756600">Bayes</span> <span m="756900">model</span>
  <span m="757890">that</span> <span m="758160">says</span> <span m="758760">if</span>
  <span m="758970">you</span> <span m="759150">have</span> <span m="759570">a</span>
  <span m="759660">disease--</span> <span m="763450">where</span> <span m="763610">is</span>
  <span m="763770">my</span> <span m="763980">cursor?</span> <span m="764390">If</span>
  <span m="764640">you</span> <span m="764790">have</span> <span m="764940">a</span>
  <span m="765030">disease,</span> <span m="766230">and</span> <span m="766410">you</span>
  <span m="766560">have</span> <span m="766770">a</span> <span m="766830">bunch</span>
  <span m="767130">of</span> <span m="767220">manifestations</span> <span m="768330">that</span>
  <span m="768510">can</span> <span m="768750">be</span> <span m="768900">caused</span>
  <span m="769320">by</span> <span m="769500">the</span> <span m="769650">disease,</span>
  <span m="770850">we</span> <span m="771030">can</span> <span m="771210">make</span>
  <span m="771450">some</span> <span m="771690">simplifying</span> <span m="772440">assumptions</span>
  <span m="773700">that</span> <span m="773940">say</span> <span m="774240">that</span>
  <span m="774540">you</span> <span m="774660">will</span> <span m="774930">only</span>
  <span m="775320">ever</span> <span m="775590">have</span> <span m="775860">one</span>
  <span m="776130">disease</span> <span m="776610">at</span> <span m="776730">a</span>
  <span m="776820">time,</span> <span m="778720">which</span> <span m="778890">means</span>
  <span m="779250">that</span> <span m="779490">the</span> <span m="780000">values</span>
  <span m="780840">of</span> <span m="781050">that</span> <span m="781320">node</span>
  <span m="781580">D</span> <span m="782730">form</span> <span m="783870">an</span>
  <span m="784020">exhaustive</span> <span m="784710">and</span> <span m="784860">mutually</span>
  <span m="785400">exclusive</span> <span m="786060">set</span> <span m="786570">of</span>
  <span m="786690">values.</span></p><p><span m="788460">And</span> <span m="788670">we</span>
  <span m="788820">can</span> <span m="789030">assume</span> <span m="789390">that</span>
  <span m="789570">the</span> <span m="789660">manifestations</span> <span m="790710">are</span>
  <span m="790830">conditionally</span> <span m="791550">independent</span> <span
  m="792450">observables</span> <span m="793800">that</span> <span m="794010">depend</span>
  <span m="794550">only</span> <span m="794970">on</span> <span m="795270">the</span>
  <span m="795420">disease</span> <span m="795900">that</span> <span m="796110">you</span>
  <span m="796260">have,</span> <span m="796650">but</span> <span m="796920">not</span>
  <span m="797190">on</span> <span m="797370">each</span> <span m="797580">other</span>
  <span m="797970">or</span> <span m="798180">not</span> <span m="798480">on</span>
  <span m="799170">any</span> <span m="799380">other</span> <span m="799590">factors.</span>
  <span m="801760">And</span> <span m="801810">if</span> <span m="801930">you</span>
  <span m="802080">make</span> <span m="802320">that</span> <span m="802530">assumption,</span>
  <span m="803470">then</span> <span m="803640">you</span> <span m="803790">can</span>
  <span m="804000">apply</span> <span m="805320">good</span> <span m="805560">old</span>
  <span m="805740">Thomas</span> <span m="806250">Bayes's</span> <span m="807180">rule.</span></p><p><span
  m="807960">This,</span> <span m="808230">by</span> <span m="808440">the</span> <span
  m="808530">way,</span> <span m="808710">is</span> <span m="808860">the</span> <span
  m="808980">Reverend</span> <span m="809400">Bayes.</span> <span m="811540">Do</span>
  <span m="811710">you</span> <span m="811770">guys</span> <span m="812040">know</span>
  <span m="812250">his</span> <span m="812460">history?</span> <span m="815310">So</span>
  <span m="815780">he</span> <span m="815940">was</span> <span m="816210">a</span>
  <span m="816270">nonconformist</span> <span m="818520">minister</span> <span m="819390">in</span>
  <span m="819540">England.</span> <span m="821410">And</span> <span m="822850">he</span>
  <span m="823060">was</span> <span m="823300">not</span> <span m="823540">a</span>
  <span m="823570">mathematician,</span> <span m="824650">except</span> <span m="826900">I</span>
  <span m="826990">mean,</span> <span m="827200">he</span> <span m="827290">was</span>
  <span m="827470">an</span> <span m="827590">amateur</span> <span m="827980">mathematician.</span>
  <span m="829360">But</span> <span m="829600">he</span> <span m="829750">decided</span>
  <span m="830350">that</span> <span m="830560">he</span> <span m="830680">wanted</span>
  <span m="830980">to</span> <span m="831190">prove</span> <span m="831580">to</span>
  <span m="831760">people</span> <span m="832240">that</span> <span m="832450">God</span>
  <span m="832780">existed.</span> <span m="834830">And</span> <span m="834880">so</span>
  <span m="835150">he</span> <span m="835330">developed</span> <span m="835810">Bayesian</span>
  <span m="836410">reasoning</span> <span m="837070">in</span> <span m="837310">order</span>
  <span m="837610">to</span> <span m="837760">make</span> <span m="838060">this</span>
  <span m="838270">proof.</span></p><p><span m="839470">And</span> <span m="839620">so</span>
  <span m="839890">his</span> <span m="840130">argument</span> <span m="840670">was,</span>
  <span m="841100">well,</span> <span m="841690">suppose</span> <span m="842310">you're</span>
  <span m="842650">completely</span> <span m="843310">in</span> <span m="843430">doubt.</span>
  <span m="844330">So</span> <span m="844550">you</span> <span m="845020">have</span>
  <span m="845140">50/50</span> <span m="845980">odds</span> <span m="846340">that</span>
  <span m="846550">God</span> <span m="846850">exists.</span> <span m="848140">And</span>
  <span m="848290">then</span> <span m="848500">you</span> <span m="848620">say,</span>
  <span m="849430">let's</span> <span m="849730">look</span> <span m="850000">at</span>
  <span m="850150">miracles.</span> <span m="852220">And</span> <span m="852400">let's</span>
  <span m="852700">ask,</span> <span m="853150">what's</span> <span m="853480">the</span>
  <span m="853600">likelihood</span> <span m="854290">of</span> <span m="854440">this</span>
  <span m="854650">miracle</span> <span m="855160">having</span> <span m="855520">occurred</span>
  <span m="856570">if</span> <span m="856810">God</span> <span m="857140">exists</span>
  <span m="857860">versus</span> <span m="858430">if</span> <span m="858580">God</span>
  <span m="858850">doesn't</span> <span m="859330">exist?</span> <span m="860560">And</span>
  <span m="860710">so</span> <span m="860950">by</span> <span m="861340">racking</span>
  <span m="861910">up</span> <span m="862120">a</span> <span m="862210">bunch</span>
  <span m="862510">of</span> <span m="862600">miracles,</span> <span m="863560">you</span>
  <span m="863740">can</span> <span m="863980">convince</span> <span m="864550">people</span>
  <span m="865600">more</span> <span m="865870">and</span> <span m="865990">more</span>
  <span m="866470">that</span> <span m="866920">God</span> <span m="867250">must</span>
  <span m="867610">exist,</span> <span m="868060">because</span> <span m="868480">otherwise</span>
  <span m="868990">all</span> <span m="869140">these</span> <span m="869350">miracles</span>
  <span m="869860">couldn't</span> <span m="870160">have</span> <span m="870280">happened.</span></p><p><span
  m="871750">So</span> <span m="871960">he</span> <span m="872140">never</span> <span
  m="872380">publish</span> <span m="872860">this</span> <span m="873100">in</span>
  <span m="873220">his</span> <span m="873340">lifetime,</span> <span m="873970">but</span>
  <span m="874150">after</span> <span m="874510">his</span> <span m="874750">death</span>
  <span m="875500">one</span> <span m="875740">of</span> <span m="875860">his</span>
  <span m="876040">colleagues</span> <span m="876610">actually</span> <span m="877090">presented</span>
  <span m="877780">this</span> <span m="878110">as</span> <span m="878290">a</span>
  <span m="878350">paper</span> <span m="879340">at</span> <span m="879520">the</span>
  <span m="879640">Royal</span> <span m="879970">Society</span> <span m="880870">in</span>
  <span m="881290">the</span> <span m="881410">UK.</span> <span m="882580">And</span>
  <span m="883450">so</span> <span m="883690">Bayes</span> <span m="884050">became</span>
  <span m="884530">famous</span> <span m="885250">as</span> <span m="885520">the</span>
  <span m="885670">originator</span> <span m="886930">of</span> <span m="887110">this</span>
  <span m="887350">notion</span> <span m="888040">of</span> <span m="888970">how</span>
  <span m="889180">to</span> <span m="889530">do</span> <span m="889750">probabilistic</span>
  <span m="890590">reasoning</span> <span m="891610">about</span> <span m="892060">at</span>
  <span m="892210">least</span> <span m="892510">fairly</span> <span m="892870">simple</span>
  <span m="893230">situations,</span> <span m="894520">like</span> <span m="894820">in</span>
  <span m="894940">his</span> <span m="895180">case,</span> <span m="895780">the</span>
  <span m="896020">existence</span> <span m="896620">or</span> <span m="896740">nonexistence</span>
  <span m="897610">of</span> <span m="897730">God.</span> <span m="898600">Or</span>
  <span m="898810">in</span> <span m="898960">our</span> <span m="899140">case,</span>
  <span m="899590">the</span> <span m="899710">cause</span> <span m="900190">of</span>
  <span m="900340">some</span> <span m="900640">disease,</span> <span m="901840">the</span>
  <span m="902200">nature</span> <span m="902620">of</span> <span m="902740">some</span>
  <span m="902980">disease.</span></p><p><span m="904340">And</span> <span m="904390">so</span>
  <span m="904570">you</span> <span m="904690">can</span> <span m="904900">draw</span>
  <span m="905200">these</span> <span m="905470">trees.</span> <span m="905980">And</span>
  <span m="906550">Bayes's</span> <span m="906940">rule</span> <span m="907210">is</span>
  <span m="907360">very</span> <span m="907600">simple.</span> <span m="908420">I'm</span>
  <span m="908440">sure</span> <span m="908680">you've</span> <span m="908890">all</span>
  <span m="909040">seen</span> <span m="909370">it.</span></p><p><span m="910870">One</span>
  <span m="911110">thing</span> <span m="911320">that,</span> <span m="911900">again,</span>
  <span m="912190">makes</span> <span m="912520">contact</span> <span m="913150">with</span>
  <span m="913330">medicine</span> <span m="915050">is</span> <span m="915320">that</span>
  <span m="916070">a</span> <span m="916130">lot</span> <span m="916400">of</span>
  <span m="916520">times,</span> <span m="917690">you're</span> <span m="917900">not</span>
  <span m="918170">just</span> <span m="918500">interested</span> <span m="919040">in</span>
  <span m="919160">the</span> <span m="919340">impact</span> <span m="919880">of</span>
  <span m="920060">one</span> <span m="920330">observable</span> <span m="921650">on</span>
  <span m="921860">your</span> <span m="922010">probability</span> <span m="922670">distribution,</span>
  <span m="923550">but</span> <span m="923690">you're</span> <span m="923840">interested</span>
  <span m="924380">in</span> <span m="924500">the</span> <span m="924650">impact</span>
  <span m="925520">of</span> <span m="925670">a</span> <span m="925730">sequence</span>
  <span m="926270">of</span> <span m="926390">observations.</span> <span m="928140">And</span>
  <span m="928190">so</span> <span m="928990">one</span> <span m="929240">thing</span>
  <span m="929480">you</span> <span m="929600">can</span> <span m="929840">do</span>
  <span m="930290">is</span> <span m="930560">you</span> <span m="930710">can</span>
  <span m="930920">say,</span> <span m="931320">well,</span> <span m="932190">here</span>
  <span m="932480">is</span> <span m="932840">my</span> <span m="933080">general</span>
  <span m="933530">population.</span></p><p><span m="934680">So</span> <span m="934820">let's</span>
  <span m="935060">say</span> <span m="935780">disease</span> <span m="936320">2</span>
  <span m="936620">has</span> <span m="936920">37%</span> <span m="938060">prevalence</span>
  <span m="938750">and</span> <span m="938900">disease</span> <span m="939910">1</span>
  <span m="940310">has</span> <span m="940660">12%,</span> <span m="941780">et</span>
  <span m="941990">cetera.</span> <span m="943100">And</span> <span m="943250">now</span>
  <span m="943460">I</span> <span m="943610">make</span> <span m="943850">some</span>
  <span m="944120">observation.</span> <span m="945470">I</span> <span m="945650">apply</span>
  <span m="946040">Bayes's</span> <span m="946430">rule.</span> <span m="947210">And</span>
  <span m="947600">I</span> <span m="947750">revise</span> <span m="948260">my</span>
  <span m="948470">probability</span> <span m="949130">distribution.</span></p><p><span
  m="950980">So</span> <span m="951060">this</span> <span m="951300">is</span> <span
  m="951450">the</span> <span m="951630">equivalent</span> <span m="952830">of</span>
  <span m="953280">finding</span> <span m="954150">a</span> <span m="954330">smaller</span>
  <span m="954810">population</span> <span m="955560">of</span> <span m="955680">patients</span>
  <span m="956760">who</span> <span m="956940">have</span> <span m="957180">all</span>
  <span m="957420">had</span> <span m="957810">whatever</span> <span m="958290">answer</span>
  <span m="958680">I</span> <span m="958830">got</span> <span m="959100">for</span>
  <span m="959310">symptom</span> <span m="959760">1.</span> <span m="960960">And</span>
  <span m="961110">then</span> <span m="961260">I</span> <span m="961380">just</span>
  <span m="961620">keep</span> <span m="961920">doing</span> <span m="962250">that.</span>
  <span m="963100">And</span> <span m="963150">so</span> <span m="963390">this</span>
  <span m="963660">is</span> <span m="963840">the</span> <span m="963960">sequential</span>
  <span m="964650">application</span> <span m="965400">of</span> <span m="965520">Bayes's</span>
  <span m="965850">rule.</span> <span m="966660">And</span> <span m="966810">of</span>
  <span m="966900">course,</span> <span m="967200">it</span> <span m="967290">does</span>
  <span m="967620">depend</span> <span m="968130">on</span> <span m="968370">the</span>
  <span m="968460">conditional</span> <span m="969090">independence</span> <span m="970410">of</span>
  <span m="970620">all</span> <span m="970770">these</span> <span m="970950">symptoms.</span></p><p><span
  m="973030">But</span> <span m="973840">in</span> <span m="974020">medicine,</span>
  <span m="974830">people</span> <span m="975220">don't</span> <span m="975550">like</span>
  <span m="975820">to</span> <span m="975970">do</span> <span m="976570">math,</span>
  <span m="977620">even</span> <span m="977890">arithmetic</span> <span m="978730">much.</span>
  <span m="979600">And</span> <span m="979780">they</span> <span m="979930">prefer</span>
  <span m="980410">doing</span> <span m="980800">addition</span> <span m="981280">rather</span>
  <span m="981740">than</span> <span m="982330">multiplication,</span> <span m="983530">because</span>
  <span m="983950">it's</span> <span m="984130">easier.</span> <span m="985400">And</span>
  <span m="985450">so</span> <span m="986050">what</span> <span m="986320">they've</span>
  <span m="986560">done</span> <span m="986860">is</span> <span m="987040">they</span>
  <span m="987220">said,</span> <span m="987590">well,</span> <span m="988250">instead</span>
  <span m="988600">of</span> <span m="988750">representing</span> <span m="989800">all</span>
  <span m="989980">this</span> <span m="990220">data</span> <span m="990820">in</span>
  <span m="991270">a</span> <span m="991510">probabilistic</span> <span m="992770">framework,</span>
  <span m="993400">let's</span> <span m="993640">represent</span> <span m="994060">it</span>
  <span m="994480">as</span> <span m="994690">odds.</span> <span m="996550">And</span>
  <span m="996910">if</span> <span m="997120">you</span> <span m="997270">represent
  it</span> <span m="997980">as</span> <span m="998200">odds,</span> <span m="999890">then</span>
  <span m="1000970">the</span> <span m="1004780">odds</span> <span m="1005470">of</span>
  <span m="1005650">some</span> <span m="1005980">disease</span> <span m="1006580">given</span>
  <span m="1006940">a</span> <span m="1007000">bunch</span> <span m="1007300">of</span>
  <span m="1007420">symptoms,</span> <span m="1008320">given</span> <span m="1008680">the</span>
  <span m="1008830">independence</span> <span m="1009520">assumption,</span> <span
  m="1010520">is</span> <span m="1010780">just</span> <span m="1011050">the</span>
  <span m="1011140">prior</span> <span m="1011590">odds</span> <span m="1011920">of</span>
  <span m="1012040">the</span> <span m="1012190">disease</span> <span m="1013720">times</span>
  <span m="1014410">the</span> <span m="1014650">conditional</span> <span m="1015460">odds,</span>
  <span m="1016440">the</span> <span m="1016540">likelihood</span> <span m="1017110">ratio</span>
  <span m="1018160">of</span> <span m="1018610">each</span> <span m="1018850">of</span>
  <span m="1018970">the</span> <span m="1019090">symptoms</span> <span m="1019690">that</span>
  <span m="1019900">you've</span> <span m="1020080">observed.</span></p><p><span m="1020560">So</span>
  <span m="1020740">you've</span> <span m="1020860">just</span> <span m="1021070">got</span>
  <span m="1021280">to</span> <span m="1021400">multiply</span> <span m="1022030">these</span>
  <span m="1022270">together.</span> <span m="1023410">And</span> <span m="1023530">then</span>
  <span m="1023770">because</span> <span m="1024160">they</span> <span m="1024339">like</span>
  <span m="1024670">adding</span> <span m="1025060">more</span> <span m="1025270">than</span>
  <span m="1025450">multiplying,</span> <span m="1026230">they</span> <span m="1026410">said,</span>
  <span m="1026750">let's</span> <span m="1026920">take</span> <span m="1027190">the</span>
  <span m="1027339">log</span> <span m="1027760">of</span> <span m="1027880">both</span>
  <span m="1028180">sides.</span> <span m="1030250">And</span> <span m="1030400">then</span>
  <span m="1030579">you</span> <span m="1030700">can</span> <span m="1030880">just</span>
  <span m="1031180">add</span> <span m="1031390">them.</span></p><p><span m="1032650">And</span>
  <span m="1032800">so</span> <span m="1033280">if</span> <span m="1033490">you</span>
  <span m="1034089">remember</span> <span m="1034630">when</span> <span m="1034839">I</span>
  <span m="1034930">was</span> <span m="1035140">talking</span> <span m="1035560">about</span>
  <span m="1035829">medical</span> <span m="1036280">data,</span> <span m="1038109">there</span>
  <span m="1038380">are</span> <span m="1038500">things</span> <span m="1038859">like</span>
  <span m="1039490">the</span> <span m="1039640">Glasgow</span> <span m="1040180">Coma</span>
  <span m="1040540">score,</span> <span m="1041109">or</span> <span m="1041230">the</span>
  <span m="1041440">APACHE</span> <span m="1041950">score,</span> <span m="1042490">or</span>
  <span m="1043240">various</span> <span m="1044109">measures</span> <span m="1044829">of</span>
  <span m="1045069">how</span> <span m="1045339">badly</span> <span m="1045910">or</span>
  <span m="1046060">well</span> <span m="1046319">a</span> <span m="1046390">patient</span>
  <span m="1046869">is</span> <span m="1047020">doing</span> <span m="1048099">that</span>
  <span m="1048310">often</span> <span m="1048730">involve</span> <span m="1049300">adding</span>
  <span m="1049750">up</span> <span m="1049930">numbers</span> <span m="1050530">corresponding</span>
  <span m="1051940">to</span> <span m="1052120">different</span> <span m="1052510">conditions</span>
  <span m="1053170">that</span> <span m="1053350">they</span> <span m="1053530">have.</span></p><p><span
  m="1054590">And</span> <span m="1054940">what</span> <span m="1055210">they're</span>
  <span m="1055390">doing</span> <span m="1055840">is</span> <span m="1056020">exactly</span>
  <span m="1056650">this.</span> <span m="1057160">They're</span> <span m="1057400">applying</span>
  <span m="1058450">sequentially</span> <span m="1059410">Bayes's</span> <span m="1059830">rule</span>
  <span m="1060730">with</span> <span m="1061030">these</span> <span m="1061330">independence</span>
  <span m="1062020">assumptions</span> <span m="1063250">in</span> <span m="1063460">the</span>
  <span m="1063550">form</span> <span m="1063940">of</span> <span m="1064420">logs</span>
  <span m="1065050">rather</span> <span m="1065500">than</span> <span m="1066130">multiplications,</span>
  <span m="1067420">log</span> <span m="1067750">odds,</span> <span m="1068650">and</span>
  <span m="1068830">that's</span> <span m="1069070">how</span> <span m="1069220">they're</span>
  <span m="1069400">doing</span> <span m="1069700">it.</span></p><p><span m="1072460">Very</span>
  <span m="1072730">quickly.</span> <span m="1075250">Somebody</span> <span m="1076420">in</span>
  <span m="1076660">a</span> <span m="1076750">previous</span> <span m="1077230">lecture</span>
  <span m="1077680">was</span> <span m="1077890">wondering</span> <span m="1078370">about</span>
  <span m="1080110">receiver</span> <span m="1080680">operator</span> <span m="1081190">characteristic</span>
  <span m="1081940">curves.</span> <span m="1082990">And</span> <span m="1083200">I</span>
  <span m="1083350">just</span> <span m="1083650">wanted</span> <span m="1083950">to</span>
  <span m="1084070">give</span> <span m="1084280">you</span> <span m="1084400">a</span>
  <span m="1084460">little</span> <span m="1084700">bit</span> <span m="1084850">of</span>
  <span m="1084970">insight</span> <span m="1085420">on</span> <span m="1085570">those.</span>
  <span m="1085880">So</span> <span m="1086770">if</span> <span m="1086950">you</span>
  <span m="1087070">do</span> <span m="1087280">a</span> <span m="1087340">test</span>
  <span m="1087820">on</span> <span m="1088600">two</span> <span m="1088810">populations</span>
  <span m="1089680">of</span> <span m="1089770">patients--</span> <span m="1090880">the</span>
  <span m="1091000">red</span> <span m="1091240">ones</span> <span m="1091600">are</span>
  <span m="1091720">sick</span> <span m="1092020">patients.</span> <span m="1092620">The</span>
  <span m="1092740">blue</span> <span m="1093010">ones</span> <span m="1093370">are</span>
  <span m="1093850">not</span> <span m="1094120">sick</span> <span m="1094420">patients.</span>
  <span m="1096130">You</span> <span m="1096310">do</span> <span m="1096490">some</span>
  <span m="1096760">test.</span> <span m="1097150">What</span> <span m="1097360">you</span>
  <span m="1097510">expect</span> <span m="1098260">is</span> <span m="1098500">that</span>
  <span m="1098800">the</span> <span m="1098920">result</span> <span m="1099490">of</span>
  <span m="1099610">that</span> <span m="1099850">test</span> <span m="1100750">will</span>
  <span m="1100930">be</span> <span m="1101110">some</span> <span m="1101350">continuous</span>
  <span m="1102010">number,</span> <span m="1103000">and</span> <span m="1103180">it'll</span>
  <span m="1103420">be</span> <span m="1103570">distributed</span> <span m="1104320">something</span>
  <span m="1104770">like</span> <span m="1105070">the</span> <span m="1105190">blue</span>
  <span m="1105430">distribution</span> <span m="1106270">for</span> <span m="1106510">the</span>
  <span m="1106630">well</span> <span m="1106930">patients</span> <span m="1108010">and</span>
  <span m="1108160">something</span> <span m="1108550">like</span> <span m="1108790">the</span>
  <span m="1108910">red</span> <span m="1109150">distribution</span> <span m="1109900">for</span>
  <span m="1110110">the ill</span> <span m="1110440">patients.</span></p><p><span
  m="1111550">And</span> <span m="1111700">typically,</span> <span m="1112840">we</span>
  <span m="1113020">choose</span> <span m="1113410">some</span> <span m="1113740">threshold.</span>
  <span m="1115190">And</span> <span m="1115270">we</span> <span m="1115420">say,</span>
  <span m="1115720">well,</span> <span m="1117340">if</span> <span m="1117580">you</span>
  <span m="1118360">choose</span> <span m="1118780">this</span> <span m="1119110">to</span>
  <span m="1119260">be</span> <span m="1119410">the</span> <span m="1119560">threshold</span>
  <span m="1120280">between</span> <span m="1121340">a</span> <span m="1121450">prediction</span>
  <span m="1122020">of</span> <span m="1122620">sick</span> <span m="1123040">or</span>
  <span m="1123760">well,</span> <span m="1124750">then</span> <span m="1125200">what</span>
  <span m="1125500">you're</span> <span m="1125650">going</span> <span m="1125800">to</span>
  <span m="1125890">get</span> <span m="1126430">is</span> <span m="1126730">that</span>
  <span m="1126940">the</span> <span m="1127060">part</span> <span m="1127420">of</span>
  <span m="1127540">the</span> <span m="1127660">blue</span> <span m="1127930">distribution</span>
  <span m="1128800">that</span> <span m="1129130">lies</span> <span m="1129520">to</span>
  <span m="1129670">the</span> <span m="1129790">right</span> <span m="1130810">is</span>
  <span m="1131020">the</span> <span m="1131140">false</span> <span m="1131500">positives</span>
  <span m="1132820">and</span> <span m="1133000">the</span> <span m="1133090">part</span>
  <span m="1133360">of</span> <span m="1133480">the</span> <span m="1133600">red</span>
  <span m="1133850">distribution</span> <span m="1134650">that</span> <span m="1134830">lies</span>
  <span m="1135190">to</span> <span m="1135310">the</span> <span m="1135460">left</span>
  <span m="1136030">is</span> <span m="1136270">the</span> <span m="1136390">false</span>
  <span m="1136750">negatives.</span> <span m="1139240">And</span> <span m="1139570">often</span>
  <span m="1139990">people</span> <span m="1140410">will</span> <span m="1140650">choose</span>
  <span m="1141580">the</span> <span m="1141730">lowest</span> <span m="1142210">point</span>
  <span m="1142630">at</span> <span m="1142780">which</span> <span m="1143050">these</span>
  <span m="1143320">two</span> <span m="1143500">curves</span> <span m="1143950">intersect</span>
  <span m="1144610">as</span> <span m="1144880">the</span> <span m="1144970">threshold,</span>
  <span m="1146110">but</span> <span m="1146320">that,</span> <span m="1146530">of</span>
  <span m="1146650">course,</span> <span m="1147010">isn't</span> <span m="1147310">necessarily</span>
  <span m="1148000">the</span> <span m="1148120">case.</span></p><p><span m="1149440">Now,</span>
  <span m="1149770">if</span> <span m="1149980">I</span> <span m="1150100">give</span>
  <span m="1150340">you</span> <span m="1150490">a</span> <span m="1150580">better</span>
  <span m="1150910">test,</span> <span m="1151630">one</span> <span m="1151870">like</span>
  <span m="1152140">this,</span> <span m="1153430">that's</span> <span m="1153760">terrific,</span>
  <span m="1154360">because</span> <span m="1154730">there</span> <span m="1154870">is</span>
  <span m="1155050">essentially</span> <span m="1155680">no</span> <span m="1156040">overlap.</span>
  <span m="1157180">Very</span> <span m="1157450">small</span> <span m="1158290">false</span>
  <span m="1158650">negative</span> <span m="1159100">and</span> <span m="1159220">false</span>
  <span m="1159550">positive</span> <span m="1160060">rates.</span> <span m="1161860">And</span>
  <span m="1162040">as</span> <span m="1162190">I</span> <span m="1162310">said,</span>
  <span m="1162640">you</span> <span m="1162760">can</span> <span m="1162970">choose</span>
  <span m="1163330">to</span> <span m="1163450">put</span> <span m="1163690">the</span>
  <span m="1163840">threshold</span> <span m="1164470">in</span> <span m="1164590">different</span>
  <span m="1164980">places,</span> <span m="1166090">depending</span> <span m="1166660">on</span>
  <span m="1166780">how</span> <span m="1166990">you</span> <span m="1167110">want</span>
  <span m="1167290">to</span> <span m="1167350">trade</span> <span m="1167610">off</span>
  <span m="1167830">sensitivity</span> <span m="1168550">and</span> <span m="1168670">specificity.</span></p><p><span
  m="1170380">And</span> <span m="1170530">we</span> <span m="1170680">measure</span>
  <span m="1171100">this</span> <span m="1171850">by</span> <span m="1172120">this</span>
  <span m="1172360">receiver</span> <span m="1172840">operator</span> <span m="1173350">characteristics</span>
  <span m="1174220">curve,</span> <span m="1175640">which</span> <span m="1175840">has</span>
  <span m="1176140">the</span> <span m="1176590">general</span> <span m="1177070">form</span>
  <span m="1178000">that</span> <span m="1179350">if</span> <span m="1179590">you</span>
  <span m="1179770">get</span> <span m="1180340">a</span> <span m="1180400">curve</span>
  <span m="1180790">like</span> <span m="1181120">this,</span> <span m="1182170">that</span>
  <span m="1182410">means</span> <span m="1182770">that</span> <span m="1182980">there's</span>
  <span m="1183310">an</span> <span m="1183460">exact</span> <span m="1183910">trade-off</span>
  <span m="1184510">for</span> <span m="1184720">sensitivity</span> <span m="1185470">and</span>
  <span m="1185590">specificity,</span> <span m="1186970">which</span> <span m="1187240">is</span>
  <span m="1187390">the</span> <span m="1187510">case</span> <span m="1187870">if</span>
  <span m="1188020">you're</span> <span m="1188200">flipping</span> <span m="1188620">coins.</span>
  <span m="1190220">So</span> <span m="1190390">it's</span> <span m="1190570">random.</span></p><p><span
  m="1192070">And</span> <span m="1192280">of</span> <span m="1192400">course,</span>
  <span m="1192850">if</span> <span m="1193060">you</span> <span m="1193660">manage</span>
  <span m="1194110">to</span> <span m="1194260">hit</span> <span m="1194470">the</span>
  <span m="1194620">top</span> <span m="1194950">corner</span> <span m="1195400">up</span>
  <span m="1195610">there,</span> <span m="1196400">that</span> <span m="1196540">means</span>
  <span m="1196840">that</span> <span m="1197050">there</span> <span m="1197230">would</span>
  <span m="1197380">be</span> <span m="1197560">no</span> <span m="1197860">overlap</span>
  <span m="1198430">whatsoever</span> <span m="1199150">between</span> <span m="1199600">the</span>
  <span m="1199720">two</span> <span m="1199900">distributions,</span> <span m="1201190">and</span>
  <span m="1201340">you</span> <span m="1201490">would</span> <span m="1201640">get</span>
  <span m="1201880">a</span> <span m="1201940">perfect</span> <span m="1202360">result.</span>
  <span m="1203350">And</span> <span m="1203500">so</span> <span m="1203740">typically</span>
  <span m="1204310">you</span> <span m="1204430">get</span> <span m="1204670">something</span>
  <span m="1205150">in</span> <span m="1205270">between.</span> <span m="1206570">And</span>
  <span m="1206650">so</span> <span m="1207190">normally,</span> <span m="1208000">if</span>
  <span m="1208210">you</span> <span m="1208360">do</span> <span m="1208570">a</span>
  <span m="1208630">study</span> <span m="1209110">and</span> <span m="1209260">your</span>
  <span m="1209620">AUC,</span> <span m="1211390">the</span> <span m="1211660">area</span>
  <span m="1212170">under</span> <span m="1212440">this</span> <span m="1212740">receiver</span>
  <span m="1213250">operator</span> <span m="1213760">characteristics</span> <span
  m="1214600">curve,</span> <span m="1215530">is</span> <span m="1216280">barely</span>
  <span m="1216790">over</span> <span m="1217120">a</span> <span m="1217180">half,</span>
  <span m="1217930">you're</span> <span m="1218140">pretty</span> <span m="1218440">close</span>
  <span m="1218800">to</span> <span m="1218950">worthless,</span> <span m="1220150">whereas</span>
  <span m="1220570">if</span> <span m="1220720">it's</span> <span m="1220900">close</span>
  <span m="1221260">to</span> <span m="1221380">1,</span> <span m="1221770">then</span>
  <span m="1222010">you</span> <span m="1222160">have</span> <span m="1222370">a</span>
  <span m="1222430">really</span> <span m="1222760">good</span> <span m="1223870">method</span>
  <span m="1224260">for</span> <span m="1225040">distinguishing</span> <span m="1225880">these</span>
  <span m="1226510">categories</span> <span m="1227500">of</span> <span m="1227650">patients.</span></p><p><span
  m="1231040">Next</span> <span m="1231310">topic.</span> <span m="1232420">What</span>
  <span m="1232600">does</span> <span m="1232750">it</span> <span m="1232870">mean</span>
  <span m="1233140">to</span> <span m="1233290">be</span> <span m="1233440">rational?</span>
  <span m="1238084">I</span> <span m="1238590">should</span> <span m="1238800">have</span>
  <span m="1238980">a</span> <span m="1239040">philosophy</span> <span m="1239670">course</span>
  <span m="1240090">here.</span></p><p><span m="1243164">AUDIENCE:</span> <span m="1243283">Are</span>
  <span m="1243402">you</span> <span m="1243521">talking</span> <span m="1243640">about
  pi?</span></p><p><span m="1244810">PETER SZOLOVITS:</span> <span m="1245005">Sorry.</span></p><p><span
  m="1245200">AUDIENCE:</span> <span m="1245298">Are</span> <span m="1245396">you</span>
  <span m="1245494">talking</span> <span m="1245595">about</span> <span m="1245990">pi?</span>
  <span m="1246540">Pi is--</span></p><p><span m="1247870">PETER SZOLOVITS:</span>
  <span m="1248015">Pi</span> <span m="1248890">is</span> <span m="1249040">irrational,</span>
  <span m="1249910">but</span> <span m="1250090">that's</span> <span m="1250360">not</span>
  <span m="1250570">what</span> <span m="1250720">I'm</span> <span m="1250870">talking</span>
  <span m="1251290">about.</span></p><p><span m="1254170">Well,</span> <span m="1254380">so</span>
  <span m="1254560">there</span> <span m="1254770">is</span> <span m="1254830">this</span>
  <span m="1255040">principle</span> <span m="1255640">of</span> <span m="1255760">rationality</span>
  <span m="1256870">that</span> <span m="1257140">says</span> <span m="1257530">that</span>
  <span m="1259000">what</span> <span m="1259270">you</span> <span m="1259420">want</span>
  <span m="1259720">to</span> <span m="1259870">do</span> <span m="1260410">is</span>
  <span m="1260620">to</span> <span m="1260800">act</span> <span m="1261220">in</span>
  <span m="1261340">such</span> <span m="1261640">a</span> <span m="1261700">way</span>
  <span m="1261940">as</span> <span m="1262090">to</span> <span m="1262210">maximize</span>
  <span m="1262900">your</span> <span m="1263050">expected</span> <span m="1263590">utility.</span>
  <span m="1264950">So</span> <span m="1265060">for</span> <span m="1265210">example,</span>
  <span m="1265790">if</span> <span m="1265840">you're</span> <span m="1265990">a</span>
  <span m="1266050">gambler</span> <span m="1267100">and</span> <span m="1267280">you</span>
  <span m="1267430">have</span> <span m="1267610">a</span> <span m="1267670">choice</span>
  <span m="1268120">of</span> <span m="1268180">various</span> <span m="1268750">ways</span>
  <span m="1269200">of</span> <span m="1269770">betting</span> <span m="1270280">in</span>
  <span m="1270460">some</span> <span m="1270850">poker</span> <span m="1271270">game</span>
  <span m="1271600">or</span> <span m="1271720">something,</span> <span m="1272740">then</span>
  <span m="1273250">if</span> <span m="1273460">you</span> <span m="1273610">were</span>
  <span m="1273820">a</span> <span m="1273880">perfect</span> <span m="1274300">calculator</span>
  <span m="1275200">of</span> <span m="1275410">the</span> <span m="1275590">odds</span>
  <span m="1276070">of</span> <span m="1276220">getting</span> <span m="1276760">a</span>
  <span m="1278680">queen</span> <span m="1279340">on</span> <span m="1279550">your</span>
  <span m="1279700">next</span> <span m="1280000">draw,</span> <span m="1280960">then</span>
  <span m="1281290">you</span> <span m="1281440">could</span> <span m="1281650">make</span>
  <span m="1281950">some</span> <span m="1282220">rational</span> <span m="1282760">decision</span>
  <span m="1283360">about</span> <span m="1283720">whether</span> <span m="1284050">to</span>
  <span m="1284200">bet</span> <span m="1284470">more</span> <span m="1284860">or</span>
  <span m="1285070">less,</span> <span m="1286180">but</span> <span m="1286450">you'd</span>
  <span m="1286600">also</span> <span m="1286960">have</span> <span m="1287170">to</span>
  <span m="1287290">take</span> <span m="1287590">into</span> <span m="1287890">account</span>
  <span m="1288310">things</span> <span m="1288640">like,</span> <span m="1290200">&quot;How</span>
  <span m="1291310">could</span> <span m="1291550">I</span> <span m="1291670">convince</span>
  <span m="1292360">my</span> <span m="1293170">opponent</span> <span m="1293800">that</span>
  <span m="1294010">I</span> <span m="1294610">am</span> <span m="1294760">not</span>
  <span m="1295060">bluffing</span> <span m="1296620">if</span> <span m="1296890">I</span>
  <span m="1297550">am</span> <span m="1297760">bluffing?&quot;</span> <span m="1298480">and</span>
  <span m="1298660">&quot;How</span> <span m="1298870">could</span> <span m="1299080">I</span>
  <span m="1299200">convince</span> <span m="1299710">them</span> <span m="1299890">that</span>
  <span m="1300580">I'm</span> <span m="1300940">bluffing</span> <span m="1301480">if</span>
  <span m="1301680">I'm</span> <span m="1301810">not</span> <span m="1302080">bluffing?&quot;</span>
  <span m="1302650">and</span> <span m="1302800">so</span> <span m="1303040">on.</span></p><p><span
  m="1304040">So</span> <span m="1304390">there</span> <span m="1304630">is</span>
  <span m="1304930">a</span> <span m="1305050">complicated</span> <span m="1305860">model</span>
  <span m="1306280">there.</span> <span m="1307130">But</span> <span m="1307270">nevertheless,</span>
  <span m="1307960">the</span> <span m="1308140">idea</span> <span m="1308530">is</span>
  <span m="1308800">that</span> <span m="1309010">you</span> <span m="1309100">should</span>
  <span m="1309340">behave</span> <span m="1309760">in</span> <span m="1309880">a</span>
  <span m="1309940">way</span> <span m="1310690">that</span> <span m="1310900">will</span>
  <span m="1311080">give</span> <span m="1311320">you</span> <span m="1311440">the</span>
  <span m="1311590">best</span> <span m="1312310">expected</span> <span m="1312910">outcome.</span>
  <span m="1314450">And</span> <span m="1314500">so</span> <span m="1315160">people</span>
  <span m="1315520">joke</span> <span m="1315880">that</span> <span m="1316090">this</span>
  <span m="1316360">is</span> <span m="1316510">Homo</span> <span m="1317110">economicus,</span>
  <span m="1318490">because</span> <span m="1319150">economists</span> <span m="1320020">make</span>
  <span m="1320350">the</span> <span m="1320470">assumption</span> <span m="1321100">that</span>
  <span m="1321310">this</span> <span m="1321550">is</span> <span m="1321700">how</span>
  <span m="1321910">people</span> <span m="1322270">behave.</span> <span m="1323680">And</span>
  <span m="1323860">we</span> <span m="1324220">now</span> <span m="1324520">know</span>
  <span m="1324940">that</span> <span m="1325150">that's</span> <span m="1325420">not</span>
  <span m="1325660">really</span> <span m="1325960">how</span> <span m="1326140">people</span>
  <span m="1326530">behave.</span> <span m="1327140">But</span> <span m="1327250">it's</span>
  <span m="1327610">a</span> <span m="1327670">pretty</span> <span m="1327970">common</span>
  <span m="1328420">model</span> <span m="1329350">of</span> <span m="1329500">their</span>
  <span m="1329710">behavior,</span> <span m="1330310">because</span> <span m="1330730">it's</span>
  <span m="1330910">easy</span> <span m="1331180">to</span> <span m="1331270">compute,</span>
  <span m="1332290">and</span> <span m="1332440">it</span> <span m="1332530">has</span>
  <span m="1332770">some</span> <span m="1333010">appropriate</span> <span m="1333610">characteristics.</span></p><p><span
  m="1336520">So</span> <span m="1337300">as</span> <span m="1337480">I</span> <span
  m="1337570">mentioned,</span> <span m="1338050">every</span> <span m="1338350">action</span>
  <span m="1338770">has</span> <span m="1339040">a</span> <span m="1339070">cost.</span>
  <span m="1340180">And</span> <span m="1340660">utility</span> <span m="1341410">measures</span>
  <span m="1341980">the</span> <span m="1342130">value</span> <span m="1342660">or</span>
  <span m="1342810">the</span> <span m="1342970">goodness</span> <span m="1343540">of</span>
  <span m="1343660">some</span> <span m="1343900">outcome,</span> <span m="1345020">which</span>
  <span m="1345220">is</span> <span m="1345460">the</span> <span m="1345880">amount</span>
  <span m="1346150">of</span> <span m="1346270">money</span> <span m="1346540">you've</span>
  <span m="1346840">won,</span> <span m="1347260">or</span> <span m="1347500">whether</span>
  <span m="1347860">you</span> <span m="1348040">live</span> <span m="1348280">or</span>
  <span m="1348400">die,</span> <span m="1348940">or</span> <span m="1349660">quality</span>
  <span m="1350170">adjusted</span> <span m="1350710">life</span> <span m="1351060">years,</span>
  <span m="1351550">or</span> <span m="1352270">various</span> <span m="1352720">other</span>
  <span m="1352990">measures</span> <span m="1353500">of</span> <span m="1353620">utility--</span>
  <span m="1355780">how</span> <span m="1355900">much</span> <span m="1356170">it</span>
  <span m="1356290">costs</span> <span m="1357070">for</span> <span m="1357340">your</span>
  <span m="1357520">hospitalization.</span></p><p><span m="1359370">So</span> <span
  m="1359440">let</span> <span m="1359560">me</span> <span m="1359650">give</span>
  <span m="1359830">you</span> <span m="1359950">an</span> <span m="1360070">example.</span>
  <span m="1360770">This</span> <span m="1361090">actually</span> <span m="1361570">comes</span>
  <span m="1362050">from</span> <span m="1363040">a</span> <span m="1363220">decision</span>
  <span m="1363760">analysis</span> <span m="1364360">service</span> <span m="1365200">at</span>
  <span m="1365410">New</span> <span m="1365680">England</span> <span m="1365830">Medical</span>
  <span m="1366280">Center</span> <span m="1367540">Tufts</span> <span m="1367930">Hospital</span>
  <span m="1369010">in</span> <span m="1369190">the</span> <span m="1369280">late</span>
  <span m="1369520">1970s.</span> <span m="1370580">So</span> <span m="1370660">this</span>
  <span m="1370900">was</span> <span m="1371110">an</span> <span m="1371290">elderly</span>
  <span m="1371770">Chinese</span> <span m="1372280">gentleman</span> <span m="1373300">whose</span>
  <span m="1373600">foot</span> <span m="1374230">had</span> <span m="1374530">gangrene.</span>
  <span m="1375460">So</span> <span m="1375670">gangrene</span> <span m="1376240">is</span>
  <span m="1376420">an</span> <span m="1376540">infection</span> <span m="1377230">that</span>
  <span m="1379120">usually</span> <span m="1379720">people</span> <span m="1380170">who</span>
  <span m="1380350">have</span> <span m="1380530">bad</span> <span m="1380830">circulation</span>
  <span m="1382570">can</span> <span m="1382810">get</span> <span m="1383080">these.</span>
  <span m="1384010">And</span> <span m="1384280">what</span> <span m="1384490">he</span>
  <span m="1384640">was</span> <span m="1384850">facing</span> <span m="1385690">was</span>
  <span m="1386020">a</span> <span m="1386080">choice</span> <span m="1386590">of</span>
  <span m="1386740">whether</span> <span m="1387040">to</span> <span m="1387220">amputate</span>
  <span m="1387730">his</span> <span m="1387910">foot</span> <span m="1389020">or</span>
  <span m="1389230">to</span> <span m="1389410">try</span> <span m="1389680">to</span>
  <span m="1390040">treat</span> <span m="1390310">him</span> <span m="1390460">medically.</span>
  <span m="1392260">To</span> <span m="1392440">treat</span> <span m="1392710">him</span>
  <span m="1392800">medically</span> <span m="1393880">means</span> <span m="1394330">injecting</span>
  <span m="1395050">antibiotics</span> <span m="1396130">into</span> <span m="1396520">his</span>
  <span m="1396580">system</span> <span m="1397600">and</span> <span m="1397780">hoping</span>
  <span m="1398260">that</span> <span m="1398470">his</span> <span m="1398530">circulation</span>
  <span m="1399370">is</span> <span m="1399550">good</span> <span m="1399760">enough</span>
  <span m="1400090">to</span> <span m="1400210">get</span> <span m="1400540">them</span>
  <span m="1400780">to</span> <span m="1400930">the</span> <span m="1401110">infected</span>
  <span m="1401680">areas.</span></p><p><span m="1403490">And</span> <span m="1403570">so</span>
  <span m="1405520">the</span> <span m="1405880">choice</span> <span m="1406360">becomes</span>
  <span m="1406810">a</span> <span m="1406870">little</span> <span m="1407080">more</span>
  <span m="1407290">complicated,</span> <span m="1408520">because</span> <span m="1409000">if</span>
  <span m="1409180">the</span> <span m="1409300">medical</span> <span m="1409720">treatment</span>
  <span m="1410170">fails,</span> <span m="1411470">then,</span> <span m="1411580">of</span>
  <span m="1411670">course,</span> <span m="1411970">the</span> <span m="1412090">patient</span>
  <span m="1412540">may</span> <span m="1412720">die,</span> <span m="1413720">a</span>
  <span m="1413860">bad</span> <span m="1414220">outcome.</span> <span m="1415360">Or</span>
  <span m="1415870">you</span> <span m="1416050">may</span> <span m="1416290">have</span>
  <span m="1416530">to</span> <span m="1416680">now</span> <span m="1417040">amputate</span>
  <span m="1417670">the</span> <span m="1417790">whole</span> <span m="1418000">leg,</span>
  <span m="1418420">because</span> <span m="1418840">the</span> <span m="1418960">gangrene</span>
  <span m="1419470">has</span> <span m="1419650">spread</span> <span m="1420640">from</span>
  <span m="1420880">his</span> <span m="1421060">foot</span> <span m="1421720">up</span>
  <span m="1421970">the</span> <span m="1422080">foot,</span> <span m="1422560">and</span>
  <span m="1422770">now</span> <span m="1423040">you're</span> <span m="1423430">cutting</span>
  <span m="1423760">off</span> <span m="1424000">his</span> <span m="1424120">leg.</span>
  <span m="1425240">So</span> <span m="1425320">what</span> <span m="1425530">should</span>
  <span m="1425710">you</span> <span m="1425830">do?</span> <span m="1426400">And</span>
  <span m="1426580">how</span> <span m="1426790">should</span> <span m="1427030">you</span>
  <span m="1427120">reason</span> <span m="1427480">about</span> <span m="1427840">this?</span></p><p><span
  m="1429040">So</span> <span m="1429790">Pauker's</span> <span m="1431380">staff</span>
  <span m="1432310">came</span> <span m="1432610">up</span> <span m="1432820">with</span>
  <span m="1433060">this</span> <span m="1433270">decision</span> <span m="1433750">tree.</span>
  <span m="1435370">By</span> <span m="1435580">the</span> <span m="1435670">way,</span>
  <span m="1435820">decision</span> <span m="1436390">tree</span> <span m="1436840">in</span>
  <span m="1437080">this</span> <span m="1437980">literature</span> <span m="1438610">means</span>
  <span m="1438880">something</span> <span m="1439360">different</span> <span m="1439840">from</span>
  <span m="1440680">decision</span> <span m="1441160">tree</span> <span m="1441530">in</span>
  <span m="1441720">like C4.5.</span> <span m="1445120">So</span> <span m="1445330">your</span>
  <span m="1445510">choices</span> <span m="1446110">here</span> <span m="1447010">are</span>
  <span m="1447160">to</span> <span m="1447340">amputate</span> <span m="1447910">the</span>
  <span m="1448030">foot</span> <span m="1448510">or</span> <span m="1448660">start</span>
  <span m="1449050">with</span> <span m="1449230">medical</span> <span m="1449650">care.</span>
  <span m="1451430">And</span> <span m="1451660">if</span> <span m="1451870">you</span>
  <span m="1452020">amputate</span> <span m="1452590">the</span> <span m="1452740">foot,</span>
  <span m="1453250">let's</span> <span m="1453520">say</span> <span m="1453990">there</span>
  <span m="1454140">is</span> <span m="1454330">a</span> <span m="1454390">99%</span>
  <span m="1455410">chance</span> <span m="1455830">that</span> <span m="1456040">the</span>
  <span m="1456160">patient</span> <span m="1456610">will</span> <span m="1456790">live.</span>
  <span m="1457730">There's</span> <span m="1457990">a</span> <span m="1458050">1%</span>
  <span m="1458710">chance</span> <span m="1459220">that</span> <span m="1459850">maybe</span>
  <span m="1460180">the</span> <span m="1460360">anesthesia</span> <span m="1460990">will</span>
  <span m="1461170">kill</span> <span m="1461470">him.</span></p><p><span m="1463120">And</span>
  <span m="1464230">if</span> <span m="1464590">we</span> <span m="1464980">treat</span>
  <span m="1465250">him</span> <span m="1465340">medically,</span> <span m="1467050">they</span>
  <span m="1467290">estimated</span> <span m="1467950">that</span> <span m="1468160">there</span>
  <span m="1468330">is</span> <span m="1468460">a</span> <span m="1468520">70%</span>
  <span m="1469360">chance</span> <span m="1469780">of</span> <span m="1469850">full</span>
  <span m="1470140">recovery,</span> <span m="1470830">a</span> <span m="1471160">25%</span>
  <span m="1472180">chance</span> <span m="1472600">that</span> <span m="1472810">he'd</span>
  <span m="1472990">get</span> <span m="1473230">worse,</span> <span m="1473710">a</span>
  <span m="1474000">5%</span> <span m="1474730">chance</span> <span m="1475180">that</span>
  <span m="1475360">he</span> <span m="1475450">would</span> <span m="1475600">die.</span>
  <span m="1477730">If</span> <span m="1477910">he</span> <span m="1478030">got</span>
  <span m="1478330">worse,</span> <span m="1479140">you're</span> <span m="1479440">now</span>
  <span m="1479710">faced</span> <span m="1480160">with</span> <span m="1480370">another</span>
  <span m="1481240">decision,</span> <span m="1482020">which</span> <span m="1482320">is,</span>
  <span m="1482500">do</span> <span m="1482650">we</span> <span m="1482920">amputate</span>
  <span m="1483550">the</span> <span m="1483670">whole</span> <span m="1483880">leg</span>
  <span m="1484330">or</span> <span m="1484540">continue</span> <span m="1485080">pushing</span>
  <span m="1485500">medicine?</span> <span m="1487360">And</span> <span m="1487540">again,</span>
  <span m="1487970">there</span> <span m="1488020">are</span> <span m="1488080">various</span>
  <span m="1488560">outcomes</span> <span m="1489250">with</span> <span m="1489520">various</span>
  <span m="1490000">estimated</span> <span m="1490570">probabilities.</span></p><p><span
  m="1493130">Now,</span> <span m="1493150">the</span> <span m="1493270">critical</span>
  <span m="1493810">thing</span> <span m="1494110">here</span> <span m="1494710">that</span>
  <span m="1495250">this</span> <span m="1495610">group</span> <span m="1496000">was</span>
  <span m="1496240">pushing</span> <span m="1497470">was</span> <span m="1497770">the</span>
  <span m="1497950">idea</span> <span m="1498490">that</span> <span m="1498880">these</span>
  <span m="1499240">decisions</span> <span m="1499900">shouldn't</span> <span m="1500320">be</span>
  <span m="1500500">based</span> <span m="1501040">on</span> <span m="1501340">what</span>
  <span m="1501580">the</span> <span m="1501700">doctor</span> <span m="1502180">thinks</span>
  <span m="1502570">is</span> <span m="1502750">good</span> <span m="1502960">for</span>
  <span m="1503260">you.</span> <span m="1504190">They</span> <span m="1504340">should</span>
  <span m="1504610">be</span> <span m="1504760">based</span> <span m="1505180">on</span>
  <span m="1505300">what</span> <span m="1505540">you</span> <span m="1505690">think</span>
  <span m="1506050">is</span> <span m="1506200">good</span> <span m="1506410">for</span>
  <span m="1506680">you.</span> <span m="1507580">And</span> <span m="1507730">so</span>
  <span m="1507970">they</span> <span m="1508360">worked</span> <span m="1508720">very</span>
  <span m="1509020">hard</span> <span m="1509380">to</span> <span m="1509590">try</span>
  <span m="1509860">to</span> <span m="1510040">elicit</span> <span m="1511780">individualized</span>
  <span m="1513250">utilities</span> <span m="1514240">from</span> <span m="1514600">patients.</span></p><p><span
  m="1515870">So</span> <span m="1516010">for</span> <span m="1516190">example,</span>
  <span m="1516860">this</span> <span m="1517030">guy</span> <span m="1517600">said</span>
  <span m="1519280">that</span> <span m="1520120">having</span> <span m="1520540">your</span>
  <span m="1520720">foot</span> <span m="1521020">amputated</span> <span m="1522280">was</span>
  <span m="1522550">worth</span> <span m="1522940">850</span> <span m="1523870">points</span>
  <span m="1524380">on</span> <span m="1524500">a</span> <span m="1524560">scale</span>
  <span m="1524950">of</span> <span m="1525070">1,000</span> <span m="1526180">where</span>
  <span m="1526630">being</span> <span m="1526990">healthy</span> <span m="1527470">was</span>
  <span m="1528200">1</span> <span m="1529100">and</span> <span m="1529420">being</span>
  <span m="1529750">dead</span> <span m="1530020">was</span> <span m="1530230">0.</span></p><p><span
  m="1533050">Now,</span> <span m="1533200">you</span> <span m="1533350">could</span>
  <span m="1533530">imagine</span> <span m="1534280">that</span> <span m="1534550">that</span>
  <span m="1534790">number</span> <span m="1535180">would</span> <span m="1535390">be</span>
  <span m="1535570">very</span> <span m="1535810">different</span> <span m="1536260">for</span>
  <span m="1536440">different</span> <span m="1536800">individuals.</span> <span m="1538630">If</span>
  <span m="1538780">you</span> <span m="1538930">asked</span> <span m="1539170">LeBron</span>
  <span m="1539650">James</span> <span m="1540310">how</span> <span m="1540550">bad</span>
  <span m="1540910">would</span> <span m="1541120">it</span> <span m="1541240">be</span>
  <span m="1541480">to</span> <span m="1541660">have</span> <span m="1541900">your</span>
  <span m="1542090">foot</span> <span m="1542300">amputated,</span> <span m="1543630">he</span>
  <span m="1543710">might</span> <span m="1544010">think</span> <span m="1544310">that</span>
  <span m="1544490">it's</span> <span m="1544670">much</span> <span m="1544970">worse</span>
  <span m="1545450">than</span> <span m="1545870">I</span> <span m="1546080">would,</span>
  <span m="1546420">because</span> <span m="1548090">it</span> <span m="1548180">would</span>
  <span m="1548360">be</span> <span m="1548540">a</span> <span m="1548600">pain</span>
  <span m="1549080">to</span> <span m="1549320">have</span> <span m="1549560">my</span>
  <span m="1549740">foot</span> <span m="1549980">amputated,</span> <span m="1551150">but</span>
  <span m="1551360">I</span> <span m="1551480">could</span> <span m="1551690">still</span>
  <span m="1552050">do</span> <span m="1552290">most</span> <span m="1552680">of</span>
  <span m="1552800">the</span> <span m="1552920">things</span> <span m="1553310">that</span>
  <span m="1553490">I</span> <span m="1553640">do</span> <span m="1553850">professionally,</span>
  <span m="1555320">whereas</span> <span m="1556520">he</span> <span m="1556670">probably</span>
  <span m="1557120">couldn't</span> <span m="1557660">as</span> <span m="1558380">a</span>
  <span m="1558410">star</span> <span m="1558740">basketball</span> <span m="1559370">player.</span></p><p><span
  m="1562170">So</span> <span m="1562430">how</span> <span m="1562550">do</span> <span
  m="1562640">you</span> <span m="1562760">solve</span> <span m="1563120">a</span>
  <span m="1563180">problem</span> <span m="1563600">like</span> <span m="1563840">this?</span>
  <span m="1564100">Well,</span> <span m="1564320">you</span> <span m="1564470">say,</span>
  <span m="1564890">OK,</span> <span m="1565940">at</span> <span m="1566150">every</span>
  <span m="1566600">chance</span> <span m="1567140">node</span> <span m="1567680">I</span>
  <span m="1567860">can</span> <span m="1568070">calculate</span> <span m="1568820">the</span>
  <span m="1569330">expected</span> <span m="1569960">value</span> <span m="1570800">of</span>
  <span m="1570980">what</span> <span m="1571160">happens</span> <span m="1571640">here.</span>
  <span m="1572550">So</span> <span m="1572690">here</span> <span m="1572930">at</span>
  <span m="1572970">it's</span> <span m="1573110">0.6</span> <span m="1573770">times</span>
  <span m="1574100">995,</span> <span m="1575306">0.4</span> <span m="1576110">times</span>
  <span m="1576470">0.</span> <span m="1577400">That</span> <span m="1577610">gets</span>
  <span m="1577880">me</span> <span m="1578050">a</span> <span m="1578120">value</span>
  <span m="1578570">for</span> <span m="1578780">this</span> <span m="1579020">decision.</span></p><p><span
  m="1580100">Do</span> <span m="1580280">the</span> <span m="1580400">same</span>
  <span m="1580700">thing</span> <span m="1580970">here.</span> <span m="1581900">I</span>
  <span m="1582050">compare</span> <span m="1582680">the</span> <span m="1582830">values</span>
  <span m="1583580">here</span> <span m="1584000">and</span> <span m="1584180">choose</span>
  <span m="1584570">the</span> <span m="1584690">best</span> <span m="1585020">one.</span>
  <span m="1586040">That</span> <span m="1586250">gives</span> <span m="1586550">me</span>
  <span m="1586730">a</span> <span m="1586790">value</span> <span m="1587240">for</span>
  <span m="1587450">this</span> <span m="1587690">decision.</span> <span m="1588630">And</span>
  <span m="1588830">so</span> <span m="1589040">I</span> <span m="1589160">fold</span>
  <span m="1589550">back</span> <span m="1590390">this</span> <span m="1590660">decision</span>
  <span m="1591170">tree.</span></p><p><span m="1592880">And</span> <span m="1593240">my</span>
  <span m="1593480">next</span> <span m="1593780">slide</span> <span m="1594950">should</span>
  <span m="1595280">have--</span> <span m="1596920">yeah,</span> <span m="1597410">so</span>
  <span m="1597620">these</span> <span m="1597890">are</span> <span m="1598010">the</span>
  <span m="1598160">numbers</span> <span m="1598640">that</span> <span m="1598850">you</span>
  <span m="1598970">get.</span> <span m="1599840">And</span> <span m="1599990">what</span>
  <span m="1600230">you</span> <span m="1600350">discover</span> <span m="1601520">is</span>
  <span m="1601820">that</span> <span m="1602090">the</span> <span m="1602210">utility</span>
  <span m="1602870">of</span> <span m="1603020">trying</span> <span m="1603380">medical</span>
  <span m="1603860">treatment</span> <span m="1604850">is</span> <span m="1605030">somewhat</span>
  <span m="1605480">higher</span> <span m="1605840">than</span> <span m="1606080">the</span>
  <span m="1606200">utility</span> <span m="1606800">of</span> <span m="1607130">immediately</span>
  <span m="1607760">amputating</span> <span m="1608420">the</span> <span m="1608510">foot</span>
  <span m="1609320">if</span> <span m="1609530">you</span> <span m="1609680">believe</span>
  <span m="1610790">these</span> <span m="1611090">numbers</span> <span m="1611750">and</span>
  <span m="1612290">those</span> <span m="1612590">utilities,</span> <span m="1613430">these</span>
  <span m="1613670">probabilities</span> <span m="1614480">and</span> <span m="1614600">those</span>
  <span m="1614840">utilities.</span></p><p><span m="1617000">Now,</span> <span m="1617150">the</span>
  <span m="1617300">difficulty</span> <span m="1618680">is</span> <span m="1618950">that</span>
  <span m="1619250">these</span> <span m="1619550">numbers</span> <span m="1620030">are</span>
  <span m="1620150">fickle.</span> <span m="1621560">And</span> <span m="1621740">so</span>
  <span m="1622490">you'd</span> <span m="1622730">like</span> <span m="1623030">to</span>
  <span m="1623150">do</span> <span m="1623360">some</span> <span m="1623630">sort</span>
  <span m="1623870">of</span> <span m="1623990">sensitivity</span> <span m="1624680">analysis.</span>
  <span m="1625400">And</span> <span m="1625550">you</span> <span m="1625670">say,</span>
  <span m="1625910">for</span> <span m="1626150">example,</span> <span m="1626630">what</span>
  <span m="1626900">if</span> <span m="1627590">this</span> <span m="1627800">gentleman</span>
  <span m="1628340">valued</span> <span m="1629480">his</span> <span m="1630470">living</span>
  <span m="1630890">with</span> <span m="1631130">an</span> <span m="1631250">amputated</span>
  <span m="1631940">foot</span> <span m="1632420">at</span> <span m="1632630">900</span>
  <span m="1633410">rather</span> <span m="1633770">than</span> <span m="1634010">850.</span>
  <span m="1635390">And</span> <span m="1635570">now</span> <span m="1635810">you</span>
  <span m="1635960">discover</span> <span m="1637070">that</span> <span m="1637520">amputating</span>
  <span m="1638240">the</span> <span m="1638330">foot</span> <span m="1639020">looks</span>
  <span m="1639350">like</span> <span m="1639590">a</span> <span m="1639650">slightly</span>
  <span m="1640160">better</span> <span m="1640460">decision</span> <span m="1641810">than</span>
  <span m="1642770">the</span> <span m="1642890">other.</span></p><p><span m="1644450">So</span>
  <span m="1645080">this</span> <span m="1645410">is</span> <span m="1645590">actually</span>
  <span m="1647870">applied</span> <span m="1648800">in</span> <span m="1648950">clinical</span>
  <span m="1649460">medicine.</span> <span m="1650630">And</span> <span m="1650840">there</span>
  <span m="1651050">are</span> <span m="1651140">now</span> <span m="1652100">thousands</span>
  <span m="1652730">of</span> <span m="1652820">doctors</span> <span m="1653450">who</span>
  <span m="1653650">have</span> <span m="1653720">been</span> <span m="1653930">trained</span>
  <span m="1654350">in</span> <span m="1654470">these</span> <span m="1654710">techniques</span>
  <span m="1655880">and</span> <span m="1656090">really</span> <span m="1656420">try</span>
  <span m="1656690">to</span> <span m="1656810">work</span> <span m="1657110">through</span>
  <span m="1657380">this</span> <span m="1657740">with</span> <span m="1657980">individual</span>
  <span m="1658580">patients.</span></p><p><span m="1659720">Of</span> <span m="1659840">course,</span>
  <span m="1660270">it's</span> <span m="1660350">used</span> <span m="1660710">much</span>
  <span m="1661010">more</span> <span m="1661520">on</span> <span m="1661760">an</span>
  <span m="1661880">epidemiological</span> <span m="1663020">basis</span> <span m="1663530">when</span>
  <span m="1663740">people</span> <span m="1664100">look</span> <span m="1664340">at</span>
  <span m="1664460">large</span> <span m="1664760">populations.</span></p><p><span
  m="1666474">AUDIENCE:</span> <span m="1666575">I</span> <span m="1666676">have</span>
  <span m="1666777">a</span> <span m="1666881">question.</span></p><p><span m="1667290">PETER
  SZOLOVITS:</span> <span m="1667375">Yeah.</span></p><p><span m="1667902">AUDIENCE:</span>
  <span m="1668012">How</span> <span m="1668122">are</span> <span m="1668232">the</span>
  <span m="1668344">probabilities</span> <span m="1670112">assessed?</span></p><p><span
  m="1675360">PETER SZOLOVITS:</span> <span m="1675485">So</span> <span m="1675610">the</span>
  <span m="1675950">service</span> <span m="1676580">that</span> <span m="1676760">did</span>
  <span m="1677060">this</span> <span m="1677240">study</span> <span m="1678110">would</span>
  <span m="1678380">read</span> <span m="1678650">the</span> <span m="1678770">literature,</span>
  <span m="1679610">and</span> <span m="1679820">they</span> <span m="1680000">would</span>
  <span m="1680180">look</span> <span m="1680450">in</span> <span m="1680570">databases.</span>
  <span m="1681530">And</span> <span m="1681650">they</span> <span m="1681800">would</span>
  <span m="1681950">try</span> <span m="1682190">to</span> <span m="1682310">estimate</span>
  <span m="1682850">those</span> <span m="1683090">probabilities.</span> <span m="1684410">We</span>
  <span m="1684560">can</span> <span m="1684740">do</span> <span m="1684950">a</span>
  <span m="1685010">lot</span> <span m="1685250">better</span> <span m="1685580">today</span>
  <span m="1686060">than</span> <span m="1686300">they</span> <span m="1686510">could</span>
  <span m="1687530">at</span> <span m="1687920">that</span> <span m="1688130">time,</span>
  <span m="1688520">because</span> <span m="1688940">we</span> <span m="1689090">have</span>
  <span m="1689240">a</span> <span m="1689300">lot</span> <span m="1689540">more</span>
  <span m="1689750">data</span> <span m="1690590">that</span> <span m="1690830">you</span>
  <span m="1690920">can</span> <span m="1691130">look</span> <span m="1691400">in.</span></p><p><span
  m="1692030">But</span> <span m="1692300">you</span> <span m="1692420">could</span>
  <span m="1692630">say,</span> <span m="1693150">OK,</span> <span m="1693470">for</span>
  <span m="1694400">people--</span> <span m="1695530">men</span> <span m="1695960">of</span>
  <span m="1696140">this</span> <span m="1696470">age</span> <span m="1697550">who</span>
  <span m="1697820">have</span> <span m="1698420">gangrenous</span> <span m="1699110">feet,</span>
  <span m="1699890">what</span> <span m="1700130">fraction</span> <span m="1700760">of</span>
  <span m="1700940">them</span> <span m="1701660">have</span> <span m="1701900">the</span>
  <span m="1702020">following</span> <span m="1702560">experience?</span> <span m="1703910">And</span>
  <span m="1704000">that's</span> <span m="1704250">how</span> <span m="1704780">these</span>
  <span m="1705050">are</span> <span m="1705170">estimated.</span></p><p><span m="1706910">Some</span>
  <span m="1707210">of</span> <span m="1707360">it</span> <span m="1707930">feels</span>
  <span m="1710210">like</span> <span m="1710420">5%.</span> <span m="1718320">OK.</span>
  <span m="1718720">So</span> <span m="1718900">I</span> <span m="1719230">just</span>
  <span m="1719480">said</span> <span m="1719740">this.</span></p><p><span m="1722320">And</span>
  <span m="1722470">then</span> <span m="1722620">the</span> <span m="1722710">question</span>
  <span m="1723190">of</span> <span m="1723310">where</span> <span m="1723490">do</span>
  <span m="1723580">you</span> <span m="1723700">get</span> <span m="1723940">these</span>
  <span m="1724180">utilities</span> <span m="1724900">is</span> <span m="1725080">a</span>
  <span m="1725140">tricky</span> <span m="1725500">one.</span> <span m="1727640">So</span>
  <span m="1728410">one</span> <span m="1728680">way</span> <span m="1728950">is</span>
  <span m="1729160">to</span> <span m="1729310">do</span> <span m="1729520">the</span>
  <span m="1729670">standard</span> <span m="1730210">gamble,</span> <span m="1731600">which</span>
  <span m="1731770">says,</span> <span m="1732860">OK,</span> <span m="1734860">Mr.</span>
  <span m="1736330">Szolovits,</span> <span m="1737090">we're</span> <span m="1737530">going</span>
  <span m="1737640">to</span> <span m="1737770">play</span> <span m="1738010">this</span>
  <span m="1738250">game.</span> <span m="1740320">We're</span> <span m="1740500">going</span>
  <span m="1740860">to</span> <span m="1741550">roll</span> <span m="1742180">a</span>
  <span m="1744760">fair</span> <span m="1745150">die</span> <span m="1745540">or</span>
  <span m="1745690">something</span> <span m="1746140">that</span> <span m="1746350">will</span>
  <span m="1746530">come</span> <span m="1746830">up</span> <span m="1747490">with</span>
  <span m="1747730">some</span> <span m="1748030">continuous</span> <span m="1748720">number</span>
  <span m="1749080">between</span> <span m="1749530">0</span> <span m="1749920">and</span>
  <span m="1750070">1,</span> <span m="1751570">and</span> <span m="1752110">then</span>
  <span m="1752440">I'm</span> <span m="1752620">going</span> <span m="1752740">to</span>
  <span m="1752800">play</span> <span m="1753070">the</span> <span m="1753160">game</span>
  <span m="1753490">where</span> <span m="1754300">either</span> <span m="1755720">I</span>
  <span m="1758110">chop</span> <span m="1758470">off</span> <span m="1758710">your</span>
  <span m="1758860">foot,</span> <span m="1760720">or</span> <span m="1761290">I</span>
  <span m="1761410">roll</span> <span m="1761680">this</span> <span m="1761890">die</span>
  <span m="1762980">and</span> <span m="1763030">if</span> <span m="1763210">it</span>
  <span m="1763330">exceeds</span> <span m="1763780">some</span> <span m="1764080">threshold,</span>
  <span m="1765980">then</span> <span m="1766510">I</span> <span m="1766660">kill</span>
  <span m="1766930">you.</span> <span m="1769300">Nice</span> <span m="1769600">game.</span></p><p><span
  m="1772300">So</span> <span m="1772540">now</span> <span m="1773140">if</span> <span
  m="1774250">you</span> <span m="1774460">find</span> <span m="1774910">the</span>
  <span m="1775060">point</span> <span m="1775510">at</span> <span m="1775690">which</span>
  <span m="1775960">I'm</span> <span m="1776170">indifferent,</span> <span m="1777790">if</span>
  <span m="1777970">I</span> <span m="1778120">say,</span> <span m="1778490">well,</span>
  <span m="1779230">0.8,</span> <span m="1782680">that's</span> <span m="1782950">a</span>
  <span m="1783010">20%</span> <span m="1783790">chance</span> <span m="1784180">of</span>
  <span m="1784270">dying.</span> <span m="1785460">It</span> <span m="1785560">seems</span>
  <span m="1785890">like</span> <span m="1786130">a</span> <span m="1786160">lot.</span>
  <span m="1787780">But</span> <span m="1788080">maybe</span> <span m="1788470">I'll</span>
  <span m="1788620">go</span> <span m="1788840">for</span> <span m="1789330">0.9,</span>
  <span m="1791050">right?</span> <span m="1791920">Now</span> <span m="1792190">you've</span>
  <span m="1792370">said,</span> <span m="1792800">OK,</span> <span m="1793100">well,</span>
  <span m="1793280">that</span> <span m="1793390">means</span> <span m="1793720">that</span>
  <span m="1793930">you</span> <span m="1794140">value</span> <span m="1794710">living</span>
  <span m="1795130">without</span> <span m="1795790">a</span> <span m="1795850">foot</span>
  <span m="1796870">at</span> <span m="1797110">0.9</span> <span m="1798370">of</span>
  <span m="1798580">the</span> <span m="1798700">value</span> <span m="1799180">of</span>
  <span m="1799270">being</span> <span m="1799570">healthy.</span> <span m="1801710">So</span>
  <span m="1801790">this</span> <span m="1802060">is</span> <span m="1802240">a</span>
  <span m="1802300">way</span> <span m="1802540">of</span> <span m="1802630">doing</span>
  <span m="1802960">it.</span> <span m="1803660">And</span> <span m="1803980">this</span>
  <span m="1804190">is</span> <span m="1804460">typically</span> <span m="1805030">done.</span></p><p><span
  m="1806070">Unfortunately,</span> <span m="1808060">of</span> <span m="1808240">course,</span>
  <span m="1808600">it's</span> <span m="1809020">difficult</span> <span m="1809590">to</span>
  <span m="1810070">ascertain</span> <span m="1810445">the</span> <span m="1810820">problem.</span>
  <span m="1811810">And</span> <span m="1811930">it's</span> <span m="1812110">also</span>
  <span m="1812440">not</span> <span m="1812680">stable.</span> <span m="1813260">So</span>
  <span m="1813400">people</span> <span m="1813730">have</span> <span m="1813880">done</span>
  <span m="1814090">experiments</span> <span m="1814810">where</span> <span m="1816220">they</span>
  <span m="1816460">get</span> <span m="1816760">somebody</span> <span m="1817210">to</span>
  <span m="1817390">give</span> <span m="1817630">them</span> <span m="1817870">this</span>
  <span m="1818080">kind</span> <span m="1818380">of</span> <span m="1818470">number</span>
  <span m="1818950">as</span> <span m="1819160">a</span> <span m="1819250">hypothetical,</span>
  <span m="1820690">and</span> <span m="1820870">then</span> <span m="1821110">when</span>
  <span m="1821320">that</span> <span m="1821500">person</span> <span m="1821950">winds</span>
  <span m="1822400">up</span> <span m="1822640">actually</span> <span m="1823390">faced</span>
  <span m="1823810">with</span> <span m="1823960">such</span> <span m="1824290">a</span>
  <span m="1824350">decision,</span> <span m="1825730">they</span> <span m="1825940">no</span>
  <span m="1826120">longer</span> <span m="1826570">will</span> <span m="1827500">abide</span>
  <span m="1827920">with</span> <span m="1828130">that</span> <span m="1828330">number.</span>
  <span m="1829060">So</span> <span m="1829420">they've</span> <span m="1829720">changed</span>
  <span m="1830080">their</span> <span m="1830230">mind</span> <span m="1831550">when</span>
  <span m="1831790">the</span> <span m="1831880">situation</span> <span m="1832510">is</span>
  <span m="1832630">real.</span></p><p><span m="1834450">AUDIENCE:</span> <span m="1834545">But</span>
  <span m="1834640">it's</span> <span m="1834880">nice,</span> <span m="1835540">because</span>
  <span m="1835780">there</span> <span m="1836125">are two feet, right?</span> <span
  m="1836470">So</span> <span m="1836740">you</span> <span m="1836820">could</span>
  <span m="1836940">run</span> <span m="1837040">this</span> <span m="1837400">experiment</span>
  <span m="1837800">and</span> <span m="1838222">see.</span></p><p><span m="1839910">PETER
  SZOLOVITS:</span> <span m="1840005">They</span> <span m="1840100">didn't</span>
  <span m="1840460">actually</span> <span m="1841060">do</span> <span m="1841310">it.</span>
  <span m="1841540">It</span> <span m="1841860">was</span> <span m="1842800">hypothetical.</span>
  <span m="1846640">OK.</span></p><p><span m="1848020">Next</span> <span m="1848290">program</span>
  <span m="1848680">I</span> <span m="1848770">want</span> <span m="1848950">to</span>
  <span m="1849040">tell</span> <span m="1849250">you</span> <span m="1849400">about,</span>
  <span m="1850270">again,</span> <span m="1850900">the</span> <span m="1851140">technique</span>
  <span m="1851740">for</span> <span m="1851980">this</span> <span m="1852280">was</span>
  <span m="1852490">developed</span> <span m="1853120">as</span> <span m="1853570">a</span>
  <span m="1853630">PhD</span> <span m="1854230">thesis</span> <span m="1854770">here</span>
  <span m="1854980">at</span> <span m="1855070">MIT</span> <span m="1855580">in</span>
  <span m="1855750">1967.</span> <span m="1857290">So</span> <span m="1857470">this</span>
  <span m="1857710">is</span> <span m="1857830">hot</span> <span m="1858070">off</span>
  <span m="1858310">the</span> <span m="1858400">presses.</span> <span m="1859970">But</span>
  <span m="1860110">it's</span> <span m="1860230">still</span> <span m="1860530">used,</span>
  <span m="1861580">this</span> <span m="1861850">type</span> <span m="1862120">of</span>
  <span m="1862240">idea.</span></p><p><span m="1864190">And</span> <span m="1864370">so</span>
  <span m="1864850">this</span> <span m="1865150">was</span> <span m="1866080">a</span>
  <span m="1866170">program</span> <span m="1866680">that</span> <span m="1866860">was</span>
  <span m="1867070">published</span> <span m="1867670">in</span> <span m="1867970">the</span>
  <span m="1868360"><i>American</i></span> <span m="1868780"><i>Journal</i></span>
  <span m="1869110"><i>of</i></span> <span m="1869200"><i>Medicine,</i></span> <span
  m="1869710">which</span> <span m="1869960">is</span> <span m="1870160">a</span>
  <span m="1870700">high</span> <span m="1870940">impact</span> <span m="1871390">medical</span>
  <span m="1871840">journal.</span> <span m="1872710">I</span> <span m="1872770">think</span>
  <span m="1872980">this</span> <span m="1873190">was</span> <span m="1873400">actually</span>
  <span m="1873850">the</span> <span m="1874000">first</span> <span m="1874390">sort</span>
  <span m="1874750">of</span> <span m="1875200">computational</span> <span m="1876130">program</span>
  <span m="1876700">that</span> <span m="1877090">journal</span> <span m="1877480">had</span>
  <span m="1878440">ever</span> <span m="1878680">published</span> <span m="1879670">as</span>
  <span m="1879850">a</span> <span m="1879910">medical</span> <span m="1880300">journal.</span></p><p><span
  m="1881980">And</span> <span m="1882280">it</span> <span m="1882490">was</span>
  <span m="1882730">addressed</span> <span m="1883270">at</span> <span m="1883480">the</span>
  <span m="1883600">problem</span> <span m="1884260">of</span> <span m="1884500">the</span>
  <span m="1884950">diagnosis</span> <span m="1886300">of</span> <span m="1886510">acute</span>
  <span m="1886990">oliguric</span> <span m="1887650">renal</span> <span m="1887980">failure.</span>
  <span m="1888650">Oliguric</span> <span m="1889270">means</span> <span m="1889570">you're</span>
  <span m="1889720">not</span> <span m="1889900">peeing</span> <span m="1890320">enough.</span>
  <span m="1892030">Renal</span> <span m="1892930">is</span> <span m="1893140">your</span>
  <span m="1893290">kidney.</span> <span m="1893870">So</span> <span m="1894010">this</span>
  <span m="1894280">is</span> <span m="1894730">something's</span> <span m="1895210">gone</span>
  <span m="1895600">wrong</span> <span m="1895870">with</span> <span m="1896080">your</span>
  <span m="1896230">kidney,</span> <span m="1896650">and</span> <span m="1896830">you're</span>
  <span m="1896950">not</span> <span m="1897190">producing</span> <span m="1897790">enough</span>
  <span m="1898060">urine.</span></p><p><span m="1900160">Now,</span> <span m="1900400">this</span>
  <span m="1900700">is</span> <span m="1901630">a</span> <span m="1901720">good</span>
  <span m="1902230">problem</span> <span m="1903220">to</span> <span m="1903460">address</span>
  <span m="1903970">with</span> <span m="1904270">these</span> <span m="1904570">techniques,</span>
  <span m="1905890">because</span> <span m="1907360">if</span> <span m="1907570">something</span>
  <span m="1908020">happens</span> <span m="1908530">to</span> <span m="1908630">you</span>
  <span m="1908800">suddenly,</span> <span m="1909970">it's</span> <span m="1910180">very</span>
  <span m="1910450">likely</span> <span m="1910990">that</span> <span m="1911230">there</span>
  <span m="1911350">is</span> <span m="1911500">one</span> <span m="1911770">cause</span>
  <span m="1912220">for</span> <span m="1912490">it.</span> <span m="1914950">If</span>
  <span m="1915160">you</span> <span m="1915520">are</span> <span m="1916690">85</span>
  <span m="1917260">years</span> <span m="1917530">old</span> <span m="1917920">and</span>
  <span m="1918040">you</span> <span m="1918190">have</span> <span m="1918430">a</span>
  <span m="1918460">little</span> <span m="1918730">heart</span> <span m="1919000">disease</span>
  <span m="1919510">and</span> <span m="1919630">a</span> <span m="1919690">little</span>
  <span m="1920740">kidney</span> <span m="1921160">disease</span> <span m="1921730">and</span>
  <span m="1921880">a</span> <span m="1921940">little</span> <span m="1922300">liver</span>
  <span m="1922660">disease</span> <span m="1923260">and</span> <span m="1923410">a</span>
  <span m="1923470">little lung</span> <span m="1923740">disease,</span> <span m="1925660">there's</span>
  <span m="1925990">no</span> <span m="1926200">guarantee</span> <span m="1926890">that</span>
  <span m="1927100">there</span> <span m="1927250">was</span> <span m="1927490">one</span>
  <span m="1927730">thing</span> <span m="1928030">that</span> <span m="1928240">went</span>
  <span m="1928480">wrong</span> <span m="1928750">with</span> <span m="1928990">you</span>
  <span m="1929320">that</span> <span m="1929560">caused</span> <span m="1929980">all</span>
  <span m="1930160">these.</span></p><p><span m="1931310">But</span> <span m="1931450">if</span>
  <span m="1931630">you</span> <span m="1931750">were</span> <span m="1931930">OK</span>
  <span m="1932380">yesterday</span> <span m="1933260">and</span> <span m="1933340">then</span>
  <span m="1933520">you</span> <span m="1933670">stopped</span> <span m="1934000">peeing,</span>
  <span m="1935290">it's</span> <span m="1935590">pretty</span> <span m="1935860">likely</span>
  <span m="1936370">that</span> <span m="1936580">there's</span> <span m="1936850">one</span>
  <span m="1937090">thing</span> <span m="1937740">that's</span> <span m="1938110">gone</span>
  <span m="1938410">wrong.</span> <span m="1938790">So</span> <span m="1939040">it's</span>
  <span m="1939220">a</span> <span m="1939250">good</span> <span m="1939460">application</span>
  <span m="1940720">of</span> <span m="1940870">this</span> <span m="1941080">model.</span>
  <span m="1942260">So</span> <span m="1942310">what</span> <span m="1942490">they</span>
  <span m="1942640">said</span> <span m="1943150">is</span> <span m="1943360">there</span>
  <span m="1943510">are</span> <span m="1943570">14</span> <span m="1944050">potential</span>
  <span m="1944650">causes.</span> <span m="1945520">And</span> <span m="1945700">these</span>
  <span m="1945940">are</span> <span m="1946060">exhaustive</span> <span m="1946660">and</span>
  <span m="1946780">mutually</span> <span m="1947230">exclusive.</span></p><p><span
  m="1948830">There</span> <span m="1948900">are</span> <span m="1949660">27</span>
  <span m="1950290">tests</span> <span m="1950800">or</span> <span m="1950920">questions</span>
  <span m="1951550">or</span> <span m="1951700">observations</span> <span m="1953080">that</span>
  <span m="1953260">are</span> <span m="1953350">relevant</span> <span m="1953860">to</span>
  <span m="1954040">the</span> <span m="1954160">differential.</span> <span m="1955570">These</span>
  <span m="1955870">are</span> <span m="1955990">cheap</span> <span m="1956350">tests,</span>
  <span m="1956800">so</span> <span m="1957070">they</span> <span m="1957250">didn't</span>
  <span m="1957520">involve</span> <span m="1958480">doing</span> <span m="1958840">anything</span>
  <span m="1959470">either</span> <span m="1959770">expensive</span> <span m="1960430">or</span>
  <span m="1960550">dangerous</span> <span m="1961150">to</span> <span m="1961270">the</span>
  <span m="1961390">patient.</span> <span m="1961960">It</span> <span m="1962050">was</span>
  <span m="1962650">measuring</span> <span m="1963100">something</span> <span m="1963520">in</span>
  <span m="1963640">the</span> <span m="1963730">lab</span> <span m="1964210">or</span>
  <span m="1964510">asking</span> <span m="1964960">questions</span> <span m="1965560">of</span>
  <span m="1965680">the</span> <span m="1965800">patient.</span></p><p><span m="1967930">But</span>
  <span m="1968470">they</span> <span m="1968710">didn't</span> <span m="1968920">want</span>
  <span m="1969130">to</span> <span m="1969220">have</span> <span m="1969460">to</span>
  <span m="1969610">ask</span> <span m="1970030">all</span> <span m="1970240">of</span>
  <span m="1970390">them,</span> <span m="1970750">because</span> <span m="1971350">that's</span>
  <span m="1971590">pretty</span> <span m="1971860">tedious.</span> <span m="1973060">And</span>
  <span m="1973240">so</span> <span m="1973510">they</span> <span m="1973720">were</span>
  <span m="1973900">trying</span> <span m="1974230">to</span> <span m="1974380">minimize</span>
  <span m="1975070">the</span> <span m="1975220">amount</span> <span m="1975490">of</span>
  <span m="1975610">information</span> <span m="1976270">that</span> <span m="1976450">they</span>
  <span m="1976600">needed</span> <span m="1976930">to</span> <span m="1977110">gather</span>
  <span m="1978070">in</span> <span m="1978220">order</span> <span m="1978490">to</span>
  <span m="1978640">come</span> <span m="1978910">up</span> <span m="1979090">with</span>
  <span m="1979270">an</span> <span m="1979390">appropriate</span> <span m="1980020">decision.</span>
  <span m="1981610">Now,</span> <span m="1981910">the</span> <span m="1982060">real</span>
  <span m="1982330">problem,</span> <span m="1983320">there</span> <span m="1983560">were</span>
  <span m="1983800">three</span> <span m="1984130">invasive</span> <span m="1984730">tests</span>
  <span m="1985360">that</span> <span m="1985720">are</span> <span m="1985930">dangerous</span>
  <span m="1986590">and</span> <span m="1986710">expensive,</span> <span m="1987940">and</span>
  <span m="1988090">then</span> <span m="1988390">eight</span> <span m="1988630">different</span>
  <span m="1989020">treatments</span> <span m="1989710">that</span> <span m="1989860">could</span>
  <span m="1990100">be</span> <span m="1990280">applied.</span></p><p><span m="1991360">And</span>
  <span m="1991540">I'm</span> <span m="1991780">only</span> <span m="1991990">going</span>
  <span m="1992140">to</span> <span m="1992230">tell</span> <span m="1992500">you</span>
  <span m="1992680">about</span> <span m="1993040">the</span> <span m="1993160">first</span>
  <span m="1993550">part</span> <span m="1994390">of</span> <span m="1994600">this</span>
  <span m="1994810">problem.</span> <span m="1996730">This</span> <span m="1997070">1973</span>
  <span m="1998560">article</span> <span m="1999820">shows</span> <span m="2000240">you</span>
  <span m="2000360">what</span> <span m="2000570">the</span> <span m="2000690">program</span>
  <span m="2001170">looked</span> <span m="2001440">like.</span> <span m="2001750">It</span>
  <span m="2001830">was</span> <span m="2002150">a</span> <span m="2002460">computer</span>
  <span m="2002970">terminal</span> <span m="2003510">where</span> <span m="2004230">it</span>
  <span m="2004350">gave</span> <span m="2004650">you</span> <span m="2004770">choices,</span>
  <span m="2005430">and</span> <span m="2005580">you</span> <span m="2005720">would</span>
  <span m="2005850">type</span> <span m="2006240">in</span> <span m="2006360">an</span>
  <span m="2006510">answer.</span> <span m="2007980">And</span> <span m="2008160">so</span>
  <span m="2008850">that</span> <span m="2009240">was</span> <span m="2009480">the</span>
  <span m="2009600">state</span> <span m="2009930">of</span> <span m="2010050">the</span>
  <span m="2010200">art</span> <span m="2010590">at</span> <span m="2010740">the</span>
  <span m="2010830">time.</span></p><p><span m="2012330">But</span> <span m="2012630">what</span>
  <span m="2012840">I'm</span> <span m="2012960">going</span> <span m="2013080">to</span>
  <span m="2013170">do</span> <span m="2013410">is,</span> <span m="2014580">god</span>
  <span m="2014910">willing,</span> <span m="2015390">I'm</span> <span m="2015510">going</span>
  <span m="2015660">to</span> <span m="2015750">demonstrate</span> <span m="2017190">a</span>
  <span m="2017250">reconstruction</span> <span m="2019080">that</span> <span m="2019320">I</span>
  <span m="2019440">made</span> <span m="2019770">of</span> <span m="2019980">this</span>
  <span m="2020220">program.</span> <span m="2023440">So</span> <span m="2026280">these</span>
  <span m="2026670">guys</span> <span m="2027330">are</span> <span m="2027570">the</span>
  <span m="2028380">potential</span> <span m="2028950">causes</span> <span m="2029760">of</span>
  <span m="2030060">stopping</span> <span m="2030600">to</span> <span m="2030790">pee--</span>
  <span m="2031310">acute</span> <span m="2031600">tubular</span> <span m="2032050">necrosis,</span>
  <span m="2033390">functional</span> <span m="2033960">acute</span> <span m="2034290">renal</span>
  <span m="2034620">failure,</span> <span m="2035700">urinary</span> <span m="2036240">tract</span>
  <span m="2036630">obstruction,</span> <span m="2037870">acute</span> <span m="2038290">glomerulonephritis,</span>
  <span m="2039520">et</span> <span m="2039780">cetera.</span> <span m="2040920">And</span>
  <span m="2041340">these</span> <span m="2041790">are</span> <span m="2042060">the</span>
  <span m="2042180">prior</span> <span m="2042600">probabilities.</span></p><p><span
  m="2044150">Now,</span> <span m="2044250">I</span> <span m="2044350">have</span>
  <span m="2044450">to</span> <span m="2044460">warn</span> <span m="2044730">you,</span>
  <span m="2044850">these</span> <span m="2045120">numbers</span> <span m="2045720">were,</span>
  <span m="2046050">in</span> <span m="2046200">fact,</span> <span m="2046800">estimated</span>
  <span m="2047490">by</span> <span m="2047730">people</span> <span m="2048090">sticking</span>
  <span m="2048540">their</span> <span m="2048719">finger</span> <span m="2049110">in</span>
  <span m="2049230">the</span> <span m="2049380">air</span> <span m="2050130">and</span>
  <span m="2050310">figuring</span> <span m="2050820">out</span> <span m="2051120">which</span>
  <span m="2051360">way</span> <span m="2051540">the</span> <span m="2051659">wind</span>
  <span m="2051870">was</span> <span m="2052050">blowing,</span> <span m="2052949">because</span>
  <span m="2054420">in</span> <span m="2054510">1973,</span> <span m="2055710">there</span>
  <span m="2055880">were</span> <span m="2056070">not</span> <span m="2056340">great</span>
  <span m="2056610">databases</span> <span m="2057929">that</span> <span m="2058170">you</span>
  <span m="2058290">could</span> <span m="2058440">turn</span> <span m="2058770">to.</span></p><p><span
  m="2060360">And</span> <span m="2060540">then</span> <span m="2060989">these</span>
  <span m="2061409">are</span> <span m="2061560">the</span> <span m="2061710">questions</span>
  <span m="2062699">that</span> <span m="2063060">were</span> <span m="2063690">available</span>
  <span m="2064320">to</span> <span m="2064469">be</span> <span m="2064710">asked.</span>
  <span m="2065730">And</span> <span m="2065880">what</span> <span m="2066120">you</span>
  <span m="2066239">see</span> <span m="2066510">in</span> <span m="2066659">the</span>
  <span m="2066719">first</span> <span m="2067110">column,</span> <span m="2067620">at</span>
  <span m="2067739">least</span> <span m="2068070">if</span> <span m="2068190">you're</span>
  <span m="2068340">sitting</span> <span m="2068699">close</span> <span m="2069030">to</span>
  <span m="2069179">the</span> <span m="2069300">screen,</span> <span m="2071790">is</span>
  <span m="2072900">the</span> <span m="2073080">expected</span> <span m="2073739">entropy</span>
  <span m="2075000">of</span> <span m="2075270">the</span> <span m="2075420">probability</span>
  <span m="2076230">distribution</span> <span m="2077219">if</span> <span m="2077460">you</span>
  <span m="2077639">answered</span> <span m="2078120">this</span> <span m="2078389">question.</span>
  <span m="2081010">So</span> <span m="2081120">this</span> <span m="2081360">is</span>
  <span m="2081510">basically</span> <span m="2082080">saying,</span> <span m="2082500">if</span>
  <span m="2082679">I</span> <span m="2082830">ask</span> <span m="2083100">this</span>
  <span m="2083310">question,</span> <span m="2084550">how</span> <span m="2084659">likely</span>
  <span m="2085170">is</span> <span m="2085350">each</span> <span m="2085560">of</span>
  <span m="2085710">the</span> <span m="2085800">possible</span> <span m="2086400">answers,</span>
  <span m="2087239">given</span> <span m="2088290">my</span> <span m="2088530">disease</span>
  <span m="2088949">distribution</span> <span m="2089670">probabilities?</span></p><p><span
  m="2091290">And</span> <span m="2091440">then</span> <span m="2091679">for</span>
  <span m="2092010">each</span> <span m="2092280">of</span> <span m="2092400">those</span>
  <span m="2092670">answers,</span> <span m="2093340">I</span> <span m="2093370">do</span>
  <span m="2093600">a</span> <span m="2093659">Bayesian</span> <span m="2094170">revision,</span>
  <span m="2095520">then</span> <span m="2095730">I</span> <span m="2095850">weight</span>
  <span m="2096420">the</span> <span m="2096960">entropy</span> <span m="2097530">of</span>
  <span m="2097680">that</span> <span m="2099090">resulting</span> <span m="2099720">distribution</span>
  <span m="2100980">by</span> <span m="2101400">the</span> <span m="2101970">probability</span>
  <span m="2102720">of</span> <span m="2102840">getting</span> <span m="2103170">that</span>
  <span m="2103410">answer.</span> <span m="2104310">And</span> <span m="2104430">that</span>
  <span m="2104610">gets</span> <span m="2104910">me</span> <span m="2105060">the</span>
  <span m="2105210">expected</span> <span m="2105780">entropy</span> <span m="2106350">for</span>
  <span m="2106710">asking</span> <span m="2107130">that</span> <span m="2107340">question.</span>
  <span m="2108300">And</span> <span m="2108450">the</span> <span m="2108570">idea
  is</span> <span m="2109200">that</span> <span m="2109410">the</span> <span m="2109530">lower</span>
  <span m="2109920">the</span> <span m="2110100">expected</span> <span m="2110670">entropy,</span>
  <span m="2111150">the</span> <span m="2111270">more</span> <span m="2111510">valuable</span>
  <span m="2112020">the</span> <span m="2112140">question.</span> <span m="2114040">Makes</span>
  <span m="2114240">sense.</span></p><p><span m="2115420">So</span> <span m="2115800">if</span>
  <span m="2116010">we</span> <span m="2116160">look,</span> <span m="2116530">for</span>
  <span m="2116640">example,</span> <span m="2117460">the</span> <span m="2117750">most</span>
  <span m="2118080">valuable</span> <span m="2118620">question</span> <span m="2119640">is,</span>
  <span m="2120750">what</span> <span m="2121020">was</span> <span m="2121260">the</span>
  <span m="2121380">blood</span> <span m="2121650">pressure</span> <span m="2122190">at</span>
  <span m="2122370">the</span> <span m="2122520">onset</span> <span m="2123030">of</span>
  <span m="2123150">oliguria?</span> <span m="2125190">And</span> <span m="2126690">I</span>
  <span m="2126900">can</span> <span m="2127710">click</span> <span m="2128100">on</span>
  <span m="2128310">this</span> <span m="2129290">and</span> <span m="2129530">say</span>
  <span m="2131940">it</span> <span m="2132180">was,</span> <span m="2133710">let's</span>
  <span m="2134130">say,</span> <span m="2135630">moderately</span> <span m="2136320">elevated.</span></p><p><span
  m="2137900">And</span> <span m="2138090">what</span> <span m="2138360">this</span>
  <span m="2138600">little</span> <span m="2138900">colorful</span> <span m="2139470">graph</span>
  <span m="2139920">is</span> <span m="2140010">showing</span> <span m="2140490">you</span>
  <span m="2141450">is</span> <span m="2141750">that</span> <span m="2142710">if</span>
  <span m="2142950">you</span> <span m="2143100">look</span> <span m="2143370">at</span>
  <span m="2143520">the</span> <span m="2143790">initial</span> <span m="2144330">probability</span>
  <span m="2145110">distribution,</span> <span m="2146830">acute</span> <span m="2147170">tubular</span>
  <span m="2147630">necrosis</span> <span m="2148470">was</span> <span m="2148890">about</span>
  <span m="2149220">25%,</span> <span m="2151050">and</span> <span m="2151230">has</span>
  <span m="2151470">gone</span> <span m="2151770">down</span> <span m="2152070">to</span>
  <span m="2152280">a</span> <span m="2152370">very</span> <span m="2152610">small</span>
  <span m="2153270">amount,</span> <span m="2154260">whereas</span> <span m="2154650">some</span>
  <span m="2154980">of</span> <span m="2155130">these</span> <span m="2155400">others</span>
  <span m="2155850">have</span> <span m="2156030">grown</span> <span m="2156630">in</span>
  <span m="2156750">importance</span> <span m="2157440">considerably.</span></p><p><span
  m="2162950">So</span> <span m="2163190">we</span> <span m="2163340">can</span> <span
  m="2163520">answer</span> <span m="2163910">more</span> <span m="2164180">questions,</span>
  <span m="2164970">we</span> <span m="2165050">can</span> <span m="2165260">say--</span>
  <span m="2167150">let's</span> <span m="2167420">see.</span> <span m="2168620">What</span>
  <span m="2168830">is</span> <span m="2169040">the</span> <span m="2170030">degree--</span>
  <span m="2170840">is</span> <span m="2171230">there</span> <span m="2171590">proteinuria?</span>
  <span m="2172160">Is</span> <span m="2172340">there</span> <span m="2172490">protein</span>
  <span m="2172970">in</span> <span m="2173120">the</span> <span m="2173240">urine?</span>
  <span m="2174630">And</span> <span m="2174800">we</span> <span m="2174980">say,</span>
  <span m="2175580">no,</span> <span m="2175940">there</span> <span m="2176150">isn't.</span>
  <span m="2178206">I think</span> <span m="2178630">we</span> <span m="2178750">say,</span>
  <span m="2179000">no,</span> <span m="2179270">there</span> <span m="2179450">isn't.</span>
  <span m="2180320">0.</span></p><p><span m="2182600">And</span> <span m="2182750">that</span>
  <span m="2182960">revises</span> <span m="2183620">the</span> <span m="2183710">probability</span>
  <span m="2184310">distribution.</span> <span m="2185770">And</span> <span m="2186040">then</span>
  <span m="2186470">it</span> <span m="2186620">says</span> <span m="2186980">the</span>
  <span m="2187070">next</span> <span m="2187400">most</span> <span m="2187760">important</span>
  <span m="2188300">thing</span> <span m="2188690">is</span> <span m="2188870">kidney</span>
  <span m="2189290">size.</span> <span m="2190460">And</span> <span m="2190700">we</span>
  <span m="2190850">say--</span> <span m="2191210">let's</span> <span m="2191480">say</span>
  <span m="2191690">the</span> <span m="2191810">kidney</span> <span m="2192200">size</span>
  <span m="2192620">is</span> <span m="2192800">normal.</span> <span m="2194040">So</span>
  <span m="2194180">now</span> <span m="2194540">all</span> <span m="2194720">of</span>
  <span m="2194840">a</span> <span m="2194900">sudden</span> <span m="2195530">functional</span>
  <span m="2196130">acute</span> <span m="2196430">renal</span> <span m="2196760">failure,</span>
  <span m="2198060">which,</span> <span m="2198200">by</span> <span m="2198380">the</span>
  <span m="2198470">way,</span> <span m="2198720">is</span> <span m="2198770">one</span>
  <span m="2198980">of</span> <span m="2199040">these</span> <span m="2199280">funny</span>
  <span m="2199550">medical</span> <span m="2200000">care</span> <span m="2200390">categories</span>
  <span m="2201060">that</span> <span m="2201200">says</span> <span m="2201470">it</span>
  <span m="2201530">doesn't</span> <span m="2201860">work</span> <span m="2202160">well,</span>
  <span m="2203150">doesn't</span> <span m="2203450">explain</span> <span m="2203930">to</span>
  <span m="2204710">why</span> <span m="2205040">it</span> <span m="2205130">doesn't</span>
  <span m="2205490">work</span> <span m="2205790">well,</span> <span m="2206210">but</span>
  <span m="2206450">it's</span> <span m="2206720">sort</span> <span m="2206990">of</span>
  <span m="2207080">a</span> <span m="2207170">generic</span> <span m="2207680">thing.</span></p><p><span
  m="2209280">And</span> <span m="2209420">sure</span> <span m="2209750">enough.</span>
  <span m="2211080">We</span> <span m="2211160">can</span> <span m="2211370">keep</span>
  <span m="2211700">answering</span> <span m="2212210">questions</span> <span m="2212990">about,</span>
  <span m="2214460">are</span> <span m="2215150">you</span> <span m="2215330">producing</span>
  <span m="2216590">less</span> <span m="2216890">than</span> <span m="2217100">50</span>
  <span m="2217400">ccs</span> <span m="2218360">of</span> <span m="2218480">urine,</span>
  <span m="2219030">which</span> <span m="2219170">is</span> <span m="2219320">a</span>
  <span m="2219380">tiny</span> <span m="2219770">amount,</span> <span m="2220700">or</span>
  <span m="2220880">somewhere</span> <span m="2221330">between</span> <span m="2221780">50</span>
  <span m="2222200">and</span> <span m="2222350">400?</span> <span m="2224090">Remember,</span>
  <span m="2224570">this</span> <span m="2224810">is</span> <span m="2224960">for</span>
  <span m="2225110">people</span> <span m="2225500">who</span> <span m="2225650">are</span>
  <span m="2225710">not</span> <span m="2225980">producing</span> <span m="2226610">enough.</span>
  <span m="2227060">So</span> <span m="2227780">normally</span> <span m="2228260">you'd</span>
  <span m="2228470">be</span> <span m="2228650">over</span> <span m="2228980">400.</span>
  <span m="2230120">So</span> <span m="2230330">these</span> <span m="2230570">are</span>
  <span m="2230720">the</span> <span m="2230870">only</span> <span m="2231110">choices.</span></p><p><span
  m="2232190">So</span> <span m="2232220">let's</span> <span m="2232400">say</span>
  <span m="2232610">it's</span> <span m="2232790">moderate.</span> <span m="2233510">And</span>
  <span m="2233690">so</span> <span m="2233900">you</span> <span m="2234080">see</span>
  <span m="2234320">the</span> <span m="2234440">probability</span> <span m="2235040">distribution</span>
  <span m="2235760">keeps</span> <span m="2236120">changing.</span> <span m="2237500">And</span>
  <span m="2237830">what</span> <span m="2238070">happened</span> <span m="2238580">in</span>
  <span m="2238760">the</span> <span m="2238880">original</span> <span m="2239390">program</span>
  <span m="2240470">is</span> <span m="2240680">they</span> <span m="2240830">had</span>
  <span m="2241070">an</span> <span m="2241220">arbitrary</span> <span m="2241850">threshold</span>
  <span m="2242480">that</span> <span m="2242720">said</span> <span m="2243470">when</span>
  <span m="2243740">the</span> <span m="2243830">probability</span> <span m="2245120">of</span>
  <span m="2245420">one</span> <span m="2245750">of</span> <span m="2245900">these</span>
  <span m="2246470">causes</span> <span m="2247310">of</span> <span m="2247490">the</span>
  <span m="2247640">disease</span> <span m="2248240">reaches</span> <span m="2248690">95%,</span>
  <span m="2251450">then</span> <span m="2251690">we</span> <span m="2251840">switch</span>
  <span m="2252230">to</span> <span m="2252410">a</span> <span m="2252500">different</span>
  <span m="2252890">mode,</span> <span m="2253940">where</span> <span m="2254150">now</span>
  <span m="2254450">we're</span> <span m="2254690">actually</span> <span m="2255140">willing</span>
  <span m="2255500">to</span> <span m="2255620">contemplate</span> <span m="2256910">doing</span>
  <span m="2257330">the</span> <span m="2257660">expensive</span> <span m="2258320">tests</span>
  <span m="2259400">and</span> <span m="2259700">doing</span> <span m="2260150">the</span>
  <span m="2261500">expensive</span> <span m="2262070">treatments.</span> <span m="2263240">And</span>
  <span m="2263450">we</span> <span m="2263600">build</span> <span m="2263940">the</span>
  <span m="2264020">decision</span> <span m="2264560">tree,</span> <span m="2265070">as</span>
  <span m="2265310">we</span> <span m="2265490">saw</span> <span m="2265880">in</span>
  <span m="2266030">the</span> <span m="2266120">case</span> <span m="2266480">of</span>
  <span m="2266600">the</span> <span m="2266690">gangrenous</span> <span m="2267320">foot,</span>
  <span m="2268160">that</span> <span m="2268370">figures</span> <span m="2268820">out</span>
  <span m="2269060">which</span> <span m="2269300">of</span> <span m="2269450">those</span>
  <span m="2269780">is</span> <span m="2269960">the</span> <span m="2270080">optimal</span>
  <span m="2271070">approach.</span></p><p><span m="2272280">So</span> <span m="2272390">the</span>
  <span m="2272540">idea</span> <span m="2272960">here</span> <span m="2273290">was</span>
  <span m="2273590">because</span> <span m="2274580">building</span> <span m="2275000">a</span>
  <span m="2275090">decision</span> <span m="2275600">tree</span> <span m="2276470">with</span>
  <span m="2276770">27</span> <span m="2277520">potential</span> <span m="2278120">questions</span>
  <span m="2279200">becomes</span> <span m="2279680">enormously</span> <span m="2280370">bushy,</span>
  <span m="2282590">we're</span> <span m="2282830">using</span> <span m="2283430">a</span>
  <span m="2283490">heuristic</span> <span m="2284240">that</span> <span m="2284450">says</span>
  <span m="2284840">information</span> <span m="2285560">maximization</span> <span
  m="2287360">or</span> <span m="2288050">entropy</span> <span m="2288500">reduction</span>
  <span m="2289460">is</span> <span m="2289880">a</span> <span m="2289970">reasonable</span>
  <span m="2290600">way</span> <span m="2290900">of</span> <span m="2291020">focusing</span>
  <span m="2291770">in</span> <span m="2292640">on</span> <span m="2292940">what's</span>
  <span m="2293240">wrong</span> <span m="2293480">with</span> <span m="2293660">this</span>
  <span m="2293840">patient.</span> <span m="2294990">And</span> <span m="2295070">then</span>
  <span m="2295280">once</span> <span m="2295610">we</span> <span m="2295760">focused</span>
  <span m="2296390">in</span> <span m="2296540">pretty</span> <span m="2296840">well,</span>
  <span m="2297230">then</span> <span m="2297470">we</span> <span m="2297620">can</span>
  <span m="2297860">begin</span> <span m="2298250">to</span> <span m="2298400">do</span>
  <span m="2299120">more</span> <span m="2299330">detailed</span> <span m="2299840">analysis</span>
  <span m="2300620">on</span> <span m="2300950">the</span> <span m="2301640">remaining</span>
  <span m="2303020">more</span> <span m="2303290">consequential</span> <span m="2304280">and</span>
  <span m="2304400">more</span> <span m="2304610">costly</span> <span m="2305090">tests</span>
  <span m="2305930">that</span> <span m="2306110">are</span> <span m="2306230">available.</span></p><p><span
  m="2307940">Now,</span> <span m="2308150">this</span> <span m="2308390">program</span>
  <span m="2309860">didn't</span> <span m="2310190">work</span> <span m="2310490">terribly</span>
  <span m="2310970">well,</span> <span m="2311510">because</span> <span m="2313280">the</span>
  <span m="2313430">numbers</span> <span m="2313940">were</span> <span m="2314810">badly</span>
  <span m="2315320">estimated,</span> <span m="2316850">and</span> <span m="2317060">also</span>
  <span m="2317480">because</span> <span m="2318450">of</span> <span m="2322070">the</span>
  <span m="2322730">utility</span> <span m="2323480">model</span> <span m="2324140">that</span>
  <span m="2324410">they</span> <span m="2324590">had</span> <span m="2325040">for</span>
  <span m="2325400">the</span> <span m="2325550">decision</span> <span m="2326090">analytic</span>
  <span m="2326570">part</span> <span m="2327530">was</span> <span m="2327800">particularly</span>
  <span m="2328580">terrible.</span> <span m="2330820">It</span> <span m="2330980">didn't</span>
  <span m="2331610">really</span> <span m="2332000">reflect</span> <span m="2332720">anything</span>
  <span m="2333260">in</span> <span m="2333380">the</span> <span m="2333470">real</span>
  <span m="2333770">world.</span> <span m="2334640">They</span> <span m="2334880">had</span>
  <span m="2335120">an</span> <span m="2335240">incremental</span> <span m="2335810">utility</span>
  <span m="2336380">model</span> <span m="2336830">that</span> <span m="2337070">said</span>
  <span m="2337790">the</span> <span m="2337910">patient</span> <span m="2338420">either</span>
  <span m="2338750">got</span> <span m="2339020">better,</span> <span m="2339330">or</span>
  <span m="2339380">stayed</span> <span m="2339770">the</span> <span m="2339890">same,</span>
  <span m="2340250">or</span> <span m="2340370">got</span> <span m="2340640">worse.</span>
  <span m="2341900">And</span> <span m="2342530">obviously</span> <span m="2344270">in</span>
  <span m="2344450">that</span> <span m="2344690">order</span> <span m="2345080">of</span>
  <span m="2345200">utilities,</span> <span m="2346070">but</span> <span m="2346370">they</span>
  <span m="2346520">didn't</span> <span m="2346760">correspond</span> <span m="2347450">to</span>
  <span m="2347630">how</span> <span m="2347840">much</span> <span m="2348170">better</span>
  <span m="2348500">he</span> <span m="2348650">got</span> <span m="2349460">or</span>
  <span m="2349640">how</span> <span m="2349820">much</span> <span m="2350090">worse</span>
  <span m="2350450">he</span> <span m="2350540">got.</span> <span m="2350960">And</span>
  <span m="2351140">so</span> <span m="2351380">it</span> <span m="2351500">wasn't</span>
  <span m="2352460">terribly</span> <span m="2352910">useful.</span></p><p><span m="2354020">So</span>
  <span m="2354290">nevertheless,</span> <span m="2356480">in</span> <span m="2356660">the</span>
  <span m="2356910">1990s,</span> <span m="2357900">I</span> <span m="2357920">was</span>
  <span m="2358100">teaching</span> <span m="2358520">a</span> <span m="2358580">tutorial</span>
  <span m="2359450">at</span> <span m="2359630">a</span> <span m="2359690">Medical</span>
  <span m="2360110">Informatics</span> <span m="2360710">conference,</span> <span
  m="2361720">and</span> <span m="2361880">there</span> <span m="2361980">were</span>
  <span m="2362060">a</span> <span m="2362120">bunch</span> <span m="2362390">of</span>
  <span m="2362660">doctors</span> <span m="2363170">in</span> <span m="2363260">the</span>
  <span m="2363410">audience.</span> <span m="2363910">And</span> <span m="2364010">I</span>
  <span m="2364130">showed</span> <span m="2364430">them</span> <span m="2364610">this</span>
  <span m="2364820">program.</span></p><p><span m="2365840">And</span> <span m="2366020">one</span>
  <span m="2366200">of</span> <span m="2366320">the</span> <span m="2366410">doctors</span>
  <span m="2366950">came</span> <span m="2367250">up</span> <span m="2367460">afterwards</span>
  <span m="2368090">and</span> <span m="2368210">said,</span> <span m="2368480">wow,</span>
  <span m="2368870">it</span> <span m="2369020">thinks</span> <span m="2369410">just</span>
  <span m="2369710">the</span> <span m="2369800">way</span> <span m="2370040">I</span>
  <span m="2370220">do.</span> <span m="2373220">And</span> <span m="2373320">I</span>
  <span m="2373400">said,</span> <span m="2374330">really?</span> <span m="2377990">I</span>
  <span m="2378080">don't</span> <span m="2378290">think</span> <span m="2378530">so.</span>
  <span m="2379760">But</span> <span m="2380060">clearly,</span> <span m="2382430">it</span>
  <span m="2382550">was</span> <span m="2382760">doing</span> <span m="2383060">something</span>
  <span m="2383630">that</span> <span m="2383870">corresponded</span> <span m="2384920">to</span>
  <span m="2385040">the</span> <span m="2385160">way</span> <span m="2385400">that</span>
  <span m="2385610">he</span> <span m="2385760">thought</span> <span m="2386300">about</span>
  <span m="2387110">these</span> <span m="2387380">cases.</span> <span m="2388550">So</span>
  <span m="2388790">I</span> <span m="2389390">thought</span> <span m="2389630">that</span>
  <span m="2389790">was</span> <span m="2390410">a</span> <span m="2390470">good</span>
  <span m="2390650">thing.</span></p><p><span m="2391730">All</span> <span m="2391790">right.</span>
  <span m="2392360">Well,</span> <span m="2392600">what</span> <span m="2392810">happens</span>
  <span m="2393500">if</span> <span m="2393680">we</span> <span m="2393830">can't</span>
  <span m="2394250">assume</span> <span m="2395300">that</span> <span m="2395540">there's</span>
  <span m="2395840">just</span> <span m="2396110">a</span> <span m="2396140">single</span>
  <span m="2396560">disease</span> <span m="2397100">underlying</span> <span m="2397670">the</span>
  <span m="2397760">person's</span> <span m="2398210">problems?</span> <span m="2400220">If</span>
  <span m="2400400">there</span> <span m="2400520">are</span> <span m="2400580">multiple</span>
  <span m="2401090">diseases,</span> <span m="2403550">we</span> <span m="2403730">can</span>
  <span m="2404000">build</span> <span m="2404420">this</span> <span m="2404720">kind</span>
  <span m="2404990">of</span> <span m="2405110">bipartite</span> <span m="2405890">model</span>
  <span m="2406760">that</span> <span m="2407000">says</span> <span m="2407300">we</span>
  <span m="2407450">have</span> <span m="2407600">a</span> <span m="2407630">list</span>
  <span m="2407930">of</span> <span m="2408020">diseases</span> <span m="2408810">and</span>
  <span m="2408860">we</span> <span m="2408980">have</span> <span m="2409100">a</span>
  <span m="2409130">list</span> <span m="2409400">of</span> <span m="2409490">manifestations.</span>
  <span m="2410630">And</span> <span m="2410900">some</span> <span m="2411320">subset</span>
  <span m="2411890">of</span> <span m="2412010">the</span> <span m="2412160">diseases</span>
  <span m="2413360">can</span> <span m="2413570">cause</span> <span m="2414080">some</span>
  <span m="2414380">subset</span> <span m="2414890">of</span> <span m="2415550">the</span>
  <span m="2415640">symptoms,</span> <span m="2416240">of</span> <span m="2416390">the</span>
  <span m="2416480">manifestations.</span></p><p><span m="2418790">And</span> <span
  m="2418970">so</span> <span m="2419210">the</span> <span m="2419330">manifestations</span>
  <span m="2420410">depend</span> <span m="2420920">only</span> <span m="2421250">on</span>
  <span m="2421370">the</span> <span m="2421490">diseases</span> <span m="2422150">that</span>
  <span m="2422330">are</span> <span m="2422450">present,</span> <span m="2422990">not</span>
  <span m="2423230">on</span> <span m="2423380">each</span> <span m="2423620">other.</span>
  <span m="2424550">And</span> <span m="2424730">therefore,</span> <span m="2425150">we</span>
  <span m="2425300">have</span> <span m="2425480">conditional</span> <span m="2426050">independence.</span>
  <span m="2427440">And</span> <span m="2427490">this</span> <span m="2427700">is</span>
  <span m="2427860">a</span> <span m="2427940">type</span> <span m="2428270">of</span>
  <span m="2428390">Bayesian</span> <span m="2428910">network,</span> <span m="2430010">which</span>
  <span m="2430460">can't</span> <span m="2430850">be</span> <span m="2431000">solved</span>
  <span m="2433940">exactly</span> <span m="2434660">because</span> <span m="2435140">of</span>
  <span m="2435290">the</span> <span m="2435410">computational</span> <span m="2436190">complexity.</span>
  <span m="2437390">So</span> <span m="2437640">a</span> <span m="2437690">program</span>
  <span m="2438140">I'll</span> <span m="2438290">show</span> <span m="2438530">you</span>
  <span m="2438710">in</span> <span m="2438830">a</span> <span m="2438860">minute</span>
  <span m="2439640">had</span> <span m="2440750">400</span> <span m="2441110">or</span>
  <span m="2441170">500</span> <span m="2442370">diseases</span> <span m="2443240">and</span>
  <span m="2443510">thousands</span> <span m="2444200">of</span> <span m="2444650">manifestations.</span>
  <span m="2446360">And</span> <span m="2446670">the</span> <span m="2446780">computational</span>
  <span m="2447590">complexity</span> <span m="2447980">of</span> <span m="2448370">exact</span>
  <span m="2448940">solution</span> <span m="2449480">techniques</span> <span m="2450080">for</span>
  <span m="2450260">these</span> <span m="2450500">networks</span> <span m="2451580">tends</span>
  <span m="2451910">to</span> <span m="2452030">go</span> <span m="2452420">exponentially</span>
  <span m="2453260">with</span> <span m="2453470">the</span> <span m="2453590">number</span>
  <span m="2453950">of</span> <span m="2454070">undirected</span> <span m="2454730">cycles</span>
  <span m="2455780">in</span> <span m="2455930">the</span> <span m="2456020">network.</span>
  <span m="2456590">And</span> <span m="2456740">of</span> <span m="2456830">course,</span>
  <span m="2457130">there</span> <span m="2457280">are</span> <span m="2457340">plenty</span>
  <span m="2457700">of</span> <span m="2457850">undirected</span> <span m="2458480">cycles</span>
  <span m="2459530">in</span> <span m="2459680">a</span> <span m="2459740">network</span>
  <span m="2460190">like</span> <span m="2460430">that.</span></p><p><span m="2462960">So</span>
  <span m="2463880">there</span> <span m="2464150">was</span> <span m="2464330">a</span>
  <span m="2464390">program</span> <span m="2465350">developed</span> <span m="2466730">originally</span>
  <span m="2467390">in</span> <span m="2467510">the</span> <span m="2468890">early</span>
  <span m="2469160">1970s</span> <span m="2470810">called</span> <span m="2471080">Dialog.</span>
  <span m="2472490">And</span> <span m="2472640">then</span> <span m="2472880">they</span>
  <span m="2473030">got</span> <span m="2473270">sued,</span> <span m="2473800">because</span>
  <span m="2473960">somebody</span> <span m="2474440">owned</span> <span m="2474650">that</span>
  <span m="2474920">name.</span> <span m="2475590">And</span> <span m="2475640">then</span>
  <span m="2475790">they</span> <span m="2475940">called</span> <span m="2476300">it</span>
  <span m="2476420">Internist,</span> <span m="2477170">and</span> <span m="2477590">they</span>
  <span m="2477800">got</span> <span m="2478040">sued</span> <span m="2478400">because</span>
  <span m="2479450">somebody</span> <span m="2480000">owned</span> <span m="2480230">that</span>
  <span m="2480530">name.</span> <span m="2481530">And</span> <span m="2481580">then</span>
  <span m="2481790">they</span> <span m="2481940">called</span> <span m="2482230">it</span>
  <span m="2482330">QMR,</span> <span m="2483410">which</span> <span m="2483800">stands</span>
  <span m="2484280">for</span> <span m="2484460">Quick</span> <span m="2484760">Medical</span>
  <span m="2485210">Reference,</span> <span m="2485750">and</span> <span m="2485860">nobody</span>
  <span m="2486320">owned</span> <span m="2486500">that</span> <span m="2486770">name.</span></p><p><span
  m="2488150">So</span> <span m="2488450">around</span> <span m="2489060">1982,</span>
  <span m="2490400">this</span> <span m="2490610">program</span> <span m="2491690">had</span>
  <span m="2491930">about</span> <span m="2492200">500</span> <span m="2492770">diseases,</span>
  <span m="2493430">which</span> <span m="2493670">they</span> <span m="2493880">estimated</span>
  <span m="2495020">represented</span> <span m="2495740">about</span> <span m="2496010">70%</span>
  <span m="2496520">to</span> <span m="2496700">75%</span> <span m="2497840">of</span>
  <span m="2497960">major</span> <span m="2498290">diagnoses</span> <span m="2499040">in</span>
  <span m="2499160">internal</span> <span m="2499610">medicine,</span> <span m="2500690">about</span>
  <span m="2501020">3,500</span> <span m="2501950">manifestations.</span> <span m="2503060">And</span>
  <span m="2503180">it</span> <span m="2503270">took</span> <span m="2503570">about</span>
  <span m="2503840">15</span> <span m="2504350">man</span> <span m="2504650">years</span>
  <span m="2505610">of</span> <span m="2506390">manual</span> <span m="2507020">effort</span>
  <span m="2507950">to</span> <span m="2508130">sit</span> <span m="2508430">there</span>
  <span m="2508730">and</span> <span m="2508880">read</span> <span m="2509150">medical</span>
  <span m="2509570">textbooks</span> <span m="2510290">and</span> <span m="2510410">journal</span>
  <span m="2510800">articles</span> <span m="2511850">and</span> <span m="2512600">look</span>
  <span m="2512870">at</span> <span m="2513290">records</span> <span m="2513830">of</span>
  <span m="2514010">patients</span> <span m="2514670">in</span> <span m="2514790">their</span>
  <span m="2514940">hospital.</span></p><p><span m="2516440">The</span> <span m="2516710">effort</span>
  <span m="2517160">was</span> <span m="2517370">led</span> <span m="2517700">by</span>
  <span m="2517970">a</span> <span m="2518030">computer</span> <span m="2518480">scientist</span>
  <span m="2520370">at</span> <span m="2520660">the</span> <span m="2520700">University</span>
  <span m="2521240">of</span> <span m="2521330">Pittsburgh</span> <span m="2522410">and</span>
  <span m="2522740">the</span> <span m="2523070">chief</span> <span m="2523430">of</span>
  <span m="2523520">medicine</span> <span m="2524270">at</span> <span m="2525140">UPMC,</span>
  <span m="2525950">the</span> <span m="2526100">University</span> <span m="2526580">of</span>
  <span m="2526670">Pittsburgh</span> <span m="2527090">Medical</span> <span m="2527480">Center,</span>
  <span m="2528800">who</span> <span m="2529010">was</span> <span m="2529370">just</span>
  <span m="2529700">a</span> <span m="2529760">fanatic.</span> <span m="2530480">And</span>
  <span m="2530960">he</span> <span m="2531110">got</span> <span m="2531380">all</span>
  <span m="2531560">the</span> <span m="2532400">medical</span> <span m="2532790">school</span>
  <span m="2533150">trainees</span> <span m="2534260">to</span> <span m="2534410">spend</span>
  <span m="2534920">hours</span> <span m="2535340">and</span> <span m="2535460">hours</span>
  <span m="2536480">coming</span> <span m="2536900">up</span> <span m="2537080">with</span>
  <span m="2537290">these</span> <span m="2537890">databases.</span></p><p><span m="2539480">By</span>
  <span m="2539710">1997,</span> <span m="2541010">they</span> <span m="2541250">had</span>
  <span m="2541430">commercialized</span> <span m="2542390">it</span> <span m="2543350">through</span>
  <span m="2543620">a</span> <span m="2543710">company</span> <span m="2544940">that</span>
  <span m="2545150">had</span> <span m="2545330">bought</span> <span m="2545630">the</span>
  <span m="2545750">rights</span> <span m="2546110">to</span> <span m="2546320">it.</span>
  <span m="2547170">And</span> <span m="2547430">they</span> <span m="2547670">had--</span>
  <span m="2547940">that</span> <span m="2548240">company</span> <span m="2548720">had</span>
  <span m="2548900">expanded</span> <span m="2549530">it</span> <span m="2549620">to</span>
  <span m="2550460">about</span> <span m="2550860">750</span> <span m="2551990">diagnoses</span>
  <span m="2552980">and</span> <span m="2553100">about</span> <span m="2553370">5,500</span>
  <span m="2554330">manifestations.</span> <span m="2555870">So</span> <span m="2555950">they</span>
  <span m="2556100">made</span> <span m="2556340">it</span> <span m="2556430">considerably</span>
  <span m="2557180">larger.</span> <span m="2558740">Details</span> <span m="2559470">are--</span>
  <span m="2560510">I've</span> <span m="2560720">tried</span> <span m="2560990">to</span>
  <span m="2561140">put</span> <span m="2561350">references</span> <span m="2562010">on</span>
  <span m="2562160">all</span> <span m="2562280">the</span> <span m="2562400">slides.</span></p><p><span
  m="2563820">So</span> <span m="2563960">here's</span> <span m="2564230">what</span>
  <span m="2564380">data</span> <span m="2564970">in</span> <span m="2565510">QMR</span>
  <span m="2566030">looks</span> <span m="2566330">like.</span> <span m="2567590">For</span>
  <span m="2568040">each</span> <span m="2568310">diagnosis,</span> <span m="2569650">there</span>
  <span m="2569890">is</span> <span m="2570050">a</span> <span m="2570080">list</span>
  <span m="2570440">of</span> <span m="2570590">associated</span> <span m="2571340">manifestations</span>
  <span m="2572960">with</span> <span m="2573470">evoking</span> <span m="2574040">strengths</span>
  <span m="2574700">and</span> <span m="2574880">frequencies.</span> <span m="2576030">So</span>
  <span m="2576140">I'll</span> <span m="2576410">explain</span> <span m="2576890">that</span>
  <span m="2577130">in</span> <span m="2577250">a</span> <span m="2577310">minute.</span></p><p><span
  m="2578900">On</span> <span m="2579080">average,</span> <span m="2579620">there</span>
  <span m="2579830">are</span> <span m="2579890">about</span> <span m="2580190">75</span>
  <span m="2580910">manifestations</span> <span m="2581990">per</span> <span m="2582260">disease.</span>
  <span m="2584270">And</span> <span m="2584720">for</span> <span m="2585050">each</span>
  <span m="2585380">disease--</span> <span m="2585950">for</span> <span m="2586160">each</span>
  <span m="2586400">manifestation</span> <span m="2587900">in</span> <span m="2588050">addition</span>
  <span m="2588470">to</span> <span m="2588620">the</span> <span m="2588770">data</span>
  <span m="2589130">you</span> <span m="2589280">see</span> <span m="2589520">here,</span>
  <span m="2590190">there</span> <span m="2590410">is</span> <span m="2590570">also</span>
  <span m="2590930">an</span> <span m="2591050">important</span> <span m="2591680">measure</span>
  <span m="2592610">that</span> <span m="2592850">says</span> <span m="2593210">how</span>
  <span m="2593420">critical</span> <span m="2593930">is</span> <span m="2594110">it</span>
  <span m="2594230">to</span> <span m="2594410">explain</span> <span m="2595580">this</span>
  <span m="2595970">particular</span> <span m="2596690">symptom</span> <span m="2597220">or</span>
  <span m="2597380">sign</span> <span m="2597860">or</span> <span m="2598010">lab</span>
  <span m="2598280">value</span> <span m="2599450">in</span> <span m="2599660">the</span>
  <span m="2599750">final</span> <span m="2600140">diagnosis.</span></p><p><span m="2601280">So</span>
  <span m="2601520">for</span> <span m="2601700">example,</span> <span m="2602570">if</span>
  <span m="2602780">you</span> <span m="2602900">have</span> <span m="2603110">a</span>
  <span m="2603170">headache,</span> <span m="2604190">that</span> <span m="2604430">could</span>
  <span m="2604640">be</span> <span m="2604820">incidental</span> <span m="2605480">and</span>
  <span m="2605600">it's</span> <span m="2605780">not</span> <span m="2605990">that</span>
  <span m="2606170">important</span> <span m="2606650">to</span> <span m="2606860">explain</span>
  <span m="2607340">it.</span> <span m="2608330">If</span> <span m="2608570">you're</span>
  <span m="2608870">bleeding</span> <span m="2609560">from</span> <span m="2609950">your</span>
  <span m="2611360">gastrointestinal</span> <span m="2612440">system,</span> <span
  m="2613760">that's</span> <span m="2614060">really</span> <span m="2614360">important</span>
  <span m="2615050">to</span> <span m="2615290">explain.</span> <span m="2616280">And</span>
  <span m="2616430">you</span> <span m="2616580">wouldn't</span> <span m="2616880">expect</span>
  <span m="2617840">a</span> <span m="2617900">diagnosis</span> <span m="2618710">of</span>
  <span m="2618830">that</span> <span m="2619040">patient</span> <span m="2619610">that</span>
  <span m="2619790">doesn't</span> <span m="2620390">explain</span> <span m="2620840">to</span>
  <span m="2620960">you</span> <span m="2621110">why</span> <span m="2621440">they</span>
  <span m="2621590">have</span> <span m="2621830">that</span> <span m="2622040">symptom.</span></p><p><span
  m="2623180">And</span> <span m="2623330">then</span> <span m="2623540">here</span>
  <span m="2623850">is</span> <span m="2623930">an</span> <span m="2624050">example</span>
  <span m="2624830">of</span> <span m="2626900">alcoholic</span> <span m="2627590">hepatitis.</span>
  <span m="2629030">And</span> <span m="2629480">the</span> <span m="2629660">two</span>
  <span m="2629930">numbers</span> <span m="2630530">here</span> <span m="2631430">are</span>
  <span m="2631880">a</span> <span m="2632060">so-called</span> <span m="2632660">evoking</span>
  <span m="2633200">strength</span> <span m="2633800">and</span> <span m="2633950">a</span>
  <span m="2634010">frequency.</span> <span m="2635210">These</span> <span m="2635480">are</span>
  <span m="2635570">both</span> <span m="2635960">on</span> <span m="2636140">scales--</span>
  <span m="2637010">well,</span> <span m="2637310">evoking</span> <span m="2637790">strength</span>
  <span m="2638220">is</span> <span m="2638390">on</span> <span m="2638540">a</span>
  <span m="2638600">scale</span> <span m="2639530">of</span> <span m="2639650">0</span>
  <span m="2640010">to</span> <span m="2640100">5,</span> <span m="2641090">and</span>
  <span m="2641270">frequency</span> <span m="2641960">is</span> <span m="2642140">on</span>
  <span m="2642290">a</span> <span m="2642350">scale</span> <span m="2642740">of</span>
  <span m="2642860">1</span> <span m="2643100">to</span> <span m="2643220">5.</span>
  <span m="2644552">And</span> <span m="2644980">I'll</span> <span m="2645110">show</span>
  <span m="2645350">you</span> <span m="2645470">what</span> <span m="2645680">those</span>
  <span m="2646220">are</span> <span m="2646340">supposed</span> <span m="2646790">to</span>
  <span m="2646910">mean.</span></p><p><span m="2647840">And</span> <span m="2647990">so,</span>
  <span m="2648230">for</span> <span m="2648470">example,</span> <span m="2648950">what</span>
  <span m="2649190">this</span> <span m="2649340">says</span> <span m="2650330">is</span>
  <span m="2650570">that</span> <span m="2650780">if</span> <span m="2650900">you're</span>
  <span m="2651140">anorexic,</span> <span m="2653090">that</span> <span m="2653900">should</span>
  <span m="2654260">not</span> <span m="2654680">make</span> <span m="2655010">you</span>
  <span m="2655190">think</span> <span m="2655670">about</span> <span m="2656210">alcoholic</span>
  <span m="2656900">hepatitis</span> <span m="2658550">as</span> <span m="2659140">a</span>
  <span m="2659250">disease.</span> <span m="2660480">But</span> <span m="2661730">you</span>
  <span m="2661910">should</span> <span m="2662150">expect</span> <span m="2662750">that</span>
  <span m="2662900">if</span> <span m="2663050">somebody</span> <span m="2663530">has</span>
  <span m="2663890">alcoholic</span> <span m="2664550">hepatitis,</span> <span m="2665720">they're</span>
  <span m="2665900">very</span> <span m="2666170">likely</span> <span m="2666620">to</span>
  <span m="2666770">have</span> <span m="2667370">anorexia.</span> <span m="2668880">So</span>
  <span m="2668960">that's</span> <span m="2669260">the</span> <span m="2669380">frequency</span>
  <span m="2669980">number.</span> <span m="2670790">This</span> <span m="2671000">is</span>
  <span m="2671180">the</span> <span m="2671330">evoking</span> <span m="2671780">strength</span>
  <span m="2672200">number.</span> <span m="2672980">And</span> <span m="2673130">you</span>
  <span m="2673250">see</span> <span m="2673520">that</span> <span m="2673730">there</span>
  <span m="2673820">is</span> <span m="2674000">a</span> <span m="2674060">variety</span>
  <span m="2674750">of</span> <span m="2674930">those.</span></p><p><span m="2675890">So</span>
  <span m="2676340">much</span> <span m="2676880">of</span> <span m="2677390">that</span>
  <span m="2678380">many,</span> <span m="2678900">many</span> <span m="2679100">years</span>
  <span m="2679430">of</span> <span m="2679550">effort</span> <span m="2680360">went</span>
  <span m="2680630">into</span> <span m="2680870">coming</span> <span m="2681290">up</span>
  <span m="2681440">with</span> <span m="2681680">these</span> <span m="2681920">lists</span>
  <span m="2682550">and</span> <span m="2682790">coming</span> <span m="2683180">up</span>
  <span m="2683360">with</span> <span m="2683540">those</span> <span m="2683810">numbers.</span>
  <span m="2685130">Here</span> <span m="2685460">are</span> <span m="2685640">the</span>
  <span m="2685760">scales.</span> <span m="2686540">So</span> <span m="2686810">the</span>
  <span m="2687140">evoking</span> <span m="2687650">strength--</span> <span m="2689440">0</span>
  <span m="2689870">means</span> <span m="2690270">nonspecific.</span> <span m="2691460">5</span>
  <span m="2691910">means</span> <span m="2692240">its</span> <span m="2692420">pathognomonic.</span>
  <span m="2693380">In</span> <span m="2693500">other</span> <span m="2693680">words,</span>
  <span m="2694410">just</span> <span m="2694640">seeing</span> <span m="2695060">the</span>
  <span m="2695220">symptom</span> <span m="2695810">is</span> <span m="2695990">enough</span>
  <span m="2696320">to</span> <span m="2696470">convince</span> <span m="2697040">you</span>
  <span m="2697670">that</span> <span m="2697880">the</span> <span m="2698000">patient</span>
  <span m="2698450">must</span> <span m="2698750">have</span> <span m="2698960">this</span>
  <span m="2699170">disease.</span></p><p><span m="2700890">Similarly,</span> <span
  m="2701960">frequency</span> <span m="2703520">1</span> <span m="2704030">means</span>
  <span m="2704390">it</span> <span m="2704550">occurs</span> <span m="2704990">rarely,</span>
  <span m="2705680">and</span> <span m="2705950">5</span> <span m="2706370">means</span>
  <span m="2706760">that</span> <span m="2706940">it</span> <span m="2707090">occurs</span>
  <span m="2707530">in</span> <span m="2707630">essentially</span> <span m="2708230">all</span>
  <span m="2708380">cases</span> <span m="2709490">with</span> <span m="2709700">scaled</span>
  <span m="2710540">values</span> <span m="2711140">in</span> <span m="2711260">between.</span>
  <span m="2712460">And</span> <span m="2712640">these</span> <span m="2712940">are</span>
  <span m="2713090">kind</span> <span m="2713540">of</span> <span m="2713690">like</span>
  <span m="2714050">odds</span> <span m="2714350">ratios.</span> <span m="2715400">And</span>
  <span m="2715610">they</span> <span m="2715850">add</span> <span m="2716150">them</span>
  <span m="2716390">kind</span> <span m="2716750">of</span> <span m="2716930">as</span>
  <span m="2717200">if</span> <span m="2717410">they</span> <span m="2717590">were</span>
  <span m="2717800">log</span> <span m="2719120">likelihood</span> <span m="2719750">ratios.</span>
  <span m="2720470">And</span> <span m="2720650">so</span> <span m="2721790">there's</span>
  <span m="2722120">been</span> <span m="2722300">a</span> <span m="2722420">big</span>
  <span m="2722660">literature</span> <span m="2723290">on</span> <span m="2723470">trying</span>
  <span m="2723770">to</span> <span m="2723920">figure</span> <span m="2724280">out</span>
  <span m="2724880">exactly</span> <span m="2725480">what</span> <span m="2725690">these</span>
  <span m="2725930">numbers</span> <span m="2726410">mean,</span> <span m="2727310">because</span>
  <span m="2727730">there's</span> <span m="2727970">no</span> <span m="2728180">formal</span>
  <span m="2728660">definition</span> <span m="2729410">in</span> <span m="2729560">terms</span>
  <span m="2729980">of</span> <span m="2730220">you</span> <span m="2730640">count</span>
  <span m="2731150">the</span> <span m="2731300">number</span> <span m="2731690">of</span>
  <span m="2731840">this</span> <span m="2732200">and</span> <span m="2732350">divide</span>
  <span m="2732800">by</span> <span m="2733010">the</span> <span m="2733160">number</span>
  <span m="2733520">of</span> <span m="2733640">that,</span> <span m="2734060">and</span>
  <span m="2734180">that</span> <span m="2734390">gives</span> <span m="2734690">you</span>
  <span m="2734810">the</span> <span m="2735290">right</span> <span m="2735530">answer.</span>
  <span m="2736530">These</span> <span m="2736670">were</span> <span m="2737480">sort</span>
  <span m="2737750">of the</span> <span m="2737900">impressionistic</span> <span m="2739280">kinds</span>
  <span m="2739730">of</span> <span m="2740090">numbers.</span></p><p><span m="2742860">So</span>
  <span m="2742970">the</span> <span m="2743120">logic</span> <span m="2743780">in</span>
  <span m="2743930">the</span> <span m="2744050">system</span> <span m="2745010">was</span>
  <span m="2745460">that</span> <span m="2748760">you</span> <span m="2749030">would</span>
  <span m="2749540">come</span> <span m="2749840">to</span> <span m="2750170">it</span>
  <span m="2750560">and</span> <span m="2750860">give</span> <span m="2751160">it</span>
  <span m="2751310">a</span> <span m="2751400">list</span> <span m="2751850">of</span>
  <span m="2752000">the</span> <span m="2752120">manifestations</span> <span m="2753200">of</span>
  <span m="2753350">a</span> <span m="2753410">case.</span> <span m="2754820">And</span>
  <span m="2755630">to</span> <span m="2755900">their</span> <span m="2756140">credit,</span>
  <span m="2756710">they</span> <span m="2756890">went</span> <span m="2757250">after</span>
  <span m="2757580">very</span> <span m="2757880">complicated</span> <span m="2758600">cases.</span>
  <span m="2759090">So</span> <span m="2759290">they</span> <span m="2759470">took</span>
  <span m="2759860">clinical</span> <span m="2760310">pathologic</span> <span m="2761160">conference</span>
  <span m="2761730">cases</span> <span m="2762750">from</span> <span m="2763050"><i>The</i></span>
  <span m="2763140"><i>New</i></span> <span m="2763320"><i>England</i></span> <span
  m="2763560"><i>Journal</i></span> <span m="2763890"><i>of</i></span> <span m="2763980"><i>Medicine.</i></span>
  <span m="2765030">These</span> <span m="2765300">are</span> <span m="2765420">cases</span>
  <span m="2765930">selected</span> <span m="2766620">to</span> <span m="2766830">be</span>
  <span m="2766980">difficult</span> <span m="2767610">enough</span> <span m="2768360">that</span>
  <span m="2768570">doctors</span> <span m="2769140">are</span> <span m="2769290">willing</span>
  <span m="2769620">to</span> <span m="2769770">read</span> <span m="2770070">these.</span>
  <span m="2771000">And</span> <span m="2771270">they're</span> <span m="2771480">typically</span>
  <span m="2772080">presented</span> <span m="2772860">at</span> <span m="2773010">Grand</span>
  <span m="2773370">Rounds</span> <span m="2773840">at</span> <span m="2773980">MGH</span>
  <span m="2775200">by</span> <span m="2775530">somebody</span> <span m="2776250">who</span>
  <span m="2776430">is</span> <span m="2776610">often</span> <span m="2776970">stumped</span>
  <span m="2777540">by</span> <span m="2777720">the</span> <span m="2777840">case.</span>
  <span m="2778470">So</span> <span m="2778710">it's</span> <span m="2779130">an</span>
  <span m="2779250">opportunity</span> <span m="2779970">to</span> <span m="2780120">watch</span>
  <span m="2780870">people</span> <span m="2781230">reason</span> <span m="2781590">interactively</span>
  <span m="2782430">about</span> <span m="2782760">these</span> <span m="2783000">things.</span></p><p><span
  m="2785050">And</span> <span m="2785130">so</span> <span m="2786990">you</span>
  <span m="2787230">evoke</span> <span m="2787590">the</span> <span m="2787740">diagnoses</span>
  <span m="2788640">that</span> <span m="2788820">have</span> <span m="2789030">a</span>
  <span m="2789090">high</span> <span m="2789390">evoking</span> <span m="2789870">strength</span>
  <span m="2790350">from</span> <span m="2790620">the</span> <span m="2790710">giving</span>
  <span m="2791250">manifestations.</span> <span m="2792870">And</span> <span m="2793050">then</span>
  <span m="2793230">you</span> <span m="2793410">do</span> <span m="2793650">a</span>
  <span m="2793740">scoring</span> <span m="2794430">calculation</span> <span m="2795390">based</span>
  <span m="2795780">on</span> <span m="2795930">those</span> <span m="2796140">numbers.</span>
  <span m="2797340">The</span> <span m="2797490">details</span> <span m="2798060">of</span>
  <span m="2798180">this</span> <span m="2798480">are</span> <span m="2798600">probably</span>
  <span m="2799170">all</span> <span m="2799440">wrong,</span> <span m="2799920">but</span>
  <span m="2800430">that's</span> <span m="2800970">the</span> <span m="2801030">way</span>
  <span m="2801210">they</span> <span m="2801390">went</span> <span m="2801600">about</span>
  <span m="2801930">it.</span> <span m="2802950">And</span> <span m="2803100">then</span>
  <span m="2803280">you</span> <span m="2803400">form</span> <span m="2803790">a</span>
  <span m="2803850">differential</span> <span m="2804810">around</span> <span m="2805290">the</span>
  <span m="2805380">highest</span> <span m="2805770">scoring</span> <span m="2806250">diagnosis.</span></p><p><span
  m="2807660">Now,</span> <span m="2807840">this</span> <span m="2808080">is</span>
  <span m="2808230">actually</span> <span m="2808740">an</span> <span m="2808860">interesting</span>
  <span m="2809400">idea.</span> <span m="2810460">It's</span> <span m="2810570">a</span>
  <span m="2810630">heuristic</span> <span m="2811230">idea,</span> <span m="2812230">but</span>
  <span m="2812310">it's</span> <span m="2812460">one</span> <span m="2812670">that</span>
  <span m="2812850">worked</span> <span m="2813180">pretty</span> <span m="2813480">well.</span>
  <span m="2814600">So</span> <span m="2814740">suppose</span> <span m="2815310">I</span>
  <span m="2815430">have</span> <span m="2815670">two</span> <span m="2815910">diseases.</span>
  <span m="2817210">D1</span> <span m="2817920">can</span> <span m="2818160">cause</span>
  <span m="2818790">manifestations</span> <span m="2819840">1</span> <span m="2820080">through</span>
  <span m="2820320">4.</span> <span m="2821250">And</span> <span m="2821460">D2</span>
  <span m="2821940">can</span> <span m="2822180">cause</span> <span m="2822570">3</span>
  <span m="2822840">through</span> <span m="2823110">6.</span></p><p><span m="2825990">So</span>
  <span m="2827010">are</span> <span m="2827250">these</span> <span m="2827760">competing</span>
  <span m="2828690">to</span> <span m="2828930">explain</span> <span m="2829920">the</span>
  <span m="2830070">same</span> <span m="2830430">case</span> <span m="2831630">or</span>
  <span m="2831840">could</span> <span m="2832110">they</span> <span m="2832320">be</span>
  <span m="2832470">complementary?</span> <span m="2834870">Well,</span> <span m="2835170">until</span>
  <span m="2835530">we</span> <span m="2835680">know</span> <span m="2835920">what</span>
  <span m="2836160">symptoms</span> <span m="2836700">the</span> <span m="2836790">patient</span>
  <span m="2837270">actually</span> <span m="2837690">has,</span> <span m="2838180">we</span>
  <span m="2838230">don't</span> <span m="2838500">know.</span> <span m="2839790">But</span>
  <span m="2839940">let's</span> <span m="2840210">trace</span> <span m="2840540">through</span>
  <span m="2840780">this.</span></p><p><span m="2841060">So</span> <span m="2841260">suppose</span>
  <span m="2841800">I</span> <span m="2841950">tell</span> <span m="2842220">you</span>
  <span m="2842430">that</span> <span m="2842640">the</span> <span m="2842760">patient</span>
  <span m="2843270">has</span> <span m="2844080">manifestations</span> <span m="2845010">3</span>
  <span m="2845310">and</span> <span m="2845440">4.</span> <span m="2847280">OK.</span>
  <span m="2848460">Well,</span> <span m="2848670">you</span> <span m="2848790">would</span>
  <span m="2848940">say,</span> <span m="2850320">there</span> <span m="2850930">is</span>
  <span m="2851160">no</span> <span m="2851430">reason</span> <span m="2851820">to</span>
  <span m="2852000">think</span> <span m="2852390">that</span> <span m="2852780">the</span>
  <span m="2852870">patient</span> <span m="2853380">may</span> <span m="2853620">have</span>
  <span m="2853860">both</span> <span m="2854190">diseases,</span> <span m="2855600">because</span>
  <span m="2855990">either</span> <span m="2856320">of</span> <span m="2856470">them</span>
  <span m="2856680">can</span> <span m="2856890">explain</span> <span m="2857460">those</span>
  <span m="2857700">manifestations,</span> <span m="2859690">right?</span> <span m="2860310">So</span>
  <span m="2860490">you</span> <span m="2860640">would</span> <span m="2860790">consider</span>
  <span m="2861300">them</span> <span m="2861540">to</span> <span m="2861720">be</span>
  <span m="2861840">competitors.</span></p><p><span m="2865860">What</span> <span
  m="2866070">about</span> <span m="2866340">if</span> <span m="2866520">I</span>
  <span m="2866700">add</span> <span m="2866930">M1?</span> <span m="2869100">So</span>
  <span m="2869370">here,</span> <span m="2870360">it's</span> <span m="2870570">getting</span>
  <span m="2870900">a</span> <span m="2870960">little</span> <span m="2871230">dicier.</span>
  <span m="2872310">Now</span> <span m="2872640">you're</span> <span m="2872910">more</span>
  <span m="2873270">likely</span> <span m="2873810">to</span> <span m="2873990">think</span>
  <span m="2874320">that</span> <span m="2874530">it's</span> <span m="2874770">D1.</span>
  <span m="2876430">But</span> <span m="2876600">if</span> <span m="2876900">it's</span>
  <span m="2877170">D1,</span> <span m="2877800">that</span> <span m="2878070">could</span>
  <span m="2878280">explain</span> <span m="2878880">all</span> <span m="2879060">the</span>
  <span m="2879150">manifestations,</span> <span m="2880440">and</span> <span m="2880710">D2</span>
  <span m="2880910">is</span> <span m="2881290">still</span> <span m="2881640">viewable</span>
  <span m="2882390">as</span> <span m="2882690">a</span> <span m="2883320">competitor.</span></p><p><span
  m="2885210">On</span> <span m="2885360">the</span> <span m="2885480">other</span>
  <span m="2885690">hand,</span> <span m="2886180">if</span> <span m="2886350">I</span>
  <span m="2886500">also</span> <span m="2886920">add</span> <span m="2887280">M6,</span>
  <span m="2888900">now</span> <span m="2889200">neither</span> <span m="2889620">disease</span>
  <span m="2890130">can</span> <span m="2890370">explain</span> <span m="2890880">all</span>
  <span m="2891030">the</span> <span m="2891120">manifestations.</span> <span m="2892890">And</span>
  <span m="2893040">so</span> <span m="2893430">it's</span> <span m="2893640">more</span>
  <span m="2893940">likely,</span> <span m="2895980">somewhat</span> <span m="2896430">more</span>
  <span m="2896640">likely,</span> <span m="2897570">that</span> <span m="2898110">there</span>
  <span m="2898650">may</span> <span m="2898830">be</span> <span m="2898980">two</span>
  <span m="2899190">diseases</span> <span m="2899820">present.</span> <span m="2901050">So</span>
  <span m="2901260">what</span> <span m="2901500">Internist</span> <span m="2902100">had</span>
  <span m="2902370">was</span> <span m="2902610">this</span> <span m="2902940">interesting</span>
  <span m="2903480">heuristic,</span> <span m="2905320">which</span> <span m="2905490">said</span>
  <span m="2906390">that</span> <span m="2906810">when</span> <span m="2907110">you</span>
  <span m="2907470">get</span> <span m="2907770">that</span> <span m="2909000">complementary</span>
  <span m="2909840">situation,</span> <span m="2911490">you</span> <span m="2911670">form</span>
  <span m="2912120">a</span> <span m="2912180">differential</span> <span m="2913410">around</span>
  <span m="2913890">the</span> <span m="2914070">top</span> <span m="2914400">ranked</span>
  <span m="2914760">hypothesis.</span> <span m="2916030">In</span> <span m="2916050">other</span>
  <span m="2916230">words,</span> <span m="2917050">you</span> <span m="2917130">retain</span>
  <span m="2918330">all</span> <span m="2918510">those</span> <span m="2918840">diseases</span>
  <span m="2919920">that</span> <span m="2920430">compete</span> <span m="2921690">with</span>
  <span m="2921960">that</span> <span m="2922170">hypothesis.</span></p><p><span m="2923830">And</span>
  <span m="2923910">that</span> <span m="2924180">defines</span> <span m="2925170">a</span>
  <span m="2925350">subproblem</span> <span m="2926230">that</span> <span m="2926460">looks</span>
  <span m="2926880">like</span> <span m="2927240">the</span> <span m="2927450">acute</span>
  <span m="2927810">renal</span> <span m="2928110">failure</span> <span m="2928500">problem,</span>
  <span m="2929700">because</span> <span m="2930120">now</span> <span m="2930360">you</span>
  <span m="2930540">have</span> <span m="2930750">one</span> <span m="2931050">set</span>
  <span m="2931740">of</span> <span m="2932280">factors</span> <span m="2933030">that</span>
  <span m="2933270">you're</span> <span m="2933390">trying</span> <span m="2933720">to</span>
  <span m="2933870">explain</span> <span m="2935010">by</span> <span m="2935250">one</span>
  <span m="2935520">disease.</span> <span m="2936900">And</span> <span m="2937050">you</span>
  <span m="2937200">set</span> <span m="2937530">aside</span> <span m="2938880">all</span>
  <span m="2939090">of</span> <span m="2939240">the</span> <span m="2939390">other</span>
  <span m="2939630">manifestations</span> <span m="2940680">and</span> <span m="2940830">all</span>
  <span m="2941010">of</span> <span m="2941130">the</span> <span m="2941250">other</span>
  <span m="2941490">diseases</span> <span m="2942180">that</span> <span m="2942390">are</span>
  <span m="2942570">potentially</span> <span m="2943260">complementary.</span> <span
  m="2944670">And</span> <span m="2944790">you</span> <span m="2944910">don't</span>
  <span m="2945120">worry</span> <span m="2945390">about</span> <span m="2945690">them</span>
  <span m="2945870">for</span> <span m="2946050">the</span> <span m="2946170">moment.</span>
  <span m="2946890">Just</span> <span m="2947160">focus</span> <span m="2948210">on</span>
  <span m="2948420">this</span> <span m="2949110">cluster</span> <span m="2949680">of</span>
  <span m="2949830">things</span> <span m="2950670">that</span> <span m="2950850">are</span>
  <span m="2950970">competitors</span> <span m="2951840">to</span> <span m="2951990">explain</span>
  <span m="2952590">some</span> <span m="2952920">subset</span> <span m="2953940">of</span>
  <span m="2954120">the</span> <span m="2954210">manifestations.</span></p><p><span
  m="2956610">And</span> <span m="2958170">then</span> <span m="2958500">there</span>
  <span m="2958650">are</span> <span m="2958740">different</span> <span m="2959670">questioning</span>
  <span m="2960300">strategies.</span> <span m="2961560">So</span> <span m="2961920">depending</span>
  <span m="2962550">on</span> <span m="2962700">the</span> <span m="2962790">scores</span>
  <span m="2963510">within</span> <span m="2963960">these</span> <span m="2964230">things,</span>
  <span m="2965160">if</span> <span m="2965400">one</span> <span m="2965670">of</span>
  <span m="2965790">those</span> <span m="2966090">diseases</span> <span m="2966750">has</span>
  <span m="2967020">a</span> <span m="2967050">very</span> <span m="2967320">high</span>
  <span m="2967590">score</span> <span m="2968070">and</span> <span m="2968220">the</span>
  <span m="2968370">others</span> <span m="2968700">have</span> <span m="2968910">relatively</span>
  <span m="2969510">low</span> <span m="2969720">scores,</span> <span m="2970890">you</span>
  <span m="2971070">would</span> <span m="2971460">choose</span> <span m="2971900">a</span>
  <span m="2971990">pursue</span> <span m="2972540">strategy</span> <span m="2973260">that</span>
  <span m="2973500">says,</span> <span m="2974890">OK,</span> <span m="2975220">I'm</span>
  <span m="2975330">interested</span> <span m="2975990">in</span> <span m="2976230">asking</span>
  <span m="2976650">questions</span> <span m="2977730">that</span> <span m="2978030">will</span>
  <span m="2978240">more</span> <span m="2978540">likely</span> <span m="2978990">convince</span>
  <span m="2979590">me</span> <span m="2980280">of</span> <span m="2980490">the</span>
  <span m="2980610">correctness</span> <span m="2981480">of</span> <span m="2981660">that</span>
  <span m="2982830">leading</span> <span m="2983190">hypothesis.</span> <span m="2984850">So</span>
  <span m="2984960">you</span> <span m="2985110">look</span> <span m="2985320">for</span>
  <span m="2985470">the</span> <span m="2985620">things</span> <span m="2985950">that</span>
  <span m="2986160">it</span> <span m="2986280">predicts</span> <span m="2986700">strongly.</span></p><p><span
  m="2988500">If</span> <span m="2988740">you</span> <span m="2990330">have</span>
  <span m="2990540">a</span> <span m="2990600">very</span> <span m="2990900">large</span>
  <span m="2991320">list</span> <span m="2991740">in</span> <span m="2991870">the</span>
  <span m="2991950">differential,</span> <span m="2993210">you</span> <span m="2993360">might</span>
  <span m="2993630">say,</span> <span m="2994200">I'm</span> <span m="2994380">going</span>
  <span m="2994500">to</span> <span m="2994620">try</span> <span m="2994860">to</span>
  <span m="2994980">reduce</span> <span m="2995550">the</span> <span m="2995670">size</span>
  <span m="2996120">of</span> <span m="2996270">the</span> <span m="2996390">differential</span>
  <span m="2997620">by</span> <span m="2997830">looking</span> <span m="2998220">for</span>
  <span m="2998460">things</span> <span m="2998970">that</span> <span m="2999360">are</span>
  <span m="3000050">likely</span> <span m="3000680">in</span> <span m="3000890">some</span>
  <span m="3001190">of</span> <span m="3001310">the</span> <span m="3001430">less</span>
  <span m="3001760">likely</span> <span m="3002540">hypotheses</span> <span m="3003890">so</span>
  <span m="3004100">that</span> <span m="3004280">I</span> <span m="3004400">can</span>
  <span m="3004610">rule</span> <span m="3004850">them</span> <span m="3005060">out</span>
  <span m="3005330">if</span> <span m="3005480">that</span> <span m="3005660">thing</span>
  <span m="3005930">is</span> <span m="3006080">not</span> <span m="3006290">present.</span>
  <span m="3007910">So</span> <span m="3008300">different</span> <span m="3008690">strategies.</span>
  <span m="3009470">And</span> <span m="3009590">I'll</span> <span m="3009710">come</span>
  <span m="3009950">back</span> <span m="3010220">to</span> <span m="3010340">that</span>
  <span m="3010750">in</span> <span m="3011120">a</span> <span m="3011150">few</span>
  <span m="3011360">minutes.</span></p><p><span m="3013030">So</span> <span m="3014810">their</span>
  <span m="3015110">test,</span> <span m="3015620">of</span> <span m="3015740">course,</span>
  <span m="3016590">based</span> <span m="3016880">on</span> <span m="3017030">their</span>
  <span m="3017210">own</span> <span m="3017420">evaluation</span> <span m="3018710">was</span>
  <span m="3018950">terrific.</span> <span m="3019550">It</span> <span m="3019700">did</span>
  <span m="3019910">wonderfully</span> <span m="3020480">well.</span> <span m="3021590">The</span>
  <span m="3021740">paper</span> <span m="3022130">got</span> <span m="3022400">published</span>
  <span m="3022910">in</span> <span m="3023030"><i>The</i></span> <span m="3023120"><i>New</i></span>
  <span m="3023300"><i>England</i></span> <span m="3023540"><i>Journal</i></span>
  <span m="3023870"><i>of</i></span> <span m="3023960"><i>Medicine,</i></span> <span
  m="3024470">which</span> <span m="3024710">was</span> <span m="3024950">an</span>
  <span m="3025220">unbelievable</span> <span m="3025940">breakthrough</span> <span
  m="3027080">to</span> <span m="3027260">have</span> <span m="3027530">an</span>
  <span m="3027650">AI</span> <span m="3027980">program</span> <span m="3028580">that</span>
  <span m="3028880">the</span> <span m="3029210">editors</span> <span m="3029720">of</span>
  <span m="3029840"><i>The</i></span> <span m="3029960"><i>New</i></span> <span m="3030140"><i>England</i></span>
  <span m="3030350"><i>Journal</i></span> <span m="3030650">considered</span> <span
  m="3031220">interesting.</span></p><p><span m="3034490">Now,</span> <span m="3034920">unfortunately,</span>
  <span m="3037590">it</span> <span m="3037610">didn't</span> <span m="3037910">hold</span>
  <span m="3038210">up</span> <span m="3038390">very</span> <span m="3038690">well.</span>
  <span m="3039080">And</span> <span m="3039260">so</span> <span m="3040370">there</span>
  <span m="3040580">was</span> <span m="3040760">this</span> <span m="3040970">paper</span>
  <span m="3041390">by</span> <span m="3041660">Eta</span> <span m="3041930">Berner</span>
  <span m="3042380">and</span> <span m="3042530">her</span> <span m="3042680">colleagues</span>
  <span m="3043340">in</span> <span m="3043500">1994</span> <span m="3045200">where</span>
  <span m="3045410">they</span> <span m="3045650">evaluated</span> <span m="3046530">QMR</span>
  <span m="3047750">and</span> <span m="3048050">three</span> <span m="3048410">other</span>
  <span m="3048650">programs.</span> <span m="3049260">DXplain</span> <span m="3050060">is</span>
  <span m="3050210">very</span> <span m="3050450">similar</span> <span m="3050990">in</span>
  <span m="3051140">structure</span> <span m="3051710">to</span> <span m="3051890">QMR.</span>
  <span m="3053020">Iliad</span> <span m="3053590">and</span> <span m="3053740">Meditel</span>
  <span m="3054570">are</span> <span m="3055780">Bayesian</span> <span m="3056330">network,</span>
  <span m="3057070">or</span> <span m="3058640">almost</span> <span m="3059120">naive</span>
  <span m="3059540">Bayesian</span> <span m="3060140">types</span> <span m="3060640">of</span>
  <span m="3061040">models</span> <span m="3061670">developed</span> <span m="3062120">by</span>
  <span m="3062330">other</span> <span m="3062570">groups.</span></p><p><span m="3063740">And</span>
  <span m="3064010">they</span> <span m="3064550">looked</span> <span m="3065090">for</span>
  <span m="3065540">results,</span> <span m="3066170">which</span> <span m="3066440">is</span>
  <span m="3066590">coverage.</span> <span m="3067890">So</span> <span m="3069320">what</span>
  <span m="3069620">fraction</span> <span m="3070400">of</span> <span m="3070610">the</span>
  <span m="3070760">real</span> <span m="3071090">diagnoses</span> <span m="3072530">in</span>
  <span m="3072710">these</span> <span m="3072980">105</span> <span m="3073670">cases</span>
  <span m="3074300">that</span> <span m="3074510">they</span> <span m="3074660">chose</span>
  <span m="3075020">to</span> <span m="3075170">test</span> <span m="3075590">on</span>
  <span m="3076640">could</span> <span m="3077030">any</span> <span m="3077330">of</span>
  <span m="3077480">these</span> <span m="3077720">programs</span> <span m="3078320">actually</span>
  <span m="3078800">diagnose?</span> <span m="3079860">So</span> <span m="3080000">if</span>
  <span m="3080120">the</span> <span m="3080210">program</span> <span m="3080660">didn't</span>
  <span m="3080960">know</span> <span m="3081290">about</span> <span m="3081590">a</span>
  <span m="3081650">certain</span> <span m="3082010">disease,</span> <span m="3083150">then</span>
  <span m="3083390">obviously</span> <span m="3083990">it</span> <span m="3084110">wasn't</span>
  <span m="3084470">going</span> <span m="3084590">to</span> <span m="3084680">get</span>
  <span m="3084890">it</span> <span m="3085010">right.</span></p><p><span m="3086750">And</span>
  <span m="3086900">then</span> <span m="3087080">they</span> <span m="3087230">said,</span>
  <span m="3087600">OK,</span> <span m="3087890">of</span> <span m="3088130">the</span>
  <span m="3088250">program's</span> <span m="3088820">diagnoses,</span> <span m="3090170">what</span>
  <span m="3090350">fraction</span> <span m="3090920">were</span> <span m="3091100">considered</span>
  <span m="3091700">correct</span> <span m="3092150">by</span> <span m="3092330">the</span>
  <span m="3092480">experts?</span> <span m="3093560">What</span> <span m="3093800">was</span>
  <span m="3094040">the</span> <span m="3094160">rank</span> <span m="3094580">order</span>
  <span m="3095000">of</span> <span m="3095180">that</span> <span m="3095420">correct</span>
  <span m="3095810">diagnosis</span> <span m="3096680">among</span> <span m="3097010">the</span>
  <span m="3097130">list</span> <span m="3097430">of</span> <span m="3097550">diagnoses</span>
  <span m="3098360">that</span> <span m="3098570">the</span> <span m="3098660">program</span>
  <span m="3099170">gave?</span> <span m="3102500">The</span> <span m="3102920">experts</span>
  <span m="3103580">were</span> <span m="3104030">asked</span> <span m="3104360">to</span>
  <span m="3104540">list</span> <span m="3105020">all</span> <span m="3105260">the</span>
  <span m="3105380">plausible</span> <span m="3106070">diagnoses</span> <span m="3107000">from</span>
  <span m="3107270">these</span> <span m="3107510">cases.</span> <span m="3109010">What</span>
  <span m="3109280">fraction</span> <span m="3109910">of</span> <span m="3110060">those</span>
  <span m="3110360">showed</span> <span m="3110750">up</span> <span m="3110990">in</span>
  <span m="3111110">the</span> <span m="3111200">program's</span> <span m="3111770">top</span>
  <span m="3112070">20?</span> <span m="3113570">And</span> <span m="3113780">then</span>
  <span m="3114410">did</span> <span m="3114710">the</span> <span m="3114830">program</span>
  <span m="3115760">have</span> <span m="3116030">any</span> <span m="3116240">value</span>
  <span m="3116720">added</span> <span m="3117620">by</span> <span m="3117860">coming</span>
  <span m="3118310">up</span> <span m="3118520">with</span> <span m="3118730">things</span>
  <span m="3119150">that</span> <span m="3119390">the</span> <span m="3119540">experts</span>
  <span m="3120050">had</span> <span m="3120230">not</span> <span m="3120530">thought</span>
  <span m="3120830">about,</span> <span m="3121610">but</span> <span m="3121850">that</span>
  <span m="3122030">they</span> <span m="3122270">agreed</span> <span m="3122750">when</span>
  <span m="3122930">they</span> <span m="3123080">saw</span> <span m="3123410">them</span>
  <span m="3124330">were</span> <span m="3124640">reasonable</span> <span m="3125240">explanations</span>
  <span m="3126200">for</span> <span m="3126470">this</span> <span m="3126680">case?</span></p><p><span
  m="3128180">So</span> <span m="3128360">here</span> <span m="3128600">are</span>
  <span m="3128660">the</span> <span m="3128810">results.</span> <span m="3130130">And</span>
  <span m="3130310">what</span> <span m="3130550">you</span> <span m="3130700">see</span>
  <span m="3131120">is</span> <span m="3131420">that</span> <span m="3132980">the</span>
  <span m="3136580">diagnoses</span> <span m="3137510">in</span> <span m="3137720">these</span>
  <span m="3137930">105</span> <span m="3138560">test</span> <span m="3138890">cases,</span>
  <span m="3140960">91%</span> <span m="3142160">of</span> <span m="3142310">them</span>
  <span m="3142700">appeared</span> <span m="3143330">in</span> <span m="3143600">the</span>
  <span m="3143750">DXplain</span> <span m="3144440">program,</span> <span m="3145460">but,</span>
  <span m="3145700">for</span> <span m="3145910">example,</span> <span m="3146590">only</span>
  <span m="3146830">73%</span> <span m="3148090">of</span> <span m="3148240">them</span>
  <span m="3148510">in</span> <span m="3148660">the</span> <span m="3148750">QMR</span>
  <span m="3149350">program.</span> <span m="3150310">So</span> <span m="3150490">that</span>
  <span m="3150730">means</span> <span m="3151060">that</span> <span m="3151240">right</span>
  <span m="3151480">off</span> <span m="3151690">the</span> <span m="3151810">bat</span>
  <span m="3152110">it's</span> <span m="3152320">missing</span> <span m="3152740">about</span>
  <span m="3153010">a</span> <span m="3153070">quarter</span> <span m="3154120">of</span>
  <span m="3154270">the</span> <span m="3154390">possible</span> <span m="3154960">cases.</span></p><p><span
  m="3156620">And</span> <span m="3156670">then</span> <span m="3156880">if</span>
  <span m="3157030">you</span> <span m="3157180">look</span> <span m="3157510">at</span>
  <span m="3157780">correct</span> <span m="3158200">diagnosis,</span> <span m="3159160">you're</span>
  <span m="3159310">seeing</span> <span m="3159700">numbers</span> <span m="3160240">like</span>
  <span m="3160930">0.69,</span> <span m="3162040">0.61,</span> <span m="3163090">0.71,</span>
  <span m="3164350">et</span> <span m="3164610">cetera.</span> <span m="3165370">So</span>
  <span m="3165580">these</span> <span m="3165910">are--</span> <span m="3167710">it's</span>
  <span m="3167920">like</span> <span m="3168190">the</span> <span m="3168640">dog</span>
  <span m="3169030">who</span> <span m="3169150">sings,</span> <span m="3169720">but</span>
  <span m="3169930">badly,</span> <span m="3171200">right?</span> <span m="3172120">It's</span>
  <span m="3172570">remarkable</span> <span m="3173350">that</span> <span m="3173560">it</span>
  <span m="3173710">can</span> <span m="3173920">sing</span> <span m="3174220">at</span>
  <span m="3174340">all,</span> <span m="3174670">but</span> <span m="3175510">it's</span>
  <span m="3175660">not</span> <span m="3175840">something</span> <span m="3176290">you</span>
  <span m="3176390">want</span> <span m="3176480">to</span> <span m="3176580">listen</span>
  <span m="3176950">to.</span></p><p><span m="3180220">And</span> <span m="3180610">then</span>
  <span m="3181060">rank</span> <span m="3181660">of</span> <span m="3183670">the</span>
  <span m="3184030">correct</span> <span m="3184420">diagnosis</span> <span m="3185290">in</span>
  <span m="3185410">the</span> <span m="3185500">program</span> <span m="3186550">is</span>
  <span m="3186880">at</span> <span m="3187060">like</span> <span m="3187360">12</span>
  <span m="3187930">or</span> <span m="3188140">10</span> <span m="3188590">or</span>
  <span m="3188740">13</span> <span m="3189370">or</span> <span m="3189490">so</span>
  <span m="3189760">on.</span> <span m="3190400">So</span> <span m="3190540">it</span>
  <span m="3190660">is</span> <span m="3190870">in</span> <span m="3190990">the</span>
  <span m="3191110">top</span> <span m="3191410">20,</span> <span m="3191860">but</span>
  <span m="3192070">it's</span> <span m="3192280">not</span> <span m="3192550">at</span>
  <span m="3192670">the</span> <span m="3192790">top</span> <span m="3193810">of</span>
  <span m="3194200">the</span> <span m="3194620">top</span> <span m="3194830">20.</span>
  <span m="3195740">So</span> <span m="3195850">the</span> <span m="3195940">results</span>
  <span m="3196450">were</span> <span m="3196900">a</span> <span m="3197170">bit</span>
  <span m="3197410">disappointing.</span> <span m="3199870">And</span> <span m="3201220">depending</span>
  <span m="3201820">on</span> <span m="3201970">where</span> <span m="3202240">you</span>
  <span m="3202420">put</span> <span m="3202660">the</span> <span m="3202810">cut</span>
  <span m="3203050">off,</span> <span m="3204310">you</span> <span m="3204550">get</span>
  <span m="3204910">the</span> <span m="3205060">proportion</span> <span m="3205720">of</span>
  <span m="3205810">cases</span> <span m="3206410">where</span> <span m="3207145">a</span>
  <span m="3207490">correct</span> <span m="3207880">diagnosis</span> <span m="3209650">is</span>
  <span m="3209920">within</span> <span m="3210400">the</span> <span m="3210550">top</span>
  <span m="3210910">end.</span> <span m="3211810">And</span> <span m="3211990">you</span>
  <span m="3212140">see</span> <span m="3212470">that</span> <span m="3213460">at</span>
  <span m="3213700">20,</span> <span m="3214610">you're</span> <span m="3214910">up</span>
  <span m="3215240">at</span> <span m="3215620">a</span> <span m="3215710">little</span>
  <span m="3216010">over</span> <span m="3216280">0.5</span> <span m="3217060">for</span>
  <span m="3217390">most</span> <span m="3217690">of</span> <span m="3217750">these</span>
  <span m="3218020">programs.</span></p><p><span m="3219280">And</span> <span m="3219550">it</span>
  <span m="3219760">gets</span> <span m="3220090">better</span> <span m="3220600">if</span>
  <span m="3220840">you</span> <span m="3221020">extend</span> <span m="3221530">the</span>
  <span m="3221650">list</span> <span m="3222190">to</span> <span m="3222340">longer</span>
  <span m="3222820">and</span> <span m="3222940">longer.</span> <span m="3223870">Of</span>
  <span m="3223990">course,</span> <span m="3224290">if</span> <span m="3224470">you</span>
  <span m="3224620">extended</span> <span m="3225190">the</span> <span m="3225340">list</span>
  <span m="3225700">to</span> <span m="3226630">100,</span> <span m="3227320">then</span>
  <span m="3227740">you</span> <span m="3228130">reach</span> <span m="3228430">100%,</span>
  <span m="3229330">but</span> <span m="3229750">it</span> <span m="3229840">wouldn't</span>
  <span m="3230110">be</span> <span m="3230290">practically</span> <span m="3230950">very</span>
  <span m="3231190">useful.</span></p><p><span m="3232013">AUDIENCE:</span> <span
  m="3232199">Why</span> <span m="3232386">didn't</span> <span m="3232760">they</span>
  <span m="3233050">somehow</span> <span m="3233320">compare</span> <span m="3233590">it</span>
  <span m="3234089">to the</span> <span m="3234588">human</span> <span m="3235087">decision?</span></p><p><span
  m="3238730">PETER SZOLOVITS:</span> <span m="3238805">Well,</span> <span m="3238880">so</span>
  <span m="3239360">first</span> <span m="3239690">of</span> <span m="3239780">all,</span>
  <span m="3239900">they</span> <span m="3240110">assumed</span> <span m="3240590">that</span>
  <span m="3240830">their</span> <span m="3241040">experts</span> <span m="3241610">were</span>
  <span m="3241760">perfect.</span> <span m="3243260">So</span> <span m="3244460">they</span>
  <span m="3244700">were</span> <span m="3244970">the</span> <span m="3245120">gold</span>
  <span m="3245390">standard.</span> <span m="3246150">So</span> <span m="3246740">they</span>
  <span m="3246980">were</span> <span m="3247250">comparing</span> <span m="3247850">it</span>
  <span m="3247910">to</span> <span m="3248180">a</span> <span m="3248230">human</span>
  <span m="3248990">in</span> <span m="3249140">a</span> <span m="3249200">way.</span></p><p><span
  m="3250090">AUDIENCE:</span> <span m="3250340">Yeah.</span></p><p><span m="3255090">PETER
  SZOLOVITS:</span> <span m="3255260">OK.</span> <span m="3255430">So</span> <span
  m="3255610">the</span> <span m="3255730">bottom</span> <span m="3256090">line</span>
  <span m="3256570">is</span> <span m="3256930">that</span> <span m="3259210">although</span>
  <span m="3259540">the</span> <span m="3259660">sensitivity</span> <span m="3260350">and</span>
  <span m="3260470">specificity</span> <span m="3261260">were</span> <span m="3261460">not</span>
  <span m="3261730">impressive,</span> <span m="3263190">the</span> <span m="3263350">programs</span>
  <span m="3264000">were</span> <span m="3264520">potentially</span> <span m="3265240">useful,</span>
  <span m="3265780">because</span> <span m="3266200">they</span> <span m="3266380">had</span>
  <span m="3267070">interactive</span> <span m="3267670">displays</span> <span m="3268420">of</span>
  <span m="3268570">signs</span> <span m="3269020">and</span> <span m="3269140">symptoms</span>
  <span m="3269650">associated</span> <span m="3270410">with</span> <span m="3270550">diseases.</span>
  <span m="3271830">They</span> <span m="3271990">could</span> <span m="3272200">give</span>
  <span m="3272380">you</span> <span m="3272530">the</span> <span m="3272650">relative</span>
  <span m="3273160">likelihood</span> <span m="3273790">of</span> <span m="3273880">various</span>
  <span m="3274810">diagnoses.</span> <span m="3276200">And</span> <span m="3278140">they</span>
  <span m="3278320">concluded</span> <span m="3279010">that</span> <span m="3279220">they</span>
  <span m="3279400">needed</span> <span m="3279700">to</span> <span m="3279850">study</span>
  <span m="3280300">the</span> <span m="3280480">effects</span> <span m="3281200">of</span>
  <span m="3281980">whether</span> <span m="3282370">a</span> <span m="3282400">program</span>
  <span m="3282940">like</span> <span m="3283180">this</span> <span m="3283510">actually</span>
  <span m="3284020">helped</span> <span m="3284420">a</span> <span m="3284500">doctor</span>
  <span m="3284980">perform</span> <span m="3285550">medicine</span> <span m="3286060">better.</span></p><p><span
  m="3287680">So</span> <span m="3288130">just</span> <span m="3289300">here's</span>
  <span m="3289630">an</span> <span m="3289720">example.</span> <span m="3290750">I</span>
  <span m="3290830">did</span> <span m="3291010">a</span> <span m="3291070">reconstruction</span>
  <span m="3292000">of</span> <span m="3292120">this</span> <span m="3292330">program.</span>
  <span m="3292970">This</span> <span m="3293110">is</span> <span m="3293290">the</span>
  <span m="3293410">kind</span> <span m="3293710">of</span> <span m="3294310">exploration</span>
  <span m="3295120">you</span> <span m="3295240">could</span> <span m="3295420">say.</span>
  <span m="3295810">So</span> <span m="3296620">if</span> <span m="3296800">you</span>
  <span m="3297790">click</span> <span m="3298090">on</span> <span m="3298330">angina</span>
  <span m="3298710">pectoris,</span> <span m="3300430">here</span> <span m="3300670">are</span>
  <span m="3300820">the</span> <span m="3300940">findings</span> <span m="3301570">that</span>
  <span m="3301690">are</span> <span m="3301810">associated</span> <span m="3302590">with</span>
  <span m="3302800">it.</span> <span m="3302950">So</span> <span m="3303130">you</span>
  <span m="3303220">can</span> <span m="3303430">browse</span> <span m="3303850">through</span>
  <span m="3304060">its</span> <span m="3304270">database.</span> <span m="3305590">You</span>
  <span m="3305800">can</span> <span m="3306280">type</span> <span m="3306640">in</span>
  <span m="3306850">an</span> <span m="3307000">example</span> <span m="3307600">case,</span>
  <span m="3308140">or</span> <span m="3308320">select</span> <span m="3308830">an</span>
  <span m="3308950">example</span> <span m="3309490">case.</span></p><p><span m="3310360">So</span>
  <span m="3310540">this</span> <span m="3310780">is</span> <span m="3310930">one</span>
  <span m="3311170">of</span> <span m="3311260">those</span> <span m="3311590">clinical</span>
  <span m="3312700">pathological</span> <span m="3313480">conference</span> <span
  m="3314050">cases,</span> <span m="3315770">and</span> <span m="3315910">then</span>
  <span m="3316420">the</span> <span m="3316840">manifestations</span> <span m="3317920">that</span>
  <span m="3318070">are</span> <span m="3318190">present</span> <span m="3318790">and</span>
  <span m="3319000">absent,</span> <span m="3320110">and</span> <span m="3320260">then</span>
  <span m="3320470">you</span> <span m="3320620">can</span> <span m="3320860">get</span>
  <span m="3321070">an</span> <span m="3321190">interpretation</span> <span m="3322690">that</span>
  <span m="3322960">says,</span> <span m="3323600">OK,</span> <span m="3324410">this</span>
  <span m="3324700">is</span> <span m="3324940">our</span> <span m="3325120">differential.</span>
  <span m="3326920">And</span> <span m="3327130">these</span> <span m="3327520">are</span>
  <span m="3327700">the</span> <span m="3327850">complementary</span> <span m="3329230">hypotheses.</span>
  <span m="3330760">And</span> <span m="3330940">therefore</span> <span m="3331480">these</span>
  <span m="3331930">are</span> <span m="3332500">the</span> <span m="3334030">manifestations</span>
  <span m="3335350">that</span> <span m="3335680">we</span> <span m="3336370">set</span>
  <span m="3336700">aside,</span> <span m="3338920">whereas</span> <span m="3339370">these</span>
  <span m="3339670">are</span> <span m="3339820">the</span> <span m="3339940">ones</span>
  <span m="3340300">explained</span> <span m="3340990">by</span> <span m="3341230">that</span>
  <span m="3341470">set</span> <span m="3341740">of</span> <span m="3341860">diseases.</span>
  <span m="3342580">And</span> <span m="3342700">so</span> <span m="3342910">you</span>
  <span m="3343000">could</span> <span m="3343210">watch</span> <span m="3344050">how</span>
  <span m="3344290">the</span> <span m="3344410">program</span> <span m="3344950">does</span>
  <span m="3345250">its</span> <span m="3345820">reasoning.</span></p><p><span m="3349210">Well,</span>
  <span m="3349660">then</span> <span m="3350080">a</span> <span m="3350140">group</span>
  <span m="3350470">at</span> <span m="3350560">Stanford</span> <span m="3352120">came</span>
  <span m="3352450">along</span> <span m="3353050">when</span> <span m="3354010">belief</span>
  <span m="3354430">networks</span> <span m="3355030">or</span> <span m="3355120">Bayesian</span>
  <span m="3355570">networks</span> <span m="3356140">were</span> <span m="3356320">created,</span>
  <span m="3357520">and</span> <span m="3357700">said,</span> <span m="3358190">hey,</span>
  <span m="3358490">why</span> <span m="3358570">don't</span> <span m="3358750">we</span>
  <span m="3359110">treat</span> <span m="3359470">this</span> <span m="3359950">database</span>
  <span m="3361330">as</span> <span m="3361690">if</span> <span m="3361990">it</span>
  <span m="3362140">were</span> <span m="3362710">a</span> <span m="3363250">Bayesian</span>
  <span m="3363730">network</span> <span m="3364960">and</span> <span m="3365170">see</span>
  <span m="3365440">if</span> <span m="3365590">we</span> <span m="3365740">can</span>
  <span m="3366580">evaluate</span> <span m="3367210">things</span> <span m="3367540">that</span>
  <span m="3367780">way?</span> <span m="3368650">So</span> <span m="3368950">they</span>
  <span m="3369160">had</span> <span m="3369370">to</span> <span m="3369520">fill</span>
  <span m="3369880">in</span> <span m="3370060">a</span> <span m="3370090">lot</span>
  <span m="3370360">of</span> <span m="3370480">details.</span></p><p><span m="3371630">They</span>
  <span m="3371920">wound</span> <span m="3372310">up</span> <span m="3372490">using</span>
  <span m="3374350">the</span> <span m="3374640">QMR</span> <span m="3376060">database</span>
  <span m="3377200">with</span> <span m="3377830">a</span> <span m="3377920">binary</span>
  <span m="3378460">interpretation.</span> <span m="3379560">So</span> <span m="3379880">a</span>
  <span m="3380170">disease</span> <span m="3380680">was</span> <span m="3380890">present</span>
  <span m="3381340">or</span> <span m="3381490">absent.</span> <span m="3381980">The</span>
  <span m="3382060">manifestation</span> <span m="3383560">was</span> <span m="3383830">present</span>
  <span m="3384280">or</span> <span m="3384400">absent.</span> <span m="3385510">They</span>
  <span m="3385720">used</span> <span m="3386050">causal</span> <span m="3386500">independence,</span>
  <span m="3387310">or</span> <span m="3387470">a</span> <span m="3387520">leaky</span>
  <span m="3387940">noisy-OR,</span> <span m="3388900">which</span> <span m="3389170">I</span>
  <span m="3389260">think</span> <span m="3389530">you've</span> <span m="3389740">seen</span>
  <span m="3390460">in</span> <span m="3390610">other</span> <span m="3390850">contexts.</span>
  <span m="3392140">So</span> <span m="3392320">this</span> <span m="3392590">just</span>
  <span m="3392830">says</span> <span m="3394150">if</span> <span m="3394360">there</span>
  <span m="3394570">are</span> <span m="3394750">multiple</span> <span m="3396220">independent</span>
  <span m="3396940">causes</span> <span m="3397510">of</span> <span m="3397630">something,</span>
  <span m="3398590">how</span> <span m="3398800">likely</span> <span m="3399310">is</span>
  <span m="3399490">it</span> <span m="3399610">to</span> <span m="3399790">happen</span>
  <span m="3400270">depending</span> <span m="3400870">on</span> <span m="3401080">which</span>
  <span m="3401350">of</span> <span m="3401470">those</span> <span m="3401870">is</span>
  <span m="3402460">present</span> <span m="3402940">or</span> <span m="3403090">not.</span>
  <span m="3403970">And</span> <span m="3404020">there</span> <span m="3404090">is</span>
  <span m="3404260">a</span> <span m="3404320">simplified</span> <span m="3405760">way</span>
  <span m="3406000">of</span> <span m="3406120">doing</span> <span m="3406420">that</span>
  <span m="3407110">calculation,</span> <span m="3408580">which</span> <span m="3409060">corresponds</span>
  <span m="3409990">to</span> <span m="3410200">sort</span> <span m="3410500">of</span>
  <span m="3410620">causal</span> <span m="3411070">independence</span> <span m="3412300">and</span>
  <span m="3412480">is</span> <span m="3412630">computationally</span> <span m="3413620">reasonably</span>
  <span m="3414820">fast</span> <span m="3415240">to</span> <span m="3415390">do.</span></p><p><span
  m="3416980">And</span> <span m="3417190">then</span> <span m="3418300">they</span>
  <span m="3418630">also</span> <span m="3419590">estimated</span> <span m="3420220">priors</span>
  <span m="3421120">on</span> <span m="3421330">the</span> <span m="3421420">various</span>
  <span m="3421900">diagnoses</span> <span m="3423250">from</span> <span m="3423580">national</span>
  <span m="3424060">health</span> <span m="3424270">statistics,</span> <span m="3425140">because</span>
  <span m="3425560">the</span> <span m="3425710">original</span> <span m="3426190">data</span>
  <span m="3426970">did</span> <span m="3427150">not</span> <span m="3427420">have</span>
  <span m="3427630">prior</span> <span m="3428020">data--</span> <span m="3428540">priors.</span>
  <span m="3430330">They</span> <span m="3430540">wound</span> <span m="3430840">up</span>
  <span m="3430990">not</span> <span m="3431320">using</span> <span m="3431860">the</span>
  <span m="3432120">evoking</span> <span m="3432610">strengths,</span> <span m="3434110">because</span>
  <span m="3434560">they</span> <span m="3434740">were</span> <span m="3435130">doing</span>
  <span m="3435700">a</span> <span m="3436120">pretty</span> <span m="3436420">straight</span>
  <span m="3436990">Bayesian</span> <span m="3437560">model</span> <span m="3438460">where</span>
  <span m="3438790">all</span> <span m="3439000">you</span> <span m="3439150">need</span>
  <span m="3439420">is</span> <span m="3439570">the</span> <span m="3439690">priors</span>
  <span m="3440250">and</span> <span m="3440380">the</span> <span m="3440470">conditionals.</span></p><p><span
  m="3441730">They</span> <span m="3441940">took</span> <span m="3442210">the</span>
  <span m="3442360">frequency</span> <span m="3443200">as</span> <span m="3443410">a</span>
  <span m="3443470">kind</span> <span m="3443800">of</span> <span m="3443920">scaled</span>
  <span m="3444460">conditional,</span> <span m="3446620">and</span> <span m="3446770">then</span>
  <span m="3447220">built</span> <span m="3447610">a</span> <span m="3447640">system</span>
  <span m="3448150">based</span> <span m="3448510">on</span> <span m="3448660">that.</span>
  <span m="3449230">And</span> <span m="3449500">I'll</span> <span m="3449620">just</span>
  <span m="3449830">show</span> <span m="3450040">you</span> <span m="3450190">the</span>
  <span m="3450310">results.</span> <span m="3451520">So</span> <span m="3453220">they</span>
  <span m="3453460">took</span> <span m="3453760">a</span> <span m="3453820">bunch</span>
  <span m="3454150">of</span> <span m="3454240"><i>Scientific</i></span> <span m="3454840"><i>American</i></span>
  <span m="3455320">medicine</span> <span m="3455830">cases</span> <span m="3456940">and</span>
  <span m="3457150">said,</span> <span m="3460580">what</span> <span m="3460750">are</span>
  <span m="3460900">the</span> <span m="3461020">ranks</span> <span m="3461560">assigned</span>
  <span m="3462010">to</span> <span m="3462190">the</span> <span m="3462310">reference</span>
  <span m="3462880">diagnoses</span> <span m="3463930">of</span> <span m="3464110">these</span>
  <span m="3464380">23</span> <span m="3464980">cases?</span> <span m="3466150">And</span>
  <span m="3466360">you</span> <span m="3466510">see</span> <span m="3466810">that</span>
  <span m="3467170">like</span> <span m="3467440">in</span> <span m="3467560">case</span>
  <span m="3467890">number</span> <span m="3468250">one,</span> <span m="3469030">QMR</span>
  <span m="3470170">ranked</span> <span m="3470710">the</span> <span m="3470890">correct</span>
  <span m="3471310">solution</span> <span m="3471940">as</span> <span m="3472150">number</span>
  <span m="3472480">six,</span> <span m="3473920">but</span> <span m="3474460">their</span>
  <span m="3475210">two</span> <span m="3475480">methods,</span> <span m="3476170">TB</span>
  <span m="3476600">and</span> <span m="3477040">iterative</span> <span m="3477640">TB</span>
  <span m="3479320">ranked</span> <span m="3479700">it</span> <span m="3479830">as</span>
  <span m="3479980">number</span> <span m="3480340">one.</span> <span m="3481180">And</span>
  <span m="3481330">then</span> <span m="3481570">these</span> <span m="3481930">are</span>
  <span m="3482800">attempts</span> <span m="3483340">to</span> <span m="3483490">do</span>
  <span m="3483940">a</span> <span m="3484030">kind</span> <span m="3484450">of</span>
  <span m="3485740">ablation</span> <span m="3486310">analysis</span> <span m="3487030">to</span>
  <span m="3487150">see</span> <span m="3487900">how</span> <span m="3488080">well</span>
  <span m="3488350">the</span> <span m="3488470">program</span> <span m="3488950">works</span>
  <span m="3489790">if</span> <span m="3490000">you</span> <span m="3490150">take</span>
  <span m="3490450">away</span> <span m="3490750">various</span> <span m="3491320">of</span>
  <span m="3491470">its</span> <span m="3491650">clever</span> <span m="3492010">features.</span></p><p><span
  m="3493670">But</span> <span m="3493930">what</span> <span m="3494170">you</span>
  <span m="3494290">see</span> <span m="3494590">is</span> <span m="3494770">that</span>
  <span m="3495140">it</span> <span m="3495340">works</span> <span m="3495700">reasonably</span>
  <span m="3496360">well,</span> <span m="3497170">except</span> <span m="3497590">for</span>
  <span m="3498340">a</span> <span m="3498400">few</span> <span m="3498670">cases.</span>
  <span m="3499210">So</span> <span m="3499510">case</span> <span m="3499840">number</span>
  <span m="3500140">23,</span> <span m="3503470">all</span> <span m="3503680">variants</span>
  <span m="3504280">of</span> <span m="3504400">the</span> <span m="3504520">program</span>
  <span m="3505060">did</span> <span m="3505300">badly.</span> <span m="3506390">And</span>
  <span m="3506440">then</span> <span m="3506620">they</span> <span m="3506830">excused</span>
  <span m="3507400">themselves</span> <span m="3508090">and</span> <span m="3508240">said,</span>
  <span m="3508510">well,</span> <span m="3508810">there's</span> <span m="3509080">actually</span>
  <span m="3510070">a</span> <span m="3510160">generalization</span> <span m="3511210">of</span>
  <span m="3511360">the</span> <span m="3511510">disease</span> <span m="3512080">that</span>
  <span m="3512320">was</span> <span m="3512560">in</span> <span m="3512680">the</span>
  <span m="3512770"><i>Scientific</i></span> <span m="3513280"><i>American</i></span>
  <span m="3513730">medicine</span> <span m="3514750">conclusion,</span> <span m="3516010">which</span>
  <span m="3516340">the</span> <span m="3516430">programs</span> <span m="3517030">did</span>
  <span m="3517250">find,</span> <span m="3518580">and</span> <span m="3518770">so</span>
  <span m="3518980">that</span> <span m="3519220">would</span> <span m="3519400">have</span>
  <span m="3519520">been</span> <span m="3519730">number</span> <span m="3520060">one</span>
  <span m="3520600">across</span> <span m="3521050">the</span> <span m="3521170">board.</span>
  <span m="3521980">So</span> <span m="3522220">they</span> <span m="3522400">can</span>
  <span m="3522610">sort of</span> <span m="3522955">make</span> <span m="3523300">a</span>
  <span m="3523480">kind</span> <span m="3523810">of</span> <span m="3523940">handwavy</span>
  <span m="3524530">argument</span> <span m="3525070">that</span> <span m="3525700">it</span>
  <span m="3525850">really</span> <span m="3526150">got</span> <span m="3526450">that</span>
  <span m="3526660">one</span> <span m="3526870">right.</span></p><p><span m="3527840">And</span>
  <span m="3527890">so</span> <span m="3528100">these</span> <span m="3528370">were</span>
  <span m="3528520">pretty</span> <span m="3528850">good.</span> <span m="3530290">And</span>
  <span m="3531670">so</span> <span m="3532150">this</span> <span m="3532420">validated</span>
  <span m="3533200">the</span> <span m="3533380">idea</span> <span m="3534340">of</span>
  <span m="3534550">using</span> <span m="3534970">this</span> <span m="3535210">model</span>
  <span m="3538030">in</span> <span m="3538420">that</span> <span m="3538660">way.</span></p><p><span
  m="3539740">Now,</span> <span m="3540280">today</span> <span m="3541300">you</span>
  <span m="3541510">can</span> <span m="3541720">go</span> <span m="3541990">out</span>
  <span m="3542530">and</span> <span m="3543340">go</span> <span m="3543610">to</span>
  <span m="3543730">your</span> <span m="3544090">favorite</span> <span m="3545260">Google</span>
  <span m="3545740">App</span> <span m="3545960">store</span> <span m="3546490">or</span>
  <span m="3547210">Apple's</span> <span m="3547660">app</span> <span m="3547900">store</span>
  <span m="3548350">or</span> <span m="3549460">anybody's</span> <span m="3550030">app</span>
  <span m="3550240">store</span> <span m="3551080">and</span> <span m="3551320">download</span>
  <span m="3551890">tons</span> <span m="3552310">and</span> <span m="3552610">tons</span>
  <span m="3552970">and</span> <span m="3553090">tons</span> <span m="3553700">of</span>
  <span m="3554240">symptom</span> <span m="3554690">checkers.</span> <span m="3556640">So</span>
  <span m="3556820">I</span> <span m="3556910">wanted</span> <span m="3557180">to</span>
  <span m="3557330">give</span> <span m="3557570">you</span> <span m="3557720">a</span>
  <span m="3557780">demo</span> <span m="3558200">of</span> <span m="3558350">one</span>
  <span m="3558560">of</span> <span m="3558680">these</span> <span m="3559130">if</span>
  <span m="3561110">it</span> <span m="3561230">works.</span></p><p><span m="3563620">OK.</span>
  <span m="3564680">So</span> <span m="3564860">I</span> <span m="3564980">was</span>
  <span m="3565160">playing</span> <span m="3565580">earlier</span> <span m="3566190">with</span>
  <span m="3566900">having</span> <span m="3567290">abdominal</span> <span m="3567860">pain</span>
  <span m="3568220">and</span> <span m="3568370">headache.</span> <span m="3569690">So</span>
  <span m="3571190">let's</span> <span m="3571460">start</span> <span m="3572090">a</span>
  <span m="3572180">new</span> <span m="3572450">one.</span> <span m="3573980">So</span>
  <span m="3574280">type</span> <span m="3574700">in</span> <span m="3575120">how</span>
  <span m="3575330">you're</span> <span m="3575480">feeling</span> <span m="3575870">today.</span></p><p><span
  m="3577070">Should</span> <span m="3577310">we</span> <span m="3577490">have</span>
  <span m="3577670">a</span> <span m="3577760">cough,</span> <span m="3578180">or</span>
  <span m="3578240">runny</span> <span m="3578570">nose,</span> <span m="3579440">abdominal</span>
  <span m="3580040">pain,</span> <span m="3580500">fever,</span> <span m="3580910">sore</span>
  <span m="3581210">throat,</span> <span m="3581570">headache,</span> <span m="3581960">back</span>
  <span m="3582260">pain,</span> <span m="3583080">fatigue,</span> <span m="3583560">diarrhea,</span>
  <span m="3584280">or</span> <span m="3584330">phlegm?</span> <span m="3587120">Phlegm?</span>
  <span m="3587630">Phlegm</span> <span m="3588020">is</span> <span m="3588170">the</span>
  <span m="3588330">winner.</span> <span m="3591530">Phlegm</span> <span m="3591920">is</span>
  <span m="3592070">like</span> <span m="3592310">coughing</span> <span m="3592850">up</span>
  <span m="3593240">crap</span> <span m="3593600">in</span> <span m="3593720">your</span>
  <span m="3593870">throat.</span></p><p><span m="3594703">AUDIENCE:</span> <span
  m="3594939">Oh,</span> <span m="3595176">luckily,</span> <span m="3595649">they
  visualize</span> <span m="3596122">it.</span></p><p><span m="3598960">PETER SZOLOVITS:</span>
  <span m="3599196">Right.</span> <span m="3600380">So</span> <span m="3601310">tell</span>
  <span m="3601580">me</span> <span m="3601730">about</span> <span m="3602090">your</span>
  <span m="3602210">phlegm.</span> <span m="3602590">When</span> <span m="3603020">did</span>
  <span m="3603170">it</span> <span m="3603290">start?</span></p><p><span m="3604658">AUDIENCE:</span>
  <span m="3604816">Last</span> <span m="3604974">week.</span></p><p><span m="3606080">PETER
  SZOLOVITS:</span> <span m="3606230">Last</span> <span m="3606680">week?</span> <span
  m="3607000">OK.</span></p><p><span m="3614870">I</span> <span m="3615230">signed</span>
  <span m="3615620">in</span> <span m="3615740">as</span> <span m="3615920">Paul,</span>
  <span m="3616370">because</span> <span m="3617570">I</span> <span m="3617630">didn't</span>
  <span m="3617810">want</span> <span m="3617990">to</span> <span m="3618050">be</span>
  <span m="3618170">associated</span> <span m="3619070">with</span> <span m="3619450">any</span>
  <span m="3619530">of</span> <span m="3619990">this</span> <span m="3620450">data.</span></p><p><span
  m="3621830">So</span> <span m="3622510">was</span> <span m="3622850">the</span>
  <span m="3622970">phlegm</span> <span m="3623360">bloody</span> <span m="3623840">or</span>
  <span m="3624320">pus-like</span> <span m="3624980">or</span> <span m="3625130">watery</span>
  <span m="3625790">or</span> <span m="3625940">none</span> <span m="3626150">of</span>
  <span m="3626270">the</span> <span m="3626390">above?</span></p><p><span m="3629558">AUDIENCE:</span>
  <span m="3629676">None</span> <span m="3629794">of</span> <span m="3629912">the</span>
  <span m="3630031">above.</span></p><p><span m="3630980">PETER SZOLOVITS:</span>
  <span m="3631070">None</span> <span m="3631160">of</span> <span m="3631280">the</span>
  <span m="3631400">above.</span> <span m="3632040">So</span> <span m="3632120">what</span>
  <span m="3632360">was</span> <span m="3632540">it</span> <span m="3632660">like?</span></p><p><span
  m="3634370">AUDIENCE:</span> <span m="3634395">I</span> <span m="3634420">don't</span>
  <span m="3634550">know.</span> <span m="3634630">Paul?</span></p><p><span m="3636920">PETER
  SZOLOVITS:</span> <span m="3636980">Is</span> <span m="3637040">it</span> <span
  m="3637160">any</span> <span m="3637370">of</span> <span m="3637490">these</span>
  <span m="3637760">colors?</span></p><p><span m="3638756">AUDIENCE:</span> <span
  m="3638969">Green.</span></p><p><span m="3640890">PETER SZOLOVITS:</span> <span
  m="3640945">I</span> <span m="3641000">think</span> <span m="3641210">I'll</span>
  <span m="3641510">make</span> <span m="3641810">it</span> <span m="3641930">yellow.</span>
  <span m="3644250">Next.</span></p><p><span m="3647520">Does</span> <span m="3647850">it</span>
  <span m="3647940">happen</span> <span m="3648360">in</span> <span m="3648450">the</span>
  <span m="3648540">morning,</span> <span m="3649000">midday,</span> <span m="3649290">evening,</span>
  <span m="3649650">nighttime,</span> <span m="3650340">or</span> <span m="3650550">a</span>
  <span m="3650580">specific</span> <span m="3651210">time</span> <span m="3651510">of</span>
  <span m="3651630">year?</span></p><p><span m="3651930">AUDIENCE:</span> <span m="3652167">Specific</span>
  <span m="3652405">time</span> <span m="3652880">of</span> <span m="3653355">year.</span></p><p><span
  m="3653830">AUDIENCE:</span> <span m="3654067">Yeah.</span> <span m="3654305">Specific
  time of year.</span></p><p><span m="3654780">PETER SZOLOVITS:</span> <span m="3654945">Specific</span>
  <span m="3655440">time</span> <span m="3655680">of year.</span></p><p><span m="3660840">And</span>
  <span m="3660990">does</span> <span m="3661230">lying</span> <span m="3661560">down</span>
  <span m="3661860">or</span> <span m="3661980">physical</span> <span m="3662490">activity</span>
  <span m="3663030">make</span> <span m="3663300">it</span> <span m="3663420">worse?</span></p><p><span
  m="3664306">AUDIENCE:</span> <span m="3664422">Well,</span> <span m="3664539">it's</span>
  <span m="3664772">generally</span> <span m="3665238">not worse.</span> <span m="3665704">So
  that's physical</span> <span m="3666170">activity.</span></p><p><span m="3668040">PETER
  SZOLOVITS:</span> <span m="3668172">Physical</span> <span m="3668570">activity.</span></p><p><span
  m="3673240">How</span> <span m="3673510">often</span> <span m="3673840">is</span>
  <span m="3673990">this</span> <span m="3674230">a</span> <span m="3674290">problem?</span>
  <span m="3676180">I</span> <span m="3676390">don't</span> <span m="3676540">know.
  A</span> <span m="3676690">couple</span> <span m="3677020">times</span> <span m="3677380">a</span>
  <span m="3677440">week</span> <span m="3677740">maybe.</span></p><p><span m="3682150">Did</span>
  <span m="3682420">eating</span> <span m="3682810">suspect</span> <span m="3683410">food</span>
  <span m="3683830">trigger</span> <span m="3684250">your</span> <span m="3684460">phlegm?</span></p><p><span
  m="3686368">AUDIENCE:</span> <span m="3686611">No.</span></p><p><span m="3687340">PETER
  SZOLOVITS:</span> <span m="3687370">I</span> <span m="3687400">don't</span> <span
  m="3687520">know.</span> <span m="3688030">I</span> <span m="3688090">don't</span>
  <span m="3688240">know</span> <span m="3688390">what</span> <span m="3688540">a</span>
  <span m="3688600">suspect</span> <span m="3689110">food</span> <span m="3689410">is.</span></p><p><span
  m="3689620">AUDIENCE:</span> <span m="3689835">[INAUDIBLE]</span> <span m="3690050">food.</span></p><p><span
  m="3692200">PETER SZOLOVITS:</span> <span m="3692305">Yeah.</span> <span m="3692410">This</span>
  <span m="3692650">is</span> <span m="3692840">going</span> <span m="3692950">to</span>
  <span m="3693280">kill</span> <span m="3693580">most</span> <span m="3693910">of</span>
  <span m="3693970">my</span> <span m="3694210">time.</span></p><p><span m="3696358">AUDIENCE:</span>
  <span m="3696507">Is</span> <span m="3696656">it</span> <span m="3696805">getting</span>
  <span m="3697252">better?</span></p><p><span m="3700150">PETER SZOLOVITS:</span>
  <span m="3700375">Is</span> <span m="3700600">it</span> <span m="3700720">improving?</span>
  <span m="3701320">Sure,</span> <span m="3701710">it's</span> <span m="3701920">improving.</span></p><p><span
  m="3706450">Can</span> <span m="3706660">I</span> <span m="3706780">think</span>
  <span m="3707080">of</span> <span m="3707200">another</span> <span m="3707500">related</span>
  <span m="3708010">symptom?</span> <span m="3708640">No.</span></p><p><span m="3709780">I'm</span>
  <span m="3709900">comparing</span> <span m="3710440">your</span> <span m="3710590">case</span>
  <span m="3710980">to</span> <span m="3711250">men</span> <span m="3711610">aged</span>
  <span m="3712030">66</span> <span m="3713080">to</span> <span m="3713230">72.</span>
  <span m="3714595">A</span> <span m="3714880">number</span> <span m="3715210">of</span>
  <span m="3715300">similar</span> <span m="3715750">cases</span> <span m="3716350">gets</span>
  <span m="3716620">more</span> <span m="3716860">refined.</span></p><p><span m="3718030">Do</span>
  <span m="3718210">I</span> <span m="3718330">have</span> <span m="3718540">shortness</span>
  <span m="3719110">of</span> <span m="3719230">breath?</span> <span m="3720220">No.</span>
  <span m="3722470">That's</span> <span m="3722770">good.</span> <span m="3723310">All</span>
  <span m="3723400">right.</span></p><p><span m="3723700">Do</span> <span m="3723940">I</span>
  <span m="3724060">have</span> <span m="3724240">a</span> <span m="3724300">runny</span>
  <span m="3724570">nose?</span> <span m="3724990">Yeah,</span> <span m="3725260">sure.</span>
  <span m="3725620">I</span> <span m="3725740">have</span> <span m="3725950">a</span>
  <span m="3725980">runny</span> <span m="3726280">nose.</span> <span m="3730900">It's--</span>
  <span m="3731680">I</span> <span m="3731830">don't</span> <span m="3731950">know--
  a</span> <span m="3732100">watery,</span> <span m="3732850">runny</span> <span m="3733180">nose.</span></p><p><span
  m="3737482">AUDIENCE:</span> <span m="3737640">Does</span> <span m="3737798">it</span>
  <span m="3737956">say you've</span> <span m="3738430">got to call</span> <span m="3738904">[INAUDIBLE]?</span></p><p><span
  m="3741280">PETER SZOLOVITS:</span> <span m="3741415">Well,</span> <span m="3741550">I'm</span>
  <span m="3741940">going</span> <span m="3742060">to</span> <span m="3742150">stop,</span>
  <span m="3742570">because</span> <span m="3742840">it</span> <span m="3742940">will</span>
  <span m="3743030">just</span> <span m="3743260">take--</span> <span m="3743950">it</span>
  <span m="3744340">takes</span> <span m="3744700">too</span> <span m="3744880">long</span>
  <span m="3745180">to</span> <span m="3745330">go</span> <span m="3745540">through</span>
  <span m="3745810">this,</span> <span m="3746080">but</span> <span m="3746250">you</span>
  <span m="3746380">get</span> <span m="3746590">the</span> <span m="3746770">idea.</span>
  <span m="3747830">So</span> <span m="3747910">what</span> <span m="3748120">this</span>
  <span m="3748360">is</span> <span m="3748510">doing</span> <span m="3749020">is</span>
  <span m="3749260">actually</span> <span m="3749770">running</span> <span m="3750190">an</span>
  <span m="3750310">algorithm</span> <span m="3750970">that</span> <span m="3751180">is</span>
  <span m="3751510">a</span> <span m="3751570">cousin</span> <span m="3752200">of</span>
  <span m="3752870">the</span> <span m="3753070">acute</span> <span m="3753370">renal</span>
  <span m="3753670">failure</span> <span m="3754120">algorithm</span> <span m="3754720">that</span>
  <span m="3754870">I</span> <span m="3754990">showed</span> <span m="3755350">you.</span>
  <span m="3756010">So</span> <span m="3756250">it's</span> <span m="3756460">trying</span>
  <span m="3756790">to</span> <span m="3757270">optimize</span> <span m="3757960">the</span>
  <span m="3758080">questions</span> <span m="3758650">that</span> <span m="3758830">it's</span>
  <span m="3759010">asking,</span> <span m="3760030">and</span> <span m="3760270">it's</span>
  <span m="3760450">trying</span> <span m="3760840">to</span> <span m="3762490">come</span>
  <span m="3762760">up</span> <span m="3762970">with</span> <span m="3763540">a</span>
  <span m="3763600">diagnostic</span> <span m="3764290">conclusion.</span></p><p><span
  m="3765400">Now,</span> <span m="3765790">in</span> <span m="3766000">order</span>
  <span m="3766300">not</span> <span m="3766570">to</span> <span m="3766720">get</span>
  <span m="3766960">in</span> <span m="3767080">trouble</span> <span m="3767470">with</span>
  <span m="3767710">things</span> <span m="3767980">like</span> <span m="3768220">the</span>
  <span m="3768370">FDA,</span> <span m="3768970">it</span> <span m="3769090">winds</span>
  <span m="3769480">up</span> <span m="3769660">wimping</span> <span m="3770140">out</span>
  <span m="3770380">at</span> <span m="3770500">the</span> <span m="3770650">end,</span>
  <span m="3771460">and</span> <span m="3771640">it</span> <span m="3771760">says,</span>
  <span m="3772330">if</span> <span m="3772480">you're</span> <span m="3772630">feeling</span>
  <span m="3772990">really</span> <span m="3773260">bad,</span> <span m="3773560">go</span>
  <span m="3773740">see</span> <span m="3773970">a</span> <span m="3774040">doctor.</span>
  <span m="3776740">But</span> <span m="3777100">nevertheless,</span> <span m="3778330">these</span>
  <span m="3778630">kinds</span> <span m="3779020">of</span> <span m="3779140">things</span>
  <span m="3779570">are</span> <span m="3780040">now</span> <span m="3780280">becoming</span>
  <span m="3780790">real,</span> <span m="3781660">and</span> <span m="3781810">they're</span>
  <span m="3781990">getting</span> <span m="3782290">better</span> <span m="3782890">because</span>
  <span m="3783310">they're</span> <span m="3783760">based</span> <span m="3784210">on</span>
  <span m="3784360">more</span> <span m="3784600">and</span> <span m="3784720">more</span>
  <span m="3784930">data.</span></p><p><span m="3786180">Yeah.</span></p><p><span
  m="3786750">AUDIENCE:</span> <span m="3786880">[INAUDIBLE]</span></p><p><span m="3789620">PETER
  SZOLOVITS:</span> <span m="3789785">Well,</span> <span m="3789950">I</span> <span
  m="3790220">can't</span> <span m="3790520">get</span> <span m="3790760">to</span>
  <span m="3790910">the</span> <span m="3791060">end,</span> <span m="3791330">because</span>
  <span m="3791570">we're</span> <span m="3791750">only</span> <span m="3792020">at</span>
  <span m="3792080">36%.</span></p><p><span m="3792720">[INTERPOSING VOICES]</span></p><p><span
  m="3795010">Yeah.</span> <span m="3795410">Here.</span> <span m="3798050">All</span>
  <span m="3798110">right.</span> <span m="3799280">Somebody--</span></p><p><span
  m="3801156">AUDIENCE:</span> <span m="3801372">Oh,</span> <span m="3801588">I think</span>
  <span m="3802020">I need</span> <span m="3802452">your finger.</span></p><p><span
  m="3802890">PETER SZOLOVITS:</span> <span m="3803075">Oh.</span> <span m="3805600">OK.</span>
  <span m="3807380">Just</span> <span m="3807620">don't</span> <span m="3807840">drain</span>
  <span m="3808130">my</span> <span m="3808310">bank</span> <span m="3808590">account.</span></p><p><span
  m="3813510">So</span> <span m="3814070"><i>The</i></span> <span m="3814280"><i>British</i></span>
  <span m="3814640"><i>Medical</i></span> <span m="3815060"><i>Journal</i></span>
  <span m="3815660">did</span> <span m="3815960">a</span> <span m="3816020">test</span>
  <span m="3817040">of</span> <span m="3817370">a</span> <span m="3817460">bunch</span>
  <span m="3817760">of</span> <span m="3817850">symptom</span> <span m="3818270">checkers,</span>
  <span m="3818615">of</span> <span m="3818960">23</span> <span m="3819500">symptom</span>
  <span m="3819950">checkers</span> <span m="3820430">like</span> <span m="3820700">this</span>
  <span m="3821630">about</span> <span m="3821930">four</span> <span m="3822200">years</span>
  <span m="3822530">ago.</span> <span m="3823170">And</span> <span m="3824300">they</span>
  <span m="3824540">said,</span> <span m="3824940">well,</span> <span m="3825630">can</span>
  <span m="3825860">it</span> <span m="3827280">on</span> <span m="3827810">45</span>
  <span m="3828420">standardized</span> <span m="3829140">patient</span> <span m="3829610">vignettes</span>
  <span m="3830690">can it</span> <span m="3831140">find</span> <span m="3831830">at</span>
  <span m="3832010">least</span> <span m="3832370">the</span> <span m="3832490">right</span>
  <span m="3832790">level</span> <span m="3833150">of</span> <span m="3833270">urgency</span>
  <span m="3833960">to</span> <span m="3834110">recommend</span> <span m="3834740">whether</span>
  <span m="3835040">you</span> <span m="3835190">should</span> <span m="3835430">go</span>
  <span m="3835580">to</span> <span m="3835670">the</span> <span m="3835820">emergency</span>
  <span m="3836420">room,</span> <span m="3837560">get</span> <span m="3838130">other</span>
  <span m="3838370">kinds</span> <span m="3838730">of</span> <span m="3838850">care,</span>
  <span m="3839270">or</span> <span m="3839480">just</span> <span m="3839690">take</span>
  <span m="3839930">care</span> <span m="3840170">of</span> <span m="3840260">yourself.</span>
  <span m="3841980">And</span> <span m="3842090">then</span> <span m="3842450">the</span>
  <span m="3842570">goals</span> <span m="3843050">were</span> <span m="3843860">that</span>
  <span m="3845000">if</span> <span m="3845210">the</span> <span m="3845330">diagnosis</span>
  <span m="3846140">is</span> <span m="3846320">given</span> <span m="3846650">by</span>
  <span m="3846860">the</span> <span m="3846950">program,</span> <span m="3847490">it</span>
  <span m="3847580">should</span> <span m="3847820">be</span> <span m="3847970">in</span>
  <span m="3848090">the</span> <span m="3848180">top</span> <span m="3848510">20</span>
  <span m="3849530">of</span> <span m="3849710">the</span> <span m="3849830">list</span>
  <span m="3850140">that</span> <span m="3850310">it</span> <span m="3850400">gives</span>
  <span m="3850760">you.</span> <span m="3851060">And</span> <span m="3851300">if</span>
  <span m="3851450">triage</span> <span m="3851990">is</span> <span m="3852140">given,</span>
  <span m="3852980">then</span> <span m="3853190">it</span> <span m="3853280">should</span>
  <span m="3853490">be</span> <span m="3853670">the</span> <span m="3853790">right</span>
  <span m="3854180">level</span> <span m="3854570">of</span> <span m="3854690">urgency.</span></p><p><span
  m="3855800">The</span> <span m="3855890">correct</span> <span m="3856250">diagnosis</span>
  <span m="3857120">was</span> <span m="3857360">first</span> <span m="3857930">in</span>
  <span m="3858110">34%</span> <span m="3859130">of</span> <span m="3859220">the</span>
  <span m="3859340">cases.</span> <span m="3860540">It</span> <span m="3860930">was</span>
  <span m="3861260">within</span> <span m="3861650">the</span> <span m="3861740">top</span>
  <span m="3862100">20</span> <span m="3862550">in</span> <span m="3862670">58%</span>
  <span m="3863720">of</span> <span m="3863810">the</span> <span m="3863930">cases.</span>
  <span m="3865160">And</span> <span m="3865400">the</span> <span m="3865490">correct</span>
  <span m="3865920">triage</span> <span m="3866540">was</span> <span m="3868010">57%</span>
  <span m="3869180">accurate.</span></p><p><span m="3870230">But</span> <span m="3870470">notice</span>
  <span m="3870830">it</span> <span m="3870920">was</span> <span m="3871130">more</span>
  <span m="3871430">accurate</span> <span m="3872000">in</span> <span m="3872180">the</span>
  <span m="3872330">emergent</span> <span m="3872840">cases,</span> <span m="3873560">which</span>
  <span m="3873830">is</span> <span m="3873980">good,</span> <span m="3874580">because</span>
  <span m="3875450">those</span> <span m="3875720">are</span> <span m="3875840">the</span>
  <span m="3875930">ones</span> <span m="3876260">where</span> <span m="3876410">you</span>
  <span m="3876530">really</span> <span m="3876800">care.</span> <span m="3878180">So</span>
  <span m="3878420">we</span> <span m="3878600">have--</span> <span m="3880430">OK.</span>
  <span m="3881480">So</span> <span m="3882020">based</span> <span m="3882410">on</span>
  <span m="3882560">what</span> <span m="3883490">he</span> <span m="3883700">said</span>
  <span m="3885080">about</span> <span m="3885470">me,</span> <span m="3886220">I</span>
  <span m="3886370">have</span> <span m="3886640">an</span> <span m="3886730">upper</span>
  <span m="3886970">respiratory</span> <span m="3887750">infection</span> <span m="3889340">with</span>
  <span m="3889670">50%</span> <span m="3890480">likelihood.</span> <span m="3891770">And</span>
  <span m="3892190">I</span> <span m="3892370">can</span> <span m="3892790">ask</span>
  <span m="3896540">what</span> <span m="3896780">to</span> <span m="3896930">do</span>
  <span m="3897170">next.</span></p><p><span m="3900050">Watch</span> <span m="3900410">for</span>
  <span m="3900560">symptoms</span> <span m="3901130">like</span> <span m="3901370">sore</span>
  <span m="3901640">throat</span> <span m="3902000">and</span> <span m="3902120">fever.</span>
  <span m="3903770">Physicians</span> <span m="3904430">often</span> <span m="3904790">perform</span>
  <span m="3905330">a</span> <span m="3905360">physical</span> <span m="3905870">exam,</span>
  <span m="3907160">explore</span> <span m="3907730">other</span> <span m="3907970">treatment</span>
  <span m="3908480">options,</span> <span m="3909650">and</span> <span m="3909920">recovery</span>
  <span m="3911000">for</span> <span m="3911240">most</span> <span m="3911540">cases</span>
  <span m="3912020">like</span> <span m="3912290">this</span> <span m="3913070">is</span>
  <span m="3913490">a</span> <span m="3913550">matter</span> <span m="3913910">of</span>
  <span m="3914030">days</span> <span m="3914330">to</span> <span m="3914430">weeks.</span>
  <span m="3916790">And</span> <span m="3916970">I</span> <span m="3917160">can</span>
  <span m="3917350">go</span> <span m="3917540">back</span> <span m="3918050">and</span>
  <span m="3918200">say,</span> <span m="3919110">I</span> <span m="3919130">might</span>
  <span m="3919400">have</span> <span m="3919610">the</span> <span m="3919730">flu,</span>
  <span m="3920780">or</span> <span m="3920990">I</span> <span m="3921110">might</span>
  <span m="3921380">have</span> <span m="3921620">allergic</span> <span m="3922100">rhinitis.</span>
  <span m="3924560">So</span> <span m="3924740">that's</span> <span m="3925010">actually</span>
  <span m="3925400">reasonable.</span> <span m="3927080">I</span> <span m="3927380">don't</span>
  <span m="3927530">know</span> <span m="3927740">exactly</span> <span m="3928250">what</span>
  <span m="3928670">you</span> <span m="3928850">put</span> <span m="3929060">in</span>
  <span m="3929210">about</span> <span m="3929540">me.</span></p><p><span m="3930425">AUDIENCE:</span>
  <span m="3930672">What</span> <span m="3930920">is</span> <span m="3931167">the</span>
  <span m="3931415">less than</span> <span m="3931910">50?</span></p><p><span m="3932405">PETER
  SZOLOVITS:</span> <span m="3932528">What</span> <span m="3932651">is</span> <span
  m="3932774">what?</span></p><p><span m="3933200">AUDIENCE:</span> <span m="3933350">The</span>
  <span m="3933500">less</span> <span m="3933996">than</span> <span m="3934492">50.</span></p><p><span
  m="3935980">[INTERPOSING VOICES]</span></p><p><span m="3937970">AUDIENCE:</span>
  <span m="3938200">Patients</span> <span m="3938430">have</span> <span m="3938760">to
  be the same</span> <span m="3939090">demographics.</span></p><p><span m="3941420">PETER
  SZOLOVITS:</span> <span m="3941540">Yeah.</span> <span m="3941660">I</span> <span
  m="3941720">don't</span> <span m="3941870">know</span> <span m="3942050">what</span>
  <span m="3942230">the</span> <span m="3942650">less</span> <span m="3942950">than</span>
  <span m="3943130">50</span> <span m="3943550">is</span> <span m="3943680">supposed</span>
  <span m="3944090">to</span> <span m="3944220">mean.</span></p><p><span m="3944430">AUDIENCE:</span>
  <span m="3944550">It</span> <span m="3944670">started</span> <span m="3944790">with</span>
  <span m="3944911">200,000</span> <span m="3945392">or</span> <span m="3945873">so.</span></p><p><span
  m="3948280">PETER SZOLOVITS:</span> <span m="3948390">Oh,</span> <span m="3948790">so</span>
  <span m="3949370">this</span> <span m="3949670">is</span> <span m="3949820">based</span>
  <span m="3950150">on</span> <span m="3950300">a</span> <span m="3950330">small</span>
  <span m="3950660">number</span> <span m="3950990">of</span> <span m="3951080">patients.</span>
  <span m="3952470">So</span> <span m="3952520">what</span> <span m="3952700">happens,</span>
  <span m="3953180">of</span> <span m="3953270">course,</span> <span m="3953630">is</span>
  <span m="3954140">as</span> <span m="3954350">you</span> <span m="3954500">slice</span>
  <span m="3954950">and</span> <span m="3955070">dice</span> <span m="3955430">a</span>
  <span m="3955520">population,</span> <span m="3956900">it</span> <span m="3957020">gets</span>
  <span m="3957260">smaller</span> <span m="3957740">and</span> <span m="3957830">smaller.</span>
  <span m="3958600">So</span> <span m="3958790">that's</span> <span m="3959330">what</span>
  <span m="3959480">we're</span> <span m="3959630">seeing.</span> <span m="3961440">OK.</span>
  <span m="3962300">Thank</span> <span m="3962510">you.</span></p><p><span m="3963740">OK.</span>
  <span m="3965780">So</span> <span m="3966200">two</span> <span m="3966380">more</span>
  <span m="3966590">topics</span> <span m="3967190">I'm</span> <span m="3967330">going
  to</span> <span m="3967800">rush</span> <span m="3968270">through.</span> <span
  m="3969890">One</span> <span m="3970190">is</span> <span m="3971150">that--</span>
  <span m="3975020">as</span> <span m="3975200">I</span> <span m="3975320">mentioned</span>
  <span m="3975750">in</span> <span m="3975890">one</span> <span m="3976070">of</span>
  <span m="3976450">the</span> <span m="3976730">much</span> <span m="3977030">earlier</span>
  <span m="3977390">slides,</span> <span m="3978530">every</span> <span m="3978830">action</span>
  <span m="3979220">has</span> <span m="3979490">a</span> <span m="3979520">cost.</span>
  <span m="3981550">It</span> <span m="3981710">at</span> <span m="3981830">least</span>
  <span m="3982130">takes</span> <span m="3982490">time.</span> <span m="3983580">And</span>
  <span m="3983660">sometimes</span> <span m="3984280">it</span> <span m="3984950">induces</span>
  <span m="3985790">potentially</span> <span m="3986480">bad</span> <span m="3986780">things</span>
  <span m="3987230">to</span> <span m="3987350">happen</span> <span m="3988160">to</span>
  <span m="3988370">a</span> <span m="3988430">patient.</span></p><p><span m="3989730">And</span>
  <span m="3989810">so</span> <span m="3990080">people</span> <span m="3990560">began</span>
  <span m="3991070">studying</span> <span m="3992120">a</span> <span m="3992390">long</span>
  <span m="3992690">time</span> <span m="3992990">ago</span> <span m="3994070">what</span>
  <span m="3994310">does</span> <span m="3994490">it</span> <span m="3994610">mean</span>
  <span m="3994880">to</span> <span m="3995030">be</span> <span m="3995180">rational</span>
  <span m="3995750">under</span> <span m="3995990">resource</span> <span m="3996530">constraints</span>
  <span m="3997280">rather</span> <span m="3997730">than</span> <span m="3997970">rational</span>
  <span m="3998960">just</span> <span m="3999270">in</span> <span m="3999410">this</span>
  <span m="3999620">Home</span> <span m="3999990">economicus</span> <span m="4000760">model.</span></p><p><span
  m="4001720">And</span> <span m="4001870">so</span> <span m="4002140">Eric</span>
  <span m="4002470">Horvitz,</span> <span m="4003070">who's</span> <span m="4003280">now</span>
  <span m="4004090">a</span> <span m="4004570">big</span> <span m="4004810">cheese</span>
  <span m="4005170">guy,</span> <span m="4006290">he's</span> <span m="4006640">head</span>
  <span m="4006820">of</span> <span m="4007360">Microsoft</span> <span m="4008140">Research,</span>
  <span m="4009790">but</span> <span m="4010300">used</span> <span m="4010600">to</span>
  <span m="4010720">be</span> <span m="4011170">just</span> <span m="4011560">a</span>
  <span m="4011950">lowly</span> <span m="4012430">graduate</span> <span m="4012940">student</span>
  <span m="4013330">at</span> <span m="4013450">Stanford</span> <span m="4014100">when</span>
  <span m="4015970">he</span> <span m="4016060">started</span> <span m="4016420">doing</span>
  <span m="4016690">this</span> <span m="4016870">work.</span> <span m="4018806">He</span>
  <span m="4019150">said,</span> <span m="4019420">well,</span> <span m="4020080">utility</span>
  <span m="4020770">comes</span> <span m="4021190">not</span> <span m="4021430">only</span>
  <span m="4021730">from</span> <span m="4021970">what</span> <span m="4022150">happens</span>
  <span m="4022600">to</span> <span m="4022720">the</span> <span m="4022840">patient,</span>
  <span m="4023410">but</span> <span m="4023620">also</span> <span m="4024040">from</span>
  <span m="4024430">the</span> <span m="4024550">reasoning</span> <span m="4024970">process</span>
  <span m="4025990">from</span> <span m="4026230">the</span> <span m="4026320">computational</span>
  <span m="4027160">process</span> <span m="4027700">itself.</span></p><p><span m="4028750">And</span>
  <span m="4028900">so</span> <span m="4029110">consider--</span> <span m="4029770">do</span>
  <span m="4030130">you</span> <span m="4030400">guys</span> <span m="4030640">watch</span>
  <span m="4030970"><i>MacGyver?</i></span> <span m="4032030">This</span> <span m="4032320">is</span>
  <span m="4032980">way</span> <span m="4033250">out</span> <span m="4033430">of</span>
  <span m="4033550">date.</span> <span m="4034630">So</span> <span m="4035890">if</span>
  <span m="4036520">MacGyver</span> <span m="4037090">is</span> <span m="4037240">defusing</span>
  <span m="4037930">some</span> <span m="4038230">bomb</span> <span m="4038590">that's</span>
  <span m="4038890">ticking</span> <span m="4039310">down</span> <span m="4039640">to</span>
  <span m="4039850">zero</span> <span m="4041290">and</span> <span m="4041590">he</span>
  <span m="4041740">runs</span> <span m="4042100">out</span> <span m="4042250">of</span>
  <span m="4042370">time,</span> <span m="4042970">then</span> <span m="4043480">his</span>
  <span m="4044200">utilities</span> <span m="4044890">take</span> <span m="4045160">a</span>
  <span m="4045220">very</span> <span m="4045490">sharp</span> <span m="4045880">drop</span>
  <span m="4046810">at</span> <span m="4047050">that</span> <span m="4047290">point.</span>
  <span m="4048290">So</span> <span m="4048760">that's</span> <span m="4049180">what</span>
  <span m="4049870">this</span> <span m="4050350">work</span> <span m="4050740">is</span>
  <span m="4050920">really</span> <span m="4051250">about,</span> <span m="4052150">saying,</span>
  <span m="4052600">well,</span> <span m="4053650">what</span> <span m="4053920">can</span>
  <span m="4054160">we</span> <span m="4054310">do</span> <span m="4054820">when</span>
  <span m="4055090">we</span> <span m="4055270">don't</span> <span m="4055570">have</span>
  <span m="4055840">all</span> <span m="4055990">the</span> <span m="4056110">time</span>
  <span m="4056410">in</span> <span m="4056530">the</span> <span m="4056590">world</span>
  <span m="4056860">to</span> <span m="4057040">do</span> <span m="4057220">the</span>
  <span m="4057340">computation</span> <span m="4058690">as</span> <span m="4058930">well</span>
  <span m="4059230">as</span> <span m="4060070">having</span> <span m="4060570">to</span>
  <span m="4060880">try</span> <span m="4061120">to</span> <span m="4061210">maximize</span>
  <span m="4061930">utility</span> <span m="4062440">to</span> <span m="4062620">the</span>
  <span m="4062710">patient?</span></p><p><span m="4064000">And</span> <span m="4064180">Daniel</span>
  <span m="4064540">Kahneman,</span> <span m="4065110">who</span> <span m="4065230">won</span>
  <span m="4065440">the</span> <span m="4065530">Nobel</span> <span m="4065890">Prize</span>
  <span m="4066280">a</span> <span m="4066340">few</span> <span m="4066610">years</span>
  <span m="4066910">ago</span> <span m="4067150">in</span> <span m="4067240">economics</span>
  <span m="4068440">for</span> <span m="4068740">this</span> <span m="4069010">notion</span>
  <span m="4069400">of</span> <span m="4069520">bounded</span> <span m="4069940">rationality</span>
  <span m="4072230">that</span> <span m="4072490">says</span> <span m="4072820">that</span>
  <span m="4073210">the</span> <span m="4074350">way</span> <span m="4074650">we</span>
  <span m="4074830">would</span> <span m="4075010">like</span> <span m="4075310">to</span>
  <span m="4075460">be</span> <span m="4075640">rational</span> <span m="4076270">is</span>
  <span m="4076480">not</span> <span m="4076750">actually</span> <span m="4077230">the</span>
  <span m="4077350">way</span> <span m="4077560">we</span> <span m="4077740">behave,</span>
  <span m="4078790">and</span> <span m="4079000">he</span> <span m="4079150">wrote</span>
  <span m="4079420">this</span> <span m="4079690">popular</span> <span m="4080260">book</span>
  <span m="4080820">that</span> <span m="4081160">I</span> <span m="4081250">really</span>
  <span m="4081550">like</span> <span m="4081850">called</span> <span m="4082210"><i>Thinking,</i></span>
  <span m="4082660"><i>Fast</i></span> <span m="4083290"><i>and</i></span> <span m="4083440"><i>Slow</i></span>
  <span m="4084760">that</span> <span m="4085000">says</span> <span m="4085390">that</span>
  <span m="4087010">if</span> <span m="4087220">you're</span> <span m="4087370">trying</span>
  <span m="4087700">to</span> <span m="4087850">figure</span> <span m="4088240">out</span>
  <span m="4088450">which</span> <span m="4088720">house</span> <span m="4089050">to</span>
  <span m="4089170">buy,</span> <span m="4090040">you</span> <span m="4090220">have</span>
  <span m="4090400">a</span> <span m="4090430">lot</span> <span m="4090670">of</span>
  <span m="4090760">time</span> <span m="4091060">to</span> <span m="4091210">do</span>
  <span m="4091450">it,</span> <span m="4092350">so</span> <span m="4092560">you</span>
  <span m="4092710">can</span> <span m="4092920">deliberate</span> <span m="4093730">and</span>
  <span m="4093880">list</span> <span m="4094240">all</span> <span m="4094390">the</span>
  <span m="4094540">advantages</span> <span m="4095320">and</span> <span m="4095440">disadvantages</span>
  <span m="4096520">and</span> <span m="4096670">costs</span> <span m="4097300">and</span>
  <span m="4097420">so</span> <span m="4097689">on</span> <span m="4097870">of</span>
  <span m="4098410">different</span> <span m="4098770">houses</span> <span m="4099399">and</span>
  <span m="4099520">take</span> <span m="4099819">your</span> <span m="4099970">time</span>
  <span m="4100300">making</span> <span m="4100660">a</span> <span m="4100720">decision.</span>
  <span m="4102700">If</span> <span m="4102910">you</span> <span m="4103060">see</span>
  <span m="4103630">a</span> <span m="4103930">car</span> <span m="4104319">barreling</span>
  <span m="4104890">toward</span> <span m="4105370">you</span> <span m="4105550">as</span>
  <span m="4105819">you</span> <span m="4105880">are</span> <span m="4106330">crossing</span>
  <span m="4106870">in</span> <span m="4106960">a</span> <span m="4107020">crosswalk,</span>
  <span m="4108520">you</span> <span m="4108700">don't</span> <span m="4108939">stop</span>
  <span m="4109420">and</span> <span m="4109540">say,</span> <span m="4109840">well,</span>
  <span m="4110120">let</span> <span m="4110229">me</span> <span m="4110380">figure</span>
  <span m="4110740">out</span> <span m="4110979">the</span> <span m="4111130">pluses</span>
  <span m="4111670">and</span> <span m="4111760">minuses</span> <span m="4112840">of</span>
  <span m="4113020">moving</span> <span m="4113439">to</span> <span m="4113590">the</span>
  <span m="4113710">left</span> <span m="4114200">or</span> <span m="4114399">moving</span>
  <span m="4114819">to</span> <span m="4114970">the</span> <span m="4116229">right,</span>
  <span m="4116890">because</span> <span m="4117370">by</span> <span m="4117550">the</span>
  <span m="4117700">time</span> <span m="4117970">you</span> <span m="4118090">figure</span>
  <span m="4118450">it</span> <span m="4118569">out,</span> <span m="4119410">you're</span>
  <span m="4119620">dead.</span></p><p><span m="4120580">And</span> <span m="4120790">so</span>
  <span m="4122319">he</span> <span m="4122890">claims</span> <span m="4123910">that</span>
  <span m="4124210">human</span> <span m="4124569">beings</span> <span m="4124960">have</span>
  <span m="4125200">evolved</span> <span m="4125890">in</span> <span m="4126100">a</span>
  <span m="4126160">way</span> <span m="4126939">where</span> <span m="4127120">we</span>
  <span m="4127300">have</span> <span m="4127569">a</span> <span m="4127630">kind</span>
  <span m="4127930">of</span> <span m="4128050">instinctual</span> <span m="4129370">very</span>
  <span m="4129670">fast</span> <span m="4130120">response,</span> <span m="4131890">and</span>
  <span m="4132189">that</span> <span m="4132939">the</span> <span m="4133120">deliberative</span>
  <span m="4133930">process</span> <span m="4135130">is</span> <span m="4135370">only</span>
  <span m="4135729">invoked</span> <span m="4136240">relatively</span> <span m="4136899">rarely.</span>
  <span m="4137890">Now,</span> <span m="4138100">he</span> <span m="4138279">bemoans</span>
  <span m="4138880">this</span> <span m="4139149">fact,</span> <span m="4139600">because</span>
  <span m="4140020">he</span> <span m="4140229">claims</span> <span m="4140800">that</span>
  <span m="4141370">people</span> <span m="4141729">make</span> <span m="4142029">too</span>
  <span m="4142240">many</span> <span m="4142510">decisions</span> <span m="4143260">that</span>
  <span m="4143470">they</span> <span m="4143649">ought</span> <span m="4143890">to</span>
  <span m="4144069">be</span> <span m="4144250">deliberative</span> <span m="4144970">about</span>
  <span m="4145840">based</span> <span m="4146260">on</span> <span m="4146410">these</span>
  <span m="4146560">sort</span> <span m="4146859">of</span> <span m="4146979">gut</span>
  <span m="4147220">instincts.</span> <span m="4148420">For</span> <span m="4148630">example,</span>
  <span m="4149240">our</span> <span m="4149290">current</span> <span m="4149620">president.</span>
  <span m="4151720">But</span> <span m="4153670">never</span> <span m="4154029">mind.</span></p><p><span
  m="4155859">So</span> <span m="4156700">what</span> <span m="4158290">Eric</span>
  <span m="4158590">and</span> <span m="4158680">his</span> <span m="4158859">colleagues</span>
  <span m="4159370">were</span> <span m="4159880">doing</span> <span m="4160240">was</span>
  <span m="4161020">trying</span> <span m="4161529">really</span> <span m="4161890">to</span>
  <span m="4162069">look</span> <span m="4162430">at</span> <span m="4163660">how</span>
  <span m="4164050">this</span> <span m="4164319">kind</span> <span m="4164590">of
  meta</span> <span m="4164710">level</span> <span m="4165399">reasoning</span> <span
  m="4166090">about</span> <span m="4166779">how</span> <span m="4166990">much</span>
  <span m="4167350">reasoning</span> <span m="4168010">and</span> <span m="4168130">what</span>
  <span m="4168370">kind</span> <span m="4168729">of</span> <span m="4168850">reasoning</span>
  <span m="4169450">is</span> <span m="4169660">worth</span> <span m="4169960">doing</span>
  <span m="4171189">plays</span> <span m="4171700">into</span> <span m="4172090">the</span>
  <span m="4172240">decision</span> <span m="4172750">making</span> <span m="4173109">process.</span>
  <span m="4174319">So</span> <span m="4174430">the</span> <span m="4174580">expected</span>
  <span m="4175090">value</span> <span m="4175450">of</span> <span m="4175569">computation</span>
  <span m="4176260">as</span> <span m="4176410">a</span> <span m="4176470">fundamental</span>
  <span m="4177040">component</span> <span m="4177609">of</span> <span m="4177760">reflection</span>
  <span m="4178930">about</span> <span m="4179229">alternative</span> <span m="4179890">inference</span>
  <span m="4180250">strategies.</span></p><p><span m="4181580">So</span> <span m="4181689">for</span>
  <span m="4181870">example,</span> <span m="4183040">I</span> <span m="4183370">mentioned</span>
  <span m="4183850">that</span> <span m="4184029">QMR</span> <span m="4184720">had</span>
  <span m="4184960">these</span> <span m="4185200">alternative</span> <span m="4185890">questioning</span>
  <span m="4186520">methods</span> <span m="4187600">depending</span> <span m="4188229">on</span>
  <span m="4188979">the</span> <span m="4189279">length</span> <span m="4189670">of</span>
  <span m="4189819">the</span> <span m="4189970">differential</span> <span m="4190689">that</span>
  <span m="4190899">it</span> <span m="4191020">was</span> <span m="4191229">working</span>
  <span m="4191680">on.</span> <span m="4192350">So</span> <span m="4192430">that's</span>
  <span m="4192729">an</span> <span m="4192850">example</span> <span m="4193600">of</span>
  <span m="4193779">a</span> <span m="4193840">kind</span> <span m="4194109">of</span>
  <span m="4194260">meta</span> <span m="4194800">level</span> <span m="4195160">reasoning</span>
  <span m="4195700">that</span> <span m="4195910">says</span> <span m="4197200">that</span>
  <span m="4197560">it</span> <span m="4197740">may</span> <span m="4197950">be</span>
  <span m="4198100">more</span> <span m="4198400">effective</span> <span m="4198970">to</span>
  <span m="4199120">do</span> <span m="4199330">one</span> <span m="4199570">kind</span>
  <span m="4199870">of</span> <span m="4199990">question</span> <span m="4200950">asking</span>
  <span m="4201370">strategy</span> <span m="4202240">than</span> <span m="4202510">another.</span>
  <span m="4203620">The</span> <span m="4203800">degree</span> <span m="4204190">of</span>
  <span m="4204340">refinement,</span> <span m="4205000">people</span> <span m="4205390">talk</span>
  <span m="4205690">about</span> <span m="4206020">things</span> <span m="4206290">like</span>
  <span m="4206500">just-in-time</span> <span m="4207280">algorithms,</span> <span
  m="4208510">where</span> <span m="4209530">if</span> <span m="4209740">you</span>
  <span m="4209890">run</span> <span m="4210130">out</span> <span m="4210340">of</span>
  <span m="4210460">time</span> <span m="4210850">to</span> <span m="4211060">think</span>
  <span m="4211540">more</span> <span m="4211820">deliberately,</span> <span m="4213160">you</span>
  <span m="4213310">can</span> <span m="4213520">just</span> <span m="4213790">take</span>
  <span m="4214060">the</span> <span m="4214360">best</span> <span m="4214750">answer</span>
  <span m="4215140">that's</span> <span m="4215410">available</span> <span m="4215980">to</span>
  <span m="4216140">you</span> <span m="4216250">now.</span></p><p><span m="4217360">And</span>
  <span m="4217510">so</span> <span m="4218680">taking</span> <span m="4219160">the</span>
  <span m="4219280">value</span> <span m="4219700">of</span> <span m="4219820">information,</span>
  <span m="4220540">the</span> <span m="4220630">value</span> <span m="4221050">of</span>
  <span m="4221170">computation,</span> <span m="4222460">and</span> <span m="4222610">the</span>
  <span m="4222700">value</span> <span m="4223120">of</span> <span m="4223240">experimentation</span>
  <span m="4224290">into</span> <span m="4224590">account</span> <span m="4225490">in</span>
  <span m="4225700">doing</span> <span m="4226090">this</span> <span m="4226330">meta</span>
  <span m="4226600">level</span> <span m="4226900">reasoning</span> <span m="4227860">is</span>
  <span m="4228070">important</span> <span m="4228610">to</span> <span m="4228760">come</span>
  <span m="4229030">up</span> <span m="4229180">with</span> <span m="4229390">the</span>
  <span m="4229480">most</span> <span m="4229780">effective</span> <span m="4230200">strategies.</span>
  <span m="4231940">So</span> <span m="4233050">he</span> <span m="4233950">gives</span>
  <span m="4234220">an</span> <span m="4234340">example</span> <span m="4235150">of</span>
  <span m="4235570">a</span> <span m="4235750">time</span> <span m="4236050">pressure</span>
  <span m="4236470">decision</span> <span m="4237010">problem</span> <span m="4238030">where</span>
  <span m="4239350">you</span> <span m="4239590">have</span> <span m="4240400">a</span>
  <span m="4240460">patient,</span> <span m="4241090">a</span> <span m="4241460">75-year-old</span>
  <span m="4242530">woman</span> <span m="4242890">in</span> <span m="4243010">the</span>
  <span m="4243130">ICU,</span> <span m="4244270">and</span> <span m="4244480">she</span>
  <span m="4244690">develops</span> <span m="4245170">sudden</span> <span m="4245560">breathing</span>
  <span m="4245980">difficulties.</span> <span m="4247870">So</span> <span m="4248020">what</span>
  <span m="4248170">do</span> <span m="4248230">you</span> <span m="4248350">do?</span></p><p><span
  m="4252820">Well,</span> <span m="4253600">it's</span> <span m="4253810">a</span>
  <span m="4253840">challenge,</span> <span m="4254560">right?</span> <span m="4255370">You</span>
  <span m="4255550">could</span> <span m="4255850">be</span> <span m="4256060">very</span>
  <span m="4256390">deliberative,</span> <span m="4257320">but</span> <span m="4257590">the</span>
  <span m="4257680">problem</span> <span m="4258160">is</span> <span m="4258370">that</span>
  <span m="4258850">she</span> <span m="4259180">may</span> <span m="4259390">die</span>
  <span m="4259810">because</span> <span m="4260170">she's</span> <span m="4260500">not</span>
  <span m="4260710">breathing</span> <span m="4261130">well,</span> <span m="4262510">or</span>
  <span m="4262840">you</span> <span m="4262990">could</span> <span m="4263230">impulsively</span>
  <span m="4264070">say,</span> <span m="4264400">well,</span> <span m="4264610">let's</span>
  <span m="4264820">put</span> <span m="4265030">her</span> <span m="4265150">on</span>
  <span m="4265300">a</span> <span m="4265330">mechanical</span> <span m="4265990">ventilator,</span>
  <span m="4266620">because</span> <span m="4267490">we</span> <span m="4267640">know</span>
  <span m="4267880">that</span> <span m="4268090">that</span> <span m="4268260">will</span>
  <span m="4268570">prevent</span> <span m="4268990">her</span> <span m="4269170">from</span>
  <span m="4269440">dying</span> <span m="4269800">in</span> <span m="4269890">the</span>
  <span m="4269980">short</span> <span m="4270280">term,</span> <span m="4271150">but</span>
  <span m="4271360">that</span> <span m="4271570">may</span> <span m="4271750">be</span>
  <span m="4271900">the</span> <span m="4272020">wrong</span> <span m="4272320">decision,</span>
  <span m="4272920">because</span> <span m="4273520">that</span> <span m="4273760">has</span>
  <span m="4274060">bad</span> <span m="4274330">side</span> <span m="4274630">effects.</span>
  <span m="4276370">She</span> <span m="4276580">may</span> <span m="4276760">get</span>
  <span m="4276940">an</span> <span m="4277090">infection,</span> <span m="4277750">get</span>
  <span m="4278020">pneumonia,</span> <span m="4278590">and</span> <span m="4278740">die</span>
  <span m="4278980">that</span> <span m="4279250">way.</span> <span m="4280210">And</span>
  <span m="4280420">you</span> <span m="4280570">certainly</span> <span m="4281020">don't</span>
  <span m="4281350">want</span> <span m="4281590">to</span> <span m="4281650">subject</span>
  <span m="4281995">her</span> <span m="4282340">to</span> <span m="4282520">that</span>
  <span m="4282790">risk</span> <span m="4283210">if</span> <span m="4283720">she</span>
  <span m="4283870">didn't</span> <span m="4284110">need</span> <span m="4284350">to</span>
  <span m="4284500">take</span> <span m="4284770">that</span> <span m="4285010">risk.</span></p><p><span
  m="4286990">So</span> <span m="4288040">they</span> <span m="4288280">designed</span>
  <span m="4288970">an</span> <span m="4290050">architecture</span> <span m="4291370">that</span>
  <span m="4291640">says,</span> <span m="4292030">well,</span> <span m="4292330">this</span>
  <span m="4292630">is</span> <span m="4292810">the</span> <span m="4292960">decision</span>
  <span m="4293530">that</span> <span m="4293770">you're</span> <span m="4293890">trying</span>
  <span m="4294220">to</span> <span m="4294370">make,</span> <span m="4295150">which</span>
  <span m="4295420">they're</span> <span m="4295630">modeling</span> <span m="4296200">by</span>
  <span m="4296410">an</span> <span m="4296530">influence</span> <span m="4297070">diagram.</span>
  <span m="4297700">So</span> <span m="4297940">this</span> <span m="4298180">is</span>
  <span m="4298780">a</span> <span m="4298840">Bayesian</span> <span m="4299350">network</span>
  <span m="4299920">with</span> <span m="4300220">the</span> <span m="4300370">addition</span>
  <span m="4301360">of</span> <span m="4301570">decision</span> <span m="4302110">nodes</span>
  <span m="4302650">and</span> <span m="4302860">value</span> <span m="4303280">nodes.</span>
  <span m="4304060">But you</span> <span m="4304460">use</span> <span m="4305290">Bayesian</span>
  <span m="4305950">network</span> <span m="4306190">techniques</span> <span m="4307240">to</span>
  <span m="4307390">calculate</span> <span m="4308110">optimal</span> <span m="4308620">decisions</span>
  <span m="4309280">here.</span> <span m="4310150">And</span> <span m="4310300">then</span>
  <span m="4310540">this</span> <span m="4310840">is</span> <span m="4310990">kind</span>
  <span m="4311290">of</span> <span m="4311410">the</span> <span m="4311530">background</span>
  <span m="4312160">knowledge</span> <span m="4312910">of</span> <span m="4313240">what</span>
  <span m="4313450">we</span> <span m="4313660">understand</span> <span m="4314800">about</span>
  <span m="4315160">the</span> <span m="4315280">relationships</span> <span m="4316180">among</span>
  <span m="4316450">different</span> <span m="4316840">things</span> <span m="4317260">in</span>
  <span m="4317410">the</span> <span m="4317530">intensive</span> <span m="4318040">care</span>
  <span m="4318310">unit.</span> <span m="4319270">And</span> <span m="4319480">this</span>
  <span m="4319840">is</span> <span m="4320020">a</span> <span m="4320110">representation</span>
  <span m="4321310">of</span> <span m="4321580">the</span> <span m="4321970">meta</span>
  <span m="4322300">reasoning</span> <span m="4323470">that</span> <span m="4323710">says,</span>
  <span m="4325030">which</span> <span m="4325360">utility</span> <span m="4325900">model</span>
  <span m="4326290">should</span> <span m="4326530">we</span> <span m="4326680">use?</span>
  <span m="4327590">Which</span> <span m="4327730">reasoning</span> <span m="4328210">technique</span>
  <span m="4328740">should</span> <span m="4328960">we</span> <span m="4329110">use?</span>
  <span m="4329560">And</span> <span m="4329680">so</span> <span m="4329920">on.</span>
  <span m="4330670">And</span> <span m="4330820">they</span> <span m="4330970">built</span>
  <span m="4331330">an</span> <span m="4331450">architecture</span> <span m="4332200">that</span>
  <span m="4332440">integrates</span> <span m="4333370">these</span> <span m="4333670">various</span>
  <span m="4334180">approaches.</span></p><p><span m="4337180">And</span> <span m="4337330">then</span>
  <span m="4337540">in</span> <span m="4337720">my</span> <span m="4337930">last</span>
  <span m="4338260">2</span> <span m="4338500">minutes,</span> <span m="4340030">I</span>
  <span m="4340150">just</span> <span m="4340420">want</span> <span m="4340600">to</span>
  <span m="4340660">tell</span> <span m="4340960">you</span> <span m="4341740">about</span>
  <span m="4342850">an</span> <span m="4342970">interesting--</span> <span m="4344170">this</span>
  <span m="4344470">is</span> <span m="4344650">a</span> <span m="4344710">modern</span>
  <span m="4345130">view,</span> <span m="4345400">not</span> <span m="4345640">historical.</span>
  <span m="4346720">So</span> <span m="4346930">this</span> <span m="4347170">was</span>
  <span m="4347380">a</span> <span m="4347440">paper</span> <span m="4347830">presented</span>
  <span m="4348580">at</span> <span m="4348850">the</span> <span m="4348970">last</span>
  <span m="4349350">NeurIPS</span> <span m="4349840">meeting,</span> <span m="4351610">which</span>
  <span m="4351910">said</span> <span m="4353440">the</span> <span m="4354130">kinds</span>
  <span m="4354520">of</span> <span m="4354640">problems</span> <span m="4355330">that</span>
  <span m="4355540">we've</span> <span m="4355780">been</span> <span m="4355930">talking</span>
  <span m="4356410">about,</span> <span m="4356890">like</span> <span m="4357310">the</span>
  <span m="4357520">acute</span> <span m="4357880">renal</span> <span m="4358150">failure</span>
  <span m="4358570">problem</span> <span m="4359170">or</span> <span m="4359410">like</span>
  <span m="4359860">any</span> <span m="4360100">of</span> <span m="4360220">these</span>
  <span m="4360490">others,</span> <span m="4362080">we</span> <span m="4362290">can</span>
  <span m="4362500">reformulate</span> <span m="4363400">this</span> <span m="4364390">as</span>
  <span m="4364900">a</span> <span m="4365350">reinforcement</span> <span m="4366220">learning</span>
  <span m="4366550">problem.</span></p><p><span m="4368690">So</span> <span m="4368800">the</span>
  <span m="4368980">idea</span> <span m="4369430">is</span> <span m="4370330">that</span>
  <span m="4372460">if</span> <span m="4372700">you</span> <span m="4372850">treat</span>
  <span m="4374350">all</span> <span m="4374620">activities,</span> <span m="4375980">including</span>
  <span m="4377140">putting</span> <span m="4377500">somebody</span> <span m="4377980">on</span>
  <span m="4378130">a</span> <span m="4378160">ventilator</span> <span m="4379360">or</span>
  <span m="4379660">concluding</span> <span m="4380380">a</span> <span m="4380440">diagnostic</span>
  <span m="4381160">conclusion</span> <span m="4382420">or</span> <span m="4382630">asking</span>
  <span m="4383130">a</span> <span m="4383200">question</span> <span m="4384070">or</span>
  <span m="4384820">any</span> <span m="4385060">of</span> <span m="4385150">the</span>
  <span m="4385330">other</span> <span m="4385540">things</span> <span m="4385900">that</span>
  <span m="4386110">we've</span> <span m="4386320">contemplated,</span> <span m="4387520">if</span>
  <span m="4387700">you</span> <span m="4387850">treat</span> <span m="4388210">those</span>
  <span m="4388690">all</span> <span m="4388960">in</span> <span m="4389080">a</span>
  <span m="4389170">uniform</span> <span m="4389710">way</span> <span m="4390070">and</span>
  <span m="4390580">say</span> <span m="4390880">these</span> <span m="4391150">are</span>
  <span m="4391300">actions,</span> <span m="4394120">we</span> <span m="4394300">then</span>
  <span m="4394540">model</span> <span m="4395320">the</span> <span m="4395500">universe</span>
  <span m="4396280">as</span> <span m="4396510">a</span> <span m="4396570">Markov</span>
  <span m="4397030">decision</span> <span m="4397510">process,</span> <span m="4399310">where</span>
  <span m="4400180">every</span> <span m="4400480">time</span> <span m="4400870">that</span>
  <span m="4401110">you</span> <span m="4401230">take</span> <span m="4401590">one</span>
  <span m="4401800">of</span> <span m="4401920">these</span> <span m="4402190">actions,</span>
  <span m="4402770">it</span> <span m="4403360">changes</span> <span m="4404080">the</span>
  <span m="4404230">state</span> <span m="4405190">of</span> <span m="4405400">the</span>
  <span m="4405520">patient,</span> <span m="4406360">or</span> <span m="4406510">the</span>
  <span m="4406630">state</span> <span m="4406930">of</span> <span m="4407050">our</span>
  <span m="4407200">knowledge</span> <span m="4407920">about</span> <span m="4408250">the</span>
  <span m="4408400">patient.</span> <span m="4410110">And</span> <span m="4410260">then</span>
  <span m="4410470">you</span> <span m="4410620">do</span> <span m="4410830">reinforcement</span>
  <span m="4411730">learning</span> <span m="4412180">to</span> <span m="4412360">figure</span>
  <span m="4412780">out</span> <span m="4413020">what</span> <span m="4413230">is</span>
  <span m="4413350">the</span> <span m="4413500">optimal</span> <span m="4414010">policy</span>
  <span m="4415120">to</span> <span m="4415360">apply</span> <span m="4416020">under</span>
  <span m="4416410">all</span> <span m="4416620">possible</span> <span m="4417220">states</span>
  <span m="4418360">in</span> <span m="4418540">order</span> <span m="4418840">to</span>
  <span m="4419320">maximize</span> <span m="4420070">the</span> <span m="4420220">expected</span>
  <span m="4420790">outcome.</span></p><p><span m="4422750">So</span> <span m="4422830">that's</span>
  <span m="4423100">exactly</span> <span m="4423670">the</span> <span m="4423850">approach</span>
  <span m="4424300">that</span> <span m="4424510">they're</span> <span m="4424690">taking.</span>
  <span m="4427360">The</span> <span m="4427480">state</span> <span m="4427870">space</span>
  <span m="4428200">is</span> <span m="4428500">the</span> <span m="4428620">set</span>
  <span m="4428890">of</span> <span m="4429010">positive</span> <span m="4429580">and</span>
  <span m="4429700">negative</span> <span m="4430090">findings.</span> <span m="4430810">The</span>
  <span m="4430960">action</span> <span m="4431410">space</span> <span m="4432340">is</span>
  <span m="4432550">to</span> <span m="4432670">ask</span> <span m="4433000">about</span>
  <span m="4433270">a</span> <span m="4433330">finding</span> <span m="4433900">or</span>
  <span m="4434080">conclude</span> <span m="4434570">a</span> <span m="4434620">diagnosis.</span>
  <span m="4436000">The</span> <span m="4436120">reward</span> <span m="4436870">is</span>
  <span m="4437140">the</span> <span m="4437320">correct</span> <span m="4437860">or</span>
  <span m="4438010">incorrect</span> <span m="4438580">single</span> <span m="4438970">diagnosis.</span></p><p><span
  m="4440140">So</span> <span m="4440320">once</span> <span m="4440590">you</span>
  <span m="4440680">reach</span> <span m="4441010">a</span> <span m="4441040">diagnosis,</span>
  <span m="4441850">the</span> <span m="4441970">process</span> <span m="4442420">stops,</span>
  <span m="4443170">and</span> <span m="4443290">you</span> <span m="4443440">get</span>
  <span m="4443630">your</span> <span m="4443770">reward.</span> <span m="4445170">It's</span>
  <span m="4445480">finite</span> <span m="4445960">horizon</span> <span m="4446590">because</span>
  <span m="4446950">they</span> <span m="4447130">impose</span> <span m="4447610">a</span>
  <span m="4447670">limit</span> <span m="4448150">on</span> <span m="4448330">the</span>
  <span m="4448390">number</span> <span m="4448750">of</span> <span m="4448870">questions.</span>
  <span m="4449920">If</span> <span m="4450100">you</span> <span m="4450220">don't</span>
  <span m="4450460">get</span> <span m="4450640">an</span> <span m="4450790">answer</span>
  <span m="4451180">by</span> <span m="4451420">then,</span> <span m="4452140">you</span>
  <span m="4452560">lose.</span> <span m="4453070">You</span> <span m="4453190">get</span>
  <span m="4453370">a</span> <span m="4453430">minus one</span> <span m="4453880">reward.</span></p><p><span
  m="4455650">There</span> <span m="4455880">is</span> <span m="4456070">a</span>
  <span m="4456130">discount</span> <span m="4456670">factor</span> <span m="4457720">so</span>
  <span m="4457990">that</span> <span m="4459910">the</span> <span m="4460120">further</span>
  <span m="4460720">away</span> <span m="4461170">a</span> <span m="4461230">reward</span>
  <span m="4461830">is,</span> <span m="4462160">the</span> <span m="4462310">less</span>
  <span m="4462610">value</span> <span m="4463090">it</span> <span m="4463210">has</span>
  <span m="4463540">to</span> <span m="4463660">you</span> <span m="4464380">at</span>
  <span m="4464560">any</span> <span m="4464740">point,</span> <span m="4465580">which</span>
  <span m="4465940">encourages</span> <span m="4466690">shorter</span> <span m="4467200">question</span>
  <span m="4467620">sequences.</span> <span m="4469000">And</span> <span m="4469180">they</span>
  <span m="4469330">use</span> <span m="4469630">a</span> <span m="4469690">pretty</span>
  <span m="4469990">standard</span> <span m="4470245">Q</span> <span m="4470500">learning</span>
  <span m="4471160">framework,</span> <span m="4472000">or</span> <span m="4472120">at</span>
  <span m="4472240">least</span> <span m="4472540">a</span> <span m="4472600">modern</span>
  <span m="4473020">Q</span> <span m="4473260">learning</span> <span m="4473890">framework</span>
  <span m="4474970">using</span> <span m="4475450">a</span> <span m="4475510">double</span>
  <span m="4475870">deep</span> <span m="4476530">neural</span> <span m="4476860">network</span>
  <span m="4477340">strategy.</span></p><p><span m="4478840">And</span> <span m="4478990">then</span>
  <span m="4479350">there</span> <span m="4479530">are</span> <span m="4479620">two</span>
  <span m="4479890">pieces</span> <span m="4480400">of</span> <span m="4480520">magic</span>
  <span m="4480970">sauce</span> <span m="4481750">that</span> <span m="4482050">make</span>
  <span m="4482320">this</span> <span m="4482560">work</span> <span m="4482860">better.</span>
  <span m="4484550">And</span> <span m="4484690">one</span> <span m="4484930">of</span>
  <span m="4485080">them</span> <span m="4485920">is</span> <span m="4486430">that</span>
  <span m="4486700">they</span> <span m="4486880">want</span> <span m="4487120">to</span>
  <span m="4487360">encourage</span> <span m="4488200">asking</span> <span m="4488680">questions</span>
  <span m="4489850">that</span> <span m="4490030">are</span> <span m="4490150">likely</span>
  <span m="4490600">to</span> <span m="4490750">have</span> <span m="4491020">positive</span>
  <span m="4491680">answers</span> <span m="4492250">rather</span> <span m="4492640">than</span>
  <span m="4492850">negative</span> <span m="4493300">answers.</span> <span m="4494440">And</span>
  <span m="4494590">the</span> <span m="4494680">reason</span> <span m="4495130">is</span>
  <span m="4495400">because</span> <span m="4495850">in</span> <span m="4496060">their</span>
  <span m="4496270">world,</span> <span m="4497200">there</span> <span m="4497500">are</span>
  <span m="4498010">hundreds</span> <span m="4498520">and</span> <span m="4498640">hundreds</span>
  <span m="4499150">of</span> <span m="4499270">questions.</span> <span m="4500020">And</span>
  <span m="4500170">of</span> <span m="4500290">course,</span> <span m="4500620">most</span>
  <span m="4500950">patients</span> <span m="4501910">don't</span> <span m="4502270">have</span>
  <span m="4502630">most</span> <span m="4503020">of</span> <span m="4503140">those</span>
  <span m="4503830">findings.</span> <span m="4505030">And</span> <span m="4505180">so</span>
  <span m="4505390">you</span> <span m="4505510">don't</span> <span m="4505750">want</span>
  <span m="4505930">to</span> <span m="4505990">ask</span> <span m="4506350">a</span>
  <span m="4506410">whole</span> <span m="4506560">bunch</span> <span m="4506860">of</span>
  <span m="4506950">questions</span> <span m="4507880">to</span> <span m="4508030">which</span>
  <span m="4508270">the</span> <span m="4508420">answer</span> <span m="4508810">is</span>
  <span m="4508990">no,</span> <span m="4509440">no,</span> <span m="4509830">no,</span>
  <span m="4510190">no,</span> <span m="4510490">no,</span> <span m="4510790">no,</span>
  <span m="4511030">no,</span> <span m="4511270">no,</span> <span m="4511510">no,</span>
  <span m="4512320">because</span> <span m="4512680">that</span> <span m="4512860">doesn't</span>
  <span m="4513190">give</span> <span m="4513370">you</span> <span m="4513520">very</span>
  <span m="4513760">much</span> <span m="4514000">guidance.</span> <span m="4514600">You</span>
  <span m="4514690">want</span> <span m="4514870">to</span> <span m="4514930">ask</span>
  <span m="4515170">questions</span> <span m="4516130">where</span> <span m="4516310">the</span>
  <span m="4516460">answer</span> <span m="4516850">is</span> <span m="4517030">yes,</span>
  <span m="4517420">because</span> <span m="4517870">that</span> <span m="4518230">helps</span>
  <span m="4518560">you</span> <span m="4518680">clue</span> <span m="4519040">in</span>
  <span m="4519640">on</span> <span m="4519820">what's</span> <span m="4520060">really</span>
  <span m="4520300">going</span> <span m="4520630">on.</span></p><p><span m="4522950">So</span>
  <span m="4524590">they</span> <span m="4524920">actually</span> <span m="4525400">have</span>
  <span m="4525610">a</span> <span m="4525670">nice</span> <span m="4526000">proof</span>
  <span m="4526990">that</span> <span m="4527590">they</span> <span m="4527920">do</span>
  <span m="4528160">this</span> <span m="4528400">thing</span> <span m="4528670">they</span>
  <span m="4528850">call</span> <span m="4529120">reward</span> <span m="4529630">shaping,</span>
  <span m="4530680">which</span> <span m="4530950">basically</span> <span m="4531910">adds</span>
  <span m="4532240">some</span> <span m="4532690">incremental</span> <span m="4533830">reward</span>
  <span m="4535540">for</span> <span m="4536140">asking</span> <span m="4536620">questions</span>
  <span m="4537310">that</span> <span m="4537580">will</span> <span m="4537730">have</span>
  <span m="4537940">a</span> <span m="4538000">positive</span> <span m="4538570">answer.</span>
  <span m="4539650">But</span> <span m="4540100">they</span> <span m="4540280">can</span>
  <span m="4540490">prove</span> <span m="4541000">that</span> <span m="4541390">an</span>
  <span m="4541600">optimal</span> <span m="4542230">policy</span> <span m="4543040">learned</span>
  <span m="4543460">from</span> <span m="4543820">that</span> <span m="4544120">reward</span>
  <span m="4544540">function</span> <span m="4545500">is</span> <span m="4545710">also</span>
  <span m="4546130">optimal</span> <span m="4546670">for</span> <span m="4546940">the</span>
  <span m="4547090">reward</span> <span m="4547450">function</span> <span m="4547930">that</span>
  <span m="4548140">would</span> <span m="4548290">not</span> <span m="4548530">include</span>
  <span m="4549000">it.</span> <span m="4550090">So</span> <span m="4550300">that's</span>
  <span m="4550940">kind</span> <span m="4551060">of</span> <span m="4551120">cool.</span></p><p><span
  m="4552510">And</span> <span m="4552560">then</span> <span m="4552740">the</span>
  <span m="4552890">other</span> <span m="4553160">thing</span> <span m="4553400">they</span>
  <span m="4553580">do</span> <span m="4553970">is</span> <span m="4554930">to</span>
  <span m="4555740">try</span> <span m="4556010">to</span> <span m="4556160">identify</span>
  <span m="4557000">a</span> <span m="4557150">reduced</span> <span m="4557690">space</span>
  <span m="4558200">of</span> <span m="4558290">findings</span> <span m="4559490">by</span>
  <span m="4559760">what</span> <span m="4560000">they</span> <span m="4560150">call</span>
  <span m="4560450">feature</span> <span m="4560900">rebuilding.</span> <span m="4562310">And</span>
  <span m="4562490">this</span> <span m="4562760">is</span> <span m="4562940">essentially</span>
  <span m="4563630">a</span> <span m="4563690">dimension</span> <span m="4564260">reduction</span>
  <span m="4564800">technique</span> <span m="4565910">where</span> <span m="4566180">they're</span>
  <span m="4566510">co-training.</span> <span m="4569060">In</span> <span m="4569240">this</span>
  <span m="4569450">dual</span> <span m="4569720">network</span> <span m="4570260">architecture,</span>
  <span m="4571510">they're</span> <span m="4571760">co-training</span> <span m="4573130">the</span>
  <span m="4573260">policy</span> <span m="4573860">model.</span> <span m="4575690">It's,</span>
  <span m="4576280">of</span> <span m="4576380">course,</span> <span m="4576710">the</span>
  <span m="4576770">neural</span> <span m="4577100">network</span> <span m="4577550">model,</span>
  <span m="4577940">this</span> <span m="4578150">being</span> <span m="4578480">that</span>
  <span m="4578870">2010s.</span></p><p><span m="4581480">And</span> <span m="4581660">so</span>
  <span m="4581930">they're</span> <span m="4582110">generating</span> <span m="4583100">a</span>
  <span m="4583250">sequence,</span> <span m="4584480">a</span> <span m="4585020">deep</span>
  <span m="4585800">layered</span> <span m="4586340">set</span> <span m="4586640">of</span>
  <span m="4586760">neural</span> <span m="4587060">networks</span> <span m="4588170">that</span>
  <span m="4588650">generate</span> <span m="4589250">an</span> <span m="4589430">output,</span>
  <span m="4590520">which</span> <span m="4590750">is</span> <span m="4590960">the</span>
  <span m="4591260">m</span> <span m="4591560">questions</span> <span m="4592430">and</span>
  <span m="4592610">the</span> <span m="4592760">n</span> <span m="4593000">conclusions</span>
  <span m="4594050">that</span> <span m="4594260">can</span> <span m="4594500">be</span>
  <span m="4594650">made.</span> <span m="4595490">And</span> <span m="4595610">I</span>
  <span m="4595730">think</span> <span m="4596000">there's</span> <span m="4596090">a</span>
  <span m="4596360">soft max</span> <span m="4597200">over</span> <span m="4597500">these</span>
  <span m="4597860">to</span> <span m="4598370">come</span> <span m="4598640">up</span>
  <span m="4598790">with</span> <span m="4599030">the</span> <span m="4599150">right</span>
  <span m="4599450">policy</span> <span m="4600470">for</span> <span m="4600800">any</span>
  <span m="4601010">particular</span> <span m="4601790">situation.</span></p><p><span
  m="4603330">But</span> <span m="4603440">at</span> <span m="4603560">the</span>
  <span m="4603680">same</span> <span m="4604010">time,</span> <span m="4604820">they</span>
  <span m="4605030">co-train</span> <span m="4605780">it</span> <span m="4606410">in</span>
  <span m="4606590">order</span> <span m="4606920">to</span> <span m="4607160">predict</span>
  <span m="4608000">a</span> <span m="4609440">number</span> <span m="4610190">of--</span>
  <span m="4611870">all</span> <span m="4612170">of</span> <span m="4612320">the</span>
  <span m="4612410">manifestations</span> <span m="4614000">from</span> <span m="4614420">what</span>
  <span m="4614690">they've</span> <span m="4614990">observed</span> <span m="4615500">before.</span>
  <span m="4616610">So</span> <span m="4616850">it's</span> <span m="4617030">using--</span>
  <span m="4617660">it's</span> <span m="4617840">learning</span> <span m="4618380">a</span>
  <span m="4618410">probabilistic</span> <span m="4619250">model</span> <span m="4620150">that</span>
  <span m="4620390">says</span> <span m="4620960">if</span> <span m="4621200">you've</span>
  <span m="4621470">answered</span> <span m="4621980">the</span> <span m="4622100">following</span>
  <span m="4622610">questions</span> <span m="4623240">in</span> <span m="4623330">the</span>
  <span m="4623420">following</span> <span m="4623930">ways,</span> <span m="4624920">here</span>
  <span m="4625190">are</span> <span m="4625370">the</span> <span m="4625490">likely</span>
  <span m="4626030">answers</span> <span m="4626660">that</span> <span m="4626900">you</span>
  <span m="4627050">would</span> <span m="4627230">give</span> <span m="4627530">to</span>
  <span m="4627710">the</span> <span m="4627860">remaining</span> <span m="4628760">manifestations.</span>
  <span m="4630560">And</span> <span m="4630710">the</span> <span m="4630800">reason</span>
  <span m="4631190">they</span> <span m="4631340">can</span> <span m="4631520">do</span>
  <span m="4631700">that,</span> <span m="4632040">of</span> <span m="4632060">course,</span>
  <span m="4632550">is</span> <span m="4632600">because</span> <span m="4632990">they</span>
  <span m="4633140">really</span> <span m="4633440">are</span> <span m="4633560">not</span>
  <span m="4633830">independent.</span> <span m="4634850">They're</span> <span m="4635420">very</span>
  <span m="4635750">often</span> <span m="4637150">co-varying.</span> <span m="4638570">And</span>
  <span m="4638750">so</span> <span m="4638960">they</span> <span m="4639170">learn</span>
  <span m="4639500">that</span> <span m="4639770">covariance,</span> <span m="4640700">and</span>
  <span m="4640880">therefore</span> <span m="4641870">can</span> <span m="4642140">predict</span>
  <span m="4642650">which</span> <span m="4642980">answers</span> <span m="4643520">are</span>
  <span m="4643640">going</span> <span m="4643820">to</span> <span m="4644030">get</span>
  <span m="4644330">yes</span> <span m="4644690">answers,</span> <span m="4646070">which</span>
  <span m="4646400">questions</span> <span m="4646940">are</span> <span m="4647060">going</span>
  <span m="4647190">to</span> <span m="4647270">get</span> <span m="4647510">yes</span>
  <span m="4647810">answers.</span> <span m="4648380">And</span> <span m="4648560">therefore,</span>
  <span m="4649040">they</span> <span m="4649220">can</span> <span m="4649460">bias</span>
  <span m="4650420">the</span> <span m="4650570">learning</span> <span m="4651020">toward</span>
  <span m="4651470">doing</span> <span m="4651860">that.</span></p><p><span m="4653330">So</span>
  <span m="4654260">last</span> <span m="4655520">slide.</span> <span m="4658400">So</span>
  <span m="4658610">this</span> <span m="4658750">system</span> <span m="4659240">is</span>
  <span m="4659390">called</span> <span m="4659690">REFUEL.</span> <span m="4661220">It's</span>
  <span m="4661490">been</span> <span m="4661700">tested</span> <span m="4662390">on</span>
  <span m="4662660">a</span> <span m="4662750">simulated</span> <span m="4663530">data</span>
  <span m="4663870">set</span> <span m="4664760">of</span> <span m="4664940">650</span>
  <span m="4665900">diseases</span> <span m="4666560">and</span> <span m="4666670">375</span>
  <span m="4667880">symptoms.</span> <span m="4669560">And</span> <span m="4669770">what</span>
  <span m="4669980">they</span> <span m="4670160">show</span> <span m="4671210">is</span>
  <span m="4671540">that</span> <span m="4672740">the</span> <span m="4673310">red</span>
  <span m="4673580">line</span> <span m="4673940">is</span> <span m="4674120">their</span>
  <span m="4674390">algorithm.</span> <span m="4676160">The</span> <span m="4676790">yellow</span>
  <span m="4677210">line</span> <span m="4677600">uses</span> <span m="4678350">only</span>
  <span m="4679220">this</span> <span m="4679460">reward</span> <span m="4679940">reshaping.</span>
  <span m="4681220">And</span> <span m="4681380">the</span> <span m="4681500">blue</span>
  <span m="4681800">line</span> <span m="4682370">is</span> <span m="4682940">just</span>
  <span m="4683330">a</span> <span m="4683360">straight</span> <span m="4683780">reinforcement</span>
  <span m="4684590">learning</span> <span m="4684950">approach.</span></p><p><span
  m="4685910">And</span> <span m="4686060">you</span> <span m="4686210">can</span>
  <span m="4686390">see</span> <span m="4686690">that</span> <span m="4687110">they're</span>
  <span m="4687350">doing</span> <span m="4687980">much</span> <span m="4688310">better</span>
  <span m="4689150">after</span> <span m="4689540">many</span> <span m="4689840">fewer</span>
  <span m="4690290">epochs</span> <span m="4690740">of</span> <span m="4690860">training</span>
  <span m="4691780">in</span> <span m="4691910">doing</span> <span m="4692240">this.</span>
  <span m="4692990">Now,</span> <span m="4693170">take</span> <span m="4693440">this</span>
  <span m="4693680">with</span> <span m="4693890">a</span> <span m="4693950">grain</span>
  <span m="4694250">of</span> <span m="4694340">salt.</span> <span m="4694860">This</span>
  <span m="4695000">is</span> <span m="4695150">all</span> <span m="4695360">fake</span>
  <span m="4695720">data.</span> <span m="4697310">So</span> <span m="4697550">they</span>
  <span m="4697700">didn't</span> <span m="4697910">have</span> <span m="4698180">real</span>
  <span m="4698420">data</span> <span m="4698750">sets</span> <span m="4699140">to</span>
  <span m="4699260">test</span> <span m="4699590">this</span> <span m="4699830">on.</span>
  <span m="4700790">They</span> <span m="4701000">got</span> <span m="4701270">statistics</span>
  <span m="4702260">on</span> <span m="4703490">what</span> <span m="4704360">diseases</span>
  <span m="4705080">are</span> <span m="4705230">common</span> <span m="4705770">and</span>
  <span m="4705920">what</span> <span m="4706130">symptoms</span> <span m="4706730">are</span>
  <span m="4706850">common</span> <span m="4707300">in</span> <span m="4707420">those</span>
  <span m="4707690">diseases.</span></p><p><span m="4708860">And</span> <span m="4709010">then</span>
  <span m="4709190">they</span> <span m="4710120">had</span> <span m="4710300">a</span>
  <span m="4710360">generative</span> <span m="4710930">model</span> <span m="4711830">that</span>
  <span m="4712010">generated</span> <span m="4712700">this</span> <span m="4712910">fake</span>
  <span m="4713210">data.</span> <span m="4714420">And</span> <span m="4714500">then</span>
  <span m="4714710">they</span> <span m="4714890">learned</span> <span m="4715340">from</span>
  <span m="4715910">that</span> <span m="4716150">generative</span> <span m="4716750">model.</span>
  <span m="4717350">So</span> <span m="4718160">of</span> <span m="4718310">course</span>
  <span m="4718640">it</span> <span m="4718730">would</span> <span m="4718880">be</span>
  <span m="4719030">really</span> <span m="4719360">important</span> <span m="4719930">to</span>
  <span m="4720200">redo</span> <span m="4720680">the</span> <span m="4720860">study</span>
  <span m="4721340">with</span> <span m="4721580">real</span> <span m="4721850">data,</span>
  <span m="4722960">but</span> <span m="4723200">they've</span> <span m="4723380">not</span>
  <span m="4723620">done</span> <span m="4723830">that.</span> <span m="4724370">This</span>
  <span m="4724580">was</span> <span m="4724760">just</span> <span m="4724970">published</span>
  <span m="4725420">a</span> <span m="4725450">few</span> <span m="4725660">months</span>
  <span m="4725960">ago.</span></p><p><span m="4727110">So</span> <span m="4727160">that's</span>
  <span m="4727400">sort</span> <span m="4727670">of</span> <span m="4727790">where</span>
  <span m="4727970">we</span> <span m="4728180">are</span> <span m="4728450">at</span>
  <span m="4728570">the</span> <span m="4728690">moment</span> <span m="4729290">in</span>
  <span m="4729560">diagnosis</span> <span m="4730470">and</span> <span m="4730590">in</span>
  <span m="4730700">differential</span> <span m="4731300">diagnosis.</span> <span
  m="4733040">And</span> <span m="4733460">I</span> <span m="4734180">wanted</span>
  <span m="4734510">to</span> <span m="4734690">start</span> <span m="4735230">by</span>
  <span m="4735710">introducing</span> <span m="4736850">these</span> <span m="4737150">ideas</span>
  <span m="4737720">in</span> <span m="4737840">a</span> <span m="4737900">kind</span>
  <span m="4738200">of</span> <span m="4738320">historical</span> <span m="4738950">framework.</span>
  <span m="4740360">But</span> <span m="4740600">it</span> <span m="4740720">means</span>
  <span m="4741050">that</span> <span m="4741260">there</span> <span m="4741440">are</span>
  <span m="4741490">a</span> <span m="4741530">tremendous</span> <span m="4742130">number</span>
  <span m="4742490">of</span> <span m="4742640">papers,</span> <span m="4743210">as</span>
  <span m="4743390">you</span> <span m="4743510">can</span> <span m="4743690">imagine,</span>
  <span m="4744710">that</span> <span m="4744920">have</span> <span m="4745130">been</span>
  <span m="4745310">written</span> <span m="4746000">since</span> <span m="4746540">the</span>
  <span m="4746750">1990s</span> <span m="4748160">and '80s</span> <span m="4748910">that</span>
  <span m="4749150">I</span> <span m="4749240">was</span> <span m="4749390">showing</span>
  <span m="4749810">you</span> <span m="4750590">that</span> <span m="4751220">are</span>
  <span m="4751640">essentially</span> <span m="4752270">elaborations</span> <span
  m="4753320">on</span> <span m="4753500">the</span> <span m="4753590">same</span>
  <span m="4753920">themes.</span> <span m="4755090">And</span> <span m="4755270">it's</span>
  <span m="4755510">only</span> <span m="4755900">in</span> <span m="4756050">the</span>
  <span m="4756230">past</span> <span m="4756590">decade</span> <span m="4757250">of</span>
  <span m="4757970">the</span> <span m="4758180">advent</span> <span m="4758690">of</span>
  <span m="4758810">these</span> <span m="4759410">neural</span> <span m="4759710">network</span>
  <span m="4760160">models</span> <span m="4761120">that</span> <span m="4761330">people</span>
  <span m="4761690">have</span> <span m="4761870">changed</span> <span m="4762710">strategy,</span>
  <span m="4764540">so</span> <span m="4764810">that</span> <span m="4764990">instead</span>
  <span m="4765440">of</span> <span m="4765560">learning</span> <span m="4766220">explicit</span>
  <span m="4766820">probabilities,</span> <span m="4767790">for</span> <span m="4767900">example,</span>
  <span m="4768440">like</span> <span m="4768710">you</span> <span m="4768830">do</span>
  <span m="4769040">in</span> <span m="4769160">a</span> <span m="4769190">Bayesian</span>
  <span m="4770120">network,</span> <span m="4771210">you</span> <span m="4771260">just</span>
  <span m="4771590">say,</span> <span m="4771920">well,</span> <span m="4772190">this</span>
  <span m="4773240">is</span> <span m="4773330">simply</span> <span m="4773900">a</span>
  <span m="4774590">prediction</span> <span m="4775130">task.</span></p><p><span m="4776030">And</span>
  <span m="4776210">so</span> <span m="4776450">we'll</span> <span m="4776720">predict</span>
  <span m="4777200">the</span> <span m="4777320">way</span> <span m="4777560">we</span>
  <span m="4777710">predict</span> <span m="4778130">everything</span> <span m="4778610">else</span>
  <span m="4778880">with</span> <span m="4779090">neural</span> <span m="4779360">network</span>
  <span m="4779810">models,</span> <span m="4780710">which</span> <span m="4780980">is</span>
  <span m="4781140">we</span> <span m="4781310">build</span> <span m="4781630">a</span>
  <span m="4781670">CNN,</span> <span m="4782330">or</span> <span m="4782540">an</span>
  <span m="4782720">RNN,</span> <span m="4783200">or</span> <span m="4783710">some</span>
  <span m="4783980">combination</span> <span m="4784760">of</span> <span m="4784880">things,</span>
  <span m="4785330">or</span> <span m="4785480">some</span> <span m="4785960">attention</span>
  <span m="4786470">model,</span> <span m="4786890">or</span> <span m="4787070">something.</span>
  <span m="4788660">And</span> <span m="4788780">we</span> <span m="4788930">throw</span>
  <span m="4789230">that</span> <span m="4789500">at</span> <span m="4789700">it.</span>
  <span m="4789980">And</span> <span m="4790190">it</span> <span m="4790280">does</span>
  <span m="4790580">typically</span> <span m="4791120">a</span> <span m="4791180">slightly</span>
  <span m="4791690">better</span> <span m="4791990">job</span> <span m="4792380">than</span>
  <span m="4792590">any</span> <span m="4792830">of</span> <span m="4792950">the</span>
  <span m="4793100">previous</span> <span m="4793580">learning</span> <span m="4793940">methods</span>
  <span m="4794420">that</span> <span m="4794600">we've</span> <span m="4794810">used</span>
  <span m="4795560">typically,</span> <span m="4796320">but</span> <span m="4796430">not</span>
  <span m="4796640">always.</span></p><p><span m="4797780">OK.</span> <span m="4798320">Peace.</span></p>
type: course
uid: 7c1732890f7067b5e9d525f49e2010e5

---
None