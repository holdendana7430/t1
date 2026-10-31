代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://mm.nszjky.cn

[A03] 常量定义
来源：http://hb.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pz.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://kf.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://eq.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://db.colortex.cn

Java: static final double PI = 3.14159;
来源：http://fb.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://ry.nszjky.cn

Ruby: PI = 3.14159
来源：http://sm.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://wd.bookmarksfly.cn

[A04] 判断变量类型
来源：http://ao.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rt.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xi.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jw.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://vw.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tk.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://si.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cz.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://wm.jctech888.com.cn

[A05] 整数除法与取模
来源：http://sd.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://om.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vn.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yx.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cm.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://fa.521024.cn

Go:   7 / 2; 7 % 2
来源：http://rz.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://bq.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://qx.521024.cn

[A06] 字符串转数字
来源：http://bh.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://wh.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ja.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wn.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jm.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qf.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bu.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://te.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kl.9csxet.cn

[A07] 数字转字符串
来源：http://on.yuntaijiaju.cn

Py:   str(42)
来源：http://qh.521024.cn

PHP:  (string) 42; strval(42)
来源：http://eq.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://pg.gzmigu.cn

TS:   String(42)
来源：http://uf.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ab.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://kt.shxzskj.cn

Ruby: 42.to_s
来源：http://pb.9csxet.cn

C#:   42.ToString()
来源：http://jt.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://rr.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xn.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pp.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qz.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qx.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ly.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mw.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uw.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://of.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://yl.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xc.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dz.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pt.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uw.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rh.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oh.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xn.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gq.9csxet.cn

[A10] 生成随机数
来源：http://ah.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://js.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://qv.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cc.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zf.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://yt.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ct.hahajie.cn

Ruby: rand(1..100)
来源：http://ub.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://bs.nicolike.cn

[A11] 条件表达式（三元）
来源：http://xe.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://uv.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://om.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lh.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zc.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://ax.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zi.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mc.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://or.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://ct.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dp.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jt.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://az.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://hr.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://do.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ru.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://ue.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://rz.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cc.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://lo.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://ok.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://ny.521024.cn

TS:   "第一行\n第二行"
来源：http://hn.lnxyls.cn

Java: "第一行\n第二行"
来源：http://us.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://ao.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://up.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ra.jctech888.com.cn

[A14] 注释写法
来源：http://ry.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://we.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iv.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://iu.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://nd.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://he.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://to.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cq.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://hv.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://iu.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://or.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://vr.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://rw.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://oq.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sb.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://nh.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://bs.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://qa.wgjwhj.cn

[A16] 真假值判断规则
来源：http://ve.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wo.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rd.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ua.hahajie.cn

TS:   if (!x) {}
来源：http://gu.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jg.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uy.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tw.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yl.szsharing.cn

[A17] 位运算
来源：http://yo.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dr.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aa.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zh.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ai.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tv.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://og.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://jp.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://sy.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xw.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jl.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://ty.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ea.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://ja.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://hl.szxytkj.cn

[A19] 交换两个变量
来源：http://zz.panjiajie.cn

Py:   a, b = b, a
来源：http://hg.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cb.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://br.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://ca.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://pc.wgjwhj.cn

Go:   a, b = b, a
来源：http://qg.colortex.cn

Ruby: a, b = b, a
来源：http://cn.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://sq.jctech888.com.cn

[A20] 读取标准输入
来源：http://sx.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://bl.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ig.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ln.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://uv.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://iv.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iq.521024.cn

Ruby: gets.chomp
来源：http://tx.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://zy.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://os.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://zu.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ow.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://uh.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://fi.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://qi.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://id.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://kd.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://ek.wgjwhj.cn

[A22] 获取字符串长度
来源：http://kt.colortex.cn

Py:   len(s)
来源：http://pw.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kl.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yg.huanxung.cn

TS:   s.length
来源：http://bd.shtwfgs.cn

Java: s.length()
来源：http://wb.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ut.newstarts.cn

Ruby: s.length
来源：http://su.yuntaijiaju.cn

C#:   s.Length
来源：http://ej.9csxet.cn

[A23] 大小写转换
来源：http://wi.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ok.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vt.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bz.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ip.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ww.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hp.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vy.nszjky.cn

[A24] 去除首尾空白
来源：http://qm.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ld.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zb.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://io.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dt.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jr.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://ne.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tx.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jx.hnjuh.cn

[A25] 字符串比较
来源：http://el.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://ry.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mo.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tm.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://co.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gw.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mo.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tc.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bz.colortex.cn

[A26] 类型转换总览
来源：http://cg.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hu.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dr.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://by.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://cu.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qj.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sw.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://he.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vk.nicolike.cn

================================================================================
来源：http://uh.shxzskj.cn

B. 流程控制
来源：http://op.shtwfgs.cn

================================================================================
来源：http://zu.szsharing.cn

[B01] 条件判断 if / else
来源：http://ku.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nu.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://az.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zy.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zc.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mf.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jp.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yx.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xj.nszjky.cn

[B02] 多分支 else if / elif
来源：http://lf.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pi.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qp.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ym.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mq.9csxet.cn

[B03] switch / match / case
来源：http://cv.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pv.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://az.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vk.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fl.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rl.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nl.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wa.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uf.lnxyls.cn

[B04] for 计数循环
来源：http://lx.521024.cn

Py:   for i in range(10): print(i)
来源：http://rs.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ri.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tl.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xv.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tt.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pg.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://fq.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nz.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://sh.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://ot.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ql.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wm.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sy.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qe.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fv.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://us.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ud.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://sx.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mf.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pn.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jx.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hb.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wv.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bw.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://or.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mi.shxzskj.cn

[B07] while 循环
来源：http://kq.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://nk.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fx.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://nt.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://wy.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://vn.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ez.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://mj.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://wq.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://kl.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ih.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jq.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://uo.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://ir.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ai.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hf.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wp.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://bl.nszjky.cn

[B09] break 与 continue
来源：http://uj.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://af.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://he.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ta.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rl.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lu.muxihuayi.cn


<!-- 参考信息 -->