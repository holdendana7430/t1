代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://hu.huixinmuqiang.cn

[A03] 常量定义
来源：http://hv.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tr.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://cf.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://io.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://mt.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://yk.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://dl.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://pd.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://zf.nszjky.cn

[A04] 判断变量类型
来源：http://en.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://da.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uj.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vr.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://yp.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://co.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cs.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sq.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://sl.shtwfgs.cn

[A05] 整数除法与取模
来源：http://yp.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xh.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gs.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ud.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fl.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://db.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://iy.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://vx.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ds.9csxet.cn

[A06] 字符串转数字
来源：http://at.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://gy.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ix.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bc.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hj.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uo.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ab.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ib.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yl.huixiangedu.cn

[A07] 数字转字符串
来源：http://bf.panjiajie.cn

Py:   str(42)
来源：http://ip.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://is.colortex.cn

JS:   String(42); (42).toString()
来源：http://td.huixiangedu.cn

TS:   String(42)
来源：http://dv.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xg.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://eq.9csxet.cn

Ruby: 42.to_s
来源：http://lz.szsharing.cn

C#:   42.ToString()
来源：http://dr.colortex.cn

[A08] 取整与四舍五入
来源：http://si.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nh.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mu.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lk.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://le.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://un.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ug.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vf.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wq.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://xi.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cw.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ur.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fh.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ka.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xz.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cz.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ry.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uc.newstarts.cn

[A10] 生成随机数
来源：http://oc.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://by.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://fw.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bl.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zj.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://nt.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ps.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://rp.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://jz.521024.cn

[A11] 条件表达式（三元）
来源：http://te.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://mc.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gx.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ty.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xa.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://eo.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xi.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cc.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hk.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ld.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qe.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://le.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://lq.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://fe.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://hu.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ts.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://ko.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://ys.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wb.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://wf.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://uy.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://nc.newstarts.cn

TS:   "第一行\n第二行"
来源：http://sh.panjiajie.cn

Java: "第一行\n第二行"
来源：http://fm.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://ba.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://rq.hahajie.cn

C#:   "第一行\n第二行"
来源：http://vz.shxzskj.cn

[A14] 注释写法
来源：http://nl.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://of.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://po.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://xr.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://ds.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nj.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://bh.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ad.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://uw.nicolike.cn

[A15] 空值判断与默认值
来源：http://iq.hahajie.cn

Py:   value = data or "默认值"
来源：http://vo.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://lh.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://jn.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://wg.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tk.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://dz.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://lj.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://jt.haigaiapp.cn

[A16] 真假值判断规则
来源：http://zc.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rg.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tr.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wg.nszjky.cn

TS:   if (!x) {}
来源：http://ck.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qw.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gz.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://te.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oh.shxzskj.cn

[A17] 位运算
来源：http://lo.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jw.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ay.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://js.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jj.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lt.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wf.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jn.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://xt.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://pp.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://nu.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xl.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jh.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://bf.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jm.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://sv.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://ez.wgjwhj.cn

[A19] 交换两个变量
来源：http://zh.bjjhwx.cn

Py:   a, b = b, a
来源：http://lb.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xz.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://rh.asd995.cn

TS:   [a, b] = [b, a];
来源：http://nk.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://oh.bjjhwx.cn

Go:   a, b = b, a
来源：http://vf.panjiajie.cn

Ruby: a, b = b, a
来源：http://sx.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://on.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://dg.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://fk.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yc.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qm.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://ak.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ny.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sc.szxytkj.cn

Ruby: gets.chomp
来源：http://zd.colortex.cn

C#:   Console.ReadLine();
来源：http://kj.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://js.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://zl.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sz.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://bo.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://mz.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://bt.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ye.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://cx.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://mj.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://ae.yuntaijiaju.cn

Py:   len(s)
来源：http://sa.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tt.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ll.panjiajie.cn

TS:   s.length
来源：http://fd.muxihuayi.cn

Java: s.length()
来源：http://kh.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qt.huixiangedu.cn

Ruby: s.length
来源：http://gm.yuexingan06.cn

C#:   s.Length
来源：http://ad.jianghongdianzi.cn

[A23] 大小写转换
来源：http://sq.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ho.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xk.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jk.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iz.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zb.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://br.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://it.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tm.shtwfgs.cn

[A24] 去除首尾空白
来源：http://tp.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sg.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hs.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dm.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hk.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sv.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://nx.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yy.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zk.shxzukj.cn

[A25] 字符串比较
来源：http://fr.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://wu.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dj.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ij.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ha.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yc.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lb.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://so.nszjky.cn

[A26] 类型转换总览
来源：http://qp.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ko.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://he.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ea.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://pr.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://on.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qm.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xp.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ne.lnxyls.cn

================================================================================
来源：http://zv.huixiangedu.cn

B. 流程控制
来源：http://pp.bookmarksfly.cn

================================================================================
来源：http://pk.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://lx.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eo.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hr.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pa.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uu.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wi.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hp.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gs.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sb.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ma.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lb.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wr.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://td.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://il.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.521024.cn

[B03] switch / match / case
来源：http://ml.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://az.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gk.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ls.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iw.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fj.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lc.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://el.huixinmuqiang.cn

[B04] for 计数循环
来源：http://lt.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ay.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dn.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hm.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pq.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sf.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mq.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://po.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qu.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://sq.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://kl.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ww.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rm.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://io.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://by.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://td.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://wj.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pj.asd995.cn

[B06] 遍历字典 / 对象
来源：http://zb.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://do.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bw.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rp.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://um.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vn.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pv.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uo.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lv.panjiajie.cn

[B07] while 循环
来源：http://xi.newstarts.cn

Py:   while i < 10: i += 1
来源：http://re.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ah.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://nn.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://va.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://fe.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kf.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://cv.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://ut.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://tt.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://rq.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hj.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://pr.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ot.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://si.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xi.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fd.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://fg.muxihuayi.cn

[B09] break 与 continue
来源：http://ng.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ye.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://is.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xp.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fv.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ol.bjjhwx.cn


<!-- 参考信息 -->