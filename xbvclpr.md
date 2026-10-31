代发 wailian999

================================================================================
来源：http://hf.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://mp.hahajie.cn

Common Programming Examples Cheat Book
来源：http://nc.yuntaijiaju.cn

================================================================================
来源：http://xj.haigaiapp.cn

【收录内容】
来源：http://nt.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cr.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://md.jctech888.com.cn

SQL · Bash · C · C++
来源：http://dg.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hy.nicolike.cn

【使用说明】
来源：http://ox.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xm.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ah.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oj.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zf.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vx.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tn.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fb.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://af.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vu.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gp.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vt.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wl.asd995.cn

【文件统计】
来源：http://br.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hu.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ub.gzmigu.cn

目  录
来源：http://wm.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://eo.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ob.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://py.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nu.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vb.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jq.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kh.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ml.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rj.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tn.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ch.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xt.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bf.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nv.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hn.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nq.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cj.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oy.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ig.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fm.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ps.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qc.jctech888.com.cn

================================================================================
来源：http://lu.yuntaijiaju.cn

A. 基础语法与类型
来源：http://av.521024.cn

================================================================================
来源：http://xx.bookmarksfly.cn

[A01] Hello World
来源：http://ou.hnjuh.cn

Py:   print("Hello, World!")
来源：http://ao.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://uo.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://aw.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://po.521024.cn

Java: System.out.println("Hello, World!");
来源：http://jf.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://nl.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://xe.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tf.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://by.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mv.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qp.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xp.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vm.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://uv.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://te.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://be.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rh.9csxet.cn

[A03] 常量定义
来源：http://xg.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fw.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://gg.huanxung.cn

JS:   const PI = 3.14159;
来源：http://qz.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://er.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://wx.lnxyls.cn

Go:   const PI = 3.14159
来源：http://pp.gzmigu.cn

Ruby: PI = 3.14159
来源：http://nk.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://jh.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://vc.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ex.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lt.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lm.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://pn.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vb.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vr.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xt.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://ar.nszjky.cn

[A05] 整数除法与取模
来源：http://mt.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nj.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fg.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hx.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aw.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://bs.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://up.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://jw.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://gh.huanxung.cn

[A06] 字符串转数字
来源：http://ok.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://tq.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ne.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dx.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sa.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xk.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zj.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rf.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://go.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://ca.szxytkj.cn

Py:   str(42)
来源：http://hs.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://oj.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://iq.szsharing.cn

TS:   String(42)
来源：http://zr.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zm.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://va.szsharing.cn

Ruby: 42.to_s
来源：http://wc.asd995.cn

C#:   42.ToString()
来源：http://lt.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://io.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dy.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gv.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hp.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bb.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gs.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mu.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://af.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://my.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://gz.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kl.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gz.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ux.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jg.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bi.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jj.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ra.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qs.muxihuayi.cn

[A10] 生成随机数
来源：http://md.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://zn.hahajie.cn

PHP:  random_int(1, 100);
来源：http://kj.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hj.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aw.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://sx.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ie.asd995.cn

Ruby: rand(1..100)
来源：http://hz.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://he.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://zv.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://pt.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dp.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zj.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ge.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://dl.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dm.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dn.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kd.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://xi.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xz.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lb.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://au.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://lo.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yv.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kg.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://cy.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://cn.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cn.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://ow.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://aa.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://rz.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://gp.hnjuh.cn

Java: "第一行\n第二行"
来源：http://lv.asd995.cn

Go:   "第一行\n第二行"
来源：http://gf.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://sr.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://cm.yuntaijiaju.cn

[A14] 注释写法
来源：http://rz.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bv.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://up.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://td.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://zt.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lh.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://go.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ko.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://ni.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://ld.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://gs.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ra.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://hf.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://zy.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hx.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://sh.colortex.cn

Ruby: value = data || "默认值"
来源：http://eb.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://eg.yuexingan06.cn

[A16] 真假值判断规则
来源：http://mn.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hu.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wg.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ab.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://kx.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aq.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eg.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bq.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nu.colortex.cn

[A17] 位运算
来源：http://ot.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wk.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zt.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://an.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yz.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://uj.521024.cn

Py:   ord("A"); chr(65)
来源：http://qt.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://th.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hs.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://ea.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uj.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://aa.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://hn.gzmigu.cn

[A19] 交换两个变量
来源：http://pj.shtwfgs.cn

Py:   a, b = b, a
来源：http://pr.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wo.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://nc.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://lp.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://oo.yuexingan06.cn

Go:   a, b = b, a
来源：http://mk.newstarts.cn

Ruby: a, b = b, a
来源：http://ga.asd995.cn

C#:   (a, b) = (b, a);
来源：http://pz.gzmigu.cn

[A20] 读取标准输入
来源：http://te.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://ya.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ym.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iu.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://dw.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://tg.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fo.9csxet.cn

Ruby: gets.chomp
来源：http://co.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://bs.newstarts.cn

[A21] 保留指定小数位输出
来源：http://gk.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://wm.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qm.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://pf.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://dw.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://su.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qo.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ug.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://md.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://yz.shxzskj.cn

Py:   len(s)
来源：http://jb.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ee.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://em.panjiajie.cn

TS:   s.length
来源：http://ra.bjjhwx.cn

Java: s.length()
来源：http://xx.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xn.szxytkj.cn

Ruby: s.length
来源：http://au.jianghongdianzi.cn

C#:   s.Length
来源：http://wb.haigaiapp.cn

[A23] 大小写转换
来源：http://fh.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oc.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ca.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gl.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dc.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dg.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wc.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jk.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qi.asd995.cn

[A24] 去除首尾空白
来源：http://eq.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ot.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yc.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yy.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oe.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qj.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://qh.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gi.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hb.9csxet.cn

[A25] 字符串比较
来源：http://iz.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://jm.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mb.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fi.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mi.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gh.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ou.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qd.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dc.huanxung.cn

[A26] 类型转换总览
来源：http://ni.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cy.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cg.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vm.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://bc.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lz.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rv.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://np.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mq.newstarts.cn

================================================================================
来源：http://oh.521024.cn

B. 流程控制
来源：http://eq.yuexingan06.cn

================================================================================
来源：http://pg.panjiajie.cn

[B01] 条件判断 if / else
来源：http://mk.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://va.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rg.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sp.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://da.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dr.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sd.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gu.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ub.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://zz.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jj.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ve.huixiangedu.cn


<!-- 参考信息 -->