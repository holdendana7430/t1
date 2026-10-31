代发 wailian999

--------------------------------------------------------------------------------
来源：http://za.wgjwhj.cn

目  录
来源：http://fk.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://il.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ml.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lw.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cc.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pd.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://js.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zv.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ki.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gs.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bb.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zj.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mr.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rf.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hs.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dm.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uk.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ji.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mn.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ml.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ox.yuexingan06.cn

================================================================================
来源：http://sh.huanxung.cn

A. 基础语法与类型
来源：http://zq.bookmarksfly.cn

================================================================================
来源：http://kt.yuntaijiaju.cn

[A01] Hello World
来源：http://qw.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://jf.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://jw.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://wz.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://un.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://cr.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://zz.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://vk.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xh.asd995.cn

[A02] 变量声明与赋值
来源：http://im.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cg.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ak.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uz.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ge.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://hc.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://df.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://zw.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jj.shxzukj.cn

[A03] 常量定义
来源：http://ml.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fu.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://uq.hahajie.cn

JS:   const PI = 3.14159;
来源：http://bt.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://ps.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://or.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://ue.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://mf.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://re.shtwfgs.cn

[A04] 判断变量类型
来源：http://ah.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nk.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oo.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vq.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://yk.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hx.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mi.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cj.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://pk.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://nj.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pw.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wc.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ch.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pc.521024.cn

Java: 7 / 2; 7 % 2
来源：http://de.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://og.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://ee.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://iv.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://wu.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://sf.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kc.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ju.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kg.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yh.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tj.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ct.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vy.wgjwhj.cn

[A07] 数字转字符串
来源：http://ly.colortex.cn

Py:   str(42)
来源：http://gh.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://jz.colortex.cn

JS:   String(42); (42).toString()
来源：http://jn.muxihuayi.cn

TS:   String(42)
来源：http://ya.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://py.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ms.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://ce.lnxyls.cn

C#:   42.ToString()
来源：http://hf.shxzskj.cn

[A08] 取整与四舍五入
来源：http://cn.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rr.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dk.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gn.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dn.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xn.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://et.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://io.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pn.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ni.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zu.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sb.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yv.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fz.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://us.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kh.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gx.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vm.asd995.cn

[A10] 生成随机数
来源：http://ld.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://ec.newstarts.cn

PHP:  random_int(1, 100);
来源：http://qr.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ni.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wk.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://fk.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dp.panjiajie.cn

Ruby: rand(1..100)
来源：http://bw.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://sx.9csxet.cn

[A11] 条件表达式（三元）
来源：http://qi.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://oz.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://as.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hw.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vz.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://oi.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vd.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://my.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ut.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://yo.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ft.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bd.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://nl.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://dr.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://mt.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ei.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://mx.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://ox.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uh.newstarts.cn

Py:   "第一行\n第二行"
来源：http://lv.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://fr.9csxet.cn

JS:   "第一行\n第二行"
来源：http://lh.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://is.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://gk.szsharing.cn

Go:   "第一行\n第二行"
来源：http://wl.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://uq.newstarts.cn

C#:   "第一行\n第二行"
来源：http://eg.newstarts.cn

[A14] 注释写法
来源：http://sl.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oo.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zp.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://kk.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://xz.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://on.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://wm.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://us.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://kl.huanxung.cn

[A15] 空值判断与默认值
来源：http://ef.lnxyls.cn

Py:   value = data or "默认值"
来源：http://iq.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://hq.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://pq.521024.cn

TS:   const value = data ?? "默认值";
来源：http://yq.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://br.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://sc.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://vv.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://zg.huanxung.cn

[A16] 真假值判断规则
来源：http://zj.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hy.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://af.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oe.gzmigu.cn

TS:   if (!x) {}
来源：http://mt.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://za.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jj.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mi.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sf.bjjhwx.cn

[A17] 位运算
来源：http://iy.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yb.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jy.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qp.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://de.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lr.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wf.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://ea.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://ya.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://yc.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cs.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ps.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://rr.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lc.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://nm.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://td.asd995.cn

[A19] 交换两个变量
来源：http://gg.asd995.cn

Py:   a, b = b, a
来源：http://ic.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bg.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://lb.521024.cn

TS:   [a, b] = [b, a];
来源：http://tp.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://nv.bjjhwx.cn

Go:   a, b = b, a
来源：http://zy.hahajie.cn

Ruby: a, b = b, a
来源：http://ce.asd995.cn

C#:   (a, b) = (b, a);
来源：http://th.bookmarksfly.cn

[A20] 读取标准输入
来源：http://sz.521024.cn

Py:   name = input("请输入：")
来源：http://gl.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zr.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ig.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://sg.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://aq.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pr.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://rg.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ju.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://oo.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://wh.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://at.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://ax.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://nz.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://ti.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mb.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://bs.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://zi.bjjhwx.cn

[A22] 获取字符串长度
来源：http://ff.chemitech.net.cn

Py:   len(s)
来源：http://tp.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yd.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tt.wgjwhj.cn

TS:   s.length
来源：http://gv.huixinmuqiang.cn

Java: s.length()
来源：http://rr.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ka.panjiajie.cn

Ruby: s.length
来源：http://ze.asd995.cn

C#:   s.Length
来源：http://dt.newstarts.cn

[A23] 大小写转换
来源：http://wr.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nz.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ms.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ud.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vm.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xx.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://em.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dg.hahajie.cn

[A24] 去除首尾空白
来源：http://zf.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pl.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ch.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ky.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wd.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://uj.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fv.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gc.hnjuh.cn

[A25] 字符串比较
来源：http://ns.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://cb.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tg.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ay.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xw.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ac.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hi.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fo.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vs.yuexingan06.cn

[A26] 类型转换总览
来源：http://ee.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hh.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tn.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aa.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://hp.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://se.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zq.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bd.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bh.panjiajie.cn

================================================================================
来源：http://ue.jianghongdianzi.cn

B. 流程控制
来源：http://fw.colortex.cn

================================================================================
来源：http://fo.huanxung.cn

[B01] 条件判断 if / else
来源：http://rn.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pp.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://br.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pu.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dn.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ez.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ae.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ue.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qj.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://rv.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zr.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xt.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ky.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xf.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.shtwfgs.cn

[B03] switch / match / case
来源：http://zw.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sh.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nc.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mg.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lj.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ta.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lb.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qf.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jz.yuntaijiaju.cn

[B04] for 计数循环
来源：http://jx.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://tz.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ja.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ix.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wa.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zv.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://um.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://ga.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wp.yuexingan06.cn


<!-- 参考信息 -->