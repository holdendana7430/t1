代发 wailian999

Py:   print("Hello, World!")
来源：http://ux.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://xg.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://vy.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zp.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://up.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://dl.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://if.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yn.shxzskj.cn

[A02] 变量声明与赋值
来源：http://xl.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xa.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sk.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://do.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://av.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://jv.521024.cn

Go:   name := "Alex"; age := 20
来源：http://yg.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://mt.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ta.szxytkj.cn

[A03] 常量定义
来源：http://sw.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rc.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://ow.9csxet.cn

JS:   const PI = 3.14159;
来源：http://ob.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://gm.asd995.cn

Java: static final double PI = 3.14159;
来源：http://ue.panjiajie.cn

Go:   const PI = 3.14159
来源：http://gq.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://oq.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://oh.huixiangedu.cn

[A04] 判断变量类型
来源：http://bd.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pj.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mu.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yy.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://gr.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lz.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eg.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tv.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://wt.hnjuh.cn

[A05] 整数除法与取模
来源：http://ht.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pj.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ja.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wo.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oz.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://lo.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://zl.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ue.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://uu.lnxyls.cn

[A06] 字符串转数字
来源：http://xp.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://fw.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uy.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rk.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ih.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ve.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rt.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ek.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mv.lnxyls.cn

[A07] 数字转字符串
来源：http://gr.jctech888.com.cn

Py:   str(42)
来源：http://bc.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://gb.asd995.cn

JS:   String(42); (42).toString()
来源：http://pr.szsharing.cn

TS:   String(42)
来源：http://pj.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ll.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://nj.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://fv.shtwfgs.cn

C#:   42.ToString()
来源：http://tz.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://ok.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kz.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fn.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fn.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ne.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://db.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ge.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vk.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yz.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://nc.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aw.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cu.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hx.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sp.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lz.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yq.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hu.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ei.colortex.cn

[A10] 生成随机数
来源：http://xt.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://bj.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://lq.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xh.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lf.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://hx.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oh.521024.cn

Ruby: rand(1..100)
来源：http://uz.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://zj.hahajie.cn

[A11] 条件表达式（三元）
来源：http://lt.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://gy.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mw.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yw.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xh.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://bk.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uf.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nh.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sp.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://wk.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rb.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ok.521024.cn

JS:   `Hello, ${name}!`
来源：http://rk.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://qc.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xk.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sv.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://yd.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://lk.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cd.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://gd.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://el.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://lt.asd995.cn

TS:   "第一行\n第二行"
来源：http://kk.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ti.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://ok.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://pc.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://kz.shxzukj.cn

[A14] 注释写法
来源：http://sw.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wp.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zq.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://js.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://mv.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://le.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://bx.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ay.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://ii.nicolike.cn

[A15] 空值判断与默认值
来源：http://vr.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://ly.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://gr.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://pz.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://gl.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lk.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://tl.nszjky.cn

Ruby: value = data || "默认值"
来源：http://cv.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://ye.haigaiapp.cn

[A16] 真假值判断规则
来源：http://pb.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://in.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gm.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lb.haigaiapp.cn

TS:   if (!x) {}
来源：http://sg.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qy.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vc.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nn.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tf.bjjhwx.cn

[A17] 位运算
来源：http://yl.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wc.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ki.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zd.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tp.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vs.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://li.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://fx.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://zd.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nt.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bv.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://tn.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xv.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://ro.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://dj.colortex.cn

[A19] 交换两个变量
来源：http://dv.jctech888.com.cn

Py:   a, b = b, a
来源：http://om.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sz.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://je.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://ye.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://lz.huixiangedu.cn

Go:   a, b = b, a
来源：http://zs.panjiajie.cn

Ruby: a, b = b, a
来源：http://qz.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://uz.yuexingan06.cn

[A20] 读取标准输入
来源：http://vq.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://xe.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://em.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dt.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ch.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://qo.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://er.gzmigu.cn

Ruby: gets.chomp
来源：http://vd.nszjky.cn

C#:   Console.ReadLine();
来源：http://rs.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://wm.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://dq.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pp.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ge.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://sj.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://rz.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zi.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://xn.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://ep.chemitech.net.cn

[A22] 获取字符串长度
来源：http://wd.521024.cn

Py:   len(s)
来源：http://wa.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://he.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mo.yuexingan06.cn

TS:   s.length
来源：http://lq.bjjhwx.cn

Java: s.length()
来源：http://ba.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zf.bookmarksfly.cn

Ruby: s.length
来源：http://hl.yuntaijiaju.cn

C#:   s.Length
来源：http://gn.nszjky.cn

[A23] 大小写转换
来源：http://fm.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jj.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nd.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gk.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xk.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xy.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://el.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pn.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://re.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://cl.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fj.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://on.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iz.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ho.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ss.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://qj.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oy.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://he.jianghongdianzi.cn

[A25] 字符串比较
来源：http://co.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://gl.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ej.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ux.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ed.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nt.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nv.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qh.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pa.haigaiapp.cn

[A26] 类型转换总览
来源：http://jo.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nz.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xs.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lj.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://fv.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pt.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vn.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bb.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qf.yuntaijiaju.cn

================================================================================
来源：http://gy.szxytkj.cn

B. 流程控制
来源：http://ly.9csxet.cn

================================================================================
来源：http://ui.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://kn.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rr.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ru.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sl.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://et.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tw.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hm.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://of.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fq.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://qy.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xq.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gk.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oj.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nu.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sh.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yr.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.huixiangedu.cn

[B03] switch / match / case
来源：http://fa.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pi.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://en.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nn.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mu.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ki.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ow.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fo.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mo.panjiajie.cn

[B04] for 计数循环
来源：http://cd.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://ay.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bh.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yh.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yl.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ck.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://hw.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nj.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://fx.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ek.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zs.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vm.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ul.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xt.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ar.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://ri.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aq.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://rf.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cf.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bw.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hg.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ms.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ua.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hv.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ks.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xg.lnxyls.cn

[B07] while 循环
来源：http://jm.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ay.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ip.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://vv.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://md.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://lg.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fz.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://oy.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ji.asd995.cn

[B08] do-while（至少执行一次）
来源：http://od.szsharing.cn


<!-- 参考信息 -->