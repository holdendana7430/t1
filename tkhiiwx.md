代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zt.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://tr.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://yv.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://ty.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ab.hahajie.cn

[A03] 常量定义
来源：http://hx.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rs.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://uf.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://wc.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://vj.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://lv.shxzukj.cn

Go:   const PI = 3.14159
来源：http://bv.gzmigu.cn

Ruby: PI = 3.14159
来源：http://ow.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://lt.colortex.cn

[A04] 判断变量类型
来源：http://hh.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pw.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jn.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yn.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://kg.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ru.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wh.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fn.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://rn.panjiajie.cn

[A05] 整数除法与取模
来源：http://if.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://si.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mu.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qh.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ah.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://ap.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://zw.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://ty.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://dt.shxzukj.cn

[A06] 字符串转数字
来源：http://bb.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://bm.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ia.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jm.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xm.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ib.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lr.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dk.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bj.hahajie.cn

[A07] 数字转字符串
来源：http://pf.szxytkj.cn

Py:   str(42)
来源：http://qn.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://dj.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://qr.yuntaijiaju.cn

TS:   String(42)
来源：http://yy.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gw.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://gr.shxzskj.cn

Ruby: 42.to_s
来源：http://gi.shxzskj.cn

C#:   42.ToString()
来源：http://sc.521024.cn

[A08] 取整与四舍五入
来源：http://yu.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sj.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ku.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fg.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sm.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://si.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kp.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://se.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bl.asd995.cn

[A09] 绝对值与最大最小值
来源：http://td.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://md.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xd.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kv.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qk.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ap.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cf.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wx.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tc.panjiajie.cn

[A10] 生成随机数
来源：http://gr.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://cl.colortex.cn

PHP:  random_int(1, 100);
来源：http://qd.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ob.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://hd.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bv.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://df.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://gd.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://es.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://gy.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ky.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pj.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ve.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://op.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lk.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nv.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mw.521024.cn

[A12] 字符串插值 / 格式化
来源：http://qx.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uh.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vm.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://cm.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://sz.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://wd.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vz.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://tg.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://fh.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oj.newstarts.cn

Py:   "第一行\n第二行"
来源：http://zk.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://mv.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://bl.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://so.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ho.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://mp.asd995.cn

Ruby: "第一行\n第二行"
来源：http://ot.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://tt.shtwfgs.cn

[A14] 注释写法
来源：http://ot.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vp.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ls.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://qu.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://za.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vc.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://ww.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cr.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://dq.nszjky.cn

[A15] 空值判断与默认值
来源：http://vl.asd995.cn

Py:   value = data or "默认值"
来源：http://fm.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://fc.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://fg.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ka.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gv.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://lu.colortex.cn

Ruby: value = data || "默认值"
来源：http://rc.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://pc.shxzukj.cn

[A16] 真假值判断规则
来源：http://qj.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kb.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oz.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xb.szxytkj.cn

TS:   if (!x) {}
来源：http://fl.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gx.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nq.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lk.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xu.panjiajie.cn

[A17] 位运算
来源：http://mg.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wo.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yy.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gl.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fu.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sh.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nd.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://bb.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ip.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://nf.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mj.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pf.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://ut.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jf.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://db.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://cw.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://aa.huixiangedu.cn

Py:   a, b = b, a
来源：http://wc.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fu.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://fw.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://ta.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://hk.szxytkj.cn

Go:   a, b = b, a
来源：http://cn.colortex.cn

Ruby: a, b = b, a
来源：http://ad.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://lr.lnxyls.cn

[A20] 读取标准输入
来源：http://bc.hahajie.cn

Py:   name = input("请输入：")
来源：http://zm.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qz.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jq.colortex.cn

TS:   // Node.js：readline 模块
来源：http://zi.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://ce.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lf.nicolike.cn

Ruby: gets.chomp
来源：http://ig.nicolike.cn

C#:   Console.ReadLine();
来源：http://tp.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://pz.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://we.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hp.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://gy.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://jl.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://fp.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gy.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://go.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://be.szsharing.cn

[A22] 获取字符串长度
来源：http://ar.newstarts.cn

Py:   len(s)
来源：http://vm.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qk.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://du.muxihuayi.cn

TS:   s.length
来源：http://oa.9csxet.cn

Java: s.length()
来源：http://sq.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tc.9csxet.cn

Ruby: s.length
来源：http://kq.shxzskj.cn

C#:   s.Length
来源：http://wg.nszjky.cn

[A23] 大小写转换
来源：http://rv.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fo.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iz.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zt.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tb.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dr.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xo.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zz.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hn.gzmigu.cn

[A24] 去除首尾空白
来源：http://sf.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://as.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wb.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vc.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://od.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rz.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ix.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kc.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lo.shtwfgs.cn

[A25] 字符串比较
来源：http://xr.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://dn.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cw.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lv.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ar.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://og.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bv.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ao.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rc.521024.cn

[A26] 类型转换总览
来源：http://qq.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vg.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mn.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qu.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://fl.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ni.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wm.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ui.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hs.bjjhwx.cn

================================================================================
来源：http://nw.shtwfgs.cn

B. 流程控制
来源：http://bj.panjiajie.cn

================================================================================
来源：http://is.colortex.cn

[B01] 条件判断 if / else
来源：http://al.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kv.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ep.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://he.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sr.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xa.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fs.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lh.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yf.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://uk.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zq.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sq.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hn.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nq.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ls.nszjky.cn

[B03] switch / match / case
来源：http://dr.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fa.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bt.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sr.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nh.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hf.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zo.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ax.huanxung.cn

[B04] for 计数循环
来源：http://gj.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://iq.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zo.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rp.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uk.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dk.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hr.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://si.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rr.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://cl.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://tu.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ce.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jy.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hy.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://md.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jo.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://qg.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fk.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://vb.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zm.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://go.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ca.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://av.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vr.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hx.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fi.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zo.panjiajie.cn

[B07] while 循环
来源：http://ak.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://tz.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rm.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://yz.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://xl.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://fi.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ta.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://jx.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://fa.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://wd.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://je.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://jl.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://cw.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://fd.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nb.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bo.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ks.wgjwhj.cn

[B09] break 与 continue
来源：http://fd.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ye.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vc.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.shtwfgs.cn


<!-- 参考信息 -->