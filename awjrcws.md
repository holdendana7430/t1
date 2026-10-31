代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mi.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zz.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lt.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qm.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://py.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xv.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://do.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ai.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wm.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kv.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hd.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nh.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jx.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lf.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rl.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yr.hnjuh.cn

================================================================================
来源：http://ix.hahajie.cn

A. 基础语法与类型
来源：http://hn.newstarts.cn

================================================================================
来源：http://sl.wgjwhj.cn

[A01] Hello World
来源：http://sg.nicolike.cn

Py:   print("Hello, World!")
来源：http://ya.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://fn.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://kb.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sz.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://jo.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://no.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://kg.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qa.shxzukj.cn

[A02] 变量声明与赋值
来源：http://jf.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bo.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://es.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ub.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jb.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://tk.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://yr.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://kn.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ec.9csxet.cn

[A03] 常量定义
来源：http://mg.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wo.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://ae.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://eq.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://xq.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://cm.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://uo.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://gv.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://st.panjiajie.cn

[A04] 判断变量类型
来源：http://pb.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nh.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lb.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vb.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://iw.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gg.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qu.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://os.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://ve.huanxung.cn

[A05] 整数除法与取模
来源：http://wy.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ho.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sk.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sy.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cy.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://us.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://gp.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ja.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://cn.gzmigu.cn

[A06] 字符串转数字
来源：http://dj.asd995.cn

Py:   int("42"); float("3.14")
来源：http://kd.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zj.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ry.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ne.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gr.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fo.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://su.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xz.bjjhwx.cn

[A07] 数字转字符串
来源：http://fm.colortex.cn

Py:   str(42)
来源：http://ny.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://hu.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://pz.panjiajie.cn

TS:   String(42)
来源：http://jj.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xy.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://to.asd995.cn

Ruby: 42.to_s
来源：http://ol.gzmigu.cn

C#:   42.ToString()
来源：http://ig.nicolike.cn

[A08] 取整与四舍五入
来源：http://aa.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yy.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ff.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lu.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ls.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dt.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vz.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pr.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ol.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://ag.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://or.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vt.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fc.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iv.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ib.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rc.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jk.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gc.yuexingan06.cn

[A10] 生成随机数
来源：http://uh.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://ro.huanxung.cn

PHP:  random_int(1, 100);
来源：http://iv.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rh.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xt.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://ce.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dg.bjjhwx.cn

Ruby: rand(1..100)
来源：http://ux.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://yb.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://yd.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://vt.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pa.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ye.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bn.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://jp.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qn.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ph.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kc.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://ym.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cv.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wi.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://uk.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://lj.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://pn.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ic.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ji.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://pj.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cd.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://zr.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://gj.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://dw.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://qe.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://iw.nicolike.cn

Go:   "第一行\n第二行"
来源：http://qk.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://ic.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://kl.nszjky.cn

[A14] 注释写法
来源：http://jp.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bl.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tb.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ws.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://uz.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pv.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://zm.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cp.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://rg.asd995.cn

[A15] 空值判断与默认值
来源：http://vp.hnjuh.cn

Py:   value = data or "默认值"
来源：http://pe.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://mw.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://zo.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://uq.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kv.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://sw.huanxung.cn

Ruby: value = data || "默认值"
来源：http://pt.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://sw.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://sr.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dt.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lj.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://he.haigaiapp.cn

TS:   if (!x) {}
来源：http://jv.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ga.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mv.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://or.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xf.yuntaijiaju.cn

[A17] 位运算
来源：http://of.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uv.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vz.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nr.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cy.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cr.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fb.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zr.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://dp.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://fw.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://ki.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jr.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vw.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://fl.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xo.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://gl.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://rl.gzmigu.cn

[A19] 交换两个变量
来源：http://vk.521024.cn

Py:   a, b = b, a
来源：http://pc.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tn.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://xk.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://hi.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ah.bookmarksfly.cn

Go:   a, b = b, a
来源：http://vh.haigaiapp.cn

Ruby: a, b = b, a
来源：http://ug.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://kb.lnxyls.cn

[A20] 读取标准输入
来源：http://ax.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://nu.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xt.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wn.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://cx.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://gm.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tl.haigaiapp.cn

Ruby: gets.chomp
来源：http://rw.hahajie.cn

C#:   Console.ReadLine();
来源：http://wa.asd995.cn

[A21] 保留指定小数位输出
来源：http://wf.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://hw.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mc.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://vm.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://xq.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://sa.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qy.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://ag.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://xa.lnxyls.cn

[A22] 获取字符串长度
来源：http://cc.shtwfgs.cn

Py:   len(s)
来源：http://ks.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yc.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vf.newstarts.cn

TS:   s.length
来源：http://ku.shtwfgs.cn

Java: s.length()
来源：http://ra.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wi.lnxyls.cn

Ruby: s.length
来源：http://sr.gzmigu.cn

C#:   s.Length
来源：http://rt.521024.cn

[A23] 大小写转换
来源：http://pl.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lf.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rx.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xi.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fa.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ko.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sr.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://os.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wq.shxzskj.cn

[A24] 去除首尾空白
来源：http://do.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://st.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ln.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tz.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iv.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://le.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://ee.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eo.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dq.colortex.cn

[A25] 字符串比较
来源：http://qz.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://xp.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xf.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qc.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xe.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qu.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qp.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xs.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fa.bookmarksfly.cn

[A26] 类型转换总览
来源：http://fr.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fx.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zk.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cc.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ts.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ud.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qe.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jv.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://na.haigaiapp.cn

================================================================================
来源：http://ff.asd995.cn

B. 流程控制
来源：http://oj.szsharing.cn

================================================================================
来源：http://bd.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://ms.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yv.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ph.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sr.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zv.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yp.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ld.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://df.hahajie.cn

[B02] 多分支 else if / elif
来源：http://gn.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tk.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rl.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bb.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xs.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eb.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.shtwfgs.cn

[B03] switch / match / case
来源：http://wn.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yy.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lr.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xp.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yb.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vn.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cl.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ek.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jq.nicolike.cn

[B04] for 计数循环
来源：http://ot.521024.cn

Py:   for i in range(10): print(i)
来源：http://az.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ql.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oc.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gz.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lt.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ue.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://wk.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qd.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://yw.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://nw.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kq.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mb.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kb.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gi.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lv.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://hh.colortex.cn


<!-- 参考信息 -->