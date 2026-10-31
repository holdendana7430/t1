代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://aq.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://bj.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://uu.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://os.nicolike.cn

[A02] 变量声明与赋值
来源：http://fo.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fg.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ok.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://du.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ii.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://uc.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://we.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://mj.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wt.521024.cn

[A03] 常量定义
来源：http://jp.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pv.521024.cn

PHP:  const PI = 3.14159;
来源：http://gf.521024.cn

JS:   const PI = 3.14159;
来源：http://lq.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ro.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ax.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://ia.shxzskj.cn

Ruby: PI = 3.14159
来源：http://mc.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://qn.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://ba.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://px.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rz.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fh.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ys.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://de.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qs.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yv.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://mu.newstarts.cn

[A05] 整数除法与取模
来源：http://di.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nd.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xn.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rq.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ps.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://uc.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://vi.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://ht.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://kk.haigaiapp.cn

[A06] 字符串转数字
来源：http://sz.521024.cn

Py:   int("42"); float("3.14")
来源：http://ma.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dx.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eg.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fx.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wj.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ne.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qi.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wp.hahajie.cn

[A07] 数字转字符串
来源：http://mc.yuexingan06.cn

Py:   str(42)
来源：http://qw.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://sn.9csxet.cn

JS:   String(42); (42).toString()
来源：http://qt.huanxung.cn

TS:   String(42)
来源：http://qq.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rt.521024.cn

Go:   strconv.Itoa(42)
来源：http://mg.hnjuh.cn

Ruby: 42.to_s
来源：http://xt.huixinmuqiang.cn

C#:   42.ToString()
来源：http://xx.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://po.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ef.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gf.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://et.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ec.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jj.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mf.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sm.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qs.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://yu.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oo.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ol.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ew.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bs.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ej.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ko.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://al.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iu.haigaiapp.cn

[A10] 生成随机数
来源：http://xx.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ma.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://iu.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://je.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gy.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://am.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qp.chemitech.net.cn

Ruby: rand(1..100)
来源：http://it.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://el.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://fd.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://dp.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mo.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pd.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jp.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://kr.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bs.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ho.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iq.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://aa.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vx.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hq.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://ip.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://bx.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ng.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ir.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://uj.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://bh.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://il.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://kk.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://nr.huanxung.cn

JS:   "第一行\n第二行"
来源：http://hc.newstarts.cn

TS:   "第一行\n第二行"
来源：http://jf.nicolike.cn

Java: "第一行\n第二行"
来源：http://rh.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://uq.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://tn.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://km.colortex.cn

[A14] 注释写法
来源：http://bq.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yn.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tw.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://kg.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ai.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gv.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://sk.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vy.521024.cn

C#:   // 单行；/* 多行 */
来源：http://mp.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://ro.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://xh.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://pf.521024.cn

JS:   const value = data ?? "默认值";
来源：http://sf.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://an.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bo.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://xl.asd995.cn

Ruby: value = data || "默认值"
来源：http://vn.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://hf.haigaiapp.cn

[A16] 真假值判断规则
来源：http://oh.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ph.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oi.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yx.521024.cn

TS:   if (!x) {}
来源：http://gf.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xv.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qg.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lh.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yz.hnjuh.cn

[A17] 位运算
来源：http://fo.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gc.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ki.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ea.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pi.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lt.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gx.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bm.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://rs.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://rz.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://al.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rc.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jq.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://jx.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cz.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://as.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://sd.colortex.cn

[A19] 交换两个变量
来源：http://yy.521024.cn

Py:   a, b = b, a
来源：http://ca.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sb.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://te.asd995.cn

TS:   [a, b] = [b, a];
来源：http://cp.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://oe.panjiajie.cn

Go:   a, b = b, a
来源：http://xh.nicolike.cn

Ruby: a, b = b, a
来源：http://vv.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://xu.panjiajie.cn

[A20] 读取标准输入
来源：http://zo.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://md.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ug.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ou.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://ng.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://np.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dd.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://rc.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://uy.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://em.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://cc.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ob.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://yh.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://gi.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://yc.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kl.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://fw.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://nv.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://xw.huanxung.cn

Py:   len(s)
来源：http://lq.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cr.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zo.bookmarksfly.cn

TS:   s.length
来源：http://yb.jianghongdianzi.cn

Java: s.length()
来源：http://nh.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pn.bjjhwx.cn

Ruby: s.length
来源：http://gk.bjjhwx.cn

C#:   s.Length
来源：http://kq.bookmarksfly.cn

[A23] 大小写转换
来源：http://yw.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ds.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zn.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ea.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nx.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vh.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lh.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zc.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uh.wgjwhj.cn

[A24] 去除首尾空白
来源：http://uc.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vp.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sz.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://im.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sz.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rb.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ud.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xl.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yb.hnjuh.cn

[A25] 字符串比较
来源：http://fq.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://ml.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qe.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kv.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ry.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uj.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pu.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nr.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fe.shtwfgs.cn

[A26] 类型转换总览
来源：http://ij.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fy.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://by.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://if.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://el.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gz.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wo.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ls.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://on.szsharing.cn

================================================================================
来源：http://dg.9csxet.cn

B. 流程控制
来源：http://nz.hnjuh.cn

================================================================================
来源：http://eg.nicolike.cn

[B01] 条件判断 if / else
来源：http://ru.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bc.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bk.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ms.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bu.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gi.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zw.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gy.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oi.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://nz.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lc.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tk.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vk.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dg.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uf.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vg.shxzskj.cn

[B03] switch / match / case
来源：http://rg.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kh.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ht.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oe.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wl.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aj.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ty.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ym.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yb.shtwfgs.cn

[B04] for 计数循环
来源：http://ih.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://yk.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ae.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sf.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fg.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pw.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tw.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://gj.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://py.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://hu.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://mh.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vl.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mi.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ej.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lx.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fj.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://zk.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kx.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://zh.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ne.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lk.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jm.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fo.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zz.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jk.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yg.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://is.bookmarksfly.cn

[B07] while 循环
来源：http://fz.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://ab.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wf.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://wy.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://wm.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://pt.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eu.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://dv.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://ei.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://po.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ir.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vn.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://yr.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://eo.szxytkj.cn


<!-- 参考信息 -->