代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://ri.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jo.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://yl.shtwfgs.cn

[A05] 整数除法与取模
来源：http://gk.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ql.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bv.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ng.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://as.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://gn.521024.cn

Go:   7 / 2; 7 % 2
来源：http://rn.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://gu.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://mh.newstarts.cn

[A06] 字符串转数字
来源：http://vg.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://re.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ez.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pc.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rz.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wu.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ko.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zp.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kf.huanxung.cn

[A07] 数字转字符串
来源：http://pf.bjjhwx.cn

Py:   str(42)
来源：http://do.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://vp.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://gi.jianghongdianzi.cn

TS:   String(42)
来源：http://hr.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zb.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://br.hnjuh.cn

Ruby: 42.to_s
来源：http://bw.hahajie.cn

C#:   42.ToString()
来源：http://qx.newstarts.cn

[A08] 取整与四舍五入
来源：http://rg.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://op.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bd.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qh.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sn.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hk.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://km.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sy.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://of.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://hr.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uf.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iy.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gu.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nz.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sx.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zl.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lp.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qg.huixiangedu.cn

[A10] 生成随机数
来源：http://li.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ui.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://kf.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nq.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lx.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://hg.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zb.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://xh.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://mo.asd995.cn

[A11] 条件表达式（三元）
来源：http://kg.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://dn.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qr.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kz.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gm.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://xt.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jz.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gx.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://is.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://tf.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dk.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fk.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://ei.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://dt.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://rc.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://an.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://cs.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://nb.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zo.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://hh.521024.cn

PHP:  "第一行\n第二行"
来源：http://rp.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://mj.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://ci.huanxung.cn

Java: "第一行\n第二行"
来源：http://tq.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://pb.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://sc.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ir.muxihuayi.cn

[A14] 注释写法
来源：http://vt.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ij.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wk.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://as.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://uu.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bw.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://zr.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lo.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://ps.shxzskj.cn

[A15] 空值判断与默认值
来源：http://ij.9csxet.cn

Py:   value = data or "默认值"
来源：http://pd.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://wc.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://yq.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://fc.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rg.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://za.nszjky.cn

Ruby: value = data || "默认值"
来源：http://rl.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://za.nszjky.cn

[A16] 真假值判断规则
来源：http://ec.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fx.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ie.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jg.asd995.cn

TS:   if (!x) {}
来源：http://he.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bd.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cq.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://es.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tg.9csxet.cn

[A17] 位运算
来源：http://pl.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://do.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ng.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mt.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ql.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fp.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wq.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qb.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fa.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://pj.colortex.cn

Py:   ord("A"); chr(65)
来源：http://yp.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://lq.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cs.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://rt.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lx.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://uh.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://tz.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://sp.newstarts.cn

Py:   a, b = b, a
来源：http://mp.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wm.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://ts.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://hf.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://ya.jctech888.com.cn

Go:   a, b = b, a
来源：http://er.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://jt.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://sy.huixiangedu.cn

[A20] 读取标准输入
来源：http://lw.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://ig.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qb.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qd.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://uo.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://kn.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hq.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://im.shxzskj.cn

C#:   Console.ReadLine();
来源：http://ly.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://qt.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://pg.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://av.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://lo.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://wg.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://pp.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qh.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://rw.521024.cn

C#:   3.14159.ToString("F2")
来源：http://jz.szxytkj.cn

[A22] 获取字符串长度
来源：http://ot.panjiajie.cn

Py:   len(s)
来源：http://az.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fo.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iq.bjjhwx.cn

TS:   s.length
来源：http://jl.jianghongdianzi.cn

Java: s.length()
来源：http://mq.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://np.hahajie.cn

Ruby: s.length
来源：http://ji.hahajie.cn

C#:   s.Length
来源：http://zi.yuexingan06.cn

[A23] 大小写转换
来源：http://zd.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ok.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wb.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ou.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ec.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dt.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rf.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ge.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gi.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://lr.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ib.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kg.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rs.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aa.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gu.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://kd.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://je.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://id.newstarts.cn

[A25] 字符串比较
来源：http://ck.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://pv.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ml.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jr.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ai.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ay.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sl.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ps.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bb.nicolike.cn

[A26] 类型转换总览
来源：http://di.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rn.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wj.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mr.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://hd.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ec.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ip.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://za.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hq.lnxyls.cn

================================================================================
来源：http://mv.shxzskj.cn

B. 流程控制
来源：http://vl.huanxung.cn

================================================================================
来源：http://km.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://bl.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lg.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mr.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wx.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dk.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jm.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ok.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://my.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://qp.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gr.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cy.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oe.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://va.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://so.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.yuexingan06.cn

[B03] switch / match / case
来源：http://mx.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ja.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gy.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wz.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ko.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ar.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ah.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yi.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ig.hnjuh.cn

[B04] for 计数循环
来源：http://nw.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://wh.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rq.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xk.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://to.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yc.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://nn.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ud.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://or.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://lz.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ih.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fm.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ju.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zq.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dn.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://ol.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xw.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://tr.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iy.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ru.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dm.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aa.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ts.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sk.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ic.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kr.shxzukj.cn

[B07] while 循环
来源：http://ia.huanxung.cn

Py:   while i < 10: i += 1
来源：http://zj.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://os.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://hl.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://qr.colortex.cn

Java: while (i < 10) { i++; }
来源：http://iu.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bu.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://mi.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://sm.asd995.cn

[B08] do-while（至少执行一次）
来源：http://wn.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://ey.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sm.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://hs.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://vl.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://tv.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://co.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wm.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://jl.muxihuayi.cn

[B09] break 与 continue
来源：http://lz.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ah.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://la.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ci.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://su.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mg.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ju.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://id.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://us.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cp.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cb.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xi.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lh.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cr.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zm.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://th.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://wy.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://yp.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://lv.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pw.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dd.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gh.colortex.cn


<!-- 参考信息 -->