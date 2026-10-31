代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kf.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://tb.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://jt.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://bw.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fb.521024.cn

[A03] 常量定义
来源：http://nf.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rx.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://ad.nszjky.cn

JS:   const PI = 3.14159;
来源：http://gd.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://dj.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://st.gzmigu.cn

Go:   const PI = 3.14159
来源：http://pt.colortex.cn

Ruby: PI = 3.14159
来源：http://nj.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://wy.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://gx.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nd.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iq.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wi.521024.cn

TS:   typeof x; x instanceof Date
来源：http://gn.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cu.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ov.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yz.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://mq.shtwfgs.cn

[A05] 整数除法与取模
来源：http://fw.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sr.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qz.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ig.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://on.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://gi.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://bf.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://qg.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://as.muxihuayi.cn

[A06] 字符串转数字
来源：http://oc.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://ti.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://te.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lz.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zb.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zd.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vj.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zy.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qd.521024.cn

[A07] 数字转字符串
来源：http://ba.shtwfgs.cn

Py:   str(42)
来源：http://xr.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://lw.newstarts.cn

JS:   String(42); (42).toString()
来源：http://ua.shtwfgs.cn

TS:   String(42)
来源：http://xw.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://id.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://yu.panjiajie.cn

Ruby: 42.to_s
来源：http://ga.hahajie.cn

C#:   42.ToString()
来源：http://jp.szxytkj.cn

[A08] 取整与四舍五入
来源：http://db.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://it.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zp.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qs.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://du.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hb.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jp.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uy.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ch.521024.cn

[A09] 绝对值与最大最小值
来源：http://oz.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hj.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kp.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://go.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jm.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zq.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bq.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nq.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mo.muxihuayi.cn

[A10] 生成随机数
来源：http://fo.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ca.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://wx.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://my.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xy.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://fw.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mz.panjiajie.cn

Ruby: rand(1..100)
来源：http://wr.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://wm.szsharing.cn

[A11] 条件表达式（三元）
来源：http://hc.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://fk.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://po.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ae.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mc.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://zw.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mc.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ny.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ez.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://hz.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jv.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mg.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://ss.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://lp.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ai.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cz.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://yi.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://jy.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pl.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://kf.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://nj.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://nz.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://pi.huanxung.cn

Java: "第一行\n第二行"
来源：http://hu.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://xj.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://mc.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://jl.nszjky.cn

[A14] 注释写法
来源：http://qt.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bz.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qw.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://mc.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ni.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iw.521024.cn

Go:   // 单行；/* 多行 */
来源：http://de.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ci.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://vn.hnjuh.cn

[A15] 空值判断与默认值
来源：http://ns.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://wb.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://rm.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://od.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://yp.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yy.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://eg.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://ar.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://hw.newstarts.cn

[A16] 真假值判断规则
来源：http://em.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lv.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uc.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tu.muxihuayi.cn

TS:   if (!x) {}
来源：http://dj.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qv.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mw.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xa.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fm.shxzskj.cn

[A17] 位运算
来源：http://bw.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mi.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fh.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vy.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zj.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://hi.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://aj.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://zu.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ov.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xz.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://nt.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ln.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://cp.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://bb.521024.cn

[A19] 交换两个变量
来源：http://nv.colortex.cn

Py:   a, b = b, a
来源：http://aq.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://re.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://mu.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://lv.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://yq.gzmigu.cn

Go:   a, b = b, a
来源：http://cd.hahajie.cn

Ruby: a, b = b, a
来源：http://us.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://vj.shxzskj.cn

[A20] 读取标准输入
来源：http://js.huanxung.cn

Py:   name = input("请输入：")
来源：http://pp.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kb.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mq.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://rp.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://xm.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xp.521024.cn

Ruby: gets.chomp
来源：http://sd.lnxyls.cn

C#:   Console.ReadLine();
来源：http://ax.huanxung.cn

[A21] 保留指定小数位输出
来源：http://zp.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://qu.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://si.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ic.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://pn.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://vx.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fd.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://wd.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://py.asd995.cn

[A22] 获取字符串长度
来源：http://nq.nszjky.cn

Py:   len(s)
来源：http://ca.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jc.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://im.panjiajie.cn

TS:   s.length
来源：http://lz.nszjky.cn

Java: s.length()
来源：http://ek.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bg.nicolike.cn

Ruby: s.length
来源：http://nh.bjjhwx.cn

C#:   s.Length
来源：http://rv.szxytkj.cn

[A23] 大小写转换
来源：http://ij.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mx.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rv.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zw.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wv.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ck.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gm.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vx.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://po.wgjwhj.cn

[A24] 去除首尾空白
来源：http://py.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vs.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sk.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gq.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mu.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wh.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ay.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rx.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vj.521024.cn

[A25] 字符串比较
来源：http://qc.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://ra.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xr.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lt.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gl.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://km.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jt.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ek.huanxung.cn

[A26] 类型转换总览
来源：http://mb.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qq.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://to.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hb.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://sh.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jb.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yk.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://op.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yq.nszjky.cn

================================================================================
来源：http://xb.yuexingan06.cn

B. 流程控制
来源：http://jh.9csxet.cn

================================================================================
来源：http://ew.lnxyls.cn

[B01] 条件判断 if / else
来源：http://or.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ts.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uw.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://me.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qx.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ww.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vb.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zw.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vd.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ks.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sm.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ky.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jx.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fn.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iw.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mx.huixinmuqiang.cn

[B03] switch / match / case
来源：http://sf.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://va.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gs.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eb.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jb.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wi.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mp.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ey.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jw.asd995.cn

[B04] for 计数循环
来源：http://lz.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://dg.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ca.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bc.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://au.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gc.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://gt.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xv.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://cm.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://kn.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kw.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://du.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vp.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wc.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xi.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://iu.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qt.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://uw.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qp.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dl.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zp.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hy.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uh.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zh.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tn.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://la.chemitech.net.cn

[B07] while 循环
来源：http://ab.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://se.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ue.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://oy.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://bf.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://kt.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://aw.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://cf.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://jl.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://xf.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wh.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ft.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://wp.521024.cn

Java: do { i++; } while (i < 10);
来源：http://fn.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mi.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ee.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://mx.muxihuayi.cn

[B09] break 与 continue
来源：http://tv.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://in.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bl.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mi.newstarts.cn


<!-- 参考信息 -->