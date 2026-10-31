代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://cq.lnxyls.cn

[A03] 常量定义
来源：http://tw.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tl.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://ja.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://mh.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://na.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://lc.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://pn.nicolike.cn

Ruby: PI = 3.14159
来源：http://kl.asd995.cn

C#:   const double PI = 3.14159;
来源：http://nn.hahajie.cn

[A04] 判断变量类型
来源：http://qa.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xu.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zi.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ck.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://nv.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uf.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lp.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zn.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://ph.muxihuayi.cn

[A05] 整数除法与取模
来源：http://yx.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qa.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qp.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ou.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://if.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://ov.521024.cn

Go:   7 / 2; 7 % 2
来源：http://ok.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://th.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://ay.bjjhwx.cn

[A06] 字符串转数字
来源：http://aq.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://sw.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xw.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fc.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://by.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rs.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://js.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xg.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fn.nicolike.cn

[A07] 数字转字符串
来源：http://ps.gzmigu.cn

Py:   str(42)
来源：http://vv.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://yt.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://vk.panjiajie.cn

TS:   String(42)
来源：http://ov.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vd.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://af.shxzskj.cn

Ruby: 42.to_s
来源：http://cv.shtwfgs.cn

C#:   42.ToString()
来源：http://mg.newstarts.cn

[A08] 取整与四舍五入
来源：http://je.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://id.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ju.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ak.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xm.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ou.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gt.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mo.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tf.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://ei.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cx.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sw.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ya.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rw.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ys.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://az.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hi.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qv.szxytkj.cn

[A10] 生成随机数
来源：http://mx.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://hx.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://xo.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mp.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sc.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://jr.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bm.asd995.cn

Ruby: rand(1..100)
来源：http://pf.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://yx.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://ex.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://xi.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zg.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rx.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bd.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://hy.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yy.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://it.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sa.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://pe.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://np.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sh.asd995.cn

JS:   `Hello, ${name}!`
来源：http://pe.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://nv.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://yx.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rp.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://yo.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://ss.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yj.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://ix.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://cr.nicolike.cn

JS:   "第一行\n第二行"
来源：http://zp.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://se.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ly.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://yw.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://yu.nszjky.cn

C#:   "第一行\n第二行"
来源：http://el.shtwfgs.cn

[A14] 注释写法
来源：http://vx.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dc.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ik.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://zl.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://qx.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ko.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://hb.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://je.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://ag.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://pe.huanxung.cn

Py:   value = data or "默认值"
来源：http://cb.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://dc.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://yg.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://fk.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qt.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://se.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://gm.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://ib.yuexingan06.cn

[A16] 真假值判断规则
来源：http://sl.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vu.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oh.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ku.bjjhwx.cn

TS:   if (!x) {}
来源：http://ju.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aj.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yy.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ur.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uy.shtwfgs.cn

[A17] 位运算
来源：http://vy.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vn.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ml.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mb.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rk.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ek.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zg.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://xy.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://yg.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ov.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kv.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fb.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://fd.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ge.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ph.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://nh.nicolike.cn

[A19] 交换两个变量
来源：http://cs.nicolike.cn

Py:   a, b = b, a
来源：http://cf.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ra.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://sf.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://al.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://jq.newstarts.cn

Go:   a, b = b, a
来源：http://pl.panjiajie.cn

Ruby: a, b = b, a
来源：http://yv.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://nw.haigaiapp.cn

[A20] 读取标准输入
来源：http://ah.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://nv.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dv.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fj.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://md.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://vy.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ai.9csxet.cn

Ruby: gets.chomp
来源：http://hm.9csxet.cn

C#:   Console.ReadLine();
来源：http://wy.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://pq.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://cs.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zo.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://mz.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://vg.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://kn.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qm.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://sf.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://aq.yuexingan06.cn

[A22] 获取字符串长度
来源：http://vg.colortex.cn

Py:   len(s)
来源：http://bc.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qk.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ik.colortex.cn

TS:   s.length
来源：http://tg.panjiajie.cn

Java: s.length()
来源：http://vy.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pe.panjiajie.cn

Ruby: s.length
来源：http://cj.gzmigu.cn

C#:   s.Length
来源：http://up.muxihuayi.cn

[A23] 大小写转换
来源：http://aj.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fh.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xr.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gv.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gt.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ih.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gz.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jc.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nr.shxzukj.cn

[A24] 去除首尾空白
来源：http://qy.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bv.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ih.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ud.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zc.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://qk.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fo.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tw.asd995.cn

[A25] 字符串比较
来源：http://zq.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://za.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uj.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uz.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fp.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://il.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hn.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zq.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xp.huanxung.cn

[A26] 类型转换总览
来源：http://mz.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ho.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bc.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rd.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://gc.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eh.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hh.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fx.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nv.shtwfgs.cn

================================================================================
来源：http://ny.521024.cn

B. 流程控制
来源：http://uf.hnjuh.cn

================================================================================
来源：http://st.hahajie.cn

[B01] 条件判断 if / else
来源：http://dr.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jl.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ms.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yj.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rn.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gx.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dk.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://to.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ef.colortex.cn

[B02] 多分支 else if / elif
来源：http://at.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bu.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hp.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qb.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gd.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dq.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.hahajie.cn

[B03] switch / match / case
来源：http://fj.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://je.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vu.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sj.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cn.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ty.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sq.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://el.nszjky.cn

[B04] for 计数循环
来源：http://lb.521024.cn

Py:   for i in range(10): print(i)
来源：http://cs.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hi.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dp.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kz.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bn.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ix.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://zm.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ye.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://ku.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ys.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tw.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ii.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ow.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kz.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yt.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://ts.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kp.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://ww.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ty.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xg.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://et.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wb.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bm.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yh.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kd.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dc.nszjky.cn

[B07] while 循环
来源：http://qz.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://sn.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nv.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://rl.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://oh.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://rw.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://be.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://by.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://mt.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ho.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://fk.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://te.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://nd.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://lm.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://pu.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vi.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ml.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://mi.shxzukj.cn

[B09] break 与 continue
来源：http://wy.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kg.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xd.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jw.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gn.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sy.bjjhwx.cn


<!-- 参考信息 -->