代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jp.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hg.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://tb.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rj.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://my.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://np.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://iz.wgjwhj.cn

[A05] 整数除法与取模
来源：http://ka.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hr.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rg.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wx.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vc.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://fi.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://su.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://ge.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://oj.hnjuh.cn

[A06] 字符串转数字
来源：http://fg.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://yz.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wh.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qr.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cx.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zz.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fl.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yu.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://af.521024.cn

[A07] 数字转字符串
来源：http://ay.bookmarksfly.cn

Py:   str(42)
来源：http://bh.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://ar.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://am.huixinmuqiang.cn

TS:   String(42)
来源：http://iu.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aw.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://el.bjjhwx.cn

Ruby: 42.to_s
来源：http://yb.hahajie.cn

C#:   42.ToString()
来源：http://ff.gzmigu.cn

[A08] 取整与四舍五入
来源：http://wa.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lf.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aj.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ad.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lr.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fq.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jy.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gq.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gl.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://qd.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cw.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ve.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tc.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ry.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ks.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://no.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ff.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bq.gzmigu.cn

[A10] 生成随机数
来源：http://ch.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://yo.nszjky.cn

PHP:  random_int(1, 100);
来源：http://pe.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ul.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mf.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://ks.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cx.9csxet.cn

Ruby: rand(1..100)
来源：http://sh.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://go.nszjky.cn

[A11] 条件表达式（三元）
来源：http://ve.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://hb.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nz.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xq.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lr.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://qz.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kl.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hc.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cu.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://ew.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vs.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zk.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://ap.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://gy.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ca.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tw.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://nb.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://og.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oy.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://ji.colortex.cn

PHP:  "第一行\n第二行"
来源：http://vc.nszjky.cn

JS:   "第一行\n第二行"
来源：http://ww.huanxung.cn

TS:   "第一行\n第二行"
来源：http://sh.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://el.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://xc.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://fy.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://ll.521024.cn

[A14] 注释写法
来源：http://xi.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nd.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://tk.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://an.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vr.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://zc.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ua.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ra.nicolike.cn

[A15] 空值判断与默认值
来源：http://ra.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://xa.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://tc.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://yy.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://gx.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ec.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://xx.huanxung.cn

Ruby: value = data || "默认值"
来源：http://vi.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://ex.shtwfgs.cn

[A16] 真假值判断规则
来源：http://kl.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vx.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xi.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bk.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://ns.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xf.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zu.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sz.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uu.9csxet.cn

[A17] 位运算
来源：http://cs.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xr.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ea.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wn.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lu.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fk.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jw.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://bf.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://es.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://dy.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tq.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dg.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://ro.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pm.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://be.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://ny.gzmigu.cn

[A19] 交换两个变量
来源：http://kz.chemitech.net.cn

Py:   a, b = b, a
来源：http://jp.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bo.521024.cn

JS:   [a, b] = [b, a];
来源：http://bj.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://ig.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://xg.chemitech.net.cn

Go:   a, b = b, a
来源：http://zo.gzmigu.cn

Ruby: a, b = b, a
来源：http://ur.colortex.cn

C#:   (a, b) = (b, a);
来源：http://hr.huanxung.cn

[A20] 读取标准输入
来源：http://gm.hahajie.cn

Py:   name = input("请输入：")
来源：http://zl.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gy.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jf.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://fb.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://df.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cs.newstarts.cn

Ruby: gets.chomp
来源：http://nh.shxzukj.cn

C#:   Console.ReadLine();
来源：http://yc.nicolike.cn

[A21] 保留指定小数位输出
来源：http://vm.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://vs.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://my.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://uy.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://wl.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://dw.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ht.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://um.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://xx.shtwfgs.cn

[A22] 获取字符串长度
来源：http://hk.huixinmuqiang.cn

Py:   len(s)
来源：http://bi.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zf.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sm.hnjuh.cn

TS:   s.length
来源：http://pd.gzmigu.cn

Java: s.length()
来源：http://ig.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lf.gzmigu.cn

Ruby: s.length
来源：http://iw.newstarts.cn

C#:   s.Length
来源：http://bg.521024.cn

[A23] 大小写转换
来源：http://en.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://an.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ai.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://er.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gm.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xl.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kd.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ft.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iw.panjiajie.cn

[A24] 去除首尾空白
来源：http://hr.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nb.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kz.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mk.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sy.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oc.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://tv.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kz.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xk.521024.cn

[A25] 字符串比较
来源：http://vx.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://mp.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gi.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dk.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ck.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ao.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lb.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sk.colortex.cn

[A26] 类型转换总览
来源：http://xr.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oj.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ep.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://en.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://ll.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yo.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://an.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gd.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xh.shtwfgs.cn

================================================================================
来源：http://ne.shxzukj.cn

B. 流程控制
来源：http://md.shxzukj.cn

================================================================================
来源：http://ka.newstarts.cn

[B01] 条件判断 if / else
来源：http://ep.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hs.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ei.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yk.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tg.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ux.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vf.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ei.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zr.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ov.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cd.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ej.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fw.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nc.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sa.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.shtwfgs.cn

[B03] switch / match / case
来源：http://pd.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://de.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yb.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ha.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://la.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aj.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://po.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sk.huixiangedu.cn

[B04] for 计数循环
来源：http://al.colortex.cn

Py:   for i in range(10): print(i)
来源：http://md.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nb.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bh.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qv.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dy.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ih.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://xy.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ld.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ba.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://zj.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ez.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vb.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ac.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xo.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tz.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://ta.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yr.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://mf.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mj.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ph.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cw.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oy.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://he.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xe.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rx.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ul.shtwfgs.cn

[B07] while 循环
来源：http://ii.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://nf.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oh.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://cm.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://kg.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://er.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qo.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://xz.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://gc.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://iw.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://xw.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tp.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://hl.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://eg.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://aa.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jv.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ol.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://wh.shxzskj.cn

[B09] break 与 continue
来源：http://wa.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hg.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rw.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jo.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sg.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ee.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://hk.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pa.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nt.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://os.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kw.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gs.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tz.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://do.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://qz.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://wk.huanxung.cn


<!-- 参考信息 -->