代发 wailian999

================================================================================
来源：http://rz.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://nk.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://uj.hahajie.cn

================================================================================
来源：http://qf.newstarts.cn

【收录内容】
来源：http://gq.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iw.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sh.newstarts.cn

SQL · Bash · C · C++
来源：http://uv.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dk.shxzskj.cn

【使用说明】
来源：http://cq.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qp.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wg.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kp.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bk.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://su.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jl.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ri.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jr.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tm.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ys.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vz.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kw.bjjhwx.cn

【文件统计】
来源：http://yw.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cg.colortex.cn

--------------------------------------------------------------------------------
来源：http://sw.haigaiapp.cn

目  录
来源：http://hb.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ec.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ew.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ar.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fp.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kc.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aq.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yk.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://js.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fq.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bt.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yx.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uk.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cv.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pm.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://me.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nu.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rs.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uz.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vu.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cu.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ay.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eh.chemitech.net.cn

================================================================================
来源：http://ti.wgjwhj.cn

A. 基础语法与类型
来源：http://ga.colortex.cn

================================================================================
来源：http://wg.wgjwhj.cn

[A01] Hello World
来源：http://wy.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://vm.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://uj.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://tu.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ci.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://mg.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://mc.asd995.cn

Ruby: puts "Hello, World!"
来源：http://fz.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xw.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://cb.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ng.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gd.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://te.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kr.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ew.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://wy.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://em.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qz.yuntaijiaju.cn

[A03] 常量定义
来源：http://ls.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ez.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://jr.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://vr.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ec.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://em.shxzukj.cn

Go:   const PI = 3.14159
来源：http://tk.nicolike.cn

Ruby: PI = 3.14159
来源：http://su.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://xa.huixiangedu.cn

[A04] 判断变量类型
来源：http://he.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://px.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cy.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ff.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://fo.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dc.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kl.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oz.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://iu.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://oh.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vn.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kh.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tt.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qf.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://vy.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://qm.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://mk.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://ho.colortex.cn

[A06] 字符串转数字
来源：http://ey.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://gf.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ky.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ea.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ix.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gi.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ln.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://js.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ty.shxzskj.cn

[A07] 数字转字符串
来源：http://yh.hnjuh.cn

Py:   str(42)
来源：http://nr.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://iz.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://ha.nicolike.cn

TS:   String(42)
来源：http://xa.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eo.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://sy.hahajie.cn

Ruby: 42.to_s
来源：http://cr.yuexingan06.cn

C#:   42.ToString()
来源：http://bg.asd995.cn

[A08] 取整与四舍五入
来源：http://nt.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mx.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kk.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dz.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yn.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mb.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tb.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jh.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bg.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://ml.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qf.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://js.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zj.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bh.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lc.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bm.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ok.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yo.gzmigu.cn

[A10] 生成随机数
来源：http://bv.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://wy.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://al.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ge.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ka.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ja.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ut.hahajie.cn

Ruby: rand(1..100)
来源：http://bh.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://du.colortex.cn

[A11] 条件表达式（三元）
来源：http://jm.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://bm.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yy.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bx.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sp.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://kh.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://be.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ip.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fo.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://zk.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dg.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xf.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ne.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://es.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://fy.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eu.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://kf.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://es.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cp.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://cf.asd995.cn

PHP:  "第一行\n第二行"
来源：http://xc.521024.cn

JS:   "第一行\n第二行"
来源：http://km.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://su.shxzukj.cn

Java: "第一行\n第二行"
来源：http://rm.huanxung.cn

Go:   "第一行\n第二行"
来源：http://wr.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://st.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://vx.gzmigu.cn

[A14] 注释写法
来源：http://gj.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wl.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qm.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://ot.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://kd.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pa.521024.cn

Go:   // 单行；/* 多行 */
来源：http://tm.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://os.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://pj.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://qf.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://pk.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://au.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://dc.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://kl.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fc.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://tu.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ut.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://uj.chemitech.net.cn

[A16] 真假值判断规则
来源：http://ll.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://om.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wp.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cx.bookmarksfly.cn

TS:   if (!x) {}
来源：http://em.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qi.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fh.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zc.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jh.muxihuayi.cn

[A17] 位运算
来源：http://qg.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ly.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ad.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ij.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://wm.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://ai.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://pl.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mk.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ds.521024.cn

Java: (int) 'A'; (char) 65
来源：http://tx.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qh.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://oe.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://qd.jctech888.com.cn

[A19] 交换两个变量
来源：http://mh.lnxyls.cn

Py:   a, b = b, a
来源：http://bi.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fk.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://uf.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://mw.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://nq.haigaiapp.cn

Go:   a, b = b, a
来源：http://lf.newstarts.cn

Ruby: a, b = b, a
来源：http://tp.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://he.9csxet.cn

[A20] 读取标准输入
来源：http://dm.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://fo.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sy.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zl.521024.cn

TS:   // Node.js：readline 模块
来源：http://mx.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://ry.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bd.colortex.cn

Ruby: gets.chomp
来源：http://zl.huanxung.cn

C#:   Console.ReadLine();
来源：http://ga.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://is.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://hr.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kb.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://ij.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://tk.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://vv.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lo.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://yy.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://zz.lnxyls.cn

[A22] 获取字符串长度
来源：http://ck.jctech888.com.cn

Py:   len(s)
来源：http://wy.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fw.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ad.colortex.cn

TS:   s.length
来源：http://jn.huanxung.cn

Java: s.length()
来源：http://rz.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yz.shxzukj.cn

Ruby: s.length
来源：http://lv.521024.cn

C#:   s.Length
来源：http://ir.hnjuh.cn

[A23] 大小写转换
来源：http://pz.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ov.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ow.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ef.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ae.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hv.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zb.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qr.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pu.asd995.cn

[A24] 去除首尾空白
来源：http://bk.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bg.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qv.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iy.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ju.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fm.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://du.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hx.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ck.yuntaijiaju.cn

[A25] 字符串比较
来源：http://fy.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://xd.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sq.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bh.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fq.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://br.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tx.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mq.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yr.shxzskj.cn

[A26] 类型转换总览
来源：http://mm.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aj.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mx.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yc.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://px.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ux.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://re.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mh.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ue.huanxung.cn

================================================================================
来源：http://xx.jianghongdianzi.cn

B. 流程控制
来源：http://qb.shxzskj.cn

================================================================================
来源：http://xs.asd995.cn

[B01] 条件判断 if / else
来源：http://tq.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hb.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xd.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://km.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vn.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bd.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ih.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ii.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qk.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://zk.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cl.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nw.nicolike.cn


<!-- 参考信息 -->