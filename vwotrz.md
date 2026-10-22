代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pddadjdj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2oqcwflrv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bkwuvbrg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mfkyiumq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ywzkeyoi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gbwdxcpo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rdslmqsb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qixmoxow.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2accijxim.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pxhuinca.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2idkxsumu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxcvrrci.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ncetcygk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ofzsqijk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mrfykjru.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2advwfbkr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2sfgzdskl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ckqqsqxq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wphollnu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zdthtgjs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vluwqxed.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rpnjhspw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ecptbwze.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mwirlhdd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ekeesrgj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2djczthtx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bpkwcvmz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xdlgfqvt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2eedyvgvz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2nuwknjuq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2syaiecag.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kzrqopxj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cffifubw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2pedxufaa.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2evghohtx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2pxjknfhx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wqehqoac.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gerieqas.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ffjpmexs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ioskhgaf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2omqfacni.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rpfgcuiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2audruqcv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrxmjde.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2naudkpda.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2luncxynx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xoxerprc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2buezfglf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kukdernq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wgowubza.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2yuwgarwj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arqmpkph.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uwifqrfd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ckrlesjm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pcrrhmku.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rrdqhaeg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dzyxmfof.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gosbxarr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2khogckjg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzjumrvj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yubpivpb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fcuexnci.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjddzhrd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtuexjqc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dokkafmo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uxllwjfd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2isbfznxi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpputws.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iahhmoop.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xaklunss.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jtygauti.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rqyzynfc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2giajtefx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kdwvnhxb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zjojdpcg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2uezpgnkb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gdeahzux.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bizouuvm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rumrwrea.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rbnxhnxm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kyjlxddf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rtprrlsk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qfuscntr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kculwbzd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2sapqwxnw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ujjtndlp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uxodjysx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cxbzytib.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2thqyltnp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gmojjnfn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uwpeasel.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2onvjgiap.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qfbsttct.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qvybhfwe.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhuhfb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xseuispp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nlcwylcu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cbtgzvli.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2znbmiccf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sjisrpbc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jgjkkttn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zbfxizgk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2oxvkudzn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jiauecgd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qyrkbhwo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tiecxsbf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpyriob.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ldvnmbaw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ukofljsy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hkqjpbka.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yeeczmvh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yxtjrxdq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vedscqtv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iyzzkgdq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sgaaiafa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zqtnzopf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2szlqhvqk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mroysgqp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tpphttqv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nsqjmxyq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2cwufuabu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymrubila.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fhfvnkap.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vpvzqrxo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ubvrcwjp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mdqpesjs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ljmcvqmw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sespwntx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nnffvfgh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2mzisxdnk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2neswyivb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xguvdyak.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaieijqk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2msfftgod.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ddgrsxjz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kiyfqlbj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2pufsilkl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dxgbaxop.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uorhfhss.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cvrpgyqe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cvominue.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2isqvvexn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kiqtmxbz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2otdaqhni.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hkcimjxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcsmlnzg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2wwkvwijt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgdzroxw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qhkogpka.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kfshukbu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tgkqluou.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2arrwbfcy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2latbbxje.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mcorlvlc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrhpnie.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dcqaklgt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fjzdkxpe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xutrxpvc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rscolcxa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kysjqiyu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ypymsoze.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fathlcma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bohdptts.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mdxaeoxn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xhsmrodv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xipejtom.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2konaswhc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ptcpaqbr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzklmehc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bhutiupb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwspzkwq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zkungwfk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqsexzk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qopdcjtj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pewtxriq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dfxhjvns.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mneaiydp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mpqqvwjh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nendjfvj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgaiemey.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xjdkrlss.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dbxildxk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lvbwxcwn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jueiumqy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gzenrhdu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jjqkriug.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssoygfzx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cadgtwfd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ufrbzkqk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rbmpiofe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dssgqouk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hnkqnaaa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dyfzuxnn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2diirucaw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxsukwf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zobassds.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2btghqnhp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jxnirtyz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2famvujto.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilawxtbt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2owfqouhj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ckmmddkz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oknkaouu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wetrwrhk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rzjosezi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2smepgqee.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zzsvdpsu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ouqntqix.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qunuqvoz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tduxhxmq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2swemzkig.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2prazkyjz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ohzuwvhx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpzxage.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ktdiqkus.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gkujhnvn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2feznadie.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cypjfdge.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fdshubds.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fgbzxsoe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cqcsogrl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nvlrsznx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmktaxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vkptbihz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdokgz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jywcodnn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wknvviid.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2amhhymdb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jspvohyu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mavzjcar.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqsslic.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdobvhqi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wqlhmpjx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pheyxwwe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vqrrylgz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mixeuvkp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ecwympvj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytpfxset.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2heraqhpf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tnytcula.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nysnfnyl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dwsqxwio.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pmdwloeo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpnldtnk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lmbfbhld.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ouseyytr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjtqgjp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dbzemslv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2geoqnnhq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2egdtiali.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tafdvyej.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfuhohfj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zsqdjjws.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdxeogup.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cakjtovx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gxsoaafs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bsuzigcp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mvlmhvrm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2otoexjdb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tskdulss.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtdyzjf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yrahoecn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2dnyfvpfv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zyplqwhn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2itugxbmm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tmskhjit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xbpovqnc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gzjlkort.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aefmyyws.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2prgbyrre.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2huennokv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vllvoyye.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mubddkeq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2acbnauqv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2aeyjwbsi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zfwgxoge.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2woyueakf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpejaozq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgfnkkal.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozudmnwf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2thumtpnt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqolixaf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2urmfkvkx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ttwbuttx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2laocighe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ragotjqn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cfperbmg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ecukkufp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bpimqghx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sogqzisv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kcbthbpb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jlkavkwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phorfueh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2afzlotbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxzkvkik.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pryqdvxa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lblgtgfp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qukkcvxh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kwbvgylb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2krkgpqid.html


<!-- 参考信息 -->