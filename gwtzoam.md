代发 wailian999

[A02] 变量声明与赋值
来源：http://eq.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ml.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jx.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lx.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://we.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://zu.521024.cn

Go:   name := "Alex"; age := 20
来源：http://fg.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://cm.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gb.szsharing.cn

[A03] 常量定义
来源：http://jq.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://av.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://be.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://co.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://bo.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://fi.gzmigu.cn

Go:   const PI = 3.14159
来源：http://vv.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://nk.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://ch.muxihuayi.cn

[A04] 判断变量类型
来源：http://nw.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wk.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pe.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://by.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://cw.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fq.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://du.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jw.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://lp.shxzukj.cn

[A05] 整数除法与取模
来源：http://en.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qy.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jg.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yj.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hp.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://cs.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://bb.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://tm.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://dk.huixiangedu.cn

[A06] 字符串转数字
来源：http://rk.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://wn.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://df.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xo.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nz.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ot.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qq.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dh.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bi.jctech888.com.cn

[A07] 数字转字符串
来源：http://kb.wgjwhj.cn

Py:   str(42)
来源：http://fa.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://ns.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://nv.huixinmuqiang.cn

TS:   String(42)
来源：http://dx.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ws.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://la.newstarts.cn

Ruby: 42.to_s
来源：http://pl.nicolike.cn

C#:   42.ToString()
来源：http://ft.shxzukj.cn

[A08] 取整与四舍五入
来源：http://ag.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jj.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://be.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tr.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wa.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eu.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://no.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://en.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xc.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://bk.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yu.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pb.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bs.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hr.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xm.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xa.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mb.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ui.bjjhwx.cn

[A10] 生成随机数
来源：http://er.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ow.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://zm.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://el.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yj.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://hd.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ti.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://yq.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://bk.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://ai.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://so.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ck.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iy.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://er.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://iq.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xf.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mc.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ig.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://zk.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ua.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vq.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://so.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://iz.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://ji.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bp.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://eo.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://jj.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wt.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://xk.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://qr.521024.cn

JS:   "第一行\n第二行"
来源：http://vp.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://yw.nszjky.cn

Java: "第一行\n第二行"
来源：http://gh.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://oi.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://oe.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://yg.jianghongdianzi.cn

[A14] 注释写法
来源：http://lq.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yj.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://as.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://rg.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://gh.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lv.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://fh.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wk.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://ff.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://bs.521024.cn

Py:   value = data or "默认值"
来源：http://iz.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://gs.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://cy.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://oi.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hh.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://sm.9csxet.cn

Ruby: value = data || "默认值"
来源：http://fx.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://vv.shxzukj.cn

[A16] 真假值判断规则
来源：http://fl.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wd.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cm.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jt.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://zt.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jq.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yw.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gl.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vl.chemitech.net.cn

[A17] 位运算
来源：http://wv.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ty.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ev.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ua.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hh.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vr.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bm.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vg.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://hq.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://aj.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ug.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uo.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ph.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://od.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ms.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://ed.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://bb.haigaiapp.cn

[A19] 交换两个变量
来源：http://hp.panjiajie.cn

Py:   a, b = b, a
来源：http://oc.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gi.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://bt.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://sr.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://pq.shxzukj.cn

Go:   a, b = b, a
来源：http://fj.nszjky.cn

Ruby: a, b = b, a
来源：http://lu.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://ut.yuexingan06.cn

[A20] 读取标准输入
来源：http://uy.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://pm.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mg.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yf.asd995.cn

TS:   // Node.js：readline 模块
来源：http://hc.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://lx.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jh.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://ll.lnxyls.cn

C#:   Console.ReadLine();
来源：http://nb.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://pq.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://oj.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lf.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://ou.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://dy.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://nj.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pj.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://vk.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://vz.bjjhwx.cn

[A22] 获取字符串长度
来源：http://eh.huixiangedu.cn

Py:   len(s)
来源：http://do.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zo.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sd.gzmigu.cn

TS:   s.length
来源：http://yw.wgjwhj.cn

Java: s.length()
来源：http://gs.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://op.hnjuh.cn

Ruby: s.length
来源：http://ft.colortex.cn

C#:   s.Length
来源：http://pa.wgjwhj.cn

[A23] 大小写转换
来源：http://ez.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ez.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kv.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yj.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cy.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mb.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://so.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tb.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xu.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ix.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fq.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ep.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hl.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yr.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yg.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://yw.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pl.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pz.hnjuh.cn

[A25] 字符串比较
来源：http://rs.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://ko.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oc.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fy.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dr.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pc.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vo.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dd.wgjwhj.cn

[A26] 类型转换总览
来源：http://ef.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bl.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rl.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fe.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://un.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rw.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xa.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://is.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nf.newstarts.cn

================================================================================
来源：http://jm.panjiajie.cn

B. 流程控制
来源：http://gz.nszjky.cn

================================================================================
来源：http://sw.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://uu.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nh.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yl.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zq.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fr.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lg.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yd.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ys.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rd.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://gp.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hs.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vj.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nn.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wg.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ho.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.lnxyls.cn

[B03] switch / match / case
来源：http://bm.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fc.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://et.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wj.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ps.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ds.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ui.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ek.yuexingan06.cn

[B04] for 计数循环
来源：http://so.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://xa.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lo.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ux.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wm.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rz.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pk.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://ig.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gc.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://di.nicolike.cn

Py:   for item in arr: print(item)
来源：http://yd.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hk.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vq.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vw.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ul.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nz.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://st.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://cn.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tv.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kd.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://or.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bn.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lg.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mi.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xf.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gw.huanxung.cn

[B07] while 循环
来源：http://rc.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://yy.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uc.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://ls.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://xf.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://dh.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vh.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://of.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://xv.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://jq.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://xa.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://th.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://no.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://mo.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://dd.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://re.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kv.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://to.huanxung.cn


<!-- 参考信息 -->