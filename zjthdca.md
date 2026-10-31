代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://tr.huixinmuqiang.cn

[A03] 常量定义
来源：http://vl.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kl.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://co.colortex.cn

JS:   const PI = 3.14159;
来源：http://hg.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://iu.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://mr.newstarts.cn

Go:   const PI = 3.14159
来源：http://ub.9csxet.cn

Ruby: PI = 3.14159
来源：http://yr.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://kq.bjjhwx.cn

[A04] 判断变量类型
来源：http://gr.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ep.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kq.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xt.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://ln.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ju.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vp.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ew.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://tn.nszjky.cn

[A05] 整数除法与取模
来源：http://qt.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lp.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://es.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hd.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://im.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://rc.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://gm.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://rf.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://pt.shxzskj.cn

[A06] 字符串转数字
来源：http://ig.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://iu.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rp.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qa.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wv.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vs.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kn.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yk.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gk.9csxet.cn

[A07] 数字转字符串
来源：http://xw.gzmigu.cn

Py:   str(42)
来源：http://bv.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://uw.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://qj.szsharing.cn

TS:   String(42)
来源：http://et.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ol.asd995.cn

Go:   strconv.Itoa(42)
来源：http://un.chemitech.net.cn

Ruby: 42.to_s
来源：http://kx.huanxung.cn

C#:   42.ToString()
来源：http://hr.9csxet.cn

[A08] 取整与四舍五入
来源：http://gs.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ic.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pp.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hv.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rm.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://um.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tj.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xb.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yx.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://ii.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ig.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://au.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uk.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xl.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fb.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eq.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vf.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ov.gzmigu.cn

[A10] 生成随机数
来源：http://sx.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://kj.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://os.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rz.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rd.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://nc.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://in.9csxet.cn

Ruby: rand(1..100)
来源：http://ea.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://ke.asd995.cn

[A11] 条件表达式（三元）
来源：http://yw.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://pk.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tn.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://op.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jh.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ia.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vn.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jz.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://it.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://be.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://km.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qr.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://we.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://xc.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://bg.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ea.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://gt.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://lr.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yi.521024.cn

Py:   "第一行\n第二行"
来源：http://um.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://ir.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://zb.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://mk.szsharing.cn

Java: "第一行\n第二行"
来源：http://nr.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://ra.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://rq.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://gf.shxzskj.cn

[A14] 注释写法
来源：http://jz.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ua.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fm.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ol.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://ko.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://op.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://tb.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qu.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://uu.521024.cn

[A15] 空值判断与默认值
来源：http://yy.shxzskj.cn

Py:   value = data or "默认值"
来源：http://jg.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://mi.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://yh.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://ob.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://my.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://ca.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://iy.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://fk.newstarts.cn

[A16] 真假值判断规则
来源：http://os.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xi.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yn.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ib.shxzskj.cn

TS:   if (!x) {}
来源：http://wl.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ew.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://za.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ln.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xo.jianghongdianzi.cn

[A17] 位运算
来源：http://pn.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yb.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gi.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ni.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ci.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lj.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gq.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xy.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://qt.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://vu.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://rk.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kj.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://qq.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ga.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://lx.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ec.bookmarksfly.cn

[A19] 交换两个变量
来源：http://uw.hahajie.cn

Py:   a, b = b, a
来源：http://cp.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rb.colortex.cn

JS:   [a, b] = [b, a];
来源：http://cx.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://of.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://qx.gzmigu.cn

Go:   a, b = b, a
来源：http://xj.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://yj.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://eg.yuexingan06.cn

[A20] 读取标准输入
来源：http://km.colortex.cn

Py:   name = input("请输入：")
来源：http://om.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ba.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://my.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://ku.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://ku.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hs.shxzskj.cn

Ruby: gets.chomp
来源：http://ps.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://zz.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://at.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://jv.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wr.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ip.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://we.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://nn.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fx.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://mu.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://oh.newstarts.cn

[A22] 获取字符串长度
来源：http://gt.jctech888.com.cn

Py:   len(s)
来源：http://hh.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zf.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sk.colortex.cn

TS:   s.length
来源：http://ax.yuexingan06.cn

Java: s.length()
来源：http://cl.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jl.haigaiapp.cn

Ruby: s.length
来源：http://fa.colortex.cn

C#:   s.Length
来源：http://eg.muxihuayi.cn

[A23] 大小写转换
来源：http://ab.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ae.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pd.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://of.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rt.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wi.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ej.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ws.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zw.shxzskj.cn

[A24] 去除首尾空白
来源：http://do.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oc.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gv.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bm.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ue.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bj.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://ob.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zb.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://um.huixinmuqiang.cn

[A25] 字符串比较
来源：http://zt.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://rp.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mz.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://am.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hm.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bd.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ut.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aw.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hi.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://kr.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oo.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ah.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qq.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://gj.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://if.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gs.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://db.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ti.bookmarksfly.cn

================================================================================
来源：http://zw.wgjwhj.cn

B. 流程控制
来源：http://dh.hahajie.cn

================================================================================
来源：http://dd.nszjky.cn

[B01] 条件判断 if / else
来源：http://bj.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qb.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vq.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wd.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xw.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://np.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dc.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lh.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://jv.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oh.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cq.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hb.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yj.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gm.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yg.chemitech.net.cn

[B03] switch / match / case
来源：http://gg.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uu.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sc.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jj.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yh.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uf.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xz.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lk.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ik.haigaiapp.cn

[B04] for 计数循环
来源：http://at.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://yf.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zl.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jg.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ik.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://af.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gv.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://lz.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://st.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://sk.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://lb.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jw.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fz.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gn.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wl.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pg.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://bu.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vz.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ec.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ca.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nj.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jb.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://os.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rn.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mp.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rh.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fp.bookmarksfly.cn

[B07] while 循环
来源：http://wf.521024.cn

Py:   while i < 10: i += 1
来源：http://fu.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yv.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://tx.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://qc.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://gp.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wd.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://nd.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://jg.asd995.cn

[B08] do-while（至少执行一次）
来源：http://qi.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://an.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tv.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://nm.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://bv.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://wf.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://la.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://py.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://qv.bookmarksfly.cn

[B09] break 与 continue
来源：http://yl.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ry.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jw.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wx.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ye.huixinmuqiang.cn


<!-- 参考信息 -->