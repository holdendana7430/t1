代发 wailian999

[A06] 字符串转数字
来源：http://wj.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://am.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vz.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tf.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pt.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fp.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bl.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mo.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hh.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://wx.huanxung.cn

Py:   str(42)
来源：http://af.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://cl.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://uw.jianghongdianzi.cn

TS:   String(42)
来源：http://ck.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xx.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://tp.wgjwhj.cn

Ruby: 42.to_s
来源：http://qc.szxytkj.cn

C#:   42.ToString()
来源：http://lo.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://kn.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fd.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dj.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fi.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yd.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lc.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fx.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fb.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sw.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://wj.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kh.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tl.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uz.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://op.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qf.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mj.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aw.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xv.chemitech.net.cn

[A10] 生成随机数
来源：http://jq.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://ae.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://jj.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pa.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ii.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://bj.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ad.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://he.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://kn.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://kp.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://xr.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://el.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://is.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yk.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://pd.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ji.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ma.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wq.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://ek.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lp.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vt.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://vu.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://rd.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://fx.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://on.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://gt.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://gk.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lu.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://jx.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://ts.szsharing.cn

JS:   "第一行\n第二行"
来源：http://yd.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://ol.hahajie.cn

Java: "第一行\n第二行"
来源：http://hw.9csxet.cn

Go:   "第一行\n第二行"
来源：http://eh.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://vx.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://cf.szsharing.cn

[A14] 注释写法
来源：http://pf.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hq.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oc.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://gf.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ag.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hy.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://fk.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wa.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://dx.521024.cn

[A15] 空值判断与默认值
来源：http://ct.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://nf.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://ww.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://gl.521024.cn

TS:   const value = data ?? "默认值";
来源：http://ei.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oa.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://vy.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://or.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://fw.lnxyls.cn

[A16] 真假值判断规则
来源：http://ti.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sa.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ma.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qd.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://mt.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vp.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rx.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kn.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rr.huanxung.cn

[A17] 位运算
来源：http://qo.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xl.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fh.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wv.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bc.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://fu.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://lu.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ky.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zo.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hh.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://pu.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://da.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://ch.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://qp.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://tf.yuexingan06.cn

Py:   a, b = b, a
来源：http://ii.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yv.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://dc.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://lm.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://yv.hahajie.cn

Go:   a, b = b, a
来源：http://ur.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://it.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://vi.nicolike.cn

[A20] 读取标准输入
来源：http://un.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://at.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hx.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mm.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://bs.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://ap.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qn.shtwfgs.cn

Ruby: gets.chomp
来源：http://nw.szxytkj.cn

C#:   Console.ReadLine();
来源：http://pj.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://au.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dl.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://oj.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://af.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://ub.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://du.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://jc.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://wa.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ef.shtwfgs.cn

Py:   len(s)
来源：http://ls.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xs.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yd.szsharing.cn

TS:   s.length
来源：http://cg.yuntaijiaju.cn

Java: s.length()
来源：http://wu.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jn.newstarts.cn

Ruby: s.length
来源：http://mr.muxihuayi.cn

C#:   s.Length
来源：http://jm.lnxyls.cn

[A23] 大小写转换
来源：http://ua.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jj.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rp.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iu.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ui.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aq.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ib.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tx.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://we.szsharing.cn

[A24] 去除首尾空白
来源：http://fd.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yl.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zs.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qi.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zc.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://vq.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cn.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://do.yuexingan06.cn

[A25] 字符串比较
来源：http://ue.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://io.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xo.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ku.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wo.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pz.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rl.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://us.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xe.nicolike.cn

[A26] 类型转换总览
来源：http://ue.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kx.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eu.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xj.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://kx.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://za.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://je.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ab.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bt.nszjky.cn

================================================================================
来源：http://kh.wgjwhj.cn

B. 流程控制
来源：http://iu.gzmigu.cn

================================================================================
来源：http://tt.lnxyls.cn

[B01] 条件判断 if / else
来源：http://aj.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ao.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qg.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xm.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zx.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ox.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hq.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hd.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://im.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://pi.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rx.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yg.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mi.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cv.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ma.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bf.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.muxihuayi.cn

[B03] switch / match / case
来源：http://nq.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pq.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wk.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rq.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vv.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sb.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wr.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cb.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qz.lnxyls.cn

[B04] for 计数循环
来源：http://ac.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://pp.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ab.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pq.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eh.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ch.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ma.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://wn.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zz.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://lf.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://za.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rn.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hq.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xk.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vq.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nu.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://bx.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yl.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://vd.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vt.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yj.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nr.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bk.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tz.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qy.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ar.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vx.huanxung.cn

[B07] while 循环
来源：http://ek.huanxung.cn

Py:   while i < 10: i += 1
来源：http://fd.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zf.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://es.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://dp.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://zy.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ez.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://da.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://bu.asd995.cn

[B08] do-while（至少执行一次）
来源：http://yq.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://th.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dd.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://pf.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://rf.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://bt.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lr.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cm.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://kv.shxzskj.cn

[B09] break 与 continue
来源：http://dv.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cq.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yt.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qn.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nf.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://da.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qi.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://do.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://xp.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dx.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jn.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ph.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cc.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rc.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rk.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rj.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yn.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://mg.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://wm.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://ff.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zf.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ep.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bm.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://zz.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gi.shxzskj.cn

[B12] 跳出多层循环
来源：http://st.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ki.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bm.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ma.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tz.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bq.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hm.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rv.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ft.9csxet.cn


<!-- 参考信息 -->