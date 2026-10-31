代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://jm.huanxung.cn

[A03] 常量定义
来源：http://gr.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ho.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://dl.hahajie.cn

JS:   const PI = 3.14159;
来源：http://eq.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://vg.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://ku.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://hs.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://hg.asd995.cn

C#:   const double PI = 3.14159;
来源：http://av.bookmarksfly.cn

[A04] 判断变量类型
来源：http://oa.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wz.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zy.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dy.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://xp.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zz.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ms.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mx.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://aj.colortex.cn

[A05] 整数除法与取模
来源：http://bo.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ud.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jz.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fz.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mv.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://up.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://he.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://if.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://cy.huanxung.cn

[A06] 字符串转数字
来源：http://yz.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://cs.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kn.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nr.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ng.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uc.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hr.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tu.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qp.shxzukj.cn

[A07] 数字转字符串
来源：http://yz.521024.cn

Py:   str(42)
来源：http://va.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://xk.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://ws.yuexingan06.cn

TS:   String(42)
来源：http://cb.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sa.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://np.huanxung.cn

Ruby: 42.to_s
来源：http://ka.yuexingan06.cn

C#:   42.ToString()
来源：http://ga.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://gh.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ty.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ca.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ue.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://az.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qi.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ct.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fx.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ck.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://bg.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uo.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vh.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qq.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fi.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iy.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bz.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dc.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vq.huanxung.cn

[A10] 生成随机数
来源：http://wx.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://ql.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://nh.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ye.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ib.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://ys.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ih.bjjhwx.cn

Ruby: rand(1..100)
来源：http://wd.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://jt.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://di.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://vs.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cj.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vu.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tx.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://xh.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yx.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iw.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iq.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://yc.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uk.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ba.521024.cn

JS:   `Hello, ${name}!`
来源：http://op.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://oi.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://lz.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xn.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://ll.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://th.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vh.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://sr.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://jc.521024.cn

JS:   "第一行\n第二行"
来源：http://km.newstarts.cn

TS:   "第一行\n第二行"
来源：http://eh.shxzskj.cn

Java: "第一行\n第二行"
来源：http://bk.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ku.colortex.cn

Ruby: "第一行\n第二行"
来源：http://wg.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://pi.panjiajie.cn

[A14] 注释写法
来源：http://ho.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pu.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://az.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ea.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://lc.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jl.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://du.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hl.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://fw.521024.cn

[A15] 空值判断与默认值
来源：http://st.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ui.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://bz.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ps.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://ry.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://it.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://zb.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://kt.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://cu.9csxet.cn

[A16] 真假值判断规则
来源：http://na.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bm.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nf.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mq.chemitech.net.cn

TS:   if (!x) {}
来源：http://yj.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ss.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zj.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pa.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wq.wgjwhj.cn

[A17] 位运算
来源：http://zp.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jf.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lu.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ac.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ed.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://se.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://tk.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://xw.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://qq.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rg.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zy.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ln.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lc.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://np.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://yb.shxzskj.cn

[A19] 交换两个变量
来源：http://pv.huanxung.cn

Py:   a, b = b, a
来源：http://fs.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yz.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://zj.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://iw.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://cn.shtwfgs.cn

Go:   a, b = b, a
来源：http://ag.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://lj.colortex.cn

C#:   (a, b) = (b, a);
来源：http://dq.bookmarksfly.cn

[A20] 读取标准输入
来源：http://us.nicolike.cn

Py:   name = input("请输入：")
来源：http://oi.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tq.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ew.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://na.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://fx.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://op.hahajie.cn

Ruby: gets.chomp
来源：http://iy.lnxyls.cn

C#:   Console.ReadLine();
来源：http://zh.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://rp.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ec.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jg.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://eg.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://cs.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ft.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://km.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://gs.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://fi.muxihuayi.cn

[A22] 获取字符串长度
来源：http://wm.yuntaijiaju.cn

Py:   len(s)
来源：http://fi.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wd.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yy.shxzskj.cn

TS:   s.length
来源：http://tc.shxzskj.cn

Java: s.length()
来源：http://zv.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cz.9csxet.cn

Ruby: s.length
来源：http://hm.muxihuayi.cn

C#:   s.Length
来源：http://ee.colortex.cn

[A23] 大小写转换
来源：http://at.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://td.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nk.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yk.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oe.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qu.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zx.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zj.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zh.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://tx.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fp.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gx.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kg.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ji.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wh.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://sx.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sn.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://os.521024.cn

[A25] 字符串比较
来源：http://go.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://nb.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hx.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wl.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vt.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rw.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rt.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ad.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mg.jctech888.com.cn

[A26] 类型转换总览
来源：http://cx.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sb.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://io.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yt.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://gk.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zb.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qq.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yc.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pc.huanxung.cn

================================================================================
来源：http://jq.huixiangedu.cn

B. 流程控制
来源：http://cv.hahajie.cn

================================================================================
来源：http://km.hahajie.cn

[B01] 条件判断 if / else
来源：http://qq.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dv.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qo.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xu.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dx.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kx.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ag.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zo.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wx.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://lf.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ts.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ab.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ej.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ay.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.wgjwhj.cn

[B03] switch / match / case
来源：http://kf.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bf.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lh.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qn.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hc.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oc.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nl.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ke.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vg.yuntaijiaju.cn

[B04] for 计数循环
来源：http://te.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ox.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oi.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://br.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kc.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://as.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gz.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://hi.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://md.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://me.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://dq.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uc.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sy.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gr.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jl.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://si.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://dm.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pq.521024.cn

[B06] 遍历字典 / 对象
来源：http://kt.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yt.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mh.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ch.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ot.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bq.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lf.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sg.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ck.haigaiapp.cn

[B07] while 循环
来源：http://qy.nicolike.cn

Py:   while i < 10: i += 1
来源：http://yt.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ma.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://pe.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://xa.colortex.cn

Java: while (i < 10) { i++; }
来源：http://ji.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bx.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://jy.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://tz.521024.cn

[B08] do-while（至少执行一次）
来源：http://on.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://dm.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://he.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://qr.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://ha.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://eg.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ip.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://af.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ax.lnxyls.cn

[B09] break 与 continue
来源：http://hm.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ir.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bk.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lx.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ge.huixinmuqiang.cn


<!-- 参考信息 -->