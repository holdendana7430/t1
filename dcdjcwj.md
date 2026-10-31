代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ce.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zs.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gy.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kf.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ic.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://wq.nicolike.cn

Py:   str(42)
来源：http://sy.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://um.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://rs.9csxet.cn

TS:   String(42)
来源：http://qg.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ua.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://ep.asd995.cn

Ruby: 42.to_s
来源：http://qf.huixiangedu.cn

C#:   42.ToString()
来源：http://jf.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://fm.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xr.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hy.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wq.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dp.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ga.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kp.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qu.colortex.cn

[A09] 绝对值与最大最小值
来源：http://wl.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gb.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fp.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xe.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ze.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dp.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tt.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wd.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://us.nszjky.cn

[A10] 生成随机数
来源：http://nr.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://mo.huanxung.cn

PHP:  random_int(1, 100);
来源：http://db.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sm.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fa.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://rf.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hx.szsharing.cn

Ruby: rand(1..100)
来源：http://vg.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://bf.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://vv.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://cd.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lo.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ot.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zr.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://xo.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cw.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dr.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ch.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://df.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hj.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zm.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://aa.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ul.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://sb.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://up.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://pp.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://zl.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hx.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://br.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://of.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://kb.hahajie.cn

TS:   "第一行\n第二行"
来源：http://qw.shxzskj.cn

Java: "第一行\n第二行"
来源：http://pv.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://hq.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://ux.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://na.szxytkj.cn

[A14] 注释写法
来源：http://qq.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dk.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yy.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://fa.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://fm.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nz.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://za.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ji.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://iy.9csxet.cn

[A15] 空值判断与默认值
来源：http://gr.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ar.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://eo.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ra.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://ep.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aa.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://kg.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://er.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://gh.muxihuayi.cn

[A16] 真假值判断规则
来源：http://ae.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ab.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://he.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fl.shxzskj.cn

TS:   if (!x) {}
来源：http://bo.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yf.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fk.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pr.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zu.521024.cn

[A17] 位运算
来源：http://lq.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ij.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xv.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://al.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ay.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ut.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jb.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dn.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://rz.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://la.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://iw.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zh.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gr.521024.cn

Java: (int) 'A'; (char) 65
来源：http://qh.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dr.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://ef.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://yc.newstarts.cn

[A19] 交换两个变量
来源：http://yk.9csxet.cn

Py:   a, b = b, a
来源：http://ab.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dt.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://nu.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://ij.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://in.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://ji.9csxet.cn

Ruby: a, b = b, a
来源：http://ot.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://bl.colortex.cn

[A20] 读取标准输入
来源：http://ji.colortex.cn

Py:   name = input("请输入：")
来源：http://ua.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cf.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jv.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://ni.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://zz.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://se.nicolike.cn

Ruby: gets.chomp
来源：http://xj.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://il.9csxet.cn

[A21] 保留指定小数位输出
来源：http://pn.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://zo.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ds.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://qp.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://re.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://jt.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oc.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ek.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://js.nszjky.cn

[A22] 获取字符串长度
来源：http://ov.chemitech.net.cn

Py:   len(s)
来源：http://ud.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cu.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oz.haigaiapp.cn

TS:   s.length
来源：http://oq.jctech888.com.cn

Java: s.length()
来源：http://wd.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ju.shtwfgs.cn

Ruby: s.length
来源：http://bg.nicolike.cn

C#:   s.Length
来源：http://kf.gzmigu.cn

[A23] 大小写转换
来源：http://ww.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ia.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://va.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lx.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://li.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://au.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://et.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dp.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jr.nicolike.cn

[A24] 去除首尾空白
来源：http://wx.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cv.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sy.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://la.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ip.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yq.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://wa.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wk.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dt.hnjuh.cn

[A25] 字符串比较
来源：http://ua.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://sx.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gv.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ll.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ma.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mn.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qp.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iy.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cf.shtwfgs.cn

[A26] 类型转换总览
来源：http://lb.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tv.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ah.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mm.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://gx.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rx.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://db.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ji.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ba.panjiajie.cn

================================================================================
来源：http://qq.nicolike.cn

B. 流程控制
来源：http://gg.521024.cn

================================================================================
来源：http://qy.szxytkj.cn

[B01] 条件判断 if / else
来源：http://vj.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://af.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ez.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lc.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cn.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kn.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fy.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qf.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://or.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://vb.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hs.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nt.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tc.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://it.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wx.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.wgjwhj.cn

[B03] switch / match / case
来源：http://mh.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bs.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lj.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://co.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fh.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vt.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ze.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rv.gzmigu.cn

[B04] for 计数循环
来源：http://nn.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ss.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bg.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xb.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dy.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fk.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://bb.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lz.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://yb.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ww.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nm.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ex.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rd.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rd.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jq.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://uk.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lj.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://pe.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xi.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pa.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ph.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ks.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rp.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://av.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wu.521024.cn

[B07] while 循环
来源：http://ga.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://bz.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://rb.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://er.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://dp.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ks.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://im.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://wo.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://es.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ir.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qo.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://wj.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://re.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://nj.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ho.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://un.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://kx.yuntaijiaju.cn

[B09] break 与 continue
来源：http://va.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wa.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://la.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tq.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dz.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://id.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gy.nicolike.cn

[B10] 遍历同时拿索引
来源：http://ox.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ln.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sp.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mm.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ns.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qz.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://il.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eg.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sf.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://ix.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://yv.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://yj.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bt.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eo.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lh.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://np.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tg.haigaiapp.cn

[B12] 跳出多层循环
来源：http://nd.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pr.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sk.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pf.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qj.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cn.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bl.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sq.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zb.haigaiapp.cn

[B13] 判断是否为数字
来源：http://kt.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ea.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://aw.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ht.huanxung.cn


<!-- 参考信息 -->