代发 wailian999

JS:   const PI = 3.14159;
来源：http://bs.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://ii.colortex.cn

Java: static final double PI = 3.14159;
来源：http://ra.9csxet.cn

Go:   const PI = 3.14159
来源：http://so.newstarts.cn

Ruby: PI = 3.14159
来源：http://tm.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://cb.szxytkj.cn

[A04] 判断变量类型
来源：http://zt.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wu.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rb.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ed.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://rq.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qw.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xs.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uq.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://fl.lnxyls.cn

[A05] 整数除法与取模
来源：http://bn.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oz.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://px.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nc.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jv.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://aq.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://mh.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://nx.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://tr.521024.cn

[A06] 字符串转数字
来源：http://fv.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://yx.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ve.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://se.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kv.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qe.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ji.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tw.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rr.shxzskj.cn

[A07] 数字转字符串
来源：http://kj.haigaiapp.cn

Py:   str(42)
来源：http://ki.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://ri.huanxung.cn

JS:   String(42); (42).toString()
来源：http://xp.asd995.cn

TS:   String(42)
来源：http://ow.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xd.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://dh.shxzukj.cn

Ruby: 42.to_s
来源：http://zn.bookmarksfly.cn

C#:   42.ToString()
来源：http://dq.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://cy.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jp.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jw.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xy.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ih.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://js.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lp.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wv.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lc.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://wq.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fx.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ze.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://no.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://us.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eo.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sl.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yw.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ju.haigaiapp.cn

[A10] 生成随机数
来源：http://zz.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://ru.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://cr.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wk.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pu.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://eu.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tk.huanxung.cn

Ruby: rand(1..100)
来源：http://sb.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://jt.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://ao.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://zp.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fc.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ac.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uy.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://co.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nm.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fl.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xl.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://er.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ya.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aa.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://mk.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://zk.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://fm.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bv.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://oy.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://ri.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jz.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://cv.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://cn.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://mr.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://cq.colortex.cn

Java: "第一行\n第二行"
来源：http://ji.9csxet.cn

Go:   "第一行\n第二行"
来源：http://uz.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://ih.colortex.cn

C#:   "第一行\n第二行"
来源：http://uk.lnxyls.cn

[A14] 注释写法
来源：http://qr.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lf.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sn.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://ig.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ke.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qi.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://xg.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kx.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://kz.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://be.newstarts.cn

Py:   value = data or "默认值"
来源：http://ws.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://dx.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://rn.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://wi.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vv.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://us.newstarts.cn

Ruby: value = data || "默认值"
来源：http://wf.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://rw.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://gj.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ac.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wb.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mn.chemitech.net.cn

TS:   if (!x) {}
来源：http://nn.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ec.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xj.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zp.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lr.huixiangedu.cn

[A17] 位运算
来源：http://gh.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qe.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gj.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ju.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://ng.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://zm.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://gn.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gr.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rv.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://nq.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kv.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://sk.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://yk.huanxung.cn

[A19] 交换两个变量
来源：http://jr.haigaiapp.cn

Py:   a, b = b, a
来源：http://it.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hq.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://pj.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://kk.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://dh.bookmarksfly.cn

Go:   a, b = b, a
来源：http://rd.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://hz.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://mz.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://xk.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://zi.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ux.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lb.asd995.cn

TS:   // Node.js：readline 模块
来源：http://xk.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://mk.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://it.lnxyls.cn

Ruby: gets.chomp
来源：http://uu.panjiajie.cn

C#:   Console.ReadLine();
来源：http://rq.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://wn.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://cx.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sg.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://eb.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://nq.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://ud.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jg.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://nf.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://wf.hahajie.cn

[A22] 获取字符串长度
来源：http://tf.newstarts.cn

Py:   len(s)
来源：http://fv.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jk.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qp.jctech888.com.cn

TS:   s.length
来源：http://bw.521024.cn

Java: s.length()
来源：http://vz.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zc.huanxung.cn

Ruby: s.length
来源：http://hb.bjjhwx.cn

C#:   s.Length
来源：http://td.huixiangedu.cn

[A23] 大小写转换
来源：http://kk.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kj.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rg.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zm.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gu.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fh.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yn.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nm.newstarts.cn

[A24] 去除首尾空白
来源：http://xz.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kj.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yg.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dg.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mc.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lv.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://ia.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://di.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hc.shxzskj.cn

[A25] 字符串比较
来源：http://cf.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://xw.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rh.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vh.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ur.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qs.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lw.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eb.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ex.chemitech.net.cn

[A26] 类型转换总览
来源：http://cb.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ua.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cn.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cr.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://yu.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ou.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vp.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zk.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://li.haigaiapp.cn

B. 流程控制
来源：http://lu.huixiangedu.cn

================================================================================
来源：http://ly.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://vm.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ns.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mc.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wl.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iy.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wy.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oo.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ev.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://wg.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ew.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xu.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pv.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://th.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://en.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nf.9csxet.cn

[B03] switch / match / case
来源：http://fx.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oz.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ea.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gy.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lf.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qq.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fx.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tc.bookmarksfly.cn

[B04] for 计数循环
来源：http://nh.521024.cn

Py:   for i in range(10): print(i)
来源：http://uq.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zp.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pk.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xo.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kb.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xt.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://cy.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ap.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://ey.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ri.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mz.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xw.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hc.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://js.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zv.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://gl.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qp.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://cf.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pb.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lo.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bh.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fz.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rg.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bt.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ix.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eh.szxytkj.cn

[B07] while 循环
来源：http://ql.szsharing.cn

Py:   while i < 10: i += 1
来源：http://hr.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hw.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://sk.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ag.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://kt.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xj.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://oo.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://jt.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ow.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://sr.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vf.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://kl.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://pv.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://vd.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dd.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nl.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://hs.muxihuayi.cn

[B09] break 与 continue
来源：http://dh.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mq.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qh.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rd.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vs.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://pf.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sz.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ko.huanxung.cn


<!-- 参考信息 -->