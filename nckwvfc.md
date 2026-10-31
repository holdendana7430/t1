代发 wailian999

--------------------------------------------------------------------------------
来源：http://zr.jctech888.com.cn

目  录
来源：http://yl.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://tr.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qh.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uk.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://as.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fz.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lh.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://co.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fe.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vg.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mf.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lk.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bc.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://no.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qg.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wt.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ls.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nd.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ca.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lc.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dn.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bf.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bm.szxytkj.cn

================================================================================
来源：http://vl.muxihuayi.cn

A. 基础语法与类型
来源：http://rz.hnjuh.cn

================================================================================
来源：http://nd.wgjwhj.cn

[A01] Hello World
来源：http://dj.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://uu.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://dt.colortex.cn

JS:   console.log("Hello, World!");
来源：http://av.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rv.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://da.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://uk.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://ea.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hs.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://vi.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ry.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ob.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xp.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lh.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://nk.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://eu.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://qv.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yf.chemitech.net.cn

[A03] 常量定义
来源：http://cd.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jg.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://ri.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://ba.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://ns.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://kz.9csxet.cn

Go:   const PI = 3.14159
来源：http://ju.shxzukj.cn

Ruby: PI = 3.14159
来源：http://if.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://xa.panjiajie.cn

[A04] 判断变量类型
来源：http://li.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hk.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ze.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pj.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://ty.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jp.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ez.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sx.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://fc.521024.cn

[A05] 整数除法与取模
来源：http://gl.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gp.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nt.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bi.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ct.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://fy.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://yv.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://jt.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://ac.shxzskj.cn

[A06] 字符串转数字
来源：http://bt.colortex.cn

Py:   int("42"); float("3.14")
来源：http://ru.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rv.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ss.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zg.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://up.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://am.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lb.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ny.hnjuh.cn

[A07] 数字转字符串
来源：http://ao.chemitech.net.cn

Py:   str(42)
来源：http://fs.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://br.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://ti.jianghongdianzi.cn

TS:   String(42)
来源：http://lr.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://se.asd995.cn

Go:   strconv.Itoa(42)
来源：http://wi.521024.cn

Ruby: 42.to_s
来源：http://ya.nicolike.cn

C#:   42.ToString()
来源：http://bi.hahajie.cn

[A08] 取整与四舍五入
来源：http://bx.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gd.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ut.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cx.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ez.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jl.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ct.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qv.colortex.cn

[A09] 绝对值与最大最小值
来源：http://ux.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dc.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sq.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ws.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ug.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bi.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ob.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sb.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yu.asd995.cn

[A10] 生成随机数
来源：http://ti.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://pp.hahajie.cn

PHP:  random_int(1, 100);
来源：http://ze.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yd.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cq.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://cb.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vr.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://px.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://wg.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://bd.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://tw.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ar.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://st.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bd.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://io.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://py.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hy.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qn.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://xl.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sx.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ea.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://mt.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://kn.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://py.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ro.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://rd.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://yt.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tu.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ut.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://hm.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://xx.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://ej.lnxyls.cn

Java: "第一行\n第二行"
来源：http://lh.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://yg.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://qm.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://lo.asd995.cn

[A14] 注释写法
来源：http://mq.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ef.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zm.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://kf.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://cq.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nh.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://xs.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://er.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://go.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://nc.newstarts.cn

Py:   value = data or "默认值"
来源：http://ui.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://xo.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://eo.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://tu.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rx.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://sq.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://yx.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://ro.colortex.cn

[A16] 真假值判断规则
来源：http://fs.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qn.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yu.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qr.nszjky.cn

TS:   if (!x) {}
来源：http://sc.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bx.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ww.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yw.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ad.shxzskj.cn

[A17] 位运算
来源：http://sm.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ep.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sh.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ll.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fk.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bb.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wt.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fw.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://il.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://gh.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://gq.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://rk.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yh.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iw.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://or.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://du.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://kt.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://do.panjiajie.cn

[A19] 交换两个变量
来源：http://qm.haigaiapp.cn

Py:   a, b = b, a
来源：http://tq.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jn.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://hi.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://nd.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://ja.gzmigu.cn

Go:   a, b = b, a
来源：http://dw.nicolike.cn

Ruby: a, b = b, a
来源：http://tb.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://rd.hnjuh.cn

[A20] 读取标准输入
来源：http://as.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://jr.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ji.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ui.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://xw.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ei.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fu.wgjwhj.cn

Ruby: gets.chomp
来源：http://cl.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://oi.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://ym.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://za.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wq.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://yf.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://xa.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://ws.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pb.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://se.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://cs.huixiangedu.cn

[A22] 获取字符串长度
来源：http://xo.9csxet.cn

Py:   len(s)
来源：http://bn.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hu.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sp.wgjwhj.cn

TS:   s.length
来源：http://mr.521024.cn

Java: s.length()
来源：http://cf.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xl.bookmarksfly.cn

Ruby: s.length
来源：http://bi.asd995.cn

C#:   s.Length
来源：http://mx.colortex.cn

[A23] 大小写转换
来源：http://ot.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fu.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://br.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lo.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oa.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hw.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rj.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zf.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nx.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ky.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ou.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qy.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zt.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hm.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ku.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kz.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aw.lnxyls.cn

[A25] 字符串比较
来源：http://qh.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://th.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bx.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iz.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lr.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wo.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ad.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bk.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kr.newstarts.cn

[A26] 类型转换总览
来源：http://sw.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oq.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jy.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://si.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://kx.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nf.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pc.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ed.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qd.shxzskj.cn

================================================================================
来源：http://us.newstarts.cn

B. 流程控制
来源：http://js.asd995.cn

================================================================================
来源：http://lg.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://bw.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lf.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://me.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jo.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gp.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rx.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://id.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cz.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://se.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://fa.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sp.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gb.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lf.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wf.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.bjjhwx.cn

[B03] switch / match / case
来源：http://wy.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sy.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ua.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cq.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ed.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://le.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mb.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ej.haigaiapp.cn

[B04] for 计数循环
来源：http://uh.colortex.cn

Py:   for i in range(10): print(i)
来源：http://gy.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lx.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hm.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ut.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vb.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zg.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://dy.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ri.huixiangedu.cn


<!-- 参考信息 -->