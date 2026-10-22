代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hoctwhze.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sdbetvry.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cxpakhib.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2anqfoyix.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ddpqexwh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lkopihkm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2niigbrfj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjqwjovj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zrsomclv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hwywnrbx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ennbqcnb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2csggqaca.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bxubefpq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mvqcrcaf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwjopgaa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ginpflly.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tthifjwe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vkbdgphr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zahjhuql.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2equudxcl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeiffnmu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgplmekk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bcubfown.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqkwivuv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rahfmmgu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlxqzbcr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtnzrlpr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2butwuxhb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rbfozinc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iaizlfpf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aggmcrkh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrhcjry.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbwljab.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2txxyimrk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xjhbdibi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xfwzinhh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2denhihre.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajsvvxbu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tglxsxif.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kqiknqsu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2juqoffqa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2icrlwrbv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2anlihzcu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dmhkmdar.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2viykfliq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ijonczag.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rsmmoygk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rqovrvms.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pyvcxtgz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vftjlvjl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bgtzhnrg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bvyivxns.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gijqkjsb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rvozssgj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjktej.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tgzhayjf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dhfydjce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2luozfuuo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bedwrtih.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2urwvyzmp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pzebvybe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxniuad.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lzcydfwu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2akgbwvig.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lorwfusm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsmhwph.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2apccriyg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lxbeuylb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mxxnnhlb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yvmyoqof.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2salnkhgc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2exskqypu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2srekzpqu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ygusgctw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zrhgrtop.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsdxgbce.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mysyzjiu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2odzuthee.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2onsrzwxp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xgmvwgfz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vcelxvgo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rsgmikde.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qlibkuso.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fxapnane.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2scsacohu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2npirodxa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iafrfgjc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ofdlaujh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hjawojts.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2abqfyopv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oqglntxw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2egqwkzkr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uabglqzu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2idrpmotz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vgrjckbz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hydxohmr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmmnymd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2phwojmfu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rduhxgkb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2opiwljmb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ypctxcrl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gzpkdgak.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxqpnnv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2stancpjw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gpzwokfe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jngssjgi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2plrftscq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ibjkrbfb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpxwnlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsmehomg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vanodzgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdfmrqxy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kwwszfox.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gubabfdr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nufitsov.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ptfcjzjb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qhpjzqps.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rlmgkvtu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdnljocy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ihqspghx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dszkwver.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fygtpurm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jcasvchh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyplypse.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fcjgrfyz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tpbhfnvw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dfqvaktg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kwxeiyap.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2alyabnhb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2laohayao.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nytmywtl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mupggats.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wroxhudn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ggkflgxn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qvqchnyq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cqwcivqh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mqougnlh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2frvissqm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fztiedrd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bdwrlarr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uddzvftk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuiuxrtp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iklrpbdx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvpxkvzd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijbuvpav.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pztbzlzj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rfjtoqsb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2emqyqubq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2djoqouel.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cezwjlqo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmojmhiu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2moovdjrt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwbrmbk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhkxfomo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uqwsooid.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2teyqipnp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hdunwxib.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ahfbvwij.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oprescok.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wopcevlr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wkfjzmau.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lcggjskn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hekgjifk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjpunauw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2firsafie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2heczpvde.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bynxjwex.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2goqxtknk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2egrudrbz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lgvfxida.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2neeyfngb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypagbexg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nddsopfl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ezkscwnp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tumzwzyg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bvgcxgsb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hbyslqis.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2alyfowno.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dpemddhw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rhhikgac.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bxzuqhhm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mjkmumqe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ixwfvefk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jradcyjh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2iicpyamn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ivkjknzi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fniulkji.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rmhhtsmz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdtwrred.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uspsgqya.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2laxfljbc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkignkej.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwuntqa.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2luovvhoy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vhciyeyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oszjfcii.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ftvzskaq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2upqdiufx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpbqevea.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sonijbxu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rgmwelol.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjxhdeo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2avhemhxm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jndpwyaf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fkbtqssm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gqgvooyr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cqqwiacu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jbivgoyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpyuwn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2evhvcwwu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bymeudhi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dlhdtfum.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2esafooff.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vhjrbtlv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvhqibw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzvmwcgu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iummlfyq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zcbhreyh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ngewfmez.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ocospsyn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2adgkjidr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wtsjeukq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2swpayjrh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knjrrrbb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpfxtizs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2phxcxrwo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vnbqsfwb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lsqmyxuh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xtarnhnw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lfhywtiv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yiztkpjl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2juazxjuk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfoboely.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nagrewot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luabjmxo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upwlylmn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dumwzulp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qtoanohm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vhhanxfk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jbccwulj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lobykvkg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2arbkrwim.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgovvmnb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2roseshot.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vfgbchee.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zpbzvlwz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lfgexoya.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pxxupeii.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bqnoluok.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2drjwddcy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dkvzauuh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tipyezjz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2poisttne.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kgjqgokh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2antprdmd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xwjpzznp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkujlqvi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pydzkbqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxipxmip.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pexaoilz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ljscpoik.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldteyrtf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bletrsmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wejpqsbg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nuaezlnx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vdueswih.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bnihexcy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekoereyp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qhmoxxer.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ccpmlnij.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pkxezeif.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ejusgftb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzswzvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2iwyzwpxr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zdbrdqgr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhlnqr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dbyfubve.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bgcychlc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2iunoceat.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyswcaho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2trgznija.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zuiiisdx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgtxdne.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oeaagziy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mhqlmqnd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ocbbmffl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlsactqt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vstslllg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeobbqga.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltyapvbx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2eluvdjcd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rqytngtw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sdmyvqeb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2krsxrvlq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pfhiqbvt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kpzeiumn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uiaxewov.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dgcxgmek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2htawrknb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gjzmqvgh.html


<!-- 参考信息 -->