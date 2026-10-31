代发 wailian999

JS:   const PI = 3.14159;
来源：http://lw.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://eb.521024.cn

Java: static final double PI = 3.14159;
来源：http://gr.521024.cn

Go:   const PI = 3.14159
来源：http://ga.huanxung.cn

Ruby: PI = 3.14159
来源：http://ar.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://lo.szsharing.cn

[A04] 判断变量类型
来源：http://qx.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ek.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://by.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lx.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://pv.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ih.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xv.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bn.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://mx.yuexingan06.cn

[A05] 整数除法与取模
来源：http://wd.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lh.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pf.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qv.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sb.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://ol.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://xx.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://hg.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://pk.haigaiapp.cn

[A06] 字符串转数字
来源：http://nv.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://io.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tk.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ia.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://os.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://al.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xb.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://au.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ub.haigaiapp.cn

[A07] 数字转字符串
来源：http://uk.yuntaijiaju.cn

Py:   str(42)
来源：http://eh.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://vf.nszjky.cn

JS:   String(42); (42).toString()
来源：http://yy.szsharing.cn

TS:   String(42)
来源：http://ys.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cu.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://un.nicolike.cn

Ruby: 42.to_s
来源：http://xp.huanxung.cn

C#:   42.ToString()
来源：http://un.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ul.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nj.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hr.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ob.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qo.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ml.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dk.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cf.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ot.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://cs.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tt.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uz.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kg.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qt.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://di.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://td.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zk.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iv.bjjhwx.cn

[A10] 生成随机数
来源：http://gf.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://fe.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://re.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gh.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://sl.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hp.asd995.cn

Ruby: rand(1..100)
来源：http://ct.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://ah.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://bs.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://jl.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vi.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vo.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uf.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://sv.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xi.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ax.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dx.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://yb.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ty.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tm.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://py.colortex.cn

TS:   `Hello, ${name}!`
来源：http://cd.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://he.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ds.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://xq.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://bj.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zc.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://xi.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://vp.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://xy.9csxet.cn

TS:   "第一行\n第二行"
来源：http://ev.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://xr.hahajie.cn

Go:   "第一行\n第二行"
来源：http://fa.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://kd.colortex.cn

C#:   "第一行\n第二行"
来源：http://lt.shxzukj.cn

[A14] 注释写法
来源：http://jd.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oz.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eq.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://sq.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://om.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zo.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://zw.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yx.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://mi.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://hf.9csxet.cn

Py:   value = data or "默认值"
来源：http://og.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://qv.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://wn.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://yc.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mk.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://je.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://hz.521024.cn

C#:   var value = data ?? "默认值";
来源：http://me.nicolike.cn

[A16] 真假值判断规则
来源：http://xt.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kj.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://me.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sv.521024.cn

TS:   if (!x) {}
来源：http://ve.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sb.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://na.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rc.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ra.huixiangedu.cn

[A17] 位运算
来源：http://eo.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ha.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gp.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ck.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rd.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ba.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://se.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://cv.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://oh.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://ji.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bc.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tb.521024.cn

Java: (int) 'A'; (char) 65
来源：http://yu.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dj.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://yx.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://dg.asd995.cn

[A19] 交换两个变量
来源：http://yy.shxzskj.cn

Py:   a, b = b, a
来源：http://oa.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://aw.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://rx.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://dx.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://zd.newstarts.cn

Go:   a, b = b, a
来源：http://jv.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ow.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://in.lnxyls.cn

[A20] 读取标准输入
来源：http://ob.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://rk.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://if.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ao.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://zq.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ic.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ul.szsharing.cn

Ruby: gets.chomp
来源：http://ni.newstarts.cn

C#:   Console.ReadLine();
来源：http://ip.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://du.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://zc.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fh.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://nu.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://nt.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://az.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zl.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://iv.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://rl.shtwfgs.cn

[A22] 获取字符串长度
来源：http://se.nszjky.cn

Py:   len(s)
来源：http://bt.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oo.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kq.shxzukj.cn

TS:   s.length
来源：http://jp.nszjky.cn

Java: s.length()
来源：http://ta.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kc.9csxet.cn

Ruby: s.length
来源：http://bh.asd995.cn

C#:   s.Length
来源：http://jn.wgjwhj.cn

[A23] 大小写转换
来源：http://kt.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ah.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tw.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cr.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://db.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xt.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mh.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vq.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kk.nicolike.cn

[A24] 去除首尾空白
来源：http://rz.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ny.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://te.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wn.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://mw.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fm.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mw.chemitech.net.cn

[A25] 字符串比较
来源：http://ic.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://np.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uu.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://an.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rm.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gt.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gx.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qg.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qo.bjjhwx.cn

[A26] 类型转换总览
来源：http://sn.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kv.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ew.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bs.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://zw.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ze.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rs.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ry.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wc.szxytkj.cn

================================================================================
来源：http://bc.colortex.cn

B. 流程控制
来源：http://gp.yuexingan06.cn

================================================================================
来源：http://kz.szsharing.cn

[B01] 条件判断 if / else
来源：http://ho.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xc.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mb.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bk.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dh.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zu.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vb.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ef.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://md.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mb.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kt.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ng.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wz.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://da.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xv.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.nicolike.cn

[B03] switch / match / case
来源：http://qk.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yc.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://va.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://px.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vt.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fs.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hn.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ad.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ld.yuexingan06.cn

[B04] for 计数循环
来源：http://it.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://iv.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vw.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kd.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fx.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jr.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vt.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ko.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dn.colortex.cn

[B05] 遍历数组 / 列表
来源：http://zy.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://qu.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ci.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ni.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xt.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gs.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gg.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://xw.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bt.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://rm.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yr.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hm.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aa.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fm.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nw.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ai.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pl.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ef.shtwfgs.cn

[B07] while 循环
来源：http://wb.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ye.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xr.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://pg.521024.cn

TS:   while (i < 10) { i++; }
来源：http://zs.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://ro.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oc.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://uu.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://vy.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://mz.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://oc.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uq.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://gv.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://rk.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://hm.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wb.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://si.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://qf.yuntaijiaju.cn

[B09] break 与 continue
来源：http://nm.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zy.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qt.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xk.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://or.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fh.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xp.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cj.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://fb.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://up.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eo.huanxung.cn


<!-- 参考信息 -->