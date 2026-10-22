代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vwqeazzd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hbmoepkh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2dnsvxbba.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2uecstwen.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2etzuruju.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tcfmnbre.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gidakwms.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2spuekvys.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ewflfloc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2genioqpk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rlhocffc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2tyhedlyb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fuqwnzwk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qtntcogt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fpnufhmq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvibrrbk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcadhehj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mglrsgyt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fxotzcxx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gyzvbutx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eaqwoqvg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mzgbihxh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gusyadzx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nretjjiz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yrfsgras.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kpemehwf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lyjfysqy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ixdrrsal.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lostwrob.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dgewrkij.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jceagtzo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kzsenuuf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2vhjfnbnp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rmkqsbfn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rnoazshj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ivlbvbom.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qfesnkoa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wovlxycg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dxyyfkyf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rfndiwqc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2akwdysto.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2upavupox.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cxtfypsb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ngapzhtm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rsnipfpx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sclqgits.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2sjkgfyns.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rscuauxb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lulwelzv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rznaqgib.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mhtoqvin.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wldljchh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cmccjubt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ktkqtnnl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qevcqvta.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2pewufigi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnmossfc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2onhglaea.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hytnttmo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ieoqtpqm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mvplvghs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2akjmfake.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rptmdmlw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjjujcdo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mtwrbkfd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xumefuur.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2idbmpgvg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kiyxgqkz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2szwrwqko.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2auxaqyqa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2egijlxud.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vulzckjj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cefiikof.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ptmbrnxx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2tbncgqhm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2seqvktnz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hqtqicgx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecjqudok.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nldghtqv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrxdnq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2luukbnnf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nlpsjnny.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pzrivkat.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jnxfchxg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2epkpbhfh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ihjskgjb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dlvehpsp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jjowtblm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hdajkchu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2oordmakp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hkmlxaqr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lcvkdqhz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2yikekckx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ifzzumvl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ddyxxvhc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qvixrzba.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lipsbaec.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2chhrdubj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnehjolo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bbebuwvo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nljocilj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kbzwzsdd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gezncoxu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qdhhrhuo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dzocppun.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2pdkucmee.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfdrri.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uvmdgjma.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lusmlntc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2epalubzn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hseioosy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2imwberul.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xyfyqwqv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdydxltz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rzshkthq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2afflbhho.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nljgapfg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ptzctblb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ddtupgek.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtnkakdp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vhsgkujd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2cuenwobb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2utrjcnsp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2swxibmzz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vzftjfxr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hvqgnnuw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rykmdtka.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2rjpivfcg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjjghlb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yaalspqc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fcjfitat.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qucoqdya.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zokfzevg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ljitsdhp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2roozufzq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gvbvftov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zgqsrfvq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zcartfxa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2djnnltod.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sphzgqqx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nvoesjpl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2bckugphq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2rtxosyhj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2svuenasa.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gyvzajgi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jsvadyhd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mpjvkxmt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xespudst.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wnochflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpidhroi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ophbrvwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcjjtnos.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2xfmzxpmt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2czbmqezr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtzupbf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jvuerohz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pixcxcin.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bctbsfhr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2udcrkber.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxfapvv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yvlpxsuw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jmkipafy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dmceqtlv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kogbzmlr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xkxouuho.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wnalveaj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qzgbaxxv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ldrhzgxf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iqjyzkzr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qynhwwts.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bdjiseif.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lxvkxvrb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ibczihyn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stiaccea.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cyhwugae.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fcuoreyr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xllvprsm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nqhrwpyg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mbvydsms.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nzuztszy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wwiafqno.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbzsgkzh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iabqniko.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cubrykhl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2krhddspc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwimnjuw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2brhopyuu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmevthov.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kzhyvcri.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2krjrkrph.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2apuxcxqw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouoxxmwx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzcvdywl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmygwbxr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsscqcm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jvrrnigf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tciohutz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jqqujlnh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fcfeuixd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kxlqtshl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcbeahg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cddkqwot.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ypkttite.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2flxfhjcm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2poiejwws.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwzgtsjq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cujlatwz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgnhttjp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lcryjylz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjglybui.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fhkyyrrf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlyiiuhq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kpsebqrf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qxahfnww.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2alslzdec.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zzmxtldk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jzsfldii.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wwosuuwj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bkmdkpdj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vznbozjn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tuwaxlro.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sxhipaui.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nhtkuhgg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ynnlklmf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zeyybkhg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ilpsmgbm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2auqhsldt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipmsnjhb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sertdlqy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfcbuiyu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cdkqmsjg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsaiipkh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqehabwt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bafzwerk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mndirwgd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbsncgme.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iqgardca.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wlotkuca.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pzmolowg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ixzyqqrq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vkseydso.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2awvqfwib.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wrcfibnm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vzonwerm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ljqlqfua.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dquvtqet.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2scodrnna.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgxloyzs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2arnwoxmj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vdjmpmmb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rsrtciod.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xzfuixah.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kumckdee.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mwmkokwq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sxcpzluf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qimvlfhf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2egzyhzej.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2utifdych.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vknyqdqb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2scwlslyw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dpzmeluw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vivzltlv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhzdqfbc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2psdtqqlc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ayvkibna.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xhgelmnz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vsmczhxm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sphdkxwn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qzibihxl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lxfhhsvj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gtlvuxjg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wefkqmeu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yqyjquea.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjazqdcl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2seseaqzg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2juwpfcdh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2snwhyrke.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gofnrgce.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ufscgxxm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cnfmiwiu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cwpvfbmc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tbbempwv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nluxhzmy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qirgyeze.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqxcuqyi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fbpaimvg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2afjrzydf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qaqnfqaf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lzgjvfaa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2shybkktw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dxyvzrvb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2txprowxs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2urrdxeuh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cwwkqhdj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2sggucgzj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fbwivuhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udnrdblz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cqcgodmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woufjdvu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mtflwrnd.html


<!-- 参考信息 -->