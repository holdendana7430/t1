代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://wh.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://xh.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://iv.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ua.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://lp.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ev.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ai.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ma.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jx.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://vs.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://we.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://or.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yg.asd995.cn

[A03] 常量定义
来源：http://sg.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rt.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://ch.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://bo.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://ci.521024.cn

Java: static final double PI = 3.14159;
来源：http://wm.nszjky.cn

Go:   const PI = 3.14159
来源：http://ja.9csxet.cn

Ruby: PI = 3.14159
来源：http://ml.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://oj.haigaiapp.cn

[A04] 判断变量类型
来源：http://ri.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cd.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lr.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://td.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://cv.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qu.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ns.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yf.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://tk.hnjuh.cn

[A05] 整数除法与取模
来源：http://cg.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ou.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ps.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://od.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zw.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://cy.521024.cn

Go:   7 / 2; 7 % 2
来源：http://vy.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://tg.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://by.asd995.cn

[A06] 字符串转数字
来源：http://mu.colortex.cn

Py:   int("42"); float("3.14")
来源：http://qz.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xe.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zh.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uk.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iy.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cp.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uf.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ho.hnjuh.cn

[A07] 数字转字符串
来源：http://em.shxzskj.cn

Py:   str(42)
来源：http://wm.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://sz.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://nk.shtwfgs.cn

TS:   String(42)
来源：http://xc.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ht.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://fd.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://fv.haigaiapp.cn

C#:   42.ToString()
来源：http://in.huanxung.cn

[A08] 取整与四舍五入
来源：http://vp.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cn.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ta.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ej.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hx.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bu.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vx.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ct.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ik.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://ci.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tn.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://we.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yw.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vn.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qw.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cl.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://go.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cv.hahajie.cn

[A10] 生成随机数
来源：http://in.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://mg.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://gx.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lp.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yn.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://lg.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cp.hahajie.cn

Ruby: rand(1..100)
来源：http://es.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://tj.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://ut.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://zr.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gv.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yr.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://af.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ct.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dg.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xm.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qw.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://yr.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://me.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ue.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://jr.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://fg.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yl.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bk.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://pt.asd995.cn

C#:   $"Hello, {name}!"
来源：http://yq.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ld.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://qs.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://ym.szsharing.cn

JS:   "第一行\n第二行"
来源：http://tj.asd995.cn

TS:   "第一行\n第二行"
来源：http://pm.asd995.cn

Java: "第一行\n第二行"
来源：http://fs.nszjky.cn

Go:   "第一行\n第二行"
来源：http://js.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://yb.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://xb.bjjhwx.cn

[A14] 注释写法
来源：http://uo.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zl.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uv.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ay.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://nx.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wj.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://cl.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ut.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://bw.shxzukj.cn

[A15] 空值判断与默认值
来源：http://xe.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://im.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://uc.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://eq.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://ho.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oc.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://dw.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://sd.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://hs.huixiangedu.cn

[A16] 真假值判断规则
来源：http://qi.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ci.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qw.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cg.jctech888.com.cn

TS:   if (!x) {}
来源：http://xe.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zr.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kb.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nf.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mv.yuexingan06.cn

[A17] 位运算
来源：http://lw.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gz.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wo.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zx.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://xu.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://gf.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://wc.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kl.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://id.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://gn.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dp.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://zr.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://zz.muxihuayi.cn

[A19] 交换两个变量
来源：http://bu.haigaiapp.cn

Py:   a, b = b, a
来源：http://ea.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vf.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ni.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://en.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://wh.muxihuayi.cn

Go:   a, b = b, a
来源：http://tl.muxihuayi.cn

Ruby: a, b = b, a
来源：http://iy.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://cd.hahajie.cn

[A20] 读取标准输入
来源：http://zu.shxzskj.cn

Py:   name = input("请输入：")
来源：http://me.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qd.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://je.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://hv.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://fl.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bc.nicolike.cn

Ruby: gets.chomp
来源：http://im.newstarts.cn

C#:   Console.ReadLine();
来源：http://qe.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ug.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ob.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jb.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://nl.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://zo.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://ln.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gu.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://qv.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://bi.chemitech.net.cn

[A22] 获取字符串长度
来源：http://sn.szxytkj.cn

Py:   len(s)
来源：http://kt.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cp.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nz.gzmigu.cn

TS:   s.length
来源：http://kw.521024.cn

Java: s.length()
来源：http://xa.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fy.szsharing.cn

Ruby: s.length
来源：http://sf.nszjky.cn

C#:   s.Length
来源：http://dl.shxzskj.cn

[A23] 大小写转换
来源：http://mk.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rk.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tr.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gi.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ur.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://av.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bo.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gk.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tn.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://ml.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nj.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pc.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ap.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://js.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ep.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://of.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wl.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zm.jctech888.com.cn

[A25] 字符串比较
来源：http://xy.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tp.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ja.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://op.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pv.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uz.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ry.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rk.bjjhwx.cn

[A26] 类型转换总览
来源：http://rx.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ad.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yj.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cp.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://pt.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pa.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ye.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sb.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xp.jctech888.com.cn

================================================================================
来源：http://kb.szsharing.cn

B. 流程控制
来源：http://sj.521024.cn

================================================================================
来源：http://vs.colortex.cn

[B01] 条件判断 if / else
来源：http://mq.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://td.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pr.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://au.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kz.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uu.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hw.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fk.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ex.hahajie.cn

[B02] 多分支 else if / elif
来源：http://fi.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ub.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ku.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dc.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oh.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sk.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wk.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ow.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ct.shxzskj.cn

[B03] switch / match / case
来源：http://zz.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ra.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dx.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hv.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oa.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bq.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ku.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vn.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://om.lnxyls.cn

[B04] for 计数循环
来源：http://ku.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://dy.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qy.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pn.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wk.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xv.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xe.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://jv.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://br.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://nc.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://iu.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pq.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wm.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gv.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fy.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ss.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://pd.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://br.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://nt.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://of.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rp.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rt.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kl.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mo.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gv.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vu.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xa.huixinmuqiang.cn

[B07] while 循环
来源：http://vz.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://cn.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lj.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://zr.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://dm.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://do.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xw.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://ab.521024.cn

C#:   while (i < 10) { i++; }
来源：http://xj.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://pq.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://sb.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kv.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://og.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://pc.wgjwhj.cn


<!-- 参考信息 -->