代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://oe.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cu.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yx.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xa.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wu.panjiajie.cn

[A07] 数字转字符串
来源：http://lj.haigaiapp.cn

Py:   str(42)
来源：http://ke.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://pa.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://nd.colortex.cn

TS:   String(42)
来源：http://cw.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rw.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://ss.521024.cn

Ruby: 42.to_s
来源：http://sw.szsharing.cn

C#:   42.ToString()
来源：http://ox.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://kw.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bb.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nw.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mg.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kp.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cm.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ml.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nc.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nn.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://kk.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wh.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ti.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ly.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ec.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cw.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ha.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uc.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ey.gzmigu.cn

[A10] 生成随机数
来源：http://no.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://mu.huanxung.cn

PHP:  random_int(1, 100);
来源：http://sc.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qn.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://el.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://ri.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eu.521024.cn

Ruby: rand(1..100)
来源：http://fx.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://hw.nszjky.cn

[A11] 条件表达式（三元）
来源：http://bb.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://qe.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gu.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xr.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ed.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://el.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xb.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fg.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rd.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://yp.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rn.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fc.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://fl.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://yl.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://vj.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mv.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://hv.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://tk.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pq.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://sv.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://bn.newstarts.cn

JS:   "第一行\n第二行"
来源：http://zk.colortex.cn

TS:   "第一行\n第二行"
来源：http://uw.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://jx.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://vg.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ei.huanxung.cn

C#:   "第一行\n第二行"
来源：http://et.szxytkj.cn

[A14] 注释写法
来源：http://kd.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ej.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nw.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://dm.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://qc.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bt.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://ow.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xy.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://tb.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://rg.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://gm.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://zk.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://lf.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ea.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://js.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://mf.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://zr.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://eu.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://yp.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://il.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ls.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rn.9csxet.cn

TS:   if (!x) {}
来源：http://hl.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mm.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qh.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ss.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iv.jctech888.com.cn

[A17] 位运算
来源：http://xa.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bo.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sh.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mh.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sl.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wy.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://iy.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://tb.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://zl.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lm.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ov.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://yk.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bq.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://rp.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://fb.asd995.cn

[A19] 交换两个变量
来源：http://ch.9csxet.cn

Py:   a, b = b, a
来源：http://pr.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uw.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://bj.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://hv.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://ah.chemitech.net.cn

Go:   a, b = b, a
来源：http://as.nicolike.cn

Ruby: a, b = b, a
来源：http://kn.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://zu.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ur.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://as.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dj.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ru.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://jd.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://en.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lu.shtwfgs.cn

Ruby: gets.chomp
来源：http://yq.nszjky.cn

C#:   Console.ReadLine();
来源：http://av.colortex.cn

[A21] 保留指定小数位输出
来源：http://il.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://va.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ua.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://of.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://wg.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://dv.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kd.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://lw.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://xj.colortex.cn

[A22] 获取字符串长度
来源：http://hu.9csxet.cn

Py:   len(s)
来源：http://fj.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vd.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aa.shxzukj.cn

TS:   s.length
来源：http://zl.muxihuayi.cn

Java: s.length()
来源：http://bo.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ja.newstarts.cn

Ruby: s.length
来源：http://yr.521024.cn

C#:   s.Length
来源：http://nh.haigaiapp.cn

[A23] 大小写转换
来源：http://yj.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zt.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cs.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://um.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zm.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zc.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tf.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ed.shxzukj.cn

[A24] 去除首尾空白
来源：http://tq.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ev.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rn.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ae.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uq.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://oe.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yv.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cw.yuexingan06.cn

[A25] 字符串比较
来源：http://qg.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://qa.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pb.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ps.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xa.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jo.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dm.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ca.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zr.huanxung.cn

[A26] 类型转换总览
来源：http://mi.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zn.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tu.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bj.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://se.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pf.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://on.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ss.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qi.jctech888.com.cn

================================================================================
来源：http://cu.huixiangedu.cn

B. 流程控制
来源：http://bf.lnxyls.cn

================================================================================
来源：http://ql.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://xt.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sh.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qx.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zi.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jo.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://su.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rs.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kk.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jd.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://bd.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ir.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nb.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iq.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bc.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vi.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cv.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xw.huixiangedu.cn

[B03] switch / match / case
来源：http://mr.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://by.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://es.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kh.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gc.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mz.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qr.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://an.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tj.muxihuayi.cn

[B04] for 计数循环
来源：http://pv.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://wn.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iy.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xw.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ib.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fn.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kz.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://kx.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qh.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://es.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ek.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bl.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ta.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lt.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://is.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jc.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://dl.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wq.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://lb.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ok.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ls.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jz.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ah.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://on.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aj.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zo.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://da.lnxyls.cn

[B07] while 循环
来源：http://ii.521024.cn

Py:   while i < 10: i += 1
来源：http://tp.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dj.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://ec.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://fn.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://mh.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mp.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://ik.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://zq.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://ka.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://wu.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ry.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://mo.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://ae.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://iz.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yz.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zm.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://hu.szsharing.cn

[B09] break 与 continue
来源：http://qu.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gi.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ex.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mq.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ox.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cn.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://lp.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iw.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rh.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kh.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ls.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zl.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://un.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fy.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hs.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://hy.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://oa.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://cq.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uu.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sr.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nt.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ov.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://cm.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sz.shxzskj.cn

[B12] 跳出多层循环
来源：http://sg.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tc.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ln.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hs.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bj.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lh.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mt.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://is.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hu.bjjhwx.cn

[B13] 判断是否为数字
来源：http://si.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://zt.asd995.cn

PHP:  is_numeric($x)
来源：http://ut.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jw.shxzukj.cn


<!-- 参考信息 -->