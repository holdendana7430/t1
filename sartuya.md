代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ko.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://sx.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://ky.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://sx.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ig.panjiajie.cn

[A03] 常量定义
来源：http://mt.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://st.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://jc.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://jm.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://wi.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://vq.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://fl.newstarts.cn

Ruby: PI = 3.14159
来源：http://uw.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://zq.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://bh.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jv.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rf.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xc.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://cz.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bz.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cp.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tb.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ox.newstarts.cn

[A05] 整数除法与取模
来源：http://ap.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://df.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://we.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xo.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ey.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://pi.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://dd.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://mh.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://rn.yuexingan06.cn

[A06] 字符串转数字
来源：http://nd.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://cq.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qz.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://te.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bf.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ab.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hc.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gg.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://go.shxzskj.cn

[A07] 数字转字符串
来源：http://tz.haigaiapp.cn

Py:   str(42)
来源：http://lk.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://go.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://un.huixiangedu.cn

TS:   String(42)
来源：http://jw.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nu.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://tt.jctech888.com.cn

Ruby: 42.to_s
来源：http://vp.9csxet.cn

C#:   42.ToString()
来源：http://rt.shxzskj.cn

[A08] 取整与四舍五入
来源：http://sx.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nq.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ia.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ys.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nb.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tk.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aq.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mg.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aa.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://os.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wb.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mu.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qk.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jv.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cf.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ex.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ox.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tl.muxihuayi.cn

[A10] 生成随机数
来源：http://ti.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://ro.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://zd.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pe.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qi.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://rz.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bb.9csxet.cn

Ruby: rand(1..100)
来源：http://bp.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://uf.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://mj.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://jh.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wh.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lp.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mo.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://lc.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sh.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mx.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ek.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://cn.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aj.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ow.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://tr.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://oy.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://ry.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vg.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://rc.colortex.cn

C#:   $"Hello, {name}!"
来源：http://vs.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ti.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://zo.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://tg.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://gv.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://qv.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://st.colortex.cn

Go:   "第一行\n第二行"
来源：http://ib.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://xw.nicolike.cn

C#:   "第一行\n第二行"
来源：http://qx.wgjwhj.cn

[A14] 注释写法
来源：http://hx.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ke.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hp.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ex.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://vk.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jb.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://lr.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yf.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://zh.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://jk.shxzukj.cn

Py:   value = data or "默认值"
来源：http://rn.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://tu.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://sn.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://vt.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fa.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://nx.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://dx.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://au.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://qb.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wa.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ih.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lt.asd995.cn

TS:   if (!x) {}
来源：http://rg.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wu.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fy.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zq.nszjky.cn

[A17] 位运算
来源：http://ac.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lp.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tv.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gj.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zi.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hi.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ce.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://gk.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://kg.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://aj.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qv.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xv.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://yf.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ym.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://iq.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://kl.haigaiapp.cn

[A19] 交换两个变量
来源：http://gp.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://mi.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uh.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://rl.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://dc.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://zg.521024.cn

Go:   a, b = b, a
来源：http://ge.shxzskj.cn

Ruby: a, b = b, a
来源：http://wo.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://ck.shxzskj.cn

[A20] 读取标准输入
来源：http://fa.szxytkj.cn

Py:   name = input("请输入：")
来源：http://hj.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gf.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wo.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://dq.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://dr.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://up.panjiajie.cn

Ruby: gets.chomp
来源：http://xq.colortex.cn

C#:   Console.ReadLine();
来源：http://qv.nszjky.cn

[A21] 保留指定小数位输出
来源：http://bc.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://uw.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uv.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://nn.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://de.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://tq.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cw.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://oi.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://sh.szxytkj.cn

[A22] 获取字符串长度
来源：http://tm.haigaiapp.cn

Py:   len(s)
来源：http://lh.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dy.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ir.colortex.cn

TS:   s.length
来源：http://ol.asd995.cn

Java: s.length()
来源：http://qe.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sg.huixinmuqiang.cn

Ruby: s.length
来源：http://tg.bookmarksfly.cn

C#:   s.Length
来源：http://cr.521024.cn

[A23] 大小写转换
来源：http://qz.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bs.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hg.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pt.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tk.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yu.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gs.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rb.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jy.huanxung.cn

[A24] 去除首尾空白
来源：http://hj.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ct.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vp.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mx.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lp.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ff.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://dq.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bq.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://we.huanxung.cn

[A25] 字符串比较
来源：http://ma.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://kt.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nv.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://al.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tx.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nf.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ad.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://me.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qh.nicolike.cn

[A26] 类型转换总览
来源：http://mx.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xf.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ca.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dr.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ju.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ab.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zg.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ms.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kh.shtwfgs.cn

================================================================================
来源：http://ny.chemitech.net.cn

B. 流程控制
来源：http://vu.huanxung.cn

================================================================================
来源：http://mu.lnxyls.cn

[B01] 条件判断 if / else
来源：http://aw.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lv.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bz.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fq.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sd.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sb.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ge.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eu.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rd.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://cf.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hp.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gw.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://io.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ea.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.huanxung.cn

[B03] switch / match / case
来源：http://so.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sm.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zl.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kc.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sn.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://au.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nr.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kn.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kb.huixinmuqiang.cn

[B04] for 计数循环
来源：http://tv.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://fp.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uw.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dm.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qd.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qq.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tl.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://ke.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ev.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://kd.521024.cn

Py:   for item in arr: print(item)
来源：http://wk.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ia.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bh.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tc.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pj.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://bl.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yx.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://cz.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pf.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ja.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zv.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://np.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yt.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sw.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qd.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aj.nszjky.cn

[B07] while 循环
来源：http://kq.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://hz.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aj.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://sa.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://ku.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://ja.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iw.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://to.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://qi.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://cd.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://gs.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wp.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://qw.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://ai.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://xy.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://av.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kx.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://lf.hahajie.cn

[B09] break 与 continue
来源：http://cf.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zd.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://co.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.jctech888.com.cn


<!-- 参考信息 -->