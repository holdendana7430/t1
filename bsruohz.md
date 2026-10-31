代发 wailian999

[A02] 变量声明与赋值
来源：http://lq.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zg.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mb.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ps.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uu.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://ot.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://da.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://bo.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yo.chemitech.net.cn

[A03] 常量定义
来源：http://qz.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ml.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://td.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://pw.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://wq.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://se.hahajie.cn

Go:   const PI = 3.14159
来源：http://sv.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://fm.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://xr.gzmigu.cn

[A04] 判断变量类型
来源：http://if.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pn.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fe.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xi.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://to.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gy.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bn.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rr.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://ya.chemitech.net.cn

[A05] 整数除法与取模
来源：http://af.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hl.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ob.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mj.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uy.521024.cn

Java: 7 / 2; 7 % 2
来源：http://op.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://jz.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ae.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://km.haigaiapp.cn

[A06] 字符串转数字
来源：http://gm.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ou.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fp.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jj.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qw.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kq.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sz.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zf.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nu.shxzukj.cn

[A07] 数字转字符串
来源：http://zz.asd995.cn

Py:   str(42)
来源：http://yp.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://ix.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://hw.newstarts.cn

TS:   String(42)
来源：http://oj.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zs.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://zc.gzmigu.cn

Ruby: 42.to_s
来源：http://ra.asd995.cn

C#:   42.ToString()
来源：http://hq.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://st.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tu.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zs.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pk.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vo.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qg.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hp.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gj.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jw.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://of.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gd.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ko.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://km.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vb.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hg.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pb.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ex.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dy.wgjwhj.cn

[A10] 生成随机数
来源：http://by.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://pg.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://cd.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://my.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wt.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://xb.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zy.panjiajie.cn

Ruby: rand(1..100)
来源：http://yt.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://wx.hahajie.cn

[A11] 条件表达式（三元）
来源：http://fn.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://vh.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pf.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qq.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://js.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wc.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jz.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pv.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zo.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://sp.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zl.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ys.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://sc.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ku.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://ns.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lu.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://ww.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://la.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ff.521024.cn

Py:   "第一行\n第二行"
来源：http://zo.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://dz.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://qz.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://pc.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://ww.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://xz.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://ru.newstarts.cn

C#:   "第一行\n第二行"
来源：http://yf.shxzukj.cn

[A14] 注释写法
来源：http://en.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rl.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sa.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://wk.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://nv.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ef.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://ud.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ns.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://iq.shxzskj.cn

[A15] 空值判断与默认值
来源：http://cs.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://pc.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://cc.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://dp.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://qb.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jc.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://du.9csxet.cn

Ruby: value = data || "默认值"
来源：http://wn.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://aj.szsharing.cn

[A16] 真假值判断规则
来源：http://bo.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cu.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bf.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yn.shxzukj.cn

TS:   if (!x) {}
来源：http://vj.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bw.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wg.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ze.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gk.huixiangedu.cn

[A17] 位运算
来源：http://nt.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yh.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bo.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rt.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nm.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://bo.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://rn.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://sm.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://od.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://hb.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eb.521024.cn

Ruby: "A".ord; 65.chr
来源：http://jd.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://en.gzmigu.cn

[A19] 交换两个变量
来源：http://dg.panjiajie.cn

Py:   a, b = b, a
来源：http://oh.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ql.asd995.cn

JS:   [a, b] = [b, a];
来源：http://sv.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://vz.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://ka.huixiangedu.cn

Go:   a, b = b, a
来源：http://ej.bjjhwx.cn

Ruby: a, b = b, a
来源：http://ju.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://qx.nszjky.cn

[A20] 读取标准输入
来源：http://js.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://vg.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hj.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ok.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ql.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ue.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wj.521024.cn

Ruby: gets.chomp
来源：http://tc.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://yp.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://us.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://ps.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xl.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://po.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://pt.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://jx.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ki.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://lr.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://qr.gzmigu.cn

[A22] 获取字符串长度
来源：http://zy.asd995.cn

Py:   len(s)
来源：http://rr.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tg.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qo.bookmarksfly.cn

TS:   s.length
来源：http://cc.newstarts.cn

Java: s.length()
来源：http://tw.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oo.hahajie.cn

Ruby: s.length
来源：http://pl.bookmarksfly.cn

C#:   s.Length
来源：http://ld.shtwfgs.cn

[A23] 大小写转换
来源：http://uv.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fp.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yc.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zc.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ah.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ht.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ed.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yu.wgjwhj.cn

[A24] 去除首尾空白
来源：http://tl.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vn.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dx.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://es.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cd.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wx.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://ss.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jb.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oq.jianghongdianzi.cn

[A25] 字符串比较
来源：http://lr.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://fc.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iq.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ar.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gm.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ce.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zo.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://el.hnjuh.cn

[A26] 类型转换总览
来源：http://ol.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aa.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wj.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sm.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://vt.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ib.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://if.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iz.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yo.szxytkj.cn

================================================================================
来源：http://li.huixiangedu.cn

B. 流程控制
来源：http://xe.hahajie.cn

================================================================================
来源：http://ri.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://sy.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iu.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://of.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zt.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wt.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://io.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zp.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ch.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gt.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://sn.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ba.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zu.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nh.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jv.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.yuntaijiaju.cn

[B03] switch / match / case
来源：http://mf.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dt.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jr.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://il.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jj.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cn.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gu.nicolike.cn

[B04] for 计数循环
来源：http://zz.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ow.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mm.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nh.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://da.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hk.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tf.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://xm.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nm.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://vf.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://tg.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bp.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dw.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pr.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://en.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jf.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://zq.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lb.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://xc.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ie.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nl.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nn.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vz.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hw.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nk.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://in.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ff.yuntaijiaju.cn

[B07] while 循环
来源：http://pc.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://bw.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bw.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://bf.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://zy.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://aw.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ns.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://on.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://bh.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://xi.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://mq.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gd.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://qy.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://uz.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://id.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tf.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xv.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://wr.bjjhwx.cn


<!-- 参考信息 -->