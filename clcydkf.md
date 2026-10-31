代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://fr.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gm.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://xv.nicolike.cn

[A05] 整数除法与取模
来源：http://ro.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aq.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pw.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ne.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tq.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://ue.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://de.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://id.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://sq.yuexingan06.cn

[A06] 字符串转数字
来源：http://ey.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://yz.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wl.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nm.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hn.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://af.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tk.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kv.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://em.shtwfgs.cn

[A07] 数字转字符串
来源：http://rg.panjiajie.cn

Py:   str(42)
来源：http://xg.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://pi.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://ap.jianghongdianzi.cn

TS:   String(42)
来源：http://xn.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tj.asd995.cn

Go:   strconv.Itoa(42)
来源：http://ui.asd995.cn

Ruby: 42.to_s
来源：http://me.shxzukj.cn

C#:   42.ToString()
来源：http://qs.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://md.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cf.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mm.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kj.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xo.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cv.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uy.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ty.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xp.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://fa.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nz.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ig.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fc.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lr.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mg.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jt.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zk.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ma.bookmarksfly.cn

[A10] 生成随机数
来源：http://ua.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://mh.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://vh.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dw.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nl.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://eq.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oy.shxzukj.cn

Ruby: rand(1..100)
来源：http://nz.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://gx.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://su.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://rq.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dl.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hk.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wj.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://dl.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ib.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ym.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gq.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://ky.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ks.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://on.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://ip.asd995.cn

TS:   `Hello, ${name}!`
来源：http://sf.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://pq.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tv.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://tr.colortex.cn

C#:   $"Hello, {name}!"
来源：http://fo.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cf.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://ff.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://im.newstarts.cn

JS:   "第一行\n第二行"
来源：http://se.newstarts.cn

TS:   "第一行\n第二行"
来源：http://hk.9csxet.cn

Java: "第一行\n第二行"
来源：http://js.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://zv.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://zb.9csxet.cn

C#:   "第一行\n第二行"
来源：http://cs.huanxung.cn

[A14] 注释写法
来源：http://gm.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xr.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rr.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://cy.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://tl.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zf.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://xv.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jt.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://jg.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://bd.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://nk.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://dq.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://yt.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://yt.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hr.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ba.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://zn.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://py.wgjwhj.cn

[A16] 真假值判断规则
来源：http://gm.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uq.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zs.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sd.haigaiapp.cn

TS:   if (!x) {}
来源：http://is.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ba.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ak.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fd.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pi.huixinmuqiang.cn

[A17] 位运算
来源：http://eb.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ej.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ob.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lv.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bs.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ni.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ql.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://uk.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://jp.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ie.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oc.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://po.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://aq.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iu.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://as.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://hj.wgjwhj.cn

[A19] 交换两个变量
来源：http://og.bookmarksfly.cn

Py:   a, b = b, a
来源：http://st.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://go.521024.cn

JS:   [a, b] = [b, a];
来源：http://ey.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://kn.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://bm.lnxyls.cn

Go:   a, b = b, a
来源：http://ez.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://fc.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://hf.bjjhwx.cn

[A20] 读取标准输入
来源：http://hw.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://pb.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uk.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ai.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://dj.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://fu.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xf.huanxung.cn

Ruby: gets.chomp
来源：http://ml.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://rx.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://nw.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://md.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ch.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://qk.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://hz.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://kn.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dx.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://nd.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://sm.yuexingan06.cn

[A22] 获取字符串长度
来源：http://ow.panjiajie.cn

Py:   len(s)
来源：http://aq.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ts.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nm.bjjhwx.cn

TS:   s.length
来源：http://ci.shxzukj.cn

Java: s.length()
来源：http://wl.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ix.hahajie.cn

Ruby: s.length
来源：http://nv.panjiajie.cn

C#:   s.Length
来源：http://fv.huixiangedu.cn

[A23] 大小写转换
来源：http://lm.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xf.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://br.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yi.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rn.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fw.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dj.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tx.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oc.bjjhwx.cn

[A24] 去除首尾空白
来源：http://sk.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sh.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wc.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://al.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ce.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ua.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://hx.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kg.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hx.521024.cn

[A25] 字符串比较
来源：http://sy.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://mp.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zb.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zk.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://af.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vk.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ad.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mg.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yt.panjiajie.cn

[A26] 类型转换总览
来源：http://rd.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ki.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ne.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ou.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://av.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eb.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qg.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ae.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ue.bjjhwx.cn

================================================================================
来源：http://sj.asd995.cn

B. 流程控制
来源：http://oi.szsharing.cn

================================================================================
来源：http://io.gzmigu.cn

[B01] 条件判断 if / else
来源：http://rk.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://at.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ol.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vx.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yd.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bo.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ho.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eu.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://el.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://rl.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lg.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mo.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wl.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.nicolike.cn

[B03] switch / match / case
来源：http://sy.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cw.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rv.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zg.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xv.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dn.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rk.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ey.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tr.nszjky.cn

[B04] for 计数循环
来源：http://rv.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://vf.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lr.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sv.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ar.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vf.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rk.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://ep.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://il.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://zl.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://qw.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lb.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vu.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ki.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hf.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iu.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://jp.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sw.colortex.cn

[B06] 遍历字典 / 对象
来源：http://zu.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qk.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wm.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xz.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://os.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vv.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lg.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zf.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://us.lnxyls.cn

[B07] while 循环
来源：http://vi.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://vx.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fv.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://rp.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://ea.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://os.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ql.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://jl.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://td.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://ps.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://cw.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ms.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://zm.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://jt.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://os.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kl.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wt.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://op.asd995.cn

[B09] break 与 continue
来源：http://ja.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cc.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rs.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fg.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://si.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://th.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qq.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ar.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xp.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://ej.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ut.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xh.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ne.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wm.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hb.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lh.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mo.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ay.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://lu.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://jy.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://hs.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gf.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yy.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tl.nszjky.cn


<!-- 参考信息 -->