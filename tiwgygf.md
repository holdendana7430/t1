代发 wailian999

[A02] 变量声明与赋值
来源：http://uo.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kw.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://df.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ax.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ex.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://pj.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://ld.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://wr.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://of.hnjuh.cn

[A03] 常量定义
来源：http://pc.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://of.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://pq.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://rq.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://uy.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://nx.521024.cn

Go:   const PI = 3.14159
来源：http://sv.gzmigu.cn

Ruby: PI = 3.14159
来源：http://aw.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://cv.shtwfgs.cn

[A04] 判断变量类型
来源：http://zl.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pd.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lp.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wv.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://pe.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://an.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://db.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://is.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://kc.9csxet.cn

[A05] 整数除法与取模
来源：http://ti.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rm.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bl.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fb.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ue.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://yt.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://ze.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ji.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://my.bjjhwx.cn

[A06] 字符串转数字
来源：http://tr.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://fe.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://it.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vv.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ny.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dh.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gg.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bi.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lo.521024.cn

[A07] 数字转字符串
来源：http://fl.asd995.cn

Py:   str(42)
来源：http://pf.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://vm.521024.cn

JS:   String(42); (42).toString()
来源：http://ah.yuntaijiaju.cn

TS:   String(42)
来源：http://og.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ox.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://op.yuexingan06.cn

Ruby: 42.to_s
来源：http://xc.shxzskj.cn

C#:   42.ToString()
来源：http://th.521024.cn

[A08] 取整与四舍五入
来源：http://rl.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ux.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nx.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dd.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sd.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kl.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nu.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xi.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dy.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://wt.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://py.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fd.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jm.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bn.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ss.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kx.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lh.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jo.shtwfgs.cn

[A10] 生成随机数
来源：http://gg.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://bm.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://vx.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://da.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kg.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://bg.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mc.shtwfgs.cn

Ruby: rand(1..100)
来源：http://it.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://pk.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://re.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://uq.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sb.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://un.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zt.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://rm.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pp.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://am.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lz.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://ej.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cq.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rr.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://yq.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://lr.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ch.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rt.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://sx.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://ua.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eo.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://sx.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://cl.9csxet.cn

JS:   "第一行\n第二行"
来源：http://yi.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://tm.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://wy.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://sh.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://mj.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://ka.9csxet.cn

[A14] 注释写法
来源：http://pf.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sz.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hx.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://gz.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://ph.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xm.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://bh.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qp.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://gi.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://eh.asd995.cn

Py:   value = data or "默认值"
来源：http://hk.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://hp.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://vj.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://cy.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ew.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://sm.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://nw.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://aa.yuexingan06.cn

[A16] 真假值判断规则
来源：http://jy.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lp.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bq.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ly.shxzukj.cn

TS:   if (!x) {}
来源：http://jj.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sd.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cz.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mz.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nf.newstarts.cn

[A17] 位运算
来源：http://px.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://no.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zv.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oa.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bo.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zp.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uw.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://jm.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://lf.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ai.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eg.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ct.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://vz.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mj.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://sc.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://fi.9csxet.cn

[A19] 交换两个变量
来源：http://yx.bookmarksfly.cn

Py:   a, b = b, a
来源：http://ly.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zl.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ae.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://mn.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://rn.nszjky.cn

Go:   a, b = b, a
来源：http://zp.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ux.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://ip.colortex.cn

[A20] 读取标准输入
来源：http://rk.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ho.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ph.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fq.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://mr.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://jo.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ko.muxihuayi.cn

Ruby: gets.chomp
来源：http://sf.colortex.cn

C#:   Console.ReadLine();
来源：http://px.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://yi.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://we.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://po.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://qt.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://yj.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://kh.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ze.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://hj.521024.cn

C#:   3.14159.ToString("F2")
来源：http://it.nicolike.cn

[A22] 获取字符串长度
来源：http://ex.shxzskj.cn

Py:   len(s)
来源：http://gn.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fu.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://us.521024.cn

TS:   s.length
来源：http://uy.muxihuayi.cn

Java: s.length()
来源：http://py.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qx.asd995.cn

Ruby: s.length
来源：http://qh.haigaiapp.cn

C#:   s.Length
来源：http://fg.muxihuayi.cn

[A23] 大小写转换
来源：http://mv.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ep.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yl.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gp.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fe.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qd.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sy.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ht.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ig.9csxet.cn

[A24] 去除首尾空白
来源：http://kq.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tl.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cf.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://du.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ri.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yd.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://ie.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://de.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://av.huixinmuqiang.cn

[A25] 字符串比较
来源：http://in.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://ed.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kn.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ie.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ys.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dl.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vv.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bq.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yb.nicolike.cn

[A26] 类型转换总览
来源：http://cf.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qt.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://on.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vt.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://qo.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wt.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ug.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xn.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vr.hahajie.cn

================================================================================
来源：http://om.jctech888.com.cn

B. 流程控制
来源：http://xn.haigaiapp.cn

================================================================================
来源：http://zo.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://dp.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dj.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vq.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vr.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vz.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fd.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bc.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gk.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tc.szsharing.cn

[B02] 多分支 else if / elif
来源：http://dd.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gq.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cp.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yr.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ov.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vu.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mw.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://go.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://st.szsharing.cn

[B03] switch / match / case
来源：http://ab.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mg.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ef.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cw.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xo.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jx.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zp.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kz.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nt.jianghongdianzi.cn

[B04] for 计数循环
来源：http://jm.asd995.cn

Py:   for i in range(10): print(i)
来源：http://jl.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ce.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jv.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uz.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ag.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://cl.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ob.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://xn.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://yy.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mp.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ng.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://if.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zq.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vo.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://wr.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lo.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://we.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://si.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gk.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rh.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zu.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ne.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nq.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mi.huixinmuqiang.cn

[B07] while 循环
来源：http://az.asd995.cn

Py:   while i < 10: i += 1
来源：http://kr.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lj.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://me.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://fp.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://th.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pm.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://hq.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://uo.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ea.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://oi.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oi.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://yv.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://bi.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://wv.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hp.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bq.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://yh.huanxung.cn


<!-- 参考信息 -->