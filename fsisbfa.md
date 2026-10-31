代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ey.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oe.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zx.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gc.huanxung.cn

================================================================================
来源：http://hk.shxzukj.cn

A. 基础语法与类型
来源：http://mt.shxzukj.cn

================================================================================
来源：http://gv.szxytkj.cn

[A01] Hello World
来源：http://aa.gzmigu.cn

Py:   print("Hello, World!")
来源：http://rd.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://hc.colortex.cn

JS:   console.log("Hello, World!");
来源：http://fq.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eq.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://fs.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://dn.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://dq.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aw.panjiajie.cn

[A02] 变量声明与赋值
来源：http://ib.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xc.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://na.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yc.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://js.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://ah.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://wz.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://yx.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vx.muxihuayi.cn

[A03] 常量定义
来源：http://ll.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://om.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://dw.hahajie.cn

JS:   const PI = 3.14159;
来源：http://dn.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://lt.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://ik.lnxyls.cn

Go:   const PI = 3.14159
来源：http://zh.9csxet.cn

Ruby: PI = 3.14159
来源：http://nq.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://sn.nszjky.cn

[A04] 判断变量类型
来源：http://ze.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zq.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ey.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uj.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://gl.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ur.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://en.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uk.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://vz.huixiangedu.cn

[A05] 整数除法与取模
来源：http://kz.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bh.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oj.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yq.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wx.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://co.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://ks.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://rh.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://wh.colortex.cn

[A06] 字符串转数字
来源：http://wf.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://im.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fm.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kg.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uh.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rt.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pn.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zn.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rs.nicolike.cn

[A07] 数字转字符串
来源：http://cb.szxytkj.cn

Py:   str(42)
来源：http://sp.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://wf.szsharing.cn

JS:   String(42); (42).toString()
来源：http://dj.szsharing.cn

TS:   String(42)
来源：http://jx.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vm.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://jz.lnxyls.cn

Ruby: 42.to_s
来源：http://ml.muxihuayi.cn

C#:   42.ToString()
来源：http://eg.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://tc.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tj.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rr.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ni.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ua.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://co.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sz.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zs.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hh.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://es.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eo.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ak.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bo.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zf.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oz.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://td.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xo.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pp.jianghongdianzi.cn

[A10] 生成随机数
来源：http://qm.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://jw.huanxung.cn

PHP:  random_int(1, 100);
来源：http://zs.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rf.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ck.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://tg.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bc.asd995.cn

Ruby: rand(1..100)
来源：http://hb.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://gz.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://hn.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://zv.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qs.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ir.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vo.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://hy.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ub.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qz.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gi.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://fv.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tf.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lq.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://nq.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://sj.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://mg.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xa.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://xf.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://yk.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yb.asd995.cn

Py:   "第一行\n第二行"
来源：http://hq.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://mt.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://px.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://mi.panjiajie.cn

Java: "第一行\n第二行"
来源：http://xe.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://jz.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://vu.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://pq.shxzskj.cn

[A14] 注释写法
来源：http://wr.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aw.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://do.521024.cn

JS:   // 单行；/* 多行 */
来源：http://oc.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://gs.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ca.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://hd.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xs.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://lu.huanxung.cn

[A15] 空值判断与默认值
来源：http://qv.shxzukj.cn

Py:   value = data or "默认值"
来源：http://dw.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://sf.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://tf.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://yd.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rj.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://pd.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://jr.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://la.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://tv.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oh.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://me.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qf.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://yk.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ve.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gi.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mi.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ij.szxytkj.cn

[A17] 位运算
来源：http://wf.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vt.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tv.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jl.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://er.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://je.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://fc.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://aw.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://mq.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jn.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yr.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://xh.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oq.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://yn.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://jc.hahajie.cn

[A19] 交换两个变量
来源：http://cy.nszjky.cn

Py:   a, b = b, a
来源：http://lq.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ts.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://io.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://kf.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://vd.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://dr.szxytkj.cn

Ruby: a, b = b, a
来源：http://bv.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://pl.521024.cn

[A20] 读取标准输入
来源：http://wp.gzmigu.cn

Py:   name = input("请输入：")
来源：http://pv.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gg.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://he.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ic.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://tn.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ug.nicolike.cn

Ruby: gets.chomp
来源：http://oj.shxzskj.cn

C#:   Console.ReadLine();
来源：http://ny.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://wv.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://zl.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ar.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://oa.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://iy.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://bb.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uy.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://mi.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://zo.huanxung.cn

[A22] 获取字符串长度
来源：http://bd.yuexingan06.cn

Py:   len(s)
来源：http://ti.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nb.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://km.9csxet.cn

TS:   s.length
来源：http://ds.bookmarksfly.cn

Java: s.length()
来源：http://tu.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qr.hahajie.cn

Ruby: s.length
来源：http://zm.huixiangedu.cn

C#:   s.Length
来源：http://yj.yuexingan06.cn

[A23] 大小写转换
来源：http://sf.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pa.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ow.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iw.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hw.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lz.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uv.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xg.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ym.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://xj.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xd.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pa.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://op.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ot.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cx.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://uv.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yr.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qm.shxzskj.cn

[A25] 字符串比较
来源：http://eu.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ro.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ya.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ws.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lg.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xg.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ej.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ss.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yp.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://iw.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ih.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yf.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gx.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://vb.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gv.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mk.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nr.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dk.jianghongdianzi.cn

================================================================================
来源：http://dq.hnjuh.cn

B. 流程控制
来源：http://oe.shxzukj.cn

================================================================================
来源：http://up.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ay.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oy.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ow.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gq.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jv.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bx.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://le.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://px.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vq.asd995.cn

[B02] 多分支 else if / elif
来源：http://xg.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qa.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sg.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pg.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ux.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mm.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.bjjhwx.cn

[B03] switch / match / case
来源：http://gn.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ib.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oa.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lz.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ur.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iv.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jr.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://am.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tq.szsharing.cn

[B04] for 计数循环
来源：http://kx.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hf.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://do.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jw.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://de.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sj.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://cm.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ks.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://ih.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://oy.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fi.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cy.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ek.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xo.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ny.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://ix.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://na.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://zq.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ob.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nm.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ba.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zv.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dl.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://td.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ie.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uk.lnxyls.cn

[B07] while 循环
来源：http://wo.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://gg.asd995.cn


<!-- 参考信息 -->