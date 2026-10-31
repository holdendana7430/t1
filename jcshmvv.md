代发 wailian999

Ruby: 42.to_s
来源：http://ih.szxytkj.cn

C#:   42.ToString()
来源：http://bi.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://zg.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jk.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ju.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jp.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qm.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yu.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mv.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://re.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ls.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://ta.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ab.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dh.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ng.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fc.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://da.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tu.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rz.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zo.jianghongdianzi.cn

[A10] 生成随机数
来源：http://sn.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://he.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://mk.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jn.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mg.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://mz.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xo.huixiangedu.cn

Ruby: rand(1..100)
来源：http://ii.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://gr.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://rc.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://md.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mh.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wb.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rj.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://et.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fm.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yr.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gs.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://oj.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mj.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://go.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://gn.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://ig.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://jj.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ws.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://ki.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://wb.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pb.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://xo.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://pk.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://ta.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://ve.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://tf.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://wp.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://yj.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://hj.shxzukj.cn

[A14] 注释写法
来源：http://nc.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bg.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wn.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://ah.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://pi.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mj.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://ai.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rx.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://do.gzmigu.cn

[A15] 空值判断与默认值
来源：http://sn.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://rj.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://nt.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://ix.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://zb.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yf.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://rx.nicolike.cn

Ruby: value = data || "默认值"
来源：http://pd.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://jn.muxihuayi.cn

[A16] 真假值判断规则
来源：http://tq.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ee.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hx.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bc.jctech888.com.cn

TS:   if (!x) {}
来源：http://ba.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iw.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zs.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ex.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://np.hnjuh.cn

[A17] 位运算
来源：http://ow.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pm.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nk.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zz.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kk.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wf.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://nv.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://kx.521024.cn

PHP:  ord("A"); chr(65)
来源：http://kl.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://co.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://xe.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kp.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://nt.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://da.hahajie.cn

[A19] 交换两个变量
来源：http://ed.9csxet.cn

Py:   a, b = b, a
来源：http://ll.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yg.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ze.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ca.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://ao.521024.cn

Go:   a, b = b, a
来源：http://jm.bjjhwx.cn

Ruby: a, b = b, a
来源：http://zv.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://gf.szxytkj.cn

[A20] 读取标准输入
来源：http://ls.nicolike.cn

Py:   name = input("请输入：")
来源：http://yv.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rw.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ww.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://zi.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://tx.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ca.huanxung.cn

Ruby: gets.chomp
来源：http://em.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://za.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://xw.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://sr.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hm.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://jr.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://dd.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://pq.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uv.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://mr.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ls.huixiangedu.cn

[A22] 获取字符串长度
来源：http://bk.yuexingan06.cn

Py:   len(s)
来源：http://mn.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fv.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hm.hnjuh.cn

TS:   s.length
来源：http://da.bookmarksfly.cn

Java: s.length()
来源：http://ad.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zk.shtwfgs.cn

Ruby: s.length
来源：http://jr.gzmigu.cn

C#:   s.Length
来源：http://vh.nicolike.cn

[A23] 大小写转换
来源：http://rs.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xe.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sy.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wc.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ml.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nq.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lo.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ph.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hf.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://wx.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pd.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ei.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gh.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gh.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ui.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://ee.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bt.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uf.gzmigu.cn

[A25] 字符串比较
来源：http://li.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://br.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mn.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hq.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://of.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mk.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rx.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vy.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sq.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://hc.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ya.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ur.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ux.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://kj.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vr.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oz.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bf.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://su.gzmigu.cn

================================================================================
来源：http://ak.haigaiapp.cn

B. 流程控制
来源：http://kp.yuexingan06.cn

================================================================================
来源：http://rr.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://vx.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hb.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kp.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dx.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gf.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mw.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sh.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mq.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://yh.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dn.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ar.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tn.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yd.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nh.shxzskj.cn

[B03] switch / match / case
来源：http://eu.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ti.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ha.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jx.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ab.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dd.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oj.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ad.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kj.asd995.cn

[B04] for 计数循环
来源：http://sf.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://ko.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zl.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rp.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iw.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tv.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://kn.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fm.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://bk.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://lt.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://td.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uo.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xm.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ij.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sq.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://rx.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://js.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://si.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ys.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nv.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ov.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dw.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ky.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ts.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qk.shxzukj.cn

[B07] while 循环
来源：http://ty.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://it.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nn.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://km.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://io.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://wa.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nt.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ie.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://hs.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://wf.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://sv.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hw.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://ci.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://ee.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://nm.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vg.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yd.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://vx.nicolike.cn

[B09] break 与 continue
来源：http://aj.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pk.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ia.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lm.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vy.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://as.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wk.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://mk.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ra.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://st.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zx.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nw.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lp.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gx.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xb.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ys.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://jx.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://hf.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://jp.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sr.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yn.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sy.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qa.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fo.nicolike.cn

[B12] 跳出多层循环
来源：http://og.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zi.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kg.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tt.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yo.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fm.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xs.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ot.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ca.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ok.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://if.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://pe.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ch.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://to.panjiajie.cn

Java: x instanceof Number
来源：http://bo.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lf.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://lf.shxzukj.cn

C#:   x is int or double or decimal
来源：http://rz.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://fx.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://la.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bw.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://az.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://nb.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sc.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sd.huixiangedu.cn


<!-- 参考信息 -->