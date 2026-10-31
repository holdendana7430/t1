代发 wailian999

JS:   const PI = 3.14159;
来源：http://yb.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://co.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ti.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://jv.521024.cn

Ruby: PI = 3.14159
来源：http://kr.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://hw.shxzukj.cn

[A04] 判断变量类型
来源：http://ie.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://un.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sw.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ei.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://zs.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ac.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rp.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://km.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://zk.shxzskj.cn

[A05] 整数除法与取模
来源：http://ce.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gg.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gq.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eo.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sr.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://vy.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://yv.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://td.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://fo.yuexingan06.cn

[A06] 字符串转数字
来源：http://ff.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://sh.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gx.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ui.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ol.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sx.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kv.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dd.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://re.asd995.cn

[A07] 数字转字符串
来源：http://ua.asd995.cn

Py:   str(42)
来源：http://zc.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://iw.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://gi.huixiangedu.cn

TS:   String(42)
来源：http://bp.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rc.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://ut.521024.cn

Ruby: 42.to_s
来源：http://rr.shxzskj.cn

C#:   42.ToString()
来源：http://qw.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://oq.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gu.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tq.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ic.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hf.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yu.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wb.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wj.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://za.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://yh.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ay.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dv.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fg.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ez.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qn.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jw.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wp.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ag.huixinmuqiang.cn

[A10] 生成随机数
来源：http://vq.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://uq.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://ny.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hj.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ts.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ze.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uy.wgjwhj.cn

Ruby: rand(1..100)
来源：http://hn.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://rm.huanxung.cn

[A11] 条件表达式（三元）
来源：http://oz.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://ps.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ll.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kj.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dl.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://fi.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dw.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xp.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yb.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://sa.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xz.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ig.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ju.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://qo.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://oj.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rf.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://jv.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://ne.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dx.nszjky.cn

Py:   "第一行\n第二行"
来源：http://qh.asd995.cn

PHP:  "第一行\n第二行"
来源：http://at.9csxet.cn

JS:   "第一行\n第二行"
来源：http://wb.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://fr.nszjky.cn

Java: "第一行\n第二行"
来源：http://ij.521024.cn

Go:   "第一行\n第二行"
来源：http://bq.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://rk.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://os.wgjwhj.cn

[A14] 注释写法
来源：http://vi.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lf.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gs.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ry.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://qk.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cp.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://ns.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eb.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://vv.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ir.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://io.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://pv.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://pv.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://qv.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hb.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://jk.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://ql.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://bu.nicolike.cn

[A16] 真假值判断规则
来源：http://sd.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://df.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://em.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vx.szsharing.cn

TS:   if (!x) {}
来源：http://ou.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oj.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://do.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://da.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kp.hnjuh.cn

[A17] 位运算
来源：http://me.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lh.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uf.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fm.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ra.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ug.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qq.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ce.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://jd.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://wg.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://hg.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vp.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ub.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://gf.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wr.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://ec.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://yt.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://pl.bookmarksfly.cn

Py:   a, b = b, a
来源：http://ku.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nu.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ac.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://ki.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://uv.szxytkj.cn

Go:   a, b = b, a
来源：http://dn.panjiajie.cn

Ruby: a, b = b, a
来源：http://jj.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://ml.panjiajie.cn

[A20] 读取标准输入
来源：http://wc.shxzskj.cn

Py:   name = input("请输入：")
来源：http://bj.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zh.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ex.521024.cn

TS:   // Node.js：readline 模块
来源：http://fy.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://ni.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nc.asd995.cn

Ruby: gets.chomp
来源：http://bi.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://vn.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://iu.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://vt.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ri.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://md.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://ik.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://is.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kc.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://te.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://rw.jctech888.com.cn

[A22] 获取字符串长度
来源：http://jd.lnxyls.cn

Py:   len(s)
来源：http://cq.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iq.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ij.colortex.cn

TS:   s.length
来源：http://pu.jianghongdianzi.cn

Java: s.length()
来源：http://hd.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fk.huanxung.cn

Ruby: s.length
来源：http://zk.muxihuayi.cn

C#:   s.Length
来源：http://qv.wgjwhj.cn

[A23] 大小写转换
来源：http://sb.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tu.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://en.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ag.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uc.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xz.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yj.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hb.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eb.szxytkj.cn

[A24] 去除首尾空白
来源：http://ea.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lj.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://or.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kg.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fv.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bl.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://yb.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ll.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xw.asd995.cn

[A25] 字符串比较
来源：http://ln.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://aq.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vy.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ui.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://so.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ct.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kz.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rk.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://in.newstarts.cn

[A26] 类型转换总览
来源：http://vi.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://av.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aq.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gl.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://rh.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://do.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wh.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nt.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ev.haigaiapp.cn

================================================================================
来源：http://sx.colortex.cn

B. 流程控制
来源：http://nt.muxihuayi.cn

================================================================================
来源：http://rb.shxzskj.cn

[B01] 条件判断 if / else
来源：http://sc.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jh.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://co.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bl.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ow.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jx.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mz.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cw.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ji.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xi.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tx.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zj.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pq.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.szsharing.cn

[B03] switch / match / case
来源：http://ez.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bv.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eg.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hh.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yb.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gu.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://et.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gd.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bc.huanxung.cn

[B04] for 计数循环
来源：http://qw.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://iy.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fl.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wu.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rt.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eu.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vp.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://jy.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bk.colortex.cn

[B05] 遍历数组 / 列表
来源：http://fb.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ku.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fc.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vk.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://en.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lv.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kh.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ue.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://hn.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vd.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://io.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://si.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ql.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mh.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://io.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xq.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ro.colortex.cn

[B07] while 循环
来源：http://ep.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://xu.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ja.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://my.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://rg.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ds.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://de.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://un.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://rg.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ng.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://yy.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ox.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://bm.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://tv.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://ej.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://re.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hz.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://nz.jianghongdianzi.cn

[B09] break 与 continue
来源：http://vp.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cz.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wr.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dk.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kj.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wp.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tu.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rb.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ik.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://wh.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sv.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://md.jianghongdianzi.cn


<!-- 参考信息 -->