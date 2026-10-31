代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://kv.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fy.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://ls.lnxyls.cn

[A05] 整数除法与取模
来源：http://ly.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nn.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fo.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ph.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ci.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://xq.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://gk.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://jq.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://vj.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://lx.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://tl.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vb.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ee.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yk.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nm.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jn.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ef.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rd.lnxyls.cn

[A07] 数字转字符串
来源：http://ye.bookmarksfly.cn

Py:   str(42)
来源：http://kg.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://lh.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://pl.colortex.cn

TS:   String(42)
来源：http://bi.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vd.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://kd.lnxyls.cn

Ruby: 42.to_s
来源：http://hp.muxihuayi.cn

C#:   42.ToString()
来源：http://wb.521024.cn

[A08] 取整与四舍五入
来源：http://oz.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zk.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://at.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hb.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vw.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lv.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oq.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://li.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mo.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://xb.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bf.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ub.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mb.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pi.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zj.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jh.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vg.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ha.nszjky.cn

[A10] 生成随机数
来源：http://ey.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://yw.nicolike.cn

PHP:  random_int(1, 100);
来源：http://wr.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cd.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://us.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ex.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ve.panjiajie.cn

Ruby: rand(1..100)
来源：http://xa.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://xe.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://dn.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://dk.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xb.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nq.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ut.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://vc.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ch.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vz.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://om.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ki.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ne.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://sh.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://kg.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://ye.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zy.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://ku.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://lz.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iv.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://mn.colortex.cn

PHP:  "第一行\n第二行"
来源：http://jk.szsharing.cn

JS:   "第一行\n第二行"
来源：http://kk.9csxet.cn

TS:   "第一行\n第二行"
来源：http://rm.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://vw.nicolike.cn

Go:   "第一行\n第二行"
来源：http://bb.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://zj.hahajie.cn

C#:   "第一行\n第二行"
来源：http://qu.panjiajie.cn

[A14] 注释写法
来源：http://jd.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jj.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bp.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://tl.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://zj.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tn.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://mv.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ru.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://dd.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://pl.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://az.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://ks.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://wl.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://ub.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ia.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://vw.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://rd.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://tp.newstarts.cn

[A16] 真假值判断规则
来源：http://fw.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kr.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://br.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fy.shxzskj.cn

TS:   if (!x) {}
来源：http://jd.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qi.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mm.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rw.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dn.bookmarksfly.cn

[A17] 位运算
来源：http://pj.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kz.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bm.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rj.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kf.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://al.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qc.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://vt.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://xy.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://nb.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dt.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://yk.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ya.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://ro.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://mw.newstarts.cn

[A19] 交换两个变量
来源：http://wt.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://gi.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fk.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://cv.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://zs.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://dg.nicolike.cn

Go:   a, b = b, a
来源：http://hq.colortex.cn

Ruby: a, b = b, a
来源：http://yb.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://yx.asd995.cn

[A20] 读取标准输入
来源：http://dq.gzmigu.cn

Py:   name = input("请输入：")
来源：http://ww.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rr.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tg.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://qs.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://bu.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kf.shtwfgs.cn

Ruby: gets.chomp
来源：http://ra.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://op.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://qw.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://gd.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://me.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://bj.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://ri.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://bl.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xp.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ve.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://kt.hahajie.cn

[A22] 获取字符串长度
来源：http://uz.9csxet.cn

Py:   len(s)
来源：http://vr.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bo.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ce.nszjky.cn

TS:   s.length
来源：http://fj.shtwfgs.cn

Java: s.length()
来源：http://rm.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zm.huanxung.cn

Ruby: s.length
来源：http://nm.szxytkj.cn

C#:   s.Length
来源：http://uy.huixiangedu.cn

[A23] 大小写转换
来源：http://ny.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dk.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pg.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pf.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ss.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uo.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wa.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fv.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://de.gzmigu.cn

[A24] 去除首尾空白
来源：http://is.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ve.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://re.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bo.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qa.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uo.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://tu.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lz.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bp.jianghongdianzi.cn

[A25] 字符串比较
来源：http://lp.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://bz.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dl.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://md.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kb.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nt.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ml.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://df.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iq.wgjwhj.cn

[A26] 类型转换总览
来源：http://ri.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sg.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zw.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ya.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://sg.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://br.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aq.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ui.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vq.shxzukj.cn

================================================================================
来源：http://vx.gzmigu.cn

B. 流程控制
来源：http://wl.lnxyls.cn

================================================================================
来源：http://ot.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://ma.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nq.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qq.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ag.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nn.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://af.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sz.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tg.9csxet.cn

[B02] 多分支 else if / elif
来源：http://bj.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wk.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://da.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sm.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://my.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bh.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ss.nicolike.cn

[B03] switch / match / case
来源：http://nz.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cy.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ax.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ol.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://je.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ce.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vl.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bc.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ax.wgjwhj.cn

[B04] for 计数循环
来源：http://lv.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ff.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://op.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://su.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qq.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ps.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xv.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://xu.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.colortex.cn

[B05] 遍历数组 / 列表
来源：http://ad.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://sh.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://an.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hh.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uw.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://js.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xc.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://sm.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cb.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://zv.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://by.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hw.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rs.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ka.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bb.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://it.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oq.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tr.huixinmuqiang.cn

[B07] while 循环
来源：http://sk.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://sr.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hf.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://eb.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://ut.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://yj.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hu.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://uk.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://fv.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://qd.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://sv.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sk.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://sq.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://cl.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://wy.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lw.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ae.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://yp.shxzskj.cn

[B09] break 与 continue
来源：http://wb.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://si.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oi.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hh.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sd.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yr.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yg.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://of.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nx.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uf.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ij.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hm.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gr.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lv.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uy.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fd.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://ua.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ow.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://ut.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tr.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ay.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://li.9csxet.cn


<!-- 参考信息 -->