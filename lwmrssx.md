代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://fz.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ej.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://db.shxzukj.cn

[A05] 整数除法与取模
来源：http://pl.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mf.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hl.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ry.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hx.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://ux.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://kl.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ql.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ip.bjjhwx.cn

[A06] 字符串转数字
来源：http://jn.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://uk.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ha.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yk.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lu.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qj.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wp.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hg.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gt.hahajie.cn

[A07] 数字转字符串
来源：http://gz.lnxyls.cn

Py:   str(42)
来源：http://uz.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://yb.nszjky.cn

JS:   String(42); (42).toString()
来源：http://ox.huixinmuqiang.cn

TS:   String(42)
来源：http://ta.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fs.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://oz.shxzukj.cn

Ruby: 42.to_s
来源：http://qi.muxihuayi.cn

C#:   42.ToString()
来源：http://uv.szxytkj.cn

[A08] 取整与四舍五入
来源：http://rt.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hu.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ne.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iq.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ep.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yq.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wd.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://um.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cg.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://hp.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://na.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ns.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lz.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pm.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://js.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kz.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ok.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lx.jianghongdianzi.cn

[A10] 生成随机数
来源：http://no.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://jr.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://sd.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dk.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xj.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://no.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oc.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://bt.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://mz.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://pg.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://la.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://si.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ts.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dh.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://db.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ll.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sw.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sj.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://zr.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vk.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://di.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://hj.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://ji.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xa.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jr.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ip.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://gt.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://so.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://uk.asd995.cn

PHP:  "第一行\n第二行"
来源：http://az.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://sy.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://xm.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://lv.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://jr.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://ry.huanxung.cn

C#:   "第一行\n第二行"
来源：http://bn.shxzukj.cn

[A14] 注释写法
来源：http://ti.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jv.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wf.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://kf.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://to.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nx.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://zb.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vz.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://eq.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://rb.hnjuh.cn

Py:   value = data or "默认值"
来源：http://lp.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://ro.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://qk.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ow.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dt.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://fj.colortex.cn

Ruby: value = data || "默认值"
来源：http://lu.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://gc.szsharing.cn

[A16] 真假值判断规则
来源：http://gf.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://he.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fy.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wc.muxihuayi.cn

TS:   if (!x) {}
来源：http://zz.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rm.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gw.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sk.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yy.szsharing.cn

[A17] 位运算
来源：http://vd.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qt.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nc.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://py.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nv.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hw.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cz.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yw.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://fs.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://cu.521024.cn

PHP:  ord("A"); chr(65)
来源：http://wx.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ga.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://em.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://ah.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qw.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://jb.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://zs.bjjhwx.cn

[A19] 交换两个变量
来源：http://zg.szsharing.cn

Py:   a, b = b, a
来源：http://oo.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lu.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://fh.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://rl.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://ex.hnjuh.cn

Go:   a, b = b, a
来源：http://cc.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://if.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://uk.chemitech.net.cn

[A20] 读取标准输入
来源：http://dg.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://iy.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nf.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uy.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://lw.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://qe.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bu.bjjhwx.cn

Ruby: gets.chomp
来源：http://ch.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://hi.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://je.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://qb.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nt.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://fy.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://kb.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://vk.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yh.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://fu.521024.cn

C#:   3.14159.ToString("F2")
来源：http://vl.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ko.szsharing.cn

Py:   len(s)
来源：http://kj.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qd.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lt.hnjuh.cn

TS:   s.length
来源：http://bk.gzmigu.cn

Java: s.length()
来源：http://dh.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ya.gzmigu.cn

Ruby: s.length
来源：http://cg.newstarts.cn

C#:   s.Length
来源：http://rd.9csxet.cn

[A23] 大小写转换
来源：http://mr.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vn.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rk.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cw.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fb.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rc.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bt.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dg.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xy.szsharing.cn

[A24] 去除首尾空白
来源：http://az.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wv.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://am.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jm.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://do.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kl.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://za.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tr.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://um.huanxung.cn

[A25] 字符串比较
来源：http://mv.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://kq.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sa.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vi.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ki.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ck.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yd.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ee.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ch.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://sy.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ka.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lh.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ty.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://bh.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cd.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kn.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wt.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pv.hahajie.cn

================================================================================
来源：http://mu.nicolike.cn

B. 流程控制
来源：http://ob.9csxet.cn

================================================================================
来源：http://qq.hahajie.cn

[B01] 条件判断 if / else
来源：http://sz.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zr.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bc.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kh.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ii.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yk.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sc.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nr.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jy.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://gf.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lo.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eb.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kp.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vo.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bs.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hf.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://po.yuntaijiaju.cn

[B03] switch / match / case
来源：http://km.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oy.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xu.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pc.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://to.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ek.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wl.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zq.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qq.lnxyls.cn

[B04] for 计数循环
来源：http://dz.colortex.cn

Py:   for i in range(10): print(i)
来源：http://xy.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lt.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tp.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zx.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yu.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://wl.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ie.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://mw.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://hc.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ks.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sa.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mj.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ef.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vy.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://pe.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ye.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://lo.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lt.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ym.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kw.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lm.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bz.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://az.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sb.chemitech.net.cn

[B07] while 循环
来源：http://lu.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://jm.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://io.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://mn.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://lr.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://fg.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bi.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://kc.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://zx.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://pz.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://nn.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xr.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://kl.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://bs.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://bx.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pr.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xm.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ui.bjjhwx.cn

[B09] break 与 continue
来源：http://vs.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bi.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://js.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cd.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://un.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.szsharing.cn

[B10] 遍历同时拿索引
来源：http://mc.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ak.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wu.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dh.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fz.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dt.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ic.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eo.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hq.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://qf.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://sj.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://og.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sx.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dw.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://js.jctech888.com.cn


<!-- 参考信息 -->