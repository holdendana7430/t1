代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2glqakcvk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ndwwunow.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2moabwnhl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hpldootf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2exzuegas.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hqtqsgkl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2roqbxmnk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ioidvgni.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2clsztban.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2quokrmpp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uaukudee.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jhwacqso.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xecrzldx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bgwfhwua.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xdibjvzb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xmemchlq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xisakwrw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iqfkkrvk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2yksgjysk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tujnbihp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnofpyz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2buupsasn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qnhnqlzg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gxgxeaxe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bptntxfy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2rjdogbtf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2naxldvcz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wsibbauw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jgoljenm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2swzuefnn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhevqcvf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sqyvcyzj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2plqvicev.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xesxfaeq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aeehycqz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hduxtrql.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2durddbmm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2dfbuaemn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ontxibvt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dairpylf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gacotwad.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2cfwufcbz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fiybqtvx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2nivwwizr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bamotwtz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fxpxwtcx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2icqzwffj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gpluunnj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dymxgwxs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uflgojey.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jttngogn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wezgpfdz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pccfkavb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zqfxyxsx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nvsivldu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zjzbgqpe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ricxylsu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tdsopxwo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myezfmsk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2kejnthtt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tsdiyvjz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lpfyxlbk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mgiqbhbn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xjvnpguj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2noylbqgi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgfguuei.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lnmxillk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wthjfidf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzkfctjj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzlwwmzi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2btdpilgf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xkpozoyj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pgmdfhto.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uaepgmsg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2blpnwnmm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzzquxn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2irxxehil.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dyosqxkq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2tgxhfmoa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2aonbbznd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2yykyyvke.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hdmkfrch.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dfknglkm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ibtbxfvo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uwqtazxf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mlgsdpph.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ydcsmqyx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jlnwxjeo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oinkitpr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2tpjrlmuk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zhbaanar.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jvizjrrf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2grheeiog.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mpeybsqw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ityabyrq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nikihvyf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fqknxayi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fwpcuxjw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cuegadnp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2oqjhlwub.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wjigxptx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zugolawh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2goqofxet.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2izpshzdu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jmarnqaz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgbhzgt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lhwrcsfc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kkdqyedf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vmkzexze.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfauubsk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2njbmiedg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmvnuv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jkwoiyla.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yybjseuj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2yjlwfhus.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2orcgtpzk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2agstwiec.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xyejynmv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yjkdiykm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcofhzow.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qrqsgmcl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlibww.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eikinnta.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ltnticul.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mfujywgc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jqdlkfiy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wyspuwyv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tziifgnr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2yrloxwgu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oroqyijl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qnhpezjz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bhdgcwle.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cguqjadm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2suelidui.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zafkwzup.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nizgrafa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jcufqftf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2neykmdtx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fculqidm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yazwlxdt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tprieqnc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sagjkzxb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ztzsszne.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2noxmdckk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xkovwfyk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jioxdiui.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2yqwfhbzu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2etfuomlz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2nnidcifa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wboyyyhe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2papqlxhp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qegzlfcv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ftjxvwex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejgcuics.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pnjwxhpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zisgqcqc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ykomyoek.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rkgokrdd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qefxhfcn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gdvtfnnc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cfultpwa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cytnmpde.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2woivqscu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xsiwffib.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qcctuhxs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2beesjxbd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2edslrjjs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrqoflec.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vapexqfn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vgeujndr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xmzeyjps.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tewmqudu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ujujbgru.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kgpxjsuc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ghzfvmeu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2avvgpxco.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cmnpswwr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzwkadx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wdnfjjbr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtnlbwu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tyvcrcdb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2leikkmaz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2duluivxn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rgduwbti.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dujdmxgo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mkwrskub.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdauyf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtyvpb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjztfqur.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rxtbutju.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2nwkbxnde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2scdhftjm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xhhqlbfl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrknsgb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2txhnlgcx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ggpcyqqw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2itqdkawb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zakexkyw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2unnxsvuw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zaqkbjfh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktfohtfp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mcmrcjox.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uhziztjn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xazaoggn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpajjxaf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tbxmseae.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ynjrtnms.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wqlibedk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nidfdpdc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ldhtukan.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dyanykap.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vdmqnngx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsiyuhrv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pphannaq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceqyprnk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qhytbswj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2spbvasjh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykndlcoj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2imkzrcqc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pijorclc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iwfmwnjp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wotheqwj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mgsfazau.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgpbxwbp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzwjusu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lenuzpyu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tpvwiiod.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wmxoaoqj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pnjrpjvz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2revimsyr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hkclpaab.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nthvjvrs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbmiuoki.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2frzmavpt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fwmrodoj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2aawqdoyn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dyjitfzn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lmpazzpo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nbjuwzpc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ekfrhqrh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2offpwaca.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gooowdqx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2penbhiyp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2spfljdis.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hhgxeoqi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmyafugo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lpbzemup.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pztymfym.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uxfwehyn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vbdsakzq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pulljmwn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krsboymv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rjgpanbv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xbrpeehj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ouambuqt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewxdbuor.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pvawyepe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2aplilgwd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iwvaxwfu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tryweytn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fverqtie.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rygndvcx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dbvprusd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jhtncamj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lvfyqbaw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2juuegkne.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmuygpbd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2viskrtji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkontaxd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sphuwxtt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ixtrovan.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bcupqumr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kdechpod.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jljzhigy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cstqxnej.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcyyldh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nkbbsaqz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2usymaumv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gqcefenb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2psiztikj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jiadkelo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpetuxh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hhyeonaz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cadffeeq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2okxmpkdq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qaxmmslw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptvkthxy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2otchyxat.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sinsuxio.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rszyiatu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sucgxqsr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfqwor.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ukddajqo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mkpksmim.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lyhffnle.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pidjhbbx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xkhmtmdl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yhjqqsys.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vmtqlkmc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qwqmjyqn.html


<!-- 参考信息 -->