代发 wailian999

Ruby: 42.to_s
来源：http://qa.lnxyls.cn

C#:   42.ToString()
来源：http://dn.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://wl.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sa.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ad.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gq.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oj.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xt.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wc.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uf.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iw.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://ql.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zt.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ke.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ce.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ti.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rf.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zf.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rb.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hw.yuexingan06.cn

[A10] 生成随机数
来源：http://zq.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://it.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ld.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ob.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nl.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://my.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sq.szsharing.cn

Ruby: rand(1..100)
来源：http://lh.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://bc.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://xu.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://zu.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zm.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ec.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mz.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://gz.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zp.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ux.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pg.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://mo.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ki.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wf.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://ta.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://ok.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ux.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sc.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://jw.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://hj.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ip.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://xt.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://xu.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ce.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://qq.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://th.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://qh.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://fp.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://sj.shtwfgs.cn

[A14] 注释写法
来源：http://pa.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ol.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://im.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://yt.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://iq.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uj.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://dc.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ub.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://hj.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ly.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://gh.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://vx.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://go.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://nu.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vy.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://wy.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://nb.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://in.huanxung.cn

[A16] 真假值判断规则
来源：http://uf.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jp.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ql.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rn.wgjwhj.cn

TS:   if (!x) {}
来源：http://ib.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dr.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qy.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sw.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xl.bookmarksfly.cn

[A17] 位运算
来源：http://db.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ir.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ul.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bf.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://du.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ap.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://fc.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://il.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://mg.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bo.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uf.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://ot.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ye.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://qk.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://ya.bjjhwx.cn

[A19] 交换两个变量
来源：http://jp.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://ci.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://se.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ya.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://sn.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://wm.wgjwhj.cn

Go:   a, b = b, a
来源：http://bv.nicolike.cn

Ruby: a, b = b, a
来源：http://fi.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://oj.nszjky.cn

[A20] 读取标准输入
来源：http://xz.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://pn.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dz.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zf.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://lw.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://qu.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://df.yuexingan06.cn

Ruby: gets.chomp
来源：http://ol.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://ct.asd995.cn

[A21] 保留指定小数位输出
来源：http://fu.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://ji.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sr.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://zm.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://nq.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://vl.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gu.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ve.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://hf.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ay.szsharing.cn

Py:   len(s)
来源：http://kf.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wf.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ax.huixiangedu.cn

TS:   s.length
来源：http://jv.muxihuayi.cn

Java: s.length()
来源：http://sr.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qa.9csxet.cn

Ruby: s.length
来源：http://wj.huixiangedu.cn

C#:   s.Length
来源：http://fz.nicolike.cn

[A23] 大小写转换
来源：http://ty.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cu.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ie.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wl.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ri.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mj.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ft.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xg.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ew.muxihuayi.cn

[A24] 去除首尾空白
来源：http://vb.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mm.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://br.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kt.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hs.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jq.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://rj.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cb.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cf.nicolike.cn

[A25] 字符串比较
来源：http://ml.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://gc.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vl.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tf.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vr.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ok.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rd.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aw.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jx.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://fe.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cu.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://it.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ml.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://dq.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wx.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jy.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mj.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oa.jctech888.com.cn

================================================================================
来源：http://cu.hahajie.cn

B. 流程控制
来源：http://wu.shxzukj.cn

================================================================================
来源：http://yh.9csxet.cn

[B01] 条件判断 if / else
来源：http://yi.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cg.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rw.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cq.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dn.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kt.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ip.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://da.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wk.newstarts.cn

[B02] 多分支 else if / elif
来源：http://qg.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jc.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hb.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hh.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eq.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.bookmarksfly.cn

[B03] switch / match / case
来源：http://lg.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ab.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oy.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ro.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://no.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cf.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bh.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pv.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vd.hahajie.cn

[B04] for 计数循环
来源：http://uq.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://pj.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rl.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rs.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sv.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sh.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uv.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://kw.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wa.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://hj.szsharing.cn

Py:   for item in arr: print(item)
来源：http://ou.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qm.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cg.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yq.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gx.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xr.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://uz.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qg.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ig.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ry.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wg.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oc.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gj.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xk.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jj.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zz.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lk.haigaiapp.cn

[B07] while 循环
来源：http://sa.nicolike.cn

Py:   while i < 10: i += 1
来源：http://tu.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zz.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://wi.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ch.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://wn.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fz.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://sy.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://em.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ws.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://bg.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://an.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://yq.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://hb.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://gh.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ov.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ja.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://sj.muxihuayi.cn

[B09] break 与 continue
来源：http://kk.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ue.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jt.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ix.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sj.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kl.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yz.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xh.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://is.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ck.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xf.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dx.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ca.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bc.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pu.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gk.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ld.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ty.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://xp.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://gn.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://yu.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rc.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://my.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bq.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xq.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://dk.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rw.521024.cn

[B12] 跳出多层循环
来源：http://xn.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://os.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dl.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gs.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iu.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wv.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mx.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://le.panjiajie.cn

[B13] 判断是否为数字
来源：http://tw.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://mh.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://xj.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sg.hnjuh.cn

Java: x instanceof Number
来源：http://uy.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ql.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://mh.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://vp.asd995.cn

[B14] 判断值是否在集合内
来源：http://bk.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ul.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gj.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://aj.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://by.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dw.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bj.hnjuh.cn


<!-- 参考信息 -->