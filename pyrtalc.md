代发 wailian999

JS:   String(42); (42).toString()
来源：http://pc.szxytkj.cn

TS:   String(42)
来源：http://oi.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lt.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://iw.jctech888.com.cn

Ruby: 42.to_s
来源：http://qf.chemitech.net.cn

C#:   42.ToString()
来源：http://pr.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://yn.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bu.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xj.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lk.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jt.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zg.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hf.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ry.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hq.521024.cn

[A09] 绝对值与最大最小值
来源：http://il.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bd.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mh.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ux.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cn.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ki.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hg.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jc.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xy.huanxung.cn

[A10] 生成随机数
来源：http://az.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://pk.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://pp.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://io.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eo.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://vg.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aq.shtwfgs.cn

Ruby: rand(1..100)
来源：http://vr.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://fp.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://kn.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://fe.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aw.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aw.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gb.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://tx.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xn.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wa.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zu.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://fb.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pw.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qv.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://md.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://em.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://xs.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mf.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://yb.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://gr.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qa.szsharing.cn

Py:   "第一行\n第二行"
来源：http://hs.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://cb.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://th.colortex.cn

TS:   "第一行\n第二行"
来源：http://il.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://zx.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://dc.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://gb.hahajie.cn

C#:   "第一行\n第二行"
来源：http://io.szsharing.cn

[A14] 注释写法
来源：http://nu.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jt.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iv.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://vv.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://sk.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rd.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://jy.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zj.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://fp.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://pl.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://fq.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://yh.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://kb.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://cq.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wh.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://be.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://bi.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://rc.shtwfgs.cn

[A16] 真假值判断规则
来源：http://uk.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qm.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cz.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jw.jctech888.com.cn

TS:   if (!x) {}
来源：http://iy.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pk.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gt.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gn.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ft.hahajie.cn

[A17] 位运算
来源：http://jz.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nn.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://td.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rp.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lk.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qe.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://an.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://nr.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://cs.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://ob.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eu.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vm.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://lq.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nc.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://jd.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://uv.hnjuh.cn

[A19] 交换两个变量
来源：http://qp.nicolike.cn

Py:   a, b = b, a
来源：http://to.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://it.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://ze.521024.cn

TS:   [a, b] = [b, a];
来源：http://us.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://cn.huanxung.cn

Go:   a, b = b, a
来源：http://rb.9csxet.cn

Ruby: a, b = b, a
来源：http://uu.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://ii.shtwfgs.cn

[A20] 读取标准输入
来源：http://fq.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://mi.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ni.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zf.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://zl.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://st.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ls.haigaiapp.cn

Ruby: gets.chomp
来源：http://dp.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://mz.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ka.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://od.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gd.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ka.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://jx.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://bz.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ub.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://al.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://lk.haigaiapp.cn

[A22] 获取字符串长度
来源：http://fi.shtwfgs.cn

Py:   len(s)
来源：http://te.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kn.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kx.huixinmuqiang.cn

TS:   s.length
来源：http://xy.colortex.cn

Java: s.length()
来源：http://ko.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nd.gzmigu.cn

Ruby: s.length
来源：http://da.colortex.cn

C#:   s.Length
来源：http://cj.huixiangedu.cn

[A23] 大小写转换
来源：http://wn.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nd.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ul.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ei.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tp.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tl.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lz.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ys.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sc.chemitech.net.cn

[A24] 去除首尾空白
来源：http://gk.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ke.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bp.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mq.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jh.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yk.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://in.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://of.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tg.szsharing.cn

[A25] 字符串比较
来源：http://fy.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://oy.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://js.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vg.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://he.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://db.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lv.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ag.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ml.shtwfgs.cn

[A26] 类型转换总览
来源：http://gh.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xy.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rp.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ej.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://ej.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vb.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mo.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qn.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ko.muxihuayi.cn

================================================================================
来源：http://ss.newstarts.cn

B. 流程控制
来源：http://bx.szxytkj.cn

================================================================================
来源：http://fj.colortex.cn

[B01] 条件判断 if / else
来源：http://sz.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wy.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xd.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mt.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lu.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jq.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yb.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gi.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nb.nszjky.cn

[B02] 多分支 else if / elif
来源：http://bg.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sq.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lu.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kp.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fj.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ua.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://up.bookmarksfly.cn

[B03] switch / match / case
来源：http://nh.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ay.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ca.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dk.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qf.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bg.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lx.szxytkj.cn

[B04] for 计数循环
来源：http://tb.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://tx.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nx.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fb.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tv.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nd.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ws.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://so.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ci.colortex.cn

[B05] 遍历数组 / 列表
来源：http://om.asd995.cn

Py:   for item in arr: print(item)
来源：http://uj.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dx.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lk.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hu.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pm.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gr.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://sb.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rh.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://mv.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ai.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qg.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yv.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vm.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nh.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xp.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wc.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bh.shxzskj.cn

[B07] while 循环
来源：http://hr.colortex.cn

Py:   while i < 10: i += 1
来源：http://qe.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ar.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://mz.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://qt.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://om.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gj.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://do.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ki.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ll.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zh.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pu.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://gh.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://oy.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://kp.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bp.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zd.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://jg.newstarts.cn

[B09] break 与 continue
来源：http://hu.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ah.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vb.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nl.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ye.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vd.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ug.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://zn.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://st.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ce.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sp.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vl.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ym.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bj.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bq.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uc.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://kk.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://yh.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://sd.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dr.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://te.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ck.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://az.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://vy.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jh.panjiajie.cn

[B12] 跳出多层循环
来源：http://rb.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yb.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nx.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nx.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mp.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ml.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sz.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xa.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qp.huixiangedu.cn

[B13] 判断是否为数字
来源：http://wk.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://fo.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://fz.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mb.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://si.asd995.cn

Java: x instanceof Number
来源：http://wi.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://op.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://hx.newstarts.cn

C#:   x is int or double or decimal
来源：http://qe.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://rq.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kj.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kf.asd995.cn


<!-- 参考信息 -->