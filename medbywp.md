代发 wailian999

JS:   const PI = 3.14159;
来源：http://nb.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://sn.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://gx.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://wp.panjiajie.cn

Ruby: PI = 3.14159
来源：http://bq.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://qq.nszjky.cn

[A04] 判断变量类型
来源：http://uj.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eh.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qq.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oq.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://ed.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lv.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ep.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ez.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://dh.bjjhwx.cn

[A05] 整数除法与取模
来源：http://qq.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yb.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ff.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yv.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gz.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://hp.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://ye.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://ri.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://pm.asd995.cn

[A06] 字符串转数字
来源：http://qk.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://gi.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ii.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ae.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sg.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tk.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zq.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vy.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yd.muxihuayi.cn

[A07] 数字转字符串
来源：http://ov.shtwfgs.cn

Py:   str(42)
来源：http://us.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://fq.newstarts.cn

JS:   String(42); (42).toString()
来源：http://nw.hahajie.cn

TS:   String(42)
来源：http://ls.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eo.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://dv.colortex.cn

Ruby: 42.to_s
来源：http://ga.szxytkj.cn

C#:   42.ToString()
来源：http://mx.asd995.cn

[A08] 取整与四舍五入
来源：http://go.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cg.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zf.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bs.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ut.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sk.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cu.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://po.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gu.521024.cn

[A09] 绝对值与最大最小值
来源：http://kv.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pl.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mu.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qa.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yb.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rk.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bn.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://av.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bh.muxihuayi.cn

[A10] 生成随机数
来源：http://bv.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://sq.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://pd.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gs.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xu.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://hj.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ce.muxihuayi.cn

Ruby: rand(1..100)
来源：http://ls.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://ms.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://pg.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://qi.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sx.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ti.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dp.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://mx.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ho.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pp.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qx.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://mk.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ht.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xd.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://fi.asd995.cn

TS:   `Hello, ${name}!`
来源：http://up.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://ga.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iv.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://yw.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://id.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fs.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://hh.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://sd.colortex.cn

JS:   "第一行\n第二行"
来源：http://ge.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://lt.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ko.nszjky.cn

Go:   "第一行\n第二行"
来源：http://ok.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://gb.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://uc.huanxung.cn

[A14] 注释写法
来源：http://gw.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ex.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fj.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://uu.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://xk.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://we.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://dl.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ye.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://nn.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://sv.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://jf.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://iw.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://ke.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://ok.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zk.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://qd.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://un.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://bn.chemitech.net.cn

[A16] 真假值判断规则
来源：http://bz.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ss.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dh.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://om.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://tw.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ni.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dc.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zo.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kg.lnxyls.cn

[A17] 位运算
来源：http://ot.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kb.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://an.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lb.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zz.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ld.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yx.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://wu.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://cx.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://xt.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cz.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tt.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://nk.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xm.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://az.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://vt.bjjhwx.cn

[A19] 交换两个变量
来源：http://zi.yuexingan06.cn

Py:   a, b = b, a
来源：http://ie.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://im.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://pu.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://po.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://lx.szsharing.cn

Go:   a, b = b, a
来源：http://tw.shxzukj.cn

Ruby: a, b = b, a
来源：http://ag.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://jb.9csxet.cn

[A20] 读取标准输入
来源：http://cb.szxytkj.cn

Py:   name = input("请输入：")
来源：http://yg.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mi.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xb.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://hm.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://qh.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wr.huanxung.cn

Ruby: gets.chomp
来源：http://vn.panjiajie.cn

C#:   Console.ReadLine();
来源：http://rc.hahajie.cn

[A21] 保留指定小数位输出
来源：http://zx.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://yz.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ka.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://yt.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://dh.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://vh.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vk.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://da.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://qj.hnjuh.cn

[A22] 获取字符串长度
来源：http://ol.shxzukj.cn

Py:   len(s)
来源：http://fi.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yf.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zv.gzmigu.cn

TS:   s.length
来源：http://fr.wgjwhj.cn

Java: s.length()
来源：http://mf.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nv.hahajie.cn

Ruby: s.length
来源：http://dg.huixiangedu.cn

C#:   s.Length
来源：http://id.lnxyls.cn

[A23] 大小写转换
来源：http://yx.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nd.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://de.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wa.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ww.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ij.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ct.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lr.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wq.szsharing.cn

[A24] 去除首尾空白
来源：http://nd.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kr.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://an.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://df.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uc.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mr.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://ue.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cw.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ue.newstarts.cn

[A25] 字符串比较
来源：http://df.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://yx.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nq.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ub.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ep.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ab.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://us.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ty.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ot.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://om.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rc.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sq.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ph.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://vp.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gf.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nf.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xm.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ha.huanxung.cn

================================================================================
来源：http://sq.huixinmuqiang.cn

B. 流程控制
来源：http://zh.yuntaijiaju.cn

================================================================================
来源：http://lw.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://rb.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://be.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ub.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bw.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://he.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bs.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kb.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wa.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ym.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://ky.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uk.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gc.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hm.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bl.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vp.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.521024.cn

[B03] switch / match / case
来源：http://rp.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cw.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tt.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tx.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wf.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://he.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://at.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cg.shxzukj.cn

[B04] for 计数循环
来源：http://bw.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://gc.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xd.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zm.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sc.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dh.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ug.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://sm.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nq.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://am.nszjky.cn

Py:   for item in arr: print(item)
来源：http://ni.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aw.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gx.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tu.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sr.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ww.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://su.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sj.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://qv.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gt.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iq.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ir.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lr.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ne.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hl.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qn.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wl.chemitech.net.cn

[B07] while 循环
来源：http://ph.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://fn.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://er.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://xi.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://hm.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://ht.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rj.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://co.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://px.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://az.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://qf.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cq.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://st.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://pg.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://lj.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rb.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dr.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://it.szxytkj.cn

[B09] break 与 continue
来源：http://lm.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vq.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://go.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nk.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pm.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ar.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.nicolike.cn

[B10] 遍历同时拿索引
来源：http://zm.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mv.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bg.muxihuayi.cn


<!-- 参考信息 -->