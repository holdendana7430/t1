代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lw.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hq.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hb.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oz.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ws.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ec.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vh.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oe.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fq.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://us.huixiangedu.cn

【文件统计】
来源：http://ae.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uk.hahajie.cn

--------------------------------------------------------------------------------
来源：http://rd.szsharing.cn

目  录
来源：http://su.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ff.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iy.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pk.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rt.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kv.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://po.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gs.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eq.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pt.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ae.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jt.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hy.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ki.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rp.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ps.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ig.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zq.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bk.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hl.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xp.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rc.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ck.hahajie.cn

================================================================================
来源：http://sn.jianghongdianzi.cn

A. 基础语法与类型
来源：http://jl.asd995.cn

================================================================================
来源：http://aw.nszjky.cn

[A01] Hello World
来源：http://bi.hahajie.cn

Py:   print("Hello, World!")
来源：http://ne.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://qx.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://xm.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kb.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://su.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://pt.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://yk.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fb.newstarts.cn

[A02] 变量声明与赋值
来源：http://so.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ps.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ln.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xd.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ua.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ij.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://zx.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://xt.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tb.asd995.cn

[A03] 常量定义
来源：http://pj.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ss.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://jz.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://xp.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://hv.asd995.cn

Java: static final double PI = 3.14159;
来源：http://tn.huanxung.cn

Go:   const PI = 3.14159
来源：http://xt.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://qj.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://yt.jctech888.com.cn

[A04] 判断变量类型
来源：http://bl.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wj.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jr.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wh.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://dr.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://he.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ky.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://az.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://hv.wgjwhj.cn

[A05] 整数除法与取模
来源：http://kr.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qt.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xp.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qf.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://la.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://to.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://fc.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://rv.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://xw.huixiangedu.cn

[A06] 字符串转数字
来源：http://hm.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://ep.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xb.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eh.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yo.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qp.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mk.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ee.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bd.panjiajie.cn

[A07] 数字转字符串
来源：http://xu.nszjky.cn

Py:   str(42)
来源：http://cu.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://hh.521024.cn

JS:   String(42); (42).toString()
来源：http://rt.colortex.cn

TS:   String(42)
来源：http://wg.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dz.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://mq.nicolike.cn

Ruby: 42.to_s
来源：http://ec.colortex.cn

C#:   42.ToString()
来源：http://de.shxzskj.cn

[A08] 取整与四舍五入
来源：http://ef.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nz.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wn.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kr.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kx.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jd.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qj.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ih.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wp.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://gj.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pt.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eq.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ym.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://po.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qn.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ck.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dq.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gd.lnxyls.cn

[A10] 生成随机数
来源：http://uq.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://hv.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://xn.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ra.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://an.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ah.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lp.muxihuayi.cn

Ruby: rand(1..100)
来源：http://ge.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://nn.colortex.cn

[A11] 条件表达式（三元）
来源：http://tc.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ga.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xd.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rc.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hy.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://jv.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vd.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zn.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yh.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://ji.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ie.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bl.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://my.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://za.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://lr.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mk.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://ru.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://yl.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oi.521024.cn

Py:   "第一行\n第二行"
来源：http://vz.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://ey.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://xj.huanxung.cn

TS:   "第一行\n第二行"
来源：http://zu.shxzskj.cn

Java: "第一行\n第二行"
来源：http://bw.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://yi.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://ik.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://av.huixiangedu.cn

[A14] 注释写法
来源：http://gb.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://or.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bn.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://hi.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://vj.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ri.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://ki.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uw.521024.cn

C#:   // 单行；/* 多行 */
来源：http://us.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://ae.9csxet.cn

Py:   value = data or "默认值"
来源：http://ko.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://mw.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://mm.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://pm.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fu.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://ga.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://fg.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://jt.asd995.cn

[A16] 真假值判断规则
来源：http://yc.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://km.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xc.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vx.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://ns.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ni.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mj.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://da.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tl.shxzskj.cn

[A17] 位运算
来源：http://dl.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nu.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vc.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uf.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bb.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rh.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://km.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://by.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://rb.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://op.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nq.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://gk.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hn.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ni.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://nn.shxzskj.cn

[A19] 交换两个变量
来源：http://dj.bjjhwx.cn

Py:   a, b = b, a
来源：http://bv.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bv.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://gv.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://cu.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://ae.nszjky.cn

Go:   a, b = b, a
来源：http://hv.szxytkj.cn

Ruby: a, b = b, a
来源：http://iy.521024.cn

C#:   (a, b) = (b, a);
来源：http://cs.shxzukj.cn

[A20] 读取标准输入
来源：http://gn.gzmigu.cn

Py:   name = input("请输入：")
来源：http://gp.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ml.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ga.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://rf.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://nx.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lp.newstarts.cn

Ruby: gets.chomp
来源：http://gv.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://zy.newstarts.cn

[A21] 保留指定小数位输出
来源：http://ol.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://ig.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pg.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ea.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://xo.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://jc.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gi.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://kb.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://lt.szxytkj.cn

[A22] 获取字符串长度
来源：http://xh.jctech888.com.cn

Py:   len(s)
来源：http://kq.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yk.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yv.asd995.cn

TS:   s.length
来源：http://tz.nszjky.cn

Java: s.length()
来源：http://uz.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yd.9csxet.cn

Ruby: s.length
来源：http://ac.9csxet.cn

C#:   s.Length
来源：http://zy.muxihuayi.cn

[A23] 大小写转换
来源：http://qf.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eu.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hq.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://db.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dj.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zi.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ct.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ft.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://an.shxzskj.cn

[A24] 去除首尾空白
来源：http://sg.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hy.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sx.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rp.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nf.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iv.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://ic.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gb.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xs.521024.cn

[A25] 字符串比较
来源：http://kf.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://an.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ct.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fk.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yd.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://it.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cz.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ih.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.shxzskj.cn

[A26] 类型转换总览
来源：http://za.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xy.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ov.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wb.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://zd.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vm.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://np.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nt.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lx.9csxet.cn

================================================================================
来源：http://ej.shxzskj.cn

B. 流程控制
来源：http://ki.shxzskj.cn

================================================================================
来源：http://ji.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://mu.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pa.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sv.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ia.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fp.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uo.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xj.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ao.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://zq.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://di.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mc.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nk.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fb.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fj.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ex.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vy.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.panjiajie.cn

[B03] switch / match / case
来源：http://xs.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kj.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ki.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ll.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vs.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cm.jianghongdianzi.cn


<!-- 参考信息 -->