代发 wailian999

================================================================================
来源：http://vz.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://lq.asd995.cn

Common Programming Examples Cheat Book
来源：http://ow.shxzukj.cn

================================================================================
来源：http://tk.huanxung.cn

【收录内容】
来源：http://bh.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yw.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mn.hahajie.cn

SQL · Bash · C · C++
来源：http://gr.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eb.hnjuh.cn

【使用说明】
来源：http://mp.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qs.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nh.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://js.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wr.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wb.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lh.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wi.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ir.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ce.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zo.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://id.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vg.jctech888.com.cn

【文件统计】
来源：http://np.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zu.huanxung.cn

--------------------------------------------------------------------------------
来源：http://iv.huixinmuqiang.cn

目  录
来源：http://md.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://fj.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fs.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ab.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bm.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rh.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ut.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rw.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ag.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ad.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ye.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ug.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hj.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ks.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qt.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oy.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lm.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gw.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vf.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uw.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ee.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tp.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cq.haigaiapp.cn

================================================================================
来源：http://yr.asd995.cn

A. 基础语法与类型
来源：http://nz.shxzukj.cn

================================================================================
来源：http://ye.shxzskj.cn

[A01] Hello World
来源：http://di.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://ma.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://gl.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://gp.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://du.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://kh.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ap.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://tl.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ky.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://sn.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bs.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://db.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wy.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vv.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://mz.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://js.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://rh.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://he.haigaiapp.cn

[A03] 常量定义
来源：http://dz.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rj.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://pu.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ve.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://ya.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://qv.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://hx.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://gp.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://cu.jctech888.com.cn

[A04] 判断变量类型
来源：http://se.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uu.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gc.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pb.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://ez.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://de.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://we.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ul.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://hs.lnxyls.cn

[A05] 整数除法与取模
来源：http://uo.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ih.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lz.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bx.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rb.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://ik.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://nl.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ad.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://kg.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://xd.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://ep.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jq.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jr.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cm.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gl.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ve.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bd.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rg.wgjwhj.cn

[A07] 数字转字符串
来源：http://ne.hahajie.cn

Py:   str(42)
来源：http://wr.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://iw.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://lm.panjiajie.cn

TS:   String(42)
来源：http://kz.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hc.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://iz.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://bu.shxzskj.cn

C#:   42.ToString()
来源：http://tu.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://zm.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://md.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eo.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xm.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fy.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xe.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pa.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xc.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lt.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://zo.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gh.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gw.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lk.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iv.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ck.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iu.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://se.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oj.shxzskj.cn

[A10] 生成随机数
来源：http://cw.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://gs.nszjky.cn

PHP:  random_int(1, 100);
来源：http://tc.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://by.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ro.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://ad.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ut.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://np.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://kj.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://gz.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://yt.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wl.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vs.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bo.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://jh.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cw.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sm.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nn.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://qs.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wy.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wm.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://bi.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ov.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://yi.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zk.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://tq.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://dv.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jq.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://lb.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://lo.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://ks.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://cv.gzmigu.cn

Java: "第一行\n第二行"
来源：http://hj.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://in.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://zy.nszjky.cn

C#:   "第一行\n第二行"
来源：http://gg.521024.cn

[A14] 注释写法
来源：http://lp.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ka.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://aa.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://lj.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://mj.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ez.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://cp.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sc.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://yc.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ym.lnxyls.cn

Py:   value = data or "默认值"
来源：http://rb.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://my.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://fb.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://hr.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gv.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://fo.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://ve.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://ft.wgjwhj.cn

[A16] 真假值判断规则
来源：http://sr.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bv.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zc.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jy.huixiangedu.cn

TS:   if (!x) {}
来源：http://ys.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oy.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vv.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ga.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ya.asd995.cn

[A17] 位运算
来源：http://ry.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://el.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uf.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://op.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bv.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ye.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iv.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://hs.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://ia.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://ai.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bx.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://qp.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vm.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://sk.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://jo.huanxung.cn

[A19] 交换两个变量
来源：http://zd.bookmarksfly.cn

Py:   a, b = b, a
来源：http://hh.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zc.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://yy.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ee.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ci.haigaiapp.cn

Go:   a, b = b, a
来源：http://rz.haigaiapp.cn

Ruby: a, b = b, a
来源：http://dw.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://qk.bjjhwx.cn

[A20] 读取标准输入
来源：http://ok.colortex.cn

Py:   name = input("请输入：")
来源：http://mh.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pv.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kt.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://vc.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://md.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bm.jctech888.com.cn

Ruby: gets.chomp
来源：http://wj.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://ha.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ie.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://cv.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ow.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://du.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ya.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://qs.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://na.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ru.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://bx.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://iq.hahajie.cn

Py:   len(s)
来源：http://sq.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qj.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rn.9csxet.cn

TS:   s.length
来源：http://cn.nszjky.cn

Java: s.length()
来源：http://gw.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nt.jctech888.com.cn

Ruby: s.length
来源：http://cw.lnxyls.cn

C#:   s.Length
来源：http://lj.bjjhwx.cn

[A23] 大小写转换
来源：http://ec.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hd.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pz.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://om.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xp.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dd.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ce.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mt.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rp.huixiangedu.cn

[A24] 去除首尾空白
来源：http://jp.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fh.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ph.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ey.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eu.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rq.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://sm.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hy.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gn.yuntaijiaju.cn

[A25] 字符串比较
来源：http://ft.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://pd.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nu.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qu.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tx.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yw.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sw.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jb.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vv.szxytkj.cn

[A26] 类型转换总览
来源：http://ij.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xe.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xz.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sb.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://ke.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uo.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nu.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dl.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://df.521024.cn

================================================================================
来源：http://ss.nszjky.cn

B. 流程控制
来源：http://ak.lnxyls.cn

================================================================================
来源：http://jt.huanxung.cn

[B01] 条件判断 if / else
来源：http://zr.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gd.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fz.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ft.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hn.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cb.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xt.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pr.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://if.huanxung.cn

[B02] 多分支 else if / elif
来源：http://jw.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wq.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ev.wgjwhj.cn


<!-- 参考信息 -->