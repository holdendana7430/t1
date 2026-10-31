代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://ht.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://pg.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://cm.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rj.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://ug.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bi.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tf.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pb.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bq.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://fq.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://vy.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://dl.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ba.yuexingan06.cn

[A03] 常量定义
来源：http://qj.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bc.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://ue.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://hc.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://jp.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://ma.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://ny.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://pb.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://zs.shxzukj.cn

[A04] 判断变量类型
来源：http://qn.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://br.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sx.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qf.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://lr.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dn.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iz.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ms.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://kd.nicolike.cn

[A05] 整数除法与取模
来源：http://bd.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qd.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zt.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qq.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qu.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://pd.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://pq.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://wx.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://zj.muxihuayi.cn

[A06] 字符串转数字
来源：http://bh.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://fp.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hf.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wy.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ej.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fz.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ew.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aq.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fs.hahajie.cn

[A07] 数字转字符串
来源：http://lp.shxzskj.cn

Py:   str(42)
来源：http://yf.521024.cn

PHP:  (string) 42; strval(42)
来源：http://nm.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://gs.panjiajie.cn

TS:   String(42)
来源：http://ns.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wn.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://fg.huixiangedu.cn

Ruby: 42.to_s
来源：http://bi.bookmarksfly.cn

C#:   42.ToString()
来源：http://se.szxytkj.cn

[A08] 取整与四舍五入
来源：http://rr.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://od.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ya.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nu.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ob.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cc.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oi.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jf.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yq.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://dn.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gt.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wm.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pu.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sr.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vq.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ou.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mv.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://db.nicolike.cn

[A10] 生成随机数
来源：http://hg.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://kn.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://vp.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rb.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rr.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://dr.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gu.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://qi.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://bb.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://dy.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://tr.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ng.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gj.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://po.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ec.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kg.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://it.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ud.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://ia.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ux.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rp.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ri.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://hc.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://no.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://co.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://ie.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://fy.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tq.nszjky.cn

Py:   "第一行\n第二行"
来源：http://ml.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://hc.nszjky.cn

JS:   "第一行\n第二行"
来源：http://xa.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://zi.huanxung.cn

Java: "第一行\n第二行"
来源：http://dl.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://gt.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://os.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://bb.panjiajie.cn

[A14] 注释写法
来源：http://ig.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yh.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ku.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://ot.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://cz.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://us.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://cm.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ku.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://zf.shxzukj.cn

[A15] 空值判断与默认值
来源：http://yu.szsharing.cn

Py:   value = data or "默认值"
来源：http://ue.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://hg.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://dc.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://gk.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zo.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://sg.colortex.cn

Ruby: value = data || "默认值"
来源：http://ue.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://tv.shtwfgs.cn

[A16] 真假值判断规则
来源：http://nx.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kh.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ux.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jn.bjjhwx.cn

TS:   if (!x) {}
来源：http://dx.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kx.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ot.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ir.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ro.szxytkj.cn

[A17] 位运算
来源：http://fw.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yx.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fk.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qh.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vq.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aa.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lt.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://uq.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://fr.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://fu.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uw.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://mx.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lg.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://fj.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://vb.muxihuayi.cn

[A19] 交换两个变量
来源：http://kl.shtwfgs.cn

Py:   a, b = b, a
来源：http://cz.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ke.asd995.cn

JS:   [a, b] = [b, a];
来源：http://gf.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://qk.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://lc.haigaiapp.cn

Go:   a, b = b, a
来源：http://jd.9csxet.cn

Ruby: a, b = b, a
来源：http://lt.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://kl.9csxet.cn

[A20] 读取标准输入
来源：http://eb.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://vx.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bz.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://io.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://to.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://af.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qx.colortex.cn

Ruby: gets.chomp
来源：http://dj.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://gz.nszjky.cn

[A21] 保留指定小数位输出
来源：http://fu.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://vm.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ed.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://sg.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://yp.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://ss.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tb.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://ps.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://mc.521024.cn

[A22] 获取字符串长度
来源：http://es.newstarts.cn

Py:   len(s)
来源：http://pk.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sq.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pd.szsharing.cn

TS:   s.length
来源：http://js.newstarts.cn

Java: s.length()
来源：http://nj.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gy.jctech888.com.cn

Ruby: s.length
来源：http://xs.szxytkj.cn

C#:   s.Length
来源：http://rt.shxzskj.cn

[A23] 大小写转换
来源：http://sa.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ds.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tc.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qd.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uo.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vh.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ci.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vb.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vy.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://bo.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ra.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wk.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xv.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uv.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ka.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://lx.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kd.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jy.shtwfgs.cn

[A25] 字符串比较
来源：http://lo.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://ur.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aj.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ep.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gn.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jj.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uz.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kl.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dg.bookmarksfly.cn

[A26] 类型转换总览
来源：http://gj.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xr.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fw.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://fp.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kq.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kp.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pf.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://df.huixinmuqiang.cn

================================================================================
来源：http://rt.nszjky.cn

B. 流程控制
来源：http://ly.szxytkj.cn

================================================================================
来源：http://wg.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://uu.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ds.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lp.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mq.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oa.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cu.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sy.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qu.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pm.huanxung.cn

[B02] 多分支 else if / elif
来源：http://bt.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xl.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zi.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sn.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dq.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iy.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.521024.cn

[B03] switch / match / case
来源：http://ph.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ej.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fa.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cc.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ji.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ft.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nq.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gj.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rt.huixinmuqiang.cn

[B04] for 计数循环
来源：http://qv.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://qr.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tz.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dy.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kq.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lg.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://io.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://cw.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bn.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://xo.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://yz.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ix.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xh.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qg.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yu.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hd.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://eu.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cu.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://pt.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jf.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ia.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sw.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qy.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cq.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wr.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ru.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hu.bookmarksfly.cn

[B07] while 循环
来源：http://kt.hahajie.cn

Py:   while i < 10: i += 1
来源：http://po.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mq.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://st.521024.cn

TS:   while (i < 10) { i++; }
来源：http://nl.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ft.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ua.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://pw.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ji.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://tv.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://dx.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gd.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://me.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://xa.szsharing.cn


<!-- 参考信息 -->