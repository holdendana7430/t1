代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pn.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://zf.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://go.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://oa.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dm.bjjhwx.cn

[A03] 常量定义
来源：http://ig.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cx.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://lv.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://uu.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://jh.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://qy.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://vk.szsharing.cn

Ruby: PI = 3.14159
来源：http://zj.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://la.521024.cn

[A04] 判断变量类型
来源：http://zo.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aj.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://un.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sa.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://qk.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sa.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://za.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rr.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://an.huanxung.cn

[A05] 整数除法与取模
来源：http://ij.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ij.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://co.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ao.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hf.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://lk.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://ge.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://na.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://kf.shxzskj.cn

[A06] 字符串转数字
来源：http://vc.521024.cn

Py:   int("42"); float("3.14")
来源：http://ij.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ru.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wr.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ek.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qy.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fd.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ch.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tg.gzmigu.cn

[A07] 数字转字符串
来源：http://oe.bookmarksfly.cn

Py:   str(42)
来源：http://lw.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://la.colortex.cn

JS:   String(42); (42).toString()
来源：http://xz.gzmigu.cn

TS:   String(42)
来源：http://zc.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hk.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://uo.shtwfgs.cn

Ruby: 42.to_s
来源：http://md.colortex.cn

C#:   42.ToString()
来源：http://oq.gzmigu.cn

[A08] 取整与四舍五入
来源：http://sc.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dr.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ou.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lu.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mi.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ss.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xc.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ra.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yh.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://ny.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bx.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cz.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vz.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xn.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hd.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ga.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hj.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ci.panjiajie.cn

[A10] 生成随机数
来源：http://zj.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://bn.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://cn.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jp.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wi.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://xf.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aq.gzmigu.cn

Ruby: rand(1..100)
来源：http://wz.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://nu.521024.cn

[A11] 条件表达式（三元）
来源：http://gj.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://cs.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rc.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ly.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iu.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://mw.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wt.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pu.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tu.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://yg.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wk.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eu.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://ql.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://lg.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://kf.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tj.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://os.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://kq.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nn.szsharing.cn

Py:   "第一行\n第二行"
来源：http://ux.colortex.cn

PHP:  "第一行\n第二行"
来源：http://hb.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://dr.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ld.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://xk.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://lj.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://jz.asd995.cn

C#:   "第一行\n第二行"
来源：http://md.szxytkj.cn

[A14] 注释写法
来源：http://xn.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qa.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mf.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://di.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://la.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bf.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://qp.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hw.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://uw.newstarts.cn

[A15] 空值判断与默认值
来源：http://im.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://bk.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://lo.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://hs.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://ck.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://nt.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://mt.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ue.jctech888.com.cn

[A16] 真假值判断规则
来源：http://qr.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sr.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eh.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rb.panjiajie.cn

TS:   if (!x) {}
来源：http://ig.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kk.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wa.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ep.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aa.shtwfgs.cn

[A17] 位运算
来源：http://rt.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gf.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bi.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bz.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zl.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gc.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lp.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sx.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ne.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://vr.colortex.cn

Py:   ord("A"); chr(65)
来源：http://eu.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://lq.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gk.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mr.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ib.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pb.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://um.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://ai.asd995.cn

[A19] 交换两个变量
来源：http://rq.hnjuh.cn

Py:   a, b = b, a
来源：http://qk.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yc.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://dg.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ca.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://qt.yuexingan06.cn

Go:   a, b = b, a
来源：http://hv.szxytkj.cn

Ruby: a, b = b, a
来源：http://fh.521024.cn

C#:   (a, b) = (b, a);
来源：http://he.asd995.cn

[A20] 读取标准输入
来源：http://yt.szxytkj.cn

Py:   name = input("请输入：")
来源：http://to.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ar.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sw.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://ln.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://dn.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kv.huixiangedu.cn

Ruby: gets.chomp
来源：http://fr.newstarts.cn

C#:   Console.ReadLine();
来源：http://xz.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://vv.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://ra.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lp.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ph.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://iy.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://it.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hk.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://lx.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://si.shxzskj.cn

[A22] 获取字符串长度
来源：http://dn.huixinmuqiang.cn

Py:   len(s)
来源：http://eo.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ey.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oh.bookmarksfly.cn

TS:   s.length
来源：http://xw.shxzukj.cn

Java: s.length()
来源：http://bu.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wc.nszjky.cn

Ruby: s.length
来源：http://so.yuntaijiaju.cn

C#:   s.Length
来源：http://ms.huixiangedu.cn

[A23] 大小写转换
来源：http://jt.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vh.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fa.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ne.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yw.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wy.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ce.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mk.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rc.jctech888.com.cn

[A24] 去除首尾空白
来源：http://jh.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jy.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ti.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://un.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://it.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mu.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://cz.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://df.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fn.huanxung.cn

[A25] 字符串比较
来源：http://rl.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://kv.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zt.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qs.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kj.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mm.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lk.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bj.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kn.panjiajie.cn

[A26] 类型转换总览
来源：http://me.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ku.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cw.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kp.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://aj.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dn.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mo.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yp.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zi.nszjky.cn

================================================================================
来源：http://xa.gzmigu.cn

B. 流程控制
来源：http://bf.muxihuayi.cn

================================================================================
来源：http://gc.nicolike.cn

[B01] 条件判断 if / else
来源：http://xh.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xu.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xk.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nn.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qa.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qh.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ig.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jw.szsharing.cn

[B02] 多分支 else if / elif
来源：http://tq.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dd.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ex.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zq.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ls.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wa.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://it.szsharing.cn

[B03] switch / match / case
来源：http://ng.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ir.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://og.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uj.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jb.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vb.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vu.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eb.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gk.shxzukj.cn

[B04] for 计数循环
来源：http://js.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://lf.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dd.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sk.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wj.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yq.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fj.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://qr.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cu.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://az.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://bk.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tg.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://by.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jh.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vw.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://st.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://uv.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ti.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://gz.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://in.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://py.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hs.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oh.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ng.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nd.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oa.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://em.jctech888.com.cn

[B07] while 循环
来源：http://ig.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://fe.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nf.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://zq.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://gz.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://by.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://as.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://wd.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://bu.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://va.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://wg.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nu.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://bd.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://ob.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://un.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ib.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wx.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://op.shxzskj.cn

[B09] break 与 continue
来源：http://rn.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rx.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ii.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.huixinmuqiang.cn


<!-- 参考信息 -->