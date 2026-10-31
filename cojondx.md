代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://lm.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://cq.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://zg.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fi.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ym.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yo.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lj.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gh.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aj.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://ij.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://kg.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://gk.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fq.wgjwhj.cn

[A03] 常量定义
来源：http://ca.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kc.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://le.colortex.cn

JS:   const PI = 3.14159;
来源：http://qo.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://eq.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://ya.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://yt.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://yx.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://ek.hahajie.cn

[A04] 判断变量类型
来源：http://nl.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://um.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tt.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iz.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ui.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ry.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kk.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ol.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://tj.huixiangedu.cn

[A05] 整数除法与取模
来源：http://kg.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://am.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dz.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nm.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tf.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://id.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://is.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://gx.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://dg.asd995.cn

[A06] 字符串转数字
来源：http://cj.colortex.cn

Py:   int("42"); float("3.14")
来源：http://cm.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lo.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ub.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rk.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mp.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rs.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://by.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vb.muxihuayi.cn

[A07] 数字转字符串
来源：http://ou.hahajie.cn

Py:   str(42)
来源：http://cy.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://do.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://ac.shxzukj.cn

TS:   String(42)
来源：http://gm.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://st.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://tz.haigaiapp.cn

Ruby: 42.to_s
来源：http://ck.hnjuh.cn

C#:   42.ToString()
来源：http://fm.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://sh.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cj.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ke.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tx.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fd.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ky.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aw.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mp.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qk.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://hl.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ji.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tl.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jk.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ls.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://te.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rz.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://js.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wr.lnxyls.cn

[A10] 生成随机数
来源：http://sm.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://us.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://sp.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xc.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ce.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://wk.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mm.chemitech.net.cn

Ruby: rand(1..100)
来源：http://dp.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://nq.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://zq.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://qw.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hn.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ky.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xd.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://dn.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yc.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ky.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ii.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://bs.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vg.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yo.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://sf.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://ke.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://bq.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lm.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://gd.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://xl.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lv.521024.cn

Py:   "第一行\n第二行"
来源：http://lm.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://re.huanxung.cn

JS:   "第一行\n第二行"
来源：http://pj.szsharing.cn

TS:   "第一行\n第二行"
来源：http://lu.hnjuh.cn

Java: "第一行\n第二行"
来源：http://lt.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ni.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ou.hahajie.cn

C#:   "第一行\n第二行"
来源：http://yb.jianghongdianzi.cn

[A14] 注释写法
来源：http://wi.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pf.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lg.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ud.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://tn.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vs.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://vw.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ai.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://wy.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://ac.hnjuh.cn

Py:   value = data or "默认值"
来源：http://qr.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://zv.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://vt.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://xr.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nz.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://sh.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://gj.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://mo.gzmigu.cn

[A16] 真假值判断规则
来源：http://at.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xm.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fy.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xr.huixiangedu.cn

TS:   if (!x) {}
来源：http://ht.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uj.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hg.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oi.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://co.bjjhwx.cn

[A17] 位运算
来源：http://uj.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ep.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zy.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wq.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hy.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ml.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ld.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ix.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://yn.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://qd.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://ev.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rh.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wj.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://ek.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://og.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://pn.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://ab.szsharing.cn

[A19] 交换两个变量
来源：http://cr.9csxet.cn

Py:   a, b = b, a
来源：http://bh.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lb.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://ps.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://vp.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://zh.haigaiapp.cn

Go:   a, b = b, a
来源：http://jp.huixiangedu.cn

Ruby: a, b = b, a
来源：http://lb.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://ev.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://xu.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://iw.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dh.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hi.colortex.cn

TS:   // Node.js：readline 模块
来源：http://fl.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://gr.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yi.newstarts.cn

Ruby: gets.chomp
来源：http://ja.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://cb.huanxung.cn

[A21] 保留指定小数位输出
来源：http://vr.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://hh.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lp.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://tv.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://lj.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://zy.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ea.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://wx.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://xg.newstarts.cn

[A22] 获取字符串长度
来源：http://er.jctech888.com.cn

Py:   len(s)
来源：http://wy.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://re.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://op.bjjhwx.cn

TS:   s.length
来源：http://do.yuexingan06.cn

Java: s.length()
来源：http://gk.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ig.colortex.cn

Ruby: s.length
来源：http://tl.huixiangedu.cn

C#:   s.Length
来源：http://mb.jctech888.com.cn

[A23] 大小写转换
来源：http://eu.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ez.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pm.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jz.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://go.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ka.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vn.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yz.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ef.gzmigu.cn

[A24] 去除首尾空白
来源：http://nv.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jk.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://za.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://my.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pl.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://wn.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jd.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ya.hahajie.cn

[A25] 字符串比较
来源：http://ti.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://lx.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sl.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ub.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cj.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xz.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xj.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hg.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://op.wgjwhj.cn

[A26] 类型转换总览
来源：http://xf.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hx.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tv.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xx.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://wn.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ey.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ja.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jk.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mf.shxzskj.cn

================================================================================
来源：http://iv.chemitech.net.cn

B. 流程控制
来源：http://pd.jianghongdianzi.cn

================================================================================
来源：http://lz.521024.cn

[B01] 条件判断 if / else
来源：http://lr.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xb.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cr.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pg.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ya.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://if.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hq.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ji.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://je.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://pm.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dt.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rz.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sh.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gq.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://og.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.9csxet.cn

[B03] switch / match / case
来源：http://nr.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ke.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ne.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dp.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qd.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://av.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zm.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gb.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yf.bookmarksfly.cn

[B04] for 计数循环
来源：http://mg.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://cd.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mc.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vn.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mr.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ov.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://by.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ks.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tr.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://go.hahajie.cn

Py:   for item in arr: print(item)
来源：http://gq.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kv.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://og.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://le.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mr.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tq.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://mh.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vl.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://zt.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://id.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xz.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fr.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tg.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fj.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ve.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iw.gzmigu.cn

[B07] while 循环
来源：http://kt.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://dj.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xp.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://vw.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://pn.521024.cn

Java: while (i < 10) { i++; }
来源：http://vj.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://so.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://pw.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://mq.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://ps.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://bt.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xs.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://pl.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://te.panjiajie.cn


<!-- 参考信息 -->