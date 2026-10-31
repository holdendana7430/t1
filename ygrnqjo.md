代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://sn.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jq.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://fu.hahajie.cn

[A05] 整数除法与取模
来源：http://ep.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gv.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ue.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://am.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wp.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://bs.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://vj.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://rs.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://wz.panjiajie.cn

[A06] 字符串转数字
来源：http://fc.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://wl.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ch.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hb.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hy.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tu.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://av.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mn.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jt.hahajie.cn

[A07] 数字转字符串
来源：http://fh.yuexingan06.cn

Py:   str(42)
来源：http://fl.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://hn.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://gq.colortex.cn

TS:   String(42)
来源：http://oe.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://us.colortex.cn

Go:   strconv.Itoa(42)
来源：http://tz.wgjwhj.cn

Ruby: 42.to_s
来源：http://du.jctech888.com.cn

C#:   42.ToString()
来源：http://ll.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://wp.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wq.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mt.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fw.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lh.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ff.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ry.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://li.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bf.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://aw.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xi.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hh.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xc.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kp.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cr.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kh.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mn.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hw.huixinmuqiang.cn

[A10] 生成随机数
来源：http://tf.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://sb.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://go.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ps.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tm.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://gg.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xa.huanxung.cn

Ruby: rand(1..100)
来源：http://wt.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://rw.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://ie.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://le.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ai.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xz.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tn.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://ib.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lm.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fe.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mj.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://jz.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pm.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lc.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://js.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://da.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://gw.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jn.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://lq.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://tq.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://db.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://zv.521024.cn

PHP:  "第一行\n第二行"
来源：http://zp.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://dq.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://bp.szsharing.cn

Java: "第一行\n第二行"
来源：http://cg.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ap.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://ki.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://fi.yuexingan06.cn

[A14] 注释写法
来源：http://ig.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yr.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ep.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://fh.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://kh.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nu.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://lq.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mi.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://sr.colortex.cn

[A15] 空值判断与默认值
来源：http://da.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://ei.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://ht.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://np.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://sb.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ef.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://na.huanxung.cn

Ruby: value = data || "默认值"
来源：http://vy.521024.cn

C#:   var value = data ?? "默认值";
来源：http://rh.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://ob.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://un.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uh.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jh.521024.cn

TS:   if (!x) {}
来源：http://rq.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wv.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qe.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ya.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sh.hahajie.cn

[A17] 位运算
来源：http://ku.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yo.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kh.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wb.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ao.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iv.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jk.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://to.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rq.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://ta.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://me.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://zm.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vt.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://vt.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zd.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://xe.asd995.cn

C#:   (int)'A'; (char)65
来源：http://nz.shtwfgs.cn

[A19] 交换两个变量
来源：http://ij.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://uz.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vg.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://bo.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://gm.521024.cn

Java: int t = a; a = b; b = t;
来源：http://tn.haigaiapp.cn

Go:   a, b = b, a
来源：http://yx.shxzukj.cn

Ruby: a, b = b, a
来源：http://jk.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://sq.9csxet.cn

[A20] 读取标准输入
来源：http://fz.521024.cn

Py:   name = input("请输入：")
来源：http://tj.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://do.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cr.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://gp.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://qt.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://os.asd995.cn

Ruby: gets.chomp
来源：http://xv.hnjuh.cn

C#:   Console.ReadLine();
来源：http://vl.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://vh.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://dx.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pb.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://si.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://qf.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ct.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://da.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://rk.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://eg.521024.cn

[A22] 获取字符串长度
来源：http://zz.huixinmuqiang.cn

Py:   len(s)
来源：http://ao.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wv.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eg.szxytkj.cn

TS:   s.length
来源：http://de.jctech888.com.cn

Java: s.length()
来源：http://tv.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rw.lnxyls.cn

Ruby: s.length
来源：http://gj.shxzskj.cn

C#:   s.Length
来源：http://jr.wgjwhj.cn

[A23] 大小写转换
来源：http://eo.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://le.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uv.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wn.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kc.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ed.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://on.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vo.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oi.nicolike.cn

[A24] 去除首尾空白
来源：http://fb.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ha.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nf.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://or.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vx.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://br.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://qp.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sn.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sc.wgjwhj.cn

[A25] 字符串比较
来源：http://cf.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://lj.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://js.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qm.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ph.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://re.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zs.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://en.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xz.shtwfgs.cn

[A26] 类型转换总览
来源：http://cc.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gq.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dv.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sk.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://cu.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oe.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pu.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vy.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cw.huanxung.cn

================================================================================
来源：http://mg.muxihuayi.cn

B. 流程控制
来源：http://jf.asd995.cn

================================================================================
来源：http://cc.nszjky.cn

[B01] 条件判断 if / else
来源：http://bm.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dj.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xv.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sq.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hu.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lm.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tg.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qy.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rc.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://fg.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rq.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://je.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rx.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pw.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jc.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://za.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.shtwfgs.cn

[B03] switch / match / case
来源：http://fn.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://io.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fb.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wn.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kf.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uh.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qb.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lz.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bt.panjiajie.cn

[B04] for 计数循环
来源：http://gu.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ye.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ht.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ib.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ko.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wc.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://zs.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uw.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://xs.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://hd.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kx.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mf.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rt.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yu.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lj.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://gn.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nl.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://qr.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uk.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://an.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ge.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cs.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pf.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lq.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ti.szxytkj.cn

[B07] while 循环
来源：http://ne.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://xk.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ya.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://zt.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://pz.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://vl.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eo.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://db.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://cb.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://uv.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://xn.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pn.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://uj.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://io.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://mb.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xz.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tj.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ld.hahajie.cn

[B09] break 与 continue
来源：http://gt.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ax.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ay.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://th.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tj.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gb.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uh.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dk.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://bk.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nz.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://im.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nz.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ww.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ss.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mg.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zx.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gl.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://sw.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://zr.asd995.cn

PHP:  range(0, 10, 2);
来源：http://hv.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mg.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lp.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qp.nicolike.cn


<!-- 参考信息 -->