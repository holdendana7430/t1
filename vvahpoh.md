代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kd.huixiangedu.cn

[A07] 数字转字符串
来源：http://aq.yuexingan06.cn

Py:   str(42)
来源：http://ox.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://um.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://ac.shtwfgs.cn

TS:   String(42)
来源：http://uu.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vh.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://pv.huixiangedu.cn

Ruby: 42.to_s
来源：http://oo.bookmarksfly.cn

C#:   42.ToString()
来源：http://sy.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://qc.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tl.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aw.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ca.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ff.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yk.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://or.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cw.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qp.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://bi.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ss.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pi.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hp.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cs.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://on.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ws.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kp.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ee.szsharing.cn

[A10] 生成随机数
来源：http://oc.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://wq.nszjky.cn

PHP:  random_int(1, 100);
来源：http://wv.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jp.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xn.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://tk.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ci.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://to.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://vf.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://yt.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://qi.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://oj.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ui.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ao.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://bt.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zp.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tt.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xr.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://yl.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wx.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lx.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://aq.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ur.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://ek.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uk.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://ui.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://zu.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tx.9csxet.cn

Py:   "第一行\n第二行"
来源：http://yd.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://ss.hahajie.cn

JS:   "第一行\n第二行"
来源：http://yo.nszjky.cn

TS:   "第一行\n第二行"
来源：http://dn.shxzskj.cn

Java: "第一行\n第二行"
来源：http://na.asd995.cn

Go:   "第一行\n第二行"
来源：http://wr.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://mw.newstarts.cn

C#:   "第一行\n第二行"
来源：http://mr.panjiajie.cn

[A14] 注释写法
来源：http://gd.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cy.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://di.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://mu.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://ps.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gq.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://of.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hg.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://lt.shxzukj.cn

[A15] 空值判断与默认值
来源：http://jx.asd995.cn

Py:   value = data or "默认值"
来源：http://qo.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://jv.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://fi.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://dr.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://po.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://tf.hahajie.cn

Ruby: value = data || "默认值"
来源：http://an.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://bw.szsharing.cn

[A16] 真假值判断规则
来源：http://zf.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xu.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cc.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lu.jctech888.com.cn

TS:   if (!x) {}
来源：http://wj.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pr.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nr.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wi.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qx.shxzskj.cn

[A17] 位运算
来源：http://qy.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://th.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zz.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dk.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bo.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ct.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qs.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://np.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://is.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://bv.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pm.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ey.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://yo.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xi.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://lf.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://ei.chemitech.net.cn

[A19] 交换两个变量
来源：http://fz.hahajie.cn

Py:   a, b = b, a
来源：http://qk.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jw.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ph.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://vm.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://eu.huixiangedu.cn

Go:   a, b = b, a
来源：http://hy.shxzukj.cn

Ruby: a, b = b, a
来源：http://eb.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://kx.szxytkj.cn

[A20] 读取标准输入
来源：http://xs.hahajie.cn

Py:   name = input("请输入：")
来源：http://pi.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://os.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cz.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://qz.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://hj.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zd.bookmarksfly.cn

Ruby: gets.chomp
来源：http://oy.shxzskj.cn

C#:   Console.ReadLine();
来源：http://zs.colortex.cn

[A21] 保留指定小数位输出
来源：http://tg.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://qp.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://be.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ow.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://yf.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://kg.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nj.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ln.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://eu.chemitech.net.cn

[A22] 获取字符串长度
来源：http://nd.colortex.cn

Py:   len(s)
来源：http://fz.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bw.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zc.gzmigu.cn

TS:   s.length
来源：http://pg.bookmarksfly.cn

Java: s.length()
来源：http://sd.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kj.hnjuh.cn

Ruby: s.length
来源：http://yd.shxzskj.cn

C#:   s.Length
来源：http://zn.szxytkj.cn

[A23] 大小写转换
来源：http://lm.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vt.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yg.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dn.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gt.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pd.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uc.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pm.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lr.bjjhwx.cn

[A24] 去除首尾空白
来源：http://cg.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wa.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bi.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pu.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ap.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fl.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://dx.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ad.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vl.chemitech.net.cn

[A25] 字符串比较
来源：http://nn.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://fd.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fr.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mq.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ep.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ry.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bj.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ja.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kc.colortex.cn

[A26] 类型转换总览
来源：http://ec.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xr.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ar.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sb.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://gc.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lj.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lr.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vs.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://it.521024.cn

================================================================================
来源：http://cg.jianghongdianzi.cn

B. 流程控制
来源：http://ph.panjiajie.cn

================================================================================
来源：http://gn.shxzskj.cn

[B01] 条件判断 if / else
来源：http://is.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xc.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eg.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dl.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rt.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vf.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oq.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ko.newstarts.cn

[B02] 多分支 else if / elif
来源：http://fv.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lg.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xi.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ww.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ra.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.muxihuayi.cn

[B03] switch / match / case
来源：http://qz.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://od.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mt.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ad.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://in.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tr.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pv.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bj.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fv.asd995.cn

[B04] for 计数循环
来源：http://lm.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://pa.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oz.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gb.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ok.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ct.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ut.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://rq.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fu.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://ke.nicolike.cn

Py:   for item in arr: print(item)
来源：http://sg.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://we.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://as.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hu.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gp.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nh.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://om.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xx.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://yz.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cd.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xd.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ol.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hv.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wk.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bn.huixinmuqiang.cn

[B07] while 循环
来源：http://ht.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://zu.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gp.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://lo.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://eh.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://xi.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://om.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://pl.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ha.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://oe.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://eo.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mm.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://ya.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://jw.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://vl.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rf.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ih.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ea.jctech888.com.cn

[B09] break 与 continue
来源：http://ss.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hu.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rx.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dd.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dl.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eb.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://li.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dw.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hv.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gq.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mq.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tv.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kq.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cu.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pc.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://yw.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://ts.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://vy.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gk.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://es.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ur.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eq.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://fj.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ah.lnxyls.cn

[B12] 跳出多层循环
来源：http://ss.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://al.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bi.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nk.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bq.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nt.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rt.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lm.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zd.huixiangedu.cn

[B13] 判断是否为数字
来源：http://nc.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://my.gzmigu.cn

PHP:  is_numeric($x)
来源：http://sp.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yo.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ja.jctech888.com.cn

Java: x instanceof Number
来源：http://lg.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jl.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.wgjwhj.cn


<!-- 参考信息 -->