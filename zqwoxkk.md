代发 wailian999

Ruby: 42.to_s
来源：http://wg.asd995.cn

C#:   42.ToString()
来源：http://zu.nicolike.cn

[A08] 取整与四舍五入
来源：http://nl.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fb.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ww.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vg.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rm.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gm.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://un.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ka.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cj.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://pm.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ib.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ze.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rq.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pa.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mj.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ox.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dq.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xb.colortex.cn

[A10] 生成随机数
来源：http://pd.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ap.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ty.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jy.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yb.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://fr.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cy.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://yq.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://ym.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://vl.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://hj.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lp.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pw.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ee.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://dj.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://be.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iv.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rb.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://br.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ji.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mi.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://ac.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://zk.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ie.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fo.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://mv.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://pu.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nu.nicolike.cn

Py:   "第一行\n第二行"
来源：http://pk.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://iy.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://on.9csxet.cn

TS:   "第一行\n第二行"
来源：http://xj.newstarts.cn

Java: "第一行\n第二行"
来源：http://mz.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://bl.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://gw.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://sj.huixiangedu.cn

[A14] 注释写法
来源：http://kh.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ab.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ka.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://mk.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://xw.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://on.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://yy.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oy.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://iw.gzmigu.cn

[A15] 空值判断与默认值
来源：http://rb.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://he.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://sj.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://om.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://xw.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nk.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://sn.colortex.cn

Ruby: value = data || "默认值"
来源：http://wu.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://ij.chemitech.net.cn

[A16] 真假值判断规则
来源：http://ni.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ro.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fz.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oa.lnxyls.cn

TS:   if (!x) {}
来源：http://gj.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ku.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ej.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yy.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zc.shtwfgs.cn

[A17] 位运算
来源：http://hd.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mh.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rp.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zh.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uc.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wr.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cw.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://fq.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://ty.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://xe.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://el.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tz.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://jz.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xs.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ya.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://hk.huanxung.cn

[A19] 交换两个变量
来源：http://hz.colortex.cn

Py:   a, b = b, a
来源：http://uq.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bl.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://xl.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://uc.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://wn.bookmarksfly.cn

Go:   a, b = b, a
来源：http://ja.wgjwhj.cn

Ruby: a, b = b, a
来源：http://ta.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://qs.hnjuh.cn

[A20] 读取标准输入
来源：http://ih.9csxet.cn

Py:   name = input("请输入：")
来源：http://kr.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hu.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gt.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://lr.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://ro.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nc.hahajie.cn

Ruby: gets.chomp
来源：http://zz.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ym.huanxung.cn

[A21] 保留指定小数位输出
来源：http://dz.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://fo.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://id.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://iv.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://pt.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://ub.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cn.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://yi.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://ie.muxihuayi.cn

[A22] 获取字符串长度
来源：http://jc.jctech888.com.cn

Py:   len(s)
来源：http://hk.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xz.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hx.bookmarksfly.cn

TS:   s.length
来源：http://vc.shtwfgs.cn

Java: s.length()
来源：http://mt.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jp.chemitech.net.cn

Ruby: s.length
来源：http://qz.521024.cn

C#:   s.Length
来源：http://ws.bjjhwx.cn

[A23] 大小写转换
来源：http://bp.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://td.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mu.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ce.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fv.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kf.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qs.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qn.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xl.panjiajie.cn

[A24] 去除首尾空白
来源：http://gt.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yg.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cj.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ag.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ch.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pp.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://aw.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vl.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ld.bookmarksfly.cn

[A25] 字符串比较
来源：http://mp.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://fv.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wh.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jk.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fx.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gf.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pr.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yv.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sy.shtwfgs.cn

[A26] 类型转换总览
来源：http://ao.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qu.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://my.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xf.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ee.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jm.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wy.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ev.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ka.asd995.cn

================================================================================
来源：http://fv.521024.cn

B. 流程控制
来源：http://vg.szsharing.cn

================================================================================
来源：http://tv.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://qu.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xa.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ur.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://la.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zo.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://su.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://he.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rm.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tm.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ud.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://po.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kn.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mx.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rs.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jw.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.wgjwhj.cn

[B03] switch / match / case
来源：http://kh.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oo.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wk.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cv.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yj.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xc.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xc.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oz.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rs.hnjuh.cn

[B04] for 计数循环
来源：http://ug.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://py.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zs.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hx.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pi.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ka.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dl.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://ly.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://te.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://pn.colortex.cn

Py:   for item in arr: print(item)
来源：http://rp.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nq.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oz.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fh.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qm.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gd.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://vm.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vw.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://pu.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sn.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ov.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://un.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ch.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ev.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uz.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ov.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sh.shtwfgs.cn

[B07] while 循环
来源：http://bt.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://jm.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zr.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://tq.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://mi.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://po.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kg.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://dm.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://to.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://pa.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://oy.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rw.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://wb.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://wm.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iq.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://em.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://pf.bjjhwx.cn

[B09] break 与 continue
来源：http://us.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fo.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uu.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gr.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ut.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://st.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://yh.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qp.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oj.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hf.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wq.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kw.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uc.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ik.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vk.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ob.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://ag.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ka.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://th.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ww.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vy.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://jj.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uv.huixiangedu.cn

[B12] 跳出多层循环
来源：http://cj.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bl.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zu.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gw.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dg.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xd.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qf.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nw.nicolike.cn

[B13] 判断是否为数字
来源：http://am.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://yp.9csxet.cn

PHP:  is_numeric($x)
来源：http://ku.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tf.shxzskj.cn

Java: x instanceof Number
来源：http://pp.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wv.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://hp.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://nf.521024.cn

[B14] 判断值是否在集合内
来源：http://np.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eu.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ns.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://yo.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ip.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sa.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rc.szxytkj.cn


<!-- 参考信息 -->