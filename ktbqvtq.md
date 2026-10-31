代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sf.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qh.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pk.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ox.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://sg.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://vy.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://df.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://bs.shxzukj.cn

[A06] 字符串转数字
来源：http://va.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://tq.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jk.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dy.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ta.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rp.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mb.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bl.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://te.wgjwhj.cn

[A07] 数字转字符串
来源：http://ib.huanxung.cn

Py:   str(42)
来源：http://pg.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ml.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://gb.haigaiapp.cn

TS:   String(42)
来源：http://sj.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dv.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://wc.shtwfgs.cn

Ruby: 42.to_s
来源：http://dj.9csxet.cn

C#:   42.ToString()
来源：http://ix.panjiajie.cn

[A08] 取整与四舍五入
来源：http://yj.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://by.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sh.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fv.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ml.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gh.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sl.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nb.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ir.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://dy.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nk.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gr.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ij.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dn.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rk.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ng.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qv.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kt.panjiajie.cn

[A10] 生成随机数
来源：http://cp.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://il.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://yr.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xz.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zp.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://yv.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vz.hahajie.cn

Ruby: rand(1..100)
来源：http://jt.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://ua.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://jh.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://zr.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zs.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rm.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xe.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://ru.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://np.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oc.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cn.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://ji.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jd.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jd.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://ar.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://qd.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://qd.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ba.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://kc.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://rv.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bz.szsharing.cn

Py:   "第一行\n第二行"
来源：http://eq.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://ve.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://tq.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://ia.hnjuh.cn

Java: "第一行\n第二行"
来源：http://li.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://us.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://pz.hahajie.cn

C#:   "第一行\n第二行"
来源：http://vk.shtwfgs.cn

[A14] 注释写法
来源：http://hy.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xy.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ac.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://yg.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://gy.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gq.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://tb.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mr.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://gt.hnjuh.cn

[A15] 空值判断与默认值
来源：http://qb.hahajie.cn

Py:   value = data or "默认值"
来源：http://nk.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://gy.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://rb.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://xj.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cf.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://xb.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://je.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://cn.wgjwhj.cn

[A16] 真假值判断规则
来源：http://ok.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cd.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hc.nicolike.cn

TS:   if (!x) {}
来源：http://vf.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kh.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ag.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vv.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://af.nszjky.cn

[A17] 位运算
来源：http://dj.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ew.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jh.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://al.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://co.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kq.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://qx.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://wj.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://sq.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vn.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oo.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ij.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tb.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://zq.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://ja.hahajie.cn

[A19] 交换两个变量
来源：http://fb.hahajie.cn

Py:   a, b = b, a
来源：http://tn.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rp.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://mi.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ex.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://eu.huanxung.cn

Go:   a, b = b, a
来源：http://ye.shxzukj.cn

Ruby: a, b = b, a
来源：http://ll.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://hf.bookmarksfly.cn

[A20] 读取标准输入
来源：http://ym.nszjky.cn

Py:   name = input("请输入：")
来源：http://vw.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://he.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://or.colortex.cn

TS:   // Node.js：readline 模块
来源：http://dr.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://uu.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gm.haigaiapp.cn

Ruby: gets.chomp
来源：http://tw.gzmigu.cn

C#:   Console.ReadLine();
来源：http://dd.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://xi.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://zk.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fx.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://su.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://tw.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ia.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pr.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://wy.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://pw.newstarts.cn

[A22] 获取字符串长度
来源：http://zp.haigaiapp.cn

Py:   len(s)
来源：http://sf.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ne.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hj.chemitech.net.cn

TS:   s.length
来源：http://tf.shtwfgs.cn

Java: s.length()
来源：http://dk.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pa.jianghongdianzi.cn

Ruby: s.length
来源：http://rb.gzmigu.cn

C#:   s.Length
来源：http://vw.shxzskj.cn

[A23] 大小写转换
来源：http://eo.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fw.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vk.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nt.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ep.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ms.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lm.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://se.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gp.9csxet.cn

[A24] 去除首尾空白
来源：http://ho.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://da.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fn.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mm.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ek.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bb.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://fd.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zy.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hq.jianghongdianzi.cn

[A25] 字符串比较
来源：http://mh.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ph.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gt.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mn.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://os.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kp.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sp.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pz.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ng.wgjwhj.cn

[A26] 类型转换总览
来源：http://se.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kk.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://py.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ne.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://bm.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mw.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pd.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hj.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tz.chemitech.net.cn

================================================================================
来源：http://oi.521024.cn

B. 流程控制
来源：http://vl.521024.cn

================================================================================
来源：http://uv.newstarts.cn

[B01] 条件判断 if / else
来源：http://lr.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qk.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ae.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vg.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ao.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ho.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ow.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tq.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ob.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://hi.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xo.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tj.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cg.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eq.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xr.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.szxytkj.cn

[B03] switch / match / case
来源：http://ye.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ap.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wy.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://en.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://md.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yl.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gi.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mf.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aw.bjjhwx.cn

[B04] for 计数循环
来源：http://tm.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://we.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cu.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eo.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jz.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://td.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://bx.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ll.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://am.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://bb.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://il.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yu.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yv.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ow.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gx.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://gg.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vn.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://ll.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://no.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mi.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gp.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qf.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bd.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ql.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wy.huixinmuqiang.cn

[B07] while 循环
来源：http://ey.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ae.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ub.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://uk.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://oi.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://we.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vy.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://xj.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://fj.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ak.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://xd.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wv.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://vi.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://nc.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://jt.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lm.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ls.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://ls.nicolike.cn

[B09] break 与 continue
来源：http://lv.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lm.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bp.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kf.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nr.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iw.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ph.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://tz.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pu.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ti.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://na.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ai.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zz.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://me.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hv.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ny.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://ha.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://pz.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://pd.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tc.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rk.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lu.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://is.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dz.huanxung.cn

[B12] 跳出多层循环
来源：http://ri.szxytkj.cn


<!-- 参考信息 -->