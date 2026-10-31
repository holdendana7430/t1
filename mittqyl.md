代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cn.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iw.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ew.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ze.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://do.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://bl.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://mz.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://hw.chemitech.net.cn

[A06] 字符串转数字
来源：http://pj.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://nh.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gm.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hc.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xb.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wo.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ty.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bo.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jj.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://eh.colortex.cn

Py:   str(42)
来源：http://fm.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://ol.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://so.huanxung.cn

TS:   String(42)
来源：http://zh.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cq.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://mq.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://mu.huixiangedu.cn

C#:   42.ToString()
来源：http://ij.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ey.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yu.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kr.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zo.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gg.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tv.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nu.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hq.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rc.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://ac.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gr.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ep.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ku.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rk.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ky.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hd.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bc.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://at.szxytkj.cn

[A10] 生成随机数
来源：http://fk.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://jn.newstarts.cn

PHP:  random_int(1, 100);
来源：http://hx.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dr.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fz.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://oo.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sx.huixiangedu.cn

Ruby: rand(1..100)
来源：http://xo.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://pt.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://tl.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tm.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ky.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qf.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gm.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://sg.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kb.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qp.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iw.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://br.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tp.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yd.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://xt.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ug.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://dx.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jn.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ds.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://nr.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://om.huanxung.cn

Py:   "第一行\n第二行"
来源：http://ij.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://nh.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://wz.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://uo.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://jf.9csxet.cn

Go:   "第一行\n第二行"
来源：http://ss.colortex.cn

Ruby: "第一行\n第二行"
来源：http://wh.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://zk.yuexingan06.cn

[A14] 注释写法
来源：http://jz.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bi.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lx.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://gp.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://bx.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xc.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://cz.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vc.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://jr.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://rt.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://qz.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://fr.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://eg.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://ds.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nm.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://fi.9csxet.cn

Ruby: value = data || "默认值"
来源：http://pf.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://nd.521024.cn

[A16] 真假值判断规则
来源：http://hk.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jc.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ic.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rx.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://xy.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wv.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vu.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cx.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ul.bookmarksfly.cn

[A17] 位运算
来源：http://rn.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ig.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vv.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tn.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://so.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jx.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gj.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ex.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://tf.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://yb.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://vd.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mr.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bc.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://xs.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yd.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://vg.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://pk.shtwfgs.cn

[A19] 交换两个变量
来源：http://rt.nszjky.cn

Py:   a, b = b, a
来源：http://qm.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://od.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://ri.asd995.cn

TS:   [a, b] = [b, a];
来源：http://uz.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://di.muxihuayi.cn

Go:   a, b = b, a
来源：http://ax.newstarts.cn

Ruby: a, b = b, a
来源：http://zv.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://uo.shxzskj.cn

[A20] 读取标准输入
来源：http://ol.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://fn.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zt.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://go.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://gz.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://sm.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qm.wgjwhj.cn

Ruby: gets.chomp
来源：http://we.hahajie.cn

C#:   Console.ReadLine();
来源：http://ir.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://hx.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://cj.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://us.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://hl.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://iq.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://lc.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qx.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://le.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://pa.9csxet.cn

[A22] 获取字符串长度
来源：http://rr.nszjky.cn

Py:   len(s)
来源：http://vm.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iz.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hq.huanxung.cn

TS:   s.length
来源：http://ua.hnjuh.cn

Java: s.length()
来源：http://ps.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://on.shtwfgs.cn

Ruby: s.length
来源：http://aj.jctech888.com.cn

C#:   s.Length
来源：http://jg.chemitech.net.cn

[A23] 大小写转换
来源：http://tr.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iy.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mw.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://le.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zf.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cs.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pt.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zi.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nq.lnxyls.cn

[A24] 去除首尾空白
来源：http://fd.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xz.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wd.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sc.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dv.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kx.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://st.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bg.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://it.chemitech.net.cn

[A25] 字符串比较
来源：http://pd.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://rl.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gx.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hd.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cy.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://po.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ag.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vz.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://db.shxzskj.cn

[A26] 类型转换总览
来源：http://ms.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ho.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pu.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vs.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://qp.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ln.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mc.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pb.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jj.panjiajie.cn

================================================================================
来源：http://gc.yuexingan06.cn

B. 流程控制
来源：http://wj.shxzskj.cn

================================================================================
来源：http://yr.colortex.cn

[B01] 条件判断 if / else
来源：http://cl.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dn.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mx.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://du.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yo.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wl.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eg.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fv.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uy.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://pd.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lw.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hi.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kt.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ak.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://za.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vi.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dk.bjjhwx.cn

[B03] switch / match / case
来源：http://sn.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ss.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://im.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pw.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ze.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pn.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xg.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tj.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ji.hnjuh.cn

[B04] for 计数循环
来源：http://pq.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://fk.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://no.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xn.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wd.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zz.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pe.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ki.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ff.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://mo.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ys.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dx.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jk.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ul.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yb.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zn.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://fb.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wg.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://iw.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ha.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mq.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tc.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yf.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rt.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ua.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rw.521024.cn

[B07] while 循环
来源：http://uh.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://sx.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lm.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://on.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://md.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://qr.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rw.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://na.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://qh.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://cr.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ai.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://or.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://tf.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ih.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://rk.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pc.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mz.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://pq.shxzukj.cn

[B09] break 与 continue
来源：http://yj.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ve.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rh.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mh.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jh.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tt.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gi.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://oj.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tc.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uk.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bt.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ks.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gx.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://do.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://os.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zv.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://fn.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://lh.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://df.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lm.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mp.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dm.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oy.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://kf.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uc.shxzskj.cn

[B12] 跳出多层循环
来源：http://wn.jctech888.com.cn


<!-- 参考信息 -->