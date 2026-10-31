代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ye.shtwfgs.cn

[A07] 数字转字符串
来源：http://ez.jianghongdianzi.cn

Py:   str(42)
来源：http://it.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://yc.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://fr.gzmigu.cn

TS:   String(42)
来源：http://cd.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kr.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://ib.asd995.cn

Ruby: 42.to_s
来源：http://qs.hahajie.cn

C#:   42.ToString()
来源：http://fi.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://hh.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dq.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cf.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dg.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pg.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ew.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://er.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sh.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://df.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://xv.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rm.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jh.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qy.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fz.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://si.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pe.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wd.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pu.gzmigu.cn

[A10] 生成随机数
来源：http://ko.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://tc.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://uw.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ts.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://no.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://zy.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xo.chemitech.net.cn

Ruby: rand(1..100)
来源：http://xt.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://cx.colortex.cn

[A11] 条件表达式（三元）
来源：http://ei.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://lf.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wf.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yj.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pr.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wt.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tw.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ei.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lo.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://nm.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ii.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://um.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://qa.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://uk.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://rq.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ld.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://rm.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://qo.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sn.9csxet.cn

Py:   "第一行\n第二行"
来源：http://qe.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://xx.hahajie.cn

JS:   "第一行\n第二行"
来源：http://xp.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://qi.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ew.colortex.cn

Go:   "第一行\n第二行"
来源：http://zb.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://eo.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://fv.chemitech.net.cn

[A14] 注释写法
来源：http://ao.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qb.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bf.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ha.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://pq.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ik.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://iv.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hi.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://qj.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://fw.panjiajie.cn

Py:   value = data or "默认值"
来源：http://sg.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://ad.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://uo.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://wt.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yp.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://az.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://qq.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://xw.panjiajie.cn

[A16] 真假值判断规则
来源：http://td.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ph.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rt.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vg.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://qf.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gw.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hx.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wz.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vr.huixiangedu.cn

[A17] 位运算
来源：http://zu.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ba.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fm.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sk.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jw.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kc.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oh.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://tk.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://sy.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://nw.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ng.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nh.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://er.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://us.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://om.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://pg.colortex.cn

[A19] 交换两个变量
来源：http://wr.hnjuh.cn

Py:   a, b = b, a
来源：http://pc.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uu.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://py.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ox.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://th.huanxung.cn

Go:   a, b = b, a
来源：http://ph.asd995.cn

Ruby: a, b = b, a
来源：http://xw.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://rz.haigaiapp.cn

[A20] 读取标准输入
来源：http://jl.szsharing.cn

Py:   name = input("请输入：")
来源：http://gt.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ng.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zn.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://hs.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://rv.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pm.shtwfgs.cn

Ruby: gets.chomp
来源：http://gs.hahajie.cn

C#:   Console.ReadLine();
来源：http://ro.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ra.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://mm.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ok.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://sc.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://sb.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://bp.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xh.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://uo.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://da.colortex.cn

[A22] 获取字符串长度
来源：http://bx.panjiajie.cn

Py:   len(s)
来源：http://pb.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hy.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ou.nicolike.cn

TS:   s.length
来源：http://ov.chemitech.net.cn

Java: s.length()
来源：http://hk.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ri.szsharing.cn

Ruby: s.length
来源：http://iy.chemitech.net.cn

C#:   s.Length
来源：http://ax.wgjwhj.cn

[A23] 大小写转换
来源：http://aj.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sd.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jd.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jv.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fa.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bj.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tv.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fa.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qg.lnxyls.cn

[A24] 去除首尾空白
来源：http://se.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ny.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tu.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ts.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ad.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://up.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://ii.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hm.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qg.szxytkj.cn

[A25] 字符串比较
来源：http://ap.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://pt.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jb.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qe.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rx.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wi.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dd.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eu.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.hahajie.cn

[A26] 类型转换总览
来源：http://sg.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xx.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kl.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ie.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://qz.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mu.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yn.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mp.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fu.szsharing.cn

================================================================================
来源：http://zx.huixiangedu.cn

B. 流程控制
来源：http://ub.chemitech.net.cn

================================================================================
来源：http://lm.huanxung.cn

[B01] 条件判断 if / else
来源：http://pt.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uj.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uu.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hs.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rp.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ef.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zl.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xv.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kn.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://kr.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tz.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dr.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fg.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sz.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vg.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gg.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lg.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rv.asd995.cn

[B03] switch / match / case
来源：http://au.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kx.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ez.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ai.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pk.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rc.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ds.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tt.lnxyls.cn

[B04] for 计数循环
来源：http://bz.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://qh.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vq.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ty.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rf.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rx.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ek.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://um.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ak.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://xw.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://dn.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sx.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nn.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uq.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ie.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tt.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://ne.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mi.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://yd.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fa.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fo.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tg.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ep.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bh.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tm.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://he.nicolike.cn

[B07] while 循环
来源：http://wj.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://hs.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rs.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://be.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://ui.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://df.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gx.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://td.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://ke.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://wl.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://mf.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ht.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://ks.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://uo.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://dy.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://er.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tb.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://he.521024.cn

[B09] break 与 continue
来源：http://fr.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ub.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ki.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ns.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kg.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://vl.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gb.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wn.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ey.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yt.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mv.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nm.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://st.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ji.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://lz.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ak.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://li.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gq.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mr.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ss.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ia.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://eo.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nt.hnjuh.cn

[B12] 跳出多层循环
来源：http://yy.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pb.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yc.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vz.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kz.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fl.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gl.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qv.haigaiapp.cn

[B13] 判断是否为数字
来源：http://oj.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://tc.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://oo.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lx.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zc.521024.cn

Java: x instanceof Number
来源：http://vz.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xz.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ou.szxytkj.cn


<!-- 参考信息 -->