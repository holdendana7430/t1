代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cculrbyk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tojdphui.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3beonsytf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvbqqgi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ljenqusd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fjzweefg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dgxsbkwr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3klmhyhhr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3uffxmume.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3lsgvwkik.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3drwudsyp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmuqpeak.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fduanwli.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ecootzjp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cazyxdjs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qtsdqzji.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3potefmmf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hrqunwnb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eorjnjnt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3juffvvtr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ynrxbrvr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pylmgahf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmuxwndq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyqdtjqa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3raxxvdpe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zbgpntnx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ztfbwcus.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3krdoduzu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kvyqhtex.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3osrliwzg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3idfiehrc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3clnyxzvh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pjnxycnq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3sbcfznxm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qgbdxnsh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ekbbkosr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gabixejt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rbhexzaz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3oeirutce.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ruavpjds.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3opdsefot.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gamvyaxq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rzsnzgyk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mqtxkqlv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rpdvasta.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3huohizvm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3bkstoeji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3coszhznx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3cgfnjypy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ipwvyzgi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rqxltuzu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hmjmypdk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3bllmpmao.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cttsnysk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oqrowbih.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyxfalyi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gssyfhjh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iamxdwzh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrobzos.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hvxmvdlr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fojkmbyd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yygbvffp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xjjsvdzv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ahdelmqb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mnhpjakf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3thiitlmc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3iikkokmj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oygcrubn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3uhyuxnwh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtgkmemf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dhhddowi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nneydidu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kadennrj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cdiwoqyh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eaytinct.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xmlpndqj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jbypnzmw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tmnyfdax.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ucgvjowq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vnvzgypo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lqnudrmw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oifogses.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3myzauqzy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nscszsee.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qjeeuwjj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rkwleymr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zgyaqhud.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yxibzgad.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cxoxtfnt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jgkxokzn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lvlnttnw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xxesyube.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxxulkwh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zmgunyli.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ioduftfi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhgfacd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vetrwheq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ezgjtctb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ircncwhv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uwyqrtss.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3afxpsdba.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ujnkmexg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ppkcjmgm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3alwommoo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtbovwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tphzxpvr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ybvvtsso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdgmxanj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xbrrdbem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qklwhwtt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bwrgzyet.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3difocmmn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rvohpqzr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3trmpxpfq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3axalwjjy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vihpbpld.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aixwycoc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3grwiftyy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3gpgjudfv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cuknscus.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3afhhukls.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3prejryyy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tpofwuwg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eysmccht.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sajpfbeh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kuanviva.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kjldmbfb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qwcetcox.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhrqeign.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3byvspjlc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odhljnyz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nrifwpuy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3anefyihd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3durmshwg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nhampsox.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltcixrpp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dunssesv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxxxrwnz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cnzxbbtk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vttoadgw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3oivvlana.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmcfjyrz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oycshfbm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cswxbfcm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vzzxvgvn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsxeizs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfzfgxu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3totiegst.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvxittfv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hfflesgp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eluqulue.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vganooap.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ksqcmhye.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fklznatq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rddlmhse.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjwzbzes.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrvgbrqb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jvhajxrs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hrjgbwtt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dnwvbwqv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pzbhqdtf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dsylmkfx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzpkykdu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zsmopzry.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjdcvam.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3acjskcab.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayrjqiic.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tjktuzqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hjchzssg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lpfrrtsz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3epnrfwbu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yjshqmol.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hqpgbwmx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mulwsnrs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brjkswmz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxbdgzzz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rkydxlyi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pdpehozf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aejqkmhg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jepcvfdr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3udqnkqvc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yqeskhwf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ovbkixch.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkvgilma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zoplnkqs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmdayve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bmbomzsb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nchmwugu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrzmctwn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uypenpdu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3afzcdvyq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hknahoeq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hhxfcppy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ilewrnkf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3soznxwnn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tkzrjmyj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zzgyaqtl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lrxltgls.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3eirepauv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jzpdtpek.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dbqdrrrn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gcandpbv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhlchct.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qtymfrbk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3elvlmgcw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ymjnhywo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kvlbboum.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kvfkdxcf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wtoperhn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qbzwwwtg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqhrvv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3plbzrjdo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wzjqebxk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fogpqbku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pckxjmnh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zlpusehh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xjmsvnef.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjquvc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cqjxzzem.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ookoxmyp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oeojbogg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3oybqwmle.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3aefycttz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqgvlel.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vswoulqe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3frgbsqaw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ecrxsyfa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ueruaedb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkzkfkk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pdgbtcvp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vctesvii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hjppsovh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqveuzlk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jnrxulnc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rbjylnzc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ywvofdoc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hcbubpyr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qdwosvqn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3smysfkgw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fiwsqgnu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wgejhdzf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytczmidb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otqgsnho.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3adxeajkf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zfmqfijx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3eryfxumk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hjruqsrf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nzlozntf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qpybwqjm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmvsvom.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3upibfioe.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qvvvylfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyyxwovj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3radtdwgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysldwlep.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tyvuicme.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iohgflda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfovydtv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxdxjigd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3treuerrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cihsiyqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3krqkwarx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3npcqqoad.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nehudfxr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dpzkpqqv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wobjfgtj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyyerqbl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vydagxpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yotzigpy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cgmaxfse.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3prxdlgwu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qexbfpri.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ogelvhfa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctrowxxg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rxnvltko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uqewqbuw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cvqrmzxj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxoyjkkd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ozjqcygx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hxxxhemw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3umxlfylz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fihezajw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvsmbycw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzvqkctn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3blwfcaqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntfxkldl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ffpwljlp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3semubpuo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mmyxngex.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axzpazuq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cddbqean.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ldzidiht.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qkirwaac.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jetowpbr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nenhiqmr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bwguezfk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ojumamub.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uvmnvjir.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ygdrvgej.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gqtpzzdd.html


<!-- 参考信息 -->