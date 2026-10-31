代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nn.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cc.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://df.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mb.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://sj.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://bh.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://wc.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://qt.asd995.cn

[A06] 字符串转数字
来源：http://ui.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://zp.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pq.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ha.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ig.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dj.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ay.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uk.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dh.szxytkj.cn

[A07] 数字转字符串
来源：http://vl.jianghongdianzi.cn

Py:   str(42)
来源：http://pa.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://ls.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://mz.huixinmuqiang.cn

TS:   String(42)
来源：http://rz.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oh.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://cv.szxytkj.cn

Ruby: 42.to_s
来源：http://ps.jctech888.com.cn

C#:   42.ToString()
来源：http://xg.hahajie.cn

[A08] 取整与四舍五入
来源：http://cd.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://as.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xk.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qy.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wm.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zn.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://im.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lo.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eh.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://xo.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fs.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rp.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qs.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bf.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yg.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oq.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gi.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vv.jctech888.com.cn

[A10] 生成随机数
来源：http://xs.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://gg.nszjky.cn

PHP:  random_int(1, 100);
来源：http://nr.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pj.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wi.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://lg.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gi.lnxyls.cn

Ruby: rand(1..100)
来源：http://dm.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://ps.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://ff.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ow.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kx.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ct.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rh.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://lj.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ga.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oj.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mw.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://yu.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ed.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fm.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://zx.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://sd.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://qk.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ou.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://mx.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://ju.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xq.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://nb.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://xa.colortex.cn

JS:   "第一行\n第二行"
来源：http://ql.521024.cn

TS:   "第一行\n第二行"
来源：http://nl.nszjky.cn

Java: "第一行\n第二行"
来源：http://ci.hahajie.cn

Go:   "第一行\n第二行"
来源：http://sg.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://yr.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://hm.chemitech.net.cn

[A14] 注释写法
来源：http://rl.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vj.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hg.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://co.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://qp.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zj.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://xh.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hi.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://zl.hahajie.cn

[A15] 空值判断与默认值
来源：http://rw.gzmigu.cn

Py:   value = data or "默认值"
来源：http://ii.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://mz.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://co.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://pi.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ki.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://sb.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://px.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://cg.bjjhwx.cn

[A16] 真假值判断规则
来源：http://pm.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dt.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gp.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nb.nszjky.cn

TS:   if (!x) {}
来源：http://np.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://al.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yb.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qz.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pg.shtwfgs.cn

[A17] 位运算
来源：http://nl.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xe.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hg.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zq.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dq.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yo.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mx.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zr.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://rv.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://hf.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://xg.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jr.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cn.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ry.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uu.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://ob.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://xi.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://hf.wgjwhj.cn

Py:   a, b = b, a
来源：http://wq.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fj.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://tb.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://ni.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://ph.shxzukj.cn

Go:   a, b = b, a
来源：http://br.shxzukj.cn

Ruby: a, b = b, a
来源：http://xc.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://ex.szxytkj.cn

[A20] 读取标准输入
来源：http://qj.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://ov.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://za.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oi.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://op.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://px.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ft.wgjwhj.cn

Ruby: gets.chomp
来源：http://sv.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://fr.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://il.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://nd.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yl.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://hf.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://dn.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://lt.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iu.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://gl.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://yc.9csxet.cn

[A22] 获取字符串长度
来源：http://bc.bjjhwx.cn

Py:   len(s)
来源：http://gh.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ws.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jf.colortex.cn

TS:   s.length
来源：http://pq.colortex.cn

Java: s.length()
来源：http://za.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ir.nszjky.cn

Ruby: s.length
来源：http://zh.huixinmuqiang.cn

C#:   s.Length
来源：http://mw.bjjhwx.cn

[A23] 大小写转换
来源：http://lh.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gk.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mn.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vd.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gp.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wc.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qh.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://td.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qw.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://ai.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bc.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dy.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sm.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gz.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zd.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://ws.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ks.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qf.jianghongdianzi.cn

[A25] 字符串比较
来源：http://fo.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://af.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://de.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://of.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ji.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cl.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bc.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iw.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gi.521024.cn

[A26] 类型转换总览
来源：http://ga.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tu.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fc.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cp.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://ul.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xw.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zq.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jp.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iv.lnxyls.cn

================================================================================
来源：http://wb.hahajie.cn

B. 流程控制
来源：http://md.hnjuh.cn

================================================================================
来源：http://xh.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://mu.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nb.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dc.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tc.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zl.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uj.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jq.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ij.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ny.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://qt.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ik.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fb.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xi.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ki.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://su.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lq.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.asd995.cn

[B03] switch / match / case
来源：http://dv.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://en.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ig.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://il.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pb.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jt.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mk.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bm.bookmarksfly.cn

[B04] for 计数循环
来源：http://ub.asd995.cn

Py:   for i in range(10): print(i)
来源：http://yq.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yz.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ug.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iu.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yh.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lq.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://xj.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sy.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://wa.nszjky.cn

Py:   for item in arr: print(item)
来源：http://vb.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pb.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lm.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qc.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wu.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vw.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://if.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zh.521024.cn

[B06] 遍历字典 / 对象
来源：http://mj.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hp.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qa.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zj.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://le.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xp.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cf.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mm.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://km.gzmigu.cn

[B07] while 循环
来源：http://si.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://yf.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vb.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://fk.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://nz.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://ri.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eg.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://um.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://og.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ty.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://of.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://au.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://wa.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://aw.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://ue.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ih.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pz.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://ye.jctech888.com.cn

[B09] break 与 continue
来源：http://nr.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qm.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ld.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yo.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cv.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ic.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://lo.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tn.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uf.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yt.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ez.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rw.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ux.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yu.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://re.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://vl.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://ad.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://lm.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sq.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fi.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ah.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qa.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://bz.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ql.colortex.cn

[B12] 跳出多层循环
来源：http://wd.nicolike.cn


<!-- 参考信息 -->