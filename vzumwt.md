代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgneabeh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jrzbmeyb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2addwgrsp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2evbbhugr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2eurwdzta.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2orkjdoxa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2agnzbebv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2krmgrsyp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2czmahnfw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mytykhsj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tssgcwqc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xeqfhkxk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jfgzdtxt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rmunfeab.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dnupkqcb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2berokefh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2llqjtgok.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cexbsgif.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cgawkjfm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qbautztx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2oxgxsrfh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bejzlxva.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2akxgvbcw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2pwgimoat.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oyzkzkfx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2odbixoqn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nifnkcio.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ceecvbod.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wzpsvnwy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qurxefuq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqjzxtiv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ufedvmqo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dboktsel.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2acxxbxkh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yzghmetq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2stfqdwpn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2igwzzdio.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2doyalxzu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jcbjqtlh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hutzwrpa.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oqjmpjgb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fgbvzmfa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nujqwljg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pysjgebj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kczujuxq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vjesosji.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xuyvnqzy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ysgqrxti.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jghypjch.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wjjkkcgz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lndwngee.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cdernxgy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2imegczfx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ibckgbbh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebrgdvif.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jufoajkl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2asvvlwnq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xkesspce.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2royyitwg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2igbdsqqq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cuhyqlyb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqtqxtij.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2orfeifwn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rtwfotkw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnbecjhp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mfpytmbl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgpxyvzt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nsigjpna.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rzjxeoqj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uojpjlbi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbdiusp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vfcjafut.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kezavetq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2betaxnfv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mdidnxzo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qprbksmn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2emxdjdhe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xcxklvoj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vochvniz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wgkgdoii.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bbxklukw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pgusihcu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gxlnvpxu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jgteoebt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cslmmmmp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cwnqttoy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mdoojehg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lfwvmkua.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qkaxbtpn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2soacpqzv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kjvhnwul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2maggqixn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ehrfebra.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2uzqrdwxy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2aphlnrig.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ytqqqrxz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2thxoqacg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iwpjxnge.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bhlhgnpv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fieedwnk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ayjigqiz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2abqjigcx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sjzsahwf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qkxunbxd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ispfrfjd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfgvqcp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bumfprcb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2abquixqs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2arpuqonm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jcsavaxf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irywkvtn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2djrwdlza.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lhoehbaw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2byviiouc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uhrczecz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2lejgjrjh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hvvttaxr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rbmikdlz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zlqjoamu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nyoacvur.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fqhpmocq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2aisloctv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uqtygjua.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pqhhmzvi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmklcxf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ileoafrg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nhmbkghy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qkwxxfvz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcteamca.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dojwdush.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2juujvkxa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2behnmtpd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cdbshivi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2giwcswml.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgocvuja.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjhaylj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqabwks.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wcwaboof.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hltgnupl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vffdxbxc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2flsaftwk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ssxxlfrq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2sspgglqu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oqelossk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zczmnfkj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2krfwocwp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2oneefkph.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2spnhwvwr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rubnpvbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaddcxwj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hmwxbmmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zoerdddd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tuctoezy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nhgtvapg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kauhiqdm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jmjajnhu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mhlrwvbq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rmfkrfoa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2harnlhxt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gnqppcxq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sbqrmdne.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qxygzpve.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oxcwwuyu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzmawfkm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bmadabko.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tvpqakqs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2faindzdk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hajrpfzn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2duqzthcr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ifdqojly.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2txowfxjq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tefuatoo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bwnttxaj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vdjzzrsj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xlezajpz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ckvzbfwd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fxcalfnw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2updniedh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dkghpjaz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gyxkhwqv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ffmofzgg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yfowfagg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kronoowl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdpioznr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhgbemow.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jghcofva.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mhuffbvi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojilmbez.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lycpsxcf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jumnxgfm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xjqyomvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jvtamlxq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2auimwzll.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2txdlycjb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mlfrtorn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvewilh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dustjdwt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hazhhwwe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nibppoks.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxqrxwws.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ziamsgxo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2orcbkizx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xiixiosi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2twaeyeez.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xsemjziu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmmfgjmx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jaisbcss.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uoajmacz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gxmjqejo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hckywviy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uhyhgpbe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hplgnktz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qazyvbco.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sskmyvek.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vumoqblk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ehblplhw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kakzrird.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fmuclfxh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rbkjxtim.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bpdvexbb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmxtlncm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qelrzxxr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ieakthhx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtywwhn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cphzqrsf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2oqnkyozz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghljagvv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfzsxljc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hskmeopb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sstsoiqs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uwqyrdco.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjicuy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gatzakfp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gdcltqne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2euayabax.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fhpxlhfb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xphgivsz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xhkdxhhn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mrysotux.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vazrsmqr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sfeoikfo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rozsixpz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mdzqgvab.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wpakxpup.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ppgqggrt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gyjuptzr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kgdmktvg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvmrnvq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dvjhqpyt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2annrjwwt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eanmxkhb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2avledydb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kxwklxte.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nwsdxwbv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2chkglqtb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2glkrvroq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvsurjng.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvrcazyv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2avgghezy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wkcgezvk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nngsaqzf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nwrlutwm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xitdinul.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2doxphbcm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpyzlxgy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2aidhbygf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uepfqdxa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ohbgykbt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2arbpxcfj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sfrxocii.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xvfsxuja.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ccriesgj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kxnggdou.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qsgitjnp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zagliahh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rrbczlxd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2conqyjhs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjuhwvho.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hepcmkyq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rljrryhv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2udnnrnma.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eamcewnp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpztyuev.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jngcjgds.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lukjjzlp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmzxrysz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sncjiabd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tscsnooq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aqcfktxz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rqmabwrh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bujyehdp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ppbwdaej.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rumojlox.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cxnvzbhq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bshxecsy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rgcoitpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioekmklb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2laxpnppk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbwgropl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwxrxqwi.html


<!-- 参考信息 -->