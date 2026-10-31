代发 wailian999

Ruby: PI = 3.14159
来源：http://wx.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://to.nicolike.cn

[A04] 判断变量类型
来源：http://bx.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xu.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mb.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ca.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://dx.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aw.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dq.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://to.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://dh.chemitech.net.cn

[A05] 整数除法与取模
来源：http://gp.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nj.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fa.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zs.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wr.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://hp.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://xq.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://ew.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://fk.asd995.cn

[A06] 字符串转数字
来源：http://et.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://tk.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xr.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uc.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gg.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kp.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jp.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qc.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zh.huanxung.cn

[A07] 数字转字符串
来源：http://mv.shtwfgs.cn

Py:   str(42)
来源：http://ev.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://cw.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://qy.newstarts.cn

TS:   String(42)
来源：http://oc.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jz.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://qk.szsharing.cn

Ruby: 42.to_s
来源：http://eh.jianghongdianzi.cn

C#:   42.ToString()
来源：http://ay.9csxet.cn

[A08] 取整与四舍五入
来源：http://id.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bt.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dh.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://md.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ik.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dh.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oy.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tc.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ln.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://vr.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ry.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qc.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kr.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://se.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wq.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mb.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://im.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bf.wgjwhj.cn

[A10] 生成随机数
来源：http://od.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://ry.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://fv.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cg.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oe.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://lf.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dx.521024.cn

Ruby: rand(1..100)
来源：http://eo.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://sp.szsharing.cn

[A11] 条件表达式（三元）
来源：http://lt.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://nn.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lg.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://os.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dg.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://ux.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bi.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://if.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ug.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://an.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lz.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zt.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://sn.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ap.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://qj.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zb.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://zr.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://vp.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fg.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://pb.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://jz.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://hu.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://pi.nicolike.cn

Java: "第一行\n第二行"
来源：http://hv.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://aa.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://xz.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://tq.bjjhwx.cn

[A14] 注释写法
来源：http://rg.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vl.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ht.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://kz.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://lj.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hx.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://jj.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ni.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://dm.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ya.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://pv.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ul.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://jf.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://fv.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kc.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://lg.nszjky.cn

Ruby: value = data || "默认值"
来源：http://zo.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://zg.nicolike.cn

[A16] 真假值判断规则
来源：http://ny.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ot.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lj.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://np.nicolike.cn

TS:   if (!x) {}
来源：http://wh.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sh.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ra.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ff.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ul.newstarts.cn

[A17] 位运算
来源：http://kg.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lj.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qf.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cf.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zj.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://xc.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://di.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://qa.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ui.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://df.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://ym.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://po.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://mo.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://qh.muxihuayi.cn

[A19] 交换两个变量
来源：http://hl.bjjhwx.cn

Py:   a, b = b, a
来源：http://yl.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ki.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ll.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://oi.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://bt.szsharing.cn

Go:   a, b = b, a
来源：http://vb.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://pr.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://gj.huanxung.cn

[A20] 读取标准输入
来源：http://xn.asd995.cn

Py:   name = input("请输入：")
来源：http://ht.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xu.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vp.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://ku.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://qk.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ex.chemitech.net.cn

Ruby: gets.chomp
来源：http://kk.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://zn.asd995.cn

[A21] 保留指定小数位输出
来源：http://hp.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://pk.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vt.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://zn.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://ue.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://rc.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qj.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://mf.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://rk.jctech888.com.cn

[A22] 获取字符串长度
来源：http://gm.wgjwhj.cn

Py:   len(s)
来源：http://xh.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sg.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dv.hahajie.cn

TS:   s.length
来源：http://km.yuntaijiaju.cn

Java: s.length()
来源：http://zz.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lz.newstarts.cn

Ruby: s.length
来源：http://ca.newstarts.cn

C#:   s.Length
来源：http://pg.nszjky.cn

[A23] 大小写转换
来源：http://jj.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://df.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wu.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ff.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fl.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ap.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://km.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qr.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://so.gzmigu.cn

[A24] 去除首尾空白
来源：http://jp.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://km.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://af.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rt.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sw.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lx.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://hp.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eq.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mw.hahajie.cn

[A25] 字符串比较
来源：http://mi.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ri.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sz.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mg.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lh.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oh.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://at.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fv.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://le.lnxyls.cn

[A26] 类型转换总览
来源：http://md.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uo.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jl.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nv.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://wh.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iy.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://si.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ym.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fr.hahajie.cn

================================================================================
来源：http://uv.huanxung.cn

B. 流程控制
来源：http://vg.yuexingan06.cn

================================================================================
来源：http://mp.asd995.cn

[B01] 条件判断 if / else
来源：http://ye.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yv.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vu.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gr.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cc.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ug.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wn.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fc.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hr.szsharing.cn

[B02] 多分支 else if / elif
来源：http://uk.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hr.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nc.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ez.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gu.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bq.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.nicolike.cn

[B03] switch / match / case
来源：http://vo.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jf.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mg.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lm.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://el.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nb.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qd.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mw.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nm.haigaiapp.cn

[B04] for 计数循环
来源：http://zs.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://rp.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wt.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zx.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pf.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rm.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pp.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://sg.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jj.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://hp.colortex.cn

Py:   for item in arr: print(item)
来源：http://hj.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pe.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ft.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xw.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ia.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mw.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://qs.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oo.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://qg.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kp.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gd.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://or.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qj.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zc.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ep.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ft.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hd.lnxyls.cn

[B07] while 循环
来源：http://bp.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://uk.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://um.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://lz.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ht.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://yn.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oe.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://on.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://um.521024.cn

[B08] do-while（至少执行一次）
来源：http://mk.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://wd.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://er.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://cg.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://nq.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://vf.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pf.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mw.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://xx.hahajie.cn

[B09] break 与 continue
来源：http://ts.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sa.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ix.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ir.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://if.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xo.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gb.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://hn.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pc.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ca.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eq.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nz.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xg.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aq.szsharing.cn


<!-- 参考信息 -->