代发 wailian999

Ruby: 42.to_s
来源：http://cp.jianghongdianzi.cn

C#:   42.ToString()
来源：http://ft.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://cp.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ua.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pi.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://io.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://os.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://em.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cj.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qf.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mf.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://cf.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ku.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jt.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nr.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ur.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qk.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rm.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nk.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hp.szxytkj.cn

[A10] 生成随机数
来源：http://id.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://jq.hahajie.cn

PHP:  random_int(1, 100);
来源：http://nh.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fr.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ko.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://vx.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pf.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://po.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://ai.521024.cn

[A11] 条件表达式（三元）
来源：http://vw.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://uh.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aj.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ld.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vw.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://bw.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pk.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vs.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jm.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://iy.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bu.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://do.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://jj.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://zx.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://rt.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ld.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://qj.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://ht.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ny.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://iu.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://mj.hahajie.cn

JS:   "第一行\n第二行"
来源：http://ji.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://bd.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ip.huanxung.cn

Go:   "第一行\n第二行"
来源：http://wm.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://xo.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://xv.szsharing.cn

[A14] 注释写法
来源：http://to.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uh.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zv.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://lc.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://eb.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xf.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://zj.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gt.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://lr.szsharing.cn

[A15] 空值判断与默认值
来源：http://cj.gzmigu.cn

Py:   value = data or "默认值"
来源：http://np.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://lx.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://qz.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://gw.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://va.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://bb.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://ht.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://fz.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ey.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mi.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ca.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ad.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://nw.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://st.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nh.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fj.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lj.shtwfgs.cn

[A17] 位运算
来源：http://sb.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gn.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uo.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wc.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nk.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://bm.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://ab.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://yf.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://va.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://sc.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eo.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://dt.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://cm.asd995.cn

[A19] 交换两个变量
来源：http://wy.shtwfgs.cn

Py:   a, b = b, a
来源：http://je.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dq.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://lh.521024.cn

TS:   [a, b] = [b, a];
来源：http://nq.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://jd.shxzukj.cn

Go:   a, b = b, a
来源：http://qa.asd995.cn

Ruby: a, b = b, a
来源：http://kd.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://dd.shxzukj.cn

[A20] 读取标准输入
来源：http://nw.hahajie.cn

Py:   name = input("请输入：")
来源：http://zj.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iw.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zr.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://ae.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://ys.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://er.colortex.cn

Ruby: gets.chomp
来源：http://or.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://fj.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://oh.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://ht.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dt.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://yf.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://ph.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://er.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gy.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://xk.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://sp.bjjhwx.cn

[A22] 获取字符串长度
来源：http://pl.huanxung.cn

Py:   len(s)
来源：http://iz.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rs.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yy.hahajie.cn

TS:   s.length
来源：http://ep.szsharing.cn

Java: s.length()
来源：http://nk.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://an.yuntaijiaju.cn

Ruby: s.length
来源：http://qb.szsharing.cn

C#:   s.Length
来源：http://sc.muxihuayi.cn

[A23] 大小写转换
来源：http://ky.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nu.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sm.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ih.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ix.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://np.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ir.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ir.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ik.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zx.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zh.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ul.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ny.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://su.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://mc.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qa.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://du.gzmigu.cn

[A25] 字符串比较
来源：http://jx.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://ja.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mu.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kt.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dh.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dg.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mq.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mn.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ko.huixiangedu.cn

[A26] 类型转换总览
来源：http://qk.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eg.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sz.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wa.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://ci.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qp.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://za.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gc.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nz.9csxet.cn

================================================================================
来源：http://zx.huanxung.cn

B. 流程控制
来源：http://fi.bookmarksfly.cn

================================================================================
来源：http://pn.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ft.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://st.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nf.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wa.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wb.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sg.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://be.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://om.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://wq.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nk.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vc.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sg.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mz.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uc.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://th.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gw.colortex.cn

[B03] switch / match / case
来源：http://cr.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sf.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kt.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://te.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lj.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cm.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://la.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kq.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vx.shxzukj.cn

[B04] for 计数循环
来源：http://sp.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://gx.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tf.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ka.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ua.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://be.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://wu.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yv.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://km.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://tb.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cv.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iw.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gs.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tm.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zh.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://zj.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sv.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://rd.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ny.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jp.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qm.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fh.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ie.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wv.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ok.shxzskj.cn

[B07] while 循环
来源：http://rs.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://bn.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://th.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://ef.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ho.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://hq.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dr.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://xh.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://cl.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://lu.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://wj.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uk.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://yy.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://tf.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://gb.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://br.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yx.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://me.yuexingan06.cn

[B09] break 与 continue
来源：http://wc.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dg.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ie.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://de.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yp.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mx.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.nszjky.cn

[B10] 遍历同时拿索引
来源：http://cr.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ow.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gb.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xd.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hv.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ae.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://og.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ys.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://jb.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://qc.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://yr.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mi.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kh.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eg.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kk.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://bi.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tv.yuexingan06.cn

[B12] 跳出多层循环
来源：http://qw.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ge.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vb.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qb.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ab.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://in.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iz.shtwfgs.cn

[B13] 判断是否为数字
来源：http://dg.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://md.hahajie.cn

PHP:  is_numeric($x)
来源：http://zm.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kd.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zi.asd995.cn

Java: x instanceof Number
来源：http://hk.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fj.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://wt.colortex.cn

C#:   x is int or double or decimal
来源：http://ho.nicolike.cn

[B14] 判断值是否在集合内
来源：http://dk.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rp.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fc.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://aw.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://uo.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wb.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mk.hnjuh.cn


<!-- 参考信息 -->