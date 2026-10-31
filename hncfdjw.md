代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yv.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wz.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://oy.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tw.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vs.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://go.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://mb.panjiajie.cn

[A05] 整数除法与取模
来源：http://nl.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tb.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pv.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://de.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cb.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://jz.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://gw.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://zv.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://pt.asd995.cn

[A06] 字符串转数字
来源：http://vl.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://pa.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vo.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ur.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wr.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ka.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://za.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ou.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wm.9csxet.cn

[A07] 数字转字符串
来源：http://rw.chemitech.net.cn

Py:   str(42)
来源：http://ak.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://ut.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://nh.shtwfgs.cn

TS:   String(42)
来源：http://fh.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ml.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://sm.yuexingan06.cn

Ruby: 42.to_s
来源：http://fe.jctech888.com.cn

C#:   42.ToString()
来源：http://bb.panjiajie.cn

[A08] 取整与四舍五入
来源：http://iz.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dx.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ao.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rh.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://td.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lh.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zs.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wy.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bb.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://oy.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hh.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vc.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ee.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pn.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ty.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wh.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ne.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nh.huixinmuqiang.cn

[A10] 生成随机数
来源：http://fk.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://lq.9csxet.cn

PHP:  random_int(1, 100);
来源：http://bb.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eb.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pl.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://gw.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zk.shxzskj.cn

Ruby: rand(1..100)
来源：http://ft.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://qm.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://en.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ap.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ha.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zj.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wb.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zl.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ri.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ug.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://by.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://fn.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://im.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gj.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://dg.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://sp.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://mq.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://be.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://wp.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://uw.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://so.nszjky.cn

Py:   "第一行\n第二行"
来源：http://fq.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ih.huanxung.cn

JS:   "第一行\n第二行"
来源：http://ag.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://au.panjiajie.cn

Java: "第一行\n第二行"
来源：http://vf.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://vo.colortex.cn

Ruby: "第一行\n第二行"
来源：http://ae.newstarts.cn

C#:   "第一行\n第二行"
来源：http://xn.yuntaijiaju.cn

[A14] 注释写法
来源：http://pi.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vt.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qp.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://qn.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://rm.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ar.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://fd.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ve.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://ds.szxytkj.cn

[A15] 空值判断与默认值
来源：http://dv.nicolike.cn

Py:   value = data or "默认值"
来源：http://ls.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://dc.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://xx.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://mt.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vp.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://gf.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://vd.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://yq.shxzukj.cn

[A16] 真假值判断规则
来源：http://pl.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wu.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tg.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lk.hnjuh.cn

TS:   if (!x) {}
来源：http://zg.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qr.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vg.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xx.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gr.colortex.cn

[A17] 位运算
来源：http://of.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qk.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fk.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oe.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sc.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://az.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pk.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ie.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://ml.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://oh.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://qg.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vu.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ty.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://as.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://px.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://su.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://nn.asd995.cn

[A19] 交换两个变量
来源：http://bb.szsharing.cn

Py:   a, b = b, a
来源：http://gf.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sq.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ku.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://bb.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://ai.shxzskj.cn

Go:   a, b = b, a
来源：http://ui.shxzukj.cn

Ruby: a, b = b, a
来源：http://uz.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://oo.9csxet.cn

[A20] 读取标准输入
来源：http://nf.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://fo.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tl.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yw.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://vb.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://wa.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://im.huanxung.cn

Ruby: gets.chomp
来源：http://ls.gzmigu.cn

C#:   Console.ReadLine();
来源：http://wj.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://xc.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://ad.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ib.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://pp.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://qn.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://tb.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rc.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://er.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://dx.shxzukj.cn

[A22] 获取字符串长度
来源：http://qt.nszjky.cn

Py:   len(s)
来源：http://ll.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xb.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ei.9csxet.cn

TS:   s.length
来源：http://ti.muxihuayi.cn

Java: s.length()
来源：http://le.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ge.hnjuh.cn

Ruby: s.length
来源：http://rx.chemitech.net.cn

C#:   s.Length
来源：http://wb.newstarts.cn

[A23] 大小写转换
来源：http://mt.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ck.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wn.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oa.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ph.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wc.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gr.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nh.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.gzmigu.cn

[A24] 去除首尾空白
来源：http://bg.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://za.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jg.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qq.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zi.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ym.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://dq.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ac.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sl.nszjky.cn

[A25] 字符串比较
来源：http://pe.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://vx.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yk.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rm.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ng.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kt.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://re.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bz.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mn.haigaiapp.cn

[A26] 类型转换总览
来源：http://eu.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hr.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rd.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sn.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://ny.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oi.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bx.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bi.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ny.newstarts.cn

================================================================================
来源：http://si.wgjwhj.cn

B. 流程控制
来源：http://zq.bjjhwx.cn

================================================================================
来源：http://ig.colortex.cn

[B01] 条件判断 if / else
来源：http://og.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gh.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ni.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bv.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gw.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rm.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rk.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lb.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tx.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://ss.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yn.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ws.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xc.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wb.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tn.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zk.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://go.huanxung.cn

[B03] switch / match / case
来源：http://yp.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vi.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vq.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rn.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://on.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wt.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://le.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gk.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bq.521024.cn

[B04] for 计数循环
来源：http://eu.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://rk.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ur.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aq.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sw.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oi.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aq.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://qu.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yh.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://xq.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://yd.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://an.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sy.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vt.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://po.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ut.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://gc.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ke.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://uy.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cu.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pv.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sj.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bo.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jc.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ng.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tz.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kl.huixinmuqiang.cn

[B07] while 循环
来源：http://rm.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://pm.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://we.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://rp.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://je.521024.cn

Java: while (i < 10) { i++; }
来源：http://ms.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zr.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://lm.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://na.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ug.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ek.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://re.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://qr.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://di.521024.cn

Java: do { i++; } while (i < 10);
来源：http://av.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tx.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ps.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://xs.nicolike.cn

[B09] break 与 continue
来源：http://le.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ns.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sp.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qi.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bi.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.szsharing.cn

[B10] 遍历同时拿索引
来源：http://as.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sv.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kk.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uw.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yx.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bf.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lb.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sj.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xp.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://tz.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://iq.lnxyls.cn


<!-- 参考信息 -->