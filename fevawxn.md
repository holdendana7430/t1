代发 wailian999

[A02] 变量声明与赋值
来源：http://ey.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nk.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gx.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hs.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rb.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ss.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://ux.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://uv.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eb.panjiajie.cn

[A03] 常量定义
来源：http://qp.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sr.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://il.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://sm.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://kl.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://aj.9csxet.cn

Go:   const PI = 3.14159
来源：http://zu.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://sa.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://vu.szsharing.cn

[A04] 判断变量类型
来源：http://jj.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nb.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dq.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cb.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://jn.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zs.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ms.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vs.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://rz.newstarts.cn

[A05] 整数除法与取模
来源：http://xm.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pz.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jj.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zq.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://py.521024.cn

Java: 7 / 2; 7 % 2
来源：http://tn.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://nz.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ru.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://xh.colortex.cn

[A06] 字符串转数字
来源：http://hn.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://xc.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mc.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xc.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mm.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yh.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://di.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lm.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cc.gzmigu.cn

[A07] 数字转字符串
来源：http://nd.huixiangedu.cn

Py:   str(42)
来源：http://qq.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ug.hahajie.cn

JS:   String(42); (42).toString()
来源：http://we.haigaiapp.cn

TS:   String(42)
来源：http://lw.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ga.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://qd.asd995.cn

Ruby: 42.to_s
来源：http://xl.9csxet.cn

C#:   42.ToString()
来源：http://xq.huanxung.cn

[A08] 取整与四舍五入
来源：http://zo.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zd.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zo.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://do.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ad.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://du.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ag.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hf.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://id.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://dx.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ik.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jv.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bu.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wg.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rl.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ze.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sw.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ay.nicolike.cn

[A10] 生成随机数
来源：http://mg.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://qy.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://qb.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yj.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xk.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://np.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ji.shxzskj.cn

Ruby: rand(1..100)
来源：http://gp.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://uz.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://lv.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://dy.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vf.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nb.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ha.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://vl.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gt.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hh.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hh.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://jn.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://te.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ih.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://pm.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ds.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://dq.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://as.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://hz.colortex.cn

C#:   $"Hello, {name}!"
来源：http://me.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lk.9csxet.cn

Py:   "第一行\n第二行"
来源：http://su.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://yx.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://ko.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://gc.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://os.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://eb.asd995.cn

Ruby: "第一行\n第二行"
来源：http://qj.colortex.cn

C#:   "第一行\n第二行"
来源：http://tj.haigaiapp.cn

[A14] 注释写法
来源：http://mu.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jj.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yh.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://fz.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://hq.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gp.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://jj.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mb.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://pv.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://hn.colortex.cn

Py:   value = data or "默认值"
来源：http://fw.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://rz.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://vh.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://xj.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://or.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ud.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://wz.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://ls.haigaiapp.cn

[A16] 真假值判断规则
来源：http://op.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://es.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://go.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bs.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://nl.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lq.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ec.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vc.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://is.shxzskj.cn

[A17] 位运算
来源：http://wq.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uw.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vn.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rj.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bs.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wc.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ru.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://gz.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://fa.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://me.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cd.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oq.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://kx.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ow.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://vc.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://fc.wgjwhj.cn

[A19] 交换两个变量
来源：http://ej.521024.cn

Py:   a, b = b, a
来源：http://ea.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mc.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://fu.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://fr.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://wx.shtwfgs.cn

Go:   a, b = b, a
来源：http://cw.gzmigu.cn

Ruby: a, b = b, a
来源：http://fa.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://kr.gzmigu.cn

[A20] 读取标准输入
来源：http://nq.gzmigu.cn

Py:   name = input("请输入：")
来源：http://wr.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rb.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vo.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://zx.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://ot.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ut.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://xb.9csxet.cn

C#:   Console.ReadLine();
来源：http://bh.huanxung.cn

[A21] 保留指定小数位输出
来源：http://mc.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://xg.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dx.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://cs.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://bn.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://yd.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pv.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://sy.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://ol.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://vr.shtwfgs.cn

Py:   len(s)
来源：http://pl.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qv.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jf.jctech888.com.cn

TS:   s.length
来源：http://qc.nszjky.cn

Java: s.length()
来源：http://lv.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ra.jianghongdianzi.cn

Ruby: s.length
来源：http://mn.nicolike.cn

C#:   s.Length
来源：http://mi.wgjwhj.cn

[A23] 大小写转换
来源：http://ut.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tg.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mr.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gm.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nm.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wp.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zd.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xq.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xr.colortex.cn

[A24] 去除首尾空白
来源：http://oi.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pc.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ma.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://je.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bp.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vz.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://jc.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uu.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ak.lnxyls.cn

[A25] 字符串比较
来源：http://ld.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://yh.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zw.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fd.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nq.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ev.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vs.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yb.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mg.hnjuh.cn

[A26] 类型转换总览
来源：http://rx.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mg.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pw.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nl.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://xf.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gz.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hq.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ou.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ms.huixiangedu.cn

================================================================================
来源：http://xj.bookmarksfly.cn

B. 流程控制
来源：http://yi.shtwfgs.cn

================================================================================
来源：http://xx.hnjuh.cn

[B01] 条件判断 if / else
来源：http://cz.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://he.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://he.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wv.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pc.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://um.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://st.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hh.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://pv.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sq.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oe.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yn.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hb.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vd.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mt.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ie.yuntaijiaju.cn

[B03] switch / match / case
来源：http://pr.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tq.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tl.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cv.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ek.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qo.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mw.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ha.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vz.shxzukj.cn

[B04] for 计数循环
来源：http://cu.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://nc.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ub.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pq.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jd.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gs.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vw.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://jh.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lc.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://pa.nszjky.cn

Py:   for item in arr: print(item)
来源：http://bn.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ix.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fe.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vk.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pj.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://va.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://yu.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pf.colortex.cn

[B06] 遍历字典 / 对象
来源：http://bl.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hj.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cy.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iw.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ln.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wu.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vl.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xs.huixiangedu.cn

[B07] while 循环
来源：http://zb.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://pw.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://au.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://nv.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://ph.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://cf.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cw.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://kp.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://if.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://ls.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ez.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qk.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://aq.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://sl.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ab.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gn.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ry.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://zq.jianghongdianzi.cn


<!-- 参考信息 -->