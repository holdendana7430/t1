代发 wailian999

[A02] 变量声明与赋值
来源：http://lv.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jx.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://of.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xm.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pu.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://ac.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://gy.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://rc.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cz.shxzskj.cn

[A03] 常量定义
来源：http://se.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yz.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ed.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://ci.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://fd.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://mo.gzmigu.cn

Go:   const PI = 3.14159
来源：http://sn.asd995.cn

Ruby: PI = 3.14159
来源：http://yb.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://wi.bookmarksfly.cn

[A04] 判断变量类型
来源：http://yc.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dc.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hv.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ng.521024.cn

TS:   typeof x; x instanceof Date
来源：http://xv.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xo.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kh.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uy.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://yj.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://lr.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ey.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xp.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ra.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jx.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://va.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://dx.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://wg.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://xk.huanxung.cn

[A06] 字符串转数字
来源：http://zu.colortex.cn

Py:   int("42"); float("3.14")
来源：http://jn.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://su.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pv.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dd.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ib.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://by.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ui.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uf.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://co.hnjuh.cn

Py:   str(42)
来源：http://cg.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://uj.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://pz.huanxung.cn

TS:   String(42)
来源：http://zv.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nb.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://tz.jctech888.com.cn

Ruby: 42.to_s
来源：http://wh.shxzskj.cn

C#:   42.ToString()
来源：http://cn.shxzukj.cn

[A08] 取整与四舍五入
来源：http://jy.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ox.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wb.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sc.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ib.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uy.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sq.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pr.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qs.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://nc.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xj.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fq.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ut.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iy.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ym.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qa.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://na.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://me.gzmigu.cn

[A10] 生成随机数
来源：http://gw.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://ga.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://te.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lc.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://on.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://io.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rm.szxytkj.cn

Ruby: rand(1..100)
来源：http://ze.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://nb.hahajie.cn

[A11] 条件表达式（三元）
来源：http://vh.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://mc.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bc.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jo.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mi.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://mn.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pv.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://em.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vz.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://ys.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zx.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kf.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://qg.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://qd.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://xu.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vs.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://aj.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://rp.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hi.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://hk.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://qu.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://sy.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://dj.szsharing.cn

Java: "第一行\n第二行"
来源：http://dy.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://wt.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://oh.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://er.bookmarksfly.cn

[A14] 注释写法
来源：http://yn.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bd.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rd.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://nz.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://vm.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gq.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://db.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sp.521024.cn

C#:   // 单行；/* 多行 */
来源：http://li.huanxung.cn

[A15] 空值判断与默认值
来源：http://vs.hnjuh.cn

Py:   value = data or "默认值"
来源：http://vo.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ia.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://qx.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://jl.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cg.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://yd.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ql.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://kx.haigaiapp.cn

[A16] 真假值判断规则
来源：http://dl.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cp.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dk.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iv.gzmigu.cn

TS:   if (!x) {}
来源：http://yj.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vg.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://va.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lz.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zq.szxytkj.cn

[A17] 位运算
来源：http://zv.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jn.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hf.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ez.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rw.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iu.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ct.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://os.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://pt.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://yl.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://np.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sg.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://dj.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qq.521024.cn

Ruby: "A".ord; 65.chr
来源：http://di.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://vk.huixiangedu.cn

[A19] 交换两个变量
来源：http://bd.9csxet.cn

Py:   a, b = b, a
来源：http://zc.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yz.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://ct.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://lm.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://ao.shxzukj.cn

Go:   a, b = b, a
来源：http://zg.nszjky.cn

Ruby: a, b = b, a
来源：http://yr.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://fd.newstarts.cn

[A20] 读取标准输入
来源：http://wr.colortex.cn

Py:   name = input("请输入：")
来源：http://mc.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ag.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://up.asd995.cn

TS:   // Node.js：readline 模块
来源：http://zl.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://dm.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rb.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://ny.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://qd.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://ah.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://ez.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://im.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://xt.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ex.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://tq.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fy.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://hp.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://pj.newstarts.cn

[A22] 获取字符串长度
来源：http://up.bjjhwx.cn

Py:   len(s)
来源：http://ju.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ad.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dg.huanxung.cn

TS:   s.length
来源：http://nm.lnxyls.cn

Java: s.length()
来源：http://ro.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tm.jianghongdianzi.cn

Ruby: s.length
来源：http://wm.hahajie.cn

C#:   s.Length
来源：http://jb.shxzukj.cn

[A23] 大小写转换
来源：http://wy.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bj.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dx.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zj.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ru.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ch.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zg.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hk.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zz.521024.cn

[A24] 去除首尾空白
来源：http://qr.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sb.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jw.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jo.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nd.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://zm.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rc.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sa.shxzskj.cn

[A25] 字符串比较
来源：http://fb.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://ob.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://po.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bz.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://px.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ps.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://je.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nb.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cr.lnxyls.cn

[A26] 类型转换总览
来源：http://fj.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ao.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rz.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ys.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://im.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ec.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://io.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yr.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zp.muxihuayi.cn

================================================================================
来源：http://yb.shxzukj.cn

B. 流程控制
来源：http://ly.yuntaijiaju.cn

================================================================================
来源：http://sv.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://mg.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ck.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mt.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jm.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jm.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kw.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ct.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ci.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cj.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://le.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lr.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ah.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rf.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xk.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pa.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fl.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.colortex.cn

[B03] switch / match / case
来源：http://fr.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nb.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rw.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jw.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hb.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cs.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hg.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fd.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nb.szxytkj.cn

[B04] for 计数循环
来源：http://ky.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://gr.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://md.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gp.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zf.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qn.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://sd.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://te.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://dj.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://of.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ts.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://it.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hk.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lg.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xr.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://gk.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://da.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://wz.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://su.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cd.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://il.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wf.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://si.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://la.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rt.colortex.cn

[B07] while 循环
来源：http://vg.colortex.cn

Py:   while i < 10: i += 1
来源：http://dj.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://qn.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://dc.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://gm.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tg.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://ue.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://qh.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://au.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://cr.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tu.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://lp.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ie.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://mb.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lq.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xu.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://nd.yuntaijiaju.cn


<!-- 参考信息 -->