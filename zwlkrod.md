代发 wailian999

================================================================================
来源：http://it.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://bu.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://mt.asd995.cn

================================================================================
来源：http://jx.yuexingan06.cn

【收录内容】
来源：http://hw.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qy.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nh.hnjuh.cn

SQL · Bash · C · C++
来源：http://ts.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ca.chemitech.net.cn

【使用说明】
来源：http://tm.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jd.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://or.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wg.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kk.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fn.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mp.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wa.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xc.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ai.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cl.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://to.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pp.chemitech.net.cn

【文件统计】
来源：http://sj.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ty.huanxung.cn

--------------------------------------------------------------------------------
来源：http://zc.szsharing.cn

目  录
来源：http://at.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://su.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fa.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ag.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zm.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ww.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iq.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://du.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ea.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gw.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xz.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ka.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jh.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ev.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ue.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gq.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bx.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ke.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tj.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ln.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xt.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ww.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qt.yuexingan06.cn

================================================================================
来源：http://ge.jctech888.com.cn

A. 基础语法与类型
来源：http://lp.9csxet.cn

================================================================================
来源：http://rl.huixiangedu.cn

[A01] Hello World
来源：http://fj.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://ru.colortex.cn

PHP:  echo "Hello, World!";
来源：http://ut.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://cx.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ls.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://ft.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://pi.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://yp.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vi.shxzskj.cn

[A02] 变量声明与赋值
来源：http://yb.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dg.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jy.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qs.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pz.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://jt.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://vj.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://jj.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ca.hnjuh.cn

[A03] 常量定义
来源：http://hx.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://af.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://du.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://mx.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://sx.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://kt.panjiajie.cn

Go:   const PI = 3.14159
来源：http://do.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://kc.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://et.jctech888.com.cn

[A04] 判断变量类型
来源：http://oa.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bx.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://my.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vo.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://qa.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tb.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ok.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yq.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://mb.haigaiapp.cn

[A05] 整数除法与取模
来源：http://ds.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gu.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://er.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ls.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qz.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://qf.521024.cn

Go:   7 / 2; 7 % 2
来源：http://cm.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://nu.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://yw.9csxet.cn

[A06] 字符串转数字
来源：http://vm.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://pz.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cx.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ql.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vb.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xa.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bq.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qp.shxzskj.cn

[A07] 数字转字符串
来源：http://xu.asd995.cn

Py:   str(42)
来源：http://et.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://xm.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://lp.szsharing.cn

TS:   String(42)
来源：http://wu.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zg.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://qz.haigaiapp.cn

Ruby: 42.to_s
来源：http://nd.lnxyls.cn

C#:   42.ToString()
来源：http://fm.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://xo.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ua.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nr.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ff.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wb.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ab.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://by.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ib.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pc.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://vt.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kv.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vu.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://th.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vj.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ks.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nz.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mk.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lh.nszjky.cn

[A10] 生成随机数
来源：http://tv.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://qn.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://lp.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ub.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sk.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://pi.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gy.9csxet.cn

Ruby: rand(1..100)
来源：http://og.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://hg.nszjky.cn

[A11] 条件表达式（三元）
来源：http://wo.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://kw.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uc.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ln.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://yd.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kv.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jn.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lh.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://sj.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dz.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pj.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://yd.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ed.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://sd.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ez.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://zq.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://jr.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pd.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://ay.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://fz.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://aw.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://md.nszjky.cn

Java: "第一行\n第二行"
来源：http://da.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://mt.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://sh.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://tv.huixinmuqiang.cn

[A14] 注释写法
来源：http://lz.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wt.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bb.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://se.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://de.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qw.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://ey.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ha.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://uw.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://dm.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://vv.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://gx.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://ts.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ch.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bk.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://xz.nszjky.cn

Ruby: value = data || "默认值"
来源：http://ll.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://gt.szsharing.cn

[A16] 真假值判断规则
来源：http://fn.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jk.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uz.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://in.lnxyls.cn

TS:   if (!x) {}
来源：http://rw.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cd.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vb.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cg.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://df.huanxung.cn

[A17] 位运算
来源：http://oz.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cf.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sl.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uf.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ta.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ev.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://ib.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://ue.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://tw.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cy.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nf.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://rr.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xf.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://fm.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://qw.huixiangedu.cn

[A19] 交换两个变量
来源：http://et.gzmigu.cn

Py:   a, b = b, a
来源：http://hw.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fa.asd995.cn

JS:   [a, b] = [b, a];
来源：http://bz.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://yf.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://ql.huixiangedu.cn

Go:   a, b = b, a
来源：http://av.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://sp.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://uc.colortex.cn

[A20] 读取标准输入
来源：http://zc.521024.cn

Py:   name = input("请输入：")
来源：http://bl.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jg.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qb.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://zh.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://lj.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bt.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://jm.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://zl.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://wt.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://gs.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hd.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://oq.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://cu.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://ty.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oe.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ft.521024.cn

C#:   3.14159.ToString("F2")
来源：http://ra.huixiangedu.cn

[A22] 获取字符串长度
来源：http://fj.bjjhwx.cn

Py:   len(s)
来源：http://jn.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pz.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vu.haigaiapp.cn

TS:   s.length
来源：http://ik.colortex.cn

Java: s.length()
来源：http://ev.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tw.panjiajie.cn

Ruby: s.length
来源：http://qk.hnjuh.cn

C#:   s.Length
来源：http://nd.nicolike.cn

[A23] 大小写转换
来源：http://ha.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bl.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cu.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://za.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yq.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uz.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fe.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rd.nszjky.cn

[A24] 去除首尾空白
来源：http://rb.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://my.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dh.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uo.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sx.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://ar.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rx.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ag.wgjwhj.cn

[A25] 字符串比较
来源：http://py.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://sn.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ek.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://we.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mg.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sk.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qx.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mu.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ne.nicolike.cn

[A26] 类型转换总览
来源：http://lf.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wc.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eq.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sz.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://wt.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iu.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iu.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zj.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ul.lnxyls.cn

================================================================================
来源：http://uz.huixiangedu.cn

B. 流程控制
来源：http://ru.hnjuh.cn

================================================================================
来源：http://kn.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://mu.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qw.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pj.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ux.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zn.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nl.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://so.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qk.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bg.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://rk.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vu.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eq.huanxung.cn


<!-- 参考信息 -->