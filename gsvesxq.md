代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://de.gzmigu.cn

【使用说明】
来源：http://bo.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dl.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ay.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nm.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uo.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xi.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pz.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sz.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kl.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://of.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ny.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dv.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dx.jctech888.com.cn

【文件统计】
来源：http://ax.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sm.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://pi.panjiajie.cn

目  录
来源：http://jc.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://sb.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://em.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bh.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nc.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mi.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nd.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lh.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fc.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://an.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xq.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://se.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gh.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ed.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bq.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fp.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cj.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gn.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lu.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ds.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xk.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://si.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qh.nicolike.cn

================================================================================
来源：http://kc.panjiajie.cn

A. 基础语法与类型
来源：http://ln.bookmarksfly.cn

================================================================================
来源：http://ew.shxzukj.cn

[A01] Hello World
来源：http://jr.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ee.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://cu.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://ho.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rd.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://tp.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://yk.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://xe.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fm.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://yw.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://as.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dt.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qm.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://os.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://wo.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://cf.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://tr.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hy.521024.cn

[A03] 常量定义
来源：http://kq.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cy.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://py.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://pd.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://wq.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://xw.colortex.cn

Go:   const PI = 3.14159
来源：http://nk.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://cb.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://ik.gzmigu.cn

[A04] 判断变量类型
来源：http://ho.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://je.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rh.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pe.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://jd.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lw.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ic.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dt.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://vw.newstarts.cn

[A05] 整数除法与取模
来源：http://ki.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zi.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qa.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tl.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ku.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://rc.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://os.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://yz.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://lu.huanxung.cn

[A06] 字符串转数字
来源：http://dp.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://tj.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xh.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bz.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zb.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://be.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lz.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xo.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zh.huanxung.cn

[A07] 数字转字符串
来源：http://yi.chemitech.net.cn

Py:   str(42)
来源：http://mn.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://rc.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://es.gzmigu.cn

TS:   String(42)
来源：http://ae.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nq.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://eb.lnxyls.cn

Ruby: 42.to_s
来源：http://xc.hnjuh.cn

C#:   42.ToString()
来源：http://wk.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://hq.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zp.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sd.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oq.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lf.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zq.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ys.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sp.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://de.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://an.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sp.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tt.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://co.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://my.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xi.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xg.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rr.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vw.shxzukj.cn

[A10] 生成随机数
来源：http://ps.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://du.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://xv.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ll.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://la.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://vx.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pi.newstarts.cn

Ruby: rand(1..100)
来源：http://ye.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://ve.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ax.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://vf.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xs.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nu.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dk.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://vx.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ce.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pb.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sx.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://qz.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ls.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kz.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://fj.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://hh.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://yy.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bc.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://gq.asd995.cn

C#:   $"Hello, {name}!"
来源：http://qg.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wk.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://fv.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://bt.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://xa.hahajie.cn

TS:   "第一行\n第二行"
来源：http://ld.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ex.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://hp.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://mp.asd995.cn

C#:   "第一行\n第二行"
来源：http://zj.nszjky.cn

[A14] 注释写法
来源：http://ff.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wx.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ft.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://yd.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://rv.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vu.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://tm.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hd.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://ee.nicolike.cn

[A15] 空值判断与默认值
来源：http://aq.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://mm.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://hp.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://yc.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://mm.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://az.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://sq.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://ev.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://hn.nicolike.cn

[A16] 真假值判断规则
来源：http://ga.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fb.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lw.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vg.bookmarksfly.cn

TS:   if (!x) {}
来源：http://wp.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hv.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nq.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xn.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qe.shtwfgs.cn

[A17] 位运算
来源：http://ka.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wd.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rv.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fs.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kt.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kv.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fk.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://tu.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://td.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://gz.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zo.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uu.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ax.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ds.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://sr.asd995.cn

C#:   (int)'A'; (char)65
来源：http://hu.yuexingan06.cn

[A19] 交换两个变量
来源：http://xo.szsharing.cn

Py:   a, b = b, a
来源：http://qa.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cg.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://gs.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://in.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://mr.szsharing.cn

Go:   a, b = b, a
来源：http://lp.chemitech.net.cn

Ruby: a, b = b, a
来源：http://yf.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://cy.yuexingan06.cn

[A20] 读取标准输入
来源：http://ez.newstarts.cn

Py:   name = input("请输入：")
来源：http://iw.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ia.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oe.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://qn.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://yp.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sf.yuexingan06.cn

Ruby: gets.chomp
来源：http://zr.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ci.szsharing.cn

[A21] 保留指定小数位输出
来源：http://om.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://yn.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xv.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://th.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://vw.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://vg.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ov.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://vn.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://nx.muxihuayi.cn

[A22] 获取字符串长度
来源：http://ms.jctech888.com.cn

Py:   len(s)
来源：http://bw.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eo.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fh.jianghongdianzi.cn

TS:   s.length
来源：http://ae.nicolike.cn

Java: s.length()
来源：http://xp.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qd.huixiangedu.cn

Ruby: s.length
来源：http://wa.huixinmuqiang.cn

C#:   s.Length
来源：http://fq.yuexingan06.cn

[A23] 大小写转换
来源：http://sf.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dc.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zo.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gd.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bh.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wg.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://br.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vj.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uz.nszjky.cn

[A24] 去除首尾空白
来源：http://ab.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hn.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ht.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pz.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rv.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bl.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://xq.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eq.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gg.haigaiapp.cn

[A25] 字符串比较
来源：http://tp.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://fm.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://id.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ov.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nh.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lv.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://er.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kt.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rz.yuexingan06.cn

[A26] 类型转换总览
来源：http://ev.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yi.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nw.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bf.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://ni.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rs.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fg.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iw.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ba.szxytkj.cn

================================================================================
来源：http://qk.nicolike.cn

B. 流程控制
来源：http://rp.hahajie.cn

================================================================================
来源：http://bk.shxzukj.cn

[B01] 条件判断 if / else
来源：http://px.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ck.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vp.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tt.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://li.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xs.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lb.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ui.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fh.nszjky.cn

[B02] 多分支 else if / elif
来源：http://xz.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pp.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://te.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://av.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ex.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bt.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.shtwfgs.cn

[B03] switch / match / case
来源：http://db.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pi.asd995.cn


<!-- 参考信息 -->