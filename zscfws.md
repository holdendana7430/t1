代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3moeojndd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pcpoutnf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pwjqvxwe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3crjkqyjw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cnrhjwxs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvuxjv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wgfucape.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fczgxcuv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xbcixawd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wwwrakqf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3adwosbzi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qtfyrpzl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tkedpcus.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wfcgmdcf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3usuyfczk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ljwtqvhm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pruuurji.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3udtzkthr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aocrlbwv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3rghsyuys.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nwazwbhk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3fwtxnqqc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3buzyeymg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qvlshuky.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hcmdpgki.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3asozmobp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdqvrnaf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hweliems.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzwebuum.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kbylxppc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uuwifwgz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hsrytdyy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3euqauqrr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vwsfqoxc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3boonpccv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jqqmxtdd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kuvrgvfb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3uonoqweo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ggjbpdxp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pihyugzx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3btdrkjku.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3srmvfjcv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yeguaucf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3olqnbsny.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jidumqnk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wdbyigmp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hkcexwwy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zscfdjap.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vnkelyfi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jhjtnkvw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ygyvcyam.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3bsenoudv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zkmklfac.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hlqgpjyp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zicpkegl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cqijkksx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrsgolp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dnaipmrc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ckodyrrw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kilbbxtv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jxuzcsxs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ivhvvqho.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3elpwpoqj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drxzvutr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ilvuoxeh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxldjnb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ufvgefdc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kbdwsvci.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fynwsgoo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iylyzfje.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3npsrkqld.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xeqfudsk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hyweohza.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3frpenwbb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fwpabbpn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3dyaebpht.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3glhdmvwc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vsctbgxb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3imhgvknx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jcmytcks.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xlfmpawy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rnspnkvu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3glvwhuxt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvvuwdd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dysbutqz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uhahdvhn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rbbyubcm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ruzdhnpo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3koktdsru.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3piyyxklr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bvsnmklh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cfuvufwo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3agllttzi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3pzvbmtkc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dfaxshfi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lvdgjqdl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3owrurzru.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqkerjj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3csschryd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiaihtg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifizhgqd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxiemfuq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bpvqrjul.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ytmhcnxi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3oygvjsyv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3bbmqlxdv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yxtisgdc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tszchvfv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pldfsmhr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3elkylojq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3prcbuqys.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3suhigekq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3krqlovxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwvtqsiz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gcucvwjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okexejpt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3oqdqkgum.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3brzccusi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yugjtvdy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aedpzhzr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ggapsrjm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3csgydgck.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3nusifqkt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nqehnlvr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gryrbmxr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xkmnncdp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mlqrxczm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbufakyx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3srwbazvb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xdajdjte.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vfjwchkj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yrdkauhd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3slhnzlwc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3phsxnpbw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lhkntrfr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vkvohldu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3epjkwicr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3deeczxvm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqkulkbu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uqikcxyk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zgzmmynv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bzbqlxjj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yxflzrpa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vlfxvhvh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3upvdpgky.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3teyuerks.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3secmggbq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aohkmsie.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mnzzfobp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ilhuaxne.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqzdilx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mpzqjxqt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3euvxfeui.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyhgdgl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwrpiirr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3swqnoorm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pgslqcxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxfcqpk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3apxkzukk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkcymb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hxtsufer.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bpilxjwn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xdnyvajv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiztnlpb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwpffa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsuxwfk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3evlehrwj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbegdav.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tllwgsyf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wbhwthny.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3euwtxzwi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixbhejvi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esfswzzv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mojupbtr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3srihsjpy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yfprhjju.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cbgnphmt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqjdgnob.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfhphblo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lvckodkx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yeugcfyd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxcvibvv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrwwrkjq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3afhdbakr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pofjykhu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3exhvyjsu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3aefbywxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hzpmateo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3npxejepc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ietjtaei.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lsaofcte.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3liptnahu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3szqnxjfm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fzpvozqy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvdyjtng.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pptdgtrc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qmutzujt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3alrovpyo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rnorwaem.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3cnbangsr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mnyueqnj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nzyeoiny.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpxrwpoq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rrvhzuvm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3maghlsse.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyyjvnmf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cyhbvycr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fckspivi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3isyamxmg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3szbupkfu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dxbousff.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ymdsafbd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jzdtestr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3csrljdbm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fmzroyiq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3scqgzkug.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mvdqivck.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3drzvwrww.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gnpbcyvc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhusduh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nydkytsm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ibfpvsfv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3safapstz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3imynqrth.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bksbqqgc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3elyrgqcl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdiyia.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3trphewep.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yjqmcgov.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nlajekto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxrnvqf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyhlnao.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oeevxrnx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rmpreehl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ablqnvvl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ircxagtb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nxjmmxkf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlthpbng.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfqcsqxr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3axayaewm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vwgcnkof.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uifciptw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tugpcygp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nvsxejmm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zfqbkpgt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ftjgzpju.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ceodqcai.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hncrbzfc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqdxssja.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cphnkxgw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3simsvoab.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uembuepv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fnryjuhd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pteyendk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3urexjkgo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kvaenlih.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zuzitjcx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhgxgsn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xloofmws.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eqoicpdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acxllxku.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tuwigbdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyxqxwsw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvzetsgt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mwwudkij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3albzmifw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ydigasya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3offqiwml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3haebqpip.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzswmso.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bynaiuie.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rtyowyzs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrgivnor.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3eephacdm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3skhbfgvl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qkypbtlk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nnwbieau.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ruimvkcf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fqbzaoqg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vghluxwz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qywhjigh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3htybefmw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bfeyjxml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3znptabro.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpixykiu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3waioltxd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3whzhwvvk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rkiopevq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gvfuxsob.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dycvjfqj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3uvmladmt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nimpxcri.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pcaabbyd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cacuyamj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xelvrakq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fwvijuow.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tqmpwidr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrhtuzu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqudunpp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3auyyjfsq.html


<!-- 参考信息 -->