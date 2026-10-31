代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://tm.huanxung.cn

[A03] 常量定义
来源：http://qq.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ix.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://zr.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://zb.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://pe.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://qc.newstarts.cn

Go:   const PI = 3.14159
来源：http://yx.hahajie.cn

Ruby: PI = 3.14159
来源：http://hh.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://sl.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://pt.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dc.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yj.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gc.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://kl.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uq.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qq.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ph.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://by.yuexingan06.cn

[A05] 整数除法与取模
来源：http://so.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gf.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cn.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vw.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zv.521024.cn

Java: 7 / 2; 7 % 2
来源：http://ju.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://cs.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://pe.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://nz.huanxung.cn

[A06] 字符串转数字
来源：http://gz.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://pf.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rk.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ik.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ou.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rg.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fn.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://an.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mc.jctech888.com.cn

[A07] 数字转字符串
来源：http://gw.bjjhwx.cn

Py:   str(42)
来源：http://qt.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://mh.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://ac.lnxyls.cn

TS:   String(42)
来源：http://xt.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tt.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://st.hahajie.cn

Ruby: 42.to_s
来源：http://fo.asd995.cn

C#:   42.ToString()
来源：http://no.lnxyls.cn

[A08] 取整与四舍五入
来源：http://uc.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mf.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eh.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iu.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://is.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yc.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xa.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lu.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pg.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://bt.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lm.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xc.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ia.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ep.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xh.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nc.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xk.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yp.huixinmuqiang.cn

[A10] 生成随机数
来源：http://rs.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://ml.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://as.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://di.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cu.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://pb.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://or.chemitech.net.cn

Ruby: rand(1..100)
来源：http://fc.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://im.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://zm.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://eo.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nj.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yd.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ka.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://nc.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eq.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aj.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ev.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://qa.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mf.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ae.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://pm.521024.cn

TS:   `Hello, ${name}!`
来源：http://jw.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://de.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jh.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://oj.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://yt.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iw.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://ne.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://tx.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://tc.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://kh.nszjky.cn

Java: "第一行\n第二行"
来源：http://ft.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://he.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://mn.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://gs.bookmarksfly.cn

[A14] 注释写法
来源：http://bl.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uk.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ea.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://vl.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://tx.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qp.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://kq.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pf.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://ro.hnjuh.cn

[A15] 空值判断与默认值
来源：http://up.huanxung.cn

Py:   value = data or "默认值"
来源：http://ti.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://pw.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://dg.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://gu.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nz.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://df.asd995.cn

Ruby: value = data || "默认值"
来源：http://vi.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://he.9csxet.cn

[A16] 真假值判断规则
来源：http://jr.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bi.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lp.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nk.asd995.cn

TS:   if (!x) {}
来源：http://on.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oi.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uu.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fw.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lm.gzmigu.cn

[A17] 位运算
来源：http://pv.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mr.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dq.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://el.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hg.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ru.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bs.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dr.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://zr.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://vj.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://ft.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hv.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cu.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://pa.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ov.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://ey.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://aq.chemitech.net.cn

[A19] 交换两个变量
来源：http://bw.521024.cn

Py:   a, b = b, a
来源：http://de.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qe.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://sz.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://tq.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://kt.9csxet.cn

Go:   a, b = b, a
来源：http://tv.521024.cn

Ruby: a, b = b, a
来源：http://ot.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://dk.bjjhwx.cn

[A20] 读取标准输入
来源：http://bc.521024.cn

Py:   name = input("请输入：")
来源：http://kk.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oe.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mh.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://qv.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://mr.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qx.szsharing.cn

Ruby: gets.chomp
来源：http://wd.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ob.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://ed.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://zo.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ji.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://pz.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://fi.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://xg.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eq.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xi.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://cz.huanxung.cn

[A22] 获取字符串长度
来源：http://qz.bookmarksfly.cn

Py:   len(s)
来源：http://up.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ko.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ah.newstarts.cn

TS:   s.length
来源：http://eo.huixinmuqiang.cn

Java: s.length()
来源：http://ud.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tl.huanxung.cn

Ruby: s.length
来源：http://qk.bookmarksfly.cn

C#:   s.Length
来源：http://cc.huanxung.cn

[A23] 大小写转换
来源：http://kz.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://om.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nl.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dw.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ah.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qy.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xh.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qo.hnjuh.cn

[A24] 去除首尾空白
来源：http://lr.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qm.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nc.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lx.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ej.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gz.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://ue.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uz.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jn.gzmigu.cn

[A25] 字符串比较
来源：http://cn.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ng.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hj.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kh.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vn.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hq.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gy.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mv.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uv.huixiangedu.cn

[A26] 类型转换总览
来源：http://sn.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yj.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cu.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ay.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://pa.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ro.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cx.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ra.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jp.bookmarksfly.cn

================================================================================
来源：http://gx.lnxyls.cn

B. 流程控制
来源：http://vx.panjiajie.cn

================================================================================
来源：http://xn.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://rv.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fo.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://su.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oj.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wu.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oc.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sz.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tz.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uj.nicolike.cn

[B02] 多分支 else if / elif
来源：http://fx.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://re.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cf.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jj.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ou.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://js.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.shxzskj.cn

[B03] switch / match / case
来源：http://ah.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qa.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bb.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kk.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://to.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rc.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sd.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qs.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://la.wgjwhj.cn

[B04] for 计数循环
来源：http://ej.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://oi.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wh.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vb.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zz.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dk.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://tg.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pp.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://vd.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://zy.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mf.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eu.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gb.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ec.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xm.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://hd.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://im.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://mz.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lc.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rk.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://au.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wu.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ug.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gv.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sj.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zx.chemitech.net.cn

[B07] while 循环
来源：http://nl.szsharing.cn

Py:   while i < 10: i += 1
来源：http://bj.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://co.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://vy.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://lj.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://sc.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ek.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://au.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://rv.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://pn.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://xh.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jp.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://wh.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://xr.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://bc.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://im.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://be.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://de.nszjky.cn

[B09] break 与 continue
来源：http://pg.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mv.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ow.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mc.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://op.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uc.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://an.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zo.521024.cn


<!-- 参考信息 -->