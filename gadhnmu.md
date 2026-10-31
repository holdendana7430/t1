代发 wailian999

JS:   const PI = 3.14159;
来源：http://fj.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://uf.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://ch.panjiajie.cn

Go:   const PI = 3.14159
来源：http://hc.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://gz.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://fy.muxihuayi.cn

[A04] 判断变量类型
来源：http://of.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vd.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eo.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pv.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ed.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xt.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://os.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gt.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://xo.asd995.cn

[A05] 整数除法与取模
来源：http://hd.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pf.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wu.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xm.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ht.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://sg.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://dq.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://vq.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://ez.muxihuayi.cn

[A06] 字符串转数字
来源：http://pb.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://ak.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ss.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kg.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fm.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rl.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kp.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://da.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hy.jctech888.com.cn

[A07] 数字转字符串
来源：http://jt.haigaiapp.cn

Py:   str(42)
来源：http://me.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://rv.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://ud.jianghongdianzi.cn

TS:   String(42)
来源：http://et.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tq.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ho.nicolike.cn

Ruby: 42.to_s
来源：http://mj.panjiajie.cn

C#:   42.ToString()
来源：http://ij.hahajie.cn

[A08] 取整与四舍五入
来源：http://ib.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hi.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ux.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pw.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jh.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hk.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xr.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mb.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wc.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://rg.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vx.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hr.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rj.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lm.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wn.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ec.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bi.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dx.newstarts.cn

[A10] 生成随机数
来源：http://ns.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://uw.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://rj.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tk.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wi.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://fr.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wz.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://uj.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://ga.521024.cn

[A11] 条件表达式（三元）
来源：http://kq.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://ir.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lz.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kl.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lr.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://ef.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mm.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nx.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iw.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://bv.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kq.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yy.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://rz.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://tg.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://xy.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yn.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://bh.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://vy.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hx.nicolike.cn

Py:   "第一行\n第二行"
来源：http://mn.colortex.cn

PHP:  "第一行\n第二行"
来源：http://dt.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://re.colortex.cn

TS:   "第一行\n第二行"
来源：http://gj.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ym.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://yj.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://kq.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://co.lnxyls.cn

[A14] 注释写法
来源：http://de.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ed.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qk.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://ba.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://bs.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qu.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://oa.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bn.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://pj.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://uv.huanxung.cn

Py:   value = data or "默认值"
来源：http://tj.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ew.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://po.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://kn.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zm.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://ve.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://fw.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://zn.muxihuayi.cn

[A16] 真假值判断规则
来源：http://wy.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vp.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xo.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fh.haigaiapp.cn

TS:   if (!x) {}
来源：http://vq.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sl.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ly.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ex.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mt.szsharing.cn

[A17] 位运算
来源：http://fc.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iw.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rd.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lc.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vb.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://sz.asd995.cn

Py:   ord("A"); chr(65)
来源：http://eo.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://vp.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gc.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rj.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://eo.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rq.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://im.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://rh.bookmarksfly.cn

[A19] 交换两个变量
来源：http://ln.szxytkj.cn

Py:   a, b = b, a
来源：http://aq.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rl.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://qy.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://ee.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://xq.chemitech.net.cn

Go:   a, b = b, a
来源：http://zf.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://bb.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://au.lnxyls.cn

[A20] 读取标准输入
来源：http://rv.9csxet.cn

Py:   name = input("请输入：")
来源：http://xb.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ok.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qy.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://na.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://rd.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nv.bjjhwx.cn

Ruby: gets.chomp
来源：http://sz.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://pt.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://oe.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://my.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hw.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://vh.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://cu.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://le.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gz.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ss.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ng.yuexingan06.cn

[A22] 获取字符串长度
来源：http://cz.asd995.cn

Py:   len(s)
来源：http://gx.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eq.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zi.nicolike.cn

TS:   s.length
来源：http://aa.huixinmuqiang.cn

Java: s.length()
来源：http://ax.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fy.yuntaijiaju.cn

Ruby: s.length
来源：http://if.jctech888.com.cn

C#:   s.Length
来源：http://kg.huixiangedu.cn

[A23] 大小写转换
来源：http://wy.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eu.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vo.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mt.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kp.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xx.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sr.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vm.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ox.szxytkj.cn

[A24] 去除首尾空白
来源：http://gc.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://im.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gn.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zz.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fh.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yp.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://vs.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wq.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xc.huixiangedu.cn

[A25] 字符串比较
来源：http://zn.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://kb.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zy.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ex.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zr.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jg.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qj.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ez.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rd.shxzskj.cn

[A26] 类型转换总览
来源：http://kp.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kc.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wy.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oa.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://st.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://az.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://au.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qr.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bf.newstarts.cn

================================================================================
来源：http://kp.shtwfgs.cn

B. 流程控制
来源：http://qz.9csxet.cn

================================================================================
来源：http://sp.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ib.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pk.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wz.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://co.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xe.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oq.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ds.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pg.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://bl.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://et.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mn.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ph.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kj.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zh.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pf.colortex.cn

[B03] switch / match / case
来源：http://no.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ja.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ws.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cm.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ry.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dy.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vj.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wl.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mn.huanxung.cn

[B04] for 计数循环
来源：http://nk.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://jg.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bo.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dc.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ov.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sr.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://up.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://gn.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kx.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ea.521024.cn

Py:   for item in arr: print(item)
来源：http://bl.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://to.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ss.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gb.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nc.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zt.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://qh.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ly.asd995.cn

[B06] 遍历字典 / 对象
来源：http://lq.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ip.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fi.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zb.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uw.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://od.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ce.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bv.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ch.shxzskj.cn

[B07] while 循环
来源：http://yw.asd995.cn

Py:   while i < 10: i += 1
来源：http://oc.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vs.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://sx.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://lz.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://sh.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xz.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://nc.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://xh.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://rb.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://ve.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nr.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://rf.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://gu.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://hn.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bm.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zf.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://oq.nicolike.cn

[B09] break 与 continue
来源：http://rc.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aq.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ms.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kk.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vb.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pe.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mz.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://ci.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dv.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hd.shtwfgs.cn


<!-- 参考信息 -->