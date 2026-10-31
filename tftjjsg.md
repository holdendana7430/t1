代发 wailian999

[A02] 变量声明与赋值
来源：http://cy.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ha.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mn.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ck.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lf.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://mf.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://tb.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://dm.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mr.9csxet.cn

[A03] 常量定义
来源：http://na.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wh.asd995.cn

PHP:  const PI = 3.14159;
来源：http://cy.szsharing.cn

JS:   const PI = 3.14159;
来源：http://pp.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://yl.colortex.cn

Java: static final double PI = 3.14159;
来源：http://qy.hnjuh.cn

Go:   const PI = 3.14159
来源：http://zm.shxzukj.cn

Ruby: PI = 3.14159
来源：http://fp.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://dt.hnjuh.cn

[A04] 判断变量类型
来源：http://jo.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ig.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://os.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kz.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://vl.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pk.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ee.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ob.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://zr.yuexingan06.cn

[A05] 整数除法与取模
来源：http://nx.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pp.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qy.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ol.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sl.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://kv.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://nv.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://tx.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://rv.szxytkj.cn

[A06] 字符串转数字
来源：http://uu.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://av.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fg.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nv.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wi.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pp.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oq.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mg.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wi.newstarts.cn

[A07] 数字转字符串
来源：http://ky.huixiangedu.cn

Py:   str(42)
来源：http://ag.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://dj.huanxung.cn

JS:   String(42); (42).toString()
来源：http://qh.wgjwhj.cn

TS:   String(42)
来源：http://de.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yx.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://uc.colortex.cn

Ruby: 42.to_s
来源：http://fa.nicolike.cn

C#:   42.ToString()
来源：http://mx.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://bh.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://st.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ax.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ss.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mu.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ax.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pz.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wb.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://te.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hs.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bw.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kh.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ul.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tt.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://km.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sb.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ii.haigaiapp.cn

[A10] 生成随机数
来源：http://re.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://jx.hahajie.cn

PHP:  random_int(1, 100);
来源：http://po.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hm.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aw.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://tt.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ya.nszjky.cn

Ruby: rand(1..100)
来源：http://gr.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://tt.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://jk.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://xt.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://is.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://du.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oe.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://wt.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vt.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://le.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bn.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://pj.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ox.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://re.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://wa.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://ih.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://jl.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xk.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://pe.521024.cn

C#:   $"Hello, {name}!"
来源：http://ld.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vb.nszjky.cn

Py:   "第一行\n第二行"
来源：http://sg.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://zb.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://ti.hahajie.cn

TS:   "第一行\n第二行"
来源：http://vy.nszjky.cn

Java: "第一行\n第二行"
来源：http://sy.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ud.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://vw.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://mj.gzmigu.cn

[A14] 注释写法
来源：http://kc.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mm.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pw.521024.cn

JS:   // 单行；/* 多行 */
来源：http://it.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://xj.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pt.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://pp.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ad.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://qn.nicolike.cn

[A15] 空值判断与默认值
来源：http://qd.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://jk.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://bz.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://bc.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://hu.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pg.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://wt.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://cm.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://um.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://lm.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://el.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ho.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://py.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://lm.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ht.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xi.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lr.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jt.chemitech.net.cn

[A17] 位运算
来源：http://iy.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dl.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mq.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xb.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zx.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yt.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ph.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://sj.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://sk.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://ky.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ho.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ie.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://vj.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ca.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://eh.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://rl.chemitech.net.cn

[A19] 交换两个变量
来源：http://hp.nicolike.cn

Py:   a, b = b, a
来源：http://il.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fy.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ck.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://fm.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://qa.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://xk.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://ls.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://my.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://gk.huanxung.cn

Py:   name = input("请输入：")
来源：http://qx.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ps.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cm.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://ss.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://fn.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uc.huanxung.cn

Ruby: gets.chomp
来源：http://kv.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://vu.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://nu.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ky.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nd.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://dw.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://gx.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://pa.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://py.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://nv.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://zn.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://fb.chemitech.net.cn

Py:   len(s)
来源：http://ku.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://me.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yj.lnxyls.cn

TS:   s.length
来源：http://gl.wgjwhj.cn

Java: s.length()
来源：http://aq.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dz.hahajie.cn

Ruby: s.length
来源：http://xt.521024.cn

C#:   s.Length
来源：http://bn.bjjhwx.cn

[A23] 大小写转换
来源：http://kz.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hn.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://up.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ag.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oc.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ip.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ll.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lu.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://as.panjiajie.cn

[A24] 去除首尾空白
来源：http://hy.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://um.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qg.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ia.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kv.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nu.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://lu.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dl.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mr.shxzukj.cn

[A25] 字符串比较
来源：http://wr.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://dh.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cu.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wz.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tr.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://md.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sx.gzmigu.cn

[A26] 类型转换总览
来源：http://kh.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vq.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dd.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ag.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://gb.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jp.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://up.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aj.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fy.hahajie.cn

================================================================================
来源：http://tk.gzmigu.cn

B. 流程控制
来源：http://yk.haigaiapp.cn

================================================================================
来源：http://wv.colortex.cn

[B01] 条件判断 if / else
来源：http://qz.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rs.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ox.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lb.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uk.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ku.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tf.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fa.9csxet.cn

[B02] 多分支 else if / elif
来源：http://ko.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kw.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://el.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bj.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://go.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uz.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ar.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xw.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qs.shtwfgs.cn

[B03] switch / match / case
来源：http://dm.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rr.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ze.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qy.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vo.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ru.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zl.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xx.nszjky.cn

[B04] for 计数循环
来源：http://jt.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ur.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qt.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ze.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oc.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ec.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://js.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ej.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://yd.nicolike.cn

Py:   for item in arr: print(item)
来源：http://nv.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ym.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bm.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wr.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ca.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ku.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://hu.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xo.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://io.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ib.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://br.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ol.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sw.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bv.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ae.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mz.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oc.haigaiapp.cn

[B07] while 循环
来源：http://ax.nszjky.cn

Py:   while i < 10: i += 1
来源：http://on.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fo.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://ex.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://vq.521024.cn

Java: while (i < 10) { i++; }
来源：http://ki.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ev.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://eo.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://rp.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://zm.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://eb.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ei.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://ub.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://zt.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://iv.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zs.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dr.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://ov.jctech888.com.cn


<!-- 参考信息 -->