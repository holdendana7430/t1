代发 wailian999

================================================================================
来源：http://gg.shxzskj.cn

A. 基础语法与类型
来源：http://lh.nszjky.cn

================================================================================
来源：http://ob.lnxyls.cn

[A01] Hello World
来源：http://lr.nszjky.cn

Py:   print("Hello, World!")
来源：http://rn.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://eh.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://mn.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kv.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://el.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://oq.521024.cn

Ruby: puts "Hello, World!"
来源：http://im.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nt.colortex.cn

[A02] 变量声明与赋值
来源：http://cy.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bs.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yw.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dz.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ul.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://uk.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://yo.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://ko.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jg.szxytkj.cn

[A03] 常量定义
来源：http://ci.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ly.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://iz.huanxung.cn

JS:   const PI = 3.14159;
来源：http://sk.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://ns.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://gw.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://gx.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://ot.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://mh.szxytkj.cn

[A04] 判断变量类型
来源：http://be.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gs.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eb.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://af.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://wm.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xc.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mo.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jm.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://qx.hahajie.cn

[A05] 整数除法与取模
来源：http://rx.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lp.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gl.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qe.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gk.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://yd.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://oj.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://cc.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://xy.wgjwhj.cn

[A06] 字符串转数字
来源：http://fz.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://ge.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qi.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://to.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pv.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dl.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zq.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qn.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://em.shxzskj.cn

[A07] 数字转字符串
来源：http://pi.bookmarksfly.cn

Py:   str(42)
来源：http://ge.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://yy.nicolike.cn

JS:   String(42); (42).toString()
来源：http://xp.huixiangedu.cn

TS:   String(42)
来源：http://io.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vm.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://lp.shxzskj.cn

Ruby: 42.to_s
来源：http://in.haigaiapp.cn

C#:   42.ToString()
来源：http://vy.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://pu.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oe.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ur.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zn.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sm.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vn.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://id.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://og.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jh.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://bl.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zw.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xu.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nv.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tt.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xw.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yx.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oz.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ft.panjiajie.cn

[A10] 生成随机数
来源：http://mf.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://tl.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://de.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uy.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yw.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://fy.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bx.panjiajie.cn

Ruby: rand(1..100)
来源：http://sm.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://dv.521024.cn

[A11] 条件表达式（三元）
来源：http://si.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://to.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ha.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://us.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gk.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://rh.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://so.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gw.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lo.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://pi.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cl.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ku.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://xl.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://wk.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://fk.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bw.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://tg.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://af.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ra.asd995.cn

Py:   "第一行\n第二行"
来源：http://qc.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://rj.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://gp.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://ef.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://vx.newstarts.cn

Go:   "第一行\n第二行"
来源：http://vz.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://aw.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://hc.huixinmuqiang.cn

[A14] 注释写法
来源：http://gl.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zh.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bt.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://im.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://zq.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xj.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://hr.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ne.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://zt.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://tm.hahajie.cn

Py:   value = data or "默认值"
来源：http://ux.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://kq.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://aj.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://xm.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rs.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://kj.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://sy.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://pi.muxihuayi.cn

[A16] 真假值判断规则
来源：http://nu.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://he.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gx.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fe.wgjwhj.cn

TS:   if (!x) {}
来源：http://hf.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sq.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fy.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://iu.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gc.hahajie.cn

[A17] 位运算
来源：http://jc.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gq.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hd.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://in.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wz.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fw.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sb.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jv.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://mm.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://aw.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://ov.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ru.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qw.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://qh.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jh.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://qr.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://um.shxzskj.cn

[A19] 交换两个变量
来源：http://xw.newstarts.cn

Py:   a, b = b, a
来源：http://rt.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wx.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://bg.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://rp.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://vo.huixiangedu.cn

Go:   a, b = b, a
来源：http://wu.asd995.cn

Ruby: a, b = b, a
来源：http://qr.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://dr.hahajie.cn

[A20] 读取标准输入
来源：http://xe.hahajie.cn

Py:   name = input("请输入：")
来源：http://tk.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xy.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rz.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://uk.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ev.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iw.hahajie.cn

Ruby: gets.chomp
来源：http://dn.colortex.cn

C#:   Console.ReadLine();
来源：http://wg.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://so.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://sn.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zp.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://aq.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://vo.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://tw.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://do.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://jj.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ye.newstarts.cn

[A22] 获取字符串长度
来源：http://qz.521024.cn

Py:   len(s)
来源：http://ho.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mb.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pu.wgjwhj.cn

TS:   s.length
来源：http://rw.muxihuayi.cn

Java: s.length()
来源：http://gh.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nm.yuntaijiaju.cn

Ruby: s.length
来源：http://vd.jianghongdianzi.cn

C#:   s.Length
来源：http://ay.shtwfgs.cn

[A23] 大小写转换
来源：http://vp.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jl.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eu.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mx.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wu.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bj.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nm.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://us.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qd.gzmigu.cn

[A24] 去除首尾空白
来源：http://lk.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qg.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xi.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tl.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iy.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ry.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://hh.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lx.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://we.jctech888.com.cn

[A25] 字符串比较
来源：http://bg.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ln.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xu.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ip.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ml.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sv.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oa.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rf.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yc.asd995.cn

[A26] 类型转换总览
来源：http://um.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zd.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ch.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mh.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://rv.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fh.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qd.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://av.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://da.jianghongdianzi.cn

================================================================================
来源：http://gv.chemitech.net.cn

B. 流程控制
来源：http://gu.bjjhwx.cn

================================================================================
来源：http://de.hahajie.cn

[B01] 条件判断 if / else
来源：http://gk.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wi.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://er.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ay.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pn.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ha.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dx.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ca.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://vf.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oa.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nm.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xn.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qv.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tp.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.bjjhwx.cn

[B03] switch / match / case
来源：http://jg.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zl.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ap.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hw.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://an.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sw.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qc.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ls.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bp.haigaiapp.cn

[B04] for 计数循环
来源：http://px.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://kq.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://om.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://de.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://na.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://by.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lp.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://yr.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bg.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://cp.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://xx.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ue.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bd.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bd.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ur.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vc.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://hh.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qa.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://qw.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cg.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://di.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vd.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zn.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jx.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wr.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zx.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ab.asd995.cn

[B07] while 循环
来源：http://bt.521024.cn

Py:   while i < 10: i += 1
来源：http://kf.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ru.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://tv.521024.cn

TS:   while (i < 10) { i++; }
来源：http://hu.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://dd.yuntaijiaju.cn


<!-- 参考信息 -->