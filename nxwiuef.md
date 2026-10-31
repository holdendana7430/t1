代发 wailian999

Ruby: PI = 3.14159
来源：http://gv.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://mq.asd995.cn

[A04] 判断变量类型
来源：http://hd.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cj.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ec.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hm.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://qj.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oq.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dm.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xm.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://qs.muxihuayi.cn

[A05] 整数除法与取模
来源：http://lb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jf.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zm.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xd.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://go.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://ow.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://so.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://qj.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://ha.shtwfgs.cn

[A06] 字符串转数字
来源：http://bh.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://bs.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ci.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zf.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oo.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vr.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qu.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nh.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vj.szxytkj.cn

[A07] 数字转字符串
来源：http://dk.hnjuh.cn

Py:   str(42)
来源：http://es.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://xm.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://lr.huixinmuqiang.cn

TS:   String(42)
来源：http://ib.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wk.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://da.9csxet.cn

Ruby: 42.to_s
来源：http://sm.newstarts.cn

C#:   42.ToString()
来源：http://iv.shxzskj.cn

[A08] 取整与四舍五入
来源：http://vy.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dl.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nr.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ru.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wx.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ta.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uf.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pu.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ai.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ru.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jt.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bu.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fw.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xs.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vy.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rm.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ta.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dz.hnjuh.cn

[A10] 生成随机数
来源：http://fn.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://pu.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://gx.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://av.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lg.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://oi.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://de.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://hg.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://ro.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://lp.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://uc.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ng.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://py.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qb.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://cp.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ct.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ci.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://on.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://gf.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://za.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nj.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://je.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://sl.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://vu.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dh.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ke.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://xf.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gy.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://th.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://zt.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://md.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://hc.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://hh.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://zb.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://gr.nszjky.cn

C#:   "第一行\n第二行"
来源：http://bf.shtwfgs.cn

[A14] 注释写法
来源：http://ko.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eq.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vh.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://cx.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://zh.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iw.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://hz.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qk.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://iv.nicolike.cn

[A15] 空值判断与默认值
来源：http://sb.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://of.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://qq.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://pz.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://av.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rm.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://xd.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://er.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://eu.chemitech.net.cn

[A16] 真假值判断规则
来源：http://sc.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dt.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dc.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://li.wgjwhj.cn

TS:   if (!x) {}
来源：http://wa.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fg.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://og.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mb.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tk.nszjky.cn

[A17] 位运算
来源：http://my.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qn.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ki.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xp.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yz.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ms.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://qo.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://fq.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://rs.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lz.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ac.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ko.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ph.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://cd.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://vg.asd995.cn

[A19] 交换两个变量
来源：http://zr.521024.cn

Py:   a, b = b, a
来源：http://ku.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dx.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://yq.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://dv.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://ow.bookmarksfly.cn

Go:   a, b = b, a
来源：http://pu.haigaiapp.cn

Ruby: a, b = b, a
来源：http://vf.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://cc.jctech888.com.cn

[A20] 读取标准输入
来源：http://sn.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://gk.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ov.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kx.asd995.cn

TS:   // Node.js：readline 模块
来源：http://oj.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://ck.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eb.lnxyls.cn

Ruby: gets.chomp
来源：http://tr.nszjky.cn

C#:   Console.ReadLine();
来源：http://ct.asd995.cn

[A21] 保留指定小数位输出
来源：http://nu.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://gs.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ky.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://yt.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://vt.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://jx.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yw.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ka.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://rg.huanxung.cn

[A22] 获取字符串长度
来源：http://fn.jctech888.com.cn

Py:   len(s)
来源：http://sy.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://if.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ny.shxzukj.cn

TS:   s.length
来源：http://ls.huixiangedu.cn

Java: s.length()
来源：http://kl.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dp.colortex.cn

Ruby: s.length
来源：http://ue.hahajie.cn

C#:   s.Length
来源：http://ej.yuexingan06.cn

[A23] 大小写转换
来源：http://rc.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zk.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://io.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qu.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kf.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xe.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tu.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yv.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ce.bjjhwx.cn

[A24] 去除首尾空白
来源：http://yj.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zq.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dc.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ub.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://et.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nd.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://fb.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sl.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cq.lnxyls.cn

[A25] 字符串比较
来源：http://kj.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://sc.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hx.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qt.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cv.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wz.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uu.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://de.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ng.chemitech.net.cn

[A26] 类型转换总览
来源：http://jq.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vy.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yz.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tx.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://jc.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wz.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://st.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ge.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dt.shxzukj.cn

================================================================================
来源：http://kl.yuexingan06.cn

B. 流程控制
来源：http://gy.chemitech.net.cn

================================================================================
来源：http://ye.asd995.cn

[B01] 条件判断 if / else
来源：http://sx.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sr.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sq.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cm.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hq.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uj.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bt.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://to.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fv.asd995.cn

[B02] 多分支 else if / elif
来源：http://by.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ha.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eg.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sv.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hs.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.shtwfgs.cn

[B03] switch / match / case
来源：http://cf.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bz.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ye.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rd.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eh.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xt.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uz.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zl.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zz.wgjwhj.cn

[B04] for 计数循环
来源：http://wi.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://go.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kw.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ph.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fd.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lx.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ih.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://us.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://lc.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://wp.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qr.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ht.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yz.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nz.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rh.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ba.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xn.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://np.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pd.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pd.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sy.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://az.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tf.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yt.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xo.chemitech.net.cn

[B07] while 循环
来源：http://oy.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://qw.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mm.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://wp.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ck.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://fw.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ma.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://ou.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://ro.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://uu.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://sw.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ha.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://pe.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://nr.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://cs.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ap.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gt.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ny.asd995.cn

[B09] break 与 continue
来源：http://sl.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://un.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qa.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://re.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xe.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://iq.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ty.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://me.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pb.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vs.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://be.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hg.jctech888.com.cn


<!-- 参考信息 -->