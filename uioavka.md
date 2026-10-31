代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xr.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xq.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oh.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://im.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nn.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lh.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://if.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ex.huixiangedu.cn

================================================================================
来源：http://ll.521024.cn

A. 基础语法与类型
来源：http://kb.shtwfgs.cn

================================================================================
来源：http://wb.haigaiapp.cn

[A01] Hello World
来源：http://vj.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://my.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://dr.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ka.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ey.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://yq.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://iq.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://yx.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://db.521024.cn

[A02] 变量声明与赋值
来源：http://ac.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eu.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dh.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hr.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gx.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://zo.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://js.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://kh.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oi.lnxyls.cn

[A03] 常量定义
来源：http://cp.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://no.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://uf.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://am.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://ik.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://pw.shxzskj.cn

Go:   const PI = 3.14159
来源：http://ku.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://em.colortex.cn

C#:   const double PI = 3.14159;
来源：http://hv.yuexingan06.cn

[A04] 判断变量类型
来源：http://yp.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ga.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gn.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cg.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://db.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xh.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xw.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xr.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ni.wgjwhj.cn

[A05] 整数除法与取模
来源：http://ce.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ss.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lm.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ez.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vr.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://rn.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://zo.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://ch.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://ef.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://oy.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://ak.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tw.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ps.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rh.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xg.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fk.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ey.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ul.nszjky.cn

[A07] 数字转字符串
来源：http://lb.bookmarksfly.cn

Py:   str(42)
来源：http://vd.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://ie.nszjky.cn

JS:   String(42); (42).toString()
来源：http://da.szxytkj.cn

TS:   String(42)
来源：http://mq.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gk.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ug.jctech888.com.cn

Ruby: 42.to_s
来源：http://rw.hnjuh.cn

C#:   42.ToString()
来源：http://ov.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://yq.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hx.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vu.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bs.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ao.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://to.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pl.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fr.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xd.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://gl.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dh.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ul.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ig.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ad.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lk.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rx.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zv.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jk.jctech888.com.cn

[A10] 生成随机数
来源：http://vm.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://np.newstarts.cn

PHP:  random_int(1, 100);
来源：http://kx.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vr.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rk.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ne.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ep.hahajie.cn

Ruby: rand(1..100)
来源：http://kl.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://ym.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://eg.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://fs.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nr.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://of.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pb.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://er.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nb.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tg.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nd.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://tg.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qv.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://io.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://rf.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://iq.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://yx.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sb.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://bs.asd995.cn

C#:   $"Hello, {name}!"
来源：http://rz.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://np.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://ry.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://ty.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://ho.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://zo.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://xl.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ky.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://qz.asd995.cn

C#:   "第一行\n第二行"
来源：http://te.newstarts.cn

[A14] 注释写法
来源：http://lj.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wk.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ft.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://cz.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://lw.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jn.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://rw.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rf.521024.cn

C#:   // 单行；/* 多行 */
来源：http://gl.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://kp.gzmigu.cn

Py:   value = data or "默认值"
来源：http://he.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://eo.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://uo.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://ew.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ry.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://og.nszjky.cn

Ruby: value = data || "默认值"
来源：http://wn.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://mw.shxzskj.cn

[A16] 真假值判断规则
来源：http://de.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zr.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gx.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jp.hnjuh.cn

TS:   if (!x) {}
来源：http://mp.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ar.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tx.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ze.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xa.hnjuh.cn

[A17] 位运算
来源：http://bb.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://of.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fo.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cc.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ip.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://ez.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://av.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://pc.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rd.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jz.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://he.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jm.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://wi.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://ab.haigaiapp.cn

[A19] 交换两个变量
来源：http://tz.chemitech.net.cn

Py:   a, b = b, a
来源：http://oh.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wy.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://pv.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://dl.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://cz.panjiajie.cn

Go:   a, b = b, a
来源：http://xe.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://rx.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://zc.hahajie.cn

[A20] 读取标准输入
来源：http://nt.hahajie.cn

Py:   name = input("请输入：")
来源：http://bu.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ft.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ty.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://im.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://we.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ge.colortex.cn

Ruby: gets.chomp
来源：http://ek.hahajie.cn

C#:   Console.ReadLine();
来源：http://yy.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://bj.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://rp.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ox.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://cn.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://bc.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://sq.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cq.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://sz.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ml.newstarts.cn

[A22] 获取字符串长度
来源：http://pj.nicolike.cn

Py:   len(s)
来源：http://oz.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rd.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wp.9csxet.cn

TS:   s.length
来源：http://ey.wgjwhj.cn

Java: s.length()
来源：http://ay.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sf.shxzukj.cn

Ruby: s.length
来源：http://ae.huixinmuqiang.cn

C#:   s.Length
来源：http://ic.jctech888.com.cn

[A23] 大小写转换
来源：http://bb.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wj.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hf.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rd.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hh.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bj.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oo.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vk.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yk.hnjuh.cn

[A24] 去除首尾空白
来源：http://ri.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ge.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cn.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ft.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gu.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hj.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://mq.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xz.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sj.szxytkj.cn

[A25] 字符串比较
来源：http://yt.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://lj.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yw.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tm.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jd.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://om.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dh.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ba.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pa.szxytkj.cn

[A26] 类型转换总览
来源：http://mf.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ya.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iv.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cb.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://jd.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sa.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wl.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bq.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wd.szxytkj.cn

================================================================================
来源：http://xc.hahajie.cn

B. 流程控制
来源：http://uk.nszjky.cn

================================================================================
来源：http://zf.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://tk.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lp.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://em.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mu.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pi.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fk.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pr.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://at.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tn.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://iv.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://to.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jg.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://od.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://df.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.muxihuayi.cn

[B03] switch / match / case
来源：http://nv.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oz.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ku.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tp.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ce.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fb.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qj.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fe.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bz.nszjky.cn

[B04] for 计数循环
来源：http://hf.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://bb.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://al.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kh.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://db.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nt.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cy.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://vo.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wp.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://li.colortex.cn

Py:   for item in arr: print(item)
来源：http://gg.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rl.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ud.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dj.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ae.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://en.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ys.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://up.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://zj.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gj.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ge.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dx.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dd.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jx.colortex.cn


<!-- 参考信息 -->