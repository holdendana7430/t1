代发 wailian999

JS:   String(42); (42).toString()
来源：http://ab.shxzskj.cn

TS:   String(42)
来源：http://jr.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bx.521024.cn

Go:   strconv.Itoa(42)
来源：http://lk.colortex.cn

Ruby: 42.to_s
来源：http://kc.shxzskj.cn

C#:   42.ToString()
来源：http://jy.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://id.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yt.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xg.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mx.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pw.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zp.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cr.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rx.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ne.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://bh.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ha.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dk.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jl.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ha.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gd.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vc.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rs.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jo.yuntaijiaju.cn

[A10] 生成随机数
来源：http://iq.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://oh.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://cd.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ui.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ra.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://pc.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ax.521024.cn

Ruby: rand(1..100)
来源：http://pa.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://fc.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://iy.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://ks.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jw.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vc.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pb.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://hg.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zm.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hy.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nw.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://km.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zc.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bg.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://dm.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://rs.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://ks.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xe.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://pc.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://fh.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iu.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://gw.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://xa.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://iq.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://tg.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://ej.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://hy.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://fo.newstarts.cn

C#:   "第一行\n第二行"
来源：http://th.shxzskj.cn

[A14] 注释写法
来源：http://gg.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dr.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lq.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://rb.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://zn.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jg.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://kp.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ek.521024.cn

C#:   // 单行；/* 多行 */
来源：http://cp.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://em.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://li.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://te.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://vi.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://te.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ol.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://yl.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://ld.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://gr.jctech888.com.cn

[A16] 真假值判断规则
来源：http://vx.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wb.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vw.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vj.huanxung.cn

TS:   if (!x) {}
来源：http://ui.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ga.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xs.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zx.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://po.bjjhwx.cn

[A17] 位运算
来源：http://tt.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ue.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ga.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://we.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gr.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wx.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vp.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zv.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://dl.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://vj.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://bh.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uc.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.521024.cn

Java: (int) 'A'; (char) 65
来源：http://mm.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ey.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://hc.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://cr.nszjky.cn

[A19] 交换两个变量
来源：http://xz.szxytkj.cn

Py:   a, b = b, a
来源：http://wp.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yp.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://dn.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://hm.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://xx.huixiangedu.cn

Go:   a, b = b, a
来源：http://to.yuexingan06.cn

Ruby: a, b = b, a
来源：http://cf.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://by.wgjwhj.cn

[A20] 读取标准输入
来源：http://hx.hnjuh.cn

Py:   name = input("请输入：")
来源：http://rk.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://br.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://al.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://gr.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://tt.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tw.bookmarksfly.cn

Ruby: gets.chomp
来源：http://jm.colortex.cn

C#:   Console.ReadLine();
来源：http://ac.huanxung.cn

[A21] 保留指定小数位输出
来源：http://ok.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://hl.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ja.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://am.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://db.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://gv.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hg.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://bj.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://lw.panjiajie.cn

[A22] 获取字符串长度
来源：http://dt.panjiajie.cn

Py:   len(s)
来源：http://nm.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://af.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fr.jianghongdianzi.cn

TS:   s.length
来源：http://ci.szsharing.cn

Java: s.length()
来源：http://yw.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gq.wgjwhj.cn

Ruby: s.length
来源：http://ca.hahajie.cn

C#:   s.Length
来源：http://pw.shxzukj.cn

[A23] 大小写转换
来源：http://da.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lz.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mt.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://we.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hn.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aq.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://es.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uk.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xp.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://lo.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ee.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ew.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qj.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wa.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iy.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://ev.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fz.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tm.shxzskj.cn

[A25] 字符串比较
来源：http://ds.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ij.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xf.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ee.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oz.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ph.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hg.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tg.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wj.szxytkj.cn

[A26] 类型转换总览
来源：http://dr.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pp.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ol.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fd.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ds.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yy.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ee.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ts.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jk.bookmarksfly.cn

================================================================================
来源：http://tz.panjiajie.cn

B. 流程控制
来源：http://tx.wgjwhj.cn

================================================================================
来源：http://ni.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ts.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xw.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rz.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kc.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jz.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ms.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sn.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wf.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mm.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ne.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hu.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ws.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sg.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dg.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.huanxung.cn

[B03] switch / match / case
来源：http://lb.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ux.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sh.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mh.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tc.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vq.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zh.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qq.panjiajie.cn

[B04] for 计数循环
来源：http://iz.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://fr.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kl.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://et.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://da.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uu.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jr.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://vl.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ew.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://xl.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://tz.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rt.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bb.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yz.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xd.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lz.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://se.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://up.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://ta.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wn.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ec.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://da.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ex.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lq.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hi.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://po.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xi.colortex.cn

[B07] while 循环
来源：http://ao.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://tg.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mq.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://oj.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://gt.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://lo.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iy.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://fg.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://nt.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://pd.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://kk.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qa.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://li.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://br.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://wl.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qx.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dt.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://zz.huixinmuqiang.cn

[B09] break 与 continue
来源：http://wj.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gx.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://en.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pf.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uk.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://nt.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ar.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://co.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oz.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ve.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wj.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yg.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pa.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aw.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://qn.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://wm.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://lw.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hk.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ho.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xc.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aa.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://xg.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qo.newstarts.cn

[B12] 跳出多层循环
来源：http://es.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tq.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ba.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qz.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://el.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kb.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://og.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ua.lnxyls.cn

[B13] 判断是否为数字
来源：http://jk.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ar.panjiajie.cn

PHP:  is_numeric($x)
来源：http://ih.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ge.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lx.muxihuayi.cn

Java: x instanceof Number
来源：http://bn.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://io.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ed.shxzskj.cn

C#:   x is int or double or decimal
来源：http://ad.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://ri.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hl.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://el.colortex.cn


<!-- 参考信息 -->