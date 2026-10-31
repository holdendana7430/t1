代发 wailian999

Ruby: PI = 3.14159
来源：http://io.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://yc.shtwfgs.cn

[A04] 判断变量类型
来源：http://ex.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cy.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yl.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lp.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://bn.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fm.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mb.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ws.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://fi.bjjhwx.cn

[A05] 整数除法与取模
来源：http://no.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sl.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nd.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jp.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pj.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://tv.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://ix.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://bt.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://zj.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://bq.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://ae.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uv.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sn.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://em.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ki.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ma.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gb.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ls.asd995.cn

[A07] 数字转字符串
来源：http://fo.hnjuh.cn

Py:   str(42)
来源：http://us.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://dt.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://ue.shtwfgs.cn

TS:   String(42)
来源：http://td.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ik.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://hu.wgjwhj.cn

Ruby: 42.to_s
来源：http://be.huixinmuqiang.cn

C#:   42.ToString()
来源：http://su.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://jg.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ue.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jl.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qf.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lw.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mv.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://if.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wy.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eh.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://hv.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qp.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ie.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://om.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vn.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jg.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pm.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bg.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ws.asd995.cn

[A10] 生成随机数
来源：http://gh.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://pc.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ve.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ng.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tg.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://yp.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vt.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://sk.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ag.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://qh.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://zw.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ol.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://re.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gd.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://jr.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pi.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vc.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rs.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://dq.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yj.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hw.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://dl.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://va.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://ud.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://on.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://wt.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://dh.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wl.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://af.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://so.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://fx.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://cc.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://pp.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://ju.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://cj.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://pr.colortex.cn

[A14] 注释写法
来源：http://ee.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vb.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fr.521024.cn

JS:   // 单行；/* 多行 */
来源：http://vn.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://uz.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ut.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://pf.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xo.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://ag.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://bb.szxytkj.cn

Py:   value = data or "默认值"
来源：http://jz.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://it.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://xw.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://wo.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wo.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://vr.521024.cn

Ruby: value = data || "默认值"
来源：http://xv.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://aq.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://kf.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gz.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iw.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pq.nicolike.cn

TS:   if (!x) {}
来源：http://fs.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zg.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jv.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fs.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://je.yuntaijiaju.cn

[A17] 位运算
来源：http://yi.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zd.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://os.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vq.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fg.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vo.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://xa.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://bb.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://il.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wg.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gn.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://uy.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sr.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://sc.colortex.cn

C#:   (int)'A'; (char)65
来源：http://gx.lnxyls.cn

[A19] 交换两个变量
来源：http://ix.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://me.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cw.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://qx.asd995.cn

TS:   [a, b] = [b, a];
来源：http://so.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://xv.szxytkj.cn

Go:   a, b = b, a
来源：http://rb.szsharing.cn

Ruby: a, b = b, a
来源：http://qu.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://xs.chemitech.net.cn

[A20] 读取标准输入
来源：http://mw.szxytkj.cn

Py:   name = input("请输入：")
来源：http://tw.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zo.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rf.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://bw.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ly.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oh.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://pk.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://dv.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://vv.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://qf.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://by.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://gg.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://jq.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://rb.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sp.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://bd.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://ui.nszjky.cn

[A22] 获取字符串长度
来源：http://rz.chemitech.net.cn

Py:   len(s)
来源：http://vu.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ey.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yx.lnxyls.cn

TS:   s.length
来源：http://fo.huanxung.cn

Java: s.length()
来源：http://xq.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ul.shtwfgs.cn

Ruby: s.length
来源：http://js.wgjwhj.cn

C#:   s.Length
来源：http://im.9csxet.cn

[A23] 大小写转换
来源：http://ca.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sx.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vu.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qn.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eh.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lb.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bh.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://se.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cd.szxytkj.cn

[A24] 去除首尾空白
来源：http://bt.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://of.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jp.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uf.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pk.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://et.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://kt.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qk.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gk.shxzukj.cn

[A25] 字符串比较
来源：http://eu.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ct.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ev.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pw.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nw.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tf.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sc.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bm.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oa.shxzukj.cn

[A26] 类型转换总览
来源：http://zo.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ii.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ln.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dm.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://vv.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gd.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ej.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lw.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jp.nicolike.cn

================================================================================
来源：http://cx.huixiangedu.cn

B. 流程控制
来源：http://iv.shtwfgs.cn

================================================================================
来源：http://rx.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://gw.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rf.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cm.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ju.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://so.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mt.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zb.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zw.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://by.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ht.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iu.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hk.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zi.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qv.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ze.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xn.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.shtwfgs.cn

[B03] switch / match / case
来源：http://gg.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ca.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jj.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sw.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fz.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sr.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://em.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ea.521024.cn

[B04] for 计数循环
来源：http://yn.colortex.cn

Py:   for i in range(10): print(i)
来源：http://mo.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oj.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tj.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://va.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xl.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ke.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://cb.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ct.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://qc.521024.cn

Py:   for item in arr: print(item)
来源：http://wp.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gx.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hf.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zo.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cs.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://om.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://fb.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ip.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://py.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hp.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kx.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gv.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://we.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ih.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qx.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ck.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fl.jctech888.com.cn

[B07] while 循环
来源：http://bj.huanxung.cn

Py:   while i < 10: i += 1
来源：http://nb.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xd.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://od.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://ft.colortex.cn

Java: while (i < 10) { i++; }
来源：http://yb.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ei.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://hu.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://gv.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://ui.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://dw.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xp.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://pd.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://kr.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://mk.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mg.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nt.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://fw.haigaiapp.cn

[B09] break 与 continue
来源：http://nd.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zb.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yw.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dj.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wv.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://fj.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sl.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lt.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oj.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ii.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aq.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pz.wgjwhj.cn


<!-- 参考信息 -->