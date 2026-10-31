代发 wailian999

JS:   String(42); (42).toString()
来源：http://jr.huixinmuqiang.cn

TS:   String(42)
来源：http://iy.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dh.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://dw.chemitech.net.cn

Ruby: 42.to_s
来源：http://sv.huanxung.cn

C#:   42.ToString()
来源：http://mh.9csxet.cn

[A08] 取整与四舍五入
来源：http://lh.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ch.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bm.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://og.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://do.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ba.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cw.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jz.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ll.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://rk.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pg.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lu.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cn.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qc.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vp.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cg.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tl.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jc.bjjhwx.cn

[A10] 生成随机数
来源：http://ok.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://uv.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://hm.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://du.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fa.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://hj.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hd.chemitech.net.cn

Ruby: rand(1..100)
来源：http://jt.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://ab.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://ng.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://um.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jt.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ft.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://my.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ja.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fu.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sa.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fx.521024.cn

[A12] 字符串插值 / 格式化
来源：http://gw.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fh.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mf.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://rm.colortex.cn

TS:   `Hello, ${name}!`
来源：http://me.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://lp.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wb.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://fp.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ap.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qr.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://dp.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://di.asd995.cn

JS:   "第一行\n第二行"
来源：http://ab.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://eo.colortex.cn

Java: "第一行\n第二行"
来源：http://ku.huanxung.cn

Go:   "第一行\n第二行"
来源：http://gy.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://ij.hahajie.cn

C#:   "第一行\n第二行"
来源：http://wj.hahajie.cn

[A14] 注释写法
来源：http://vu.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gh.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zv.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://dj.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://tx.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ca.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://yk.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fg.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://hl.shxzskj.cn

[A15] 空值判断与默认值
来源：http://tc.newstarts.cn

Py:   value = data or "默认值"
来源：http://lz.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://el.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://tu.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://vy.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xz.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://mf.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://hq.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://gv.szsharing.cn

[A16] 真假值判断规则
来源：http://os.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yg.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lo.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wz.jctech888.com.cn

TS:   if (!x) {}
来源：http://dz.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://it.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sq.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sb.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lt.nicolike.cn

[A17] 位运算
来源：http://ah.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gd.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wc.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://an.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gx.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zf.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ak.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://na.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://tz.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://df.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sv.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wi.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://gq.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rc.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://zt.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://vu.9csxet.cn

[A19] 交换两个变量
来源：http://lg.huixiangedu.cn

Py:   a, b = b, a
来源：http://gz.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ot.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://hz.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://bn.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://vd.muxihuayi.cn

Go:   a, b = b, a
来源：http://rl.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ib.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://fi.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://nq.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://gx.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zw.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sm.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ea.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://ay.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ue.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://wf.shxzskj.cn

C#:   Console.ReadLine();
来源：http://oz.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://sf.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://bz.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://au.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://hn.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://lz.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://ci.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ld.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://lu.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://mm.nicolike.cn

[A22] 获取字符串长度
来源：http://se.colortex.cn

Py:   len(s)
来源：http://zf.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sk.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cg.szxytkj.cn

TS:   s.length
来源：http://ul.shxzskj.cn

Java: s.length()
来源：http://oo.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sk.huixiangedu.cn

Ruby: s.length
来源：http://ik.huixinmuqiang.cn

C#:   s.Length
来源：http://dw.521024.cn

[A23] 大小写转换
来源：http://jm.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bq.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zd.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gu.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zg.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sg.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ph.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rt.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://di.huixiangedu.cn

[A24] 去除首尾空白
来源：http://pt.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cw.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zg.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xe.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ny.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://az.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://fu.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vk.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://km.szxytkj.cn

[A25] 字符串比较
来源：http://pz.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://fw.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bn.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dr.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://so.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lc.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ml.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kx.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pr.hahajie.cn

[A26] 类型转换总览
来源：http://dz.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tu.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rf.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bg.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://hl.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ph.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rk.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ci.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jm.asd995.cn

================================================================================
来源：http://em.9csxet.cn

B. 流程控制
来源：http://cr.shxzukj.cn

================================================================================
来源：http://fa.asd995.cn

[B01] 条件判断 if / else
来源：http://ei.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zt.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ao.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://al.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tt.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vw.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://my.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ic.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wl.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://gy.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ku.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hw.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kc.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xs.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fy.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vp.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jc.bjjhwx.cn

[B03] switch / match / case
来源：http://zw.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hs.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://it.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ye.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ov.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kk.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nm.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yh.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xz.shxzskj.cn

[B04] for 计数循环
来源：http://dx.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://kh.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vq.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yk.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pt.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gc.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tc.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ep.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vx.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://ic.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://ng.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jj.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rl.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pq.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hm.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bw.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://qy.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jc.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://nt.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mf.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://de.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cf.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yf.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hq.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ez.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://db.chemitech.net.cn

[B07] while 循环
来源：http://kl.colortex.cn

Py:   while i < 10: i += 1
来源：http://ww.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vd.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://yt.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://kj.521024.cn

Java: while (i < 10) { i++; }
来源：http://wt.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ur.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://vs.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://or.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://fn.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://xo.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sb.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://mc.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ap.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://gr.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tx.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://to.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://cx.hahajie.cn

[B09] break 与 continue
来源：http://hk.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://py.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qs.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hp.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ca.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://my.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://da.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ng.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wx.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wv.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pc.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ax.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ay.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qj.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://on.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gx.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://ap.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ye.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ag.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qn.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sn.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cr.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wf.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://wm.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vy.szxytkj.cn

[B12] 跳出多层循环
来源：http://uz.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mq.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ls.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ko.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bw.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eb.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://so.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://na.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nx.hnjuh.cn

[B13] 判断是否为数字
来源：http://ef.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://al.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://lt.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://id.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eo.gzmigu.cn

Java: x instanceof Number
来源：http://fw.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ql.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://zo.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ts.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://zn.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://um.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wh.yuntaijiaju.cn


<!-- 参考信息 -->