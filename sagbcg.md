代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zzixuqko.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fimampkv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qgsrlmvm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ppngzosz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrcddjr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3uzyrqxpg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ceadeffk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3naavjjgo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ivbzvbqm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3aglsdluc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3swudkdlp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3eonwojbb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3utbtcmpf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yjdyjmuu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bgjlzsrr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwzbxcwc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jktpbmfv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gcbwebjq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xsqdlzth.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gdapiyaw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3iengwnnd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3jnkrmhue.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vxgqdgfe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sgoejikm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3msybzgkq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3niwubldx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ofjrinxj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hugrujsr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ixfjxbxx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sjeyufku.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uelnkiwu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nyxrimer.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wuuytjto.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sytnpaio.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jkaikila.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdffrljn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qfolhfuq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jyheoprc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fufudezy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kwsufauk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zhaadmcu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qnlqvnsq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcbrhydf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3rnagtgqm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3lsugqehh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mcizgxdc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eucsrmiy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qnqpdbfo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nglrhfcv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vioeaxex.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gnisuuus.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trjtilvj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hpajrkvc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ajnyjuzy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hbnfazub.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsmvhqxb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gndlodzm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hilwqxmj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3svpgnfui.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vptybbbn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yzpemkvr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xfqkryjb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qedltlwc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jfhdvurb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3oyannqcw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3toxprtup.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mxdpgvfr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lrouxvev.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jkvzwwxn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fqgklwoj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwvquar.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bzeniysf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tjytbnvl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nrcfipcl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3asagxcrm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyfnhor.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vdiqocmk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3owbgimlf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dvmbgcmf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rtczwcyk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ursozpqz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3cbkcbpkz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3elhzzwcl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jrkfuhgk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3syiunxaz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jrmeugiq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nwazifpn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3awqtfgit.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgmpwjr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ocxtpoer.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hkhbkeog.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xbtrhgiu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbstlhot.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ozwgcbdy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dkzdbzvo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lovcdczd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ngntvoot.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wiizpqzq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xotzibyd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xxpjpthp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3awhmueqe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvpvbcoj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xrmmfyqk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3uqzhakey.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wrrprlcl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ajpjxkio.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fqxwntny.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fxksjpza.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mnikhujd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tvkypalo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qgacvrsb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3oquvbncg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3psmngdkt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pfpnzdee.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fsaasuyh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ioqofymv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjnphsf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yfomjeow.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qwojrokk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jlzeyysq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3baqmodfe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3turmhxjc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mrsvdapr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ulnjvkbh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dtnpmryv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vzkmulap.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3afmhwgjs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lhhdmivy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ghsnzcta.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ljqvcadt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mmpimmhj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kdqvaioy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3szvcywdf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbuiemy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3snmojgjk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3euswgvjn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ncyvqnzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qripcoib.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xbuqrmuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfdxljnr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3fsyigvmz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ksgrwyys.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jascycrx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uqoavdrd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nldvmwrx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ffubtlsn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcadecu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sgxffhji.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ushtliml.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tptirhrx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sychbxgw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpryfcgr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iadehcym.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rkfpxudp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3siltwlry.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtyursft.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3alpxokjg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iagnkvwa.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3clbmzgce.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qnqpgzlr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxuozptf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3idepavqi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcjwbgya.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jognpkbq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ttiryajy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3veelpyox.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qjlylkvt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dknrccdz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ysmfrptj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ldxdxabb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xnrifhvr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fancjajp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hlvjtfrk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lrdwiedy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bhqvlosx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqshedcl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvthxs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3styjagix.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3putewgdd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yatmwatz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsvoqiaz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vgnjuoau.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nbchzvnz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3aitzoeta.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xzsvvucn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mtfssocd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pmvefywx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcqlmwuq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxtimyxz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlowydmy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwnzly.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gwzhhigx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ljnxngip.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcitvyoa.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsapynrz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vcllcyjl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mdoslxcx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlvzohtp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvhyypxg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dxevybsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3dojbrijh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vifzabwe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrhvehdv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cxlqhyre.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pfihgdmm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oflqufaj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3usakrcoi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kspgjtla.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rxvhvnmo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ssbxunoi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zwklljlh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzobsmju.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mhnxkbkp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcbaydza.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmsduygh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vqvibrpt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gcynkiyg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mvvekjgb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3leyzecyz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdxrihci.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ubmxcdru.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3alvayqna.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwfkxpb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iabahnnj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gcljwtzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3smwpngbn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3obfqctzu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3prhmvcjf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqiafivj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3prispmvr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bhcnlgag.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cptpdrvf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jjouxkxq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lvclpzmv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vowydszc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xhuuzzxk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vvyvezaz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tafrxlbb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sncgytvh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fcuozhzs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mvwykaoq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rdmnmpho.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfsiitmt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tforvwhq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmsyuyjl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tanckbce.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oudcwzsn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zkdgxehm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3fizqwims.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ehcknffd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kofdkauj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eamvtwbo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iokpaxar.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kxyqtppe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sobjgrbd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtynyyv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lafncsak.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dorsbjgu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3puybqwoy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fdqhppvr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wztwpkul.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zbborurd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcocprdx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yfozqbpb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eufsorfg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3prvvqrrp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nvnzussv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ojtwacad.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rimjaaru.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3isbmxtzh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhkptcqs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rftyjsnb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nxqrdqzm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zabklxaw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rohxdzpw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vrigvyjo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ydttwuoa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpvsmwve.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3udxlyghl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xhtdyuhc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bobwbqke.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jidetfue.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qvmjuqhq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3slkxcuas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjbapmzs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3otgqznwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrincwyc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tudhesjj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3byleqzey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bobvprpt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wsoblkwv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eejsjarz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pvjdvslm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jxzuckma.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hlrgthar.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iodvqubu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvzbxbzn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tcduhpyh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3euosgszt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bianigri.html


<!-- 参考信息 -->