代发 wailian999

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gfehzqbor.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/glsczjzdl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gagspwjrl.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gnrlssezm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gssjawioi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/gnihebvgs.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gypmbozpt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gaswnwiyu.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtafzncwf.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gkiifyfmf.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gdiwfcyto.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gvsuyehjf.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gilhcwwuw.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gkyotvmwx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gamumpphs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gwzjelcbu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gqcfopobg.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gilqdnihx.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gznzqwdxk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gfoosgybj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gjxdhdjfj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gcucdsppr.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gbijjctme.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gdjacypkc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gckqempop.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gpydqifne.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gndisjjga.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gafppomsi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/ggemznojb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwaqukqvg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gnfzfgdws.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gtkxjaste.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gfkzhatqi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gvlssvzkm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gsntngvag.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxslzqdgv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gpgkufizm.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gofskikze.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gjthnkmel.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/ghblvhlro.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gbncfssso.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fehbvm.com/Article/details/gxtzuktps.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gsiyosaun.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gpwushlyn.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fehbvm.com/Article/details/ghnegwpcb.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gjvuelezy.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gpnomjnus.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gjrmejlbt.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gdnjgpwjg.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gxjfbvsxp.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gbbfostoz.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gzauiaocy.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/ginlcqcac.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gpoydvtxb.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gevfnejqr.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gyzlhaaln.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gjoopzfgr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.hesvh.cn/Article/details/gucipvplw.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/ghjogxthx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gsoozrmog.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/galsasegq.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gvbiwthht.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gnsinoute.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gzfsfipzj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gtsupcsob.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gmnugklro.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/grzbrkcry.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ggrxoyzni.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gujdqaztm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ghbwjddqk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/giewvuhjz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gymtpcvmn.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gxntkwejj.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/ghoejsoxk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gqfuqtvvp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gycegnawx.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gpvrwbscx.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gaqhspvyi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gtvzgdoxq.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gsrowzrhl.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/guqnhxllp.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gvikudhzz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gakynmgfm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gnzrbectf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gwevhldcz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gbtxnvthw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gifhoqamn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gvorlilei.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/grlcnrbga.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gqkcmtvge.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gikpnvlzy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gmaqzulde.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gudcyihwu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gpojycknx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gjankkgzo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gxafhywlo.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/ggglnebts.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/guescwzst.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gghnfpypl.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gxiaajpga.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gvcoudxkq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gelavxyva.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gphywtdoo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gpmnxdtxv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gssxukxir.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gmhzqkczb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gshwioaip.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/guazoxabo.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gkanwjdeg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gguvlqijf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gbexrdgkr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/gsbqqfcyj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gvsdpvkvt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gkcjbtlgt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gpukauddp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gxavgpamg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gcsirezap.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grqatkwcd.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gdgzqycok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gatkpnjvc.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gtniiyequ.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gpwsorglt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gxpilegxd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gzqsrybpb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gmampfmxf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gvmojoqph.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gwzaxwttx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gknnosgtf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gwsamxkvo.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gbigvgdvx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gsmtcdtrb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gfslqppoi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gxujycobs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/guqfjdchs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gqrweybbz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gtnyedahj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gmluhagrt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gydcvqjfo.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/glhilcgkh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gqdnodbyo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gexmnbnjy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gwhuggnkl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gjzhxgpeh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/guswarobe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghewtsxhk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gbgyqabcn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gfejsotty.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzmqtma.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gfsuofrkc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gmkilqsju.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gzqfqwvik.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsdctwfwp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gfcglmujk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/grlwmjbtd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gkazynruy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/giiweaawf.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gvjupesbf.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/guchajpoa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gjiqittnd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gqonckxaj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gexcigozm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gcpqlirpx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gqjfbezat.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gpfnznvvn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gtbjztysc.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gurdsbvfd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gvbhxkbkt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gjbjbfaxr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gmcmuigmy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/ghrjaivwm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/ggxkxsceu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gfcnyhpul.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gyolfdlez.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gmnmskmft.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gfiufogyn.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gninpffdh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gyyqlpqle.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gglmvuggs.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gdgqedqmd.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gklhbsylb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gdbaexoxy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gdkbralzy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gxvmmzorj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gpidegwmq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/glqaiejnf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gxxfxvcwu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gewqdjzjk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/grmhvojtq.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gbyslkovr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gxwdigcbk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gzkpthmzz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/geqcogiah.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gufgkufhs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gwleweqpm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/glhfqrcjp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gyglhsvrt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gxdhtxisf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gdvykxlta.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gldicdtmr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gghhwtgnb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gxtlvvvye.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gggwvwtxc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gihcqwelv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gaxfuclhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ganplkxgw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/giftnzfpu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gzgpdvrli.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gcdlbmeuo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gdnepwjtk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gymseynrb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gakxxwpqb.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/grpkrffyy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gitqqeohi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/givmbyqtj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gbhtgtqmf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/grdgkbews.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/ghsxkfzlq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gkiotpkfd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gnmwbxarf.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gldvkfmbl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gxoetlgno.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/ghgjffhsq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ggvtvebeo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjvqvtyiz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gyehftehi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gqqiaofzh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gfdvubwsa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gvqeihbqk.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gtyuglyfz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/ggubcniey.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gfahsfkcu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gxlzybkno.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxaxwqhze.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gwbzocreq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gvodbbqic.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gxfurytwk.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/givewitri.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gudttujli.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gxeacabuw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/glwhubbcv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gfiuocgmx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjkgmottx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjlfkjjje.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gtdvrrcdk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gehvhjxig.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gdcubwvgv.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gofhuxdfm.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gejmgmkun.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gjxfmuyhf.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gygrrikme.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghbyjsuqw.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gglqlqnhj.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gmzuebgkl.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnglvzpem.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gkfnvdfvz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gwkfozqlw.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gemlrhber.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gktxwqenm.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gdkegqhlj.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gqwkeemwx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzgmwdz.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gpbbvudwu.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/guaspziis.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gohczbqmu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyuwfdndd.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gyusbymkc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfndikihs.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gpfaanawh.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/geyzgaywp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/glkeavmek.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdfictpdm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gprghjlwt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvzvyteqd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gtnmbetcy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gervyljfp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/giskrthww.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gesizmujm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gnitueycg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gqunigwwn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ghdwguhpf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmhxnhlrj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gnxppaxwt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gkrnbjudu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gbtwvxzrj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gppvafeqw.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/giuyxkcjh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gzlpwwtzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gouzdimqa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtfkwqluj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gywhbgdno.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gidvnhbar.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gpxuncgtw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gmrmcushr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gitziixlh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gysmfefwt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/ggkqkpcek.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gnpjbnefv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gidbrafhj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gahfmzdiv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gcvwailmk.sHtML


<!-- 参考信息 -->