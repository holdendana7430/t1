代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rg.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gx.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oq.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lc.521024.cn

Java: 7 / 2; 7 % 2
来源：http://ch.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://kf.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://hb.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://la.huixiangedu.cn

[A06] 字符串转数字
来源：http://gr.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ud.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tm.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ot.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nd.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cl.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jl.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wo.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://td.szxytkj.cn

[A07] 数字转字符串
来源：http://wk.521024.cn

Py:   str(42)
来源：http://rw.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://iy.521024.cn

JS:   String(42); (42).toString()
来源：http://er.shtwfgs.cn

TS:   String(42)
来源：http://uf.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tb.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://aj.lnxyls.cn

Ruby: 42.to_s
来源：http://hx.newstarts.cn

C#:   42.ToString()
来源：http://fa.hnjuh.cn

[A08] 取整与四舍五入
来源：http://vj.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eu.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wn.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nm.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eo.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ju.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zw.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wf.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rr.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://en.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ya.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dn.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bj.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nd.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fo.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fr.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pe.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qg.jctech888.com.cn

[A10] 生成随机数
来源：http://fd.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://cl.newstarts.cn

PHP:  random_int(1, 100);
来源：http://ku.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uh.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ou.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ee.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ck.haigaiapp.cn

Ruby: rand(1..100)
来源：http://lv.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://he.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://lq.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://mi.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bv.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ty.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zq.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://my.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mj.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xx.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xp.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://cj.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ik.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cu.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://wf.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://lw.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://sz.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mm.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://xy.521024.cn

C#:   $"Hello, {name}!"
来源：http://do.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fl.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://sw.asd995.cn

PHP:  "第一行\n第二行"
来源：http://qq.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://du.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://bw.newstarts.cn

Java: "第一行\n第二行"
来源：http://lt.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://ps.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://lm.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://jm.hnjuh.cn

[A14] 注释写法
来源：http://uw.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mg.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jo.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://lw.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://nx.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hj.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://gt.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mc.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://nr.lnxyls.cn

[A15] 空值判断与默认值
来源：http://uu.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ra.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://xp.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ho.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://ue.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xc.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://he.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://fm.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://rb.yuexingan06.cn

[A16] 真假值判断规则
来源：http://hf.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ke.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fi.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ip.szxytkj.cn

TS:   if (!x) {}
来源：http://ht.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://js.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aq.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uh.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://un.bjjhwx.cn

[A17] 位运算
来源：http://gb.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ir.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lx.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ik.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fg.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wu.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vb.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cc.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://fd.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://oa.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://gp.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ft.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://io.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://eu.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tt.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://za.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://go.hnjuh.cn

[A19] 交换两个变量
来源：http://ie.bjjhwx.cn

Py:   a, b = b, a
来源：http://wn.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kd.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://nf.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://uo.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://hm.jctech888.com.cn

Go:   a, b = b, a
来源：http://jk.gzmigu.cn

Ruby: a, b = b, a
来源：http://er.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://eh.bjjhwx.cn

[A20] 读取标准输入
来源：http://en.nszjky.cn

Py:   name = input("请输入：")
来源：http://pq.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oo.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://xj.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://ww.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lu.szsharing.cn

Ruby: gets.chomp
来源：http://yx.newstarts.cn

C#:   Console.ReadLine();
来源：http://vr.huanxung.cn

[A21] 保留指定小数位输出
来源：http://fn.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://qp.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kq.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://um.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://fm.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://ed.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wq.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ih.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://tw.huixiangedu.cn

[A22] 获取字符串长度
来源：http://tc.newstarts.cn

Py:   len(s)
来源：http://fk.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tb.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yb.haigaiapp.cn

TS:   s.length
来源：http://ig.bookmarksfly.cn

Java: s.length()
来源：http://me.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://da.bookmarksfly.cn

Ruby: s.length
来源：http://aw.nicolike.cn

C#:   s.Length
来源：http://ew.haigaiapp.cn

[A23] 大小写转换
来源：http://yx.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fx.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mf.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ew.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://px.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ht.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ke.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wq.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hr.9csxet.cn

[A24] 去除首尾空白
来源：http://mv.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://li.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pj.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vr.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eh.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gf.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://ug.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cy.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qn.hahajie.cn

[A25] 字符串比较
来源：http://yy.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://rm.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lo.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://px.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ji.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xq.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tp.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ob.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sy.yuexingan06.cn

[A26] 类型转换总览
来源：http://hi.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qz.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wa.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mx.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://bk.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hc.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fr.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rn.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uz.hahajie.cn

================================================================================
来源：http://ct.haigaiapp.cn

B. 流程控制
来源：http://rd.yuexingan06.cn

================================================================================
来源：http://wj.nszjky.cn

[B01] 条件判断 if / else
来源：http://mi.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wb.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://li.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xn.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yw.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fa.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uq.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pd.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fh.colortex.cn

[B02] 多分支 else if / elif
来源：http://rr.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vw.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yf.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ku.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://en.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ti.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.bjjhwx.cn

[B03] switch / match / case
来源：http://ai.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ya.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tr.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gn.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vs.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ia.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ke.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://em.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gj.huixinmuqiang.cn

[B04] for 计数循环
来源：http://nn.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://rn.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mz.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ng.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yv.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mp.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://dp.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://am.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://gf.szsharing.cn

Py:   for item in arr: print(item)
来源：http://jy.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mb.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cx.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vb.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bg.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://si.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://uv.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://er.521024.cn

[B06] 遍历字典 / 对象
来源：http://zo.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fm.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tz.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gl.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qe.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rt.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vj.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hf.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://al.colortex.cn

[B07] while 循环
来源：http://xt.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://yi.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vp.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://vj.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://oa.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ql.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mk.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://rl.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ox.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://xk.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://xo.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://md.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://kn.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://li.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://dh.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xv.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zi.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://zc.huixiangedu.cn

[B09] break 与 continue
来源：http://qr.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dj.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ug.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kq.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://as.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qr.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ig.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ds.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://md.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xm.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://up.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fo.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cc.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sd.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://px.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fp.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ug.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://pe.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://nv.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ox.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yz.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sk.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://su.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://eg.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ri.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ad.gzmigu.cn


<!-- 参考信息 -->