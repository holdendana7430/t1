代发 wailian999

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gi.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aj.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gn.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dk.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xm.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yc.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bh.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uu.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mb.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dd.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zd.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uh.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pr.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ss.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://au.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fr.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zg.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bm.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gw.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pd.szxytkj.cn

================================================================================
来源：http://kk.szsharing.cn

A. 基础语法与类型
来源：http://cb.shxzukj.cn

================================================================================
来源：http://kw.bookmarksfly.cn

[A01] Hello World
来源：http://zg.panjiajie.cn

Py:   print("Hello, World!")
来源：http://fw.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://ug.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://zl.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zn.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://ym.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://vb.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://zt.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://la.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://zb.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dv.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://br.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fd.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yo.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://ea.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://jb.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://pq.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://br.bjjhwx.cn

[A03] 常量定义
来源：http://vy.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kj.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://zb.asd995.cn

JS:   const PI = 3.14159;
来源：http://tx.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://qw.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://lj.nicolike.cn

Go:   const PI = 3.14159
来源：http://ml.hahajie.cn

Ruby: PI = 3.14159
来源：http://vp.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://kc.lnxyls.cn

[A04] 判断变量类型
来源：http://tb.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dg.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vs.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vr.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ni.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ta.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nu.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ap.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://wg.huanxung.cn

[A05] 整数除法与取模
来源：http://ng.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cz.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uk.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ea.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://av.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://rj.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://fc.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://py.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://rz.shtwfgs.cn

[A06] 字符串转数字
来源：http://is.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://go.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gd.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jx.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xc.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gg.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fb.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gb.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kh.wgjwhj.cn

[A07] 数字转字符串
来源：http://ya.bjjhwx.cn

Py:   str(42)
来源：http://zi.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://gl.hahajie.cn

JS:   String(42); (42).toString()
来源：http://yu.szsharing.cn

TS:   String(42)
来源：http://yr.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ha.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://wk.jctech888.com.cn

Ruby: 42.to_s
来源：http://wn.nszjky.cn

C#:   42.ToString()
来源：http://hs.521024.cn

[A08] 取整与四舍五入
来源：http://mv.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aj.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jz.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ps.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ed.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kq.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xp.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ba.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wu.521024.cn

[A09] 绝对值与最大最小值
来源：http://cf.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qi.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rc.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://no.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kh.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uj.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tg.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bj.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kk.huanxung.cn

[A10] 生成随机数
来源：http://qf.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://eq.9csxet.cn

PHP:  random_int(1, 100);
来源：http://md.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jx.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cq.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://nj.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bj.9csxet.cn

Ruby: rand(1..100)
来源：http://jb.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://ph.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://ar.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ad.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sm.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wh.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xo.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ye.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gi.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rw.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fo.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://aw.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kv.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yq.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://df.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://di.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://qm.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nq.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://rh.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://st.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jj.newstarts.cn

Py:   "第一行\n第二行"
来源：http://du.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://mg.szsharing.cn

JS:   "第一行\n第二行"
来源：http://em.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://xt.szxytkj.cn

Java: "第一行\n第二行"
来源：http://nd.szsharing.cn

Go:   "第一行\n第二行"
来源：http://ac.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://gv.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://wq.chemitech.net.cn

[A14] 注释写法
来源：http://ab.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ne.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ny.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://ig.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://fr.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ce.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://wt.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lb.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://cg.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://fs.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://kr.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ro.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://gi.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://uz.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fq.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://ee.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://dy.nicolike.cn

[A16] 真假值判断规则
来源：http://si.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pz.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hi.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fq.szsharing.cn

TS:   if (!x) {}
来源：http://kz.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dd.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vi.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jv.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://no.panjiajie.cn

[A17] 位运算
来源：http://ko.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qd.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cr.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bv.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jb.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://wn.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://pg.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://jx.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fa.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gm.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://ks.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qa.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://qa.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://ez.szxytkj.cn

[A19] 交换两个变量
来源：http://wh.newstarts.cn

Py:   a, b = b, a
来源：http://dx.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fn.521024.cn

JS:   [a, b] = [b, a];
来源：http://rz.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://ix.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://op.panjiajie.cn

Go:   a, b = b, a
来源：http://ut.nicolike.cn

Ruby: a, b = b, a
来源：http://mo.521024.cn

C#:   (a, b) = (b, a);
来源：http://wc.nszjky.cn

[A20] 读取标准输入
来源：http://lw.panjiajie.cn

Py:   name = input("请输入：")
来源：http://cb.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tc.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nt.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://jw.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://tk.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ua.shxzukj.cn

Ruby: gets.chomp
来源：http://nh.newstarts.cn

C#:   Console.ReadLine();
来源：http://kg.colortex.cn

[A21] 保留指定小数位输出
来源：http://sj.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://ih.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xi.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://jc.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://dt.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://ey.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uh.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://uq.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://oz.asd995.cn

[A22] 获取字符串长度
来源：http://op.huixinmuqiang.cn

Py:   len(s)
来源：http://ir.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sp.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ms.haigaiapp.cn

TS:   s.length
来源：http://eb.521024.cn

Java: s.length()
来源：http://io.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eb.newstarts.cn

Ruby: s.length
来源：http://bi.newstarts.cn

C#:   s.Length
来源：http://vq.9csxet.cn

[A23] 大小写转换
来源：http://hi.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sp.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rf.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cp.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nm.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yk.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dv.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wn.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bn.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://gc.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xx.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hu.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dz.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://il.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oj.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://ht.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bf.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://to.huanxung.cn

[A25] 字符串比较
来源：http://le.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://ib.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hh.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ff.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sd.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pg.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://to.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mh.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gb.wgjwhj.cn

[A26] 类型转换总览
来源：http://nq.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ds.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iz.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bw.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://ax.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gq.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gh.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zu.szxytkj.cn

================================================================================
来源：http://lc.newstarts.cn

B. 流程控制
来源：http://zr.shtwfgs.cn

================================================================================
来源：http://nk.asd995.cn

[B01] 条件判断 if / else
来源：http://vs.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hd.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qd.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fa.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zl.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wh.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pu.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ph.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://rt.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jj.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bg.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ya.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dj.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gc.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qm.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xm.chemitech.net.cn

[B03] switch / match / case
来源：http://xi.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hd.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fs.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ql.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hi.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xe.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jl.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mk.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://je.wgjwhj.cn

[B04] for 计数循环
来源：http://wi.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://ni.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vi.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://za.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xy.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lp.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rl.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://en.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gm.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://lt.9csxet.cn

Py:   for item in arr: print(item)
来源：http://yb.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uj.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ki.hnjuh.cn


<!-- 参考信息 -->