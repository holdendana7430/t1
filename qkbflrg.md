代发 wailian999

Ruby: 42.to_s
来源：http://qk.huanxung.cn

C#:   42.ToString()
来源：http://di.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://ym.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mx.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yx.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nl.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cf.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jc.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://is.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://te.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ox.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://pn.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wb.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wv.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bp.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ua.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tl.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tz.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rb.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://im.shxzukj.cn

[A10] 生成随机数
来源：http://ad.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://fe.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://qj.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cg.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pl.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://do.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://od.muxihuayi.cn

Ruby: rand(1..100)
来源：http://yx.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://eq.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://tq.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://gv.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vb.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sd.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kq.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://ue.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iv.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://px.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cm.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://mt.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://la.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://al.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://hs.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://nc.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://fv.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rp.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://eu.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://ut.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ey.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://su.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://pi.huanxung.cn

JS:   "第一行\n第二行"
来源：http://so.hahajie.cn

TS:   "第一行\n第二行"
来源：http://xk.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ev.9csxet.cn

Go:   "第一行\n第二行"
来源：http://xt.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://zd.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://oq.nszjky.cn

[A14] 注释写法
来源：http://ou.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sf.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hq.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://gd.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://zh.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cq.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://qq.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hw.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://jb.szsharing.cn

[A15] 空值判断与默认值
来源：http://ci.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://ly.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://js.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://jq.521024.cn

TS:   const value = data ?? "默认值";
来源：http://xv.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hy.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://zc.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://om.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ih.huanxung.cn

[A16] 真假值判断规则
来源：http://gy.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bb.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bq.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nu.gzmigu.cn

TS:   if (!x) {}
来源：http://pr.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gx.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cg.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://es.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ag.lnxyls.cn

[A17] 位运算
来源：http://hu.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://le.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ee.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wo.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uq.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://up.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qk.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://mi.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://fm.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://go.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ck.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://md.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ub.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tv.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://ys.colortex.cn

C#:   (int)'A'; (char)65
来源：http://gj.shxzskj.cn

[A19] 交换两个变量
来源：http://xy.wgjwhj.cn

Py:   a, b = b, a
来源：http://mi.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hb.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://lf.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://nx.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://zr.haigaiapp.cn

Go:   a, b = b, a
来源：http://jo.hnjuh.cn

Ruby: a, b = b, a
来源：http://ea.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://bl.panjiajie.cn

[A20] 读取标准输入
来源：http://vs.asd995.cn

Py:   name = input("请输入：")
来源：http://ex.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ke.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nv.asd995.cn

TS:   // Node.js：readline 模块
来源：http://wt.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://td.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://si.haigaiapp.cn

Ruby: gets.chomp
来源：http://zb.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://ov.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://ks.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://iz.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qi.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://hl.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://ie.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://sa.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zl.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://bz.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://ha.hnjuh.cn

[A22] 获取字符串长度
来源：http://ne.szsharing.cn

Py:   len(s)
来源：http://aa.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gp.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hm.lnxyls.cn

TS:   s.length
来源：http://aj.yuntaijiaju.cn

Java: s.length()
来源：http://un.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ji.haigaiapp.cn

Ruby: s.length
来源：http://ut.colortex.cn

C#:   s.Length
来源：http://nf.hnjuh.cn

[A23] 大小写转换
来源：http://in.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lc.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lk.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ct.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gx.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hd.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xp.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vv.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xb.nszjky.cn

[A24] 去除首尾空白
来源：http://ek.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vc.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lo.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mc.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ij.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gs.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://tr.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://au.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hr.huixinmuqiang.cn

[A25] 字符串比较
来源：http://gz.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ma.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dl.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nw.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ip.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lw.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vu.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ih.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wq.jctech888.com.cn

[A26] 类型转换总览
来源：http://ut.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kz.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ya.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ux.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://eg.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ha.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ux.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qc.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.bjjhwx.cn

================================================================================
来源：http://jc.gzmigu.cn

B. 流程控制
来源：http://eh.huanxung.cn

================================================================================
来源：http://mn.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ec.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ll.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wj.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ka.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ub.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ox.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://of.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qp.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gd.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://uq.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://du.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xq.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ye.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cg.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bv.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://io.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sk.gzmigu.cn

[B03] switch / match / case
来源：http://mi.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ri.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sj.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wl.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zt.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gr.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ak.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iy.huixinmuqiang.cn

[B04] for 计数循环
来源：http://su.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://hh.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bp.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fr.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ru.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qg.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nw.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://eq.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://id.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ow.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://it.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wo.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dw.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fu.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fz.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://he.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://hn.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yf.asd995.cn

[B06] 遍历字典 / 对象
来源：http://cu.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lo.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gv.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ek.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ht.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ue.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yv.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ro.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://za.hnjuh.cn

[B07] while 循环
来源：http://tv.asd995.cn

Py:   while i < 10: i += 1
来源：http://gb.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fs.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://fo.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://vl.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://ik.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://db.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ua.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://qy.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://tb.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://bb.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zo.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://do.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://rh.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://df.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hq.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zl.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://es.muxihuayi.cn

[B09] break 与 continue
来源：http://fz.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nc.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sq.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bh.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nv.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ed.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mr.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.huanxung.cn

[B10] 遍历同时拿索引
来源：http://rj.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tf.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ib.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xs.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gj.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wi.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://no.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bs.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mn.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://fn.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://yy.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://cr.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gc.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fn.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ab.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sv.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://dv.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hp.yuexingan06.cn

[B12] 跳出多层循环
来源：http://fc.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ya.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sn.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rx.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ml.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://le.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rl.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wx.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ik.jctech888.com.cn

[B13] 判断是否为数字
来源：http://ow.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://vb.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://dl.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wb.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fm.shtwfgs.cn

Java: x instanceof Number
来源：http://zx.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://co.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://iv.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://oe.9csxet.cn

[B14] 判断值是否在集合内
来源：http://jm.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sq.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tf.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://he.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ro.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ts.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dm.hnjuh.cn


<!-- 参考信息 -->