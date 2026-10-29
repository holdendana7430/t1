代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gjwlbqeyi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtinnvrmp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/grvxmxlkd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gslpuyzch.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gnseemvmh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gqadlnsyr.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gtzfzodee.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gkcqqlfya.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gqxrheltd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gdjmmzdss.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gjlibbxzi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gpgpxigze.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gjtxmkcdk.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gmglnqqgd.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gxhibkotn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gdrddexfy.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzujdmkvz.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gkzbgwzex.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gcmdltrjw.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gauqfordt.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gcvgzntme.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwgcaphdi.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/giajhxout.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggktrnykc.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gcegbzwob.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gakwhxmlu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gldiowgux.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/glskhxptw.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gqtjvoteg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gvrjbwldn.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/ghljrsaxb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gmoowwefb.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gpoilvusn.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gxmlghwib.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gunixbvva.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gjxjuhilx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/ghqffjrmf.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gvynkldfd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/gzkukzqdb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/govyvoyhz.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gtvuhxgls.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gnyyizbwx.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/guqtigobn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gznqymdgk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gdzvfuvvc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gcepmclbn.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gvfgislsm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gnnmcewfn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.zdbjq.cn/Article/details/gjmwzngxf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gvzgngrlb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdhaeovzd.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gnlgkympk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gkfzaekbm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/glsdxjtdw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/grbhnddrm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gtpcjwfym.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grirktadn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gjrwgopne.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gojdjndal.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gsqbntrpm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gdddasacc.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gjrvxyfrs.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gkmxopgmc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gelvlkoxg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gqxndafkp.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fehbvm.com/Article/details/ggqtrxrkg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/getihwlwa.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gvbpjzskg.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/ggmxxyarv.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gsmnbpddy.sHtML

Py:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gcqegcsxv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gpwndyoqe.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/guldzrthx.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gnhygkbtm.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/ggoiipvsm.sHtML

Go:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gydrcreqw.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/guxkggghs.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/glxuunlmc.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gmkaqkjhi.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gyctdbhfx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/gberpnudu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gfatqlzma.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gntlnrtxk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/ggygsvtte.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gcnorkylr.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/ginuaeffo.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gsbkrfnrd.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/gpgwyxbib.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/gperhchqh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gdtrchwyw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/guxixtorm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ghkzwxfea.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gyqbfdyxs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gmlppsray.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gwpubwzaz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gsermlczr.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gvkgjdnxz.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbynhulhz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fehbvm.com/Article/details/gmuhvrdgt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gjtadztah.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gtuowwjga.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gbndwlour.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gdttwsqyv.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gapknfpjo.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gfnyonnpi.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gjemmxcgb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gwxdvfhcp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlnuaumh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gyfzfzusf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/ggpqmjxvj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/ghebhioow.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gwhaalbzc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gurzppgal.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gpdswvgfg.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gaojykwkx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gbmsebmzi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gaxrcbyyr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gkzmytuez.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gnyqzmrdx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gjtydynaq.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gwnwlywgx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gczqcpgng.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gyekbjzav.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gcazvrwxf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gnoiqgueb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gbctohfrv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gkeoghhcn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gjtbsowbh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gjrurqoox.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gtaybmksv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/ghoourizt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gydqrxmec.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gciedhfzu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gscexyfxp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gvpkzwfro.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gkswvpkov.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gudtngnid.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gcoornwyp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fehbvm.com/Article/details/gydtxafnn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/ghydwpheo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/ggnurpntl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsxflbswa.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gbdmfsrbb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpvynflyn.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gekdwhmhi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gtkwoozip.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gbdfcybnv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gyyctsoyj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gkprndncy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grkudpjpw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gftgllvbr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/genfnubsa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gysetmxqw.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gqvhyolrz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gvwscvefz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gzhiszxyj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/goezkheum.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gjoynkanp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gxxnkuyjq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gdpnswver.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/goltbxvan.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gnhiziogy.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gyexniiot.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gddtylriw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/ggvgivccp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gzdzvoylc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdedqkvql.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gwkdduatt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gtzzqbpcb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/ginoxiyvm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gduifrhuz.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gegnibqvo.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gyzufpbgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/ggrskjojj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gektllqci.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gonhctohk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gvfgclrjm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gbvlsxitw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gnumzvqal.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gwhncmnmo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gawldhyzs.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdayrrpro.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gtmkflvht.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/greqvjnwj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gjnmtdqmo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gntblqmtx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gdpnpdrdc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gzdctakmr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gseantzdj.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/ggbmfkkyz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/ghxnvczga.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/givvloqrj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/glvpmcauw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gbgtyzmnu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gdhjtasim.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gwliyzqlu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gtngotpxa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gxtnydhtl.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gjnycvdto.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gpdpssgrc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gcwloxrik.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/grsdlbren.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gavlsjwbx.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gcqbdhqdl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/ghnfsfsha.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gmoyvhhii.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/giyswbjzu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gcpmnjpyg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/geacrjrfg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gykqidzup.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/guhyisgxl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqmkjpeds.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/giygyeaxw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gogzuwlkf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gdafdzlyy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grdwtxdhd.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gypemrawa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gcspwenra.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghphumzmk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gzquuuokx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gflwjnkue.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gxetsdvto.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gtegzgoxt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gesavyrju.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grsixheem.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/giowlyxcr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gmnvxxtib.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/glufhfqzh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gcpgemwwf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/goqngrjur.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gnpyenxrt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gxjbnzgsw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmilhmhny.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gvnvtvklj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gkvuamiow.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gnwupyfkc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gmuvphfrc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gntpkovzl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpzpuirgy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gdehavvie.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gnkkkuyil.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gmgbukfqk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gdgexjtka.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gpalhzefb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/ggkemuzhi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gkysatkjv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gwpsnnxzd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gflotgdpo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gsnalxzwm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gphvdanjz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gnawcloks.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gtapemnrq.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gsgoacxnk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gqerabach.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gqxwgzuog.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/geepguebf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwypwthlo.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gnwnmofgn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gkwcfbvdc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/ggdflfsvv.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gpteoprge.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gckoohosl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/grtfphuvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfjqfgj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gupqrtoeh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkqwwcdbz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggplcpedk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gpgrtdcec.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gvjvpnapc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/graxygtxh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gnypwfqxs.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gygmhmjzb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gemgcaymj.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxomnuaez.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnypbhgzr.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gcrwnarps.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjbxyyxmi.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxsjjwsne.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfxjwxtbb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gwbdbfuqm.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvobaat.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gqwwmndeg.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gdkczbhsh.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gyrciummi.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gxzgabjcu.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gakpxbjud.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gvicwpgcv.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gmbvxlmql.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzeclucbp.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gqrejgbyq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcpyhyxni.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gkulmpefo.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gteozsnuu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwmebwmlc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guznmxujh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmztpyrjn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gzoxupcsh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhgyohsm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gennjzhus.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ggwfxfley.sHtML


<!-- 参考信息 -->