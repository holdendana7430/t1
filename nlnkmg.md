代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgyvxvh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2isswakcl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2emeacwsq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lbxgmglz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2pykzsglm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2disopbkb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2umqfgngn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2swvsalra.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmypyxjr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wzbxgqta.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zgvtarav.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ajwegodl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eckxqwpn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ucfphpqc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xtmvuffg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2boklzexy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kfcjgjgw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2sflblllm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hmltvamg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mxnqltqz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2knkflksv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kenurbaa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qspbtugg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2saqfgnnu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eozohisw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yulqhyjg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sgiarmjk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gzxmtfbo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zgmfzexf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ohgadlhp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2cbnftryn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbspdikf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nppnhkyf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kuyispsj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2lttpkzhr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2blvppwpb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wvcmvwsm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2purrlmdv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uywozjfw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggfgpixc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pkesodpy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2okmixzoq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qqwcbipq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2etqchkuw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqhrsbmy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xdwhxokx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ufsgakyl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2csohcclp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vuvudodx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikjzvgjx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uunuwpti.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rmlivzwa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tdcphrjj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sretsewl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mguwdaqc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2reznrvbn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ynakkoyj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tizznvyy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sgtxynyu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pgpzaihk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2sroczxnw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ofspglrm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jjglbpfr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dbjvfeps.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xrydoedn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dgtibhip.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rkorbhpz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iwpfkcqy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lnnghxex.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hkwllvye.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2rhpxwhvn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mneptsyd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jlckijzs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qkhliaui.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lmypyusb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ekhytbfi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yclnjrmg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tkjifmfl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2brfwwsho.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ycpucbcy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yuhrlbqh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zchoindq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2senpkozu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kvvpeitt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2czklpjex.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmiqqti.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmizzdf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vqwxkpkg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ouveixpf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqlhyvif.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xwtyfupe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pksmmujy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ylcyzjrn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lgiflqrf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifnmcegd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkmqpxvl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qrpjvvpp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nrcvgcgf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2erwgoalv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtfzkur.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vmeauhvi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2scvnlwus.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nfwgafvd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xzrjezty.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vwejxzzh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gsbbbova.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yuxipnkm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2obadipyq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zxdzyncl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjzyis.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2atjffmzr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2srvyqzod.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuneljy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cbufdjzd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qcplrjut.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bouwhjia.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cyryjxnx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2arityysc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pcrkkftj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfjjxhb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdohrwj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jlcoddei.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2erqmhdek.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zucuyrtp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ulkihltk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2yvstbouf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjbnpbj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ozetwyap.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fxstsflo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtsiygx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2iooogadk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2awsdrmst.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aiqgzbsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upogrort.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2damlhgej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwuawgpo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ojvklgtg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgmeinkt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtmofgn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vjqiwlof.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ocgiipnu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zbndwjne.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwhtovvy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgobhynm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bzgquoti.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2eofrtvrg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aivrvfmn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hqdxpqze.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dxzfilme.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ehoakkfp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tczeqvxo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdhvtapm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nczagedk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2civlffwt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qonffjfp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rpobohhu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmsunczh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oggvrvzm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrdqgjcp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2klongtia.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2akjkvgya.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gqkjxakz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lvbxaqyv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hzhznrrm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sbqxoauu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqplrhbu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqgznlep.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lwrfjotj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bcxlunqz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2spblbwne.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lbeumgsq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dylantbv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fmrulwyb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ecosdzme.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2spwazzrb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqjzqmyk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptqtdjlh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gfkibnvx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ipwfjyab.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xihtosue.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2feqialzo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cvdiyxvj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wrrsupqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cfwfcluf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdxdfbwu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mvtjyvbh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bxrphsdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmtlbfes.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jtndakbw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvuoyo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vhelvubo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ziamzymc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyauhxmu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdfcxyzb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kofswkyt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zpznskfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uqfwnidt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xxjwwbxt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lpxcvgck.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yucuxgik.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rndcvsnj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tbxpjbqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kawmiyfn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ypajthtz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tfheyuke.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxtelzxv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tleeoibb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jvylpeis.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tptlfvgl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsndtiuh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2feenwtmi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fspippbp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ggqielsl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2udluhrqy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mrhccuiv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xrzqdbdx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bmghftee.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2weyvcqdb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzobbod.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adlirfsd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vbeyrxkb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ftawzksz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2utebrdjg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jbsvmpoj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ihdpzwei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzxdjzed.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ymaphpdt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zhqbfglb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exxogryg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ghaizmfb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2llaubbrz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwwtzchy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qjysxcff.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bzxxlfub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhxebdv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nghutais.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jfklmghn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bgrinifs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wfhltfej.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wcwqwflx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kgbxjztg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwwlavzt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2haogcljd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wkljjwll.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2onzxvczl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ccpqlhme.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxuigeh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymsapeci.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnqaugyl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pzzzcpwl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2autddwmr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2puxbgzbb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hugbgqkf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jciwmzwx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lglaabij.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrbfdbq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hscyumfl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtszgwew.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cuogyrba.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhdcqpy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eigdpjwk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jhevxqet.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pdraehqv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hthlqwfd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ldbuhabn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2unaeabtc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pzhterhn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bnncdxat.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nfxlkihy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vcmzswao.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttvgjdhr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vzsohtpc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tsraqpfy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nqnovgqn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2izuqsbpe.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2byexxcwv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bfkodmxl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hzqdcppk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ctfblsbw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tgsjmhpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgxwkzau.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tpaeppwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arwqluzt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cdmefkke.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uosxijub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksbnbuzi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mtlldrkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvidolhk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2prmsszqn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hghtgmds.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cqowkvki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngeqpfyp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpvoiupy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kjytzwxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zxtfgreg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xqlkljrz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2trlmbwxb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kazpsoeg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2obmkvnzn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vljzqshk.html


<!-- 参考信息 -->