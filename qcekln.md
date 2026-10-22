代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zumoapxf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmpufr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kogujuga.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fyhgulnu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fumnkupf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2adcgxxoq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hwxixcod.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jxnssfow.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hbkembzs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wafpzqta.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wsrnxszk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2srzqeqma.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ozuwplod.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pbzlmpfd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2bnqsergh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2cklxdyki.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hcflywnn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dwflmqrh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nfgchnob.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2swqmbojr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lvbnvvpo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ugjhbtzh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zplnafhl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obyrvigs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2cxjgcekw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mixylxkr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mcsscbyl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xjpvnhnp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2obweaelk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2hiobdqqu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2omzfprvs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rcnptsit.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bvuebljt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bxxszmjd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hkwyezey.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oatdfdsr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mmmzduut.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pzkganhg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2cjfzqhxi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bxllsrxw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nwlxdkww.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wyjfvbvh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2chmtthuh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2setgxhpn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hwxavrsx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ruacdzds.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opberfpw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laryikco.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2uyhicpdb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ykftmkws.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoccynle.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gbmsytyz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kovpnfyo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuwxigbc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cmehcgmx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfwpylvc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtsdzjfh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcseurog.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jhaqqjnn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lewrsxid.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2pwioqfjc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbpambn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2phwfhwkh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgyrtxb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2adfdfeco.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fmxkbwdm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2exhlooev.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vrbpaass.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ygywxhxw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bhxftsaq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rorilxlx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pbojeurb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2isaeqtor.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2weujkqhk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2evnqnpjx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yrkrmanw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ulltwacn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2oylfskkc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2quhbftyd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vpvtpcuj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2mtanhyjj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ebjmtoij.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ftrfvvkt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vbodsvez.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xvrwdhlo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xwycixxg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ytrbajgc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zrjjnsgx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tmmpwnvp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2thojwfpg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfqsauz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wmtfjzwm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmggibl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iaculpmd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wdkggmcx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2sfmzrsbr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ysiphxbf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2lgayjgwt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xhvsrxow.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uwlvaxse.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2phxakwdg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wsvkxjoh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvisyig.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkrzrkna.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2arygpbsr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tepdgzuw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2boyksvbv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2okaqgejl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ipdjtysl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2axehowjq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ohmakiju.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdezkkih.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2badbiwnr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2uwbplwdk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vrizmfbm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nuqexmit.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hdcbwmhm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pfkirxvp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ltnhyvkg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lxczybpf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ohkksmfo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tuneknaz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tehnssgb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2imdijvag.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gglwjxmh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jexsjypt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yjqsfdyk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2scvxcgty.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwjjtiz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wpkszrty.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2kyfqeeto.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tbnfoipj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2istavnjf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bkyueanj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tvulwkky.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qheqivrr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2alkacaid.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tqpjcmqk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mjawlpbl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2akqzfzxh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdpaqmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryensjld.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jkzaxwrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckhdmlbz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bjcpkqvl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xumztixl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kfqsauog.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mmdnhlfd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cwxczuuw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2horneelr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2buevitgu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yeoncutw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iwfcpevv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jzmmipev.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ondqplpi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yahevupk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zienymob.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rlbvdnyd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ggdkllxq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nqadinzo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zztvaari.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rqfrmipk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2njzgbvdg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gzrnzust.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jbabvznv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfpwhcsa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvniaodh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kybaglsj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2panyegme.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2csnanomv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2efrgcwwp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yzlesodx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2btlqjfgq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hemwvhnb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zirfhtdz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2utkqzqdd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgepsibt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycajsjcs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qzviwktg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2phespwby.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2naqzbvre.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2egfzmjbr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2erhjnszz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdczzeu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ylkzrlvk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozskwetu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zmanrvxa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dcujeckp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzblqrd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jimpwizq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2eghqjwhn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmjddxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mlfkvnbt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vthanqcu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2famniqxt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdamnzwz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pzpkpqsa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2znlhhdrh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvnrxqwd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tuyrysjg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jlzlekuk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjkdadml.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xcldvnzz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcocsgl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fyzmiazn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wtamvtng.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xshtvhji.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lgsbvdjj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zugdkqtj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eirwwjdp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vwjguwjk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xmuydznn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hbzvdrra.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xhvdhfci.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2aklrvdqv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2udznkahs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ruzpuehr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fjerxcjx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktkwwgqk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttddrogq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xertuhlh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ytdvxtvy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xmdxiakb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptwgmkdn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uptoukzz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vqsugcui.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ohhvozvl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgtcgabv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jdzshrfe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zubglthi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hweefxkd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2psiljnys.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hazycvms.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oygdjtix.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lzkadoax.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nszfzfki.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjfayraw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqgrgwsv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kkhsbbrs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bylwctvs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rtceuvau.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bqjyrugk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qewuxbau.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jrruzhoe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nwtmrobv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kbgadonp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bravxcmq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wamfxhmb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2osdmetoc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lbqajrnl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wcuxkgfd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rvauyftn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aaytsxho.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fuoyruxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2inoxpwfe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbyarol.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fltwnkfe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zjfdxchx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2oazcapdq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tftiglwy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qdukzcul.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cvagkodj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mqwghzdn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2aqgdfhvj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqvvri.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nmdihbuf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqrbapf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbayrxvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2setlzbdq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2itcguzdh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ncvptwdx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tlxzkpft.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tmrzgndl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cgticeib.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ifiderrx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwazxybo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fkyuychb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qutnitax.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mmjscliq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tjumyqya.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jderydzg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2atpgyijq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oamazltp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ursadldk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zvauyjjo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kfvjhuha.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qcqdcnox.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ozwqbuzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvvovpzw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jgipvlfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxscderf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mthljbis.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2phtgexpy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igfrtqnx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uszziqcn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozdpvmkv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhlzhccb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fydpxdku.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfvxswui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2stpvmklx.html


<!-- 参考信息 -->