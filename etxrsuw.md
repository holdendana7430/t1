代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hm.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rj.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://cw.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vv.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cn.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ak.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://mq.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://qn.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jk.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://en.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cb.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pk.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://ah.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://au.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://ir.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://rl.nszjky.cn

[A06] 字符串转数字
来源：http://bi.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://qp.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ci.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wu.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vx.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rx.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uw.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hh.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mq.gzmigu.cn

[A07] 数字转字符串
来源：http://vn.huixinmuqiang.cn

Py:   str(42)
来源：http://iy.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://dp.521024.cn

JS:   String(42); (42).toString()
来源：http://oi.muxihuayi.cn

TS:   String(42)
来源：http://eg.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mk.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://kd.panjiajie.cn

Ruby: 42.to_s
来源：http://bm.nszjky.cn

C#:   42.ToString()
来源：http://xk.hnjuh.cn

[A08] 取整与四舍五入
来源：http://sn.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ia.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zm.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mm.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xf.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fm.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mi.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nf.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xd.asd995.cn

[A09] 绝对值与最大最小值
来源：http://xg.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fw.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yy.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oz.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xn.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yn.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cs.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yt.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fs.szxytkj.cn

[A10] 生成随机数
来源：http://jy.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://an.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://ps.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eq.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yx.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://oy.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gb.asd995.cn

Ruby: rand(1..100)
来源：http://ri.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://nq.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://dt.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://qj.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bn.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xh.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jl.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://qa.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xk.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xc.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dv.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://rn.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://as.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nu.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://jd.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://gc.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://wy.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aa.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://az.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://uj.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bx.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://ov.asd995.cn

PHP:  "第一行\n第二行"
来源：http://bv.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://kx.asd995.cn

TS:   "第一行\n第二行"
来源：http://jc.9csxet.cn

Java: "第一行\n第二行"
来源：http://ap.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://nf.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://gy.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://ff.nszjky.cn

[A14] 注释写法
来源：http://hf.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ve.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ij.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://zd.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://de.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ht.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://jh.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sq.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://bc.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://ev.asd995.cn

Py:   value = data or "默认值"
来源：http://yb.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://od.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://hl.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://vg.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://du.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://ol.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://pi.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://bh.szxytkj.cn

[A16] 真假值判断规则
来源：http://pc.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qo.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qy.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ly.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://gy.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ra.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gz.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sf.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ie.colortex.cn

[A17] 位运算
来源：http://yp.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mj.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ie.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bc.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oj.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bx.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jq.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gx.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jp.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://oq.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://tm.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://lj.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ri.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vu.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://ek.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gr.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://ar.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://bc.huixiangedu.cn

[A19] 交换两个变量
来源：http://ic.bjjhwx.cn

Py:   a, b = b, a
来源：http://bd.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lr.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://sh.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://sz.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://wa.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://rg.colortex.cn

Ruby: a, b = b, a
来源：http://em.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://qu.panjiajie.cn

[A20] 读取标准输入
来源：http://nq.nszjky.cn

Py:   name = input("请输入：")
来源：http://sm.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sx.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rd.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://dy.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ef.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xf.jctech888.com.cn

Ruby: gets.chomp
来源：http://ml.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://hc.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://cm.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://ce.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bo.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://mr.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://kl.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://sn.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bs.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://rp.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://cv.colortex.cn

[A22] 获取字符串长度
来源：http://lj.9csxet.cn

Py:   len(s)
来源：http://tl.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tz.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ai.hnjuh.cn

TS:   s.length
来源：http://oc.asd995.cn

Java: s.length()
来源：http://ei.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://df.yuexingan06.cn

Ruby: s.length
来源：http://oq.wgjwhj.cn

C#:   s.Length
来源：http://qs.nicolike.cn

[A23] 大小写转换
来源：http://ir.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tc.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sp.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xe.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://px.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ho.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tn.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dx.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cs.hahajie.cn

[A24] 去除首尾空白
来源：http://ty.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zu.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://np.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cm.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sm.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bn.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://mb.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://th.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wm.shxzskj.cn

[A25] 字符串比较
来源：http://ef.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://zy.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pu.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iv.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bd.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sx.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pp.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dy.nicolike.cn

[A26] 类型转换总览
来源：http://ab.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ei.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oa.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zz.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://tq.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ru.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ak.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rg.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sg.muxihuayi.cn

================================================================================
来源：http://bk.521024.cn

B. 流程控制
来源：http://co.huixinmuqiang.cn

================================================================================
来源：http://yc.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://hn.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ur.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qe.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hy.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ag.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qg.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zd.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sr.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gi.colortex.cn

[B02] 多分支 else if / elif
来源：http://bl.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://by.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ox.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ai.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eo.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vt.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.szsharing.cn

[B03] switch / match / case
来源：http://ar.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ux.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://se.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://py.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rb.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tp.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nn.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yz.asd995.cn

[B04] for 计数循环
来源：http://ha.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://ca.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wq.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ze.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mc.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hf.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zx.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://yj.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dk.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://uy.521024.cn

Py:   for item in arr: print(item)
来源：http://ob.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://td.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yq.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sq.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lc.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hi.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://vv.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vr.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ub.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ht.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ss.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vl.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uy.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://su.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lv.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pq.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cc.yuexingan06.cn

[B07] while 循环
来源：http://bj.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://kx.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hd.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://rl.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://jo.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://bu.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kk.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://lk.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://eb.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://pv.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://eu.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kb.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://gy.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://gj.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://zv.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://it.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://on.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://tz.jianghongdianzi.cn

[B09] break 与 continue
来源：http://fh.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qr.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ew.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ai.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dn.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.szsharing.cn

[B10] 遍历同时拿索引
来源：http://vn.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lh.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pz.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yz.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ib.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ww.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aw.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tg.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ay.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://kf.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ld.bjjhwx.cn


<!-- 参考信息 -->