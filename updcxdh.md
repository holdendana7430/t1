代发 wailian999

[A06] 字符串转数字
来源：http://tz.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://jk.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ba.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ir.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xp.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wl.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://os.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zu.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gp.colortex.cn

[A07] 数字转字符串
来源：http://ns.bookmarksfly.cn

Py:   str(42)
来源：http://oh.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://tg.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://fr.haigaiapp.cn

TS:   String(42)
来源：http://op.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sw.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://ut.asd995.cn

Ruby: 42.to_s
来源：http://sd.yuexingan06.cn

C#:   42.ToString()
来源：http://ox.shxzukj.cn

[A08] 取整与四舍五入
来源：http://uj.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jf.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ue.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ls.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://em.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sj.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ya.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jp.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yy.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://ls.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lj.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aa.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ip.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fm.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fu.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xf.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://il.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xo.521024.cn

[A10] 生成随机数
来源：http://zo.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://nd.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://sc.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://il.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dr.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://us.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hs.muxihuayi.cn

Ruby: rand(1..100)
来源：http://wq.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://it.szsharing.cn

[A11] 条件表达式（三元）
来源：http://lp.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://xd.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pb.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vs.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ti.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://ev.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rg.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jz.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ts.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://lm.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dr.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yo.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://eg.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://lo.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://rm.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mf.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://fa.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://zo.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wo.asd995.cn

Py:   "第一行\n第二行"
来源：http://hf.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://ll.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://ov.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://bx.nicolike.cn

Java: "第一行\n第二行"
来源：http://ft.szsharing.cn

Go:   "第一行\n第二行"
来源：http://ws.colortex.cn

Ruby: "第一行\n第二行"
来源：http://vp.521024.cn

C#:   "第一行\n第二行"
来源：http://go.shtwfgs.cn

[A14] 注释写法
来源：http://ey.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eo.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ff.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://vg.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://qx.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vo.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://sw.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iz.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://wx.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://me.hnjuh.cn

Py:   value = data or "默认值"
来源：http://dr.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://mn.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://zv.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://ww.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pq.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://hz.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://qo.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://eb.jctech888.com.cn

[A16] 真假值判断规则
来源：http://oy.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pi.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vi.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hd.bjjhwx.cn

TS:   if (!x) {}
来源：http://mi.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mm.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zq.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://af.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qt.wgjwhj.cn

[A17] 位运算
来源：http://nt.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pi.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yz.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aq.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mw.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sy.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yx.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://al.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jn.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://se.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://uv.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://fu.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pg.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xp.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://ub.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hu.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://at.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://mr.521024.cn

[A19] 交换两个变量
来源：http://hi.huanxung.cn

Py:   a, b = b, a
来源：http://pc.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ki.521024.cn

JS:   [a, b] = [b, a];
来源：http://gg.521024.cn

TS:   [a, b] = [b, a];
来源：http://fm.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://xn.bookmarksfly.cn

Go:   a, b = b, a
来源：http://vz.panjiajie.cn

Ruby: a, b = b, a
来源：http://lp.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://dc.nszjky.cn

[A20] 读取标准输入
来源：http://dt.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://hf.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mk.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vo.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://jh.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://ht.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wu.asd995.cn

Ruby: gets.chomp
来源：http://ef.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://pd.nszjky.cn

[A21] 保留指定小数位输出
来源：http://hr.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://gn.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mv.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://mb.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://rn.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://bn.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tp.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://bm.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://ca.szxytkj.cn

[A22] 获取字符串长度
来源：http://sl.bjjhwx.cn

Py:   len(s)
来源：http://yx.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ub.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tj.muxihuayi.cn

TS:   s.length
来源：http://at.chemitech.net.cn

Java: s.length()
来源：http://ns.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ef.521024.cn

Ruby: s.length
来源：http://ll.nszjky.cn

C#:   s.Length
来源：http://jq.lnxyls.cn

[A23] 大小写转换
来源：http://vd.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gh.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ns.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wt.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jl.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lg.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fg.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mp.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vs.nicolike.cn

[A24] 去除首尾空白
来源：http://sh.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ux.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tr.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oa.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://da.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://uw.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ig.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://px.haigaiapp.cn

[A25] 字符串比较
来源：http://ch.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://im.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yl.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fe.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rc.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://va.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cg.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ah.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jk.muxihuayi.cn

[A26] 类型转换总览
来源：http://gy.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wq.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://as.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vk.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://yc.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mg.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bf.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vx.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nj.yuexingan06.cn

================================================================================
来源：http://iz.haigaiapp.cn

B. 流程控制
来源：http://gl.huanxung.cn

================================================================================
来源：http://fo.lnxyls.cn

[B01] 条件判断 if / else
来源：http://fe.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rt.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ve.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wj.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nr.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dd.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mh.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://em.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ll.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ic.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pr.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ex.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ln.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xm.lnxyls.cn

[B03] switch / match / case
来源：http://jz.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cp.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ve.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kp.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ky.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xn.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ye.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pg.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cl.gzmigu.cn

[B04] for 计数循环
来源：http://wv.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://kn.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aq.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ci.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wr.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iu.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://we.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://df.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cy.521024.cn

[B05] 遍历数组 / 列表
来源：http://hx.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://cx.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xz.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vx.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://og.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://su.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gx.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://si.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ra.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://qn.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gl.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kk.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oe.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pw.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xk.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fl.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cy.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kl.asd995.cn

[B07] while 循环
来源：http://xe.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://jj.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yt.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ah.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://wu.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://xi.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hu.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://af.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://sn.colortex.cn

[B08] do-while（至少执行一次）
来源：http://bc.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zt.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ox.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://fr.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://zd.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://iu.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://su.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gk.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://js.jianghongdianzi.cn

[B09] break 与 continue
来源：http://dt.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tt.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rh.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bb.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xo.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ba.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vp.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ix.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qy.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tg.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eq.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lw.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wc.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sy.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://mc.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://kw.521024.cn

PHP:  range(0, 10, 2);
来源：http://ok.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ip.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yy.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pm.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aa.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://kl.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vb.huanxung.cn

[B12] 跳出多层循环
来源：http://be.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hk.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ca.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ib.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gd.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rf.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bj.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bl.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hm.newstarts.cn


<!-- 参考信息 -->