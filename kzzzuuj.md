代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://ic.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://aw.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://kz.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://hs.shtwfgs.cn

[A06] 字符串转数字
来源：http://jm.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://ex.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hh.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nk.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jz.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pw.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wr.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mx.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wb.newstarts.cn

[A07] 数字转字符串
来源：http://qw.newstarts.cn

Py:   str(42)
来源：http://wl.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://yx.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://lc.shxzskj.cn

TS:   String(42)
来源：http://rw.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bl.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://cg.huanxung.cn

Ruby: 42.to_s
来源：http://um.chemitech.net.cn

C#:   42.ToString()
来源：http://qp.lnxyls.cn

[A08] 取整与四舍五入
来源：http://ia.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ba.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uk.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tm.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mb.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ne.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://op.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jq.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ak.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://og.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lk.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pr.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gt.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hb.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nu.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://or.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ts.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://it.lnxyls.cn

[A10] 生成随机数
来源：http://ze.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://rm.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ct.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zy.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ik.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ip.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nj.gzmigu.cn

Ruby: rand(1..100)
来源：http://bf.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://li.9csxet.cn

[A11] 条件表达式（三元）
来源：http://hv.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://qu.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://as.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kr.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hi.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://fw.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xt.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uj.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://al.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://iy.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ye.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dp.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://jj.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://vv.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ta.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mp.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://rw.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://xf.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rs.hahajie.cn

Py:   "第一行\n第二行"
来源：http://to.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://yj.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://pu.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://rw.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://tj.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://so.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://zi.huanxung.cn

C#:   "第一行\n第二行"
来源：http://zt.huixinmuqiang.cn

[A14] 注释写法
来源：http://ga.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lj.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fp.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://eh.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://gv.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://je.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://ax.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rr.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://pi.shxzskj.cn

[A15] 空值判断与默认值
来源：http://lr.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://me.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://dp.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://kf.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://gw.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://mc.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://tt.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://pd.panjiajie.cn

[A16] 真假值判断规则
来源：http://ll.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tp.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kj.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cv.nicolike.cn

TS:   if (!x) {}
来源：http://hm.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uz.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://si.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://et.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nt.lnxyls.cn

[A17] 位运算
来源：http://vr.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xc.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qt.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wl.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://um.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kv.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://um.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://eb.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://kd.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vz.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://df.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://cl.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ym.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://du.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://um.szsharing.cn

[A19] 交换两个变量
来源：http://gj.nicolike.cn

Py:   a, b = b, a
来源：http://ju.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ce.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://cd.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://eo.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://ig.nszjky.cn

Go:   a, b = b, a
来源：http://zn.huanxung.cn

Ruby: a, b = b, a
来源：http://oe.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://kq.huixiangedu.cn

[A20] 读取标准输入
来源：http://gk.9csxet.cn

Py:   name = input("请输入：")
来源：http://pm.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qc.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yb.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://zm.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://wm.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sl.9csxet.cn

Ruby: gets.chomp
来源：http://vk.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://lw.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://gj.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://nl.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xw.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://gp.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://cg.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://fy.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lw.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://aq.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://xf.hnjuh.cn

[A22] 获取字符串长度
来源：http://hp.yuntaijiaju.cn

Py:   len(s)
来源：http://ut.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bk.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://na.jctech888.com.cn

TS:   s.length
来源：http://ce.newstarts.cn

Java: s.length()
来源：http://my.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mr.haigaiapp.cn

Ruby: s.length
来源：http://jz.newstarts.cn

C#:   s.Length
来源：http://tw.jianghongdianzi.cn

[A23] 大小写转换
来源：http://pr.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nc.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ya.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tn.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fa.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iu.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ua.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pe.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nj.bjjhwx.cn

[A24] 去除首尾空白
来源：http://gf.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fq.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jj.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cu.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pv.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xl.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://ku.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xq.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tc.newstarts.cn

[A25] 字符串比较
来源：http://mu.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://ux.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gm.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cd.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gw.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qf.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://et.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ej.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pf.wgjwhj.cn

[A26] 类型转换总览
来源：http://wi.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bj.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://id.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ix.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://gc.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vy.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://di.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hv.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kw.hnjuh.cn

================================================================================
来源：http://pz.521024.cn

B. 流程控制
来源：http://af.hnjuh.cn

================================================================================
来源：http://wp.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://mb.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ud.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gn.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jh.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ku.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vr.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qx.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://od.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ob.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://yd.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ax.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zj.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jx.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zs.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ul.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ah.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cv.asd995.cn

[B03] switch / match / case
来源：http://kj.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kw.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fy.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gn.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ix.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wx.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zi.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rq.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.colortex.cn

[B04] for 计数循环
来源：http://jx.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://xg.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://en.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sj.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jp.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oa.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ph.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://dt.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uf.521024.cn

[B05] 遍历数组 / 列表
来源：http://dt.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://ca.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eu.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wd.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sh.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wb.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bc.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://iu.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hb.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://yh.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cr.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gj.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zq.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bx.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qp.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pp.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rg.hnjuh.cn

[B07] while 循环
来源：http://lr.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://fw.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pr.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://lg.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://zj.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://vp.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dw.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://sb.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://sb.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://cz.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://dx.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fa.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://fg.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://fh.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://da.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qz.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gq.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.wgjwhj.cn

[B09] break 与 continue
来源：http://vy.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mn.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ou.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aw.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ma.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://se.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.colortex.cn

[B10] 遍历同时拿索引
来源：http://ka.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ts.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qk.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sg.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pe.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nh.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rm.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ij.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ks.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://nn.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://yc.asd995.cn

PHP:  range(0, 10, 2);
来源：http://fk.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qd.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tn.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bb.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cm.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://zv.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ts.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://uu.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mk.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iu.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mq.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://il.nicolike.cn


<!-- 参考信息 -->