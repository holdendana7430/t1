代发 wailian999

Py:   print("Hello, World!")
来源：http://sf.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://al.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://wm.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fm.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://qe.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://hi.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://ig.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ba.huanxung.cn

[A02] 变量声明与赋值
来源：http://nu.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vf.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xf.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nl.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vy.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://id.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://wr.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://mw.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sq.lnxyls.cn

[A03] 常量定义
来源：http://fp.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ec.colortex.cn

PHP:  const PI = 3.14159;
来源：http://lf.asd995.cn

JS:   const PI = 3.14159;
来源：http://sg.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://zb.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://jq.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://dd.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://ha.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://ak.asd995.cn

[A04] 判断变量类型
来源：http://go.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qm.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oi.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://io.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://zz.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kf.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://et.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://as.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://fy.gzmigu.cn

[A05] 整数除法与取模
来源：http://ix.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://im.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jh.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qs.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ev.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://di.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://gd.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://ey.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://xc.yuexingan06.cn

[A06] 字符串转数字
来源：http://xh.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://mn.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qv.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bs.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wh.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pf.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ne.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://th.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yf.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://pn.huixiangedu.cn

Py:   str(42)
来源：http://du.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://ez.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://gx.yuntaijiaju.cn

TS:   String(42)
来源：http://cw.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dx.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://uc.hnjuh.cn

Ruby: 42.to_s
来源：http://pw.shtwfgs.cn

C#:   42.ToString()
来源：http://vf.shxzukj.cn

[A08] 取整与四舍五入
来源：http://pk.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qg.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lf.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tx.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xy.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fk.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ry.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ag.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ih.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://az.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rn.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qu.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://og.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eq.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pc.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vs.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ge.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://if.szsharing.cn

[A10] 生成随机数
来源：http://ni.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://wi.colortex.cn

PHP:  random_int(1, 100);
来源：http://hv.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://it.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gm.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://to.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sk.shxzukj.cn

Ruby: rand(1..100)
来源：http://mp.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://ir.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://ol.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://rz.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cr.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sl.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xu.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://qr.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yi.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ox.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jw.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://kn.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ex.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ej.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://vr.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://fc.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ov.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://in.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://mu.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://rw.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://om.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://xf.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://so.szsharing.cn

JS:   "第一行\n第二行"
来源：http://mt.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://vv.huanxung.cn

Java: "第一行\n第二行"
来源：http://ce.szsharing.cn

Go:   "第一行\n第二行"
来源：http://wu.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://mk.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://xg.9csxet.cn

[A14] 注释写法
来源：http://kn.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ot.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ky.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://ww.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://sp.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xn.521024.cn

Go:   // 单行；/* 多行 */
来源：http://hl.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://om.521024.cn

C#:   // 单行；/* 多行 */
来源：http://ac.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://bk.szxytkj.cn

Py:   value = data or "默认值"
来源：http://vz.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://gz.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://bb.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://vw.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gr.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://aj.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://gl.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ps.jctech888.com.cn

[A16] 真假值判断规则
来源：http://dw.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://em.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nb.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wr.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://ha.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xx.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lk.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qp.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kb.yuexingan06.cn

[A17] 位运算
来源：http://rj.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bc.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iy.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gv.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qj.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jd.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pv.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://xa.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://si.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://wv.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ob.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lm.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://gq.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qn.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://tr.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://at.shtwfgs.cn

[A19] 交换两个变量
来源：http://or.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://fg.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ge.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://zx.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://uq.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://ct.bjjhwx.cn

Go:   a, b = b, a
来源：http://gx.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://yt.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://lm.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://zx.nicolike.cn

Py:   name = input("请输入：")
来源：http://mp.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tl.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fr.colortex.cn

TS:   // Node.js：readline 模块
来源：http://yf.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ct.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cf.nszjky.cn

Ruby: gets.chomp
来源：http://jp.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://dg.asd995.cn

[A21] 保留指定小数位输出
来源：http://dz.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://in.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yq.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://pp.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://xp.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://ju.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ku.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://el.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://td.muxihuayi.cn

[A22] 获取字符串长度
来源：http://pp.shxzskj.cn

Py:   len(s)
来源：http://zx.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sc.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ww.hnjuh.cn

TS:   s.length
来源：http://es.hnjuh.cn

Java: s.length()
来源：http://zs.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://db.521024.cn

Ruby: s.length
来源：http://bq.hnjuh.cn

C#:   s.Length
来源：http://tm.jctech888.com.cn

[A23] 大小写转换
来源：http://fo.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nd.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oy.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ca.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hd.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://he.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xz.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uz.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pb.shxzskj.cn

[A24] 去除首尾空白
来源：http://rf.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rd.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hp.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://he.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vv.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://od.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://bg.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wy.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ci.gzmigu.cn

[A25] 字符串比较
来源：http://dq.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://li.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zn.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bv.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ex.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tt.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dv.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uz.nszjky.cn

[A26] 类型转换总览
来源：http://dh.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xl.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nm.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dv.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://nu.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mn.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nh.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vg.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ms.shxzskj.cn

================================================================================
来源：http://lz.yuexingan06.cn

B. 流程控制
来源：http://lm.bjjhwx.cn

================================================================================
来源：http://eo.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://nv.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fj.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ls.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tf.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xd.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tj.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fu.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bt.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qk.szsharing.cn

[B02] 多分支 else if / elif
来源：http://lb.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yg.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lq.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fq.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ip.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mt.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nb.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.nicolike.cn

[B03] switch / match / case
来源：http://zf.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xm.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://om.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uc.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zd.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ey.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pn.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://an.huixiangedu.cn

[B04] for 计数循环
来源：http://pr.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://kl.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ib.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dt.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ua.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hg.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rq.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://rq.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://du.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://mw.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://jk.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ck.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yz.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mz.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tf.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uf.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://rx.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mj.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://uk.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bc.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lb.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sh.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tu.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mc.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wq.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bv.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hr.chemitech.net.cn

[B07] while 循环
来源：http://ui.asd995.cn

Py:   while i < 10: i += 1
来源：http://oi.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wb.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://iw.521024.cn

TS:   while (i < 10) { i++; }
来源：http://fi.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://on.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aj.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://pz.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://bn.521024.cn

[B08] do-while（至少执行一次）
来源：http://dx.jianghongdianzi.cn


<!-- 参考信息 -->