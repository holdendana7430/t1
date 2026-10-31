代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://gl.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://de.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://ky.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qw.asd995.cn

[A02] 变量声明与赋值
来源：http://ro.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uy.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://on.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fq.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kb.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://ox.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://gf.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://jo.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jl.nszjky.cn

[A03] 常量定义
来源：http://kd.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ke.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://nj.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://xh.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://yv.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ua.shxzskj.cn

Go:   const PI = 3.14159
来源：http://gn.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://ei.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://ff.chemitech.net.cn

[A04] 判断变量类型
来源：http://fj.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yi.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gj.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qx.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://pa.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kg.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jf.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://di.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://kt.nszjky.cn

[A05] 整数除法与取模
来源：http://he.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cy.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vv.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pg.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fa.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://ka.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://ol.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dp.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://ne.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://ci.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://bz.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ch.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bf.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ts.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://si.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://he.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sx.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ga.bookmarksfly.cn

[A07] 数字转字符串
来源：http://kk.yuntaijiaju.cn

Py:   str(42)
来源：http://iz.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://hd.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://sn.hahajie.cn

TS:   String(42)
来源：http://yx.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pu.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://wl.asd995.cn

Ruby: 42.to_s
来源：http://fy.szsharing.cn

C#:   42.ToString()
来源：http://hj.szxytkj.cn

[A08] 取整与四舍五入
来源：http://nc.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gz.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pb.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gs.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://io.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dl.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vp.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qe.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bb.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://xu.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tn.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zj.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uk.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hs.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ko.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qc.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://st.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bi.muxihuayi.cn

[A10] 生成随机数
来源：http://wm.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://ih.521024.cn

PHP:  random_int(1, 100);
来源：http://jr.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vc.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://py.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://cj.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sp.szsharing.cn

Ruby: rand(1..100)
来源：http://ri.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://fr.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://zf.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://pg.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://us.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aa.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://id.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://oo.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rv.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gy.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ru.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://hl.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pq.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bu.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://gg.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://cj.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://qe.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tg.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://fh.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://uf.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gf.9csxet.cn

Py:   "第一行\n第二行"
来源：http://eu.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ay.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://aw.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://nz.nszjky.cn

Java: "第一行\n第二行"
来源：http://yy.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://lc.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://nx.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://wu.haigaiapp.cn

[A14] 注释写法
来源：http://rn.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ma.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qf.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://pb.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://tu.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pi.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://mw.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rh.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://cg.shxzskj.cn

[A15] 空值判断与默认值
来源：http://ib.lnxyls.cn

Py:   value = data or "默认值"
来源：http://ax.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://sd.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://hr.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://dq.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oy.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://eq.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://ka.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://ed.shxzskj.cn

[A16] 真假值判断规则
来源：http://ud.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qo.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hg.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ha.bjjhwx.cn

TS:   if (!x) {}
来源：http://oe.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ve.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dq.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xt.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xy.521024.cn

[A17] 位运算
来源：http://lq.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pg.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jv.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xu.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vx.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vi.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://db.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://me.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://av.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://kc.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qw.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rs.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://xk.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dw.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://mh.asd995.cn

C#:   (int)'A'; (char)65
来源：http://es.colortex.cn

[A19] 交换两个变量
来源：http://on.bookmarksfly.cn

Py:   a, b = b, a
来源：http://kw.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fh.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://pm.colortex.cn

TS:   [a, b] = [b, a];
来源：http://fs.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://ih.asd995.cn

Go:   a, b = b, a
来源：http://yc.521024.cn

Ruby: a, b = b, a
来源：http://dd.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://tm.muxihuayi.cn

[A20] 读取标准输入
来源：http://pi.nszjky.cn

Py:   name = input("请输入：")
来源：http://sb.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qh.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wy.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://jz.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://xg.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bg.bjjhwx.cn

Ruby: gets.chomp
来源：http://ih.lnxyls.cn

C#:   Console.ReadLine();
来源：http://tt.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://nm.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ri.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ug.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://gf.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://sy.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://lw.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rh.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://gl.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://vx.521024.cn

[A22] 获取字符串长度
来源：http://ib.shxzskj.cn

Py:   len(s)
来源：http://df.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ax.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wg.newstarts.cn

TS:   s.length
来源：http://lq.panjiajie.cn

Java: s.length()
来源：http://xh.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://db.haigaiapp.cn

Ruby: s.length
来源：http://tx.huanxung.cn

C#:   s.Length
来源：http://gg.asd995.cn

[A23] 大小写转换
来源：http://nk.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://im.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lk.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gl.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pn.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://go.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nv.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hw.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yu.muxihuayi.cn

[A24] 去除首尾空白
来源：http://pl.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ak.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ok.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dy.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vu.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qy.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://yg.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://as.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://il.shxzukj.cn

[A25] 字符串比较
来源：http://bx.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://yb.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ym.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ml.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oy.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ds.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oe.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tm.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aj.szsharing.cn

[A26] 类型转换总览
来源：http://sz.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ur.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hv.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://do.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ql.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vk.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lj.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ux.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cs.shxzskj.cn

================================================================================
来源：http://jx.nicolike.cn

B. 流程控制
来源：http://bx.szsharing.cn

================================================================================
来源：http://wm.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://dp.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ri.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fr.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vt.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wz.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qx.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ht.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ma.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://to.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://gn.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yx.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ay.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zs.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bp.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xx.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oc.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.chemitech.net.cn

[B03] switch / match / case
来源：http://bs.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cs.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mv.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ug.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jv.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ow.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xx.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mr.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cu.9csxet.cn

[B04] for 计数循环
来源：http://dj.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://dd.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ai.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rk.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ii.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://il.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dz.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://fh.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://bx.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://lm.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ay.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yr.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://po.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tb.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tt.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ux.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uu.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://zb.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ew.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tt.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ix.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ll.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yv.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ul.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kg.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yw.huanxung.cn

[B07] while 循环
来源：http://mc.hahajie.cn

Py:   while i < 10: i += 1
来源：http://ch.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xv.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://kz.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://tq.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://pt.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vc.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://vx.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://yh.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://rr.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://iq.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dd.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://pe.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://oy.jctech888.com.cn


<!-- 参考信息 -->