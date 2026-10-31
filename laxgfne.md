代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://js.nszjky.cn

[A03] 常量定义
来源：http://mn.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dc.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://nr.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://ze.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://sm.asd995.cn

Java: static final double PI = 3.14159;
来源：http://xd.nicolike.cn

Go:   const PI = 3.14159
来源：http://tz.szsharing.cn

Ruby: PI = 3.14159
来源：http://ld.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://he.lnxyls.cn

[A04] 判断变量类型
来源：http://rc.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://db.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://el.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dy.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://mo.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zn.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fg.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rb.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://lv.wgjwhj.cn

[A05] 整数除法与取模
来源：http://uy.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ue.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://aj.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bx.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ct.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://xk.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://qb.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://mv.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://mw.hahajie.cn

[A06] 字符串转数字
来源：http://nv.521024.cn

Py:   int("42"); float("3.14")
来源：http://wr.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cd.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bk.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lg.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ie.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aj.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uo.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://du.hnjuh.cn

[A07] 数字转字符串
来源：http://zp.huixiangedu.cn

Py:   str(42)
来源：http://my.521024.cn

PHP:  (string) 42; strval(42)
来源：http://fk.521024.cn

JS:   String(42); (42).toString()
来源：http://gl.shxzukj.cn

TS:   String(42)
来源：http://en.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nd.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://oy.jctech888.com.cn

Ruby: 42.to_s
来源：http://wc.yuntaijiaju.cn

C#:   42.ToString()
来源：http://qc.huanxung.cn

[A08] 取整与四舍五入
来源：http://yy.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wg.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uy.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qk.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pp.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lx.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dm.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pg.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hc.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://ky.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eb.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zq.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lx.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ij.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yy.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jl.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yj.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ql.huixiangedu.cn

[A10] 生成随机数
来源：http://op.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://zj.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://hl.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fj.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dk.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://fi.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wj.szxytkj.cn

Ruby: rand(1..100)
来源：http://zm.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://qr.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://ec.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ch.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://co.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ky.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dd.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://mb.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://np.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mv.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hv.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://zs.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tv.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nw.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://cn.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://vj.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://sj.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://is.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://hn.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://sc.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rv.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://mp.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://ew.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://ai.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://pd.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://yd.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://ka.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://lc.colortex.cn

C#:   "第一行\n第二行"
来源：http://vh.9csxet.cn

[A14] 注释写法
来源：http://lr.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gc.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wz.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://vd.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://yn.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fp.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://ul.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uo.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://dk.nicolike.cn

[A15] 空值判断与默认值
来源：http://fv.521024.cn

Py:   value = data or "默认值"
来源：http://rc.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://ci.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://zx.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://uq.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lh.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://xx.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://de.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://fn.muxihuayi.cn

[A16] 真假值判断规则
来源：http://wl.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wp.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fj.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ud.bjjhwx.cn

TS:   if (!x) {}
来源：http://dm.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ii.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://li.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sf.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cc.szxytkj.cn

[A17] 位运算
来源：http://hy.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ls.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://az.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ra.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://is.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vs.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lk.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://un.asd995.cn

Py:   ord("A"); chr(65)
来源：http://jk.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://kc.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bs.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kb.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://xv.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rd.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://tw.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://ol.521024.cn

[A19] 交换两个变量
来源：http://xg.haigaiapp.cn

Py:   a, b = b, a
来源：http://ei.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fe.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://gz.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://ks.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://vy.nicolike.cn

Go:   a, b = b, a
来源：http://qu.shxzskj.cn

Ruby: a, b = b, a
来源：http://as.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://nh.muxihuayi.cn

[A20] 读取标准输入
来源：http://ef.lnxyls.cn

Py:   name = input("请输入：")
来源：http://kg.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kt.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wc.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://qo.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://qm.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dj.panjiajie.cn

Ruby: gets.chomp
来源：http://cb.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://yw.9csxet.cn

[A21] 保留指定小数位输出
来源：http://kq.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://xm.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ko.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://uk.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://rw.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://zh.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sn.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://zh.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://br.asd995.cn

[A22] 获取字符串长度
来源：http://xb.huixinmuqiang.cn

Py:   len(s)
来源：http://ij.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://in.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zi.gzmigu.cn

TS:   s.length
来源：http://qx.bjjhwx.cn

Java: s.length()
来源：http://qm.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ug.newstarts.cn

Ruby: s.length
来源：http://tb.shtwfgs.cn

C#:   s.Length
来源：http://gb.muxihuayi.cn

[A23] 大小写转换
来源：http://tu.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eb.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rq.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bm.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yx.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://py.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yy.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pm.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jq.shtwfgs.cn

[A24] 去除首尾空白
来源：http://nz.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jk.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fp.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://df.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zg.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jx.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://dj.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nm.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wp.bjjhwx.cn

[A25] 字符串比较
来源：http://ge.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://vu.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ku.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fj.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://px.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ui.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qx.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ch.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hs.hnjuh.cn

[A26] 类型转换总览
来源：http://xr.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xk.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vn.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rr.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://ay.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wh.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qa.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hc.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uo.szxytkj.cn

================================================================================
来源：http://kq.muxihuayi.cn

B. 流程控制
来源：http://fy.shtwfgs.cn

================================================================================
来源：http://hc.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://pf.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://es.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://au.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pj.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://we.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bo.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ue.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sf.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://uy.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fv.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xe.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ag.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fk.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sx.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.9csxet.cn

[B03] switch / match / case
来源：http://mo.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hd.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://of.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xe.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://td.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wv.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vw.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://si.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aa.shtwfgs.cn

[B04] for 计数循环
来源：http://bh.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://qb.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fh.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rf.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://me.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nl.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fp.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://lk.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pu.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://jl.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://zc.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wq.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lt.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dp.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ep.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vg.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://bk.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://av.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://mo.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sj.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vi.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cd.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lo.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ir.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vk.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rx.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dh.jctech888.com.cn

[B07] while 循环
来源：http://mi.521024.cn

Py:   while i < 10: i += 1
来源：http://zw.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xz.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://sh.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ya.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://uv.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jh.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://vm.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://yt.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://gx.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://qu.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zs.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://fm.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://ea.521024.cn

Java: do { i++; } while (i < 10);
来源：http://wy.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://df.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lz.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://nk.yuntaijiaju.cn

[B09] break 与 continue
来源：http://eu.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zk.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zy.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kh.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ef.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ao.szxytkj.cn


<!-- 参考信息 -->