代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ra.shxzskj.cn

[A07] 数字转字符串
来源：http://cj.nszjky.cn

Py:   str(42)
来源：http://du.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://wi.huanxung.cn

JS:   String(42); (42).toString()
来源：http://tf.szxytkj.cn

TS:   String(42)
来源：http://jm.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oj.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://we.muxihuayi.cn

Ruby: 42.to_s
来源：http://qc.bjjhwx.cn

C#:   42.ToString()
来源：http://vl.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://qh.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ch.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://co.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xr.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zf.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lv.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tk.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cu.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xm.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://uo.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rf.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sg.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fk.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kx.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bx.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xe.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zm.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://do.panjiajie.cn

[A10] 生成随机数
来源：http://vg.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://ka.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://ei.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sf.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vy.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://ud.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tf.muxihuayi.cn

Ruby: rand(1..100)
来源：http://qb.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://tq.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://xf.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://vn.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://do.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pp.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://im.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://df.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ae.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ww.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pl.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://va.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jl.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jh.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://yg.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://go.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://hw.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cy.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://bk.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://pa.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vu.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://se.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://td.huanxung.cn

JS:   "第一行\n第二行"
来源：http://kv.colortex.cn

TS:   "第一行\n第二行"
来源：http://qc.asd995.cn

Java: "第一行\n第二行"
来源：http://pu.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://jm.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://kb.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://un.nicolike.cn

[A14] 注释写法
来源：http://zk.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yv.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bv.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://jz.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://jn.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cy.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://mx.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qm.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://yz.szsharing.cn

[A15] 空值判断与默认值
来源：http://lq.521024.cn

Py:   value = data or "默认值"
来源：http://dl.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://tb.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ss.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://fv.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fp.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://wk.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://mw.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://wc.shxzukj.cn

[A16] 真假值判断规则
来源：http://nw.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dr.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cc.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dg.hnjuh.cn

TS:   if (!x) {}
来源：http://bc.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wd.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aq.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nl.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ff.gzmigu.cn

[A17] 位运算
来源：http://yh.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oy.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wh.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://li.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fk.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xw.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://in.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://lk.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://so.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zo.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dw.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://qd.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://do.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://gu.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://kq.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://sj.shxzskj.cn

Py:   a, b = b, a
来源：http://oo.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ax.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://kb.521024.cn

TS:   [a, b] = [b, a];
来源：http://aj.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://vd.wgjwhj.cn

Go:   a, b = b, a
来源：http://dm.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://wa.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://ou.muxihuayi.cn

[A20] 读取标准输入
来源：http://jj.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://rx.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ap.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vg.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://gx.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://zk.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gr.wgjwhj.cn

Ruby: gets.chomp
来源：http://kr.nszjky.cn

C#:   Console.ReadLine();
来源：http://yt.nszjky.cn

[A21] 保留指定小数位输出
来源：http://es.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://gz.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mo.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://kh.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://qe.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://ye.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rr.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://oh.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://px.huanxung.cn

[A22] 获取字符串长度
来源：http://ie.9csxet.cn

Py:   len(s)
来源：http://fw.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bu.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://is.szsharing.cn

TS:   s.length
来源：http://em.521024.cn

Java: s.length()
来源：http://im.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yc.szsharing.cn

Ruby: s.length
来源：http://br.asd995.cn

C#:   s.Length
来源：http://pe.shxzukj.cn

[A23] 大小写转换
来源：http://ll.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tk.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iq.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mw.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ju.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nt.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fg.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jn.szxytkj.cn

[A24] 去除首尾空白
来源：http://vs.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://as.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://to.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://db.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zk.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://we.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://oc.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qb.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xb.asd995.cn

[A25] 字符串比较
来源：http://dz.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://pe.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://az.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ux.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sn.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vz.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zv.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://br.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zr.huixiangedu.cn

[A26] 类型转换总览
来源：http://ro.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lu.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iq.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xb.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://vs.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mn.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zb.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hd.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://te.gzmigu.cn

================================================================================
来源：http://ux.muxihuayi.cn

B. 流程控制
来源：http://or.nicolike.cn

================================================================================
来源：http://kj.hahajie.cn

[B01] 条件判断 if / else
来源：http://sy.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://na.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ro.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ro.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gr.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qf.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ym.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ak.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jx.newstarts.cn

[B02] 多分支 else if / elif
来源：http://up.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jh.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jv.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ml.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ag.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qp.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://md.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cv.shxzskj.cn

[B03] switch / match / case
来源：http://tt.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hp.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mo.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dn.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://up.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mm.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gy.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eq.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rs.gzmigu.cn

[B04] for 计数循环
来源：http://zk.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://wx.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://up.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qd.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pl.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uv.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xa.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://as.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nk.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://dm.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://be.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fw.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ou.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cg.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ec.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fw.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://gq.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vr.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://jy.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://et.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kd.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bg.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gv.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://on.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zg.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vm.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vq.gzmigu.cn

[B07] while 循环
来源：http://gt.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ai.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pl.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://vg.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://hk.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://dv.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ai.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://lf.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ze.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://fs.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://dz.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://df.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ne.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://vf.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://hf.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lh.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ma.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://go.9csxet.cn

[B09] break 与 continue
来源：http://pd.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yj.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mk.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qg.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lo.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gw.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jg.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://vy.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ba.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ky.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kk.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://su.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uj.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nn.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eo.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://in.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://uc.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://ox.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://xt.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ts.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tj.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ws.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cc.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://xh.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ec.nszjky.cn

[B12] 跳出多层循环
来源：http://lc.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iy.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rq.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bu.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oq.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://we.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jd.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ym.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fq.huanxung.cn

[B13] 判断是否为数字
来源：http://ph.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://vo.asd995.cn

PHP:  is_numeric($x)
来源：http://vv.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rd.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xx.muxihuayi.cn

Java: x instanceof Number
来源：http://qg.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yt.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://hw.bjjhwx.cn


<!-- 参考信息 -->