代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://cr.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jf.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uf.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uz.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jw.yuexingan06.cn

[A07] 数字转字符串
来源：http://lb.newstarts.cn

Py:   str(42)
来源：http://hw.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://gz.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://xb.shxzukj.cn

TS:   String(42)
来源：http://ob.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fr.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://qe.shxzskj.cn

Ruby: 42.to_s
来源：http://mu.gzmigu.cn

C#:   42.ToString()
来源：http://eq.szxytkj.cn

[A08] 取整与四舍五入
来源：http://km.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lq.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://te.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fi.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ej.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ut.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://op.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zx.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pu.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://xu.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cf.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vb.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nj.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ai.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lu.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nb.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://do.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ci.hnjuh.cn

[A10] 生成随机数
来源：http://zf.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://qz.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://em.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hk.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dj.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://ij.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ba.lnxyls.cn

Ruby: rand(1..100)
来源：http://lk.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://fh.nszjky.cn

[A11] 条件表达式（三元）
来源：http://tv.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://qa.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ap.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cd.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sy.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://zv.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wn.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rm.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xc.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://hw.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://of.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gu.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://fh.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://ke.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://xe.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ca.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://hj.asd995.cn

C#:   $"Hello, {name}!"
来源：http://ob.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dc.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://il.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://sm.colortex.cn

JS:   "第一行\n第二行"
来源：http://bg.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://tv.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://qs.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://zl.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://yg.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://zj.shtwfgs.cn

[A14] 注释写法
来源：http://zd.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pj.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zg.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ot.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://bd.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pi.521024.cn

Go:   // 单行；/* 多行 */
来源：http://hl.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://us.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ph.hahajie.cn

[A15] 空值判断与默认值
来源：http://ds.szsharing.cn

Py:   value = data or "默认值"
来源：http://ct.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://yy.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ht.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://wp.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nf.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://yk.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://in.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://dm.hnjuh.cn

[A16] 真假值判断规则
来源：http://of.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://te.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pu.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ik.shxzskj.cn

TS:   if (!x) {}
来源：http://vw.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hj.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fl.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://po.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fp.newstarts.cn

[A17] 位运算
来源：http://dp.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zk.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pf.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zy.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gi.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sy.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://fk.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://yk.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://oh.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hv.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fh.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://ou.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zc.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://sk.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://xe.muxihuayi.cn

[A19] 交换两个变量
来源：http://uo.huanxung.cn

Py:   a, b = b, a
来源：http://yo.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gg.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://xm.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://eb.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://yr.huixiangedu.cn

Go:   a, b = b, a
来源：http://ej.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://na.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://jn.yuexingan06.cn

[A20] 读取标准输入
来源：http://zk.panjiajie.cn

Py:   name = input("请输入：")
来源：http://sd.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bn.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yh.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://cg.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://bp.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eg.wgjwhj.cn

Ruby: gets.chomp
来源：http://aw.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://hd.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ej.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zs.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://wl.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://lc.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://nn.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hd.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://qm.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://fy.panjiajie.cn

[A22] 获取字符串长度
来源：http://tl.521024.cn

Py:   len(s)
来源：http://ds.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fc.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nz.hahajie.cn

TS:   s.length
来源：http://uz.bookmarksfly.cn

Java: s.length()
来源：http://ct.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dn.yuexingan06.cn

Ruby: s.length
来源：http://nm.bookmarksfly.cn

C#:   s.Length
来源：http://ef.9csxet.cn

[A23] 大小写转换
来源：http://gz.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oe.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vj.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tt.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ty.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fj.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bl.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lz.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://zw.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dg.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://im.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jb.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ax.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lv.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://pb.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://od.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fb.colortex.cn

[A25] 字符串比较
来源：http://wq.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://ni.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hl.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fl.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://al.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qe.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vx.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rk.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ta.huixiangedu.cn

[A26] 类型转换总览
来源：http://hb.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mq.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qd.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yr.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://bt.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ao.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mf.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fm.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yt.haigaiapp.cn

================================================================================
来源：http://rs.jianghongdianzi.cn

B. 流程控制
来源：http://ew.521024.cn

================================================================================
来源：http://qv.nszjky.cn

[B01] 条件判断 if / else
来源：http://yg.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wp.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wb.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dq.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ss.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vy.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qj.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mj.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vj.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://ii.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yo.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jo.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sd.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bg.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://de.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.chemitech.net.cn

[B03] switch / match / case
来源：http://uf.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://up.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bl.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rx.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ls.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yk.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rz.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ua.yuntaijiaju.cn

[B04] for 计数循环
来源：http://za.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://qf.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://og.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qk.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lh.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ag.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ru.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://zv.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cs.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://vl.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://wt.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://he.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vs.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zr.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eg.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://fa.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pl.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://in.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jl.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yu.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gv.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xp.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xm.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ct.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nt.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pl.huixinmuqiang.cn

[B07] while 循环
来源：http://th.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://qh.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wv.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://wn.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://yp.521024.cn

Java: while (i < 10) { i++; }
来源：http://bj.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rz.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ia.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://qw.521024.cn

[B08] do-while（至少执行一次）
来源：http://cn.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://nt.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zg.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://as.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://kt.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://ao.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mx.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gq.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://rt.nicolike.cn

[B09] break 与 continue
来源：http://ee.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ay.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rn.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rg.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hk.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mr.newstarts.cn

[B10] 遍历同时拿索引
来源：http://rs.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dv.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sx.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dk.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tm.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wy.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ed.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fp.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lp.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://xx.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://xc.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://iq.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qy.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bj.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vn.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kd.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://du.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bv.panjiajie.cn

[B12] 跳出多层循环
来源：http://wn.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://it.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xt.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fe.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wt.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bs.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tt.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xk.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cu.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ok.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://ge.asd995.cn

PHP:  is_numeric($x)
来源：http://oz.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eg.huanxung.cn


<!-- 参考信息 -->