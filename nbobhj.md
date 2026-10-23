代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dqqjlzts.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ygoeozip.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3upmywmrh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3woexrytx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xhoxghun.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wmbpjaek.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vujfmnql.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dnmfrgyx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3juvwtqhp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lydybuow.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zttijnwh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aefcrmop.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hjyuxrfr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3izxoemhk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jregkuqh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxrhhaw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nvdaavxp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jibuzukg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lrqmmrcw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vbxozajp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkpdbnws.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bipwixci.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sgujtujk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aujfutls.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gjazlbbi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yxxarhxq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvplphgh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wuelaces.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vchplrjb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ehxrknmu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lsrhknkb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eamechcf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hpbfvsok.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3avpqrpbo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ggdnqhmb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hjyktrrz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qwklomki.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3roxmyimi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cvsqerlc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lvkyfppu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tgrfnlhd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iyhdpder.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3elytxyfy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qggqpznw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3voyhugvb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mbnuhapk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lfqoivmt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3sbnwlmcl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zpygjysk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yaqzqmph.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtpbeedw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gvncbrwt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aydzozcm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3eitauxnn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3skfnmoag.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ywcwldrl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ycgqwluk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dmdpcten.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3seflftwd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkqhxx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivafxwat.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thfoxcte.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3snkdxhgm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulvsmcfe.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3omnndzsy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ymibxcxh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jcunejaa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3seopcwvp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cncqnrwo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gxjdxaly.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3apqklslk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ezuxjhmf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qxgrddtm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hhgsbnvy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oniqkyjo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3imykbuwq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3talivpfg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3swwfgzzu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jitpkvnu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uurlgcwj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cxhlowbd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ukkgoizk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kdnddcqd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uviktyyo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3icocdxzt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ehjsnncw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mjsbdtxo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3osrohjke.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3iqwieqec.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ylamonhe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ziefsloh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3myflerpy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ixdzcqys.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yhajvqrv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3crrcbzye.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ktmxanri.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdtdjmt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cffdiheu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3naihiada.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgalsog.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3witqrzsb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cddlnwot.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qcikgeaf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qwifkyhy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mkpexihn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hjgejhyu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmlozqa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ewleslic.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3crjccbhl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lffoiyfg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pwxsnjda.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwmcriyk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nxhazipd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wrhkftjv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3abxayvfg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdrvxhpe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lhdxsmwg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rymfafjx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3apejxkvv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3houqimpf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bavdzmfy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3srxpyhdj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lsahlgfd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ynlghmgl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmyyiiii.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ctdqnbnw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xyeamsem.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxmbve.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uacfbmwp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbltnqzj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vpjejynz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwwxokm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgljvss.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xgcatqwb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nxgplaxu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rewinlph.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3whntxmkl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tteffwhv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3agwhtusd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrxaex.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fqhhpome.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sqcnhecx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wlqtdsxq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hektrbyq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rrznnrxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwynvjte.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sciceuxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esznfxmx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3raqaktux.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cnvzzlvr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgqeewa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ljciintb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rnofldtp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xacewgwv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrezxy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uorqbaqo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qwixxpzb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ukoirujj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3holiwuqn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ypivieov.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tmtyjlvg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ufnyfacn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rfoupygz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wjmhdnzo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kkwaqplj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wxwbxrpr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zgvnetlf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hzuwotwu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3htakiuma.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiuceuup.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcazkcj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ejxwsihh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbooznzz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nuaxfnis.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vtyyutoo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dveqpbib.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nzovrtbo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmiollyp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxzllrd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xbdsljmr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzolvqmw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jnnibyle.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qjynarxj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ywroqrwa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3shyjmnlo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fnesbvka.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ebuhwoty.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rpzvmgod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3svswconp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfpsekz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrvjzwz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jryzeylm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qptaiiob.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ignfhyab.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mdebdomm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uowjuodq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bfiksvgl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibwfszob.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qcfkrwcv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ednyvxam.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hpyljcop.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3auybqlza.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bgsmrpno.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3alfhfkxp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nrrfyerh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lyszhvgb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicxlwja.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jrqgvomm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3prcpshlg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ejicbjfu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfghomwe.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zbnuebaz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3crpajyjd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ajpsdqzt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtmqcg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rbpcbyhz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gfhznugi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wshlvxdh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vjglbijh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sygwvoaq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tyssdauk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wjfihjnd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ymhssnph.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqxevqpl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sayqavrd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wciuxgnh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bokflyvn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cusshbrw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3klztgrtx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mlhtyjac.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wsidrcoc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txwzzyzc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ivlwgnla.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3swyhcdtl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxlmolpm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbdonorh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3urttwgum.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqorzvki.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cnkksfot.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xuafuwov.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fvekotpt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3slzojyql.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jwjrjird.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqknaior.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ihirxnag.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kxmdxtco.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcfwtqjx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbwbhmkd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wuuzglpz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jclsnysq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cslzpxti.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xhjuwzgm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mvfecyhs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3oszyzbim.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mxvhyrvk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vrqxrahq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xsxmeysz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3aoxasflb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfiahet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jnstjnqe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3khuptbss.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3stvkobpp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wiclonnr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3brogyrdl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3iajltoib.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3byhsdehm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtnqos.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dilppmxp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfyktqmm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qxeauquy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozifefbn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rjrufpdt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3twpumzvd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qkydjgak.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mtrpicft.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ogawmbve.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qoolmunu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ntzkgpgj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tffmpsat.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3soytygiy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wdmdjzav.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tnnheujb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nujbbgvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qjiyrouo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vjyggrbg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tvyndyvx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oaotkjnm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bhsdarox.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bjeqoqof.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3shwcficz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lebpouii.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kohuagea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujlewhkv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbpyjzxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaylzryg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uvtrqlus.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lbyudpkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btpzngnc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qngywmwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aisdpsgt.html


<!-- 参考信息 -->