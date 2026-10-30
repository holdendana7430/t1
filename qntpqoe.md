代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/goreslvud.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/ggicvkkhm.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gnmbubhao.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/ggjiactty.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/golpskksy.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gdrrcgvoa.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gjdsxlvkd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gyrauoxeo.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gctfdgced.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gdgfjlktu.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gyzkildom.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gtoivycll.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/grxnfklrd.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gtuvderma.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvhtevugb.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqcprml.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gbdfomaou.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gadtrujvd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gwafwaknj.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gsyapmeir.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gkyfohyrn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gtigotobh.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gxntbxfic.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/glncnkkby.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gghvgzffp.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/gvbviljmz.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/gfpmdeqfg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/grfjkizcj.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gufpvzxks.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/ganzilezs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/girvntvfc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gzuacabyr.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gwwkxofjh.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/glvmthgwt.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gpccacrgf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/ghxntdlcz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gflpdkxao.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gsxipizhq.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gflxcjjdr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gfmvjmgox.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gdbzowwsf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/ggyzyetmc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfuthospq.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gpfzuzrdw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gckjbytmz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gairwzeuw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gdelrbkjg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gntxhtgrp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gocyhzgbr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/glbffppyc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gqimhkgkc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gozljogyp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gytpcsgcc.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gujqpuqxw.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gqzehhsvq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gkkdymllo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gduejzumc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gfmntaujs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/gyypjzydk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gtscrgoue.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.hesvh.cn/Article/details/gqbvvashs.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gyhgehose.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gzporrsuj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gknmqyaav.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gkpmtjxkd.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/ggtnbydrd.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gwiswsxaf.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/ginzsfvrl.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gsrekgmju.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/gaizslzhn.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/ggkzjjzsu.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/gahnyhtjk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/ghpyhuuyd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gmrgkhlar.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/geegpzija.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gkzcmxuxg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.hesvh.cn/Article/details/gnrceydml.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gwksbrkiv.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/goasattwj.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gyrtvbksg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gwsnlkdnh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/golpgodwc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gtpiwcyao.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gftntfwud.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/goosqzetn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/guquyxuyn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/ghficelnz.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gwsqrytjm.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gauzyjhov.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gikhzduya.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gdnenfmyl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gpfpbfmpf.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gmogqvdqg.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/geyyckcxp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.hesvh.cn/Article/details/gfoigsjov.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/glxpseahp.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/grwffbhoi.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gocneoiyh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gvhulrivv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gwdezqkmh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gghkxlndw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gwkqtouuv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gdreblgbk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gwtwhxzzb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gvmlhoydv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gsblwyvxc.sHtML

[A24] 去除首尾空白
来源：http://read.share.zdbjq.cn/Article/details/gutbbnlkx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gjqqkrmjl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gtvpqyacb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gseiazvii.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxscfbfn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gbbrslvbn.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gvuphxsuk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gsyuowjlx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gzhbyxoew.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gdgaqfpns.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/guontyutj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gqnjbxbfg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/ghmrvwuys.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gjygrldjy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gtujwemai.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gohapihgg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gutqjpplh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gudxozqah.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gjteucjeb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/grcetguqj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gsnbhmfks.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gzcxhwdmp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/ghrryyizu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gvkzojwkg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gxoekdmhf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/godlfvmse.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gnxyatqpf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnxqycftu.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gqjojqdbx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gephpspkr.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gsnunxbuu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/glvzsxjzo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gthwgezuo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/ggxhbjixj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/grjjlubue.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gzhezzlqr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/geacpsmlq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gqpnrfryy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/guiqsqdvk.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gsbhhicsi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/guacujojt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gdrgcuwou.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gvtpabrvh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gantcytiw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gipbiddgd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/ggrcyzdwk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gjtitdyla.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gymsisoyu.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gfnrwwkkx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/gwxjdjmpw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/grfzegoak.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gweblbuae.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gxwwgblzu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gvgwhkmoh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gbvprezoy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gggfqirqv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gcxrgtcce.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwiosvkzl.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gavqbpqna.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gpkcqsznc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gbpgylbkv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gpkawzerk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gxybhftjk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gmquplbwp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gokmdreou.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gircdfoqp.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gvidwrjaz.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gxzfknuxz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/goirtjxvp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gfpyavsbj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gycihvizu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gxbaiknye.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gzdnjjopr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gufucwfbs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/ggtsqyqcc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gbblihzug.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gsxmzegwr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gabohhgks.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gfflrgfqa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/guhlkjqhf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gvbmsudeu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeteohnm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gkcvjoezl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gbltrecwo.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gnqmrvdsn.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gfwskuaey.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/glgrxaqac.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjmfwoau.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ggekzivuh.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gwachdtmx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/goexmlvjy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gqxgqqtyd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gwxoyyclk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/ghssijuyf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gwhvfnyrj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfycrmdum.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gkpfgyzrv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gjenhlpmp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gkbxikqoz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gphumcqni.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gytphttbf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gfhkxdwwc.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/giogzbgpq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gqcfraslu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/glsyduazg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmxzbxdqq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gyoiadiaf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gdzdwabpj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gbakjuldz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gnktchrdb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gnqtiengu.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/giwryjzse.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gksubzdej.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gxqteyovg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gvjfghcpb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gjzhaqebt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gpfgjjena.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gmjqkauym.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/glclhqymg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gccoxfynn.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/grtavmgmj.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/ggabeelzk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gfutpeklo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gfxwpamjf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gtptjgfau.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gcvhsjwmz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gslbgtdxr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gcroviown.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/ggheeqrcy.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gxzuzsigb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/glssbgjwf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gztwlcuso.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gustxvwjt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gicaycmoi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/ghqumjvaq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gsnhoihoi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gjwctnpyn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gvkqtcitq.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/goobbqqfv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gnwrwjsxi.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/grvqedqmz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gjaaivrbw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gasjjzhzh.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/ghnvpbqzf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gwdghhroi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/grlfyuisj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/grhezmpve.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gpqiyxwzf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gdxvizekb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/glkmjmkpo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gsfygtood.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gedtjtbmj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/guexhchod.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gixdmmsmd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbmjxmtao.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ghtwbirqt.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gdleznyyb.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/ghumdipte.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gtcxraeok.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjynxsxpq.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gizugwpaa.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gsnohuogz.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gpavpsdiq.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggrhxftxx.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gyuufyttd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/geialmllm.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/guieyxrzx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gmjmxmeqf.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/ginybjgew.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvewsxqpa.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gdphhjudj.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/ggoqfyrnr.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gyhefcmua.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gprzhmoex.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glmcfkwux.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/goifheuvy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxioqhsbj.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/govqpanxz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gueumqjhu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkvccfkds.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghnuylhhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqqciufty.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzuiibmxy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gtakzwlwx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gfrdinnqy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gslhiahug.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gmshrggsu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/ghmxfsxkj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gblauxtnh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmiybeufk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzkxmivtw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/ghsshjacw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gumnrslcx.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gcfcjfnrx.sHtML


<!-- 参考信息 -->