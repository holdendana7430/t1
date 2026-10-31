代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bc.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://yk.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://xb.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://fj.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mt.huixinmuqiang.cn

[A03] 常量定义
来源：http://cp.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yz.asd995.cn

PHP:  const PI = 3.14159;
来源：http://ew.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://uz.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://yh.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ui.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://co.lnxyls.cn

Ruby: PI = 3.14159
来源：http://qn.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://rt.huixiangedu.cn

[A04] 判断变量类型
来源：http://xf.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://se.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wg.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gg.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://wh.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ur.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gv.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yk.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://pw.bjjhwx.cn

[A05] 整数除法与取模
来源：http://lk.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ep.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ic.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bz.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vu.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://ka.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://ar.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://nf.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://it.bookmarksfly.cn

[A06] 字符串转数字
来源：http://ii.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://yo.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wn.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ev.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fy.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://io.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ku.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ap.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ao.9csxet.cn

[A07] 数字转字符串
来源：http://um.shtwfgs.cn

Py:   str(42)
来源：http://yw.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://gy.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://ze.huanxung.cn

TS:   String(42)
来源：http://rg.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rn.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://ns.panjiajie.cn

Ruby: 42.to_s
来源：http://wk.yuexingan06.cn

C#:   42.ToString()
来源：http://hw.gzmigu.cn

[A08] 取整与四舍五入
来源：http://hy.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cd.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jx.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jp.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zr.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://td.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jb.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cl.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iu.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://ak.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://md.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gi.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ck.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rr.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yh.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ix.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rz.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xi.szxytkj.cn

[A10] 生成随机数
来源：http://gk.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://su.huanxung.cn

PHP:  random_int(1, 100);
来源：http://vu.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ow.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oo.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://xm.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wm.gzmigu.cn

Ruby: rand(1..100)
来源：http://gp.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://vg.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://wn.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://hn.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cp.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xd.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jn.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://qx.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nj.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rc.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ve.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://bn.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://la.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://to.colortex.cn

JS:   `Hello, ${name}!`
来源：http://mg.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://oy.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://kd.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ns.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://qt.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://yu.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://do.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://qa.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://rf.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://ar.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://uy.521024.cn

Java: "第一行\n第二行"
来源：http://bi.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://zt.asd995.cn

Ruby: "第一行\n第二行"
来源：http://nv.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://wn.hahajie.cn

[A14] 注释写法
来源：http://da.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ay.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sf.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ws.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://jc.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://al.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://nj.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ry.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ky.shxzukj.cn

[A15] 空值判断与默认值
来源：http://gb.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ch.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://nz.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://ou.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://tc.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cr.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://ui.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://pw.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://fr.szsharing.cn

[A16] 真假值判断规则
来源：http://wa.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wq.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tq.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ej.bookmarksfly.cn

TS:   if (!x) {}
来源：http://pr.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pj.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kd.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zn.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wx.asd995.cn

[A17] 位运算
来源：http://wv.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://db.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://li.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vu.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fy.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hw.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xn.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zc.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://my.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://kf.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ku.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ia.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://me.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://xr.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qt.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://hk.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://yz.huanxung.cn

[A19] 交换两个变量
来源：http://kj.bookmarksfly.cn

Py:   a, b = b, a
来源：http://il.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ur.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://yq.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://ym.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://gt.nszjky.cn

Go:   a, b = b, a
来源：http://qu.521024.cn

Ruby: a, b = b, a
来源：http://kq.asd995.cn

C#:   (a, b) = (b, a);
来源：http://bl.wgjwhj.cn

[A20] 读取标准输入
来源：http://rp.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ek.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wc.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gz.asd995.cn

TS:   // Node.js：readline 模块
来源：http://xo.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://qn.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vh.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://re.newstarts.cn

C#:   Console.ReadLine();
来源：http://xt.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://po.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://kf.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zb.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://sr.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://rr.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://as.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ea.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://nz.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://um.shxzukj.cn

[A22] 获取字符串长度
来源：http://lp.haigaiapp.cn

Py:   len(s)
来源：http://xp.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ha.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mx.colortex.cn

TS:   s.length
来源：http://ur.asd995.cn

Java: s.length()
来源：http://of.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gq.gzmigu.cn

Ruby: s.length
来源：http://bh.chemitech.net.cn

C#:   s.Length
来源：http://qx.colortex.cn

[A23] 大小写转换
来源：http://lm.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://is.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fu.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qu.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mg.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://he.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vx.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pp.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sp.newstarts.cn

[A24] 去除首尾空白
来源：http://my.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ps.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kb.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mo.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zw.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vu.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://sn.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ca.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yj.newstarts.cn

[A25] 字符串比较
来源：http://je.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ov.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bm.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ky.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pn.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://he.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://po.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cy.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fm.huixiangedu.cn

[A26] 类型转换总览
来源：http://vs.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ii.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xs.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qz.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://lu.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bs.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://po.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dd.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kh.gzmigu.cn

================================================================================
来源：http://xu.huanxung.cn

B. 流程控制
来源：http://rd.shtwfgs.cn

================================================================================
来源：http://ca.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://jm.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mj.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cj.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tb.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bg.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aq.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nz.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gx.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://id.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://vk.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://km.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://di.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ba.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gy.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xn.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hl.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.szsharing.cn

[B03] switch / match / case
来源：http://eo.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rx.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xk.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://so.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cz.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ol.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sc.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gb.szsharing.cn

[B04] for 计数循环
来源：http://ny.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://th.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iv.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qr.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nj.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ub.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tc.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://op.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xu.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ij.colortex.cn

Py:   for item in arr: print(item)
来源：http://ki.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ml.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aj.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qn.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kk.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mj.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://cp.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ri.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://sr.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yf.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hy.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wn.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://we.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fd.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wf.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rw.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oi.hahajie.cn

[B07] while 循环
来源：http://yc.asd995.cn

Py:   while i < 10: i += 1
来源：http://cc.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ns.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://qg.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://gw.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://bw.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oc.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://sr.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://pw.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://rv.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ar.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dt.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://kc.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://tq.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://zn.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rc.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://up.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://pp.szxytkj.cn

[B09] break 与 continue
来源：http://rm.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qs.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rv.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.huanxung.cn


<!-- 参考信息 -->