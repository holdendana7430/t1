代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vx.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aw.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vm.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qs.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ix.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pk.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qj.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://fk.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ty.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://en.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bt.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gf.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gx.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fa.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qn.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ko.huanxung.cn

[A10] 生成随机数
来源：http://ji.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://pi.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://bm.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xi.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kz.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://io.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nh.hnjuh.cn

Ruby: rand(1..100)
来源：http://po.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://fv.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://fr.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://ng.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sr.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ka.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uk.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://md.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ae.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bg.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ol.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://vs.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rv.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fl.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://px.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ry.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://zg.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vj.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://ek.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://pp.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dr.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://bl.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://st.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://oa.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://xe.9csxet.cn

Java: "第一行\n第二行"
来源：http://pc.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://cc.colortex.cn

Ruby: "第一行\n第二行"
来源：http://dv.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://rt.yuexingan06.cn

[A14] 注释写法
来源：http://qf.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://er.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zc.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://ud.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://nl.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oh.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://tt.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yi.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://lc.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://sz.nicolike.cn

Py:   value = data or "默认值"
来源：http://yg.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://tl.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://zq.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://pb.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ai.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://cg.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://ri.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://md.lnxyls.cn

[A16] 真假值判断规则
来源：http://je.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://km.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ac.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ef.asd995.cn

TS:   if (!x) {}
来源：http://le.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yq.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rp.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ib.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lc.asd995.cn

[A17] 位运算
来源：http://su.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ha.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sn.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fn.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zt.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cj.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ai.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dh.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://tp.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://mk.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://ad.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pi.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ef.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://at.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://md.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://jy.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://bv.9csxet.cn

[A19] 交换两个变量
来源：http://uh.nicolike.cn

Py:   a, b = b, a
来源：http://kr.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wd.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://ox.colortex.cn

TS:   [a, b] = [b, a];
来源：http://lc.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://oh.yuexingan06.cn

Go:   a, b = b, a
来源：http://ms.shxzskj.cn

Ruby: a, b = b, a
来源：http://hw.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://vr.panjiajie.cn

[A20] 读取标准输入
来源：http://fm.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://nq.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xf.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wy.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://qp.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://ds.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eq.huixiangedu.cn

Ruby: gets.chomp
来源：http://xj.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://wc.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://oh.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://kl.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nb.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://yc.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://se.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://xp.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hs.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://pz.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://mw.wgjwhj.cn

[A22] 获取字符串长度
来源：http://jk.9csxet.cn

Py:   len(s)
来源：http://sy.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sr.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kg.newstarts.cn

TS:   s.length
来源：http://ry.colortex.cn

Java: s.length()
来源：http://wq.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qw.newstarts.cn

Ruby: s.length
来源：http://so.nszjky.cn

C#:   s.Length
来源：http://td.shxzskj.cn

[A23] 大小写转换
来源：http://gc.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wm.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kt.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cq.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vz.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zn.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uy.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ir.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xc.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://fr.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fy.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uf.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pa.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ur.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fw.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hp.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ux.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uu.panjiajie.cn

[A25] 字符串比较
来源：http://yt.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://pf.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ky.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://za.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kt.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fp.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fu.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vx.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nz.shxzskj.cn

[A26] 类型转换总览
来源：http://rh.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gy.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uk.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cg.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://zo.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mt.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tp.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kr.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zz.jianghongdianzi.cn

================================================================================
来源：http://xr.colortex.cn

B. 流程控制
来源：http://um.nicolike.cn

================================================================================
来源：http://rb.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://dz.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ys.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://se.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ve.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eu.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ey.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gb.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ch.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cd.colortex.cn

[B02] 多分支 else if / elif
来源：http://bc.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rc.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vr.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pg.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yj.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vk.szsharing.cn

[B03] switch / match / case
来源：http://or.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://du.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kc.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yv.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://se.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ht.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xa.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wh.hnjuh.cn

[B04] for 计数循环
来源：http://ob.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://kq.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sn.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tl.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zg.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xi.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ke.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://dw.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ae.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://qy.colortex.cn

Py:   for item in arr: print(item)
来源：http://li.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yv.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yo.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gp.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ao.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yj.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://lr.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rb.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://rf.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hj.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ez.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ma.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wg.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qz.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gl.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://au.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oj.nszjky.cn

[B07] while 循环
来源：http://du.asd995.cn

Py:   while i < 10: i += 1
来源：http://jy.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://td.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://ba.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://zd.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://hj.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sf.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://zw.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ox.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://tb.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://rp.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gi.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://ho.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ow.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://nl.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eh.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://af.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://rx.shtwfgs.cn

[B09] break 与 continue
来源：http://ro.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dz.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tl.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oa.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sw.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wh.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mu.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xo.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://vs.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cf.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://us.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xv.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ht.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zo.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ca.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pu.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://si.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://na.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://rn.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://rc.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wz.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xy.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qq.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wc.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ze.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qw.huanxung.cn

[B12] 跳出多层循环
来源：http://fw.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bk.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yh.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rg.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wg.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mh.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pb.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gv.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xc.asd995.cn

[B13] 判断是否为数字
来源：http://vp.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ek.nicolike.cn

PHP:  is_numeric($x)
来源：http://uy.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cl.hahajie.cn

Java: x instanceof Number
来源：http://nq.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ib.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://zv.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://yh.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://fk.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://co.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fl.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://te.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://kd.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yo.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pk.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xz.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lv.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ef.huixiangedu.cn

Py:   a and b or not c
来源：http://rn.9csxet.cn


<!-- 参考信息 -->