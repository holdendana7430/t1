代发 wailian999

================================================================================
来源：http://ek.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://uw.colortex.cn

Common Programming Examples Cheat Book
来源：http://jv.szsharing.cn

================================================================================
来源：http://uf.haigaiapp.cn

【收录内容】
来源：http://vd.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bi.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rw.huanxung.cn

SQL · Bash · C · C++
来源：http://ht.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gt.hahajie.cn

【使用说明】
来源：http://rm.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jd.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zh.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bi.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ty.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://js.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://av.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ru.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pa.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dc.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qw.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wh.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://te.9csxet.cn

【文件统计】
来源：http://el.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://or.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ou.szxytkj.cn

目  录
来源：http://nm.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://do.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kn.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qz.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tv.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ik.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oj.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pm.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://to.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fw.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ve.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gl.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uz.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fm.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hc.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://od.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tg.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ko.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nm.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wt.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ct.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://et.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tk.haigaiapp.cn

================================================================================
来源：http://lh.asd995.cn

A. 基础语法与类型
来源：http://nw.wgjwhj.cn

================================================================================
来源：http://iz.nicolike.cn

[A01] Hello World
来源：http://nz.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://qs.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://sv.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://vw.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yq.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://hh.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://zn.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://py.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dy.gzmigu.cn

[A02] 变量声明与赋值
来源：http://gb.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nw.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ew.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wl.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ep.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://rg.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://aq.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://pk.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hl.colortex.cn

[A03] 常量定义
来源：http://sb.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mx.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://su.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://sb.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://so.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://wq.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://hn.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://pl.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://dg.wgjwhj.cn

[A04] 判断变量类型
来源：http://xn.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gc.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mg.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sr.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://ql.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bd.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dk.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cj.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://su.shtwfgs.cn

[A05] 整数除法与取模
来源：http://cb.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hl.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zk.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://if.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ws.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://fg.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://ne.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://dw.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://kn.colortex.cn

[A06] 字符串转数字
来源：http://kg.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://sc.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bx.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://db.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zi.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ty.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://un.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yf.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dq.panjiajie.cn

[A07] 数字转字符串
来源：http://qc.bjjhwx.cn

Py:   str(42)
来源：http://cd.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://uz.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://jh.lnxyls.cn

TS:   String(42)
来源：http://pk.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xh.colortex.cn

Go:   strconv.Itoa(42)
来源：http://ik.asd995.cn

Ruby: 42.to_s
来源：http://zo.hahajie.cn

C#:   42.ToString()
来源：http://ok.gzmigu.cn

[A08] 取整与四舍五入
来源：http://bz.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hq.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://na.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ye.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bs.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vh.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://du.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cw.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pp.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://hh.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://te.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uq.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sa.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ap.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yu.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://av.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qq.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tn.wgjwhj.cn

[A10] 生成随机数
来源：http://mg.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://pb.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://ug.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cc.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xs.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://rp.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cv.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://vx.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://pt.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://cf.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://vg.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jj.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hx.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lr.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://gs.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nx.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yb.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jv.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://ct.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yj.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zr.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://bl.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://xp.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://sc.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vb.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://wa.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://zf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rd.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://px.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://am.newstarts.cn

JS:   "第一行\n第二行"
来源：http://nf.9csxet.cn

TS:   "第一行\n第二行"
来源：http://zx.nszjky.cn

Java: "第一行\n第二行"
来源：http://rt.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://bt.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://ma.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://av.muxihuayi.cn

[A14] 注释写法
来源：http://id.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lg.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rv.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ec.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://kp.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dw.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://hn.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ty.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://hl.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://dn.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://jk.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://yu.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://at.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://lv.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ym.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://jn.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://wh.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://sl.hahajie.cn

[A16] 真假值判断规则
来源：http://ep.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://he.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cv.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nz.hnjuh.cn

TS:   if (!x) {}
来源：http://jl.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oq.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qv.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nv.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jb.yuntaijiaju.cn

[A17] 位运算
来源：http://cq.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xg.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zx.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ca.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lk.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://za.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cg.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://dg.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://ix.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://sk.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gz.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dh.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://mh.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xz.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://uz.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://ds.huixiangedu.cn

[A19] 交换两个变量
来源：http://zs.haigaiapp.cn

Py:   a, b = b, a
来源：http://pj.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ix.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://ep.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://kl.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://sw.panjiajie.cn

Go:   a, b = b, a
来源：http://wb.colortex.cn

Ruby: a, b = b, a
来源：http://yy.asd995.cn

C#:   (a, b) = (b, a);
来源：http://wn.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://yz.panjiajie.cn

Py:   name = input("请输入：")
来源：http://eg.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xy.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ms.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://ol.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://bu.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mq.yuexingan06.cn

Ruby: gets.chomp
来源：http://zu.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://tc.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://qk.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://da.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hn.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://fm.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://sl.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://up.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tl.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://hf.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ll.hnjuh.cn

[A22] 获取字符串长度
来源：http://kw.huanxung.cn

Py:   len(s)
来源：http://ul.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nk.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://np.huanxung.cn

TS:   s.length
来源：http://gk.shtwfgs.cn

Java: s.length()
来源：http://rf.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nb.panjiajie.cn

Ruby: s.length
来源：http://vg.nicolike.cn

C#:   s.Length
来源：http://ve.shtwfgs.cn

[A23] 大小写转换
来源：http://sk.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ym.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://db.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lt.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://if.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wb.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gn.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ah.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qa.nicolike.cn

[A24] 去除首尾空白
来源：http://st.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yn.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wr.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yr.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kd.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sa.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://wk.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yz.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yv.newstarts.cn

[A25] 字符串比较
来源：http://qd.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://wx.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qo.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ga.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ik.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ba.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bv.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ad.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ob.yuexingan06.cn

[A26] 类型转换总览
来源：http://hu.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dd.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ya.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gf.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://md.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uq.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yd.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gt.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hw.shxzskj.cn

================================================================================
来源：http://dr.szxytkj.cn

B. 流程控制
来源：http://cd.bookmarksfly.cn

================================================================================
来源：http://ee.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ht.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cv.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://av.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ai.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jt.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sn.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ot.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ri.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lw.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://ci.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://od.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://te.huanxung.cn


<!-- 参考信息 -->