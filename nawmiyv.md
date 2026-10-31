代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ka.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rz.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fv.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mg.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tn.nicolike.cn

[A07] 数字转字符串
来源：http://sa.shxzskj.cn

Py:   str(42)
来源：http://ek.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://ab.521024.cn

JS:   String(42); (42).toString()
来源：http://bb.yuexingan06.cn

TS:   String(42)
来源：http://qj.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cu.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://at.huanxung.cn

Ruby: 42.to_s
来源：http://tc.yuexingan06.cn

C#:   42.ToString()
来源：http://pp.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://ta.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ni.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iy.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vw.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ju.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ta.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ch.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fz.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lv.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://lp.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mw.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gr.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nb.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://io.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aj.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gm.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ec.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cb.muxihuayi.cn

[A10] 生成随机数
来源：http://zw.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ky.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://xe.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cb.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mm.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://gq.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sy.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://lp.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://bq.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://ic.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://gz.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://il.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bp.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bu.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://js.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mf.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oc.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jo.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://ef.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tj.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cy.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://dm.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://aq.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://yk.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rv.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://nk.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://gn.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sh.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://lk.521024.cn

PHP:  "第一行\n第二行"
来源：http://gj.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://do.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://vt.nszjky.cn

Java: "第一行\n第二行"
来源：http://nn.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://vo.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://or.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ud.szxytkj.cn

[A14] 注释写法
来源：http://eh.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ak.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pn.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://bb.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://pr.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bu.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://au.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qu.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://wp.gzmigu.cn

[A15] 空值判断与默认值
来源：http://on.colortex.cn

Py:   value = data or "默认值"
来源：http://ci.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://rk.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://at.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://gi.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nl.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://vl.colortex.cn

Ruby: value = data || "默认值"
来源：http://dj.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://bd.shxzukj.cn

[A16] 真假值判断规则
来源：http://lh.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jb.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qu.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xb.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://vt.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dj.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://co.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wi.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pe.colortex.cn

[A17] 位运算
来源：http://pi.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gx.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yf.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://br.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qo.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://br.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://br.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ff.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://bi.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nl.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://cp.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mw.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://ei.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://kq.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://il.jctech888.com.cn

Py:   a, b = b, a
来源：http://bl.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qy.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://vl.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://is.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://re.9csxet.cn

Go:   a, b = b, a
来源：http://nm.wgjwhj.cn

Ruby: a, b = b, a
来源：http://ia.colortex.cn

C#:   (a, b) = (b, a);
来源：http://ly.huixiangedu.cn

[A20] 读取标准输入
来源：http://me.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://rd.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ci.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ih.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://ti.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://lk.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sp.shxzukj.cn

Ruby: gets.chomp
来源：http://ap.shxzskj.cn

C#:   Console.ReadLine();
来源：http://qf.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://st.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://jd.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hv.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://kt.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://uy.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://ms.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vz.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://gk.521024.cn

C#:   3.14159.ToString("F2")
来源：http://us.newstarts.cn

[A22] 获取字符串长度
来源：http://wh.haigaiapp.cn

Py:   len(s)
来源：http://ip.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yk.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://um.nicolike.cn

TS:   s.length
来源：http://ua.bookmarksfly.cn

Java: s.length()
来源：http://ka.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sz.yuexingan06.cn

Ruby: s.length
来源：http://vv.muxihuayi.cn

C#:   s.Length
来源：http://by.nszjky.cn

[A23] 大小写转换
来源：http://wu.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mr.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yd.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mh.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://on.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qm.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bc.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yp.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qq.asd995.cn

[A24] 去除首尾空白
来源：http://wx.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ze.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fw.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zb.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://et.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://al.521024.cn

Go:   strings.TrimSpace(s)
来源：http://kx.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ae.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ks.jianghongdianzi.cn

[A25] 字符串比较
来源：http://jv.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://oe.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bg.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uk.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nt.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xv.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fu.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cz.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yc.hnjuh.cn

[A26] 类型转换总览
来源：http://vt.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ds.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pp.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uq.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://bc.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wt.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hx.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yd.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rx.wgjwhj.cn

================================================================================
来源：http://fs.shxzskj.cn

B. 流程控制
来源：http://gn.9csxet.cn

================================================================================
来源：http://km.shxzukj.cn

[B01] 条件判断 if / else
来源：http://iq.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nb.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wy.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://px.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ap.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pr.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nh.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bp.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ai.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://zu.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lh.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vd.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ww.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://su.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ks.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xm.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.szsharing.cn

[B03] switch / match / case
来源：http://ta.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bo.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xn.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://be.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ks.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ln.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ll.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gr.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://an.huixiangedu.cn

[B04] for 计数循环
来源：http://yh.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://kn.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lc.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ft.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jc.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sx.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fv.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://jn.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uk.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ob.521024.cn

Py:   for item in arr: print(item)
来源：http://tg.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gp.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xx.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://do.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vz.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hd.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://kk.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xx.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://pw.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xs.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fd.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tk.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pz.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ig.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aa.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qa.asd995.cn

[B07] while 循环
来源：http://tb.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://hk.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zo.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://jl.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://bl.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://qs.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rd.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://qj.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://ap.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://xv.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://ah.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pc.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://wm.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://fo.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://op.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fr.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qi.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ua.hnjuh.cn

[B09] break 与 continue
来源：http://ti.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pe.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://to.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://um.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fj.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vs.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gg.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ec.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://pa.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vc.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bw.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ux.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xm.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xc.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cc.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vb.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ea.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://it.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://qo.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://bp.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zg.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ca.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vs.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tc.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://vp.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nr.muxihuayi.cn

[B12] 跳出多层循环
来源：http://uy.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pi.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tc.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fi.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vr.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ve.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://by.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ay.huanxung.cn

[B13] 判断是否为数字
来源：http://zs.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ap.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://av.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kf.muxihuayi.cn


<!-- 参考信息 -->