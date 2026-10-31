代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ni.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kx.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ud.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nh.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mj.shtwfgs.cn

[A07] 数字转字符串
来源：http://ko.huixinmuqiang.cn

Py:   str(42)
来源：http://lm.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://hd.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://jf.hahajie.cn

TS:   String(42)
来源：http://ce.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dl.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://ik.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://br.chemitech.net.cn

C#:   42.ToString()
来源：http://od.lnxyls.cn

[A08] 取整与四舍五入
来源：http://uz.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mf.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fi.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ao.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://si.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pa.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cv.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pr.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://as.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://wj.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ue.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tv.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uo.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xg.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mj.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oc.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ub.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://av.chemitech.net.cn

[A10] 生成随机数
来源：http://gn.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://ir.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://wy.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yg.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kr.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://ym.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hnjuh.cn

Ruby: rand(1..100)
来源：http://ef.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://yp.huanxung.cn

[A11] 条件表达式（三元）
来源：http://th.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://ju.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hx.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jz.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://li.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://zh.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nr.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jy.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ns.521024.cn

[A12] 字符串插值 / 格式化
来源：http://tp.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mp.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vc.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://kg.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://hy.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://nl.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mu.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://ap.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ig.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ei.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://sv.asd995.cn

PHP:  "第一行\n第二行"
来源：http://nz.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://xy.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://su.szsharing.cn

Java: "第一行\n第二行"
来源：http://jc.colortex.cn

Go:   "第一行\n第二行"
来源：http://ev.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://gc.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://kt.bookmarksfly.cn

[A14] 注释写法
来源：http://dn.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://up.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ja.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://dr.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://ky.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ti.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://cv.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nd.521024.cn

C#:   // 单行；/* 多行 */
来源：http://vl.newstarts.cn

[A15] 空值判断与默认值
来源：http://vp.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ib.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://op.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://nz.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://iq.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zd.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://jw.521024.cn

Ruby: value = data || "默认值"
来源：http://aq.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ty.asd995.cn

[A16] 真假值判断规则
来源：http://gd.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xy.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fo.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://af.chemitech.net.cn

TS:   if (!x) {}
来源：http://td.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bb.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ns.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ov.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nh.9csxet.cn

[A17] 位运算
来源：http://zu.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jc.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tm.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rq.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gq.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://qx.521024.cn

Py:   ord("A"); chr(65)
来源：http://fl.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://wk.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sg.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yy.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://by.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zr.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://sd.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://tb.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://hx.szxytkj.cn

Py:   a, b = b, a
来源：http://xp.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zg.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://xq.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://pu.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://gb.haigaiapp.cn

Go:   a, b = b, a
来源：http://kp.bjjhwx.cn

Ruby: a, b = b, a
来源：http://uq.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://gp.asd995.cn

[A20] 读取标准输入
来源：http://fu.newstarts.cn

Py:   name = input("请输入：")
来源：http://lq.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ih.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ht.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://xx.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://gg.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xl.newstarts.cn

Ruby: gets.chomp
来源：http://wk.szsharing.cn

C#:   Console.ReadLine();
来源：http://aw.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://du.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://mb.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kk.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://ge.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ma.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://yn.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qn.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://ak.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://tr.shtwfgs.cn

[A22] 获取字符串长度
来源：http://lt.chemitech.net.cn

Py:   len(s)
来源：http://zr.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ef.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dc.jianghongdianzi.cn

TS:   s.length
来源：http://sp.hahajie.cn

Java: s.length()
来源：http://mh.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oo.9csxet.cn

Ruby: s.length
来源：http://fp.lnxyls.cn

C#:   s.Length
来源：http://ab.haigaiapp.cn

[A23] 大小写转换
来源：http://hj.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://st.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nk.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://so.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qb.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ih.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://to.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tk.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cn.haigaiapp.cn

[A24] 去除首尾空白
来源：http://eo.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iy.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lk.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rx.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tf.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://oi.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bd.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://io.jctech888.com.cn

[A25] 字符串比较
来源：http://di.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://ek.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tt.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bz.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://td.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nd.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dw.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cy.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://yg.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lb.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hx.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ow.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://un.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bp.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ok.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fp.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pn.yuexingan06.cn

================================================================================
来源：http://sn.colortex.cn

B. 流程控制
来源：http://ls.newstarts.cn

================================================================================
来源：http://rf.hahajie.cn

[B01] 条件判断 if / else
来源：http://jn.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://re.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ob.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zf.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ax.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mm.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pa.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ie.9csxet.cn

[B02] 多分支 else if / elif
来源：http://ys.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fv.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tz.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ci.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lt.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tw.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.colortex.cn

[B03] switch / match / case
来源：http://fo.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lr.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bu.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ft.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kx.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pt.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ug.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oh.jctech888.com.cn

[B04] for 计数循环
来源：http://xs.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ll.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sp.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://si.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://en.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uj.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gp.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://nk.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mu.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://qe.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://dl.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ip.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://so.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gf.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://di.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zp.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://gc.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rw.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://va.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://af.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wu.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jl.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sf.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://az.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yk.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yy.9csxet.cn

[B07] while 循环
来源：http://jf.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://wg.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rp.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://oz.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://gu.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://iz.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gr.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://eu.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ac.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://hs.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ca.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ys.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://lc.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://nf.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://mb.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://no.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cy.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://gr.szxytkj.cn

[B09] break 与 continue
来源：http://yq.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wk.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hl.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kh.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pv.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oa.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://ol.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qa.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rr.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yj.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gm.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kw.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ae.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dd.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kh.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://nr.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://xw.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://jc.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xd.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hj.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cc.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ho.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://fe.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xp.hnjuh.cn

[B12] 跳出多层循环
来源：http://rl.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nt.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vt.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pw.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zb.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vh.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tf.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uz.haigaiapp.cn

[B13] 判断是否为数字
来源：http://pe.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://jk.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ex.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xa.colortex.cn


<!-- 参考信息 -->