代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://qb.nszjky.cn

[A03] 常量定义
来源：http://ph.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gm.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://qm.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://kk.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://fw.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://or.nszjky.cn

Go:   const PI = 3.14159
来源：http://pf.hahajie.cn

Ruby: PI = 3.14159
来源：http://ds.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://wt.huixiangedu.cn

[A04] 判断变量类型
来源：http://iu.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dm.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ok.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uh.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://yw.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ho.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pa.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uz.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://ku.asd995.cn

[A05] 整数除法与取模
来源：http://zm.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cs.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xn.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ij.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://za.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://jf.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://ff.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://op.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://en.nicolike.cn

[A06] 字符串转数字
来源：http://bf.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://uu.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wb.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ks.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lp.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ot.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nu.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nu.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hn.lnxyls.cn

[A07] 数字转字符串
来源：http://tu.lnxyls.cn

Py:   str(42)
来源：http://hw.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://nf.521024.cn

JS:   String(42); (42).toString()
来源：http://jb.shxzukj.cn

TS:   String(42)
来源：http://cj.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nn.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://an.szxytkj.cn

Ruby: 42.to_s
来源：http://lt.huixinmuqiang.cn

C#:   42.ToString()
来源：http://hb.nicolike.cn

[A08] 取整与四舍五入
来源：http://ot.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sc.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cg.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fh.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sf.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bd.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kf.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sy.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iz.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://hs.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xi.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sv.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zd.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ki.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jo.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zd.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sg.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kd.newstarts.cn

[A10] 生成随机数
来源：http://ee.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://if.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://qa.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uz.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ss.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://cb.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rj.lnxyls.cn

Ruby: rand(1..100)
来源：http://gm.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://in.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://ks.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://xs.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pw.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tf.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hv.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://vg.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zt.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rw.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yo.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://la.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://in.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bw.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://fe.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ba.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://lj.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qy.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://lx.521024.cn

C#:   $"Hello, {name}!"
来源：http://op.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://je.colortex.cn

Py:   "第一行\n第二行"
来源：http://dg.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://xd.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://cp.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://ap.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://gw.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ls.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://mg.hahajie.cn

C#:   "第一行\n第二行"
来源：http://qh.asd995.cn

[A14] 注释写法
来源：http://ze.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nj.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ln.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://pk.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://sd.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gj.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://uj.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pz.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://zu.521024.cn

[A15] 空值判断与默认值
来源：http://qt.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://yt.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://zv.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://cr.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://lm.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pr.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://zd.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://od.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://un.asd995.cn

[A16] 真假值判断规则
来源：http://lz.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xk.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qv.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pm.521024.cn

TS:   if (!x) {}
来源：http://ei.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://je.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sg.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fi.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qb.asd995.cn

[A17] 位运算
来源：http://xw.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ci.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vs.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ic.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bk.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vb.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://yv.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://gq.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://ot.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://it.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qv.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://wb.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sp.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://iv.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://tv.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://oj.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://oj.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pj.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://ti.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://nd.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://fi.hahajie.cn

Go:   a, b = b, a
来源：http://jl.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://pk.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://hl.wgjwhj.cn

[A20] 读取标准输入
来源：http://bt.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://cm.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uk.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://we.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://ne.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://fg.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dx.521024.cn

Ruby: gets.chomp
来源：http://bu.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://ul.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://xd.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://ld.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yg.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ti.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://rn.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://br.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mp.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://rb.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://xk.wgjwhj.cn

[A22] 获取字符串长度
来源：http://bx.shtwfgs.cn

Py:   len(s)
来源：http://ef.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ks.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://be.panjiajie.cn

TS:   s.length
来源：http://qa.huixiangedu.cn

Java: s.length()
来源：http://ey.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kr.bjjhwx.cn

Ruby: s.length
来源：http://kv.hahajie.cn

C#:   s.Length
来源：http://mf.panjiajie.cn

[A23] 大小写转换
来源：http://ml.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://si.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fw.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hn.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yj.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vm.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ei.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zh.hnjuh.cn

[A24] 去除首尾空白
来源：http://tz.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gs.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iq.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qm.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kh.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://zf.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://at.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://re.shxzskj.cn

[A25] 字符串比较
来源：http://qt.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ps.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yk.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vh.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cp.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fh.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://co.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pf.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fg.newstarts.cn

[A26] 类型转换总览
来源：http://jl.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ai.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mh.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://od.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://bk.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zf.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://db.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://es.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ih.panjiajie.cn

================================================================================
来源：http://zt.jctech888.com.cn

B. 流程控制
来源：http://ad.bookmarksfly.cn

================================================================================
来源：http://tx.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ee.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://en.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wq.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iy.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fh.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gm.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zo.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hi.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yd.9csxet.cn

[B02] 多分支 else if / elif
来源：http://qa.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xe.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hv.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ul.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://by.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wt.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fq.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.wgjwhj.cn

[B03] switch / match / case
来源：http://fn.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vy.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sb.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ku.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sc.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lr.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://la.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jd.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cx.haigaiapp.cn

[B04] for 计数循环
来源：http://ie.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://rx.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nd.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rz.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vv.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ae.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://it.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://xv.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://os.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ws.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ao.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ih.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wb.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://se.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cs.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://cp.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qi.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://wb.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lu.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gt.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://td.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ia.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hf.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iw.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ak.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ia.bookmarksfly.cn

[B07] while 循环
来源：http://ll.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://xb.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qp.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://vb.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://le.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://fh.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nc.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://ug.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://wv.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://tr.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://lu.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://an.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://wm.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://zq.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://eo.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mr.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kx.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://fu.hnjuh.cn

[B09] break 与 continue
来源：http://xl.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sr.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ws.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ld.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fo.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bi.shtwfgs.cn


<!-- 参考信息 -->