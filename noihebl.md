代发 wailian999

================================================================================
来源：http://gp.huixiangedu.cn

A. 基础语法与类型
来源：http://vl.shxzukj.cn

================================================================================
来源：http://mf.yuexingan06.cn

[A01] Hello World
来源：http://oc.hahajie.cn

Py:   print("Hello, World!")
来源：http://gw.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://kl.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://xr.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sa.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://ze.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://nu.colortex.cn

Ruby: puts "Hello, World!"
来源：http://ds.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vh.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://hs.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bv.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lo.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cn.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wz.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://tm.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ie.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://lg.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://su.huanxung.cn

[A03] 常量定义
来源：http://ag.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jq.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://cr.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://yn.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://hg.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://fn.9csxet.cn

Go:   const PI = 3.14159
来源：http://dg.shxzskj.cn

Ruby: PI = 3.14159
来源：http://wf.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://mt.huixiangedu.cn

[A04] 判断变量类型
来源：http://yq.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hc.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xy.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://if.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://lx.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nv.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xn.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vl.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://oc.9csxet.cn

[A05] 整数除法与取模
来源：http://ef.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bv.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ya.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cb.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mt.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://in.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://ia.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://dz.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://au.szsharing.cn

[A06] 字符串转数字
来源：http://jy.colortex.cn

Py:   int("42"); float("3.14")
来源：http://da.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cb.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lt.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qx.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tb.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ql.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sh.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sy.hnjuh.cn

[A07] 数字转字符串
来源：http://wj.bjjhwx.cn

Py:   str(42)
来源：http://ij.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://gc.9csxet.cn

JS:   String(42); (42).toString()
来源：http://sv.huanxung.cn

TS:   String(42)
来源：http://uk.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rj.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://aq.haigaiapp.cn

Ruby: 42.to_s
来源：http://lu.jianghongdianzi.cn

C#:   42.ToString()
来源：http://sv.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://xg.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fc.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cw.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oh.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ud.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tp.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cb.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hb.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://re.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://nf.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ye.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zp.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ye.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qi.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jp.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iq.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://za.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kt.yuexingan06.cn

[A10] 生成随机数
来源：http://gn.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://wt.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://fc.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bb.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kh.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://jg.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qj.asd995.cn

Ruby: rand(1..100)
来源：http://eb.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://qw.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://db.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://up.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ii.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hf.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ub.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://pr.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fj.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xf.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ub.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://ch.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ix.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mh.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://tt.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://mi.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://df.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uz.521024.cn

Ruby: "Hello, #{name}!"
来源：http://yu.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://gh.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nm.colortex.cn

Py:   "第一行\n第二行"
来源：http://mc.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://at.521024.cn

JS:   "第一行\n第二行"
来源：http://ce.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://yp.szsharing.cn

Java: "第一行\n第二行"
来源：http://td.9csxet.cn

Go:   "第一行\n第二行"
来源：http://lx.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://uw.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://fz.newstarts.cn

[A14] 注释写法
来源：http://nf.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ec.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oo.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://lu.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://pc.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://md.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://xi.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zp.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://qt.gzmigu.cn

[A15] 空值判断与默认值
来源：http://ih.nicolike.cn

Py:   value = data or "默认值"
来源：http://li.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://mm.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://iz.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://pn.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bk.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://jk.521024.cn

Ruby: value = data || "默认值"
来源：http://dd.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://pc.shxzukj.cn

[A16] 真假值判断规则
来源：http://qt.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kq.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ri.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ji.shxzskj.cn

TS:   if (!x) {}
来源：http://xk.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sl.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ij.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cj.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qu.chemitech.net.cn

[A17] 位运算
来源：http://rs.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cz.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yg.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fy.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pn.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bf.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://qh.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://lu.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://uh.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://di.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ds.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://dt.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vd.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://xi.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://fj.wgjwhj.cn

[A19] 交换两个变量
来源：http://aj.szxytkj.cn

Py:   a, b = b, a
来源：http://ce.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://id.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://pz.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://bw.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://ym.521024.cn

Go:   a, b = b, a
来源：http://wx.szsharing.cn

Ruby: a, b = b, a
来源：http://uz.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://io.huanxung.cn

[A20] 读取标准输入
来源：http://mm.panjiajie.cn

Py:   name = input("请输入：")
来源：http://wm.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aq.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://on.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://ae.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://rf.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://za.chemitech.net.cn

Ruby: gets.chomp
来源：http://mi.colortex.cn

C#:   Console.ReadLine();
来源：http://bq.szsharing.cn

[A21] 保留指定小数位输出
来源：http://ci.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://zh.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cg.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://dw.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://os.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://ip.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tr.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://dn.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://eo.gzmigu.cn

[A22] 获取字符串长度
来源：http://qq.lnxyls.cn

Py:   len(s)
来源：http://bk.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hy.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vj.jctech888.com.cn

TS:   s.length
来源：http://hp.asd995.cn

Java: s.length()
来源：http://mv.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://or.nszjky.cn

Ruby: s.length
来源：http://nw.shxzukj.cn

C#:   s.Length
来源：http://ux.shxzukj.cn

[A23] 大小写转换
来源：http://zy.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tn.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tc.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nh.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lp.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kd.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ro.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ry.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gw.newstarts.cn

[A24] 去除首尾空白
来源：http://lb.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ao.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mv.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ns.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cp.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lr.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://vm.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jg.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wr.lnxyls.cn

[A25] 字符串比较
来源：http://gx.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://zt.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ec.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gv.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cm.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eg.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lq.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://we.huixiangedu.cn

[A26] 类型转换总览
来源：http://wj.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dt.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://za.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xg.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://tx.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dd.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mw.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tz.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bz.szxytkj.cn

================================================================================
来源：http://ib.gzmigu.cn

B. 流程控制
来源：http://rq.521024.cn

================================================================================
来源：http://km.hnjuh.cn

[B01] 条件判断 if / else
来源：http://hg.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fj.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ol.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kz.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qf.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cj.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ny.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wg.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pm.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://oj.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gz.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mi.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nf.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bi.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tc.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pf.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.yuntaijiaju.cn

[B03] switch / match / case
来源：http://ye.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yc.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xq.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eb.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qn.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://is.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bc.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fc.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yu.huixinmuqiang.cn

[B04] for 计数循环
来源：http://zn.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://ca.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://js.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lr.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jb.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rt.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://us.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jv.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://vr.asd995.cn

Py:   for item in arr: print(item)
来源：http://bv.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nf.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nv.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bq.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mu.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xd.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://co.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aq.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://fm.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ct.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xn.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eo.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rf.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wy.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zg.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xc.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ww.huixiangedu.cn

[B07] while 循环
来源：http://eb.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://hv.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ut.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://ms.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://jg.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://hv.szsharing.cn


<!-- 参考信息 -->