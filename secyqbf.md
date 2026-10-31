代发 wailian999

JS:   const PI = 3.14159;
来源：http://qe.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://wq.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://df.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://kk.asd995.cn

Ruby: PI = 3.14159
来源：http://xc.521024.cn

C#:   const double PI = 3.14159;
来源：http://bg.shtwfgs.cn

[A04] 判断变量类型
来源：http://kb.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sa.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://as.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uq.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://za.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iu.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ef.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ya.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://qe.shxzskj.cn

[A05] 整数除法与取模
来源：http://xx.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qy.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qw.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ge.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://km.521024.cn

Java: 7 / 2; 7 % 2
来源：http://tz.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://tj.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://xm.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://cf.chemitech.net.cn

[A06] 字符串转数字
来源：http://ij.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://zl.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://js.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ii.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qj.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fv.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nc.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kb.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zd.newstarts.cn

[A07] 数字转字符串
来源：http://eo.wgjwhj.cn

Py:   str(42)
来源：http://ux.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://dh.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://cq.yuntaijiaju.cn

TS:   String(42)
来源：http://sf.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hd.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://he.panjiajie.cn

Ruby: 42.to_s
来源：http://ix.nicolike.cn

C#:   42.ToString()
来源：http://zw.hahajie.cn

[A08] 取整与四舍五入
来源：http://vq.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cj.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hr.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zb.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aa.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pe.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nl.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://to.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xd.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://zk.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bu.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://df.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xd.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rn.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://by.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ys.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xj.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bo.521024.cn

[A10] 生成随机数
来源：http://tm.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://sm.9csxet.cn

PHP:  random_int(1, 100);
来源：http://na.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kx.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yu.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://sj.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pk.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://bs.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://go.asd995.cn

[A11] 条件表达式（三元）
来源：http://pd.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ii.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vz.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pn.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cg.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://gz.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yq.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tn.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xh.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://bc.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lk.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pp.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://qd.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://wv.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://je.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qy.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://me.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://xd.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eo.nicolike.cn

Py:   "第一行\n第二行"
来源：http://yy.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://nb.hahajie.cn

JS:   "第一行\n第二行"
来源：http://ha.9csxet.cn

TS:   "第一行\n第二行"
来源：http://hp.panjiajie.cn

Java: "第一行\n第二行"
来源：http://gd.colortex.cn

Go:   "第一行\n第二行"
来源：http://ko.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://oz.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://ch.yuexingan06.cn

[A14] 注释写法
来源：http://lg.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pk.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kp.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://pq.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://po.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ly.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://jy.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xq.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://ez.hahajie.cn

[A15] 空值判断与默认值
来源：http://sn.newstarts.cn

Py:   value = data or "默认值"
来源：http://fx.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://lb.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://fh.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://fw.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ol.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://vf.hahajie.cn

Ruby: value = data || "默认值"
来源：http://rq.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://li.nszjky.cn

[A16] 真假值判断规则
来源：http://si.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wn.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yg.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qx.szxytkj.cn

TS:   if (!x) {}
来源：http://ah.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yu.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://og.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vb.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fp.9csxet.cn

[A17] 位运算
来源：http://wz.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ty.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cf.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wl.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tn.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tz.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qt.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://kh.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://ef.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://fv.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sm.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uq.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://um.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://at.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://ue.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://ky.szsharing.cn

[A19] 交换两个变量
来源：http://vu.colortex.cn

Py:   a, b = b, a
来源：http://ql.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zc.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://vb.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://sn.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://pf.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://vk.nszjky.cn

Ruby: a, b = b, a
来源：http://km.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://ml.muxihuayi.cn

[A20] 读取标准输入
来源：http://to.hahajie.cn

Py:   name = input("请输入：")
来源：http://dw.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yj.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wj.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ck.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://vi.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hm.nicolike.cn

Ruby: gets.chomp
来源：http://ti.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://sk.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://hi.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ti.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wi.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ue.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://xe.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ug.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uj.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://jl.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://ry.shxzskj.cn

[A22] 获取字符串长度
来源：http://ga.huanxung.cn

Py:   len(s)
来源：http://qb.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tn.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ui.newstarts.cn

TS:   s.length
来源：http://zf.shxzukj.cn

Java: s.length()
来源：http://kf.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pd.huixinmuqiang.cn

Ruby: s.length
来源：http://em.huanxung.cn

C#:   s.Length
来源：http://zz.asd995.cn

[A23] 大小写转换
来源：http://gw.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hv.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oe.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vl.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gc.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cb.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jq.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vo.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://fe.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://be.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wn.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bd.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lk.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lp.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://vp.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xa.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hh.yuntaijiaju.cn

[A25] 字符串比较
来源：http://sv.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://pu.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hp.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ct.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ab.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nr.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fc.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://is.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fv.newstarts.cn

[A26] 类型转换总览
来源：http://xj.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pk.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oy.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ed.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://dz.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tc.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cb.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cg.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://it.jctech888.com.cn

================================================================================
来源：http://ev.muxihuayi.cn

B. 流程控制
来源：http://dh.hnjuh.cn

================================================================================
来源：http://ov.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ct.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://px.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kx.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fa.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tm.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bh.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jo.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mm.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ly.hahajie.cn

[B02] 多分支 else if / elif
来源：http://ax.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sr.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://za.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kr.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xy.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dj.huixinmuqiang.cn

[B03] switch / match / case
来源：http://tz.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xe.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pd.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ln.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ng.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fa.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yk.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zk.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dz.nicolike.cn

[B04] for 计数循环
来源：http://sy.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ff.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ut.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rx.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ga.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://in.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yw.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://wa.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sd.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://ww.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://kz.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://so.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ri.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eo.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zr.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dy.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://mn.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jd.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://qg.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fp.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yp.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gp.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ld.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sc.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dc.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xy.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tu.hahajie.cn

[B07] while 循环
来源：http://uh.nszjky.cn

Py:   while i < 10: i += 1
来源：http://vc.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lq.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://gs.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://qp.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://hr.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sd.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://gk.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://gz.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://cn.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ms.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gn.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://ck.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://nc.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ts.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gn.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lw.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://ys.bookmarksfly.cn

[B09] break 与 continue
来源：http://jm.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ki.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xy.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vi.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yt.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ga.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nk.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zl.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ow.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://du.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://td.wgjwhj.cn


<!-- 参考信息 -->