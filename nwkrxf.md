代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mnugzgtr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ttgghmie.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2twmcohsp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kmkrjqjx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2umhtmnyo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bhntcbyt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gexcwhec.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgicoxul.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxylaqi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hibfwral.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tatkjsfy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbzanyi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2uahovpkb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2svhbliwi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jceppxxr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vdlvtooj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zydguvwe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dsvpderm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eskdqbwa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ubpowkvg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jvydehde.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lfkwpbld.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ymvoggyq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nspqlxwv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xklrtpjh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xofupyig.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2redfzbfg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xoowmrrv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxsnpqyb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wkdrimjx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ljnjmguu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2cyqyesnn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nkkkhjzv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2cbrchovf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fyfbxuhs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gwkfleqa.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kvobfdct.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pjcczkzy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzyfwvu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2sbyrtoqc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fbvjlchm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2osbqiqek.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yyuiqxtq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2txlcywhp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fycsizze.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2njiwhhjq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quhvkkgv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2magethbz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vsoeihaw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ykkloofx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2iasqbzxe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ggzbpmyh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmrafnkm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmapchiy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dmazvmci.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttnltzvc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mrkrvmtt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjkeocgr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjkdgzzl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2elbgxybz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2urtefhok.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lwlzkyvy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wqascpzw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cskhgpzw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tqjufgwj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hofylqjq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bhtowhvs.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2tmwxydgm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tpursgiv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wrrsbfxc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ftulgjgd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lntgamez.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wzptexwo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ileqpwcr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fwmycobt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fpcssetv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xgvxxanr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2issqwzmg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vkidyxdd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fadkjpni.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nkewyozw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cqamhzgl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qnzfplof.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kuzstiyw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfxcrbj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2pnpndvuu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yxvzcpkz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tgynzsrv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2plwcalso.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ftypshjy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xomepapl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzjfndut.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vgqnwicb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdjahzi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kakkirki.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2tnqgbptd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2digtzpgx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zqxbqdlq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ioghuxuo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2okatngfb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fymtnblu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sxcdxwhs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2joggaqea.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ejubmmvs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xuxguvro.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfdgblwl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cdsqzeye.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2iyadojsm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zqtqwnva.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gfzlfpgs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zvgxnvsx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vvgunxhu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jzsdpfez.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vdrmtdrx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2luizzbnb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cxzoxcee.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kxrrzshe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2omothtkq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nbbxyaom.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qlkliwxa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rcscebpc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vmsoawqa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dsqwtswr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ojficqbo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2trxnywsq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uejjqdij.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cgoooxwx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzmwpktj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nwaxuioy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zqzximbd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2swsakdle.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rbvjbpiy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xtgtemkz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qsethlor.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2szlgrbec.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2oyggtrhg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lbtdydds.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fulmcvkr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xbrikmad.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xlplfckg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nworjhkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bstnjmbi.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hgbexhop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aotfvafn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ahiqyvoo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2erebcmqv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrhbataq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2owsjblio.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wtyptnum.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bewesnuq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rzpjmcmc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uaoxwgvc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qikvluaw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2sfxanjap.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yisctunl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swlhfmeb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uxirqwtz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hsmsynom.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2odwueklm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fjhyzabm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wtihkygh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kkmwmnsp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mqdbgepx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2klzppqmr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iynmahej.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fefjyftg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ldaqtsuz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsyvtyly.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vbukcqfh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vbyjtpla.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nooomauz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ionfacbu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ucoaglwi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqbswdo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ivmvctud.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zoqhcyvh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqtwlbns.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2emgcnord.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbrlycz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wnkctuxk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ccueqxfc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtkrvrc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vuurvumj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2evymnwng.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sqdqsqpn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xyogtdxb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ltipfboa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2grqttsgn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cvtkmchn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2adamtngb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxstbit.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ezyowqrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vexpplgb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mhmkueiz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2djmcmzcg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2oqhvzbcs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nhrqmmib.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eouffonf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2icthwxtd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2llwyvffe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vprfwqzm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilzaqadk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tewsbdir.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jtcstcyq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2aylcusxx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gavdqjpw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebonqhec.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zxkrdwqi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cwnpdjzg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zkyfrzxg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlvglzj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2phbnozio.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2crjrraqw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ohuhxjcg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2prsspwwr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aotbdacv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2aefcwnbv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2isgrtjxr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2orpzdyey.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wdzuajtk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bzkckihm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgdtsdhm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jnbpvrra.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pwrjusuw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xuzxaubs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jjkkcwlt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rekunalc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjygpsnh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zevchyxo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kicpjrwb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddssojfd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dhnrwsjk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yhlcyzvn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dtalynqa.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hcftrtlp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iouvazpv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2outffogq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbzdahzt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2heliuebf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ioqndfzw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cdxfexnz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2myzrhaon.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tkcqlcck.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2efmvetem.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2egsmiiip.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2otarjvdo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2womzxafc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hghewwbi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bnqjgfiu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xfmmnozc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2furoginz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bkoqslee.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gjlycgfk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jmwbevcl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2knzqikmb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdotywms.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2poconbka.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ghsmnief.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2aseggynm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pvkvrzte.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2llkatysd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xqvunmdv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2curqneji.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2teutjsdb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzpxaej.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywtlrfwk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qrfpnkst.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwmfdtc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kdloxxjr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htkfzpfn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bfdskayx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tiovinha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2csmdguwy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2thxhwhsf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dmdddhio.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bhliqxxn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agmhdvty.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2saxtdlob.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2owltbcwf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fnjrwgjh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rmgwinse.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2khzvprfd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2igorkmnp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hvebewaf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jkuhohzg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2outxcayo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dfpzwnbd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ukeeujgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmeqwvqk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yygbaotv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jknxbqrt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpmatubh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oleqcpyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjkotftb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xtpqlklh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjkyexu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dccxakhq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gkdtxzus.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtuxdolz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvzykshc.html


<!-- 参考信息 -->