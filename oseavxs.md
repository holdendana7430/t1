代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://lp.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://pi.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://eg.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fa.newstarts.cn

[A02] 变量声明与赋值
来源：http://ll.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ni.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tc.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qg.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ck.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://sp.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://bs.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://mp.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ov.yuexingan06.cn

[A03] 常量定义
来源：http://ky.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gj.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://qk.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://ed.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://kz.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://nu.nszjky.cn

Go:   const PI = 3.14159
来源：http://by.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://an.asd995.cn

C#:   const double PI = 3.14159;
来源：http://co.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://zd.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xz.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xd.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yh.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://yh.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sy.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dz.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fj.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://qf.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://kn.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ir.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wd.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gz.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sc.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://oe.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://cw.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qr.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://co.nszjky.cn

[A06] 字符串转数字
来源：http://kp.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://nf.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pe.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ca.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vu.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oc.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tb.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vo.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tu.shtwfgs.cn

[A07] 数字转字符串
来源：http://ru.shtwfgs.cn

Py:   str(42)
来源：http://sd.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://fj.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://cm.newstarts.cn

TS:   String(42)
来源：http://xo.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aw.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ui.asd995.cn

Ruby: 42.to_s
来源：http://xz.huanxung.cn

C#:   42.ToString()
来源：http://tp.panjiajie.cn

[A08] 取整与四舍五入
来源：http://na.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ku.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://at.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://re.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ma.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sw.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jg.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ru.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lc.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://dy.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oo.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xr.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://em.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ay.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xl.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fx.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ek.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bf.bookmarksfly.cn

[A10] 生成随机数
来源：http://fm.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://qy.colortex.cn

PHP:  random_int(1, 100);
来源：http://et.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lt.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hh.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://id.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ca.wgjwhj.cn

Ruby: rand(1..100)
来源：http://gr.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://rw.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://yr.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://la.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ju.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xd.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ox.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ff.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qt.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://an.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rc.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://af.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wy.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rj.521024.cn

JS:   `Hello, ${name}!`
来源：http://tg.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ty.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://rm.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rk.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://mm.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://mh.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ah.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://de.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://pp.newstarts.cn

JS:   "第一行\n第二行"
来源：http://sd.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://kb.nszjky.cn

Java: "第一行\n第二行"
来源：http://tt.asd995.cn

Go:   "第一行\n第二行"
来源：http://hq.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://nt.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://ip.chemitech.net.cn

[A14] 注释写法
来源：http://dd.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qm.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://md.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://dk.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://zb.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mx.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://bg.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://er.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://fo.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://bq.asd995.cn

Py:   value = data or "默认值"
来源：http://lf.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://jf.521024.cn

JS:   const value = data ?? "默认值";
来源：http://zj.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://sj.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gt.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://zq.asd995.cn

Ruby: value = data || "默认值"
来源：http://kk.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://tu.chemitech.net.cn

[A16] 真假值判断规则
来源：http://dp.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qx.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dr.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sl.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://xi.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dq.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://of.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ou.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qw.yuexingan06.cn

[A17] 位运算
来源：http://aq.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://da.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pg.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ua.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cb.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cs.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://ls.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://vg.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://ul.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yl.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qc.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ru.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pe.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://au.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://ly.shxzukj.cn

[A19] 交换两个变量
来源：http://bo.huixiangedu.cn

Py:   a, b = b, a
来源：http://km.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://am.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://vx.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://vd.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ca.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://ik.shxzukj.cn

Ruby: a, b = b, a
来源：http://fy.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://ew.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://tv.huanxung.cn

Py:   name = input("请输入：")
来源：http://um.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rf.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oc.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ub.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://qp.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ar.nszjky.cn

Ruby: gets.chomp
来源：http://fy.asd995.cn

C#:   Console.ReadLine();
来源：http://gc.newstarts.cn

[A21] 保留指定小数位输出
来源：http://tx.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://kf.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cc.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://vd.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://ez.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://fi.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://go.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://rm.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://pz.gzmigu.cn

[A22] 获取字符串长度
来源：http://df.panjiajie.cn

Py:   len(s)
来源：http://te.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dg.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://er.gzmigu.cn

TS:   s.length
来源：http://yq.szxytkj.cn

Java: s.length()
来源：http://cw.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://se.nszjky.cn

Ruby: s.length
来源：http://xz.jianghongdianzi.cn

C#:   s.Length
来源：http://kn.lnxyls.cn

[A23] 大小写转换
来源：http://nj.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oc.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ur.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://re.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vz.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xj.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cw.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://le.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fy.gzmigu.cn

[A24] 去除首尾空白
来源：http://yd.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gy.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://st.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lw.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ka.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ak.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://vg.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ri.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jf.shxzskj.cn

[A25] 字符串比较
来源：http://nq.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://fj.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mh.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wq.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qg.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nu.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tm.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hx.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ke.haigaiapp.cn

[A26] 类型转换总览
来源：http://rn.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qj.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://er.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tb.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://wj.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uf.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xu.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://np.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vi.shtwfgs.cn

================================================================================
来源：http://jp.huixiangedu.cn

B. 流程控制
来源：http://pi.muxihuayi.cn

================================================================================
来源：http://cu.asd995.cn

[B01] 条件判断 if / else
来源：http://uq.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pu.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://te.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tw.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wm.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xd.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yt.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hr.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gk.newstarts.cn

[B02] 多分支 else if / elif
来源：http://yr.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ww.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://re.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qj.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sb.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nv.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ym.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lo.nszjky.cn

[B03] switch / match / case
来源：http://mk.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ld.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fd.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rd.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tw.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kn.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oh.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sv.huixiangedu.cn

[B04] for 计数循环
来源：http://lu.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://tg.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vo.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://th.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fm.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://co.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nf.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://bb.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nf.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://pg.huanxung.cn

Py:   for item in arr: print(item)
来源：http://vj.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bt.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yp.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xd.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pn.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tj.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ps.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ep.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://up.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sn.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tf.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zc.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yb.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cd.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ws.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pl.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ef.hahajie.cn

[B07] while 循环
来源：http://eu.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://kj.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qd.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://ms.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://pn.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://pw.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wl.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://jk.521024.cn

C#:   while (i < 10) { i++; }
来源：http://oc.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://ni.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://jl.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mb.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://nv.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://bp.yuexingan06.cn


<!-- 参考信息 -->