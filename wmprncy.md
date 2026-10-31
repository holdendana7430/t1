代发 wailian999

================================================================================
来源：http://vi.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://qo.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://cc.colortex.cn

================================================================================
来源：http://re.lnxyls.cn

【收录内容】
来源：http://fe.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qx.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ma.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://kk.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ql.521024.cn

【使用说明】
来源：http://cd.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gd.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mn.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yx.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nf.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sy.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ge.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lt.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hm.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://li.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mv.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://od.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jw.huixiangedu.cn

【文件统计】
来源：http://nr.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jh.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://hs.shxzskj.cn

目  录
来源：http://li.nicolike.cn

--------------------------------------------------------------------------------
来源：http://dy.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aa.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tb.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rv.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://in.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ic.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yh.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://za.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fh.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ew.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mf.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://su.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ke.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eo.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://um.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://px.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oi.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ov.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mq.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dk.huixiangedu.cn

================================================================================
来源：http://zw.panjiajie.cn

A. 基础语法与类型
来源：http://ug.szxytkj.cn

================================================================================
来源：http://wh.shxzukj.cn

[A01] Hello World
来源：http://mq.hahajie.cn

Py:   print("Hello, World!")
来源：http://jo.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://mg.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://su.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://et.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://tn.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://xa.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://aq.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eg.gzmigu.cn

[A02] 变量声明与赋值
来源：http://yj.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dq.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://su.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zt.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oj.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://oi.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://hb.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://fy.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hj.bookmarksfly.cn

[A03] 常量定义
来源：http://ib.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yk.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://rr.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://xp.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://zh.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://xp.hahajie.cn

Go:   const PI = 3.14159
来源：http://qs.szxytkj.cn

Ruby: PI = 3.14159
来源：http://pc.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://en.asd995.cn

[A04] 判断变量类型
来源：http://du.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mp.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nb.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://il.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://oo.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oy.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dz.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yf.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://kl.bjjhwx.cn

[A05] 整数除法与取模
来源：http://kr.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dl.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xi.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gq.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ur.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://as.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://de.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://kn.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://cu.shxzukj.cn

[A06] 字符串转数字
来源：http://ks.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://ez.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bn.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pm.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ua.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uk.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://es.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iy.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gi.szsharing.cn

[A07] 数字转字符串
来源：http://fi.521024.cn

Py:   str(42)
来源：http://yx.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://ir.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ds.9csxet.cn

TS:   String(42)
来源：http://yy.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nr.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://ud.yuexingan06.cn

Ruby: 42.to_s
来源：http://ov.huixiangedu.cn

C#:   42.ToString()
来源：http://nw.szxytkj.cn

[A08] 取整与四舍五入
来源：http://mu.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kd.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://af.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kn.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vb.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://et.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zc.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ej.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rk.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://nx.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bc.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ex.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ke.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://by.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tk.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kx.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mb.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://an.gzmigu.cn

[A10] 生成随机数
来源：http://ju.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://ke.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://bi.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sy.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kq.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://xe.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zy.hnjuh.cn

Ruby: rand(1..100)
来源：http://ya.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://aq.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ho.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://gn.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://io.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sm.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ck.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ss.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oh.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qm.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rz.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://fh.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xi.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lp.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://qi.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://it.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://fy.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ro.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://gc.colortex.cn

C#:   $"Hello, {name}!"
来源：http://be.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jq.nszjky.cn

Py:   "第一行\n第二行"
来源：http://cx.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://sy.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://oc.asd995.cn

TS:   "第一行\n第二行"
来源：http://sk.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://wp.hahajie.cn

Go:   "第一行\n第二行"
来源：http://qw.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://mu.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://te.521024.cn

[A14] 注释写法
来源：http://yh.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wu.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://im.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://fr.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://me.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gz.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://ma.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://my.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://eb.panjiajie.cn

[A15] 空值判断与默认值
来源：http://tp.nicolike.cn

Py:   value = data or "默认值"
来源：http://ll.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ty.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://ex.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://mv.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ht.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://dt.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://as.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ju.asd995.cn

[A16] 真假值判断规则
来源：http://mb.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fn.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mq.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zv.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://et.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vn.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mp.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ql.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vi.newstarts.cn

[A17] 位运算
来源：http://tg.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ui.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ez.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ig.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xv.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ia.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pe.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pg.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://qr.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://wm.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://vw.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tn.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kz.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://xy.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eq.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://go.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://qd.shtwfgs.cn

[A19] 交换两个变量
来源：http://ri.bookmarksfly.cn

Py:   a, b = b, a
来源：http://ph.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ws.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ct.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://pi.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://pp.shxzukj.cn

Go:   a, b = b, a
来源：http://uc.szsharing.cn

Ruby: a, b = b, a
来源：http://rc.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://iq.nicolike.cn

[A20] 读取标准输入
来源：http://nr.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://ew.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jc.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gh.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://lz.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://ji.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fk.yuexingan06.cn

Ruby: gets.chomp
来源：http://in.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://vv.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://qp.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://ry.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ss.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://gx.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://ll.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://do.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qv.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://je.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://jh.521024.cn

[A22] 获取字符串长度
来源：http://uu.nszjky.cn

Py:   len(s)
来源：http://cs.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ff.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aw.lnxyls.cn

TS:   s.length
来源：http://pk.panjiajie.cn

Java: s.length()
来源：http://dn.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sv.shxzukj.cn

Ruby: s.length
来源：http://zp.jianghongdianzi.cn

C#:   s.Length
来源：http://ig.huixiangedu.cn

[A23] 大小写转换
来源：http://ic.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mt.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mf.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ir.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jt.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dd.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mh.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gp.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hp.huanxung.cn

[A24] 去除首尾空白
来源：http://vj.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nl.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ci.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wn.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rs.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://ck.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sx.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yy.nicolike.cn

[A25] 字符串比较
来源：http://ve.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://tb.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pt.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mr.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dx.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://so.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fg.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rl.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sc.huixiangedu.cn

[A26] 类型转换总览
来源：http://ya.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oo.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bb.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gq.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://mu.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jo.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://po.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sy.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xe.haigaiapp.cn

================================================================================
来源：http://oo.huixinmuqiang.cn

B. 流程控制
来源：http://cr.huixinmuqiang.cn

================================================================================
来源：http://yx.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://kp.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ak.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qv.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ir.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vh.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hc.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zk.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gs.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://gj.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dw.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fm.9csxet.cn


<!-- 参考信息 -->