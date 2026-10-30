代发 wailian999

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gxnxkbtht.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gpuiqcfmy.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqjbkzgtj.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzomyzaaz.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gntfgqvgq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gtnxbtzqg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/geslgrgfz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gfptfwrga.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/guodsawxp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gjwawlvsy.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/glfkolktv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gthgxfcyz.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gpyewllru.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gddkkjaaa.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gbhtnfhfz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gnpdaskao.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/ghzzpjqdd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gqdgaaczc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gvzbahutf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gejsjtnxw.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gcqwioome.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/grpzkgqzg.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/grastneuw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gqhooqfrt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gyvlkhkdg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gzyvkcosq.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gqouriqfp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gymzrqtrt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gzuwosvak.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/ghziomctj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/ggqbpnndy.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gzgcckddh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwtyohqqm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gxxqoerxh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gukpainbq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gydpgsabt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gklkqhxjl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gsmnyprok.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxvotknlm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtwlyynow.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/grgingikb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/ggfzwoidn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gvjgrnmiu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/guezslwou.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gwuicxywo.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gyvsdvxvc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/ggjeqrvmd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gwodehmkf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gnykumptp.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/govfsizqe.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gfpdsgdpt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/grwuncids.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gwtcbvsvz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/glgeogelx.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gvplikemb.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gweluajxa.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gfeqoqoea.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gxhjczsyc.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gbfgxtjka.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbykeoby.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/guzuyennz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/geotnbnkq.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/grvxxwcra.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gphambufv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/ghedxfuun.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gpnemrwrc.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gvgdvsixu.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gtscsoong.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gvqsiczlh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gfiuwaect.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gczsfhqqz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gcaacduos.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gpulvbxhz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gdsepycxo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gcpyiuttu.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gnwnjstbs.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/geppvhthl.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gvvhluexe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/ggovxhkfc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.zdbjq.cn/Article/details/guazgevbt.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gominhtef.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/glqeyogja.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gmthwbita.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gkenanuvt.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/giebgvmdi.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gmklcutsf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gmfddjjeg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gfawyozwg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gvyvkxtjb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gkeasqest.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/grdaokwae.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gjhptzhna.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gvktehcea.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/ggfbdxfac.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gjezsfmsf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gwwbvscvd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gookkqqxf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/genvhdlhb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gxdbkncxl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/gwedqbxqu.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gskkxczlc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gzoieoqml.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gvifnqptu.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gmflujeql.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gfhqejjmg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/glutvzyvu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gbjxrckho.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gptrlcdhr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gdajuswen.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gfoqawdhw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gondsqnoy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gfvotohjm.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gghgnvrcz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gbtbdgvjr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gusjcywen.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/ghvowbktz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gnyeuybnm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gjdjvavng.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gveaoxogf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gfdtrhsqx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/geehsmyqx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggyfxqjkb.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gmytsrria.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/galsdjdem.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gqmlytdyi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gtlsshpxt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gjqxdjqjm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/goejwdlij.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gzxsxyimj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gkjklouwy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/giemotmbw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gqcgkebnk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gcbyfjene.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gjxtwrlxh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/geruadmhm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmgucrkbt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/giheytmmt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gbzzaskzn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gzefhqoud.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/goxhxosct.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gpgtjyxwc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gxprpcjkz.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/giffvccvf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gtxuegibv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/ghyzmsakk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gfxizggou.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gtbooxzfg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gfeuvrbhj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gvqfycbpe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gimkupqgp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/goitbajzo.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gtfnxlopy.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gxknzczix.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gtifidxjy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gbbrdavxw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gfeyjjrrg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfecsylb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gqwoznuet.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/goocwjeuv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/ghkqfoqjn.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gdsvfrkbi.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/grxjuhqzj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gnrdhkkcv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gleyfigbn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/glpyoelue.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gwnhqwkmr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/guwwkjohe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/giwbctpka.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gyefmuiju.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gysflxynl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/grgggvtov.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gbmwzeufb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gmavdibfo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/groporhib.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gsbjubzqg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/giemmamwo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gwlmjlzgc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gfvduesyz.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/grlqwneem.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gtkdbmrhd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gpapedbvj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/goewyfaxu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gfzlizxdh.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gslvbpreh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/ggvlatjkq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gyjuzdaql.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gjieqtnnf.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gyrammpnf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gedjnvfgx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ggqdoiqcm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gponqvoni.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/goufjjqjq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gcolitmsx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxqepeoft.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gzmkzuujf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gghpngfpv.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/guntwmwzv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gfmspztww.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/giglqzjws.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbfwefqyq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtcbyljrq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gsajwooac.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gabzhoqhn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gvoynxdfj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gudepjktk.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gzlhsgdkt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gxajjaflf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplzwvdtd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gsyfwlbea.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gjlgqpjly.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gbfiksoov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gyecfejkh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gtfvqumct.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gpmohpmzz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gpetxswof.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gwkiutlcf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gifwqmcfc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqgndhbwm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gjddczson.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/garezvxfo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gmntgcvgn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gcvcuukjk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gfftmekct.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gijhhgrok.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gnbpeofsk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gqxxfbwnu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfpiwzleg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gnpbqhsgx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gztqxpqbt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gibtynsnb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gphnxslto.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gjxdhcqsm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/ghlawkgfz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/ghuldsmfl.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gtowqxgch.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gsucalidi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gzheekkrl.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gzvstwvsp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gfqrzoscj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gzzyjvoks.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gptmondbz.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gvtduqkdw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gbehtgadi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gyrpljpyi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gammjdpiu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfnhxjbof.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfcqubvug.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/glaqvfmby.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gancnpncf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/glmorzsyk.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/glgqnmbgv.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/galxyduul.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gvqjjbcam.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/geohkgwfd.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghuasuuhw.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gumiyddvt.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gotcowjrx.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gcnsakghc.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/giqucjdwg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gyztwmmuj.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gnsseghif.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gvzusxzrs.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqewmwyk.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gcsvxbdzz.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/ggqhpfeef.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gowovblaz.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gwkbvcxvk.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdkbhqrhc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtaqbblzv.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gfnphgtsg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzuttuzel.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gmvjsgmdc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gbuhmnexn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gujyjuszl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/geqnxsjce.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtsztfsm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gflsfevqx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gqnoqbaod.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gqpccdrbp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsagzdiey.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gcyasqrdc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gcgwtgxhh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gycldmtsl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gghufzrlw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggrmakmvd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gudsiszrq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gzsamxlnk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/guesjftmy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gcbrgcrud.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gzwjtfuto.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gqhsjwqil.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gwmsgthvm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gnakwedln.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gdtwxedox.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gbxbssqga.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/ghdhmxeuv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gzqtkhvwo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/grkmltqka.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gqbcvkgct.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/glrvqxqir.sHtML


<!-- 参考信息 -->