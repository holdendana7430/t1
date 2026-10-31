代发 wailian999

================================================================================
来源：http://bx.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ej.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://wo.huanxung.cn

================================================================================
来源：http://vg.hnjuh.cn

【收录内容】
来源：http://fr.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pg.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fg.nicolike.cn

SQL · Bash · C · C++
来源：http://jl.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fc.huanxung.cn

【使用说明】
来源：http://sg.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sn.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lx.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vq.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ma.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kt.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zq.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sa.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ir.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zz.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gm.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fy.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://af.newstarts.cn

【文件统计】
来源：http://qc.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gu.521024.cn

--------------------------------------------------------------------------------
来源：http://wa.jianghongdianzi.cn

目  录
来源：http://eu.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ja.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aw.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lt.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sj.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hd.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qw.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sh.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ij.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://he.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ot.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qx.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oy.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gd.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kz.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vb.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dd.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nl.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xs.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ew.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jx.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fp.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ox.shxzukj.cn

================================================================================
来源：http://cd.bjjhwx.cn

A. 基础语法与类型
来源：http://if.hahajie.cn

================================================================================
来源：http://ar.huixinmuqiang.cn

[A01] Hello World
来源：http://rb.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ia.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://zg.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://bn.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gd.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://ka.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://nz.colortex.cn

Ruby: puts "Hello, World!"
来源：http://fg.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ln.huanxung.cn

[A02] 变量声明与赋值
来源：http://ub.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zl.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ft.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qm.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sx.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://wm.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://hp.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://qf.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ve.gzmigu.cn

[A03] 常量定义
来源：http://tv.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ij.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://pi.nicolike.cn

JS:   const PI = 3.14159;
来源：http://qa.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://sm.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://ec.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ko.shxzukj.cn

Ruby: PI = 3.14159
来源：http://lx.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://eb.colortex.cn

[A04] 判断变量类型
来源：http://of.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ve.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gp.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qh.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://ek.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ii.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ps.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sx.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://qz.szxytkj.cn

[A05] 整数除法与取模
来源：http://hh.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ix.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fh.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wr.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ho.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://te.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://cj.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://kc.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://ge.szxytkj.cn

[A06] 字符串转数字
来源：http://uv.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://nz.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tw.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://po.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cd.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hq.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xc.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pz.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zm.shtwfgs.cn

[A07] 数字转字符串
来源：http://ke.bjjhwx.cn

Py:   str(42)
来源：http://qy.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://sz.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://zs.huixinmuqiang.cn

TS:   String(42)
来源：http://zd.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://by.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://jb.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://lw.shtwfgs.cn

C#:   42.ToString()
来源：http://nf.asd995.cn

[A08] 取整与四舍五入
来源：http://wd.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tx.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://av.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ou.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://if.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://se.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lu.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://by.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ek.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://pw.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://be.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wv.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cg.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wj.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zh.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zv.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ct.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sg.hahajie.cn

[A10] 生成随机数
来源：http://tz.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://hj.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://ya.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ih.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uf.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://ai.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iw.yuexingan06.cn

Ruby: rand(1..100)
来源：http://dy.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://wy.szsharing.cn

[A11] 条件表达式（三元）
来源：http://xy.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://ci.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jx.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mr.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cc.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://rt.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://va.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tg.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fo.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://tv.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qa.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://np.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://mn.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://lq.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://eg.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ui.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://ow.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://bq.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://je.huanxung.cn

Py:   "第一行\n第二行"
来源：http://gq.asd995.cn

PHP:  "第一行\n第二行"
来源：http://za.newstarts.cn

JS:   "第一行\n第二行"
来源：http://he.szsharing.cn

TS:   "第一行\n第二行"
来源：http://tm.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://aq.asd995.cn

Go:   "第一行\n第二行"
来源：http://hy.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://va.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://je.gzmigu.cn

[A14] 注释写法
来源：http://xr.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ri.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qk.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://is.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://pc.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uh.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://yi.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tc.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://yd.9csxet.cn

[A15] 空值判断与默认值
来源：http://ol.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ug.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://ol.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://gs.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://bx.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ll.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://bo.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://hw.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://fd.nicolike.cn

[A16] 真假值判断规则
来源：http://qv.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xx.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ba.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bs.bookmarksfly.cn

TS:   if (!x) {}
来源：http://bg.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yl.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://da.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qm.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pg.hahajie.cn

[A17] 位运算
来源：http://mw.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kz.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pj.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lq.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ic.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fh.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jr.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://pa.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://lw.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://tn.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rk.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zy.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://pt.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oo.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://oh.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://iz.bjjhwx.cn

[A19] 交换两个变量
来源：http://uv.521024.cn

Py:   a, b = b, a
来源：http://zs.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://br.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://pq.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://dv.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ts.szxytkj.cn

Go:   a, b = b, a
来源：http://cl.gzmigu.cn

Ruby: a, b = b, a
来源：http://xv.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://vv.shxzukj.cn

[A20] 读取标准输入
来源：http://bw.hahajie.cn

Py:   name = input("请输入：")
来源：http://dx.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://se.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xy.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://vc.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://vq.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xc.asd995.cn

Ruby: gets.chomp
来源：http://lw.huanxung.cn

C#:   Console.ReadLine();
来源：http://ht.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://ms.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://wc.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dw.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://gq.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://qk.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://zm.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nz.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://rg.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://jd.colortex.cn

[A22] 获取字符串长度
来源：http://qi.shtwfgs.cn

Py:   len(s)
来源：http://gy.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oc.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yb.nszjky.cn

TS:   s.length
来源：http://am.asd995.cn

Java: s.length()
来源：http://ka.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uv.yuexingan06.cn

Ruby: s.length
来源：http://ib.panjiajie.cn

C#:   s.Length
来源：http://ed.szxytkj.cn

[A23] 大小写转换
来源：http://fp.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dc.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ac.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fd.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tq.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://po.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tx.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lm.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yp.muxihuayi.cn

[A24] 去除首尾空白
来源：http://oh.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ej.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rr.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nd.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vx.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://rm.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tc.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nm.nszjky.cn

[A25] 字符串比较
来源：http://gl.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://cl.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zj.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gh.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://me.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fw.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rw.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lv.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gk.huixiangedu.cn

[A26] 类型转换总览
来源：http://qk.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pe.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jy.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ea.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://qv.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fh.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ri.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ks.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tq.hnjuh.cn

================================================================================
来源：http://ys.gzmigu.cn

B. 流程控制
来源：http://rk.szxytkj.cn

================================================================================
来源：http://zb.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://id.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://th.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nw.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hc.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vl.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yq.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wt.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sr.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gn.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://cb.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://di.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lc.panjiajie.cn


<!-- 参考信息 -->