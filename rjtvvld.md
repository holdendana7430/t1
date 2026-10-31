代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kd.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vb.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wu.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://di.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://sz.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://uv.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://fn.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://rj.hahajie.cn

[A06] 字符串转数字
来源：http://gp.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://xi.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hb.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ib.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gm.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ei.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rr.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oy.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://id.bjjhwx.cn

[A07] 数字转字符串
来源：http://ka.hnjuh.cn

Py:   str(42)
来源：http://fv.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://fc.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://vi.huanxung.cn

TS:   String(42)
来源：http://po.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qg.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://gj.gzmigu.cn

Ruby: 42.to_s
来源：http://sd.szsharing.cn

C#:   42.ToString()
来源：http://mt.newstarts.cn

[A08] 取整与四舍五入
来源：http://qq.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hk.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://an.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ay.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eh.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iw.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ls.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://om.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uz.asd995.cn

[A09] 绝对值与最大最小值
来源：http://ze.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vu.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://il.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vt.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://av.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bx.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eq.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ri.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ke.muxihuayi.cn

[A10] 生成随机数
来源：http://je.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://dm.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://qm.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oy.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hp.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://sa.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hq.chemitech.net.cn

Ruby: rand(1..100)
来源：http://hp.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://rg.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://ze.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://ae.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vv.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bn.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ze.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://gi.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xe.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ym.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ys.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://te.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cv.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dt.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://mr.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://tz.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://hk.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yt.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://dj.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://pu.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://td.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://nj.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://xn.colortex.cn

JS:   "第一行\n第二行"
来源：http://pk.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://we.shxzukj.cn

Java: "第一行\n第二行"
来源：http://ok.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://hw.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://tl.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://li.hahajie.cn

[A14] 注释写法
来源：http://pe.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ud.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uk.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://jd.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://wb.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zu.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://ya.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fe.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://mw.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ql.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://ep.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://sc.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://om.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://uo.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wq.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ws.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://yq.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://gj.nszjky.cn

[A16] 真假值判断规则
来源：http://ir.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rq.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jh.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zv.nicolike.cn

TS:   if (!x) {}
来源：http://mc.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xw.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ci.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tz.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pv.yuntaijiaju.cn

[A17] 位运算
来源：http://cf.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uh.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fa.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pb.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oj.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vm.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cz.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oa.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://az.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://iq.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://nk.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uo.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cp.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://ka.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://if.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://kk.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://vp.shtwfgs.cn

[A19] 交换两个变量
来源：http://zj.bookmarksfly.cn

Py:   a, b = b, a
来源：http://ib.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cc.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://cg.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://zy.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://jy.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://ly.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://yd.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://lj.shxzskj.cn

[A20] 读取标准输入
来源：http://rj.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://sh.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://um.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wf.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://kp.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://ed.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pr.colortex.cn

Ruby: gets.chomp
来源：http://zo.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://pq.9csxet.cn

[A21] 保留指定小数位输出
来源：http://vv.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://vl.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cl.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://qh.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://rw.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://dx.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ym.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://dt.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://im.szxytkj.cn

[A22] 获取字符串长度
来源：http://ql.gzmigu.cn

Py:   len(s)
来源：http://bd.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fn.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vr.wgjwhj.cn

TS:   s.length
来源：http://hk.huixinmuqiang.cn

Java: s.length()
来源：http://fb.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ut.panjiajie.cn

Ruby: s.length
来源：http://on.chemitech.net.cn

C#:   s.Length
来源：http://ji.shxzskj.cn

[A23] 大小写转换
来源：http://oi.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rh.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xm.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eg.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://te.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mg.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ic.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ax.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gs.hnjuh.cn

[A24] 去除首尾空白
来源：http://ue.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xy.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ds.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iy.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kk.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pi.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://tu.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ck.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bh.huixiangedu.cn

[A25] 字符串比较
来源：http://di.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://wz.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://re.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nf.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fi.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ms.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ik.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nw.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://px.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://za.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cr.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ap.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lq.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://ka.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bs.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zi.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://or.shxzskj.cn

================================================================================
来源：http://ub.jianghongdianzi.cn

B. 流程控制
来源：http://hr.wgjwhj.cn

================================================================================
来源：http://ex.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://cw.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zt.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mw.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fs.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ib.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yi.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kb.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tt.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://mo.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cf.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://im.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gv.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.hahajie.cn

[B03] switch / match / case
来源：http://oa.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://is.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wq.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bl.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mu.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ox.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ye.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dx.huanxung.cn

[B04] for 计数循环
来源：http://tm.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://bm.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nf.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bl.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://su.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://to.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cd.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://zz.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nr.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://fe.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://vo.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bb.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ob.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cs.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pq.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uw.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://qt.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nf.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://iu.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sl.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ug.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ht.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kg.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://us.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ok.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lp.huixinmuqiang.cn

[B07] while 循环
来源：http://fs.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ar.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iv.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://rl.521024.cn

TS:   while (i < 10) { i++; }
来源：http://eo.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://in.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://js.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://mi.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://ty.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://mr.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://dk.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dr.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://pu.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://lt.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://nt.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://il.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://is.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://pz.haigaiapp.cn

[B09] break 与 continue
来源：http://tr.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pi.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jy.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qg.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vn.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jj.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tx.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jl.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ny.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kn.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kb.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ve.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yl.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mg.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tk.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wf.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://um.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://ns.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://jg.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://ou.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dx.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sy.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ve.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ya.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://ak.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fm.shtwfgs.cn

[B12] 跳出多层循环
来源：http://he.yuntaijiaju.cn


<!-- 参考信息 -->