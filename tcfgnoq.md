代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kq.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://dc.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://qv.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://sh.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://so.asd995.cn

[A03] 常量定义
来源：http://ox.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cf.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://be.nszjky.cn

JS:   const PI = 3.14159;
来源：http://rb.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://id.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://aa.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://bh.colortex.cn

Ruby: PI = 3.14159
来源：http://jg.colortex.cn

C#:   const double PI = 3.14159;
来源：http://gh.hahajie.cn

[A04] 判断变量类型
来源：http://qh.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ah.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ez.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vg.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://yc.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pc.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pv.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ef.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://jf.newstarts.cn

[A05] 整数除法与取模
来源：http://kw.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aw.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wy.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rt.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ww.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://sn.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://pz.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dc.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://zw.muxihuayi.cn

[A06] 字符串转数字
来源：http://vt.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://qr.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eg.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jr.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pa.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wz.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ss.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://le.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nb.colortex.cn

[A07] 数字转字符串
来源：http://gy.asd995.cn

Py:   str(42)
来源：http://ns.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://nx.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://vp.bjjhwx.cn

TS:   String(42)
来源：http://fi.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nz.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://gm.yuexingan06.cn

Ruby: 42.to_s
来源：http://at.nszjky.cn

C#:   42.ToString()
来源：http://fs.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://fm.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ax.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wz.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://am.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gw.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xr.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yf.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dq.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lc.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://rj.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lf.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tf.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qt.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bp.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zi.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ic.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://no.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dz.hahajie.cn

[A10] 生成随机数
来源：http://cz.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ek.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://qu.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cs.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rg.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ns.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aw.nszjky.cn

Ruby: rand(1..100)
来源：http://fq.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://yd.colortex.cn

[A11] 条件表达式（三元）
来源：http://wh.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://qh.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://la.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ac.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yb.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://ez.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dn.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dy.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://it.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://zm.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tt.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ij.colortex.cn

JS:   `Hello, ${name}!`
来源：http://bi.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://tr.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ph.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://mu.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://wt.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kw.nicolike.cn

Py:   "第一行\n第二行"
来源：http://wl.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://tf.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://ir.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://yh.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://fn.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://fh.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://by.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://ri.shtwfgs.cn

[A14] 注释写法
来源：http://cx.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gd.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kv.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://fa.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ag.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mi.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://mc.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zu.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://gh.szsharing.cn

[A15] 空值判断与默认值
来源：http://qu.szxytkj.cn

Py:   value = data or "默认值"
来源：http://tv.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://po.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://id.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://ua.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://is.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://yq.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://hy.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://rv.hnjuh.cn

[A16] 真假值判断规则
来源：http://uq.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qm.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ni.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://as.newstarts.cn

TS:   if (!x) {}
来源：http://ms.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ve.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://um.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mi.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rq.szxytkj.cn

[A17] 位运算
来源：http://id.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kv.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pz.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jh.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qp.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ez.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wl.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qc.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://ig.asd995.cn

Py:   ord("A"); chr(65)
来源：http://vs.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://bk.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ol.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wl.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://do.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ci.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://dv.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://by.yuexingan06.cn

[A19] 交换两个变量
来源：http://ot.nszjky.cn

Py:   a, b = b, a
来源：http://lq.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nq.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://fb.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://wx.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://xb.szsharing.cn

Go:   a, b = b, a
来源：http://fg.newstarts.cn

Ruby: a, b = b, a
来源：http://pg.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ub.newstarts.cn

[A20] 读取标准输入
来源：http://iu.panjiajie.cn

Py:   name = input("请输入：")
来源：http://mc.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qs.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rr.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://vy.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://kw.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aw.colortex.cn

Ruby: gets.chomp
来源：http://vb.hnjuh.cn

C#:   Console.ReadLine();
来源：http://nr.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://rn.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://bo.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ry.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://av.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ca.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://ht.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jk.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mk.521024.cn

C#:   3.14159.ToString("F2")
来源：http://fe.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://xp.nszjky.cn

Py:   len(s)
来源：http://br.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oo.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kr.szxytkj.cn

TS:   s.length
来源：http://wd.yuexingan06.cn

Java: s.length()
来源：http://qo.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jz.huixiangedu.cn

Ruby: s.length
来源：http://jx.bookmarksfly.cn

C#:   s.Length
来源：http://bo.nicolike.cn

[A23] 大小写转换
来源：http://dq.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qv.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mf.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yx.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jg.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fh.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://as.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gw.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cs.bjjhwx.cn

[A24] 去除首尾空白
来源：http://tr.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qq.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sy.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zt.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xv.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qd.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://pj.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oi.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ub.wgjwhj.cn

[A25] 字符串比较
来源：http://by.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://dz.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hv.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ct.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ml.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gz.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uk.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://id.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ds.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://vu.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://my.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jw.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nr.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://kh.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://it.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pv.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ns.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://df.newstarts.cn

================================================================================
来源：http://ts.asd995.cn

B. 流程控制
来源：http://we.colortex.cn

================================================================================
来源：http://jm.521024.cn

[B01] 条件判断 if / else
来源：http://di.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xy.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fw.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://em.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ou.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rm.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pj.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sa.szsharing.cn

[B02] 多分支 else if / elif
来源：http://nx.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zz.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oh.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ue.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wg.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.jianghongdianzi.cn

[B03] switch / match / case
来源：http://yu.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qq.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nc.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yk.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vo.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uo.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hw.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zj.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zb.szsharing.cn

[B04] for 计数循环
来源：http://zf.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://lx.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mb.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hv.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://po.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ic.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://du.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://mv.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://so.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ph.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://bb.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bo.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yg.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://po.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ox.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rp.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://ik.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lw.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://nq.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nk.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qm.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lz.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yc.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mw.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zb.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sc.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fv.521024.cn

[B07] while 循环
来源：http://jk.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://nk.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ul.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://tj.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://oe.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://qu.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lm.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://me.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://mn.asd995.cn

[B08] do-while（至少执行一次）
来源：http://lz.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://hd.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pe.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://zs.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://mm.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://hr.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cw.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jd.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://vs.shtwfgs.cn

[B09] break 与 continue
来源：http://wx.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jy.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pf.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mx.huanxung.cn


<!-- 参考信息 -->