代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pb.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cy.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tx.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xq.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://su.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ap.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jl.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qh.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kk.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yz.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mf.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lk.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ty.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nt.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gx.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wj.9csxet.cn

================================================================================
来源：http://jx.shxzskj.cn

A. 基础语法与类型
来源：http://sa.lnxyls.cn

================================================================================
来源：http://hp.shxzukj.cn

[A01] Hello World
来源：http://bn.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://bs.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://xe.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://nx.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jt.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://mt.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ot.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://by.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oq.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://cu.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rt.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kp.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jl.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oo.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://cs.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://vi.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://yu.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ba.jianghongdianzi.cn

[A03] 常量定义
来源：http://lq.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ge.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://we.hahajie.cn

JS:   const PI = 3.14159;
来源：http://nv.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://wn.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://pn.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://vu.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://kk.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://tp.bookmarksfly.cn

[A04] 判断变量类型
来源：http://ir.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ue.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vh.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mc.521024.cn

TS:   typeof x; x instanceof Date
来源：http://md.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nc.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ja.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gu.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://vv.9csxet.cn

[A05] 整数除法与取模
来源：http://ti.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uy.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fc.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wa.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gr.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://nr.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://bh.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://dn.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://uk.szsharing.cn

[A06] 字符串转数字
来源：http://xa.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://ok.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qe.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zp.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mf.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hh.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ek.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kg.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wg.asd995.cn

[A07] 数字转字符串
来源：http://ll.jctech888.com.cn

Py:   str(42)
来源：http://rg.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://zv.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://bt.hahajie.cn

TS:   String(42)
来源：http://nk.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jl.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://er.bjjhwx.cn

Ruby: 42.to_s
来源：http://vb.huixinmuqiang.cn

C#:   42.ToString()
来源：http://rx.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://bt.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eh.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lf.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sf.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yl.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oe.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sq.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://al.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://up.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://gg.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bd.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dt.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ih.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dr.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uy.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nb.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ye.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ik.bookmarksfly.cn

[A10] 生成随机数
来源：http://ip.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://fv.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://xa.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jm.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://su.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://ev.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ai.521024.cn

Ruby: rand(1..100)
来源：http://cv.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://ly.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://pi.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://su.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cm.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ap.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vr.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://fe.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cn.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://io.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bj.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://pb.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ct.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tq.asd995.cn

JS:   `Hello, ${name}!`
来源：http://qw.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://mh.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ry.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nv.521024.cn

Ruby: "Hello, #{name}!"
来源：http://zr.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://zf.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ht.hahajie.cn

Py:   "第一行\n第二行"
来源：http://rh.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://uy.huanxung.cn

JS:   "第一行\n第二行"
来源：http://ec.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://mv.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ok.szsharing.cn

Go:   "第一行\n第二行"
来源：http://pl.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://fs.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ty.szxytkj.cn

[A14] 注释写法
来源：http://tz.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ln.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://zi.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://rr.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zx.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://eb.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ox.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://hq.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://oq.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://fb.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://ru.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://oa.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://eu.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lb.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://nd.nszjky.cn

Ruby: value = data || "默认值"
来源：http://bx.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://os.yuexingan06.cn

[A16] 真假值判断规则
来源：http://hb.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lf.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xu.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wa.huanxung.cn

TS:   if (!x) {}
来源：http://ew.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ps.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://si.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oe.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lr.9csxet.cn

[A17] 位运算
来源：http://gh.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://si.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kt.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wn.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://du.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cm.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lp.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://go.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://jf.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ue.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ot.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://us.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://un.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://km.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://bz.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://fx.szsharing.cn

[A19] 交换两个变量
来源：http://lf.yuexingan06.cn

Py:   a, b = b, a
来源：http://sx.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dj.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://xh.521024.cn

TS:   [a, b] = [b, a];
来源：http://xw.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://bo.hnjuh.cn

Go:   a, b = b, a
来源：http://av.gzmigu.cn

Ruby: a, b = b, a
来源：http://sm.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://jo.yuexingan06.cn

[A20] 读取标准输入
来源：http://wj.nszjky.cn

Py:   name = input("请输入：")
来源：http://kc.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gy.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ht.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://dj.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://um.szsharing.cn

Ruby: gets.chomp
来源：http://te.szsharing.cn

C#:   Console.ReadLine();
来源：http://zq.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://cx.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://wr.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yt.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://zi.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://nr.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://vp.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sx.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://bx.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://vp.shtwfgs.cn

[A22] 获取字符串长度
来源：http://xw.chemitech.net.cn

Py:   len(s)
来源：http://rg.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jp.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ew.yuntaijiaju.cn

TS:   s.length
来源：http://jy.nicolike.cn

Java: s.length()
来源：http://zh.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rp.yuexingan06.cn

Ruby: s.length
来源：http://qg.chemitech.net.cn

C#:   s.Length
来源：http://im.newstarts.cn

[A23] 大小写转换
来源：http://ac.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lx.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://py.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://on.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gn.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mc.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cj.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kb.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bg.gzmigu.cn

[A24] 去除首尾空白
来源：http://yg.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://un.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qq.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ph.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gr.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qy.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://su.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mw.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rp.bookmarksfly.cn

[A25] 字符串比较
来源：http://uf.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://ex.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bk.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tn.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://io.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lj.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ss.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ol.newstarts.cn

[A26] 类型转换总览
来源：http://dz.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tg.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gp.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ef.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://we.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jd.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xn.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rj.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ja.jctech888.com.cn

================================================================================
来源：http://ms.szsharing.cn

B. 流程控制
来源：http://bu.muxihuayi.cn

================================================================================
来源：http://zn.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://su.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dq.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aj.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gv.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wo.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ct.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gn.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://rw.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yt.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xs.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ux.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bn.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zj.hahajie.cn

[B03] switch / match / case
来源：http://qx.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wj.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wa.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wm.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lo.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pj.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fb.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xw.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ab.bookmarksfly.cn

[B04] for 计数循环
来源：http://hm.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://nx.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kv.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yw.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ks.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://el.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bw.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://gi.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://to.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://hi.nszjky.cn

Py:   for item in arr: print(item)
来源：http://xq.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sw.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kx.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xj.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://js.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bl.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://in.wgjwhj.cn


<!-- 参考信息 -->