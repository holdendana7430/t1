代发 wailian999

JS:   const PI = 3.14159;
来源：http://ux.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://zo.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://qz.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://oq.asd995.cn

Ruby: PI = 3.14159
来源：http://gx.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://tb.colortex.cn

[A04] 判断变量类型
来源：http://rw.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pg.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qw.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://db.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://de.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ab.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cp.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ay.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://nl.szsharing.cn

[A05] 整数除法与取模
来源：http://ad.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://za.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ti.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qi.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://yk.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://od.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://pn.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://me.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://wn.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://wt.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ii.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wn.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rs.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ft.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nh.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bi.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lg.521024.cn

[A07] 数字转字符串
来源：http://vx.haigaiapp.cn

Py:   str(42)
来源：http://xb.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://py.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://rl.newstarts.cn

TS:   String(42)
来源：http://hu.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vd.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://xl.muxihuayi.cn

Ruby: 42.to_s
来源：http://xz.szxytkj.cn

C#:   42.ToString()
来源：http://js.szsharing.cn

[A08] 取整与四舍五入
来源：http://mw.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fe.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sy.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://om.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://in.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sb.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rb.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wx.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://by.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://bd.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rg.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uo.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jt.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://se.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qe.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rv.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://de.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ip.shtwfgs.cn

[A10] 生成随机数
来源：http://be.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://pt.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://bi.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://me.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://jl.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lw.szsharing.cn

Ruby: rand(1..100)
来源：http://hd.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://cs.szsharing.cn

[A11] 条件表达式（三元）
来源：http://hj.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://fk.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lq.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mi.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nm.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://xj.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ni.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yx.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sq.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://km.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sw.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://us.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://of.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://xz.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://xn.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cg.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://cy.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://rq.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://th.nicolike.cn

Py:   "第一行\n第二行"
来源：http://qs.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://mo.colortex.cn

JS:   "第一行\n第二行"
来源：http://ui.9csxet.cn

TS:   "第一行\n第二行"
来源：http://gi.szxytkj.cn

Java: "第一行\n第二行"
来源：http://fe.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://em.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://of.huanxung.cn

C#:   "第一行\n第二行"
来源：http://ne.yuexingan06.cn

[A14] 注释写法
来源：http://ru.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://da.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tz.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://sq.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://qr.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uh.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://kr.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://du.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ss.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://fx.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://ui.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://on.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://df.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://vm.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qd.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://wq.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://qv.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://jm.yuexingan06.cn

[A16] 真假值判断规则
来源：http://tt.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eh.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ii.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rk.asd995.cn

TS:   if (!x) {}
来源：http://yh.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://la.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aq.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tz.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://db.huixiangedu.cn

[A17] 位运算
来源：http://wo.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lx.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lh.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tc.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aa.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ch.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sp.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://vi.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://fi.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://wj.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nq.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cf.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://lr.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yp.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://fa.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://xv.chemitech.net.cn

[A19] 交换两个变量
来源：http://av.newstarts.cn

Py:   a, b = b, a
来源：http://nq.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cy.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://na.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://oc.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://yn.szsharing.cn

Go:   a, b = b, a
来源：http://uy.521024.cn

Ruby: a, b = b, a
来源：http://da.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://at.szxytkj.cn

[A20] 读取标准输入
来源：http://vb.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://jp.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pj.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iw.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ru.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://tl.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mw.gzmigu.cn

Ruby: gets.chomp
来源：http://bp.nszjky.cn

C#:   Console.ReadLine();
来源：http://as.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://oj.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://vh.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yc.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://yn.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://lc.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://to.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pr.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://jf.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://lr.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://ro.yuntaijiaju.cn

Py:   len(s)
来源：http://je.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hx.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lu.bjjhwx.cn

TS:   s.length
来源：http://kp.panjiajie.cn

Java: s.length()
来源：http://lc.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zk.huixiangedu.cn

Ruby: s.length
来源：http://vp.shxzskj.cn

C#:   s.Length
来源：http://en.huixiangedu.cn

[A23] 大小写转换
来源：http://mf.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://am.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ht.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dv.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xe.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fk.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ik.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://if.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://bl.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ad.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lb.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mm.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://my.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ps.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://ak.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pz.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uz.chemitech.net.cn

[A25] 字符串比较
来源：http://gf.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://mz.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pz.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gk.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nq.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iz.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zz.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eo.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ot.shxzukj.cn

[A26] 类型转换总览
来源：http://fd.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://li.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hn.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ea.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://jk.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mu.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mv.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ds.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wp.szsharing.cn

================================================================================
来源：http://dz.jianghongdianzi.cn

B. 流程控制
来源：http://fk.bjjhwx.cn

================================================================================
来源：http://pu.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://xe.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vt.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yg.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qa.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oz.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vm.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://am.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://le.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jp.521024.cn

[B02] 多分支 else if / elif
来源：http://di.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qt.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nt.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dy.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ai.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dg.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.yuntaijiaju.cn

[B03] switch / match / case
来源：http://lv.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mv.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bv.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tb.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vy.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nh.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ao.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nr.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ix.hnjuh.cn

[B04] for 计数循环
来源：http://mr.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://lm.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bb.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gl.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kf.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ea.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zo.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://vc.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fr.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://fe.asd995.cn

Py:   for item in arr: print(item)
来源：http://bt.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lg.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ft.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yz.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eo.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dk.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://oa.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eq.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://hy.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ta.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wm.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tg.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://af.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tw.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kj.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gf.hnjuh.cn

[B07] while 循环
来源：http://zo.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://oa.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bv.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://zo.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://fp.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://sk.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oi.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://ux.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://vi.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://na.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://vp.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ye.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ds.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://qg.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ei.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uh.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cy.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://pe.bjjhwx.cn

[B09] break 与 continue
来源：http://za.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vn.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iu.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gd.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lx.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://na.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jk.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://cy.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://du.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ar.521024.cn


<!-- 参考信息 -->