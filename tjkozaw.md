代发 wailian999

================================================================================
来源：http://ce.asd995.cn

A. 基础语法与类型
来源：http://ux.szsharing.cn

================================================================================
来源：http://yn.shxzskj.cn

[A01] Hello World
来源：http://fs.shxzskj.cn

Py:   print("Hello, World!")
来源：http://nw.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://mh.colortex.cn

JS:   console.log("Hello, World!");
来源：http://wo.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zg.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://ie.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://yf.colortex.cn

Ruby: puts "Hello, World!"
来源：http://xc.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jn.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://wr.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ki.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ty.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ak.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dz.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://sz.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://lc.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://if.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fr.gzmigu.cn

[A03] 常量定义
来源：http://ba.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uo.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://fl.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://dp.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ge.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://yn.szxytkj.cn

Go:   const PI = 3.14159
来源：http://lp.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://gv.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://nr.shxzskj.cn

[A04] 判断变量类型
来源：http://kp.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kp.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uj.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gb.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://gn.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uo.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aa.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ed.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://zc.nicolike.cn

[A05] 整数除法与取模
来源：http://oc.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hi.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xv.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tc.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bp.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://xj.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://zn.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://fl.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://pg.haigaiapp.cn

[A06] 字符串转数字
来源：http://fj.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://mg.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rg.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ev.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kd.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kd.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wu.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dk.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wa.haigaiapp.cn

[A07] 数字转字符串
来源：http://rk.9csxet.cn

Py:   str(42)
来源：http://gi.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://wq.szsharing.cn

JS:   String(42); (42).toString()
来源：http://hc.521024.cn

TS:   String(42)
来源：http://pi.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://st.asd995.cn

Go:   strconv.Itoa(42)
来源：http://vb.muxihuayi.cn

Ruby: 42.to_s
来源：http://tx.szxytkj.cn

C#:   42.ToString()
来源：http://re.lnxyls.cn

[A08] 取整与四舍五入
来源：http://ra.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eh.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wq.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yd.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vm.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ok.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mv.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oj.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://om.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://wp.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ql.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rm.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xp.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qj.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pq.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kx.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pb.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vq.hnjuh.cn

[A10] 生成随机数
来源：http://rh.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://rw.asd995.cn

PHP:  random_int(1, 100);
来源：http://hb.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zl.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xz.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://td.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pf.szsharing.cn

Ruby: rand(1..100)
来源：http://qj.521024.cn

C#:   new Random().Next(1, 101)
来源：http://zv.szsharing.cn

[A11] 条件表达式（三元）
来源：http://pw.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://eu.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hv.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lp.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jw.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://iq.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pl.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xt.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xo.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://ep.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bb.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xh.521024.cn

JS:   `Hello, ${name}!`
来源：http://we.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://vc.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ig.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ps.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://eq.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://fr.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gd.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://kf.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://bf.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://ek.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ab.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://yg.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://dc.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://in.asd995.cn

C#:   "第一行\n第二行"
来源：http://ci.hahajie.cn

[A14] 注释写法
来源：http://vc.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pf.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://if.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://hx.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://sv.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fy.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://lf.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zy.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ud.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://fz.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://tr.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://nm.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://ph.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://xt.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rg.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://bt.colortex.cn

Ruby: value = data || "默认值"
来源：http://sc.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://ks.nszjky.cn

[A16] 真假值判断规则
来源：http://om.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vm.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mw.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://di.jctech888.com.cn

TS:   if (!x) {}
来源：http://fj.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fx.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qz.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kk.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ok.newstarts.cn

[A17] 位运算
来源：http://gg.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xf.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jr.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tj.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cg.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kv.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fd.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://iq.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://jq.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://yo.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eg.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sk.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://kb.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mv.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://xd.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://at.szsharing.cn

[A19] 交换两个变量
来源：http://vn.lnxyls.cn

Py:   a, b = b, a
来源：http://kz.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gf.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://ec.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://vg.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://wk.521024.cn

Go:   a, b = b, a
来源：http://ku.lnxyls.cn

Ruby: a, b = b, a
来源：http://ol.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://qn.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://wd.szxytkj.cn

Py:   name = input("请输入：")
来源：http://rw.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://it.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bt.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://mu.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://mo.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eh.huanxung.cn

Ruby: gets.chomp
来源：http://bc.lnxyls.cn

C#:   Console.ReadLine();
来源：http://en.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://cv.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ij.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pt.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ry.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://dm.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://gv.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gq.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://go.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://rn.521024.cn

[A22] 获取字符串长度
来源：http://gj.hnjuh.cn

Py:   len(s)
来源：http://eg.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tf.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gu.wgjwhj.cn

TS:   s.length
来源：http://tw.chemitech.net.cn

Java: s.length()
来源：http://rt.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://me.huixinmuqiang.cn

Ruby: s.length
来源：http://ma.yuexingan06.cn

C#:   s.Length
来源：http://zq.nicolike.cn

[A23] 大小写转换
来源：http://mb.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://da.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://de.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gp.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tc.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wi.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hq.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qy.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yd.521024.cn

[A24] 去除首尾空白
来源：http://yk.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rh.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vp.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oj.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yg.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fe.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://zq.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sx.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nk.hnjuh.cn

[A25] 字符串比较
来源：http://hp.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://wh.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ax.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wy.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oc.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://at.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vu.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zi.shtwfgs.cn

[A26] 类型转换总览
来源：http://ws.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://no.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://py.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gl.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ja.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://es.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gy.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kb.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qa.chemitech.net.cn

================================================================================
来源：http://bt.nicolike.cn

B. 流程控制
来源：http://va.nszjky.cn

================================================================================
来源：http://zq.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://zt.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zz.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sc.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oz.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xb.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ey.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://un.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ne.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://za.nszjky.cn

[B02] 多分支 else if / elif
来源：http://yk.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qd.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://se.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fu.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ge.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wo.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://he.nszjky.cn

[B03] switch / match / case
来源：http://qz.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wp.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://up.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hx.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sd.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://il.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ep.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sr.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uw.bjjhwx.cn

[B04] for 计数循环
来源：http://uy.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://kn.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yg.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ip.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sr.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yj.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vl.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://mo.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sy.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://dh.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://le.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yl.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dl.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bw.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://si.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gb.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://rl.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xq.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://hg.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fd.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mp.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ly.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fw.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bq.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nm.nicolike.cn

[B07] while 循环
来源：http://kd.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://wq.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yc.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://vl.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://gv.colortex.cn

Java: while (i < 10) { i++; }
来源：http://hm.nicolike.cn


<!-- 参考信息 -->