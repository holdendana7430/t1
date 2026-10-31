代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tc.gzmigu.cn

【使用说明】
来源：http://sj.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xq.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qe.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dk.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://br.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vk.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zn.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://us.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bv.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ha.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cy.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ul.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://il.huixiangedu.cn

【文件统计】
来源：http://nu.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yo.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://mf.yuexingan06.cn

目  录
来源：http://ec.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://cx.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wh.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eh.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ru.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ja.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qc.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tv.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://km.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hm.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jn.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://li.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ym.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://af.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kn.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ia.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tz.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jl.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ck.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ye.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ai.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lw.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hj.gzmigu.cn

================================================================================
来源：http://qs.huixinmuqiang.cn

A. 基础语法与类型
来源：http://bx.asd995.cn

================================================================================
来源：http://wv.521024.cn

[A01] Hello World
来源：http://ze.nicolike.cn

Py:   print("Hello, World!")
来源：http://aq.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://xi.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://fy.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yw.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://yb.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://kx.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://nw.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jj.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://cx.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rf.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://le.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ex.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jf.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://di.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://gm.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://pb.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ie.muxihuayi.cn

[A03] 常量定义
来源：http://od.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://im.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://nq.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://za.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://dn.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://tp.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://ao.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://lm.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://yn.nicolike.cn

[A04] 判断变量类型
来源：http://wh.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://au.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vo.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zd.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://nx.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tg.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vc.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vl.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://mu.nicolike.cn

[A05] 整数除法与取模
来源：http://lq.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nu.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://de.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zz.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mh.521024.cn

Java: 7 / 2; 7 % 2
来源：http://mf.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://um.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://be.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://jz.colortex.cn

[A06] 字符串转数字
来源：http://om.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://wu.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uf.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rv.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xl.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gd.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://us.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jq.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bm.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://ws.huixiangedu.cn

Py:   str(42)
来源：http://uk.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://ns.hahajie.cn

JS:   String(42); (42).toString()
来源：http://pu.gzmigu.cn

TS:   String(42)
来源：http://rj.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://im.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://nt.shxzukj.cn

Ruby: 42.to_s
来源：http://sd.nszjky.cn

C#:   42.ToString()
来源：http://gr.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://mg.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xj.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vp.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kt.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ua.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ex.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://no.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fa.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sx.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://xn.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lf.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ij.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ay.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fo.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rn.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hw.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qr.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mx.521024.cn

[A10] 生成随机数
来源：http://jr.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://iu.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://mx.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pw.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://nx.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dm.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://es.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://as.521024.cn

[A11] 条件表达式（三元）
来源：http://se.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://wb.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ym.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eq.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sj.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://oq.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ml.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jk.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cy.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://vt.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ni.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://th.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://rt.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://jk.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://hz.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iv.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://yk.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://ej.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qv.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://ox.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://le.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://ej.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://za.hnjuh.cn

Java: "第一行\n第二行"
来源：http://pe.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://db.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://fc.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://pe.shxzukj.cn

[A14] 注释写法
来源：http://nn.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://in.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://on.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://tf.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://nn.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rq.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://pf.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dz.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://aj.hnjuh.cn

[A15] 空值判断与默认值
来源：http://ga.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://gr.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://tr.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://nz.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://rc.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://de.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://iy.nicolike.cn

Ruby: value = data || "默认值"
来源：http://ta.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://oz.szxytkj.cn

[A16] 真假值判断规则
来源：http://nf.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tr.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kj.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ug.newstarts.cn

TS:   if (!x) {}
来源：http://br.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ag.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wk.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ir.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hj.muxihuayi.cn

[A17] 位运算
来源：http://bz.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wi.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uc.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ix.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pu.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ib.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://op.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://yq.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://dh.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://pp.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://en.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qv.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://lm.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gx.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://lg.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://fr.jctech888.com.cn

[A19] 交换两个变量
来源：http://vg.gzmigu.cn

Py:   a, b = b, a
来源：http://vz.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ny.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://ki.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://ao.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://vr.bjjhwx.cn

Go:   a, b = b, a
来源：http://kx.nszjky.cn

Ruby: a, b = b, a
来源：http://zx.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://zj.shtwfgs.cn

[A20] 读取标准输入
来源：http://ie.gzmigu.cn

Py:   name = input("请输入：")
来源：http://oo.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tl.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xw.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://dr.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://oy.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ye.szxytkj.cn

Ruby: gets.chomp
来源：http://zg.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://vm.hahajie.cn

[A21] 保留指定小数位输出
来源：http://tg.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://ia.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gs.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://wm.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://nh.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://zn.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sf.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://tt.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://fs.muxihuayi.cn

[A22] 获取字符串长度
来源：http://lx.bjjhwx.cn

Py:   len(s)
来源：http://tq.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mp.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://do.chemitech.net.cn

TS:   s.length
来源：http://zf.panjiajie.cn

Java: s.length()
来源：http://ht.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ve.colortex.cn

Ruby: s.length
来源：http://qr.nicolike.cn

C#:   s.Length
来源：http://vc.newstarts.cn

[A23] 大小写转换
来源：http://gy.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ad.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yq.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://if.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cb.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zy.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nr.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lr.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mm.9csxet.cn

[A24] 去除首尾空白
来源：http://bf.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sf.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xl.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yz.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mz.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cq.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://pc.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rj.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xy.9csxet.cn

[A25] 字符串比较
来源：http://yg.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://wy.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://og.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cv.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cq.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qa.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ke.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hi.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ex.szsharing.cn

[A26] 类型转换总览
来源：http://zf.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lk.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xr.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lj.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://sw.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://se.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fy.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ak.hahajie.cn

================================================================================
来源：http://ke.hahajie.cn

B. 流程控制
来源：http://pt.wgjwhj.cn

================================================================================
来源：http://hl.szsharing.cn

[B01] 条件判断 if / else
来源：http://uj.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gx.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ak.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://os.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ox.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fe.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bz.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rf.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zj.szsharing.cn

[B02] 多分支 else if / elif
来源：http://rb.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hx.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ee.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ak.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gb.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jc.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bm.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.shxzskj.cn

[B03] switch / match / case
来源：http://vr.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wi.panjiajie.cn


<!-- 参考信息 -->