代发 wailian999

Py:   print("Hello, World!")
来源：http://mc.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://iu.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://am.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zy.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://wn.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://jw.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://is.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ud.colortex.cn

[A02] 变量声明与赋值
来源：http://hc.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ek.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uu.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dv.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lx.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://ld.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://hc.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://sx.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gs.hnjuh.cn

[A03] 常量定义
来源：http://vr.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dg.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://nu.nszjky.cn

JS:   const PI = 3.14159;
来源：http://ru.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://ev.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://du.panjiajie.cn

Go:   const PI = 3.14159
来源：http://ja.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://tl.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://mg.haigaiapp.cn

[A04] 判断变量类型
来源：http://xp.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jx.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uc.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hw.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://zw.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dh.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fs.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vw.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://xk.jctech888.com.cn

[A05] 整数除法与取模
来源：http://vs.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://je.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://js.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vb.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zt.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://es.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://xw.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://am.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://zw.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://ww.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://el.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ky.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sg.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://er.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lc.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gx.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ok.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cw.gzmigu.cn

[A07] 数字转字符串
来源：http://gg.hahajie.cn

Py:   str(42)
来源：http://nc.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ba.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://uz.asd995.cn

TS:   String(42)
来源：http://ao.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://do.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://vd.szsharing.cn

Ruby: 42.to_s
来源：http://od.muxihuayi.cn

C#:   42.ToString()
来源：http://ve.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://su.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jw.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jq.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yn.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ge.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rp.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vy.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kq.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sh.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://xg.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hq.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ag.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ij.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ar.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jn.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yw.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kj.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mf.colortex.cn

[A10] 生成随机数
来源：http://dp.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://lo.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://hl.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cf.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yc.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://bj.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ig.shxzukj.cn

Ruby: rand(1..100)
来源：http://ys.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://el.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://yu.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://to.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pr.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gp.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://by.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://dh.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sh.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qo.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bk.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://jj.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pf.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bd.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://ql.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://lw.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://ke.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bv.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://lm.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://qb.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kw.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://ac.colortex.cn

PHP:  "第一行\n第二行"
来源：http://ox.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://tq.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://dr.shxzukj.cn

Java: "第一行\n第二行"
来源：http://yj.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://rh.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://nj.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://uc.lnxyls.cn

[A14] 注释写法
来源：http://so.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oi.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wv.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://oo.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://ix.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mj.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://ri.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rr.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://rn.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://mh.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://kq.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://jk.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://uu.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://fo.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ci.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://mv.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://hf.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://oe.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://pk.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zj.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ub.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xd.asd995.cn

TS:   if (!x) {}
来源：http://tt.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nz.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gs.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://om.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mp.huanxung.cn

[A17] 位运算
来源：http://tu.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sr.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cp.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yr.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kd.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vh.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gl.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://nr.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://dt.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://rp.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nb.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vu.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://yo.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ac.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://xf.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://pi.9csxet.cn

[A19] 交换两个变量
来源：http://dh.9csxet.cn

Py:   a, b = b, a
来源：http://yd.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wn.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://ud.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://aa.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://cl.lnxyls.cn

Go:   a, b = b, a
来源：http://zl.shxzskj.cn

Ruby: a, b = b, a
来源：http://pv.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://cb.huanxung.cn

[A20] 读取标准输入
来源：http://ee.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://zf.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ff.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rp.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://az.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://qz.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yy.newstarts.cn

Ruby: gets.chomp
来源：http://og.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ca.521024.cn

[A21] 保留指定小数位输出
来源：http://zg.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://fu.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xz.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://bc.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ul.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://wd.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ko.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://aw.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://gp.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://dq.nszjky.cn

Py:   len(s)
来源：http://vr.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yw.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://md.colortex.cn

TS:   s.length
来源：http://cr.yuntaijiaju.cn

Java: s.length()
来源：http://ay.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rn.nszjky.cn

Ruby: s.length
来源：http://uc.bookmarksfly.cn

C#:   s.Length
来源：http://nc.yuexingan06.cn

[A23] 大小写转换
来源：http://nh.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xa.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mj.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nq.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ux.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xk.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xe.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wi.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dj.gzmigu.cn

[A24] 去除首尾空白
来源：http://kh.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://va.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zi.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bb.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uy.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cl.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://ey.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uq.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vw.521024.cn

[A25] 字符串比较
来源：http://dg.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://mj.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fv.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hj.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dx.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wj.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ut.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yi.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zt.szxytkj.cn

[A26] 类型转换总览
来源：http://lv.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ce.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rg.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://or.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://gb.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bn.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ea.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ql.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ck.nszjky.cn

================================================================================
来源：http://zd.asd995.cn

B. 流程控制
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://oc.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://ra.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gp.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xo.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fh.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ds.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://br.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ge.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bw.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fx.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://ua.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mx.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dd.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pp.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tc.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pi.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ii.muxihuayi.cn

[B03] switch / match / case
来源：http://qa.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://el.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lp.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dz.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oi.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ct.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vc.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pd.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tm.wgjwhj.cn

[B04] for 计数循环
来源：http://mw.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://du.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ef.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wn.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ik.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bm.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ki.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://pd.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://un.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://cu.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://qj.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wz.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hs.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mt.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fk.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://if.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://do.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kq.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://jo.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wc.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rf.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pa.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ao.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bp.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vz.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uo.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gc.hnjuh.cn

[B07] while 循环
来源：http://eh.nicolike.cn

Py:   while i < 10: i += 1
来源：http://wt.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://np.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://kg.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://vz.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://zx.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gd.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://mc.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://mi.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ok.huixinmuqiang.cn


<!-- 参考信息 -->