代发 wailian999

JS:   String(42); (42).toString()
来源：http://ih.nicolike.cn

TS:   String(42)
来源：http://ue.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vw.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://up.nszjky.cn

Ruby: 42.to_s
来源：http://zp.bookmarksfly.cn

C#:   42.ToString()
来源：http://dh.nszjky.cn

[A08] 取整与四舍五入
来源：http://sq.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gl.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fk.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xs.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rl.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://de.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dg.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sq.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vb.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://jn.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kc.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fe.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mm.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jr.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gj.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iv.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xm.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hp.hahajie.cn

[A10] 生成随机数
来源：http://wd.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://mg.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://fr.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fh.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ek.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://xp.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wo.gzmigu.cn

Ruby: rand(1..100)
来源：http://al.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ml.9csxet.cn

[A11] 条件表达式（三元）
来源：http://ao.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://oy.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lh.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sy.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xa.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://rd.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bi.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://so.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tf.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://sd.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hc.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pg.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://ph.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://do.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://pl.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yc.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://io.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ly.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tt.colortex.cn

Py:   "第一行\n第二行"
来源：http://eo.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://lt.9csxet.cn

JS:   "第一行\n第二行"
来源：http://od.szsharing.cn

TS:   "第一行\n第二行"
来源：http://sm.nicolike.cn

Java: "第一行\n第二行"
来源：http://by.colortex.cn

Go:   "第一行\n第二行"
来源：http://gu.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://yv.asd995.cn

C#:   "第一行\n第二行"
来源：http://uo.chemitech.net.cn

[A14] 注释写法
来源：http://to.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uy.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ui.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://gx.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://sw.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sm.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://bp.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nb.521024.cn

C#:   // 单行；/* 多行 */
来源：http://fi.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://qt.szxytkj.cn

Py:   value = data or "默认值"
来源：http://xc.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://fq.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://ws.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://ex.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://du.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://ko.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://na.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://cg.yuexingan06.cn

[A16] 真假值判断规则
来源：http://pt.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rc.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hw.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cp.shtwfgs.cn

TS:   if (!x) {}
来源：http://gt.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qw.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vl.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qf.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fh.huixinmuqiang.cn

[A17] 位运算
来源：http://xr.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yr.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qs.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://is.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aw.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://el.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://tz.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://qv.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://bl.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xq.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ik.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://zz.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dm.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://yl.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://jp.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://iq.muxihuayi.cn

Py:   a, b = b, a
来源：http://ak.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ck.521024.cn

JS:   [a, b] = [b, a];
来源：http://dm.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://rc.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://lk.chemitech.net.cn

Go:   a, b = b, a
来源：http://wl.haigaiapp.cn

Ruby: a, b = b, a
来源：http://ob.colortex.cn

C#:   (a, b) = (b, a);
来源：http://mz.chemitech.net.cn

[A20] 读取标准输入
来源：http://yi.asd995.cn

Py:   name = input("请输入：")
来源：http://sh.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mh.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lq.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://of.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://qr.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jz.9csxet.cn

Ruby: gets.chomp
来源：http://oo.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ti.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://cl.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://tx.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hw.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://gz.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://om.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://eb.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://on.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://gn.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://le.szsharing.cn

[A22] 获取字符串长度
来源：http://zr.muxihuayi.cn

Py:   len(s)
来源：http://ys.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vo.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wk.szxytkj.cn

TS:   s.length
来源：http://rn.nszjky.cn

Java: s.length()
来源：http://zn.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://et.nicolike.cn

Ruby: s.length
来源：http://wu.jctech888.com.cn

C#:   s.Length
来源：http://ma.asd995.cn

[A23] 大小写转换
来源：http://te.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nk.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wa.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sv.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://av.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://if.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://es.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://du.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dp.nicolike.cn

[A24] 去除首尾空白
来源：http://fp.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jf.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bz.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mv.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bs.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kp.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://dq.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wy.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://av.9csxet.cn

[A25] 字符串比较
来源：http://iu.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://zp.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sq.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oy.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bo.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ma.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hy.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yg.jctech888.com.cn

[A26] 类型转换总览
来源：http://no.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bo.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ev.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ea.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://yr.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pw.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://js.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vq.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ep.shxzskj.cn

================================================================================
来源：http://iw.hahajie.cn

B. 流程控制
来源：http://sm.hnjuh.cn

================================================================================
来源：http://qd.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://fq.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fw.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pz.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ov.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ue.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wx.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kg.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://js.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qe.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://es.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kr.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dj.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rg.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://td.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gu.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hi.9csxet.cn

[B03] switch / match / case
来源：http://wy.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bu.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wz.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zl.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jl.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tf.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xq.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zj.szsharing.cn

[B04] for 计数循环
来源：http://ea.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://hm.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kx.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rv.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qi.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ys.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uy.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ig.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wh.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://br.asd995.cn

Py:   for item in arr: print(item)
来源：http://pc.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ph.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xc.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ng.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kz.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zi.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://wz.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sa.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://tq.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sk.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kn.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sq.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gt.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kd.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cd.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pc.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bp.9csxet.cn

[B07] while 循环
来源：http://yg.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ky.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xb.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://zl.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://le.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://mp.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qj.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://cm.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://vh.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://kl.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://mt.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rh.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://jq.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://sz.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://op.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uk.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kb.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://xq.newstarts.cn

[B09] break 与 continue
来源：http://fo.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ga.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qn.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ti.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pp.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zf.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ws.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://kh.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jq.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kq.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gs.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qb.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pr.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mb.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zs.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hc.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://ao.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://mb.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://vy.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://io.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xo.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ft.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bi.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://tr.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kn.shxzukj.cn

[B12] 跳出多层循环
来源：http://dp.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hd.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jz.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jv.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dx.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xy.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qo.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ox.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ah.newstarts.cn

[B13] 判断是否为数字
来源：http://yj.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://fv.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://ze.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://to.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jo.bookmarksfly.cn

Java: x instanceof Number
来源：http://mf.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qt.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://pa.gzmigu.cn

C#:   x is int or double or decimal
来源：http://da.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://fb.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nn.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ga.colortex.cn


<!-- 参考信息 -->