代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qxtoioyk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2plbsedfc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ngjeoyfp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2lukxbgkt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hpnxrvet.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2arhbksnr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vupayydt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2azxchxkq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2sbqzddeb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ummbgbkz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ugtzdxgn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtugupp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tujzxhvz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zczndvbc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nfsvxbue.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2uayngnep.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mtfkxpxi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bqlocdxh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jzdqhhnz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uollhqtc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxepsf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rruebrll.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwrfxyva.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2evyxbktl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2oayhnrnk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2earaqjqa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bkqsaikx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxqsedop.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tjeuaqtg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nbxqisdg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2heelzxwx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2myothelr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gmoyltrb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wmmlehfv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ajgtbpla.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xozugxff.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2awhtaaum.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sebqgvda.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2aojolauw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbqokw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lsvbsaxn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wjeebihe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sqimlrur.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2rdajopeq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dtlqyulq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2sakqhwgb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihxyajtk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jwcivrdy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2bdrqhjrp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xzxhndav.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sszaivih.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2znwsfqjr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ekmnwiqw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bpaqnmrs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdopnojp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcikihco.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqolqzwt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2njkqxrvq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yljuvuho.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2inemyxbu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wdoynvqy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vsrtpujc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxzcoig.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ynblvpym.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhyzrgz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2nomyrkyv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2przmutji.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xlkzwvwx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ibvqfiee.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekjklceh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rpuwcojn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zqsljynb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wjpqbpdg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cmprkgio.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2gdcnhqoa.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gabclika.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hprsdslq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bnlfvetg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2tuexcgvz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jwhbnpkf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2knihqoqu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wlrfxyvl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2odiyvnnp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pmbqguqm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wennlixt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wpfiqocc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ecdvoscn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2miesrvsf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2meaitsrj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ztqirdom.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tvndxusq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kgmuudmv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vygpxiyr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqmddck.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fbsnkhbv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sdvuggqq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uwlguchq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guwvdisk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2uybhkvck.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2iiwuykxc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfkmjgse.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bdtsnuzk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qafsarqq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oxpkiguh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2egvlwmby.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydohnnpd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lvxektzv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdnjiec.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bqilzufu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhjfyob.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zmhfymjg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2huvyfzdl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zzouddkh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qhteqluj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2stcadqzp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2byhqiztn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2yrnudrnb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2crhhkpwi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ryjcracx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pklaafgp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvndytcg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iikudrkk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eslddawg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qietopbf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jrlhwoxq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvrdihn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sbrzgvsh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bldmwzcp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pemlerlq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ekuwxgij.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2uyljpmdr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxxwtbf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qaceuzqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2brpgrjcx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlbuoyp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qfffgwjt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2hegfbcdl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tovgyocm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gveoghwu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2onriahdl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlosnru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igzvjspa.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2scupksfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxmgzwgo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xwmcovcj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ffnzrceu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukijyrvv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oanfxjst.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2douzpxrr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aphfycmj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wbhdrirw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gjoybczu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lwizeezq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kvnejhgu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtggsib.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nipdjqkr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ndtxhmug.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nqbvttal.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ozgtnugk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2burtnsff.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uobisyvt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eyzqdyht.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ndhvnsys.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yrhinqda.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ajffhdga.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ujctwked.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bodrgegc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpurehjb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwadohe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nkggtuwf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ynfdcozc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hitqfidr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wscjorbi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jxxldunz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnrucul.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqafaatu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2buegybcr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qphmwwuw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xmwjstxe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2csiyaqvo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fbqwevfn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xvwcitmr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2glxurfpx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmphlluq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnrzeqto.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bdskeoic.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsllfpx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lpeawrix.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qnguwths.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mpdkjagu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hywpmzro.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dclimuhp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aoqyyojf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggdgtmpj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gqworapj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2utldaopi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fsetblhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2euhjtlmf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wpvfvbjt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsokkywh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rqapvzfb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvffokud.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjswkfxi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfdoiawz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qfkmqvwb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xqttvlyp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2knsgzmss.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fbtiwgvb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dfhtmkgh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pjuatash.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfscgnhf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ayexhgwb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ygwzbfsn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zslywsjl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ykmpzowv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2afkvstwt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ajepuigo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2grggsnyw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dslsumrl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eztpndqt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2crtpekgc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vvuitenf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vrdakdqx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vvcwzppx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fpqkpkuk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hasxzfyj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xscscfab.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2iniaearm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lwjdkxjb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dsahdvui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dywsgqbc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhvnoajc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vugatzay.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnepzstc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lcqfctfr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tbgwmzbd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2svvtlgld.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qgdaizzz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rnkspxpd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrfhwwsw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vvrgzhyk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dnwsvgsv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhoiwtg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mcfiwxih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pdiqjmdk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2afexucpv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dsrrhuku.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lxqpxusp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hyoeafgc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2evmtftrb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nvjswdgc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2swyproyr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tktdveux.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2moeoszla.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwmkadc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyaruodq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvbripsu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fsqljhbn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wpcydero.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qwvoutie.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cxgejxya.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dxlyhtmy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zxppgsqy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dhvecfri.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vicqnkex.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzwdpkyl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gghiudyq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfrvdon.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkbdokn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdwtonk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ulrgrtoe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2urhppcha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2spzkdxam.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lftnaatt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fkcqjdtp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ddstghlf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ajnntalq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nijfpxdp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2skfygukk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zpaznnju.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hhdpvmrc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yygrxwyj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2iktotrkp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2psmoqeha.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fcrphnym.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vpvkbbaq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2icyqrxnl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2heeycmkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nptybsdw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yddzxuvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbzynrbc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2btuefjqw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jmqeaqlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qbwnpdnc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pdxqhwgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pfvrxcqj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjfpcghy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ecqxpcdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ticlaupg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mphfsyty.html


<!-- 参考信息 -->