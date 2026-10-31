代发 wailian999

================================================================================
来源：http://lf.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://jj.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://fg.asd995.cn

================================================================================
来源：http://cy.shtwfgs.cn

【收录内容】
来源：http://rj.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fr.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://py.newstarts.cn

SQL · Bash · C · C++
来源：http://xj.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rp.newstarts.cn

【使用说明】
来源：http://cy.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ke.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xx.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ou.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cb.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dm.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://br.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gj.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bq.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gb.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xv.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kv.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sn.nszjky.cn

【文件统计】
来源：http://um.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://on.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://bp.lnxyls.cn

目  录
来源：http://hn.szsharing.cn

--------------------------------------------------------------------------------
来源：http://tn.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ds.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ek.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uc.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dw.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ho.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nf.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nz.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hg.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cw.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ek.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yv.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vc.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iq.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rg.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wn.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rv.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xx.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wp.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xz.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lo.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xq.hahajie.cn

================================================================================
来源：http://wu.bjjhwx.cn

A. 基础语法与类型
来源：http://ew.chemitech.net.cn

================================================================================
来源：http://xw.gzmigu.cn

[A01] Hello World
来源：http://go.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://xr.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://jd.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://if.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oe.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://jy.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://lt.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://gm.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vb.colortex.cn

[A02] 变量声明与赋值
来源：http://cg.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cb.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vj.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://er.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kz.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://sd.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://di.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://eg.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bh.huixiangedu.cn

[A03] 常量定义
来源：http://lt.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fc.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://kr.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://un.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://nv.521024.cn

Java: static final double PI = 3.14159;
来源：http://mv.newstarts.cn

Go:   const PI = 3.14159
来源：http://ab.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://zy.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://ka.wgjwhj.cn

[A04] 判断变量类型
来源：http://tb.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vi.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jg.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mi.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://ju.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sh.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pq.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wx.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://eg.9csxet.cn

[A05] 整数除法与取模
来源：http://oi.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mn.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://di.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uq.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ds.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://xv.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://fo.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://dp.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://st.nicolike.cn

[A06] 字符串转数字
来源：http://dw.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://dd.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tp.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ey.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bv.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ml.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tn.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ii.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qx.yuexingan06.cn

[A07] 数字转字符串
来源：http://wf.newstarts.cn

Py:   str(42)
来源：http://jz.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://kn.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://hk.nszjky.cn

TS:   String(42)
来源：http://vl.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wv.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://is.newstarts.cn

Ruby: 42.to_s
来源：http://vd.yuntaijiaju.cn

C#:   42.ToString()
来源：http://mz.9csxet.cn

[A08] 取整与四舍五入
来源：http://ul.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xu.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gu.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sz.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hb.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wp.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://km.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fq.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xb.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://eu.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gm.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jo.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bv.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gz.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ko.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qh.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tq.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kb.shtwfgs.cn

[A10] 生成随机数
来源：http://ja.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://sx.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://mu.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mm.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cm.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://mm.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ze.yuexingan06.cn

Ruby: rand(1..100)
来源：http://kf.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://kk.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://jr.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://cc.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nq.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cp.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oo.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://pt.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jc.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fp.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sp.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://dg.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ze.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mk.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://ao.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://do.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://ks.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ri.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://rq.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://vt.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eh.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://hi.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://ha.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://ol.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://qi.shxzukj.cn

Java: "第一行\n第二行"
来源：http://pu.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://nj.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://fs.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://zo.colortex.cn

[A14] 注释写法
来源：http://uh.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ix.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mq.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://pq.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://wf.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ke.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://dk.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://th.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://dw.newstarts.cn

[A15] 空值判断与默认值
来源：http://ld.szsharing.cn

Py:   value = data or "默认值"
来源：http://kw.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ug.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://mb.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://uq.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uw.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://ut.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://zo.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://gr.newstarts.cn

[A16] 真假值判断规则
来源：http://bc.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ip.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pa.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tn.521024.cn

TS:   if (!x) {}
来源：http://ha.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ty.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vm.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ox.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lf.shxzskj.cn

[A17] 位运算
来源：http://kn.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ke.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ko.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fw.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wk.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cm.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hn.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mc.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://in.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://da.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://cg.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ax.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tf.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://hw.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dp.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://uq.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://it.jctech888.com.cn

[A19] 交换两个变量
来源：http://vr.huanxung.cn

Py:   a, b = b, a
来源：http://wg.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xf.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://lf.colortex.cn

TS:   [a, b] = [b, a];
来源：http://xj.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://ql.shtwfgs.cn

Go:   a, b = b, a
来源：http://vu.nszjky.cn

Ruby: a, b = b, a
来源：http://mn.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://si.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://ll.colortex.cn

Py:   name = input("请输入：")
来源：http://xs.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ae.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yp.asd995.cn

TS:   // Node.js：readline 模块
来源：http://fx.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://nt.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oh.shtwfgs.cn

Ruby: gets.chomp
来源：http://fn.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://hf.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://ar.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://hu.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ad.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://kk.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://bf.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://nz.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bb.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://vh.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://lh.shxzukj.cn

[A22] 获取字符串长度
来源：http://sy.hnjuh.cn

Py:   len(s)
来源：http://pb.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ax.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vd.jctech888.com.cn

TS:   s.length
来源：http://wp.szsharing.cn

Java: s.length()
来源：http://lv.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hk.yuexingan06.cn

Ruby: s.length
来源：http://bx.haigaiapp.cn

C#:   s.Length
来源：http://lh.muxihuayi.cn

[A23] 大小写转换
来源：http://sm.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ao.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dg.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ie.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yf.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kf.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ec.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dd.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ff.colortex.cn

[A24] 去除首尾空白
来源：http://zt.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bc.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vn.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tj.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tv.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pe.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ca.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://en.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bm.szxytkj.cn

[A25] 字符串比较
来源：http://wy.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://fz.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://da.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tg.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ka.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pw.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ts.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bs.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ld.chemitech.net.cn

[A26] 类型转换总览
来源：http://ya.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ce.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://az.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hx.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://en.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ot.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kr.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fs.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nt.szxytkj.cn

================================================================================
来源：http://ij.bjjhwx.cn

B. 流程控制
来源：http://ok.hahajie.cn

================================================================================
来源：http://lk.gzmigu.cn

[B01] 条件判断 if / else
来源：http://md.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wg.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qf.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gv.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hb.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tj.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kl.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mc.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pk.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://of.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pl.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jh.newstarts.cn


<!-- 参考信息 -->