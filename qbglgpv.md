代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://tb.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fa.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gq.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eo.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oo.chemitech.net.cn

[A07] 数字转字符串
来源：http://xb.hahajie.cn

Py:   str(42)
来源：http://jy.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://ly.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://lg.shxzskj.cn

TS:   String(42)
来源：http://hf.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uj.521024.cn

Go:   strconv.Itoa(42)
来源：http://un.shxzskj.cn

Ruby: 42.to_s
来源：http://hw.hahajie.cn

C#:   42.ToString()
来源：http://ta.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://sb.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pk.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ow.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ms.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ux.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lf.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gt.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pi.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qk.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://yw.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://la.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qw.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mf.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bq.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vm.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ep.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ez.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tg.huixiangedu.cn

[A10] 生成随机数
来源：http://un.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://ri.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://qd.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oj.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qx.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://hi.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tg.bjjhwx.cn

Ruby: rand(1..100)
来源：http://qz.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://tt.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://rj.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://vx.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eb.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vr.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vo.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://zv.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ey.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://os.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://as.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://oc.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rj.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jr.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://qq.asd995.cn

TS:   `Hello, ${name}!`
来源：http://he.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://ev.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vt.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://qe.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://bf.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rs.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://jq.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://tn.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://zd.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://ek.newstarts.cn

Java: "第一行\n第二行"
来源：http://mv.nszjky.cn

Go:   "第一行\n第二行"
来源：http://le.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://fe.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://ye.colortex.cn

[A14] 注释写法
来源：http://ol.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vd.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://us.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://sa.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://ab.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oj.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://zn.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ik.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ns.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://pn.9csxet.cn

Py:   value = data or "默认值"
来源：http://vq.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://wh.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ui.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://zq.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hj.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://pk.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://nb.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://nu.hnjuh.cn

[A16] 真假值判断规则
来源：http://de.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cm.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tp.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uf.szxytkj.cn

TS:   if (!x) {}
来源：http://ir.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xa.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xp.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gd.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pm.jianghongdianzi.cn

[A17] 位运算
来源：http://vs.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://im.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ge.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tt.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tv.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kq.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wg.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rk.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://ak.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://hw.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://rw.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cm.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ql.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://hj.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vc.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://na.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://tg.wgjwhj.cn

[A19] 交换两个变量
来源：http://ad.jctech888.com.cn

Py:   a, b = b, a
来源：http://pg.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kh.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://lr.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://qr.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ds.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ys.lnxyls.cn

Ruby: a, b = b, a
来源：http://gn.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://eo.yuexingan06.cn

[A20] 读取标准输入
来源：http://mi.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://vu.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ha.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xe.521024.cn

TS:   // Node.js：readline 模块
来源：http://ds.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://yq.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dn.521024.cn

Ruby: gets.chomp
来源：http://hx.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://sz.nicolike.cn

[A21] 保留指定小数位输出
来源：http://vc.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://es.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gv.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ew.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://tn.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://js.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ia.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://gh.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://cn.yuexingan06.cn

[A22] 获取字符串长度
来源：http://qm.521024.cn

Py:   len(s)
来源：http://ch.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eu.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rh.szxytkj.cn

TS:   s.length
来源：http://an.521024.cn

Java: s.length()
来源：http://zq.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cy.gzmigu.cn

Ruby: s.length
来源：http://ib.panjiajie.cn

C#:   s.Length
来源：http://pr.newstarts.cn

[A23] 大小写转换
来源：http://je.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vf.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zu.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ul.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bn.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nc.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zm.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xk.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nl.nicolike.cn

[A24] 去除首尾空白
来源：http://rc.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nb.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qo.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tw.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gu.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://op.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://fc.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zq.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ck.nszjky.cn

[A25] 字符串比较
来源：http://xx.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://vv.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nq.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rf.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jl.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nu.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ow.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lg.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://jk.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://il.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cr.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nh.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://ch.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cc.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oo.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xr.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dq.hnjuh.cn

================================================================================
来源：http://xp.lnxyls.cn

B. 流程控制
来源：http://vv.hnjuh.cn

================================================================================
来源：http://mx.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://sm.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ee.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lf.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ss.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://do.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cm.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ga.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ue.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ew.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ux.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://at.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ga.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gk.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://za.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ph.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wl.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bh.shxzukj.cn

[B03] switch / match / case
来源：http://du.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ue.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rl.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wy.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bb.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cz.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://or.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aj.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rc.wgjwhj.cn

[B04] for 计数循环
来源：http://hn.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://bf.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bm.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hb.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sl.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ts.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://hb.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gd.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://de.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://tc.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ek.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cw.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gm.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sw.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qa.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ch.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mv.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://ky.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vn.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://op.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ys.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wz.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mc.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kh.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aw.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wo.wgjwhj.cn

[B07] while 循环
来源：http://yw.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://lx.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ms.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://de.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://qi.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://dr.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gi.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://vv.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://cx.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://rs.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://cu.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yk.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://df.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://qu.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://hf.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pe.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jo.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://sf.newstarts.cn

[B09] break 与 continue
来源：http://gs.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://de.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nh.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dm.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pl.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jr.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xt.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iv.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ms.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mc.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gd.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rb.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hi.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xo.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oz.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://os.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ea.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://dt.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ex.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ao.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nk.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ub.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ot.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://vw.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dc.nicolike.cn

[B12] 跳出多层循环
来源：http://ic.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ye.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://en.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yv.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qz.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://im.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jj.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pn.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xa.hnjuh.cn

[B13] 判断是否为数字
来源：http://vx.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://va.gzmigu.cn

PHP:  is_numeric($x)
来源：http://zy.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.wgjwhj.cn


<!-- 参考信息 -->