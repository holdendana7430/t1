代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sp.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://sr.521024.cn

Go:   name := "Alex"; age := 20
来源：http://te.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://it.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tp.huanxung.cn

[A03] 常量定义
来源：http://rf.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://br.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://ho.asd995.cn

JS:   const PI = 3.14159;
来源：http://ry.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://xw.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://qi.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://xh.hahajie.cn

Ruby: PI = 3.14159
来源：http://dn.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://qn.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://wz.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://md.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fj.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://im.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://jq.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sb.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sm.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oy.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://ur.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://qz.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sf.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ip.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sp.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://my.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://hu.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://vm.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://ar.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://rf.muxihuayi.cn

[A06] 字符串转数字
来源：http://dd.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://sr.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bu.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fh.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fh.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xb.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ts.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://af.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jt.szsharing.cn

[A07] 数字转字符串
来源：http://mr.yuexingan06.cn

Py:   str(42)
来源：http://pf.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://bi.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://nk.haigaiapp.cn

TS:   String(42)
来源：http://xc.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vz.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://dv.huixiangedu.cn

Ruby: 42.to_s
来源：http://sl.panjiajie.cn

C#:   42.ToString()
来源：http://ef.shxzskj.cn

[A08] 取整与四舍五入
来源：http://gg.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ji.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://md.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qu.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bj.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wr.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nh.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ax.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vx.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://ob.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://na.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cu.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://an.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jx.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://id.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qn.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rt.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sf.521024.cn

[A10] 生成随机数
来源：http://qo.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://hk.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://xl.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uy.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lt.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ro.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mw.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://lv.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://rk.nszjky.cn

[A11] 条件表达式（三元）
来源：http://xr.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ag.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zv.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pq.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sv.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://tk.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vv.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zm.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ws.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://yp.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ug.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vk.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://ju.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://xw.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://cl.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tk.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://jf.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://la.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jv.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://qk.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://uv.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://yv.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://jf.colortex.cn

Java: "第一行\n第二行"
来源：http://mb.521024.cn

Go:   "第一行\n第二行"
来源：http://ua.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://sm.asd995.cn

C#:   "第一行\n第二行"
来源：http://fl.muxihuayi.cn

[A14] 注释写法
来源：http://gc.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vc.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nh.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://xe.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://mr.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qy.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://ra.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://as.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://af.colortex.cn

[A15] 空值判断与默认值
来源：http://xx.shxzskj.cn

Py:   value = data or "默认值"
来源：http://fy.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://js.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://fa.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://ay.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://he.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://tv.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://ph.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://tj.hahajie.cn

[A16] 真假值判断规则
来源：http://uw.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ys.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xo.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kv.gzmigu.cn

TS:   if (!x) {}
来源：http://sz.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fz.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ou.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xv.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mm.haigaiapp.cn

[A17] 位运算
来源：http://sa.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yb.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tq.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ko.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nr.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sl.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iu.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://bi.colortex.cn

Py:   ord("A"); chr(65)
来源：http://vz.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://yo.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ka.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ym.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://lw.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pt.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://bq.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://ja.szxytkj.cn

[A19] 交换两个变量
来源：http://vr.yuexingan06.cn

Py:   a, b = b, a
来源：http://ep.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://br.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://kj.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://fy.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://vw.asd995.cn

Go:   a, b = b, a
来源：http://wv.9csxet.cn

Ruby: a, b = b, a
来源：http://xa.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://ke.haigaiapp.cn

[A20] 读取标准输入
来源：http://en.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://pd.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xv.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pf.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://dj.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://vk.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vs.bjjhwx.cn

Ruby: gets.chomp
来源：http://hx.newstarts.cn

C#:   Console.ReadLine();
来源：http://cb.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://ra.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://eo.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ra.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://gp.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://wo.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://gr.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uj.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://bq.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://op.newstarts.cn

[A22] 获取字符串长度
来源：http://tv.nicolike.cn

Py:   len(s)
来源：http://jb.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ye.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ma.hnjuh.cn

TS:   s.length
来源：http://vf.szxytkj.cn

Java: s.length()
来源：http://zq.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ku.colortex.cn

Ruby: s.length
来源：http://qk.huixinmuqiang.cn

C#:   s.Length
来源：http://pb.huanxung.cn

[A23] 大小写转换
来源：http://iy.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ub.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://od.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hc.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lf.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ef.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ak.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ix.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tw.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://nl.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qr.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xt.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://te.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oq.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ua.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://wf.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lo.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cr.nszjky.cn

[A25] 字符串比较
来源：http://cm.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://pw.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hg.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sn.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ox.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dl.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fq.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wp.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ot.colortex.cn

[A26] 类型转换总览
来源：http://fm.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kr.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dr.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://cs.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aj.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pv.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://sq.nicolike.cn

B. 流程控制
来源：http://uw.szxytkj.cn

================================================================================
来源：http://bv.asd995.cn

[B01] 条件判断 if / else
来源：http://vb.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fr.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bc.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uy.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tg.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mk.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lr.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vl.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://if.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://fl.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ag.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mr.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bi.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gh.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rx.nszjky.cn

[B03] switch / match / case
来源：http://up.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://un.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://of.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ze.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ql.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bx.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oc.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://us.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ok.9csxet.cn

[B04] for 计数循环
来源：http://xw.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://uz.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qi.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dh.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rz.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nv.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://br.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xp.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://rr.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://et.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tp.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fp.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nl.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xi.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cj.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://bd.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://co.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://lc.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oe.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bg.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qv.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cn.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ot.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://id.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lh.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xm.lnxyls.cn

[B07] while 循环
来源：http://pu.521024.cn

Py:   while i < 10: i += 1
来源：http://wt.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pl.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://fq.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://qy.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://py.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qy.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://wo.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://dy.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://lu.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://mj.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ge.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://ad.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ei.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://fo.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wg.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ty.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://oi.szxytkj.cn

[B09] break 与 continue
来源：http://xk.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yr.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.jianghongdianzi.cn


<!-- 参考信息 -->