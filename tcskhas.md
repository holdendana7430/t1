代发 wailian999

[A06] 字符串转数字
来源：http://vm.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ql.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mo.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ed.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xx.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uh.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ce.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rh.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pv.lnxyls.cn

[A07] 数字转字符串
来源：http://ww.jctech888.com.cn

Py:   str(42)
来源：http://pd.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://ot.521024.cn

JS:   String(42); (42).toString()
来源：http://fc.szsharing.cn

TS:   String(42)
来源：http://zc.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://os.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://yo.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://pl.colortex.cn

C#:   42.ToString()
来源：http://xt.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://vx.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://is.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xf.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ae.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mf.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gs.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jv.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hy.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ys.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://cg.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jf.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://du.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cz.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bj.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zo.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cl.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cj.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pr.wgjwhj.cn

[A10] 生成随机数
来源：http://au.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://zn.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://tn.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qs.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dk.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ct.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ts.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ib.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://ho.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://fx.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://by.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mu.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cu.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wu.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://oz.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sp.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pv.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://do.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://fm.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ix.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bi.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://ms.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://dx.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://pi.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cb.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://kz.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://kn.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gk.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://gj.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://gh.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://nf.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://to.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://ll.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ge.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://gp.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ck.szxytkj.cn

[A14] 注释写法
来源：http://za.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qd.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ic.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://bh.521024.cn

TS:   // 单行；/* 多行 */
来源：http://tb.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wi.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://bx.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://id.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://dg.nicolike.cn

[A15] 空值判断与默认值
来源：http://ar.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://ez.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://nw.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://hg.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://dx.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rx.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://ki.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://sl.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://zc.yuexingan06.cn

[A16] 真假值判断规则
来源：http://rs.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zj.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lp.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yg.szxytkj.cn

TS:   if (!x) {}
来源：http://ws.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://th.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ln.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yl.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gm.haigaiapp.cn

[A17] 位运算
来源：http://vv.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wt.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zh.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tk.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vu.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://la.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://he.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://gp.521024.cn

PHP:  ord("A"); chr(65)
来源：http://oe.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kn.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ff.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://hl.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tf.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://bd.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://jf.shxzukj.cn

[A19] 交换两个变量
来源：http://js.nszjky.cn

Py:   a, b = b, a
来源：http://jg.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ob.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://jz.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://kq.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://yk.panjiajie.cn

Go:   a, b = b, a
来源：http://fc.haigaiapp.cn

Ruby: a, b = b, a
来源：http://pf.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://un.hahajie.cn

[A20] 读取标准输入
来源：http://cs.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://cm.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tl.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kh.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://la.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ga.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xy.9csxet.cn

Ruby: gets.chomp
来源：http://nu.nicolike.cn

C#:   Console.ReadLine();
来源：http://pz.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://zh.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://jj.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ed.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ks.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://vu.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://zo.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cx.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://cv.521024.cn

C#:   3.14159.ToString("F2")
来源：http://io.gzmigu.cn

[A22] 获取字符串长度
来源：http://cf.szsharing.cn

Py:   len(s)
来源：http://dc.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bf.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gl.hahajie.cn

TS:   s.length
来源：http://cx.huixiangedu.cn

Java: s.length()
来源：http://jm.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://po.szsharing.cn

Ruby: s.length
来源：http://qp.yuntaijiaju.cn

C#:   s.Length
来源：http://qh.shtwfgs.cn

[A23] 大小写转换
来源：http://xg.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://de.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qw.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gl.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dw.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cl.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ep.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ov.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oo.szxytkj.cn

[A24] 去除首尾空白
来源：http://mk.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://to.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ig.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://by.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ny.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wl.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://ai.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jf.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vw.jianghongdianzi.cn

[A25] 字符串比较
来源：http://lv.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://kl.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tn.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zb.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yh.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iy.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bd.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lq.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dq.hahajie.cn

[A26] 类型转换总览
来源：http://ya.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kd.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ex.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mz.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://gs.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pb.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tp.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yn.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qt.huixinmuqiang.cn

================================================================================
来源：http://ve.shxzskj.cn

B. 流程控制
来源：http://gt.huixiangedu.cn

================================================================================
来源：http://jy.szsharing.cn

[B01] 条件判断 if / else
来源：http://xq.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ij.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xn.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qq.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ik.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qk.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mz.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hy.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oo.hahajie.cn

[B02] 多分支 else if / elif
来源：http://vf.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://al.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ra.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xg.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rq.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bc.521024.cn

[B03] switch / match / case
来源：http://zx.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xr.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xb.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xv.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fu.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wf.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ij.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eb.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://la.szxytkj.cn

[B04] for 计数循环
来源：http://nh.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ef.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ks.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xk.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ni.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nn.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cw.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ij.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xw.521024.cn

[B05] 遍历数组 / 列表
来源：http://mt.nszjky.cn

Py:   for item in arr: print(item)
来源：http://vq.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fo.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ib.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xk.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ie.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://te.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://zj.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xy.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://mf.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kr.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://am.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ko.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cb.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jk.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yl.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yo.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://we.jctech888.com.cn

[B07] while 循环
来源：http://qr.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://mg.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ez.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://la.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://dd.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://pd.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://io.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://se.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://tb.521024.cn

[B08] do-while（至少执行一次）
来源：http://tr.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://rn.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tz.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://xe.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://kg.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ti.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uo.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wm.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ol.521024.cn

[B09] break 与 continue
来源：http://il.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bd.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bn.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ab.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ez.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zp.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://lg.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ar.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cs.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xa.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mj.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ts.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ad.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fu.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ye.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://ea.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://rf.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://kd.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uk.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nq.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pc.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tm.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://zr.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ag.jctech888.com.cn

[B12] 跳出多层循环
来源：http://ur.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ec.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ga.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zy.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uc.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ym.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tt.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gl.jctech888.com.cn


<!-- 参考信息 -->