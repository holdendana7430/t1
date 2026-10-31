代发 wailian999

JS:   String(42); (42).toString()
来源：http://np.szxytkj.cn

TS:   String(42)
来源：http://ww.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://es.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://vo.bjjhwx.cn

Ruby: 42.to_s
来源：http://rc.huixiangedu.cn

C#:   42.ToString()
来源：http://pk.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://rb.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rt.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ea.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ic.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://og.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mh.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ut.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fa.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fz.asd995.cn

[A09] 绝对值与最大最小值
来源：http://pn.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qi.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ki.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ni.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kk.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vn.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://au.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vi.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rq.huanxung.cn

[A10] 生成随机数
来源：http://ev.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://of.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://fz.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iu.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cw.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://st.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://co.shxzukj.cn

Ruby: rand(1..100)
来源：http://pk.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://sg.huanxung.cn

[A11] 条件表达式（三元）
来源：http://jv.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://xa.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yp.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ap.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ra.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://af.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ac.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aj.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vl.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ky.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://is.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qa.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://ks.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://sd.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://xw.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://us.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://rr.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://xm.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yc.szsharing.cn

Py:   "第一行\n第二行"
来源：http://ii.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://rs.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://fk.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://oo.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://tx.newstarts.cn

Go:   "第一行\n第二行"
来源：http://vb.asd995.cn

Ruby: "第一行\n第二行"
来源：http://ez.asd995.cn

C#:   "第一行\n第二行"
来源：http://jy.bjjhwx.cn

[A14] 注释写法
来源：http://vt.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vr.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zs.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://bt.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://qf.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qu.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://ny.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vg.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://kg.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://ud.shxzskj.cn

Py:   value = data or "默认值"
来源：http://tg.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://qf.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://nw.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://ya.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hh.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ls.521024.cn

Ruby: value = data || "默认值"
来源：http://by.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://yy.521024.cn

[A16] 真假值判断规则
来源：http://st.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tc.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ud.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://wm.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dt.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oj.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xn.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cu.colortex.cn

[A17] 位运算
来源：http://ww.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rl.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://od.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lg.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://he.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tj.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mk.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://kr.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://wq.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://vy.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xb.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yu.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://bs.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://he.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://se.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://wj.nszjky.cn

[A19] 交换两个变量
来源：http://wr.huanxung.cn

Py:   a, b = b, a
来源：http://op.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ar.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://oz.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ya.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://gx.szsharing.cn

Go:   a, b = b, a
来源：http://al.521024.cn

Ruby: a, b = b, a
来源：http://pn.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://hl.szsharing.cn

[A20] 读取标准输入
来源：http://ba.9csxet.cn

Py:   name = input("请输入：")
来源：http://qb.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ht.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yr.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://hs.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ua.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nx.bookmarksfly.cn

Ruby: gets.chomp
来源：http://zn.szsharing.cn

C#:   Console.ReadLine();
来源：http://yo.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://gs.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://vi.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://di.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://tc.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://gl.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://kg.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vk.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://ul.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ky.newstarts.cn

[A22] 获取字符串长度
来源：http://sx.colortex.cn

Py:   len(s)
来源：http://jb.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ec.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vo.huixinmuqiang.cn

TS:   s.length
来源：http://nb.huixinmuqiang.cn

Java: s.length()
来源：http://pr.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://km.colortex.cn

Ruby: s.length
来源：http://ia.haigaiapp.cn

C#:   s.Length
来源：http://pp.newstarts.cn

[A23] 大小写转换
来源：http://ip.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qh.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ta.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lv.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oi.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pe.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dm.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gm.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qd.521024.cn

[A24] 去除首尾空白
来源：http://bc.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uq.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://we.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cf.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iu.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ey.521024.cn

Go:   strings.TrimSpace(s)
来源：http://ao.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xd.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://il.shxzukj.cn

[A25] 字符串比较
来源：http://sp.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://cc.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oc.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://al.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dg.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wh.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zh.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qn.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://im.jctech888.com.cn

[A26] 类型转换总览
来源：http://ja.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rw.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qa.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wf.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://cu.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://io.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sq.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ma.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xw.jianghongdianzi.cn

================================================================================
来源：http://ah.jctech888.com.cn

B. 流程控制
来源：http://mz.haigaiapp.cn

================================================================================
来源：http://et.9csxet.cn

[B01] 条件判断 if / else
来源：http://ia.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xi.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hq.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ji.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tb.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ww.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uf.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gn.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ex.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://wm.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iy.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cb.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hs.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qp.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ep.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pk.9csxet.cn

[B03] switch / match / case
来源：http://gm.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ro.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dj.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xu.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tr.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lh.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xj.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qs.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zy.yuexingan06.cn

[B04] for 计数循环
来源：http://gk.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://gw.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uh.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sc.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ao.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lp.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ss.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://pa.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mc.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://fg.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://yl.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yj.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ki.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qw.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yy.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pl.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://bj.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ei.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://rh.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sg.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kp.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mo.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ow.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qr.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://az.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ng.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dl.shtwfgs.cn

[B07] while 循环
来源：http://xo.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://zj.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tw.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://fj.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://et.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://ca.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kt.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://na.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://wj.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://jd.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://iz.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vl.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://sm.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://zv.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://wi.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ol.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mf.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://it.newstarts.cn

[B09] break 与 continue
来源：http://nk.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gg.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oc.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ok.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gl.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tf.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://su.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qw.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://es.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bf.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fc.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://as.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://us.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ip.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://on.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://vu.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://lu.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yo.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ca.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lz.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gk.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://sj.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.colortex.cn

[B12] 跳出多层循环
来源：http://uz.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iu.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yf.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://re.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oy.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://go.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qu.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://go.shxzukj.cn

[B13] 判断是否为数字
来源：http://fw.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://fj.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://zk.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kg.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jo.haigaiapp.cn

Java: x instanceof Number
来源：http://vl.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uv.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ln.lnxyls.cn

C#:   x is int or double or decimal
来源：http://yk.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://zc.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rp.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://do.muxihuayi.cn


<!-- 参考信息 -->