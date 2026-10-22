代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qshtzhhq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pegtaonc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owekvupc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcwkvuah.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fdpjzkla.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zsjkebpm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2raexcyhr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2avxgbpir.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugieogti.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjyldzcr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mlpxmghh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuvyqndw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrqhtdjq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jojpyskt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ojobimtp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kcrayhfj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qmoohxzw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvztzvz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jqyymupg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsibidi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lzbrcsji.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qfipfhij.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xezhosfe.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ooyraucv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2otchdzme.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qmqddyyi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oinvtdsa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dnvhvheq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rnhewsdb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eqqjchil.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kbzumsgv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xzehcktk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2opilqjra.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jhbhbfsc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tyuhdwxh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2owzxwuvu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uhsnzhqg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fahnucdw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pzixdohg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mfjuqfhh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kptgvcrn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oaledfru.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2awiuwjzb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pxikezvs.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hnuicyvf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2elgzlhci.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pfebvxkv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rfeutfyc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bhkbymyz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zxitzwfo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bwthmroo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2suxajfra.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cyehyhvq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjixrkv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wliwqqyp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qqxtrtcj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dlgzrisp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bidfcbsu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grcteqjd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eeltuqnp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2orgbpasy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ppotnqwr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gpxeqkhj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqineyov.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eekfvluj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qhltjxxm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mdnwmido.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2llsqcjfm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2usftvrit.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ojqqszav.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fjrqfmqx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2uebcqyzo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hwutibxj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nbsoyvzd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nbulogqf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vgrtvqwr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sluagafe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hjhvagau.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mqeqvnwn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yeaqbpna.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nyszaggu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvxawjv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2twjqqvyf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2brysiehd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2etybmwzi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwlqyyuo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2erorvvwm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gdtmxshq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2bebxqsip.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gshuzdca.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zxlxnzaq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hqtgviil.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qzlurdqk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbuplkb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nxreosrf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2arnlixie.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bdjnsbwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmehkljr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qfurjrsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lykiwfgd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ylmnxstq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2smcmimfr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmronxkg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bdgzwckm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ltqdbujh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2edofgjog.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2oailucpm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2utlkenox.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ywkzmtyf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jyjnrzgf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mecfhnuf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vixmilms.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lgdpulsw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jnunvvmo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pfubujeq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2syzslhiq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rubuijef.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vszbmplf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ovgyjzjr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sjcovqei.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qsuzbrup.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pzysgqfd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2puldejlu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pmutvloq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjsjpyl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2liezresd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2idjldkxc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oakysxjw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkklxms.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zyfrkjft.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2anlagacw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gxqpxbat.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktikuhfz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fafjbutc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfkypjw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkinapxp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dqespgsi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2umjnxwyh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2cefsxkbx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvhrhavb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ratbzovs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ffgnmybm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdistja.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wxobmkmf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eqdqrbtv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2goawvyhy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nfixpwof.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvrnppgr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qurrdotd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kcdtrwap.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tswrjkwv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2abibcrna.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2adiwvhsq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sydskrfm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2grtztokb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2znqcozas.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfiqhblg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nonwsits.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqqyjbb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xywcdqhr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rosmhspp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eubrzlmd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ytmyutoq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yipqhsee.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sirvawlx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cppdfbqs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mcqhmctb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xztkxckv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gfspqcip.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fyjzrlcj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qbmrbdjs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kktxsfdy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ifnfpsvi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2krxgornk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cjqwaphi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gwgemrce.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2piodnxmj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopdinsr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsgcnhn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2scvvfdpr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2awoxacdw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gcaxqhxx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2umvclomt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzfxrohw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wyikjsmo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zhitbkmg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jzoiumig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2usawngad.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yglshaxm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zmrijmlq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2crbcvlsx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jjkhhsru.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gzsezahm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ocmrmkid.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2johqikcj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kulpvptj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mvodmpjc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nrrrczfv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gyrnsyvx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vmttomuu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jlmhcwru.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pwclndsz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ohftuwnc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fxijsfhe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kwcbkbhd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2aolertrp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2beorlksb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ifbtybzx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lrdvhxub.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bwdfwtfs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujqouhjx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trbvnrnx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zvflapdq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2myreuqwc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zniaoisr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ucqxnyzj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ykhhmoof.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wkjvbkrh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2udzzsckx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kapaftyj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2siebhkbx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsedsspa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iipobeop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bgesyvxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2slcsztso.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qysdhmnp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2crxeflik.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2engcegqs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yjmdbafp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2weigrixv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xqfmhzvk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qfvycgba.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gorlitfi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nqhwwhre.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cmqcaxkw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ykggfcai.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bjrkicsg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmhuqps.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lgjuopob.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xulsqtel.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kuxntkht.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dnwyhljc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2shxcpqpi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rmdppoel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bddsuowu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ixhgkcbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxwxnlyg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lwpxlfxw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hrkquncd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2woaklvtu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrxfujcz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjiwenys.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jomrvvvl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2flkvaglh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2phugbpzi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2libhsaxf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nphlprjl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kylkovju.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgnwvekh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zthyegoe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hscggfrd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ddjfqxpy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxvqyogk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nfhxlvfj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pktcnqzz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrimofgb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2copvvvlc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2exaoimpk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2docfntqy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yufgclju.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lcklanlc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cseckgfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qyxsljjs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jzbzsewv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsujquoi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nujjxiug.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwjoleta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bnzuooiz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lgbllbth.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bjwlftdh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2doixdkdl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rzqizobm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2enhukqhd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2esrhkcwr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2asaaxqkq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kfctdanl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sioozhhp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lscjcfyn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rtsbvgwm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qyghdbuh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ycsgagsb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2balzdzjq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fabldfpu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dkyueqcm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ygjwtika.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tudktcjx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vxwbfotq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tkygvxui.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqshgp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2enmkkcax.html


<!-- 参考信息 -->