代发 wailian999

JS:   String(42); (42).toString()
来源：http://ox.jctech888.com.cn

TS:   String(42)
来源：http://bi.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nx.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://bp.colortex.cn

Ruby: 42.to_s
来源：http://dz.chemitech.net.cn

C#:   42.ToString()
来源：http://lr.newstarts.cn

[A08] 取整与四舍五入
来源：http://gz.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mz.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nj.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ea.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fw.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gb.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uw.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ge.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ke.asd995.cn

[A09] 绝对值与最大最小值
来源：http://qd.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ws.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://go.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oa.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qj.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://de.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://go.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lm.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vc.szxytkj.cn

[A10] 生成随机数
来源：http://ya.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://pn.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://gu.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zg.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dd.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://by.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tr.gzmigu.cn

Ruby: rand(1..100)
来源：http://dh.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://sy.asd995.cn

[A11] 条件表达式（三元）
来源：http://cb.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://ej.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kf.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pi.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ln.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://jl.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fa.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mz.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fz.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://tc.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ic.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vi.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://zh.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://km.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://qh.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yr.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://rk.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://xb.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xl.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://nm.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://gj.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://od.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://lm.hahajie.cn

Java: "第一行\n第二行"
来源：http://eb.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://zx.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://kb.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://ec.haigaiapp.cn

[A14] 注释写法
来源：http://fl.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ph.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kw.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ll.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://uw.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ii.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://fk.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ga.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://la.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://sb.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://aq.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://cd.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://jn.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://mp.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zl.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://px.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://tv.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://bi.shtwfgs.cn

[A16] 真假值判断规则
来源：http://qu.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://le.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ma.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fd.szxytkj.cn

TS:   if (!x) {}
来源：http://bt.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wz.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pl.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dy.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oh.shxzskj.cn

[A17] 位运算
来源：http://ww.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lp.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cg.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ol.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://js.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sv.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://vp.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://nw.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://nf.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mc.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oc.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://el.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nk.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://rz.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://eb.haigaiapp.cn

[A19] 交换两个变量
来源：http://oe.huixiangedu.cn

Py:   a, b = b, a
来源：http://qj.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bv.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ed.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://zh.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://on.panjiajie.cn

Go:   a, b = b, a
来源：http://go.hahajie.cn

Ruby: a, b = b, a
来源：http://jc.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://cm.asd995.cn

[A20] 读取标准输入
来源：http://ow.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://kw.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xh.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bq.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://yu.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ke.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vx.bookmarksfly.cn

Ruby: gets.chomp
来源：http://cj.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://fk.colortex.cn

[A21] 保留指定小数位输出
来源：http://uc.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://zx.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kw.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ft.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://za.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://wl.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pg.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://yo.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://vf.521024.cn

[A22] 获取字符串长度
来源：http://dx.jctech888.com.cn

Py:   len(s)
来源：http://is.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fv.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hl.lnxyls.cn

TS:   s.length
来源：http://mt.hnjuh.cn

Java: s.length()
来源：http://gf.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xg.bookmarksfly.cn

Ruby: s.length
来源：http://ei.gzmigu.cn

C#:   s.Length
来源：http://lf.yuexingan06.cn

[A23] 大小写转换
来源：http://yy.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lo.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kj.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://be.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zg.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ht.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gd.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ei.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lb.yuexingan06.cn

[A24] 去除首尾空白
来源：http://ir.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aq.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://op.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ag.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lt.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dv.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://wn.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eg.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gz.colortex.cn

[A25] 字符串比较
来源：http://ub.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://ma.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xi.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://md.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oc.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ph.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://no.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mv.wgjwhj.cn

[A26] 类型转换总览
来源：http://cl.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ec.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cb.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yj.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ns.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uf.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hv.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ph.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lm.huanxung.cn

================================================================================
来源：http://sn.jianghongdianzi.cn

B. 流程控制
来源：http://cd.wgjwhj.cn

================================================================================
来源：http://sa.hnjuh.cn

[B01] 条件判断 if / else
来源：http://sp.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cj.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ss.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zz.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vg.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pp.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oy.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nw.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://tz.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nr.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://px.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://by.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vt.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xl.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bi.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bm.bjjhwx.cn

[B03] switch / match / case
来源：http://ql.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pu.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ur.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ky.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://by.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rz.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aq.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hk.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vd.huixiangedu.cn

[B04] for 计数循环
来源：http://mz.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://wc.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ml.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ba.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gu.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fo.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sn.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://wp.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sw.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://si.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://tf.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jr.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lv.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tb.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kn.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ud.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://al.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ki.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://rz.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ep.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uk.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rl.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ia.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pi.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iw.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://on.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ov.colortex.cn

[B07] while 循环
来源：http://uy.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://or.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bt.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ej.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://in.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://qm.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zc.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://mx.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://wq.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ot.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://yg.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zu.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://oh.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://wg.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://yk.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://be.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://af.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://bt.haigaiapp.cn

[B09] break 与 continue
来源：http://gv.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zb.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://po.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oe.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rj.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dt.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://st.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://si.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ez.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://az.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://it.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gf.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ly.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://an.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tl.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bw.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ql.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ad.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://op.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://cy.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vk.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ex.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rq.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pr.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ij.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gf.panjiajie.cn

[B12] 跳出多层循环
来源：http://qq.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uc.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dr.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gf.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://af.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kk.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zv.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://os.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vw.521024.cn

[B13] 判断是否为数字
来源：http://eu.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://dr.shxzskj.cn

PHP:  is_numeric($x)
来源：http://zn.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yo.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iz.hahajie.cn

Java: x instanceof Number
来源：http://sl.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://em.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://ej.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://uc.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://su.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nw.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nl.panjiajie.cn


<!-- 参考信息 -->