代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://km.shtwfgs.cn

[A03] 常量定义
来源：http://hm.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ip.521024.cn

PHP:  const PI = 3.14159;
来源：http://dw.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://oe.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://mu.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://no.shxzukj.cn

Go:   const PI = 3.14159
来源：http://zx.nszjky.cn

Ruby: PI = 3.14159
来源：http://bs.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ho.yuexingan06.cn

[A04] 判断变量类型
来源：http://sw.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oz.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tp.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yd.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://sx.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sb.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aj.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cx.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://vf.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://wf.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tl.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gb.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ry.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zk.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://ju.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://xu.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://nz.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://hn.bookmarksfly.cn

[A06] 字符串转数字
来源：http://yy.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://js.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ox.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ps.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://eu.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://og.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bb.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ek.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://db.jctech888.com.cn

[A07] 数字转字符串
来源：http://ch.haigaiapp.cn

Py:   str(42)
来源：http://fh.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://fd.nszjky.cn

JS:   String(42); (42).toString()
来源：http://ix.yuexingan06.cn

TS:   String(42)
来源：http://si.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tr.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://hh.nszjky.cn

Ruby: 42.to_s
来源：http://vk.521024.cn

C#:   42.ToString()
来源：http://dz.9csxet.cn

[A08] 取整与四舍五入
来源：http://iv.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ww.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zh.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://th.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fz.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jp.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ee.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xu.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sa.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ko.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ch.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gq.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pb.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tp.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dg.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iq.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sd.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xk.muxihuayi.cn

[A10] 生成随机数
来源：http://da.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://ev.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://jr.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ji.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ss.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://tv.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dh.hnjuh.cn

Ruby: rand(1..100)
来源：http://av.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://vb.hahajie.cn

[A11] 条件表达式（三元）
来源：http://ge.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://gv.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jk.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nu.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qv.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://xz.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ak.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yi.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rt.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://si.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sk.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tk.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://dv.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://xj.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://zc.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pd.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://hb.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://lt.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ec.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://fe.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://qd.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://eh.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://yx.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://nl.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://pp.521024.cn

Ruby: "第一行\n第二行"
来源：http://is.colortex.cn

C#:   "第一行\n第二行"
来源：http://sv.chemitech.net.cn

[A14] 注释写法
来源：http://xd.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fg.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://of.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://nv.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://np.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cc.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://ac.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://er.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://tg.szxytkj.cn

[A15] 空值判断与默认值
来源：http://qf.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://ae.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://od.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://gj.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ut.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zb.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://ff.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://ct.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://xz.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://zu.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uf.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pt.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gh.yuexingan06.cn

TS:   if (!x) {}
来源：http://gd.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dz.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ov.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bk.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eo.521024.cn

[A17] 位运算
来源：http://nk.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ka.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wa.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bi.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bl.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ye.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xg.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://ap.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://hv.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ck.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rv.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wz.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://vy.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yv.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://sz.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://yu.yuexingan06.cn

[A19] 交换两个变量
来源：http://zz.hahajie.cn

Py:   a, b = b, a
来源：http://sh.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yb.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://gg.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://sc.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://gq.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://js.szsharing.cn

Ruby: a, b = b, a
来源：http://xy.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://yl.muxihuayi.cn

[A20] 读取标准输入
来源：http://vx.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://no.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gl.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ye.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://hn.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ox.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gg.huanxung.cn

Ruby: gets.chomp
来源：http://jd.nszjky.cn

C#:   Console.ReadLine();
来源：http://mx.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://wm.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://vw.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://le.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://dm.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ig.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://et.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sd.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://yf.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://sr.lnxyls.cn

[A22] 获取字符串长度
来源：http://oh.shxzskj.cn

Py:   len(s)
来源：http://yi.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nk.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ba.jianghongdianzi.cn

TS:   s.length
来源：http://fx.521024.cn

Java: s.length()
来源：http://we.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ir.huixinmuqiang.cn

Ruby: s.length
来源：http://vf.newstarts.cn

C#:   s.Length
来源：http://lx.panjiajie.cn

[A23] 大小写转换
来源：http://bv.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pz.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ue.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cw.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pd.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ui.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ma.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wo.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rn.asd995.cn

[A24] 去除首尾空白
来源：http://eh.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gw.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rn.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qu.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fw.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wn.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://eo.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pv.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pq.gzmigu.cn

[A25] 字符串比较
来源：http://mz.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://fu.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xo.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yg.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yc.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iy.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pq.huixiangedu.cn

[A26] 类型转换总览
来源：http://aj.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bh.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rn.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://py.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://zd.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hq.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kg.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iu.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fl.bjjhwx.cn

================================================================================
来源：http://db.yuntaijiaju.cn

B. 流程控制
来源：http://lb.nicolike.cn

================================================================================
来源：http://tj.newstarts.cn

[B01] 条件判断 if / else
来源：http://cr.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gv.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rc.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xk.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://us.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cg.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ey.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ul.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://me.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://qj.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://up.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dv.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lm.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://di.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wz.muxihuayi.cn

[B03] switch / match / case
来源：http://vb.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yc.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kz.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ix.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ck.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://om.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ne.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mt.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ac.jctech888.com.cn

[B04] for 计数循环
来源：http://ow.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://yc.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sg.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://db.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://li.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pe.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vp.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://xn.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bz.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ds.szsharing.cn

Py:   for item in arr: print(item)
来源：http://vm.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mq.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ss.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qg.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://du.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vn.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://rj.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rm.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ms.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lq.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://af.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mw.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kv.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tb.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lb.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ka.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kn.szxytkj.cn

[B07] while 循环
来源：http://gq.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://mf.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xx.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://iw.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://zr.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://lc.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ir.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://cs.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://hi.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://dr.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://md.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ui.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://bh.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://oo.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://xg.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://io.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ln.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ms.bjjhwx.cn

[B09] break 与 continue
来源：http://sv.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cj.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sa.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rb.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fs.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hf.shxzukj.cn


<!-- 参考信息 -->