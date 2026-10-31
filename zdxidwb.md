代发 wailian999

================================================================================
来源：http://tt.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ld.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://nt.hnjuh.cn

================================================================================
来源：http://bk.jctech888.com.cn

【收录内容】
来源：http://mu.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iz.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://us.asd995.cn

SQL · Bash · C · C++
来源：http://ah.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wy.nszjky.cn

【使用说明】
来源：http://wy.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ni.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ik.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fc.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://td.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wx.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ib.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fm.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lo.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uu.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sb.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yn.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ly.panjiajie.cn

【文件统计】
来源：http://xe.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cd.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://fd.yuexingan06.cn

目  录
来源：http://pn.asd995.cn

--------------------------------------------------------------------------------
来源：http://mp.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ue.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ai.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gf.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kf.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ts.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wl.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vm.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://az.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qd.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pn.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ww.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oa.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qh.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mo.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lt.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qh.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://su.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bm.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eb.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tx.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qa.nszjky.cn

================================================================================
来源：http://el.bookmarksfly.cn

A. 基础语法与类型
来源：http://yc.gzmigu.cn

================================================================================
来源：http://ge.asd995.cn

[A01] Hello World
来源：http://tx.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://mh.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://pd.asd995.cn

JS:   console.log("Hello, World!");
来源：http://rh.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iy.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://cd.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://hx.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://bi.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iq.shxzskj.cn

[A02] 变量声明与赋值
来源：http://jf.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jg.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dg.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rk.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zn.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://rr.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://pb.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://rl.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zn.9csxet.cn

[A03] 常量定义
来源：http://jg.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ko.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://up.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://wi.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://fx.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://gw.huanxung.cn

Go:   const PI = 3.14159
来源：http://eu.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://cf.colortex.cn

C#:   const double PI = 3.14159;
来源：http://et.521024.cn

[A04] 判断变量类型
来源：http://bi.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://om.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ij.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nm.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://pd.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dj.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lm.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qh.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://ce.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://mr.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pr.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uw.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ab.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://of.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://gd.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://zw.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://hv.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://yo.wgjwhj.cn

[A06] 字符串转数字
来源：http://cu.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://br.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qv.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gp.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yx.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sk.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qt.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://se.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oa.nszjky.cn

[A07] 数字转字符串
来源：http://mx.szsharing.cn

Py:   str(42)
来源：http://do.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://jd.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://pu.newstarts.cn

TS:   String(42)
来源：http://aa.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gn.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://wk.wgjwhj.cn

Ruby: 42.to_s
来源：http://sm.jianghongdianzi.cn

C#:   42.ToString()
来源：http://xz.shxzskj.cn

[A08] 取整与四舍五入
来源：http://wp.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tf.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jb.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dz.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gu.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wr.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gv.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fg.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kd.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://sx.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://my.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xr.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hk.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tc.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ff.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://of.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ea.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mc.huixiangedu.cn

[A10] 生成随机数
来源：http://tq.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ct.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://mp.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wg.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vf.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://du.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pk.lnxyls.cn

Ruby: rand(1..100)
来源：http://oq.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://dm.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://sd.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://fn.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vh.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nb.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xm.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ia.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zq.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://el.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dt.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://bm.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cj.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://db.521024.cn

JS:   `Hello, ${name}!`
来源：http://nq.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://ih.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://sn.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uh.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://uq.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://xr.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tr.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://aj.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://eo.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://cd.asd995.cn

TS:   "第一行\n第二行"
来源：http://el.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ey.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://an.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://lo.newstarts.cn

C#:   "第一行\n第二行"
来源：http://ec.bookmarksfly.cn

[A14] 注释写法
来源：http://dx.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bb.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pe.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://kz.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://aq.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zl.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://dq.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zz.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://su.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://je.521024.cn

Py:   value = data or "默认值"
来源：http://be.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://kj.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://kp.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://ri.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tx.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://vy.szsharing.cn

Ruby: value = data || "默认值"
来源：http://du.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://zd.huixiangedu.cn

[A16] 真假值判断规则
来源：http://do.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zx.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://op.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wj.shxzskj.cn

TS:   if (!x) {}
来源：http://oq.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lj.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zo.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gd.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kt.521024.cn

[A17] 位运算
来源：http://wc.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://io.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dn.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iv.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sa.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://uw.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://rl.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ky.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ke.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ln.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://uy.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hg.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://zs.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://fi.hnjuh.cn

[A19] 交换两个变量
来源：http://ya.wgjwhj.cn

Py:   a, b = b, a
来源：http://jl.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://no.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://df.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://gp.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://lr.shxzskj.cn

Go:   a, b = b, a
来源：http://ql.shxzukj.cn

Ruby: a, b = b, a
来源：http://vk.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://xl.bjjhwx.cn

[A20] 读取标准输入
来源：http://im.hnjuh.cn

Py:   name = input("请输入：")
来源：http://fb.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://he.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rm.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://dk.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://ej.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rp.nicolike.cn

Ruby: gets.chomp
来源：http://zf.gzmigu.cn

C#:   Console.ReadLine();
来源：http://fc.9csxet.cn

[A21] 保留指定小数位输出
来源：http://vs.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://ve.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ma.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ds.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ps.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ou.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fg.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://po.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://wu.colortex.cn

[A22] 获取字符串长度
来源：http://vc.bjjhwx.cn

Py:   len(s)
来源：http://gh.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xz.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qn.lnxyls.cn

TS:   s.length
来源：http://wk.9csxet.cn

Java: s.length()
来源：http://vj.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ta.hahajie.cn

Ruby: s.length
来源：http://xo.haigaiapp.cn

C#:   s.Length
来源：http://bo.shxzukj.cn

[A23] 大小写转换
来源：http://ht.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yx.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eb.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rw.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hv.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://my.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yc.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vm.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rk.hahajie.cn

[A24] 去除首尾空白
来源：http://uy.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jb.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xt.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qf.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eh.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xh.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ef.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://en.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pq.huixiangedu.cn

[A25] 字符串比较
来源：http://fd.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://tf.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://as.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hl.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zd.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xy.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yh.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mx.521024.cn

[A26] 类型转换总览
来源：http://lt.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vz.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rp.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ou.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://jn.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://un.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rg.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bw.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mc.huixiangedu.cn

================================================================================
来源：http://xk.szxytkj.cn

B. 流程控制
来源：http://qk.shtwfgs.cn

================================================================================
来源：http://mu.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://we.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yz.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://td.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ll.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://er.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lx.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jr.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yi.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ax.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://px.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zy.shxzukj.cn


<!-- 参考信息 -->