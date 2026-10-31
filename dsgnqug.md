代发 wailian999

Py:   print("Hello, World!")
来源：http://mb.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://bo.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://qc.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lr.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ig.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://yc.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://bw.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aa.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://ks.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hq.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rs.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kc.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ho.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://xp.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://sk.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://yh.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vg.huixiangedu.cn

[A03] 常量定义
来源：http://dx.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ar.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://xj.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://ep.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://rb.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://iq.huanxung.cn

Go:   const PI = 3.14159
来源：http://nl.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://pm.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://js.hnjuh.cn

[A04] 判断变量类型
来源：http://hh.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jg.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tr.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zc.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://eb.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://af.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tk.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mz.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://lr.nicolike.cn

[A05] 整数除法与取模
来源：http://ke.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yd.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://th.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rd.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jz.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://wy.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://wz.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://uk.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://vo.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://qo.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://kf.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wa.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xd.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qt.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fr.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ws.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pm.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zm.jctech888.com.cn

[A07] 数字转字符串
来源：http://sq.yuexingan06.cn

Py:   str(42)
来源：http://yy.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://ri.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ce.huanxung.cn

TS:   String(42)
来源：http://ex.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kf.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://aw.chemitech.net.cn

Ruby: 42.to_s
来源：http://hl.hnjuh.cn

C#:   42.ToString()
来源：http://pz.szxytkj.cn

[A08] 取整与四舍五入
来源：http://in.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://el.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ek.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qv.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dg.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xx.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wp.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uk.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://df.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://rd.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://va.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sl.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zr.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ml.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qt.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dx.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kr.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kv.9csxet.cn

[A10] 生成随机数
来源：http://zf.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://xd.9csxet.cn

PHP:  random_int(1, 100);
来源：http://mh.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://us.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wn.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://uq.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bi.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://pz.521024.cn

C#:   new Random().Next(1, 101)
来源：http://jl.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://xm.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://df.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ms.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jf.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ls.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://xl.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qj.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xl.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eq.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://yo.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ui.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zh.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://ga.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ra.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://jw.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://du.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://oh.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://bb.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zi.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://ig.colortex.cn

PHP:  "第一行\n第二行"
来源：http://gt.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://hn.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://oi.lnxyls.cn

Java: "第一行\n第二行"
来源：http://xg.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://cv.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ny.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://ki.szxytkj.cn

[A14] 注释写法
来源：http://nb.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://be.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bc.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://qo.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://nl.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vn.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://ea.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lz.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://gl.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://xc.hahajie.cn

Py:   value = data or "默认值"
来源：http://bn.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://oa.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://yx.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://vb.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mg.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://vy.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://sf.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://kx.yuexingan06.cn

[A16] 真假值判断规则
来源：http://yq.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qi.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wu.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ge.hahajie.cn

TS:   if (!x) {}
来源：http://nt.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tw.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qa.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ly.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uv.hahajie.cn

[A17] 位运算
来源：http://ai.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hr.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vb.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mv.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://if.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xm.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://eb.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://mz.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://oa.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bl.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hp.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ij.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hc.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://vb.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://wq.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://qp.nszjky.cn

Py:   a, b = b, a
来源：http://sv.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yn.521024.cn

JS:   [a, b] = [b, a];
来源：http://tl.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://lw.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://tc.yuexingan06.cn

Go:   a, b = b, a
来源：http://ge.muxihuayi.cn

Ruby: a, b = b, a
来源：http://qb.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://qb.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://rl.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://xt.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jd.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ct.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://wc.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ny.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jh.chemitech.net.cn

Ruby: gets.chomp
来源：http://ee.szsharing.cn

C#:   Console.ReadLine();
来源：http://jy.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://nx.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://hd.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ui.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://tb.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://qs.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://lb.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bw.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://ay.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://sc.huanxung.cn

[A22] 获取字符串长度
来源：http://nc.haigaiapp.cn

Py:   len(s)
来源：http://hh.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qn.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tv.huanxung.cn

TS:   s.length
来源：http://xy.hnjuh.cn

Java: s.length()
来源：http://ih.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yw.haigaiapp.cn

Ruby: s.length
来源：http://sj.haigaiapp.cn

C#:   s.Length
来源：http://af.panjiajie.cn

[A23] 大小写转换
来源：http://ct.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qh.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tk.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hb.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vd.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oz.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bp.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dp.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hx.gzmigu.cn

[A24] 去除首尾空白
来源：http://bl.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://az.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pv.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tq.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wz.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fj.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://jv.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zo.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sf.bjjhwx.cn

[A25] 字符串比较
来源：http://aw.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://nt.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rt.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fh.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dx.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tl.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ee.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sd.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xa.bookmarksfly.cn

[A26] 类型转换总览
来源：http://oq.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wr.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lp.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aw.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ib.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rc.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cr.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://au.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iv.shxzukj.cn

================================================================================
来源：http://et.hnjuh.cn

B. 流程控制
来源：http://gv.nicolike.cn

================================================================================
来源：http://ud.asd995.cn

[B01] 条件判断 if / else
来源：http://kg.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aj.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uu.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vy.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zl.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://in.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wn.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tg.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://og.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://va.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lq.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mq.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iw.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cg.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tb.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yv.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.nicolike.cn

[B03] switch / match / case
来源：http://rp.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vd.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cz.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://on.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cc.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pn.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wk.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ax.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://np.jctech888.com.cn

[B04] for 计数循环
来源：http://jp.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://uw.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hq.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zv.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ez.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ts.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://mn.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sn.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://dv.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://lm.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bh.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nx.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xf.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kk.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mj.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gm.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://hi.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tf.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rp.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sv.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sr.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ts.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ea.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fo.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bj.jianghongdianzi.cn

[B07] while 循环
来源：http://ip.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://nb.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qk.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://dt.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://fq.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://yz.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://av.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://nd.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://qb.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://zc.bookmarksfly.cn


<!-- 参考信息 -->