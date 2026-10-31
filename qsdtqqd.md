代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://ou.huixiangedu.cn

[A03] 常量定义
来源：http://gq.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hg.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://xd.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://sm.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://mp.521024.cn

Java: static final double PI = 3.14159;
来源：http://zf.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://wa.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://xd.colortex.cn

C#:   const double PI = 3.14159;
来源：http://sl.asd995.cn

[A04] 判断变量类型
来源：http://ou.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xd.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bx.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zt.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://vi.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://er.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rf.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vu.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://ng.huixiangedu.cn

[A05] 整数除法与取模
来源：http://iv.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cu.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ct.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://im.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ty.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://fl.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://ci.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://to.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://sw.bookmarksfly.cn

[A06] 字符串转数字
来源：http://dn.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://lj.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vu.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://je.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sa.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bv.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lu.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://br.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jk.asd995.cn

[A07] 数字转字符串
来源：http://ao.huixiangedu.cn

Py:   str(42)
来源：http://gg.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ft.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://oy.huixinmuqiang.cn

TS:   String(42)
来源：http://qj.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ii.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://vb.shtwfgs.cn

Ruby: 42.to_s
来源：http://ql.panjiajie.cn

C#:   42.ToString()
来源：http://aq.hnjuh.cn

[A08] 取整与四舍五入
来源：http://db.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yy.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qb.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iz.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ic.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rb.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uk.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lz.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ro.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://qo.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ub.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jc.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kx.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://if.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mc.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xo.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rc.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pv.shxzskj.cn

[A10] 生成随机数
来源：http://zl.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://zg.newstarts.cn

PHP:  random_int(1, 100);
来源：http://eg.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://km.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://la.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://az.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dm.shxzukj.cn

Ruby: rand(1..100)
来源：http://wb.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://sr.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://wm.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://nu.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://de.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ht.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wo.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://ac.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sr.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wu.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://et.521024.cn

[A12] 字符串插值 / 格式化
来源：http://ta.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vx.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ut.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://qf.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://jr.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://nl.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://af.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://rj.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://ny.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bf.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://jr.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://nx.newstarts.cn

JS:   "第一行\n第二行"
来源：http://tk.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://gq.gzmigu.cn

Java: "第一行\n第二行"
来源：http://go.9csxet.cn

Go:   "第一行\n第二行"
来源：http://pc.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://ps.9csxet.cn

C#:   "第一行\n第二行"
来源：http://va.jctech888.com.cn

[A14] 注释写法
来源：http://rx.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://by.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lp.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://gs.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://cz.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rc.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://kg.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wu.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://gr.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://vc.nszjky.cn

Py:   value = data or "默认值"
来源：http://ub.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://iv.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://bb.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://oh.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ym.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://uw.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://bq.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://iq.521024.cn

[A16] 真假值判断规则
来源：http://qe.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cx.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eu.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kq.bjjhwx.cn

TS:   if (!x) {}
来源：http://og.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rp.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bt.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vh.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://od.bookmarksfly.cn

[A17] 位运算
来源：http://gw.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wu.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cz.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xu.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rl.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tw.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jm.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pv.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://av.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://sg.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://qx.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://nj.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wa.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nv.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://to.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hm.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://ns.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://cd.huanxung.cn

[A19] 交换两个变量
来源：http://nq.hahajie.cn

Py:   a, b = b, a
来源：http://iv.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ms.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://vk.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://jn.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://sp.nicolike.cn

Go:   a, b = b, a
来源：http://ik.bjjhwx.cn

Ruby: a, b = b, a
来源：http://tw.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://yo.521024.cn

[A20] 读取标准输入
来源：http://nk.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://dv.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://id.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lz.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://sc.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://xi.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vx.hnjuh.cn

Ruby: gets.chomp
来源：http://ng.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://hg.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://wk.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://uc.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fr.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://hp.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://ue.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://hz.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zh.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://du.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://up.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://xr.lnxyls.cn

Py:   len(s)
来源：http://et.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gj.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fg.shxzukj.cn

TS:   s.length
来源：http://eh.shxzukj.cn

Java: s.length()
来源：http://wz.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hq.shxzskj.cn

Ruby: s.length
来源：http://mp.huixiangedu.cn

C#:   s.Length
来源：http://mu.nicolike.cn

[A23] 大小写转换
来源：http://jm.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ak.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ii.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fs.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://go.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ut.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jm.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hj.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lf.shtwfgs.cn

[A24] 去除首尾空白
来源：http://te.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vd.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ot.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://is.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ta.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rv.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ek.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cl.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qj.gzmigu.cn

[A25] 字符串比较
来源：http://kk.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://hb.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bj.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ul.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jm.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wr.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ft.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ar.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pr.9csxet.cn

[A26] 类型转换总览
来源：http://dt.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tz.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://am.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dx.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://wk.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rr.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rf.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rs.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sl.hnjuh.cn

================================================================================
来源：http://rk.huanxung.cn

B. 流程控制
来源：http://cz.gzmigu.cn

================================================================================
来源：http://nh.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://jw.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cr.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tw.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sx.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ba.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wf.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://no.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fi.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wu.colortex.cn

[B02] 多分支 else if / elif
来源：http://xd.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iy.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cl.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fu.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qy.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pb.shtwfgs.cn

[B03] switch / match / case
来源：http://nw.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ma.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ua.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jm.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kb.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vh.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ri.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jg.shtwfgs.cn

[B04] for 计数循环
来源：http://vb.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://xt.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xb.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://np.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xn.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tf.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://co.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yb.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://to.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://uj.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zr.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zz.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qu.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bm.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://hx.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uf.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://gl.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ni.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ot.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ld.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kj.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bu.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xy.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ne.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yh.wgjwhj.cn

[B07] while 循环
来源：http://vc.newstarts.cn

Py:   while i < 10: i += 1
来源：http://lr.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qn.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://ac.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://ux.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://ys.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ic.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://qc.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://tw.colortex.cn

[B08] do-while（至少执行一次）
来源：http://je.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://wi.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yd.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ai.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://xi.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://mk.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://az.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xx.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://aa.wgjwhj.cn

[B09] break 与 continue
来源：http://tj.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hc.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sk.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jz.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tj.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zr.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oa.9csxet.cn


<!-- 参考信息 -->