代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://os.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kd.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bh.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rs.hnjuh.cn

================================================================================
来源：http://ps.gzmigu.cn

A. 基础语法与类型
来源：http://yz.521024.cn

================================================================================
来源：http://as.colortex.cn

[A01] Hello World
来源：http://ei.nicolike.cn

Py:   print("Hello, World!")
来源：http://oc.521024.cn

PHP:  echo "Hello, World!";
来源：http://ep.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://iv.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mc.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://tc.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://vx.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://ex.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dl.521024.cn

[A02] 变量声明与赋值
来源：http://fp.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hb.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oa.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xe.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ip.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://yn.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://iz.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://ay.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://np.huixiangedu.cn

[A03] 常量定义
来源：http://oo.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dv.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://iv.521024.cn

JS:   const PI = 3.14159;
来源：http://bf.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://uo.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://cn.colortex.cn

Go:   const PI = 3.14159
来源：http://rc.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://nd.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://pv.gzmigu.cn

[A04] 判断变量类型
来源：http://ib.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xh.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yy.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oh.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://yg.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pq.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fq.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ju.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://re.muxihuayi.cn

[A05] 整数除法与取模
来源：http://hx.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yt.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://om.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ba.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ls.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://sa.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://fo.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://na.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://es.yuexingan06.cn

[A06] 字符串转数字
来源：http://rb.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://jy.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qw.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ti.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wc.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gu.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zf.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eb.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bg.gzmigu.cn

[A07] 数字转字符串
来源：http://sk.asd995.cn

Py:   str(42)
来源：http://un.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://zq.nicolike.cn

JS:   String(42); (42).toString()
来源：http://jx.9csxet.cn

TS:   String(42)
来源：http://ut.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ui.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://oj.521024.cn

Ruby: 42.to_s
来源：http://dx.jianghongdianzi.cn

C#:   42.ToString()
来源：http://uz.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://iz.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mn.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hg.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qn.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://es.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mu.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fq.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zm.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vd.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ly.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jh.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://au.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eb.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cz.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://my.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qe.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gs.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fn.9csxet.cn

[A10] 生成随机数
来源：http://mg.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://ks.colortex.cn

PHP:  random_int(1, 100);
来源：http://xe.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yt.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mt.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://sx.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ry.szxytkj.cn

Ruby: rand(1..100)
来源：http://ke.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://tm.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://cj.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://rf.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mq.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ky.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sc.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://eg.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fw.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ka.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ok.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://aq.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kz.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://up.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://bw.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://pg.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://bn.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://er.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ta.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://qv.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wu.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://zb.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://mg.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://xl.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://dn.521024.cn

Java: "第一行\n第二行"
来源：http://wq.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://ik.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://uf.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://lm.9csxet.cn

[A14] 注释写法
来源：http://cm.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ng.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://is.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://ua.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://rp.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ca.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://ud.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ut.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://ui.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://ky.szxytkj.cn

Py:   value = data or "默认值"
来源：http://dn.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://hh.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://nu.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://sy.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ku.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fr.nicolike.cn

Ruby: value = data || "默认值"
来源：http://by.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://tq.yuexingan06.cn

[A16] 真假值判断规则
来源：http://aq.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://de.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lw.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uo.bookmarksfly.cn

TS:   if (!x) {}
来源：http://ea.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ux.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kq.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://le.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wu.nicolike.cn

[A17] 位运算
来源：http://is.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ic.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pz.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hl.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bt.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sb.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://pg.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://fb.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://ta.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ee.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ky.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://os.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tq.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://wi.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://sd.panjiajie.cn

[A19] 交换两个变量
来源：http://qn.newstarts.cn

Py:   a, b = b, a
来源：http://gu.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ow.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://iq.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://oz.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://mf.nszjky.cn

Go:   a, b = b, a
来源：http://tm.szxytkj.cn

Ruby: a, b = b, a
来源：http://lo.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://wf.shxzskj.cn

[A20] 读取标准输入
来源：http://yh.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://jq.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://as.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://em.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://yg.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://zu.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lz.szsharing.cn

Ruby: gets.chomp
来源：http://ql.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://cn.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://hx.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://tc.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ol.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://ff.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ny.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://qn.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wk.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://gu.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://cs.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://gk.shtwfgs.cn

Py:   len(s)
来源：http://nc.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xo.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kk.shxzskj.cn

TS:   s.length
来源：http://cd.huixinmuqiang.cn

Java: s.length()
来源：http://ex.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ms.wgjwhj.cn

Ruby: s.length
来源：http://rj.wgjwhj.cn

C#:   s.Length
来源：http://jy.9csxet.cn

[A23] 大小写转换
来源：http://mz.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ax.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lx.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://la.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oo.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ad.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://si.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fg.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fs.huixiangedu.cn

[A24] 去除首尾空白
来源：http://wd.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bo.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aw.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bu.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kf.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gl.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://zm.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://td.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ru.hnjuh.cn

[A25] 字符串比较
来源：http://jq.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://jg.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ub.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mp.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zs.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ee.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yv.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hx.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uc.jctech888.com.cn

[A26] 类型转换总览
来源：http://ub.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://py.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ef.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yp.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://nw.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qx.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ri.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://un.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fz.9csxet.cn

================================================================================
来源：http://yz.haigaiapp.cn

B. 流程控制
来源：http://ow.haigaiapp.cn

================================================================================
来源：http://fi.szxytkj.cn

[B01] 条件判断 if / else
来源：http://aw.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ha.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lg.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://np.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ev.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://po.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wh.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yc.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rs.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://nk.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fo.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rr.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pm.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rh.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ac.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uj.yuexingan06.cn

[B03] switch / match / case
来源：http://nz.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ec.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://to.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wi.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eo.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fn.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ug.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dy.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uz.asd995.cn

[B04] for 计数循环
来源：http://wo.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://fc.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ts.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zk.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nq.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ft.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rv.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://gi.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zy.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://xy.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ux.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uy.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wh.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tc.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fs.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wc.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://mi.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tp.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://dp.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wh.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rm.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://da.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bb.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wh.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cc.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ob.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bi.bookmarksfly.cn

[B07] while 循环
来源：http://bo.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://rz.szsharing.cn


<!-- 参考信息 -->