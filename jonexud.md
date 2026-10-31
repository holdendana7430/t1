代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pn.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mq.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://re.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oz.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ce.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ba.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pe.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jj.hnjuh.cn

================================================================================
来源：http://kc.huixinmuqiang.cn

A. 基础语法与类型
来源：http://rv.yuntaijiaju.cn

================================================================================
来源：http://wa.gzmigu.cn

[A01] Hello World
来源：http://ct.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://wj.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://wc.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://va.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ue.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://mi.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://zp.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://jj.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jo.colortex.cn

[A02] 变量声明与赋值
来源：http://ly.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wz.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://au.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ao.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lp.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://za.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://ys.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://xc.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ew.panjiajie.cn

[A03] 常量定义
来源：http://ye.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tg.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://th.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://bx.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://fv.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://zw.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://zj.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://xz.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://ss.nicolike.cn

[A04] 判断变量类型
来源：http://gy.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ql.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ph.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bj.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://ol.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rj.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rt.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ph.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://tt.muxihuayi.cn

[A05] 整数除法与取模
来源：http://xh.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xs.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://au.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jk.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cv.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://oa.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://sa.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://cq.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://yw.wgjwhj.cn

[A06] 字符串转数字
来源：http://ot.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://bi.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tv.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mt.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pe.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wn.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://co.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iv.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qi.shtwfgs.cn

[A07] 数字转字符串
来源：http://vp.newstarts.cn

Py:   str(42)
来源：http://cj.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://tr.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://dr.jianghongdianzi.cn

TS:   String(42)
来源：http://ql.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ug.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://wl.9csxet.cn

Ruby: 42.to_s
来源：http://iw.shxzskj.cn

C#:   42.ToString()
来源：http://hi.lnxyls.cn

[A08] 取整与四舍五入
来源：http://uk.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ek.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vc.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wr.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oh.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qk.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jm.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hp.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yn.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ju.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vo.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gx.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lu.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ab.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lk.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lt.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vv.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eq.nicolike.cn

[A10] 生成随机数
来源：http://gm.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://rt.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://kf.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rw.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zv.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://wj.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ig.colortex.cn

Ruby: rand(1..100)
来源：http://mx.521024.cn

C#:   new Random().Next(1, 101)
来源：http://lk.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://yi.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://kk.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://um.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://in.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uy.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://gs.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xj.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yf.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aw.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://ut.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ni.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zr.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://dw.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://zx.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://bc.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rv.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://vm.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://wo.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://at.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://kr.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://fa.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://xx.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://am.9csxet.cn

Java: "第一行\n第二行"
来源：http://po.nicolike.cn

Go:   "第一行\n第二行"
来源：http://at.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://ry.hahajie.cn

C#:   "第一行\n第二行"
来源：http://sr.jianghongdianzi.cn

[A14] 注释写法
来源：http://pz.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vy.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wt.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://jn.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://qs.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bh.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://yn.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xr.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://wu.shxzukj.cn

[A15] 空值判断与默认值
来源：http://oy.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://iu.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://uj.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://dq.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://mh.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mk.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://bb.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://rj.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://jn.shxzukj.cn

[A16] 真假值判断规则
来源：http://cr.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qw.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fz.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ts.wgjwhj.cn

TS:   if (!x) {}
来源：http://cz.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kx.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tf.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tz.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://om.nszjky.cn

[A17] 位运算
来源：http://sr.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tt.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hs.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kg.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nt.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mr.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://my.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://do.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://qw.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://rb.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://jv.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xk.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vt.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://gd.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://by.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://he.asd995.cn

C#:   (int)'A'; (char)65
来源：http://dc.shxzskj.cn

[A19] 交换两个变量
来源：http://nq.chemitech.net.cn

Py:   a, b = b, a
来源：http://zl.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://um.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://mb.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://qq.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://pj.yuexingan06.cn

Go:   a, b = b, a
来源：http://yq.shtwfgs.cn

Ruby: a, b = b, a
来源：http://rz.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://xh.haigaiapp.cn

[A20] 读取标准输入
来源：http://vg.nszjky.cn

Py:   name = input("请输入：")
来源：http://os.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://my.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sy.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ro.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://xi.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gf.521024.cn

Ruby: gets.chomp
来源：http://oj.nszjky.cn

C#:   Console.ReadLine();
来源：http://ok.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://jg.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://na.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wt.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://sz.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://uu.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://rc.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rk.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://mx.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://jg.newstarts.cn

[A22] 获取字符串长度
来源：http://qt.yuntaijiaju.cn

Py:   len(s)
来源：http://vw.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zx.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qp.newstarts.cn

TS:   s.length
来源：http://zd.huixinmuqiang.cn

Java: s.length()
来源：http://qj.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vn.szxytkj.cn

Ruby: s.length
来源：http://mu.muxihuayi.cn

C#:   s.Length
来源：http://er.jianghongdianzi.cn

[A23] 大小写转换
来源：http://ef.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zz.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wq.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xs.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kv.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gv.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nk.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gc.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gl.lnxyls.cn

[A24] 去除首尾空白
来源：http://cg.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tb.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lm.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mo.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://br.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://sl.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cg.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ow.yuntaijiaju.cn

[A25] 字符串比较
来源：http://pw.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://nv.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zk.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pr.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hx.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ak.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://se.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lf.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uk.szsharing.cn

[A26] 类型转换总览
来源：http://kx.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lp.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gj.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bl.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://ac.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rd.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jw.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://en.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ly.panjiajie.cn

================================================================================
来源：http://hn.shtwfgs.cn

B. 流程控制
来源：http://ub.9csxet.cn

================================================================================
来源：http://hi.lnxyls.cn

[B01] 条件判断 if / else
来源：http://gd.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://em.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xa.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oh.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rp.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lo.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cf.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tx.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://oy.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gt.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://da.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://co.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ek.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.hahajie.cn

[B03] switch / match / case
来源：http://fh.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eb.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xc.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nv.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kg.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tm.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ct.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ch.muxihuayi.cn

[B04] for 计数循环
来源：http://rn.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://mg.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wx.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wa.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sr.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hm.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://aw.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fa.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://wg.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://hs.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yj.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rx.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tf.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rk.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xn.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://pf.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nh.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ss.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bq.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ij.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vj.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ts.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://la.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cz.asd995.cn


<!-- 参考信息 -->