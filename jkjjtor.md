代发 wailian999

Ruby: PI = 3.14159
来源：http://iu.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://cy.lnxyls.cn

[A04] 判断变量类型
来源：http://nk.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aw.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ds.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pe.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://if.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ve.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://op.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gl.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://tk.asd995.cn

[A05] 整数除法与取模
来源：http://ez.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ne.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oj.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hp.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pq.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://vf.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://di.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ux.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ex.lnxyls.cn

[A06] 字符串转数字
来源：http://et.asd995.cn

Py:   int("42"); float("3.14")
来源：http://ua.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qv.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pc.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cc.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mb.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://io.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oy.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nb.shxzskj.cn

[A07] 数字转字符串
来源：http://wh.szsharing.cn

Py:   str(42)
来源：http://ca.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ln.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://ev.szsharing.cn

TS:   String(42)
来源：http://qk.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wd.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://tc.wgjwhj.cn

Ruby: 42.to_s
来源：http://qm.newstarts.cn

C#:   42.ToString()
来源：http://pi.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://hf.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qf.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xf.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zh.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iq.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jg.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ic.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fz.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qg.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://oa.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ba.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hi.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kz.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kz.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sg.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://go.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rk.wgjwhj.cn

[A10] 生成随机数
来源：http://ft.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://aq.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ai.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mp.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fr.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ro.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sq.muxihuayi.cn

Ruby: rand(1..100)
来源：http://nh.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://eq.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://zd.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://iq.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cb.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lq.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tw.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://fk.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nx.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mg.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ql.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://zv.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cj.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gz.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://eg.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://tn.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://xm.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wf.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://jj.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://dt.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ns.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://yb.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://eb.nicolike.cn

JS:   "第一行\n第二行"
来源：http://cn.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://et.hnjuh.cn

Java: "第一行\n第二行"
来源：http://uw.huanxung.cn

Go:   "第一行\n第二行"
来源：http://xh.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://xk.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://bw.colortex.cn

[A14] 注释写法
来源：http://ik.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fj.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uj.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://us.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://cw.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jw.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://xb.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xk.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://ia.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://op.9csxet.cn

Py:   value = data or "默认值"
来源：http://lh.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://pe.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://wu.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://gd.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dm.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://qd.nszjky.cn

Ruby: value = data || "默认值"
来源：http://ha.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://th.huixiangedu.cn

[A16] 真假值判断规则
来源：http://gv.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ei.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://td.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ih.lnxyls.cn

TS:   if (!x) {}
来源：http://qj.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ga.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lv.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cm.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lv.asd995.cn

[A17] 位运算
来源：http://ed.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vq.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yx.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ri.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hv.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://nc.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://dj.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://pm.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ul.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zp.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://ap.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sy.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ox.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ge.szxytkj.cn

[A19] 交换两个变量
来源：http://zw.muxihuayi.cn

Py:   a, b = b, a
来源：http://rm.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ea.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://xj.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://fu.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://pr.hnjuh.cn

Go:   a, b = b, a
来源：http://fg.bjjhwx.cn

Ruby: a, b = b, a
来源：http://yt.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://vy.521024.cn

[A20] 读取标准输入
来源：http://cm.9csxet.cn

Py:   name = input("请输入：")
来源：http://mr.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pv.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yi.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://jn.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://eb.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fx.huixiangedu.cn

Ruby: gets.chomp
来源：http://yv.huanxung.cn

C#:   Console.ReadLine();
来源：http://ry.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://dx.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://ch.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tk.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://vg.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://rq.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ob.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ox.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://ff.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://fc.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ho.wgjwhj.cn

Py:   len(s)
来源：http://tw.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mb.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hk.hnjuh.cn

TS:   s.length
来源：http://tu.panjiajie.cn

Java: s.length()
来源：http://tp.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://op.haigaiapp.cn

Ruby: s.length
来源：http://ya.jianghongdianzi.cn

C#:   s.Length
来源：http://dh.huixinmuqiang.cn

[A23] 大小写转换
来源：http://oc.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://an.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://em.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lh.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xs.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vv.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ur.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jy.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://is.hnjuh.cn

[A24] 去除首尾空白
来源：http://ib.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ys.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wb.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ai.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gu.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yy.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ry.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aq.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rx.yuntaijiaju.cn

[A25] 字符串比较
来源：http://kz.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://as.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lv.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mo.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://no.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xy.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://se.panjiajie.cn

[A26] 类型转换总览
来源：http://wp.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oz.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ig.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yd.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://uj.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bj.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wb.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nt.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kn.shtwfgs.cn

================================================================================
来源：http://xh.hnjuh.cn

B. 流程控制
来源：http://ei.lnxyls.cn

================================================================================
来源：http://ba.colortex.cn

[B01] 条件判断 if / else
来源：http://vn.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fc.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zd.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yl.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ey.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fk.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vj.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://du.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hv.asd995.cn

[B02] 多分支 else if / elif
来源：http://hy.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://em.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ob.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wv.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tx.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.nszjky.cn

[B03] switch / match / case
来源：http://ep.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sc.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tl.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ic.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pn.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ij.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fu.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qy.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lo.yuexingan06.cn

[B04] for 计数循环
来源：http://gi.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://vh.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iv.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qv.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jc.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://am.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vl.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ng.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sf.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://sy.nicolike.cn

Py:   for item in arr: print(item)
来源：http://tf.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ix.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://di.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ox.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pt.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gd.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://qc.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sh.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://aa.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qs.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kl.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zl.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://is.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kl.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xo.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ua.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gn.yuntaijiaju.cn

[B07] while 循环
来源：http://la.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://jq.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://na.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://mx.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://py.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://yr.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tr.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://ec.521024.cn

C#:   while (i < 10) { i++; }
来源：http://tf.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://pf.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://tt.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://cl.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://ky.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://ow.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lw.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://dq.521024.cn

[B09] break 与 continue
来源：http://ls.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fy.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pe.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xt.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ao.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tr.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://bi.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ri.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zh.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://of.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bm.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pe.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aw.jianghongdianzi.cn


<!-- 参考信息 -->