代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://sm.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://hu.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://tv.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://wi.szsharing.cn

[A06] 字符串转数字
来源：http://zq.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://as.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ax.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xi.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ms.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://on.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qm.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nz.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cw.shxzskj.cn

[A07] 数字转字符串
来源：http://we.yuntaijiaju.cn

Py:   str(42)
来源：http://wd.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://ov.colortex.cn

JS:   String(42); (42).toString()
来源：http://pl.asd995.cn

TS:   String(42)
来源：http://gd.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qh.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://jw.wgjwhj.cn

Ruby: 42.to_s
来源：http://bo.hahajie.cn

C#:   42.ToString()
来源：http://zp.shxzskj.cn

[A08] 取整与四舍五入
来源：http://du.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dt.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ia.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wt.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rh.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mm.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mp.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mx.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ou.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://ll.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://on.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dr.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cw.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ij.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nw.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mw.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pq.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wg.nicolike.cn

[A10] 生成随机数
来源：http://xc.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://nb.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://fl.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cc.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://oz.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vc.gzmigu.cn

Ruby: rand(1..100)
来源：http://jy.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://cf.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://fh.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://vc.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jv.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zq.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wc.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://te.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ss.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mm.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vb.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://om.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uf.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mq.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://gv.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://yf.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://bb.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xz.521024.cn

Ruby: "Hello, #{name}!"
来源：http://uq.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://hg.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aa.nszjky.cn

Py:   "第一行\n第二行"
来源：http://ae.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://gx.nicolike.cn

JS:   "第一行\n第二行"
来源：http://md.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://ma.nicolike.cn

Java: "第一行\n第二行"
来源：http://da.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ku.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ju.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://pw.asd995.cn

[A14] 注释写法
来源：http://dm.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gk.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lm.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ke.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://zx.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iu.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://ey.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tr.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://om.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://bp.521024.cn

Py:   value = data or "默认值"
来源：http://hy.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://ft.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://fn.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://jk.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yi.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://ur.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://xw.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://vh.haigaiapp.cn

[A16] 真假值判断规则
来源：http://he.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rb.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fu.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gu.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://zi.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kr.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zq.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tm.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wr.wgjwhj.cn

[A17] 位运算
来源：http://sp.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xf.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oj.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uq.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lp.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://le.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yz.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ks.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://gq.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://pg.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://vh.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ra.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pl.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://ws.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nv.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://qg.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ui.nszjky.cn

[A19] 交换两个变量
来源：http://kj.newstarts.cn

Py:   a, b = b, a
来源：http://md.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oh.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://jv.colortex.cn

TS:   [a, b] = [b, a];
来源：http://qv.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://ql.panjiajie.cn

Go:   a, b = b, a
来源：http://tg.asd995.cn

Ruby: a, b = b, a
来源：http://ja.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://qv.shtwfgs.cn

[A20] 读取标准输入
来源：http://wp.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://mu.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hc.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://so.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://tr.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://eu.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bn.521024.cn

Ruby: gets.chomp
来源：http://zz.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://tv.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://vu.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://qz.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://du.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://id.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://gt.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://br.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qb.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://ld.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://po.huixiangedu.cn

[A22] 获取字符串长度
来源：http://au.nicolike.cn

Py:   len(s)
来源：http://ky.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wp.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://af.yuexingan06.cn

TS:   s.length
来源：http://zh.shtwfgs.cn

Java: s.length()
来源：http://iv.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ji.huixiangedu.cn

Ruby: s.length
来源：http://uj.9csxet.cn

C#:   s.Length
来源：http://lf.huanxung.cn

[A23] 大小写转换
来源：http://xk.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://di.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cy.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hx.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bi.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yw.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fe.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cu.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ht.shtwfgs.cn

[A24] 去除首尾空白
来源：http://mt.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cp.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ft.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oe.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tz.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yh.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://px.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ln.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xy.gzmigu.cn

[A25] 字符串比较
来源：http://zp.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://cs.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jc.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ai.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://db.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zc.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ms.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aj.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xn.nicolike.cn

[A26] 类型转换总览
来源：http://wr.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pa.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ad.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://no.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://qy.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xv.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ml.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://et.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uo.shtwfgs.cn

================================================================================
来源：http://wf.szxytkj.cn

B. 流程控制
来源：http://ro.gzmigu.cn

================================================================================
来源：http://ek.521024.cn

[B01] 条件判断 if / else
来源：http://pu.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kx.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iy.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lp.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aa.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xt.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fx.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ul.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cu.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ar.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ox.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yz.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ez.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jo.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bl.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zv.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.bjjhwx.cn

[B03] switch / match / case
来源：http://vo.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://me.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pm.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lj.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hu.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yc.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zv.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rv.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uf.lnxyls.cn

[B04] for 计数循环
来源：http://vq.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://im.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fj.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://du.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jf.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://we.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://or.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sg.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://wr.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://fl.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nd.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ae.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tn.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tp.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sy.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://zr.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ua.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://rs.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rg.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://di.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bz.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pi.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dw.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hg.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://el.nicolike.cn

[B07] while 循环
来源：http://dr.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://jo.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wv.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://qf.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://fu.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://wq.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iy.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://wl.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://sr.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://xc.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://um.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zq.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://mk.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://cy.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://kx.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yj.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xx.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://yr.wgjwhj.cn

[B09] break 与 continue
来源：http://cq.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://px.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jq.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ou.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dt.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://se.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ef.hahajie.cn

[B10] 遍历同时拿索引
来源：http://cv.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bu.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pv.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xr.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ma.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xv.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uf.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://au.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tk.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://wf.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://bf.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://yh.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ko.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yf.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dz.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wb.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://yt.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tr.9csxet.cn

[B12] 跳出多层循环
来源：http://yf.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://il.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jr.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.panjiajie.cn


<!-- 参考信息 -->