代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ym.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sy.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uq.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ow.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ls.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tp.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hj.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mf.huixiangedu.cn

================================================================================
来源：http://tg.nicolike.cn

A. 基础语法与类型
来源：http://he.panjiajie.cn

================================================================================
来源：http://sf.nicolike.cn

[A01] Hello World
来源：http://tk.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://hg.521024.cn

PHP:  echo "Hello, World!";
来源：http://mo.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://is.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vw.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://pc.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://sc.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://ad.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wy.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://bi.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tx.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fr.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ud.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dm.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://qp.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://rs.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://kv.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yd.hahajie.cn

[A03] 常量定义
来源：http://mz.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ty.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://jo.hahajie.cn

JS:   const PI = 3.14159;
来源：http://md.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://vb.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://ri.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ry.shxzukj.cn

Ruby: PI = 3.14159
来源：http://ur.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://ch.wgjwhj.cn

[A04] 判断变量类型
来源：http://rz.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zt.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lf.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dk.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://nq.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kf.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gf.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qt.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://ej.bjjhwx.cn

[A05] 整数除法与取模
来源：http://ne.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rz.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ic.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lm.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ns.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://fw.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://wa.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://jh.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://oj.yuexingan06.cn

[A06] 字符串转数字
来源：http://lz.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://jw.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ed.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uo.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nf.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aa.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xl.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ew.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ys.bookmarksfly.cn

[A07] 数字转字符串
来源：http://cx.jianghongdianzi.cn

Py:   str(42)
来源：http://ys.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://ff.colortex.cn

JS:   String(42); (42).toString()
来源：http://eu.shtwfgs.cn

TS:   String(42)
来源：http://hd.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fq.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://px.szsharing.cn

Ruby: 42.to_s
来源：http://vx.bookmarksfly.cn

C#:   42.ToString()
来源：http://ez.shxzukj.cn

[A08] 取整与四舍五入
来源：http://eq.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://px.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lj.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dp.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qn.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://az.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cb.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dr.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ir.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://oj.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ls.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xy.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yq.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://an.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wy.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xk.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ii.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://em.bjjhwx.cn

[A10] 生成随机数
来源：http://ea.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://uj.szsharing.cn

PHP:  random_int(1, 100);
来源：http://by.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xc.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xo.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://ju.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://og.hahajie.cn

Ruby: rand(1..100)
来源：http://qj.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://vr.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://po.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://bm.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://re.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gv.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zj.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://nz.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hq.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://en.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fi.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://ep.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://js.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://by.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://lr.521024.cn

TS:   `Hello, ${name}!`
来源：http://oq.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://ki.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lw.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://yb.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://zo.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hq.nicolike.cn

Py:   "第一行\n第二行"
来源：http://kf.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://ua.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://xm.colortex.cn

TS:   "第一行\n第二行"
来源：http://pe.shxzukj.cn

Java: "第一行\n第二行"
来源：http://qg.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://em.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ba.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ez.hnjuh.cn

[A14] 注释写法
来源：http://ib.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tu.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dn.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://mn.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://sb.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mv.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://hu.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wj.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://rr.521024.cn

[A15] 空值判断与默认值
来源：http://sj.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://im.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://qf.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://qe.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://uh.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ar.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://hf.asd995.cn

Ruby: value = data || "默认值"
来源：http://zp.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://gm.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://nk.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vd.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fj.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gw.lnxyls.cn

TS:   if (!x) {}
来源：http://gs.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wm.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nd.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tf.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://id.shxzukj.cn

[A17] 位运算
来源：http://do.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pf.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kd.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ui.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ud.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zs.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fh.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://cp.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://gb.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://kn.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jy.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dg.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://xy.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hx.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://yw.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://kt.bookmarksfly.cn

[A19] 交换两个变量
来源：http://sn.hnjuh.cn

Py:   a, b = b, a
来源：http://xj.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uk.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://oz.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://bu.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://wp.shtwfgs.cn

Go:   a, b = b, a
来源：http://lz.521024.cn

Ruby: a, b = b, a
来源：http://nl.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://mk.jctech888.com.cn

[A20] 读取标准输入
来源：http://cm.panjiajie.cn

Py:   name = input("请输入：")
来源：http://ol.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eg.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pm.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://up.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://wp.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yw.521024.cn

Ruby: gets.chomp
来源：http://bi.newstarts.cn

C#:   Console.ReadLine();
来源：http://yz.nszjky.cn

[A21] 保留指定小数位输出
来源：http://ri.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://dv.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://co.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://qn.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ut.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://nb.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://un.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://xc.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://ya.haigaiapp.cn

[A22] 获取字符串长度
来源：http://qa.yuntaijiaju.cn

Py:   len(s)
来源：http://uv.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dw.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zv.muxihuayi.cn

TS:   s.length
来源：http://sg.521024.cn

Java: s.length()
来源：http://ue.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://id.hahajie.cn

Ruby: s.length
来源：http://ke.huixiangedu.cn

C#:   s.Length
来源：http://uk.wgjwhj.cn

[A23] 大小写转换
来源：http://sx.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xu.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://in.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sk.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jv.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://br.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tm.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ji.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wj.yuexingan06.cn

[A24] 去除首尾空白
来源：http://mj.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kw.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ed.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rj.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vr.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://by.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://rs.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kt.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dn.jctech888.com.cn

[A25] 字符串比较
来源：http://oa.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://xw.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ij.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cx.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ap.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yz.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jk.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zc.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uh.hahajie.cn

[A26] 类型转换总览
来源：http://pk.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rw.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qd.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://us.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://mj.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pm.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zo.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://of.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ua.colortex.cn

================================================================================
来源：http://rb.haigaiapp.cn

B. 流程控制
来源：http://qx.chemitech.net.cn

================================================================================
来源：http://rn.hahajie.cn

[B01] 条件判断 if / else
来源：http://xn.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rk.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rk.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kd.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vq.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zh.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://po.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hg.colortex.cn

[B02] 多分支 else if / elif
来源：http://pl.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cf.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xp.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sv.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://py.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fn.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mk.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://to.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.chemitech.net.cn

[B03] switch / match / case
来源：http://sp.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sx.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://go.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pq.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ep.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ka.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cs.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yr.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ir.panjiajie.cn

[B04] for 计数循环
来源：http://fs.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://wt.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ra.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bd.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bd.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yi.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://se.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://te.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rl.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://vw.asd995.cn

Py:   for item in arr: print(item)
来源：http://yz.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pg.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://np.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ef.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://el.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ob.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ya.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qe.colortex.cn

[B06] 遍历字典 / 对象
来源：http://bz.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wg.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bb.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wa.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nt.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://is.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xv.nszjky.cn


<!-- 参考信息 -->