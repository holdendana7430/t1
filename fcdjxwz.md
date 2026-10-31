代发 wailian999

JS:   String(42); (42).toString()
来源：http://pn.muxihuayi.cn

TS:   String(42)
来源：http://fo.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vg.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://aj.shtwfgs.cn

Ruby: 42.to_s
来源：http://sz.jctech888.com.cn

C#:   42.ToString()
来源：http://mt.hahajie.cn

[A08] 取整与四舍五入
来源：http://vq.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gl.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ri.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dg.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rx.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ao.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oj.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wd.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rx.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://wz.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tc.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zz.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xc.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://un.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ss.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vw.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lr.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://be.jctech888.com.cn

[A10] 生成随机数
来源：http://vd.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://il.nszjky.cn

PHP:  random_int(1, 100);
来源：http://ix.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://er.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dm.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://ie.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fs.shxzskj.cn

Ruby: rand(1..100)
来源：http://zf.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://tr.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://pf.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://vq.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vl.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rx.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bh.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://fw.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zn.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ub.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ao.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://xj.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://za.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jv.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://is.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ru.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://zh.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dt.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://pr.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://ew.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cx.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://re.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://bf.9csxet.cn

JS:   "第一行\n第二行"
来源：http://rs.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://si.521024.cn

Java: "第一行\n第二行"
来源：http://mn.hahajie.cn

Go:   "第一行\n第二行"
来源：http://gp.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://fv.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://hz.nszjky.cn

[A14] 注释写法
来源：http://ov.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ak.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hw.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://oz.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://be.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bo.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://ls.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://il.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://pz.asd995.cn

[A15] 空值判断与默认值
来源：http://tv.colortex.cn

Py:   value = data or "默认值"
来源：http://lh.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://lh.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://so.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://gz.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yt.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://mt.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://li.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://sh.huanxung.cn

[A16] 真假值判断规则
来源：http://au.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eg.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qk.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ih.huixiangedu.cn

TS:   if (!x) {}
来源：http://uk.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mn.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jy.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gz.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pr.yuntaijiaju.cn

[A17] 位运算
来源：http://mz.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cz.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bx.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vs.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iq.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://li.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xi.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://cp.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://af.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://gz.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://in.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://vd.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yf.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://ja.colortex.cn

C#:   (int)'A'; (char)65
来源：http://mp.hahajie.cn

[A19] 交换两个变量
来源：http://cs.colortex.cn

Py:   a, b = b, a
来源：http://rh.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zp.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://gn.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://cc.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://an.huanxung.cn

Go:   a, b = b, a
来源：http://lu.panjiajie.cn

Ruby: a, b = b, a
来源：http://ng.521024.cn

C#:   (a, b) = (b, a);
来源：http://wv.newstarts.cn

[A20] 读取标准输入
来源：http://bz.9csxet.cn

Py:   name = input("请输入：")
来源：http://st.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pr.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hj.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://ht.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ef.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gh.gzmigu.cn

Ruby: gets.chomp
来源：http://pz.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://vt.newstarts.cn

[A21] 保留指定小数位输出
来源：http://tr.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ya.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vo.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://zs.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://kp.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://ll.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xc.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://vt.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://xd.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ry.gzmigu.cn

Py:   len(s)
来源：http://jg.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jg.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bg.haigaiapp.cn

TS:   s.length
来源：http://lq.9csxet.cn

Java: s.length()
来源：http://gz.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ly.szxytkj.cn

Ruby: s.length
来源：http://ck.9csxet.cn

C#:   s.Length
来源：http://ve.szsharing.cn

[A23] 大小写转换
来源：http://yd.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xz.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zp.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ds.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bl.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xa.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jc.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nk.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jg.haigaiapp.cn

[A24] 去除首尾空白
来源：http://oc.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pl.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qr.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mb.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kb.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://ri.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://em.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ri.muxihuayi.cn

[A25] 字符串比较
来源：http://ng.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://ot.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iw.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cp.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bf.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sx.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://du.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wt.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ir.bookmarksfly.cn

[A26] 类型转换总览
来源：http://ps.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ul.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://es.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ix.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://mg.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xo.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yu.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zw.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yz.yuexingan06.cn

================================================================================
来源：http://cs.newstarts.cn

B. 流程控制
来源：http://rn.huixiangedu.cn

================================================================================
来源：http://cq.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://fu.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lt.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://og.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yu.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zk.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bj.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fq.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pu.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ya.huanxung.cn

[B02] 多分支 else if / elif
来源：http://kx.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xu.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sg.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ar.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kf.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://og.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nd.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lu.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ku.bjjhwx.cn

[B03] switch / match / case
来源：http://yr.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vx.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bl.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yg.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lx.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://at.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ub.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ot.chemitech.net.cn

[B04] for 计数循环
来源：http://ew.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://qw.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ik.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hu.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://en.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hr.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://af.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://mv.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fo.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://sv.asd995.cn

Py:   for item in arr: print(item)
来源：http://yx.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yx.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tf.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fa.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ap.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ae.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://vd.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lg.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://bi.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vn.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nc.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://np.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lp.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ac.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://we.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lr.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.newstarts.cn

[B07] while 循环
来源：http://bj.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://dp.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tn.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://xb.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ac.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://vc.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ro.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://sl.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://qo.colortex.cn

[B08] do-while（至少执行一次）
来源：http://gp.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jh.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://im.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://dh.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://kx.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://mk.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tq.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ct.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://ax.huanxung.cn

[B09] break 与 continue
来源：http://fh.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ar.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wu.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fu.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lm.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jf.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qr.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jj.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://vd.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rr.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eq.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sy.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ua.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mn.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ug.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fu.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://la.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://cl.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://kq.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://gj.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kd.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xx.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bw.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://fb.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ne.9csxet.cn

[B12] 跳出多层循环
来源：http://co.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ea.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dq.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ed.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lg.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sm.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kc.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jv.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://io.panjiajie.cn

[B13] 判断是否为数字
来源：http://dy.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://ym.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://li.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xk.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jg.bjjhwx.cn

Java: x instanceof Number
来源：http://xu.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vr.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://tg.521024.cn

C#:   x is int or double or decimal
来源：http://hg.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://xm.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vt.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://se.chemitech.net.cn


<!-- 参考信息 -->