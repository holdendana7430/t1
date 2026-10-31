代发 wailian999

Py:   print("Hello, World!")
来源：http://bb.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://zl.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://nw.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gf.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://vp.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://nm.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://ej.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cy.9csxet.cn

[A02] 变量声明与赋值
来源：http://js.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uj.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uq.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dq.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cp.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://bm.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://mz.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://ug.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gj.lnxyls.cn

[A03] 常量定义
来源：http://qo.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ze.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://yb.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://th.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://of.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://lz.shxzukj.cn

Go:   const PI = 3.14159
来源：http://up.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://zz.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://rk.wgjwhj.cn

[A04] 判断变量类型
来源：http://lt.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://se.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gy.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cp.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://ye.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tk.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bl.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gj.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://gy.asd995.cn

[A05] 整数除法与取模
来源：http://ex.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kc.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xc.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kp.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yt.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://to.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://jz.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://zz.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://id.lnxyls.cn

[A06] 字符串转数字
来源：http://ge.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://mr.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ta.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iu.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pi.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fd.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hw.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oz.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jv.bookmarksfly.cn

[A07] 数字转字符串
来源：http://gn.colortex.cn

Py:   str(42)
来源：http://bk.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://ck.nicolike.cn

JS:   String(42); (42).toString()
来源：http://kq.nszjky.cn

TS:   String(42)
来源：http://hh.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cj.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://wm.haigaiapp.cn

Ruby: 42.to_s
来源：http://is.hnjuh.cn

C#:   42.ToString()
来源：http://jl.shxzukj.cn

[A08] 取整与四舍五入
来源：http://sc.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ic.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cf.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ru.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ko.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nw.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sx.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wi.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eo.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://rh.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rl.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gm.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kx.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wj.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yu.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qv.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cc.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uv.asd995.cn

[A10] 生成随机数
来源：http://qy.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://vm.newstarts.cn

PHP:  random_int(1, 100);
来源：http://kq.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ig.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bs.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://wk.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uf.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://ba.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://pa.huanxung.cn

[A11] 条件表达式（三元）
来源：http://pb.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://nn.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ig.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pz.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://td.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://vd.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pg.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nw.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fu.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://sz.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nj.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mi.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://zs.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://mf.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yz.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dg.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://ux.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://su.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eb.9csxet.cn

Py:   "第一行\n第二行"
来源：http://rm.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://py.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://ru.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://pp.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ff.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://xf.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://ng.nszjky.cn

C#:   "第一行\n第二行"
来源：http://le.yuntaijiaju.cn

[A14] 注释写法
来源：http://dk.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sf.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ct.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://eo.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://if.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kd.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://tl.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ca.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://vd.shxzskj.cn

[A15] 空值判断与默认值
来源：http://lk.9csxet.cn

Py:   value = data or "默认值"
来源：http://fv.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://di.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://cp.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://iq.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qh.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://cv.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ka.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://sz.huanxung.cn

[A16] 真假值判断规则
来源：http://fe.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jq.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zn.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bx.shtwfgs.cn

TS:   if (!x) {}
来源：http://xq.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fn.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vj.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zl.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://me.szxytkj.cn

[A17] 位运算
来源：http://kq.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sg.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wm.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cm.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ny.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://js.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mi.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://ro.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://qe.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://sk.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yd.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zj.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://mj.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zd.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://qy.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://ov.shtwfgs.cn

[A19] 交换两个变量
来源：http://ck.chemitech.net.cn

Py:   a, b = b, a
来源：http://lx.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ll.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://bx.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://cq.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ch.panjiajie.cn

Go:   a, b = b, a
来源：http://ur.hnjuh.cn

Ruby: a, b = b, a
来源：http://up.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://ix.muxihuayi.cn

[A20] 读取标准输入
来源：http://pk.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://tr.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fv.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://tr.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://pf.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iu.wgjwhj.cn

Ruby: gets.chomp
来源：http://tf.nicolike.cn

C#:   Console.ReadLine();
来源：http://up.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://bc.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://dw.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://em.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://pj.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://xm.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://af.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rn.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://ib.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://et.szxytkj.cn

[A22] 获取字符串长度
来源：http://oj.yuntaijiaju.cn

Py:   len(s)
来源：http://ag.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wg.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lc.huixiangedu.cn

TS:   s.length
来源：http://hb.nszjky.cn

Java: s.length()
来源：http://hk.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xu.wgjwhj.cn

Ruby: s.length
来源：http://fx.jianghongdianzi.cn

C#:   s.Length
来源：http://yv.9csxet.cn

[A23] 大小写转换
来源：http://ec.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yz.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://br.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ce.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bb.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hy.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lp.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://us.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gx.asd995.cn

[A24] 去除首尾空白
来源：http://ob.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sl.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jr.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://be.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ol.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jy.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://gg.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://km.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mb.nicolike.cn

[A25] 字符串比较
来源：http://kw.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://md.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tw.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wo.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gy.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lm.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qi.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rt.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://na.shxzukj.cn

[A26] 类型转换总览
来源：http://rj.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ln.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wu.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lr.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://ct.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lp.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://se.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ug.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fu.shxzskj.cn

================================================================================
来源：http://yu.haigaiapp.cn

B. 流程控制
来源：http://tn.muxihuayi.cn

================================================================================
来源：http://vx.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://cp.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zt.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rj.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lr.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oo.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://by.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ii.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lp.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zg.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://qy.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wk.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dh.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oq.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tb.shtwfgs.cn

[B03] switch / match / case
来源：http://fz.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pg.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qf.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dr.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nk.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jz.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kl.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://as.yuexingan06.cn

[B04] for 计数循环
来源：http://fg.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://xt.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oz.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pn.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://du.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gy.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ht.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cx.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://kp.521024.cn

Py:   for item in arr: print(item)
来源：http://ev.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vy.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yv.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zy.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://po.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zd.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://hp.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dv.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://ch.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tu.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yg.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tq.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ag.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jm.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qh.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vt.9csxet.cn

[B07] while 循环
来源：http://vm.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://nh.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ls.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://kb.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://cu.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://xm.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uu.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://kh.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://ux.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://hi.nszjky.cn


<!-- 参考信息 -->