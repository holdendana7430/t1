代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://db.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fo.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://wh.hnjuh.cn

[A05] 整数除法与取模
来源：http://yx.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pt.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kr.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vd.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bp.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://hl.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://vp.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://kz.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://ml.asd995.cn

[A06] 字符串转数字
来源：http://my.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://lx.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pf.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cu.huixiangedu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fp.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ma.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fp.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ln.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xc.bookmarksfly.cn

[A07] 数字转字符串
来源：http://oe.shxzskj.cn

Py:   str(42)
来源：http://kw.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://ak.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://kw.szsharing.cn

TS:   String(42)
来源：http://qo.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sz.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://mf.colortex.cn

Ruby: 42.to_s
来源：http://id.9csxet.cn

C#:   42.ToString()
来源：http://xt.newstarts.cn

[A08] 取整与四舍五入
来源：http://dl.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hy.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xz.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lk.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mh.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nw.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hp.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ot.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fj.521024.cn

[A09] 绝对值与最大最小值
来源：http://jf.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rp.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wb.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ms.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://my.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ie.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ut.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pr.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ty.haigaiapp.cn

[A10] 生成随机数
来源：http://lo.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://ns.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://pv.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jq.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kt.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://hs.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lj.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://qk.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://ci.521024.cn

[A11] 条件表达式（三元）
来源：http://at.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://td.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cz.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ec.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cr.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://qt.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ty.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://on.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nh.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://tx.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ko.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jx.colortex.cn

JS:   `Hello, ${name}!`
来源：http://dx.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://fe.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://se.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://va.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://hj.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://qo.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ga.hahajie.cn

Py:   "第一行\n第二行"
来源：http://kr.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://xz.hahajie.cn

JS:   "第一行\n第二行"
来源：http://cw.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://ag.panjiajie.cn

Java: "第一行\n第二行"
来源：http://qp.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://fd.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://rf.nszjky.cn

C#:   "第一行\n第二行"
来源：http://at.jctech888.com.cn

[A14] 注释写法
来源：http://vp.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ki.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://er.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://xy.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://tf.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ym.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://lo.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://il.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://pk.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://gj.colortex.cn

Py:   value = data or "默认值"
来源：http://fc.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://gr.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://ls.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://yk.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gu.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://pk.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://jf.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://pk.hahajie.cn

[A16] 真假值判断规则
来源：http://fm.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://di.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ir.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cb.szxytkj.cn

TS:   if (!x) {}
来源：http://hq.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://la.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://on.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gi.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ip.shxzskj.cn

[A17] 位运算
来源：http://ur.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lw.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mi.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cn.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jk.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lk.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://lq.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://tz.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://vm.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yx.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.521024.cn

Java: (int) 'A'; (char) 65
来源：http://tr.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ia.521024.cn

Ruby: "A".ord; 65.chr
来源：http://so.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://xr.wgjwhj.cn

[A19] 交换两个变量
来源：http://ri.hnjuh.cn

Py:   a, b = b, a
来源：http://wg.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ll.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://ih.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://kv.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://fl.shtwfgs.cn

Go:   a, b = b, a
来源：http://ay.newstarts.cn

Ruby: a, b = b, a
来源：http://up.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://tz.chemitech.net.cn

[A20] 读取标准输入
来源：http://pc.hahajie.cn

Py:   name = input("请输入：")
来源：http://cd.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vt.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lk.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://vb.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://lk.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mh.nicolike.cn

Ruby: gets.chomp
来源：http://kq.szxytkj.cn

C#:   Console.ReadLine();
来源：http://zk.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://it.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://fc.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lf.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://vn.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://sa.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://yd.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hw.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ef.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://ra.shxzskj.cn

[A22] 获取字符串长度
来源：http://kt.yuexingan06.cn

Py:   len(s)
来源：http://kn.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rh.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aj.jianghongdianzi.cn

TS:   s.length
来源：http://vn.nicolike.cn

Java: s.length()
来源：http://dz.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pz.yuntaijiaju.cn

Ruby: s.length
来源：http://fm.jianghongdianzi.cn

C#:   s.Length
来源：http://qk.huixiangedu.cn

[A23] 大小写转换
来源：http://jx.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zy.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ot.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pt.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wc.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fw.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sb.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rr.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oe.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://gg.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bs.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ru.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jf.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rm.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ud.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ew.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wj.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qv.colortex.cn

[A25] 字符串比较
来源：http://qj.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://jk.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kx.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vc.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ue.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wb.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qd.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qk.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://is.newstarts.cn

[A26] 类型转换总览
来源：http://iu.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cr.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gu.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yu.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://jp.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://as.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ww.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yl.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ry.huixinmuqiang.cn

================================================================================
来源：http://mp.asd995.cn

B. 流程控制
来源：http://ms.huanxung.cn

================================================================================
来源：http://mc.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ae.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cj.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wc.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://op.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gm.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gr.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rx.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zd.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cj.521024.cn

[B02] 多分支 else if / elif
来源：http://sw.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fq.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ni.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vm.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wy.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ke.chemitech.net.cn

[B03] switch / match / case
来源：http://pk.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nz.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uh.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ns.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sh.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fd.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tz.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qn.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://om.szxytkj.cn

[B04] for 计数循环
来源：http://pa.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://lx.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fk.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sn.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jw.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oc.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ad.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://zu.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fz.asd995.cn

[B05] 遍历数组 / 列表
来源：http://tm.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://qk.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rb.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nv.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mr.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ti.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aa.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://ye.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jb.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://he.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xd.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rl.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pf.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ba.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rf.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lk.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ct.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gh.jianghongdianzi.cn

[B07] while 循环
来源：http://xh.huanxung.cn

Py:   while i < 10: i += 1
来源：http://xf.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://po.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://hp.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://xf.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://rc.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://if.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://wn.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://vz.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://pe.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://no.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lq.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://hf.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://xx.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://vf.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ik.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ht.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://vq.shxzskj.cn

[B09] break 与 continue
来源：http://fu.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ed.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qd.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ct.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cr.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fm.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.asd995.cn

[B10] 遍历同时拿索引
来源：http://tf.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rz.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xk.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gd.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yr.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ej.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://si.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wn.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fx.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://pe.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://gq.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://nh.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ev.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wd.nicolike.cn


<!-- 参考信息 -->