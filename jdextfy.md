代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bk.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mv.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://jz.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ch.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sj.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nx.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://uu.bjjhwx.cn

[A05] 整数除法与取模
来源：http://yd.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://df.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ka.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cd.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fk.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://xu.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://tt.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://lz.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://mq.lnxyls.cn

[A06] 字符串转数字
来源：http://ol.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://zx.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dd.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://au.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iu.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ys.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ou.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cf.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jy.wgjwhj.cn

[A07] 数字转字符串
来源：http://ub.gzmigu.cn

Py:   str(42)
来源：http://qt.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://me.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://kx.yuexingan06.cn

TS:   String(42)
来源：http://ei.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qp.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://wr.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://xa.jctech888.com.cn

C#:   42.ToString()
来源：http://tu.nszjky.cn

[A08] 取整与四舍五入
来源：http://cm.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lq.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rd.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qz.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pq.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rb.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ex.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xa.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kc.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://lk.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cg.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wq.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ry.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fn.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pu.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xs.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uj.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vu.huixinmuqiang.cn

[A10] 生成随机数
来源：http://qc.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://en.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://th.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vn.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ae.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://cr.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jt.wgjwhj.cn

Ruby: rand(1..100)
来源：http://md.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://td.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://pr.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://vy.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zv.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://as.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fg.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://hm.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://so.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rp.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lh.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://mt.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cq.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://og.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://ab.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://qn.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://on.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sg.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://he.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://zu.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dw.huanxung.cn

Py:   "第一行\n第二行"
来源：http://fb.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://us.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://cr.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://fm.huanxung.cn

Java: "第一行\n第二行"
来源：http://tt.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://kr.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://ai.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://mm.shtwfgs.cn

[A14] 注释写法
来源：http://ql.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oq.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hw.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://io.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://pw.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dy.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://uk.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qo.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://np.colortex.cn

[A15] 空值判断与默认值
来源：http://cy.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ny.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://cp.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://rd.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://hf.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xc.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://bx.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://fo.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ee.chemitech.net.cn

[A16] 真假值判断规则
来源：http://lh.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ea.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eu.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ff.bjjhwx.cn

TS:   if (!x) {}
来源：http://jh.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ie.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ks.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ni.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pg.wgjwhj.cn

[A17] 位运算
来源：http://hc.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qv.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qn.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gp.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yu.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://or.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://mo.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://dg.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ln.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mv.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://ab.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yr.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://by.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ns.huixiangedu.cn

[A19] 交换两个变量
来源：http://db.haigaiapp.cn

Py:   a, b = b, a
来源：http://vk.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jv.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://tq.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://tc.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://xd.hnjuh.cn

Go:   a, b = b, a
来源：http://dt.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://dp.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://du.huixiangedu.cn

[A20] 读取标准输入
来源：http://wp.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://cx.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://co.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ai.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://xt.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ia.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qw.szsharing.cn

Ruby: gets.chomp
来源：http://fj.szxytkj.cn

C#:   Console.ReadLine();
来源：http://pe.nszjky.cn

[A21] 保留指定小数位输出
来源：http://hy.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://ex.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://op.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://mx.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://xb.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://lm.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xe.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://ic.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://sz.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://jt.gzmigu.cn

Py:   len(s)
来源：http://ag.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ci.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sw.yuntaijiaju.cn

TS:   s.length
来源：http://nr.panjiajie.cn

Java: s.length()
来源：http://wi.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ow.hnjuh.cn

Ruby: s.length
来源：http://bt.shxzukj.cn

C#:   s.Length
来源：http://fm.9csxet.cn

[A23] 大小写转换
来源：http://bb.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uz.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hy.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ts.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bf.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gd.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sb.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lo.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hs.shtwfgs.cn

[A24] 去除首尾空白
来源：http://re.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xx.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pl.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hw.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jt.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fo.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://kd.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vs.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vb.wgjwhj.cn

[A25] 字符串比较
来源：http://wl.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://gs.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qc.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bj.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dt.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ud.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gu.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ew.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jv.521024.cn

[A26] 类型转换总览
来源：http://gh.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lx.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cd.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ul.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://so.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pf.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ic.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ah.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nd.bjjhwx.cn

================================================================================
来源：http://fs.hahajie.cn

B. 流程控制
来源：http://jk.jctech888.com.cn

================================================================================
来源：http://ij.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ia.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qm.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ls.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oh.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gt.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dh.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uo.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mc.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wz.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://ir.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://av.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ip.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fa.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fg.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zt.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ff.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vx.huixinmuqiang.cn

[B03] switch / match / case
来源：http://lg.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ch.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jp.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ho.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lo.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://do.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mo.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bk.hnjuh.cn

[B04] for 计数循环
来源：http://fo.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://tx.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vw.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sq.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://an.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://si.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://by.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://qn.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rt.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://sb.huanxung.cn

Py:   for item in arr: print(item)
来源：http://nv.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vx.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bd.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ia.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aw.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://go.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://mb.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gp.521024.cn

[B06] 遍历字典 / 对象
来源：http://cw.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sg.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uf.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ar.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qp.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ae.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://es.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ke.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hh.muxihuayi.cn

[B07] while 循环
来源：http://kz.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://tx.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rd.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://im.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://zb.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://iu.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gu.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://ob.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://hk.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://qs.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://tq.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pi.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://lp.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://yb.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://lc.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tv.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nr.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://mr.asd995.cn

[B09] break 与 continue
来源：http://nx.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cf.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zm.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sy.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qx.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.521024.cn

[B10] 遍历同时拿索引
来源：http://au.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oj.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ip.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ss.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tt.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mv.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kb.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wr.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jd.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://mt.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://nu.colortex.cn


<!-- 参考信息 -->