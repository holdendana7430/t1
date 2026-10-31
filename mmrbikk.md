代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ry.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tw.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oi.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lt.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tl.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kg.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nr.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kh.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ez.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qi.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rz.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vj.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zl.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fi.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yd.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sn.bookmarksfly.cn

================================================================================
来源：http://bv.jianghongdianzi.cn

A. 基础语法与类型
来源：http://nq.nicolike.cn

================================================================================
来源：http://xk.521024.cn

[A01] Hello World
来源：http://pe.newstarts.cn

Py:   print("Hello, World!")
来源：http://yc.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://ho.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://kc.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gu.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://jl.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://wo.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://fw.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nd.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ge.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gs.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fm.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dr.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nk.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://vr.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://gy.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://rh.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sh.wgjwhj.cn

[A03] 常量定义
来源：http://gr.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nw.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://rs.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://tx.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://yn.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://gj.lnxyls.cn

Go:   const PI = 3.14159
来源：http://eg.nszjky.cn

Ruby: PI = 3.14159
来源：http://om.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ih.shxzskj.cn

[A04] 判断变量类型
来源：http://dr.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nk.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fk.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fs.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://ms.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kc.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pd.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jt.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://xd.shxzukj.cn

[A05] 整数除法与取模
来源：http://pe.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gv.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qz.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://na.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yv.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://ps.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://fl.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://nn.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://fe.bookmarksfly.cn

[A06] 字符串转数字
来源：http://bz.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://tq.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yn.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yg.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hj.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ih.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rv.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hj.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vm.shtwfgs.cn

[A07] 数字转字符串
来源：http://zc.szxytkj.cn

Py:   str(42)
来源：http://cs.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://ms.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://nq.wgjwhj.cn

TS:   String(42)
来源：http://em.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ry.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://nh.muxihuayi.cn

Ruby: 42.to_s
来源：http://lb.hahajie.cn

C#:   42.ToString()
来源：http://dk.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://ht.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://su.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jv.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ce.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kq.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yh.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oj.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hm.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://jz.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://md.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ly.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wm.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fc.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pb.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xg.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cm.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ly.colortex.cn

[A10] 生成随机数
来源：http://sq.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://an.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://eh.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://md.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ay.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://wx.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hl.hnjuh.cn

Ruby: rand(1..100)
来源：http://vo.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://ps.newstarts.cn

[A11] 条件表达式（三元）
来源：http://dc.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://kf.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ee.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://so.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qi.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://hv.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ic.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ji.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wn.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://km.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mr.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wc.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://gx.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://vs.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://jd.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tv.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://ua.521024.cn

C#:   $"Hello, {name}!"
来源：http://ei.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pb.hahajie.cn

Py:   "第一行\n第二行"
来源：http://yv.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://vz.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://nn.szsharing.cn

TS:   "第一行\n第二行"
来源：http://jg.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://gf.huanxung.cn

Go:   "第一行\n第二行"
来源：http://wx.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://xx.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://wh.yuexingan06.cn

[A14] 注释写法
来源：http://pt.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rq.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ok.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://gq.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ih.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ak.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://hz.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wi.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://og.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://mv.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://qg.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://dn.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://jb.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ug.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hj.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://nx.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://zu.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://ps.chemitech.net.cn

[A16] 真假值判断规则
来源：http://qz.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ac.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zh.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vo.szxytkj.cn

TS:   if (!x) {}
来源：http://my.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zl.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fy.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ei.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yf.jctech888.com.cn

[A17] 位运算
来源：http://rk.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wo.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tb.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yg.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qw.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vc.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://od.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://eq.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://cx.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://bm.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ny.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://td.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://uo.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gc.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://dw.521024.cn

C#:   (int)'A'; (char)65
来源：http://de.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://aq.lnxyls.cn

Py:   a, b = b, a
来源：http://ap.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pv.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://lc.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://ue.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://gf.huanxung.cn

Go:   a, b = b, a
来源：http://ec.shtwfgs.cn

Ruby: a, b = b, a
来源：http://tw.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://ba.bjjhwx.cn

[A20] 读取标准输入
来源：http://yf.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ax.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ie.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nx.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://yt.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://md.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://op.nszjky.cn

Ruby: gets.chomp
来源：http://ep.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://wa.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://hr.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://hg.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ey.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://vs.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://pp.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://co.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ak.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://st.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://rv.gzmigu.cn

[A22] 获取字符串长度
来源：http://ef.asd995.cn

Py:   len(s)
来源：http://se.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ps.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qn.gzmigu.cn

TS:   s.length
来源：http://ol.yuexingan06.cn

Java: s.length()
来源：http://me.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jg.hnjuh.cn

Ruby: s.length
来源：http://vi.jianghongdianzi.cn

C#:   s.Length
来源：http://cm.asd995.cn

[A23] 大小写转换
来源：http://yk.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yt.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ia.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://my.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pe.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ka.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gj.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xu.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ju.jctech888.com.cn

[A24] 去除首尾空白
来源：http://zp.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sz.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lp.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ta.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iq.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zn.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ue.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tc.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xe.haigaiapp.cn

[A25] 字符串比较
来源：http://rd.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://oq.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nf.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ls.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vb.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uy.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lx.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ge.huixiangedu.cn

[A26] 类型转换总览
来源：http://fq.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ql.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://al.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vw.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://ru.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ak.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jv.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ki.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qq.haigaiapp.cn

================================================================================
来源：http://ae.haigaiapp.cn

B. 流程控制
来源：http://wp.haigaiapp.cn

================================================================================
来源：http://nu.colortex.cn

[B01] 条件判断 if / else
来源：http://qr.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ed.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sa.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kz.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://os.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ot.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uv.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vh.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uu.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://mi.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mm.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vr.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bf.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vv.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hs.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ch.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ll.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iv.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zf.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xm.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ie.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fg.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ma.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sh.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://in.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ld.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://eb.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bb.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oa.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yp.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pk.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kz.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://wl.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://et.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://zs.nicolike.cn

Py:   for item in arr: print(item)
来源：http://rc.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lx.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://er.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cc.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cx.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qq.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://sy.colortex.cn


<!-- 参考信息 -->