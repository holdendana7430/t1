代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tj.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://si.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://er.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fb.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uv.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://az.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://gq.szxytkj.cn

[A05] 整数除法与取模
来源：http://gg.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wk.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zn.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ml.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cy.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://mv.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://bh.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://hx.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://vy.9csxet.cn

[A06] 字符串转数字
来源：http://yd.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://nf.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sv.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mt.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fh.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://th.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://af.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hm.bjjhwx.cn

[A07] 数字转字符串
来源：http://nq.jianghongdianzi.cn

Py:   str(42)
来源：http://pv.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://ij.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://be.haigaiapp.cn

TS:   String(42)
来源：http://ee.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ee.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://zx.shtwfgs.cn

Ruby: 42.to_s
来源：http://ii.asd995.cn

C#:   42.ToString()
来源：http://oj.colortex.cn

[A08] 取整与四舍五入
来源：http://ap.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lc.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xj.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oc.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ng.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hq.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ox.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://st.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nb.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://qq.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xw.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nt.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sw.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ku.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mw.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lr.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qh.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://np.hahajie.cn

[A10] 生成随机数
来源：http://hv.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://qj.asd995.cn

PHP:  random_int(1, 100);
来源：http://mp.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vl.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://io.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://ur.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://db.nszjky.cn

Ruby: rand(1..100)
来源：http://ud.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://id.nicolike.cn

[A11] 条件表达式（三元）
来源：http://yt.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://dm.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vy.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mu.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rq.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://xz.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gr.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qh.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eu.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://ug.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xk.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://td.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://ks.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://wq.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://gy.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gz.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://px.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://nn.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rs.huanxung.cn

Py:   "第一行\n第二行"
来源：http://sj.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://nr.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://hx.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://vn.hahajie.cn

Java: "第一行\n第二行"
来源：http://cq.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://ek.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://kx.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://wu.chemitech.net.cn

[A14] 注释写法
来源：http://na.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://en.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kx.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://fi.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://ih.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zf.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://yi.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dt.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://vu.newstarts.cn

[A15] 空值判断与默认值
来源：http://ca.asd995.cn

Py:   value = data or "默认值"
来源：http://wg.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://ru.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://gb.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://xy.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://uv.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://au.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://so.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://if.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gt.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gm.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bg.yuexingan06.cn

TS:   if (!x) {}
来源：http://at.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hw.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://il.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zd.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bj.yuntaijiaju.cn

[A17] 位运算
来源：http://pc.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sx.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pa.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ig.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xz.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://au.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lh.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dx.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://qc.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://jf.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://hx.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qh.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oe.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://va.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pt.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://du.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ru.bookmarksfly.cn

[A19] 交换两个变量
来源：http://ro.shtwfgs.cn

Py:   a, b = b, a
来源：http://ui.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xb.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://mk.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://vt.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://rn.shtwfgs.cn

Go:   a, b = b, a
来源：http://cy.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://zb.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://ir.bjjhwx.cn

[A20] 读取标准输入
来源：http://vx.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://rs.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sm.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vt.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://fb.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://co.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yz.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://rm.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ij.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://tl.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://qb.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tn.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://ih.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://iq.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://ur.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ih.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ao.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://sp.9csxet.cn

[A22] 获取字符串长度
来源：http://pe.hnjuh.cn

Py:   len(s)
来源：http://lg.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ex.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eo.huixiangedu.cn

TS:   s.length
来源：http://bn.haigaiapp.cn

Java: s.length()
来源：http://pe.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ky.nicolike.cn

Ruby: s.length
来源：http://wo.521024.cn

C#:   s.Length
来源：http://ta.yuexingan06.cn

[A23] 大小写转换
来源：http://si.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cu.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ht.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zk.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gw.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hs.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ed.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qg.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fy.nszjky.cn

[A24] 去除首尾空白
来源：http://xc.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ls.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ti.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zt.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kx.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oh.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://cu.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nq.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://je.hahajie.cn

[A25] 字符串比较
来源：http://am.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://xh.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ol.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ce.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yb.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kt.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cy.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kx.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ov.gzmigu.cn

[A26] 类型转换总览
来源：http://eo.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mv.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zc.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hr.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://lu.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sr.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pm.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zn.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mh.huixinmuqiang.cn

================================================================================
来源：http://bt.huixiangedu.cn

B. 流程控制
来源：http://jc.lnxyls.cn

================================================================================
来源：http://vd.shxzukj.cn

[B01] 条件判断 if / else
来源：http://qy.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ej.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uo.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lf.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qu.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iz.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dv.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jh.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oo.szsharing.cn

[B02] 多分支 else if / elif
来源：http://pv.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ui.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://he.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ht.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ec.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.huixinmuqiang.cn

[B03] switch / match / case
来源：http://je.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yz.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ym.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uj.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cq.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zs.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oz.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ip.nszjky.cn

[B04] for 计数循环
来源：http://mm.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://fh.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ay.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qu.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lp.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qb.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://jg.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rd.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://xz.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://tw.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mo.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sx.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ig.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lc.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oy.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://qy.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://te.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://ad.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uw.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yc.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vb.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hi.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xh.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xj.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nq.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://za.jctech888.com.cn

[B07] while 循环
来源：http://ns.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://jk.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://et.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://cf.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://iu.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://uo.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://co.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://dd.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://zr.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ay.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://ar.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ih.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://hs.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://la.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://zz.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bf.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lq.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://lm.szsharing.cn

[B09] break 与 continue
来源：http://hx.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wg.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mh.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://og.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qa.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ot.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ib.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dj.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rl.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ry.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lo.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fy.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tu.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gm.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://tj.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ds.jianghongdianzi.cn


<!-- 参考信息 -->