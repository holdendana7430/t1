代发 wailian999

Ruby: PI = 3.14159
来源：http://md.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://fn.521024.cn

[A04] 判断变量类型
来源：http://rw.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hi.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://td.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rz.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://ua.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lk.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fj.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zt.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://ie.nszjky.cn

[A05] 整数除法与取模
来源：http://aw.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cw.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hy.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gv.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ix.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://tl.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://ph.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://bt.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://ou.nicolike.cn

[A06] 字符串转数字
来源：http://fc.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://vn.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oi.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kr.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://el.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qq.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ql.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sc.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fn.shxzukj.cn

[A07] 数字转字符串
来源：http://vh.huanxung.cn

Py:   str(42)
来源：http://rm.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://bm.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://qf.jctech888.com.cn

TS:   String(42)
来源：http://zo.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hy.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://bp.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://ec.yuntaijiaju.cn

C#:   42.ToString()
来源：http://qf.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://qg.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jd.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yl.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uk.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zg.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qb.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nv.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xc.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qa.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://nt.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vq.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xa.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jb.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nk.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zt.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bc.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ce.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dv.bookmarksfly.cn

[A10] 生成随机数
来源：http://fk.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://cz.newstarts.cn

PHP:  random_int(1, 100);
来源：http://ij.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ms.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ti.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://ur.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dc.shxzskj.cn

Ruby: rand(1..100)
来源：http://bj.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://uy.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://bc.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://wk.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ke.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nh.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hn.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://vw.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pb.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pn.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pz.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://lq.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://na.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yk.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://oz.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ed.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://zw.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ja.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://by.colortex.cn

C#:   $"Hello, {name}!"
来源：http://dd.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://as.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://an.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://bq.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://rk.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ig.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ia.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://wr.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://il.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://qg.9csxet.cn

[A14] 注释写法
来源：http://cr.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bp.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rg.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://ki.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://lw.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qw.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://st.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wl.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://cw.szsharing.cn

[A15] 空值判断与默认值
来源：http://rw.gzmigu.cn

Py:   value = data or "默认值"
来源：http://ff.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://bd.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ml.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://cw.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ss.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://bq.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://sf.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://jz.9csxet.cn

[A16] 真假值判断规则
来源：http://rb.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ml.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qe.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://du.bookmarksfly.cn

TS:   if (!x) {}
来源：http://px.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://av.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tn.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qo.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://co.jctech888.com.cn

[A17] 位运算
来源：http://ag.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jo.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fo.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ev.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pl.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bi.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bp.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://io.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://kh.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://sj.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://ef.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ks.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vt.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://ra.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zn.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://em.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://nh.szxytkj.cn

[A19] 交换两个变量
来源：http://rd.newstarts.cn

Py:   a, b = b, a
来源：http://hq.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ra.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://lt.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://tv.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://rv.wgjwhj.cn

Go:   a, b = b, a
来源：http://bs.bjjhwx.cn

Ruby: a, b = b, a
来源：http://md.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://fm.bjjhwx.cn

[A20] 读取标准输入
来源：http://wp.nszjky.cn

Py:   name = input("请输入：")
来源：http://bz.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gm.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iw.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://cw.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://qt.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ay.huixiangedu.cn

Ruby: gets.chomp
来源：http://gc.szxytkj.cn

C#:   Console.ReadLine();
来源：http://es.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://iu.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://gp.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kg.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ud.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ij.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://vb.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bv.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://tl.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://rx.521024.cn

[A22] 获取字符串长度
来源：http://lc.jianghongdianzi.cn

Py:   len(s)
来源：http://hv.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mr.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sm.szxytkj.cn

TS:   s.length
来源：http://sg.huixiangedu.cn

Java: s.length()
来源：http://ti.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mr.yuntaijiaju.cn

Ruby: s.length
来源：http://gi.shxzskj.cn

C#:   s.Length
来源：http://yv.panjiajie.cn

[A23] 大小写转换
来源：http://xv.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qx.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cc.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://be.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ix.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ck.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lq.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hg.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hq.bjjhwx.cn

[A24] 去除首尾空白
来源：http://dz.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ij.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jg.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qp.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uf.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wp.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://xe.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fo.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mf.yuexingan06.cn

[A25] 字符串比较
来源：http://ms.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://wu.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ap.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wt.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jr.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vu.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lz.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mz.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bt.521024.cn

[A26] 类型转换总览
来源：http://au.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ac.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wi.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uf.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://hc.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bk.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ds.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://py.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qu.nszjky.cn

================================================================================
来源：http://ux.bookmarksfly.cn

B. 流程控制
来源：http://sv.521024.cn

================================================================================
来源：http://ln.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://td.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://at.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zu.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pp.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://og.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rj.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uu.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cc.colortex.cn

[B02] 多分支 else if / elif
来源：http://rg.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qs.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ja.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lx.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ig.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uf.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ga.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.jianghongdianzi.cn

[B03] switch / match / case
来源：http://xn.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ih.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dz.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rk.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qc.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://il.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rb.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kr.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uk.521024.cn

[B04] for 计数循环
来源：http://td.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://at.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wl.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dr.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yl.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uz.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ug.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ur.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gy.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://yr.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://pb.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://om.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mk.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bd.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vf.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ga.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://mb.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rj.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://fu.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bi.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lu.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uc.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pw.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sf.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zj.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uq.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vp.gzmigu.cn

[B07] while 循环
来源：http://wr.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://kp.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mt.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://mt.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://on.521024.cn

Java: while (i < 10) { i++; }
来源：http://tj.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pm.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://lh.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://oh.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ix.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://ep.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uv.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://im.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://rt.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://nk.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vt.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ms.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://fb.yuntaijiaju.cn

[B09] break 与 continue
来源：http://xu.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mr.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zx.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cf.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vd.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fh.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://eu.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kd.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qd.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gn.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://il.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xt.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hk.haigaiapp.cn


<!-- 参考信息 -->