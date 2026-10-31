代发 wailian999

Ruby: PI = 3.14159
来源：http://gg.colortex.cn

C#:   const double PI = 3.14159;
来源：http://oo.szsharing.cn

[A04] 判断变量类型
来源：http://uy.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fs.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mc.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tm.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://kn.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ie.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kb.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vu.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://sd.szxytkj.cn

[A05] 整数除法与取模
来源：http://kt.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gg.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pk.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ys.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nu.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://sl.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://zm.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://aa.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://gh.jctech888.com.cn

[A06] 字符串转数字
来源：http://sm.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://gp.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vj.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qs.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jf.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qe.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ro.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vq.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uu.shxzskj.cn

[A07] 数字转字符串
来源：http://xd.huanxung.cn

Py:   str(42)
来源：http://dk.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://xf.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://vh.yuntaijiaju.cn

TS:   String(42)
来源：http://we.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cq.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://aj.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://xf.yuexingan06.cn

C#:   42.ToString()
来源：http://ny.shxzukj.cn

[A08] 取整与四舍五入
来源：http://mr.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mg.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xh.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fp.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zd.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nk.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mx.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zu.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xv.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://lz.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://of.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tr.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hw.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cm.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://td.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vk.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bl.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rx.shxzskj.cn

[A10] 生成随机数
来源：http://ca.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://xp.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://bs.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oo.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rt.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://uj.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ps.asd995.cn

Ruby: rand(1..100)
来源：http://kw.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://zy.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://zw.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://ib.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mz.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zf.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ss.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://vj.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://og.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zy.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pm.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://lf.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ic.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ez.asd995.cn

JS:   `Hello, ${name}!`
来源：http://qw.521024.cn

TS:   `Hello, ${name}!`
来源：http://ap.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://rp.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xm.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://wi.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://fy.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oi.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://li.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://gk.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://ms.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://im.521024.cn

Java: "第一行\n第二行"
来源：http://vy.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://nh.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://ie.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://hm.nszjky.cn

[A14] 注释写法
来源：http://va.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ul.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sa.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://gr.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://ee.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kt.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ks.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pe.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://he.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://re.gzmigu.cn

Py:   value = data or "默认值"
来源：http://mq.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://aw.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://ex.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://hi.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://re.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://ke.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://ez.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://qj.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://ry.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ib.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vm.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rl.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://wk.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yz.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://um.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fp.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lv.shxzukj.cn

[A17] 位运算
来源：http://xu.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://or.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ux.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ey.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xc.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://mc.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://zx.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://wg.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://js.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://up.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://hz.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://er.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ew.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://on.9csxet.cn

[A19] 交换两个变量
来源：http://lj.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://xl.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ia.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://ih.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://cv.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://uq.bjjhwx.cn

Go:   a, b = b, a
来源：http://mo.huanxung.cn

Ruby: a, b = b, a
来源：http://ny.521024.cn

C#:   (a, b) = (b, a);
来源：http://xj.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://ue.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://rn.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pu.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rf.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://jn.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://rs.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nt.muxihuayi.cn

Ruby: gets.chomp
来源：http://jg.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ho.colortex.cn

[A21] 保留指定小数位输出
来源：http://jj.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://dy.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oc.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://ak.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://ms.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://jf.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://up.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://xk.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://kl.nicolike.cn

[A22] 获取字符串长度
来源：http://yx.asd995.cn

Py:   len(s)
来源：http://jd.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fx.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lb.shxzskj.cn

TS:   s.length
来源：http://ao.lnxyls.cn

Java: s.length()
来源：http://jf.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bj.szxytkj.cn

Ruby: s.length
来源：http://ru.hnjuh.cn

C#:   s.Length
来源：http://wo.colortex.cn

[A23] 大小写转换
来源：http://re.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ks.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cl.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://je.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zg.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hu.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://we.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gw.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ou.hahajie.cn

[A24] 去除首尾空白
来源：http://wp.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mk.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uz.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sw.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lm.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bh.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://xc.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rf.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kj.521024.cn

[A25] 字符串比较
来源：http://pc.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://oc.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hl.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ob.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pa.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ie.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yu.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ej.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fj.hahajie.cn

[A26] 类型转换总览
来源：http://cw.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hc.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tv.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sy.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://wg.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://my.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jo.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iq.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mu.yuntaijiaju.cn

================================================================================
来源：http://nx.hahajie.cn

B. 流程控制
来源：http://cg.huixiangedu.cn

================================================================================
来源：http://hd.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://ty.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cr.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ck.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ma.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ml.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qd.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wr.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jc.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://un.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://cn.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sm.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ao.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uk.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vl.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dz.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://db.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.panjiajie.cn

[B03] switch / match / case
来源：http://br.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fe.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yi.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uy.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ku.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vz.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ox.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://so.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jv.yuntaijiaju.cn

[B04] for 计数循环
来源：http://ui.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://mu.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cm.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hs.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sp.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vc.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qa.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://hr.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yi.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://hl.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ui.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ot.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xm.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xe.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uq.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vn.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://uh.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xe.asd995.cn

[B06] 遍历字典 / 对象
来源：http://eh.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lp.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fj.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hp.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ao.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yk.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mu.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tk.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ev.nicolike.cn

[B07] while 循环
来源：http://ll.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://xb.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sz.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://nj.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://mi.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://fv.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ct.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ea.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ig.colortex.cn

[B08] do-while（至少执行一次）
来源：http://hy.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://ld.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ri.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://oj.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://gh.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://tf.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://re.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wx.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://yo.asd995.cn

[B09] break 与 continue
来源：http://xy.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ba.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ca.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ov.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ma.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bw.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://nh.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yz.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qc.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gg.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ya.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ir.lnxyls.cn


<!-- 参考信息 -->