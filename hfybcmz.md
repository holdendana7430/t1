代发 wailian999

Ruby: 42.to_s
来源：http://at.asd995.cn

C#:   42.ToString()
来源：http://uu.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://ln.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yq.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mo.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fe.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ss.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mg.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rl.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jt.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hs.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://so.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ui.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://om.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fa.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cs.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sp.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://br.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qw.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://br.newstarts.cn

[A10] 生成随机数
来源：http://hz.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://vy.asd995.cn

PHP:  random_int(1, 100);
来源：http://xo.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xb.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zf.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ml.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ih.huanxung.cn

Ruby: rand(1..100)
来源：http://hf.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://ue.nszjky.cn

[A11] 条件表达式（三元）
来源：http://bc.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://ur.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ub.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ei.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fd.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yd.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yw.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dc.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://io.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://om.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oi.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xt.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://jk.521024.cn

TS:   `Hello, ${name}!`
来源：http://ay.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://sn.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hj.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://gi.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://hv.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ik.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://pv.521024.cn

PHP:  "第一行\n第二行"
来源：http://je.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://mu.nszjky.cn

TS:   "第一行\n第二行"
来源：http://pq.nicolike.cn

Java: "第一行\n第二行"
来源：http://pr.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://au.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ze.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://ui.haigaiapp.cn

[A14] 注释写法
来源：http://vs.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fi.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gt.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://qd.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://bv.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://al.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://uk.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mh.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://eu.newstarts.cn

[A15] 空值判断与默认值
来源：http://rp.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://id.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://oo.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ay.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://xx.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nm.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://wm.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://uo.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://nj.nszjky.cn

[A16] 真假值判断规则
来源：http://ia.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dv.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bm.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://if.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://pi.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kk.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tw.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hi.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hx.lnxyls.cn

[A17] 位运算
来源：http://lu.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ac.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ju.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://md.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uw.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ec.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://li.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://vo.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://sq.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qc.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ql.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://mz.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lw.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://cb.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://wh.9csxet.cn

[A19] 交换两个变量
来源：http://kb.lnxyls.cn

Py:   a, b = b, a
来源：http://xu.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zr.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ph.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://sf.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://lw.hnjuh.cn

Go:   a, b = b, a
来源：http://fb.huanxung.cn

Ruby: a, b = b, a
来源：http://aq.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://ou.panjiajie.cn

[A20] 读取标准输入
来源：http://yo.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://qo.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ho.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tw.521024.cn

TS:   // Node.js：readline 模块
来源：http://sf.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://zv.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pz.nicolike.cn

Ruby: gets.chomp
来源：http://qh.hahajie.cn

C#:   Console.ReadLine();
来源：http://kb.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://xc.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://lo.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mu.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://hw.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://cx.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://ib.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dv.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://eo.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://mw.bjjhwx.cn

[A22] 获取字符串长度
来源：http://pc.jctech888.com.cn

Py:   len(s)
来源：http://ki.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hm.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zk.panjiajie.cn

TS:   s.length
来源：http://zl.nszjky.cn

Java: s.length()
来源：http://qk.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zi.szsharing.cn

Ruby: s.length
来源：http://dp.gzmigu.cn

C#:   s.Length
来源：http://sw.szsharing.cn

[A23] 大小写转换
来源：http://da.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ds.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qi.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://st.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yl.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wt.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mx.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cc.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://my.9csxet.cn

[A24] 去除首尾空白
来源：http://lt.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aj.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ze.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ae.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qq.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://es.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xg.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nq.haigaiapp.cn

[A25] 字符串比较
来源：http://iu.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://fw.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jv.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nm.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bk.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ht.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yd.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://si.muxihuayi.cn

[A26] 类型转换总览
来源：http://lp.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zt.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xz.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://om.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://ky.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fh.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pt.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aq.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://em.colortex.cn

================================================================================
来源：http://qz.wgjwhj.cn

B. 流程控制
来源：http://hx.hnjuh.cn

================================================================================
来源：http://pl.newstarts.cn

[B01] 条件判断 if / else
来源：http://hx.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ll.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wh.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nk.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sv.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sz.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nd.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rz.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://td.521024.cn

[B02] 多分支 else if / elif
来源：http://lp.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rs.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eh.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yt.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cy.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.bjjhwx.cn

[B03] switch / match / case
来源：http://jd.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ol.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yt.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tf.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kt.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rr.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qc.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ks.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mm.muxihuayi.cn

[B04] for 计数循环
来源：http://tt.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://uw.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://po.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rs.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lu.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pc.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://su.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://iv.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mo.asd995.cn

[B05] 遍历数组 / 列表
来源：http://mz.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ex.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dq.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qe.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lm.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ug.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ct.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://tf.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sw.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://dy.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hc.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pr.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zc.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lu.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vv.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ql.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sa.chemitech.net.cn

[B07] while 循环
来源：http://uw.szsharing.cn

Py:   while i < 10: i += 1
来源：http://br.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dg.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://li.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://gm.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://dc.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ny.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://hz.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://ow.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://my.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://qp.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bp.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://xe.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://og.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://mw.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rd.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ql.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://kd.shxzukj.cn

[B09] break 与 continue
来源：http://gk.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bx.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ec.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zj.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://px.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ww.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jc.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.nicolike.cn

[B10] 遍历同时拿索引
来源：http://lu.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://de.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fu.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mp.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dn.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dl.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bx.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uk.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ek.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://jt.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://yd.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://al.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lk.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jx.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tp.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ag.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://hd.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vl.newstarts.cn

[B12] 跳出多层循环
来源：http://ef.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pd.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pa.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rt.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://il.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fp.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ou.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dp.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fk.shxzskj.cn

[B13] 判断是否为数字
来源：http://wy.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://jk.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://jt.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bz.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yj.bookmarksfly.cn

Java: x instanceof Number
来源：http://te.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rp.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ng.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://hl.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://hz.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://de.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mw.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://yj.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://un.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lk.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://is.yuexingan06.cn


<!-- 参考信息 -->