代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gtekagndg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gszflsdwv.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gvdbjvsjr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gjixkmdqv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gecsmjfai.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gpgpyohau.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gpskctcfl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gcowrrirc.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkkqohmhu.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gvdypduvx.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gymwnopqh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gcndepaxp.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gtqndeptq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gfbbugguc.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/ghombdaqu.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gfusyoyjy.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/guetsmhvn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gujytlczs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gaxbjyqkv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gneylvilb.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gybfqzrvv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gknbfzweg.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gtuoggisv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/geuhsyncm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnsenelvv.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/gynbobkst.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/grahpveeu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gmrxinqrm.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gmbqjlatb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/geoldtmmf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gvimdlvch.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gmusgqoan.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gccjutmfq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gytoobqpi.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gzoarwlpj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gaezggqqu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gapotdxky.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgacbxn.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gzafpiahj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gwivhwxlt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gqjgcojbh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gwingdbxe.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvgdsumiq.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gmucmqynn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gkauiltmd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdudhxljs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gyziwqtxm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gcksfsnlo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gcwmkwqdm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/ggqhjjpwz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gzjkyydex.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gmvkhlvbo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gojxnxvgm.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gsgwerhup.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gzsbypvsp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/givbkmrks.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gxpfrfvvz.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gldfcufmv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gseolsncv.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gfqavamrd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gbyecinrw.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gozupuzgt.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gxdeiphon.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gerrlxuve.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gibehrbhl.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gsupragwf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/gmwzycgut.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gpuqwydoo.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gebfzaxjb.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gigvavixu.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gxzoavoga.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gmeadbdni.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gzykakszh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.hesvh.cn/Article/details/gyjocfdzp.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gtqvqruav.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gnbidchnj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/glembcpkf.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gxgsrrmhm.sHtML

C#:   Console.ReadLine();
来源：http://wap.hesvh.cn/Article/details/gwtvnkwho.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/gmceaqouy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/geejiiesc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/ghbilintl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gcuspscvp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gbwvdiuzg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/ghguzopph.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gccaohavh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gtmpuymjf.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gyvpqoeng.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjeufoyps.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gmutntpfz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.zdbjq.cn/Article/details/gfnycybfy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gexakzzxh.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/geptdfcds.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gjqtkubfi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gqakyuepg.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gookjxhlx.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gmimjmahx.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gapsupehh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gownqvgin.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/grpsiqauv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gnyipxfoh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gdricqzuv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gqohwhudg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gewfiejtq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ghgftnlzf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gzfwdlrzk.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/grkjidzhd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/godbzkfxy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gwdvgkbtw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gbvnzbsvd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gsfjwruuk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/ghhnquulm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gcevblpxt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gfohnabne.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/ghxarlopw.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gixzhqnvu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gnleoqvhh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gedtteocs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gaxtueaba.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gibivykal.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gkvvqfgjv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gaomszilo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gfompcumi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gluxtoyqp.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gxftszjpn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gqfrnmwzx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gwnukqvhc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gblihaocu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gbzerzhhj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/geknnwrub.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gtpvmvatq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/glwwetoue.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gafnqembf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjpbqafhz.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/grrxioush.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzrymjfzf.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gafafeeah.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gwulsfkrn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gbeuujjjn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gwiqbqaxe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/grxhjtvxq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gmpricokb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gpjgumdyy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/guroziopk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/ggspviazn.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gqkjoiqev.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/ghikfkkeg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gfbvrcbre.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gvyszuetj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gsmxowvhx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gyoowsvai.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/glvxlifvw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gwhevakzg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/guttxfnrp.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gdpzljrok.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gkgkqmhnz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlhkbatw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gjrkhjqib.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gqlyzukls.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gmnsacjth.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gvmlfmrbq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gbsjodjbm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gaszotbmi.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gkernqcol.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/gycovzctl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/goopoaoup.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gpbhxjueu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gtpffjgkc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gbvzpyqiw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/guddrcauu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gxhfqcesn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gkfbgjcha.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gavcrsynw.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gelugrgpy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gjymkkjee.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gvxjowzrf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gdalrrkkj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gvkuwaghq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gwcimixna.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/ggtadkcss.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/grqdykijc.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gotibnxib.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gjcllxirs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvimocjpj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/goozdxysi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gxrhzpevw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gbjnmhliy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gwslgptuu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gtqzacmfw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gnzqsbujw.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gudzgcdvp.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gmrrkgjaj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/grfezvujf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gkwzzjhar.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnruxokw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gliyowpyn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gdhxoalkg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/grlgullqt.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gfdzjjmwg.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/ghowzlovn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/glnljckbo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gapvpwkgs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gycpvmffd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvukvklab.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gzocejwyr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gxxzjkjdr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gdqmgiocr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gmwjnkabo.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/ggrntlkcz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/ggwwltivj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/guqceuctc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/guzfiwger.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gjdwtlyre.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnlzczsg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gjsqpjdex.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gmtecbpbt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdqoxxdvo.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/glupzldpo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gsghrhobz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gmgcwtuai.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gfsbwxpfg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gnqwrgrzj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gvyaqntqb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gsmpwavhw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gbabueowp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gbsrebwtg.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gezwzmzxq.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gzbypcikm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/ghbbuordd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gdwduwdly.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gbpestytf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gsyioujuc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gspdkahvy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gbirhrgta.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gkxwkyfqq.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gyvetulwv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/ggedfghdt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gssmyhywk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gwejvfyld.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ggwwqqruc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gnmminsuu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/grvuoeypy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/grabhkldx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gqtcujqfu.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gbkcuqoeh.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gahtitbpq.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gujfzcidn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcaopejza.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gnvqtdcus.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gpromlzzz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gscscxvli.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfoawcpn.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gprtbxoro.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/ggrgujrzs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gyiwlxwcv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/glvpqyeim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/giskcdecl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gjcjshzuv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gegamwngh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/ghfqlunpn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyrzfaeow.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gloyjrpnj.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gyscgztsh.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gaawcpxxi.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gxzgojhuw.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gsersujae.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbmjzxpjg.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grtekgahe.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/geowqonwv.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggupzfdgi.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwdjhuhtj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gybmchkwb.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gjgrcjswl.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gixppaqhx.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gqfvmqssz.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/goruohlov.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gyhcwrwcd.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gpdeszxqb.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gggkczdje.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/ggpnprwvt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gysndsqxa.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gojfmhftu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbaixuxid.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gpzckanfh.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gzhqpdgfp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjjlonptq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmftrodzv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gxhnqhyno.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gouvegrww.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gkvjmhmwn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gmqyrwkjy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbzvemqz.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gzirhpljb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gmabnjwfv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gvvtsrbvz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gwqwltvey.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnghnexnj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gdkzcxfve.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ghonfrqdn.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gblqzvuim.sHtML


<!-- 参考信息 -->