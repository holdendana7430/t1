代发 wailian999

Ruby: PI = 3.14159
来源：http://ko.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://sg.nicolike.cn

[A04] 判断变量类型
来源：http://mn.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bv.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ln.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fs.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://iu.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gy.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tk.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kp.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://er.huixiangedu.cn

[A05] 整数除法与取模
来源：http://lx.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nq.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iz.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://us.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kt.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://xm.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://zp.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://pu.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://rd.lnxyls.cn

[A06] 字符串转数字
来源：http://pq.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://mg.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ow.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ak.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ws.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dc.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wj.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ab.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jr.gzmigu.cn

[A07] 数字转字符串
来源：http://si.bookmarksfly.cn

Py:   str(42)
来源：http://bj.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://ft.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://bt.huixinmuqiang.cn

TS:   String(42)
来源：http://iy.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sf.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://zn.huixiangedu.cn

Ruby: 42.to_s
来源：http://dw.lnxyls.cn

C#:   42.ToString()
来源：http://ae.521024.cn

[A08] 取整与四舍五入
来源：http://uq.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yv.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hv.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dx.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ai.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yy.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rn.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zo.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ti.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://ov.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bp.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bq.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sp.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ox.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bi.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sj.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yt.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ds.panjiajie.cn

[A10] 生成随机数
来源：http://dr.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://bk.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ai.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yd.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qe.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://ke.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ox.huixiangedu.cn

Ruby: rand(1..100)
来源：http://bx.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://ww.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://po.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ye.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dy.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pa.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yl.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://bi.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ac.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eq.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://io.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://pq.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ig.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ca.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://gn.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://vr.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://rd.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pg.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://oj.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://in.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://or.9csxet.cn

Py:   "第一行\n第二行"
来源：http://pu.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://rg.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://ty.huanxung.cn

TS:   "第一行\n第二行"
来源：http://gc.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://sq.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://ft.521024.cn

Ruby: "第一行\n第二行"
来源：http://bc.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://eq.hahajie.cn

[A14] 注释写法
来源：http://wr.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cf.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bi.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://gr.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://sb.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vl.521024.cn

Go:   // 单行；/* 多行 */
来源：http://zr.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xt.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://ck.gzmigu.cn

[A15] 空值判断与默认值
来源：http://ee.hahajie.cn

Py:   value = data or "默认值"
来源：http://oq.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://wo.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://qt.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://qo.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vr.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://yp.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://xq.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ol.nszjky.cn

[A16] 真假值判断规则
来源：http://jm.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://is.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mh.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dj.521024.cn

TS:   if (!x) {}
来源：http://iw.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://at.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mn.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ol.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vq.haigaiapp.cn

[A17] 位运算
来源：http://kf.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mt.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cu.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gk.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ez.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ij.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://sg.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://de.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://vr.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ab.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ya.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://as.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yy.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://vf.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://cf.colortex.cn

[A19] 交换两个变量
来源：http://ux.9csxet.cn

Py:   a, b = b, a
来源：http://lu.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kx.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://pk.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://rq.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://wy.9csxet.cn

Go:   a, b = b, a
来源：http://ss.muxihuayi.cn

Ruby: a, b = b, a
来源：http://lq.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://mb.shxzskj.cn

[A20] 读取标准输入
来源：http://qr.nszjky.cn

Py:   name = input("请输入：")
来源：http://my.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kx.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jf.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://by.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ob.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jw.chemitech.net.cn

Ruby: gets.chomp
来源：http://sw.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://xl.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://sa.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://ud.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lo.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://xy.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://mx.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://nt.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nu.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://qd.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://uw.muxihuayi.cn

[A22] 获取字符串长度
来源：http://cn.wgjwhj.cn

Py:   len(s)
来源：http://ep.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ga.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sp.shxzskj.cn

TS:   s.length
来源：http://fe.521024.cn

Java: s.length()
来源：http://qz.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uq.yuntaijiaju.cn

Ruby: s.length
来源：http://wt.shtwfgs.cn

C#:   s.Length
来源：http://oa.newstarts.cn

[A23] 大小写转换
来源：http://jf.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ga.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://or.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://om.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ld.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pl.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hi.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pq.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://os.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://aw.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fz.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://io.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://us.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://la.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ty.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://wk.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cq.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eu.nicolike.cn

[A25] 字符串比较
来源：http://kk.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://gs.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kz.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dr.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yv.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dw.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tf.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ur.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vj.shxzukj.cn

[A26] 类型转换总览
来源：http://hy.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qk.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uw.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cq.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://te.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ox.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rh.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tb.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rf.newstarts.cn

================================================================================
来源：http://no.newstarts.cn

B. 流程控制
来源：http://zm.nszjky.cn

================================================================================
来源：http://ai.lnxyls.cn

[B01] 条件判断 if / else
来源：http://jh.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pj.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://os.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ya.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xl.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lw.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xa.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wo.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jp.colortex.cn

[B02] 多分支 else if / elif
来源：http://ji.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mm.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tk.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mh.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ms.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ha.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.yuexingan06.cn

[B03] switch / match / case
来源：http://bd.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cm.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bp.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mh.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nm.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uv.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fw.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gk.colortex.cn

[B04] for 计数循环
来源：http://ba.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://ez.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://al.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aa.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dg.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xg.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dw.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://xz.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://me.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://qz.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ta.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kk.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pe.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qj.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tv.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://mi.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kz.colortex.cn

[B06] 遍历字典 / 对象
来源：http://wh.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ty.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mq.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://at.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rs.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ib.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zq.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zy.nszjky.cn

[B07] while 循环
来源：http://xw.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://xd.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iv.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://qk.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://ps.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ec.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://th.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ke.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://xy.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://dr.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://yq.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aw.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://vo.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://xb.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://vc.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sa.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wk.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://xn.yuexingan06.cn

[B09] break 与 continue
来源：http://my.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kh.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bc.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mi.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gs.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rq.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.9csxet.cn

[B10] 遍历同时拿索引
来源：http://ak.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cw.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xp.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ch.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vz.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ch.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sc.hahajie.cn


<!-- 参考信息 -->