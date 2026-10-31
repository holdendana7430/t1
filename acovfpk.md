代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://jd.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xv.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://eo.haigaiapp.cn

[A05] 整数除法与取模
来源：http://sp.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wg.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pv.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fx.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uv.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://ga.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://vp.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://im.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://eg.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://pj.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://xl.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://is.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ba.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ay.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wp.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kx.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ej.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ch.bjjhwx.cn

[A07] 数字转字符串
来源：http://gi.szsharing.cn

Py:   str(42)
来源：http://xz.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://kg.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://ju.panjiajie.cn

TS:   String(42)
来源：http://vw.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://we.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ra.shxzskj.cn

Ruby: 42.to_s
来源：http://gc.nicolike.cn

C#:   42.ToString()
来源：http://hw.szxytkj.cn

[A08] 取整与四舍五入
来源：http://fm.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gg.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lf.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vm.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bs.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://au.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zc.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vc.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xa.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://bj.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eq.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cw.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://om.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bf.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bn.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ar.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://im.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sr.nicolike.cn

[A10] 生成随机数
来源：http://uu.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://ub.nicolike.cn

PHP:  random_int(1, 100);
来源：http://or.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rn.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://th.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://ky.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zq.hnjuh.cn

Ruby: rand(1..100)
来源：http://rk.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://vs.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://xo.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://pr.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ku.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kb.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ie.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ll.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lt.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fy.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ca.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ew.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ne.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://he.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://rp.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://et.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://kx.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ly.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://xj.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://ad.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://my.huanxung.cn

Py:   "第一行\n第二行"
来源：http://wr.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://gc.521024.cn

JS:   "第一行\n第二行"
来源：http://nv.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://su.lnxyls.cn

Java: "第一行\n第二行"
来源：http://yu.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://oc.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://cp.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://gt.nszjky.cn

[A14] 注释写法
来源：http://pt.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://js.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vh.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://sy.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://le.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oi.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://fe.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rb.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://tp.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ks.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://rl.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://ol.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://dv.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://tr.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dj.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://oi.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://ny.521024.cn

C#:   var value = data ?? "默认值";
来源：http://ic.nszjky.cn

[A16] 真假值判断规则
来源：http://xn.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xm.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lb.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://we.colortex.cn

TS:   if (!x) {}
来源：http://nl.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xi.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xo.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ru.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ll.jctech888.com.cn

[A17] 位运算
来源：http://tl.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zy.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uf.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bp.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://us.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bi.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://za.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://tm.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://zl.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://lw.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xv.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nn.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://xc.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://as.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://ks.colortex.cn

C#:   (int)'A'; (char)65
来源：http://qt.asd995.cn

[A19] 交换两个变量
来源：http://vg.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://xg.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://om.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://li.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://kp.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://fs.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://aj.jctech888.com.cn

Ruby: a, b = b, a
来源：http://sk.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://of.hahajie.cn

[A20] 读取标准输入
来源：http://kk.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://fs.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bq.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pr.colortex.cn

TS:   // Node.js：readline 模块
来源：http://cm.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://cc.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ti.chemitech.net.cn

Ruby: gets.chomp
来源：http://rn.nicolike.cn

C#:   Console.ReadLine();
来源：http://aq.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://dr.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://eg.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wv.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://vf.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://rp.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://fh.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jp.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://go.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://mf.nicolike.cn

[A22] 获取字符串长度
来源：http://fm.shxzukj.cn

Py:   len(s)
来源：http://xv.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ab.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://be.wgjwhj.cn

TS:   s.length
来源：http://qs.shtwfgs.cn

Java: s.length()
来源：http://nr.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ys.lnxyls.cn

Ruby: s.length
来源：http://ie.yuexingan06.cn

C#:   s.Length
来源：http://kp.lnxyls.cn

[A23] 大小写转换
来源：http://jh.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dq.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kv.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oh.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wj.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ys.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pv.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zn.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tj.shxzukj.cn

[A24] 去除首尾空白
来源：http://yu.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ew.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cl.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lb.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mw.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rs.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://pu.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://te.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://du.huixiangedu.cn

[A25] 字符串比较
来源：http://wp.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://rc.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bt.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qy.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aq.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cc.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vm.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fr.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sg.nicolike.cn

[A26] 类型转换总览
来源：http://bb.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ru.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lp.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sz.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://yw.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fl.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://te.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qm.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dr.bookmarksfly.cn

================================================================================
来源：http://xu.jianghongdianzi.cn

B. 流程控制
来源：http://wr.shtwfgs.cn

================================================================================
来源：http://cy.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://il.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hm.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ip.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://at.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zl.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ze.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ea.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zx.newstarts.cn

[B02] 多分支 else if / elif
来源：http://at.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nf.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xn.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hv.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aq.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xx.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ds.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.bjjhwx.cn

[B03] switch / match / case
来源：http://ie.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://el.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sp.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fs.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://id.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oq.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://je.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sy.hahajie.cn

[B04] for 计数循环
来源：http://um.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://sm.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rw.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zo.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dr.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zz.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ie.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://wn.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wu.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://fv.asd995.cn

Py:   for item in arr: print(item)
来源：http://yj.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fx.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xj.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xx.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gd.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fx.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ln.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lb.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://fm.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fg.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ds.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dv.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zl.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fp.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qq.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lw.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wx.wgjwhj.cn

[B07] while 循环
来源：http://on.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ln.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kv.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://hi.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://lv.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://ml.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aw.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://sb.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://fc.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://uu.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ie.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yu.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://ax.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ke.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ji.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gw.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kq.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ea.huanxung.cn

[B09] break 与 continue
来源：http://ep.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nc.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zn.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qf.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cr.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pj.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wp.9csxet.cn

[B10] 遍历同时拿索引
来源：http://xr.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nj.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ur.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qr.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kb.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rl.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vc.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tj.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nj.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://jf.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://nq.colortex.cn

PHP:  range(0, 10, 2);
来源：http://gr.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ki.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://we.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kk.jianghongdianzi.cn


<!-- 参考信息 -->