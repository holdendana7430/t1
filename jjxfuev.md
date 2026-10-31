代发 wailian999

JS:   const PI = 3.14159;
来源：http://qq.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://vh.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://mu.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://sb.panjiajie.cn

Ruby: PI = 3.14159
来源：http://uo.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://vr.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://xr.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ib.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rb.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dn.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://hf.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xy.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xe.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ih.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://xh.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://kn.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ot.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sc.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jh.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ov.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://jg.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://ff.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://td.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://db.gzmigu.cn

[A06] 字符串转数字
来源：http://eu.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://on.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vd.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ur.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://it.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mw.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://od.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tw.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jx.gzmigu.cn

[A07] 数字转字符串
来源：http://ms.521024.cn

Py:   str(42)
来源：http://da.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://yy.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://tu.wgjwhj.cn

TS:   String(42)
来源：http://ip.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ar.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://oh.nszjky.cn

Ruby: 42.to_s
来源：http://uc.shxzskj.cn

C#:   42.ToString()
来源：http://xs.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://ds.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dh.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dp.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dg.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ww.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gd.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rp.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lu.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sx.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://pg.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xr.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gr.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sz.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sj.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pn.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://az.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kh.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yx.bjjhwx.cn

[A10] 生成随机数
来源：http://pm.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://pn.newstarts.cn

PHP:  random_int(1, 100);
来源：http://mi.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sb.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hr.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://zk.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zq.muxihuayi.cn

Ruby: rand(1..100)
来源：http://yl.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://aa.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://tl.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://nz.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fk.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lu.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pg.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://zl.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jx.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iw.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vp.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://vp.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zq.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jn.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://ct.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://xx.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://zr.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fj.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://vt.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://eo.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ob.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://io.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://xv.hahajie.cn

JS:   "第一行\n第二行"
来源：http://nw.newstarts.cn

TS:   "第一行\n第二行"
来源：http://iv.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://et.huanxung.cn

Go:   "第一行\n第二行"
来源：http://eo.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://bq.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://qs.yuexingan06.cn

[A14] 注释写法
来源：http://js.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ha.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pt.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://gc.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ae.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tl.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://cz.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jj.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://ql.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://wp.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://ju.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://cs.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://iy.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ux.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ak.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://lj.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://fn.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://gm.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://qx.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pd.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wf.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://im.hnjuh.cn

TS:   if (!x) {}
来源：http://hy.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cl.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xh.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qv.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ss.asd995.cn

[A17] 位运算
来源：http://cg.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wr.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qk.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gg.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sg.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cg.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://we.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nc.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lk.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://im.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://kt.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ni.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nx.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hd.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://ta.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gq.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://nt.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://by.panjiajie.cn

[A19] 交换两个变量
来源：http://hq.haigaiapp.cn

Py:   a, b = b, a
来源：http://ll.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hp.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://yw.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://hh.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://iv.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://wz.gzmigu.cn

Ruby: a, b = b, a
来源：http://yw.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://ro.hahajie.cn

[A20] 读取标准输入
来源：http://ho.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://xa.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iu.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vx.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://he.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hv.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vi.shtwfgs.cn

Ruby: gets.chomp
来源：http://by.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://sy.colortex.cn

[A21] 保留指定小数位输出
来源：http://td.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://fe.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rs.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://tx.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://yf.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://pc.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ii.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://dk.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://xa.chemitech.net.cn

[A22] 获取字符串长度
来源：http://cy.szxytkj.cn

Py:   len(s)
来源：http://dv.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qy.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ym.szxytkj.cn

TS:   s.length
来源：http://uw.jctech888.com.cn

Java: s.length()
来源：http://uj.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://js.hahajie.cn

Ruby: s.length
来源：http://ts.521024.cn

C#:   s.Length
来源：http://be.hnjuh.cn

[A23] 大小写转换
来源：http://wp.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jh.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://py.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bb.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ew.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nl.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mx.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://df.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fz.jctech888.com.cn

[A24] 去除首尾空白
来源：http://dd.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hj.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oo.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ii.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oi.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yg.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://re.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wz.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nb.huixiangedu.cn

[A25] 字符串比较
来源：http://eh.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://og.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ym.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kp.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ix.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nr.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xj.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ow.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pj.nicolike.cn

[A26] 类型转换总览
来源：http://tv.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xh.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pc.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iq.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://og.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oz.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hy.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fd.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zo.9csxet.cn

================================================================================
来源：http://hh.wgjwhj.cn

B. 流程控制
来源：http://lt.szsharing.cn

================================================================================
来源：http://xq.hahajie.cn

[B01] 条件判断 if / else
来源：http://xw.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ob.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wx.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cn.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ls.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ck.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://al.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://st.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sw.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://jt.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ut.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cz.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lc.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zr.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gb.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://au.lnxyls.cn

[B03] switch / match / case
来源：http://tx.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ti.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://to.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jm.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ma.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qw.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ex.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rh.shxzskj.cn

[B04] for 计数循环
来源：http://fc.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://jx.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aw.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ti.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://az.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jc.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ql.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://un.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dq.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ev.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://eb.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kw.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zx.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yo.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ur.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wz.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://lo.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ed.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://in.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vb.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xc.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://to.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jm.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ax.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ew.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ix.jianghongdianzi.cn

[B07] while 循环
来源：http://um.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://fl.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lq.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://qx.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://ak.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://fa.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://he.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://ag.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://mi.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://gv.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://py.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jq.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://oh.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://tn.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ll.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hm.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uv.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://bo.yuntaijiaju.cn

[B09] break 与 continue
来源：http://so.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cl.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ie.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ks.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mj.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://em.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://el.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hk.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://mv.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zi.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fq.newstarts.cn


<!-- 参考信息 -->