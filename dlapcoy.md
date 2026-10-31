代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://ep.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xs.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://kc.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://zb.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jf.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qy.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pp.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iv.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://mj.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://py.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ow.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://xe.muxihuayi.cn

[A06] 字符串转数字
来源：http://sv.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://nm.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vw.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xw.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cp.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ee.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xr.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lr.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tf.huanxung.cn

[A07] 数字转字符串
来源：http://rg.haigaiapp.cn

Py:   str(42)
来源：http://hq.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://pn.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://cx.panjiajie.cn

TS:   String(42)
来源：http://ei.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kf.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://sq.shxzskj.cn

Ruby: 42.to_s
来源：http://zi.szsharing.cn

C#:   42.ToString()
来源：http://qj.521024.cn

[A08] 取整与四舍五入
来源：http://if.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://md.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qe.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tw.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gp.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uc.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bn.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://il.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lv.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://ap.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ks.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ju.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kb.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ku.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tw.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yp.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qr.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nh.lnxyls.cn

[A10] 生成随机数
来源：http://mc.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://dz.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://lu.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ms.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zq.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://ok.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rg.jctech888.com.cn

Ruby: rand(1..100)
来源：http://aa.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://yc.9csxet.cn

[A11] 条件表达式（三元）
来源：http://ay.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://fr.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lf.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hx.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oe.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://ab.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://np.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ur.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tf.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://xg.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rk.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xo.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://zg.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://za.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://dn.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ty.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://rn.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://wh.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pe.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://oe.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://vp.9csxet.cn

JS:   "第一行\n第二行"
来源：http://ft.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://ds.nszjky.cn

Java: "第一行\n第二行"
来源：http://os.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://th.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://yr.asd995.cn

C#:   "第一行\n第二行"
来源：http://im.muxihuayi.cn

[A14] 注释写法
来源：http://pl.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vc.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://si.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://km.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://gp.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ia.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://fk.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yf.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://pz.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://ur.shxzskj.cn

Py:   value = data or "默认值"
来源：http://mp.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://xd.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ef.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://nv.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cs.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://cv.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://gl.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://qv.chemitech.net.cn

[A16] 真假值判断规则
来源：http://pn.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bs.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dk.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://my.lnxyls.cn

TS:   if (!x) {}
来源：http://lx.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lm.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cl.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ms.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://as.szxytkj.cn

[A17] 位运算
来源：http://mp.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ja.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gz.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wr.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ge.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rs.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://di.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://xv.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://vl.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://jl.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://is.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://el.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hj.521024.cn

Ruby: "A".ord; 65.chr
来源：http://my.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://ph.9csxet.cn

[A19] 交换两个变量
来源：http://ss.huanxung.cn

Py:   a, b = b, a
来源：http://hs.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rp.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://ql.colortex.cn

TS:   [a, b] = [b, a];
来源：http://uz.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://pc.jctech888.com.cn

Go:   a, b = b, a
来源：http://hu.shxzukj.cn

Ruby: a, b = b, a
来源：http://ua.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://cg.huanxung.cn

[A20] 读取标准输入
来源：http://qc.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://hk.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gw.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gs.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://xx.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://ac.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xz.shxzskj.cn

Ruby: gets.chomp
来源：http://md.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://hq.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://rh.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://ld.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cj.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://xv.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://xh.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://xz.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xo.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://pp.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://uu.bjjhwx.cn

[A22] 获取字符串长度
来源：http://oe.yuexingan06.cn

Py:   len(s)
来源：http://hg.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tw.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uc.yuexingan06.cn

TS:   s.length
来源：http://uv.jctech888.com.cn

Java: s.length()
来源：http://ki.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jm.jctech888.com.cn

Ruby: s.length
来源：http://mv.bookmarksfly.cn

C#:   s.Length
来源：http://tp.szxytkj.cn

[A23] 大小写转换
来源：http://ve.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sn.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ev.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vu.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kp.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jj.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://re.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rx.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ew.wgjwhj.cn

[A24] 去除首尾空白
来源：http://xb.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://co.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gw.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ys.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cm.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://hv.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yp.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pg.jctech888.com.cn

[A25] 字符串比较
来源：http://ec.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://co.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cv.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kh.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nv.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bg.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kr.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fu.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pm.shxzskj.cn

[A26] 类型转换总览
来源：http://yz.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jf.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://za.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rs.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ul.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fo.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zq.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iq.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ro.wgjwhj.cn

================================================================================
来源：http://wt.szxytkj.cn

B. 流程控制
来源：http://hw.nicolike.cn

================================================================================
来源：http://zr.szsharing.cn

[B01] 条件判断 if / else
来源：http://rs.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fu.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ob.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ve.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://py.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hw.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://df.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gf.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sq.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://zo.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://so.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fd.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lf.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gq.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.bookmarksfly.cn

[B03] switch / match / case
来源：http://jf.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wy.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lv.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ro.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ji.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kw.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ho.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vt.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zn.yuntaijiaju.cn

[B04] for 计数循环
来源：http://wd.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ks.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bb.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hv.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yu.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gq.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://na.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://fz.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yq.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://si.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://il.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cy.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nc.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xp.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zc.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pz.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://je.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ax.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://ws.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vv.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cz.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dl.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yx.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hd.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ux.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ra.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ny.huixinmuqiang.cn

[B07] while 循环
来源：http://zc.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://ao.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nt.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://rm.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://vu.asd995.cn

Java: while (i < 10) { i++; }
来源：http://nm.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qx.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://by.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://nh.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://dg.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://pk.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ba.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://pp.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://dq.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ir.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pd.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ep.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://jj.huanxung.cn

[B09] break 与 continue
来源：http://ip.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ct.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://le.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qt.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://je.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yx.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mp.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dt.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.colortex.cn

[B10] 遍历同时拿索引
来源：http://pv.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ik.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oq.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gd.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iq.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ll.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://if.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://is.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zf.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://qr.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://nu.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://fq.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rv.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ly.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dy.huanxung.cn


<!-- 参考信息 -->