代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zh.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dy.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://io.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pc.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zo.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qi.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ct.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://cw.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wv.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://na.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yp.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yz.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gr.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rd.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hf.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mf.jianghongdianzi.cn

[A10] 生成随机数
来源：http://xc.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://vr.hahajie.cn

PHP:  random_int(1, 100);
来源：http://vq.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wu.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nu.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ka.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rn.asd995.cn

Ruby: rand(1..100)
来源：http://jh.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://ka.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://km.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://ij.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bb.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qz.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://or.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://uq.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yn.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aa.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yc.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://wg.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xp.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yy.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://ey.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://fr.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://fg.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xp.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://lu.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://cd.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ts.colortex.cn

Py:   "第一行\n第二行"
来源：http://hr.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://dh.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://wx.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://md.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://tw.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://zf.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://fx.asd995.cn

C#:   "第一行\n第二行"
来源：http://ua.gzmigu.cn

[A14] 注释写法
来源：http://ot.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://um.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dn.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://xo.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ss.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ja.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://eb.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wd.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://sw.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://na.hahajie.cn

Py:   value = data or "默认值"
来源：http://fq.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ws.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://de.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://ly.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jv.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://rv.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://at.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://ov.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://ac.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://po.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nz.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sm.colortex.cn

TS:   if (!x) {}
来源：http://ri.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yz.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rh.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vn.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cz.huixiangedu.cn

[A17] 位运算
来源：http://lm.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://em.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bx.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zf.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gj.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ua.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nz.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://ij.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://yl.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://lg.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wx.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://st.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://yo.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://do.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://sb.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://xt.nszjky.cn

[A19] 交换两个变量
来源：http://eh.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://xj.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tj.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://kc.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://qe.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://le.huanxung.cn

Go:   a, b = b, a
来源：http://gh.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://st.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://oh.szxytkj.cn

[A20] 读取标准输入
来源：http://ir.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://fe.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fr.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nl.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ou.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://ds.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pt.nicolike.cn

Ruby: gets.chomp
来源：http://ri.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://gf.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://hn.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://mp.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iy.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://mr.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://qm.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://iz.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cj.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://ah.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://au.nicolike.cn

[A22] 获取字符串长度
来源：http://yc.shtwfgs.cn

Py:   len(s)
来源：http://sv.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ag.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vs.nicolike.cn

TS:   s.length
来源：http://xt.9csxet.cn

Java: s.length()
来源：http://dj.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ed.yuntaijiaju.cn

Ruby: s.length
来源：http://gf.colortex.cn

C#:   s.Length
来源：http://yk.bookmarksfly.cn

[A23] 大小写转换
来源：http://sv.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ca.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fx.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ih.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ax.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hy.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yg.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hy.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qx.panjiajie.cn

[A24] 去除首尾空白
来源：http://xv.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ni.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zs.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qx.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gr.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ho.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ae.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zx.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rp.hahajie.cn

[A25] 字符串比较
来源：http://mf.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://xn.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mp.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ic.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nk.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zu.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://np.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uy.asd995.cn

[A26] 类型转换总览
来源：http://rs.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://px.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mp.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ls.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://uy.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eq.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ko.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mw.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kw.jctech888.com.cn

================================================================================
来源：http://vb.colortex.cn

B. 流程控制
来源：http://yz.asd995.cn

================================================================================
来源：http://xh.gzmigu.cn

[B01] 条件判断 if / else
来源：http://st.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bs.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sd.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ch.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pc.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ye.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tj.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pn.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ri.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://xy.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sq.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://go.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yw.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gi.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iy.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.newstarts.cn

[B03] switch / match / case
来源：http://zy.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mb.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ts.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xw.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yj.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jj.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fb.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dq.nszjky.cn

[B04] for 计数循环
来源：http://uu.521024.cn

Py:   for i in range(10): print(i)
来源：http://zz.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ri.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nw.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kz.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://no.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yk.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://be.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jy.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://fo.521024.cn

Py:   for item in arr: print(item)
来源：http://aq.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ev.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jy.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://of.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sp.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sb.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://ey.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wr.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://eo.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gf.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kc.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://if.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kh.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rj.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kf.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rl.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cw.asd995.cn

[B07] while 循环
来源：http://as.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ju.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ak.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://ye.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://ht.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://zc.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tq.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://lj.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://mt.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://dk.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ep.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iw.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://tg.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://aq.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://ig.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zd.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vp.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://rs.nszjky.cn

[B09] break 与 continue
来源：http://ng.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lw.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jo.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gg.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://en.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://st.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.newstarts.cn

[B10] 遍历同时拿索引
来源：http://cv.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hm.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ng.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mm.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iz.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bc.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ka.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vz.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xg.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://yz.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://la.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://xz.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fs.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dp.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dp.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ie.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://jf.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ui.colortex.cn

[B12] 跳出多层循环
来源：http://tb.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lj.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jf.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yx.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qz.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rx.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rq.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zd.bjjhwx.cn

[B13] 判断是否为数字
来源：http://qr.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://ee.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://gx.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pa.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fo.shtwfgs.cn

Java: x instanceof Number
来源：http://hz.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ve.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ra.panjiajie.cn

C#:   x is int or double or decimal
来源：http://fr.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://qr.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cc.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ds.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://nf.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nc.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qs.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://df.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vq.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tl.szsharing.cn

[B15] 布尔运算与取反
来源：http://ba.szsharing.cn

Py:   a and b or not c
来源：http://cn.lnxyls.cn


<!-- 参考信息 -->