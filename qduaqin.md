代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://ik.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://fj.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://tw.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://ea.colortex.cn

[A06] 字符串转数字
来源：http://lp.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://jl.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pw.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dy.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vt.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mb.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://on.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ci.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bg.chemitech.net.cn

[A07] 数字转字符串
来源：http://cf.huixinmuqiang.cn

Py:   str(42)
来源：http://fv.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://nv.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://wi.gzmigu.cn

TS:   String(42)
来源：http://kc.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ol.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://jn.panjiajie.cn

Ruby: 42.to_s
来源：http://el.yuexingan06.cn

C#:   42.ToString()
来源：http://pi.hnjuh.cn

[A08] 取整与四舍五入
来源：http://na.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rs.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://us.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lu.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zi.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qc.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ic.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dk.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xn.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://tj.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ur.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ye.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://th.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ci.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qm.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bk.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://av.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jx.szsharing.cn

[A10] 生成随机数
来源：http://uo.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://vx.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://dx.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uo.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sj.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://eb.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wp.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://ny.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://jc.nszjky.cn

[A11] 条件表达式（三元）
来源：http://da.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://sd.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ed.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uu.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://td.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://qj.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://em.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://up.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ze.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://lm.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pp.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cx.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://vr.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://ko.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://hw.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://da.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://ob.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://ck.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yy.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://rw.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://fd.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://qf.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://nk.nicolike.cn

Java: "第一行\n第二行"
来源：http://bc.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://hd.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://dy.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://fp.hahajie.cn

[A14] 注释写法
来源：http://zy.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gh.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cf.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://ei.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://jq.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sl.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://my.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gy.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://is.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://gy.szxytkj.cn

Py:   value = data or "默认值"
来源：http://bl.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://ff.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://bv.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://ru.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zl.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://ag.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://we.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://ih.colortex.cn

[A16] 真假值判断规则
来源：http://jl.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jf.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oy.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gy.521024.cn

TS:   if (!x) {}
来源：http://xb.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ol.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kx.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oh.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qg.nicolike.cn

[A17] 位运算
来源：http://cm.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bw.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lx.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ro.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://nn.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://fk.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://pl.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lj.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lo.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://qc.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mi.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://ua.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://ot.hnjuh.cn

[A19] 交换两个变量
来源：http://xn.lnxyls.cn

Py:   a, b = b, a
来源：http://ym.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hm.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://va.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://tn.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://rp.521024.cn

Go:   a, b = b, a
来源：http://dn.colortex.cn

Ruby: a, b = b, a
来源：http://po.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://cy.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://mc.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ol.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ok.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fs.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://wz.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://pc.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aa.shxzukj.cn

Ruby: gets.chomp
来源：http://zv.hnjuh.cn

C#:   Console.ReadLine();
来源：http://bt.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://mt.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://at.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iu.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://af.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://tt.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://lk.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pt.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://cl.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://xv.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://ta.nszjky.cn

Py:   len(s)
来源：http://jy.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xp.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jw.wgjwhj.cn

TS:   s.length
来源：http://vx.jianghongdianzi.cn

Java: s.length()
来源：http://pm.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zl.jctech888.com.cn

Ruby: s.length
来源：http://wu.asd995.cn

C#:   s.Length
来源：http://yq.shtwfgs.cn

[A23] 大小写转换
来源：http://hg.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ix.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ei.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iu.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bi.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xd.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yi.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mx.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tl.lnxyls.cn

[A24] 去除首尾空白
来源：http://xr.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xz.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pi.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xq.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://of.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://qe.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qd.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://av.hahajie.cn

[A25] 字符串比较
来源：http://qe.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://dy.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qt.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gd.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mw.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xj.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jg.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cy.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ix.521024.cn

[A26] 类型转换总览
来源：http://gh.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sr.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ag.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://be.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://hv.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zf.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zt.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mm.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jg.panjiajie.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

B. 流程控制
来源：http://ru.shxzukj.cn

================================================================================
来源：http://py.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://mw.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uz.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yh.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nj.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://og.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zz.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eb.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dw.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ud.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ha.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gd.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ib.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://it.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ii.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.bookmarksfly.cn

[B03] switch / match / case
来源：http://sb.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ll.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tc.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ad.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vt.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gg.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yk.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cu.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ye.muxihuayi.cn

[B04] for 计数循环
来源：http://su.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://mz.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nl.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xl.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fo.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mq.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://he.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://ol.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qo.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://az.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://yq.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nv.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kv.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jw.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vz.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ey.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://dx.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fe.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://fi.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ff.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://se.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://la.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ow.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lk.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wn.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bz.muxihuayi.cn

[B07] while 循环
来源：http://vp.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://zn.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ux.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://nq.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://ft.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://mz.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yg.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://bm.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://qw.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://hj.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://lc.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://th.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://gs.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://dy.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://ke.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cv.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uw.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://qc.shxzukj.cn

[B09] break 与 continue
来源：http://vs.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ad.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://px.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qx.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sd.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aq.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pb.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kt.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ox.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xz.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vf.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ku.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iv.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xk.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sm.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ej.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://pb.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://fm.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ac.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://py.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://np.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cq.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lr.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://gj.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uj.gzmigu.cn

[B12] 跳出多层循环
来源：http://tr.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pw.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hb.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vp.szxytkj.cn


<!-- 参考信息 -->