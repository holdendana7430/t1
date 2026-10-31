代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://io.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pc.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://hn.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hh.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ue.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ds.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://vf.szsharing.cn

[A05] 整数除法与取模
来源：http://gi.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zz.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fj.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ew.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://td.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://ca.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://mj.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://sx.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://ha.nszjky.cn

[A06] 字符串转数字
来源：http://yh.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://wt.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sh.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dj.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hf.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oh.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ok.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sl.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wr.panjiajie.cn

[A07] 数字转字符串
来源：http://bf.yuexingan06.cn

Py:   str(42)
来源：http://ri.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://fn.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://se.bookmarksfly.cn

TS:   String(42)
来源：http://mt.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://no.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://dp.nicolike.cn

Ruby: 42.to_s
来源：http://xk.chemitech.net.cn

C#:   42.ToString()
来源：http://yy.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://hh.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ng.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pz.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sp.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ov.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sx.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dh.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lq.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://sx.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qz.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cp.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vj.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://un.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ar.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nj.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://it.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ez.nicolike.cn

[A10] 生成随机数
来源：http://ot.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ru.huanxung.cn

PHP:  random_int(1, 100);
来源：http://ry.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rt.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mh.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://um.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dc.jctech888.com.cn

Ruby: rand(1..100)
来源：http://eu.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://vy.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://ek.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://mr.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ev.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pk.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bv.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://yd.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vs.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pi.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nw.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://ou.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://js.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gx.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://wv.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://ir.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://jl.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zp.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://ta.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://ng.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lh.newstarts.cn

Py:   "第一行\n第二行"
来源：http://hs.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://ox.9csxet.cn

JS:   "第一行\n第二行"
来源：http://uj.521024.cn

TS:   "第一行\n第二行"
来源：http://yu.szsharing.cn

Java: "第一行\n第二行"
来源：http://bb.huanxung.cn

Go:   "第一行\n第二行"
来源：http://pa.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://ja.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://bf.shxzskj.cn

[A14] 注释写法
来源：http://sw.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gm.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oo.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://yy.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ky.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xz.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://ej.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wf.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://lq.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ap.shxzukj.cn

Py:   value = data or "默认值"
来源：http://hy.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ji.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://sv.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://nw.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gp.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://jb.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://nl.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://fy.nszjky.cn

[A16] 真假值判断规则
来源：http://ap.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ke.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://of.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yr.9csxet.cn

TS:   if (!x) {}
来源：http://tg.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vg.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dc.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yc.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yd.bookmarksfly.cn

[A17] 位运算
来源：http://wg.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oe.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zx.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oq.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nx.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rd.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jd.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://od.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://an.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://uz.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://lu.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fq.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pv.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://kx.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ne.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://aw.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://ga.huixiangedu.cn

[A19] 交换两个变量
来源：http://dk.huixiangedu.cn

Py:   a, b = b, a
来源：http://lr.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gb.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://ea.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://bd.521024.cn

Java: int t = a; a = b; b = t;
来源：http://ys.szxytkj.cn

Go:   a, b = b, a
来源：http://ne.wgjwhj.cn

Ruby: a, b = b, a
来源：http://fk.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://zz.wgjwhj.cn

[A20] 读取标准输入
来源：http://hh.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ld.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yp.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bz.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://rr.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://wf.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://te.hnjuh.cn

Ruby: gets.chomp
来源：http://kj.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://zm.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://vm.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://qm.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tm.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://yj.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://va.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://xh.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ut.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://zm.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://ma.chemitech.net.cn

[A22] 获取字符串长度
来源：http://rf.yuntaijiaju.cn

Py:   len(s)
来源：http://rh.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vn.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://su.hnjuh.cn

TS:   s.length
来源：http://cx.huixinmuqiang.cn

Java: s.length()
来源：http://wq.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bq.huixiangedu.cn

Ruby: s.length
来源：http://wn.huixiangedu.cn

C#:   s.Length
来源：http://ut.nszjky.cn

[A23] 大小写转换
来源：http://zr.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yw.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ae.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mv.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lv.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qq.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://he.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nw.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pa.shtwfgs.cn

[A24] 去除首尾空白
来源：http://wf.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qo.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cx.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fl.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ek.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://at.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eh.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://om.haigaiapp.cn

[A25] 字符串比较
来源：http://nw.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://as.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rf.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sf.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qk.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zv.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ke.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sc.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ct.nszjky.cn

[A26] 类型转换总览
来源：http://ui.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kk.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mo.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pi.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://ke.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hu.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wk.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ad.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bh.haigaiapp.cn

================================================================================
来源：http://oz.shxzskj.cn

B. 流程控制
来源：http://lp.muxihuayi.cn

================================================================================
来源：http://ou.shxzukj.cn

[B01] 条件判断 if / else
来源：http://ww.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fv.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uh.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pt.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://px.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fd.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eg.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://ws.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ta.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ti.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://av.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bi.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wx.huanxung.cn

[B03] switch / match / case
来源：http://ky.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dh.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bc.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cp.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wn.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zh.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qi.haigaiapp.cn

[B04] for 计数循环
来源：http://fq.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://kb.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pa.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yp.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://df.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oq.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pz.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://sj.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fy.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ux.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://fx.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ys.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dg.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xx.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oh.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ty.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://ms.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://pn.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ee.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yb.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sl.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vt.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oh.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pl.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ds.huixinmuqiang.cn

[B07] while 循环
来源：http://ic.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://vv.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aw.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://la.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://zz.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://im.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jy.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://eb.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://fv.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://vc.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ev.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tf.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://zf.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://fq.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://of.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jy.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://md.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://zz.gzmigu.cn

[B09] break 与 continue
来源：http://oa.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rn.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ta.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xz.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://un.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://if.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yf.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cy.szsharing.cn

[B10] 遍历同时拿索引
来源：http://dr.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lk.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zn.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wb.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mp.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vo.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yz.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yv.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://st.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://id.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ak.szxytkj.cn


<!-- 参考信息 -->