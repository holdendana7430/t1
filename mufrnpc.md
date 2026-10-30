代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnusuzmts.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gzaascwgc.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiskthl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gbxhszarp.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gnshhrcja.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gstxzyxmi.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmgigkazl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gtugeglrb.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtmnafgti.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/grxmhtysl.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtnugzgco.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gvrtbgdet.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gyavuspxb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gqaprjthq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gmjcwbfbj.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gogdiwuth.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gsspwbtgx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gpzsxeghz.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gxtzpkgcu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/goqkuccru.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gttcqpiwn.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gkmpslptw.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gbzpvboxr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/geyuzjdvd.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/geutzwzgp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gphmhlphj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gjtclsbay.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gswpmakjk.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/ggzgfeklr.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gfrzetnzv.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gluddgbas.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gxtsdkmix.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gjfcuqnpv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gfhelzkxn.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwtfnmkbk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdyugzgii.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/ggvmywcbk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gnbseockn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gezsvtafd.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gzinghkxa.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gcyyxnvio.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gfruftbew.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gvntgkgyx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ghnboaiuy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/guqtkfbtr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gluaxbbnd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gegnubcnn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ghaxxudsy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gglhktedv.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gzqsidugm.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gzrgldqfs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/guakrtqye.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/giekjmmxq.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gzhgqbwxg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gcsyaszwo.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/gjsyujqcc.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gmqfzptrx.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gnnopkncf.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gtusifscf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gzzophdhm.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gvodjnznp.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gahgfibrt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/gldfscorp.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gaunqsvyf.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/ghhyymfff.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gqluzryir.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/govfpmhvr.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gsorvabdq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gsmlfbtzl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/giibsjavq.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gnoisfryi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/ghbadpsgr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gayvvrrxd.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gzhdikbww.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gnxtggqlg.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gkfudrqbs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gbwnkylma.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gnefyyajs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/geoileyni.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gztlgwusz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/grafxjrwy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/glekxlchm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/glazjmize.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gtyqmumjp.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmpxoexym.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkpgjdcnr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fehbvm.com/Article/details/gumjymefv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gjgzrmrrf.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gfpbgpijn.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/ghsgasgge.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gyhrigwtc.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gbfbgtpym.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpzwszjov.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghxqjxdhf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gazmqwdxu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/gfdlatlai.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gxtjootyu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gnrbboacx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gfgqbktrh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxupbubta.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gszdafafy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gxdflkpgt.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gbgcfliot.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gllnrkkkw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gavfbgwrh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gryxntdrs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gjhgjasxs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/glimrgltk.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/geuntjehd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gllguqalj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gfmgrrass.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gezkfzkpj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gwsthrzhr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gunqzgivj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/giqbmucbi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/ggxnyyyrf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gtuojretw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gtblrpkrr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/ghwsqdhiq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gbodsoqdo.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gbhjfmhuk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/guxsemhes.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gswidamtd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gctvkffmq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gtcidthxs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gkkgxkprf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gktbdrfhg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gffurzchq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gditjyeot.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyoxhcjkp.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/ghscyyozv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyjhtkxih.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gbxrovbxb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gobaukeqq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gqimtgdik.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/geeujdycm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gdflzheve.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gbyzkkmcm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gevxvmbnk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gwvfdfflg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gycaterjs.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/ggsqqeglt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gdqsddohb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqyrxmkks.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/galvknwqy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gsiliieiz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gahfdgfjw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gxojdassi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gyuvsmdmr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gqrqodtpu.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/ghpurmyqy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gpqbnkgvf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/guclpjyhr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gxudtcfxv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrohwsbi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gdcstwtnf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gbsvmlpbi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gcibarnqx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gkmrejhro.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/glaizvmni.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/grvgmbdlx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gzfkdukwc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/grurcycjy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/glfguvcmh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gqjxcoqsh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gxemxuoll.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gmhymlatw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/glhpglgwk.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gfueqttzw.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gvqxnagcw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/glgxmqxsf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gamqwwaqq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gkhwugmud.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gcwtrivzs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/grshyjkaj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/ggwbnagxc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ggmryuhgg.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gpqsbujnd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/geifroxpx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyvfzkia.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gguaawnfn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gucjdvevl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gueqepgkh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gubyvmvdo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gpdeqlmsv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gcydlbvfe.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gutticqjx.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gdmgmbork.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gcgizpxpy.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gssorhtjt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvddjbran.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ggveskzwf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/giefrueec.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gfomhspmu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ghgqtbnjn.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gedwufsub.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gjmupufpc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gdpiapkyx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gqtvtmhfo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/goizlipvc.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gccbkuqlv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gskvsosoo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/grhqpsbgj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gjuuomuxo.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gukdhxjsa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gsjcelzfr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqajrbtlh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gwtirpdgj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gdpwrbvop.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbnqlxbgz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/golxxkuoh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gywhgrlfk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqkdfqgi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/grmzjwhsv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gfffncwhj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gumszlznl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gjhefibdc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gpeplayhg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gebmdiuvd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gscspsvsx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbbnsrk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gmlslysrl.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gnknbriia.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gxrxqtxtg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/ggaxvedht.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gbnjefmlr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtiwczbhx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gxqkwzzxn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gqjroeuve.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gakfxpibo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/ghlwgjtcz.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gjobmfcau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/giixkyksx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gyyfuogpz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gpdqhzood.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gbtnkagev.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/goyjnzeua.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gpcamuwdv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gnzdnstvs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gzoxlxgbw.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gitinufjt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gqimuugaz.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gqtomgtyv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/glwbljkit.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/guvuubnec.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/ggilpcfzk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gmqpmijgn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gbkpzentt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gtyvqukgx.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gduqlvxqr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/guhdomddn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/goihlquxs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gcpmbwpyw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gdrakhrgf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gpziysnyx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gpxkatlct.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gkudybvls.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcvxiwgdw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gwqtkzewz.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/goujluwia.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gkxlgnjfg.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyirzbbgm.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnkmkvjaa.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gbjzsnpig.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcztzxtui.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggymtlwni.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/grrqrbylr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gocgfsqwb.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gojjxeojp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gzkisusfj.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/glnsljefs.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gumlvhwcv.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gbsjihpjs.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/ghbildqkn.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gappzypob.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gacfiwgjw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcdeidhog.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gxmxclayz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gthkniiue.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gqfqobtkc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gwnqsbzwz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfniwufne.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzmouvarm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggmncsztv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjmsszaht.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gjlrgfgwf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/ggqdjbhao.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdlkhmbrw.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gostlkwfx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gkcjtblyk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/grbkvikcg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbfkmnxzd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpzbhblon.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gvxxuypnc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/galmxfwlh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/glbvibkul.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gsafyuacj.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gfdmccsly.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gjfzjkplu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gjrkgmfgv.sHtML


<!-- 参考信息 -->