代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hd.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://di.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://yf.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://gb.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ov.colortex.cn

[A03] 常量定义
来源：http://vg.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iq.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://fe.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://gg.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://yc.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://zz.gzmigu.cn

Go:   const PI = 3.14159
来源：http://xi.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://hk.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://ci.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://zi.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wq.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://es.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ui.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://pp.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zg.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hi.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tk.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://fz.muxihuayi.cn

[A05] 整数除法与取模
来源：http://dv.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gv.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://od.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wa.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kp.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://pj.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://rr.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://fo.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://hd.yuexingan06.cn

[A06] 字符串转数字
来源：http://ti.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://qa.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://na.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ks.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qz.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jn.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mb.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fl.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vx.jctech888.com.cn

[A07] 数字转字符串
来源：http://nr.yuexingan06.cn

Py:   str(42)
来源：http://sa.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://rj.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://av.huixinmuqiang.cn

TS:   String(42)
来源：http://nb.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lg.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://on.hahajie.cn

Ruby: 42.to_s
来源：http://xx.szsharing.cn

C#:   42.ToString()
来源：http://jx.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://sk.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hy.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hc.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wi.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ow.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ci.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xc.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sr.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kc.asd995.cn

[A09] 绝对值与最大最小值
来源：http://dy.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bs.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sk.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rk.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ct.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ny.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ad.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bd.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gq.huixinmuqiang.cn

[A10] 生成随机数
来源：http://az.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ja.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://nq.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vj.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vg.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://ye.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dp.panjiajie.cn

Ruby: rand(1..100)
来源：http://le.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://mx.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://nx.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://yl.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ic.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qn.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oy.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://gy.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qg.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xx.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ud.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://qk.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dn.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ce.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://cv.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://uj.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ix.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eu.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://vb.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://mo.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yk.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://lo.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://yx.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://iu.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://zi.szxytkj.cn

Java: "第一行\n第二行"
来源：http://hw.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://rk.521024.cn

Ruby: "第一行\n第二行"
来源：http://ka.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://jj.shxzukj.cn

[A14] 注释写法
来源：http://qg.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bv.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ai.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://jt.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://fn.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://da.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://xc.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ge.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://wx.shxzskj.cn

[A15] 空值判断与默认值
来源：http://kp.newstarts.cn

Py:   value = data or "默认值"
来源：http://an.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://pt.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://bi.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://sg.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://la.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://hc.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://be.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://am.szxytkj.cn

[A16] 真假值判断规则
来源：http://wx.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cj.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pa.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mh.hahajie.cn

TS:   if (!x) {}
来源：http://sf.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cr.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://my.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://el.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vm.colortex.cn

[A17] 位运算
来源：http://bc.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nx.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lz.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pu.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wl.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qu.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ga.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://ff.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ru.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qw.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://hy.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qm.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://jw.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://rn.jctech888.com.cn

[A19] 交换两个变量
来源：http://tv.jctech888.com.cn

Py:   a, b = b, a
来源：http://zt.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://at.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://gk.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://ji.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://tw.shtwfgs.cn

Go:   a, b = b, a
来源：http://fa.nszjky.cn

Ruby: a, b = b, a
来源：http://yp.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://tv.bjjhwx.cn

[A20] 读取标准输入
来源：http://bw.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://sy.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lw.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ek.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://qa.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://wh.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qn.bookmarksfly.cn

Ruby: gets.chomp
来源：http://vj.shxzukj.cn

C#:   Console.ReadLine();
来源：http://ii.huanxung.cn

[A21] 保留指定小数位输出
来源：http://kd.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://cg.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cs.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://jv.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://yx.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://ye.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ek.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://lj.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://vx.gzmigu.cn

[A22] 获取字符串长度
来源：http://qb.hahajie.cn

Py:   len(s)
来源：http://td.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pe.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hb.wgjwhj.cn

TS:   s.length
来源：http://ed.shxzskj.cn

Java: s.length()
来源：http://vs.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ex.colortex.cn

Ruby: s.length
来源：http://pd.huixinmuqiang.cn

C#:   s.Length
来源：http://ug.wgjwhj.cn

[A23] 大小写转换
来源：http://pv.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zs.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ek.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tu.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ui.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xf.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hk.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eo.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bp.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://ac.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://je.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://px.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://il.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kz.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ds.521024.cn

Go:   strings.TrimSpace(s)
来源：http://tf.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sh.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tb.wgjwhj.cn

[A25] 字符串比较
来源：http://wx.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://fa.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qo.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://id.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zx.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wo.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fj.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aa.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ez.shxzskj.cn

[A26] 类型转换总览
来源：http://ri.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yj.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nq.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lq.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://gl.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gr.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sw.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://di.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gt.chemitech.net.cn

================================================================================
来源：http://az.huixinmuqiang.cn

B. 流程控制
来源：http://cc.hahajie.cn

================================================================================
来源：http://nj.521024.cn

[B01] 条件判断 if / else
来源：http://hc.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wd.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ma.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ua.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pg.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gi.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vr.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xv.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cs.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://kw.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sp.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mw.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lf.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sz.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.shxzskj.cn

[B03] switch / match / case
来源：http://rb.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yu.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zn.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wr.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dm.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nn.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ku.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bp.huixinmuqiang.cn

[B04] for 计数循环
来源：http://qs.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://es.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ep.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xs.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jo.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pg.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sn.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://jb.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vo.521024.cn

[B05] 遍历数组 / 列表
来源：http://hx.9csxet.cn

Py:   for item in arr: print(item)
来源：http://dg.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fu.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yt.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eu.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sd.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://as.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://kb.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ts.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://jo.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uo.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://es.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zd.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iw.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ig.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zu.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zi.shxzskj.cn

[B07] while 循环
来源：http://nw.nicolike.cn

Py:   while i < 10: i += 1
来源：http://gx.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iz.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://kz.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://oq.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ry.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xn.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ld.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://ks.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://pl.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://fi.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jg.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ew.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://tf.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://ha.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wq.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ik.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://sq.szsharing.cn

[B09] break 与 continue
来源：http://oa.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zb.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ra.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.szxytkj.cn


<!-- 参考信息 -->