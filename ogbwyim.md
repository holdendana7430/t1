代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://fw.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://xn.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://st.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://bc.bjjhwx.cn

[A06] 字符串转数字
来源：http://hf.asd995.cn

Py:   int("42"); float("3.14")
来源：http://yl.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hd.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ia.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jj.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pu.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gq.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xh.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pz.jctech888.com.cn

[A07] 数字转字符串
来源：http://bn.szsharing.cn

Py:   str(42)
来源：http://ai.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://ke.9csxet.cn

JS:   String(42); (42).toString()
来源：http://ob.asd995.cn

TS:   String(42)
来源：http://hu.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mb.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://bf.lnxyls.cn

Ruby: 42.to_s
来源：http://qb.bjjhwx.cn

C#:   42.ToString()
来源：http://iy.9csxet.cn

[A08] 取整与四舍五入
来源：http://sa.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iq.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ip.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ml.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hg.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jj.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dl.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ku.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wz.colortex.cn

[A09] 绝对值与最大最小值
来源：http://hl.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://am.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ys.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qb.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hq.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tq.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ho.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wb.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eg.szxytkj.cn

[A10] 生成随机数
来源：http://fh.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://qa.521024.cn

PHP:  random_int(1, 100);
来源：http://nt.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kd.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nd.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://lf.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wh.shxzskj.cn

Ruby: rand(1..100)
来源：http://ss.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://um.9csxet.cn

[A11] 条件表达式（三元）
来源：http://gx.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://vm.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://px.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rp.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uo.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://mp.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yt.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gz.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zg.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ra.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dh.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ej.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://qn.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://it.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ex.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pt.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://sg.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://gp.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pq.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://gt.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://zx.newstarts.cn

JS:   "第一行\n第二行"
来源：http://xw.huanxung.cn

TS:   "第一行\n第二行"
来源：http://bq.521024.cn

Java: "第一行\n第二行"
来源：http://cu.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://xd.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://mr.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://ac.asd995.cn

[A14] 注释写法
来源：http://ra.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wq.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yj.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://ai.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://al.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bj.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://lk.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ir.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://xo.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://bd.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://mb.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://aj.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://tl.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://yd.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pe.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://yj.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://wi.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://fz.haigaiapp.cn

[A16] 真假值判断规则
来源：http://jc.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pr.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ut.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dj.newstarts.cn

TS:   if (!x) {}
来源：http://nr.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://eq.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tk.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uh.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.jianghongdianzi.cn

[A17] 位运算
来源：http://kq.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rq.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jd.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://io.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gi.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vd.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://et.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://xc.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://tk.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://um.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jx.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ut.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bx.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ya.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://ju.huanxung.cn

[A19] 交换两个变量
来源：http://iu.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://gi.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ju.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://yh.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://xi.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://lq.hnjuh.cn

Go:   a, b = b, a
来源：http://bm.hnjuh.cn

Ruby: a, b = b, a
来源：http://hy.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://rv.hahajie.cn

[A20] 读取标准输入
来源：http://ux.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://cf.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://al.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cl.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://im.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://cc.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ji.yuexingan06.cn

Ruby: gets.chomp
来源：http://ye.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://dd.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://ag.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://eo.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gg.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://jm.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://wc.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://sz.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://om.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xn.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://sh.newstarts.cn

[A22] 获取字符串长度
来源：http://gn.shxzskj.cn

Py:   len(s)
来源：http://lf.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://or.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ri.yuntaijiaju.cn

TS:   s.length
来源：http://lj.521024.cn

Java: s.length()
来源：http://po.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mr.hahajie.cn

Ruby: s.length
来源：http://ig.hahajie.cn

C#:   s.Length
来源：http://ra.haigaiapp.cn

[A23] 大小写转换
来源：http://rb.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vm.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eu.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sg.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gj.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mt.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rg.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xf.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ul.yuexingan06.cn

[A24] 去除首尾空白
来源：http://di.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jj.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sj.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aa.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wx.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://fw.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wu.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jg.nszjky.cn

[A25] 字符串比较
来源：http://ca.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://uy.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ml.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zx.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tt.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://me.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nr.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pn.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tf.hnjuh.cn

[A26] 类型转换总览
来源：http://yp.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oc.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://od.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kq.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://gn.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pg.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gp.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pi.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aj.colortex.cn

================================================================================
来源：http://mz.wgjwhj.cn

B. 流程控制
来源：http://mo.bookmarksfly.cn

================================================================================
来源：http://qy.shxzukj.cn

[B01] 条件判断 if / else
来源：http://kq.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ou.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dc.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://om.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aa.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ci.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://en.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://he.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://my.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://dm.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xb.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iy.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fa.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fo.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.shxzukj.cn

[B03] switch / match / case
来源：http://ou.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xb.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fm.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mn.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pj.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qm.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bn.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zs.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xn.bjjhwx.cn

[B04] for 计数循环
来源：http://nv.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://zo.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nv.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qe.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ov.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://il.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jz.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://gx.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wp.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ha.nicolike.cn

Py:   for item in arr: print(item)
来源：http://iz.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zw.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://am.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vg.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ev.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gh.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://ps.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://he.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://zh.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fx.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ty.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pp.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pw.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ga.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ij.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://el.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kp.haigaiapp.cn

[B07] while 循环
来源：http://oq.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://mq.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://or.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://nd.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://vy.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://zp.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ai.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://sd.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ut.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://vr.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://eb.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yc.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://pi.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://af.521024.cn

Java: do { i++; } while (i < 10);
来源：http://mn.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vt.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jp.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://ha.hahajie.cn

[B09] break 与 continue
来源：http://sh.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vw.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iw.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lb.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bj.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gl.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://us.521024.cn

[B10] 遍历同时拿索引
来源：http://vi.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ov.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mp.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gp.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kq.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nb.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://is.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iy.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fz.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://jy.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ho.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://lj.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yj.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oq.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ed.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qv.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://gq.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fq.hnjuh.cn

[B12] 跳出多层循环
来源：http://xj.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jn.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mf.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wq.huixinmuqiang.cn


<!-- 参考信息 -->