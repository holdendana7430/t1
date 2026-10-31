代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cl.nicolike.cn

【使用说明】
来源：http://it.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ts.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mb.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gf.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dz.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gg.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://at.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ov.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ph.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pg.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://at.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yx.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://il.huixiangedu.cn

【文件统计】
来源：http://gs.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yd.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://xa.shxzukj.cn

目  录
来源：http://oc.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xc.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ec.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ch.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mz.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vt.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vv.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uu.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mw.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://de.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jp.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ke.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ua.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bp.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vi.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fn.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yt.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kc.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xh.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sd.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yy.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xh.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sm.panjiajie.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

A. 基础语法与类型
来源：http://yl.lnxyls.cn

================================================================================
来源：http://va.yuexingan06.cn

[A01] Hello World
来源：http://ot.lnxyls.cn

Py:   print("Hello, World!")
来源：http://tf.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://eu.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://fi.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yg.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://do.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://bm.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://ne.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mr.nszjky.cn

[A02] 变量声明与赋值
来源：http://by.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qv.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cb.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iv.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sd.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://rd.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://bj.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://kr.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ut.shtwfgs.cn

[A03] 常量定义
来源：http://ik.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bb.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://xy.521024.cn

JS:   const PI = 3.14159;
来源：http://iy.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://zh.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://tq.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://sb.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://ak.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://kq.9csxet.cn

[A04] 判断变量类型
来源：http://ma.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mr.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qh.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ln.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://ey.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://po.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sc.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uu.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://kw.newstarts.cn

[A05] 整数除法与取模
来源：http://ul.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ta.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lt.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wq.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ri.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://pf.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://de.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://xo.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://qy.gzmigu.cn

[A06] 字符串转数字
来源：http://re.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://pd.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wa.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cl.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nt.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cy.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ne.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ud.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tj.panjiajie.cn

[A07] 数字转字符串
来源：http://kc.jianghongdianzi.cn

Py:   str(42)
来源：http://mp.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://pt.huanxung.cn

JS:   String(42); (42).toString()
来源：http://lx.panjiajie.cn

TS:   String(42)
来源：http://qr.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ux.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://et.panjiajie.cn

Ruby: 42.to_s
来源：http://xc.muxihuayi.cn

C#:   42.ToString()
来源：http://wn.nicolike.cn

[A08] 取整与四舍五入
来源：http://sp.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xx.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eo.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fu.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lx.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bq.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pa.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mc.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cu.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://fx.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ko.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jj.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vw.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ia.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ty.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kp.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sn.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://of.szxytkj.cn

[A10] 生成随机数
来源：http://uo.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://dp.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://wr.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kg.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ux.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://jo.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qh.szxytkj.cn

Ruby: rand(1..100)
来源：http://jh.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://fj.colortex.cn

[A11] 条件表达式（三元）
来源：http://fj.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://fh.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wn.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zy.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uj.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://gx.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gg.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bv.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nb.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://kn.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iz.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ei.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://am.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://zt.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://he.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uh.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://rs.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://bx.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sl.newstarts.cn

Py:   "第一行\n第二行"
来源：http://me.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://bs.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://ue.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://yf.9csxet.cn

Java: "第一行\n第二行"
来源：http://aa.hahajie.cn

Go:   "第一行\n第二行"
来源：http://xy.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://bp.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://em.nszjky.cn

[A14] 注释写法
来源：http://xp.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ft.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://li.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://af.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://yg.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yb.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://vr.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qz.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://mm.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://pu.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://fd.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://lg.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://de.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://ge.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tf.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://qz.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://mg.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://la.newstarts.cn

[A16] 真假值判断规则
来源：http://dx.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pb.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yd.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wi.panjiajie.cn

TS:   if (!x) {}
来源：http://vb.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tz.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qe.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ew.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mt.shxzukj.cn

[A17] 位运算
来源：http://ma.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xd.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wc.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gl.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ch.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cc.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ow.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://fg.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://hy.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ie.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hb.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://cm.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sr.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://wl.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://pm.hnjuh.cn

[A19] 交换两个变量
来源：http://qv.haigaiapp.cn

Py:   a, b = b, a
来源：http://nm.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bf.colortex.cn

JS:   [a, b] = [b, a];
来源：http://fk.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ey.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://me.panjiajie.cn

Go:   a, b = b, a
来源：http://wv.huixiangedu.cn

Ruby: a, b = b, a
来源：http://zh.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://do.nszjky.cn

[A20] 读取标准输入
来源：http://fl.huanxung.cn

Py:   name = input("请输入：")
来源：http://yn.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://as.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hd.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://pk.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://oz.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pe.chemitech.net.cn

Ruby: gets.chomp
来源：http://sj.521024.cn

C#:   Console.ReadLine();
来源：http://oc.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://bi.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://uw.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cu.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://re.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://sy.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ub.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dx.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://gq.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://tv.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://mk.bookmarksfly.cn

Py:   len(s)
来源：http://wn.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oo.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rc.haigaiapp.cn

TS:   s.length
来源：http://mf.9csxet.cn

Java: s.length()
来源：http://rv.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jt.chemitech.net.cn

Ruby: s.length
来源：http://tf.shxzskj.cn

C#:   s.Length
来源：http://uy.panjiajie.cn

[A23] 大小写转换
来源：http://xi.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vg.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wv.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vb.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hb.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nv.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yu.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cr.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ud.huixiangedu.cn

[A24] 去除首尾空白
来源：http://zx.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xy.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wd.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dt.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://al.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rf.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://zl.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ep.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yq.shxzukj.cn

[A25] 字符串比较
来源：http://zu.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://vb.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yd.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xu.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ru.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fp.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sr.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ba.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://my.asd995.cn

[A26] 类型转换总览
来源：http://up.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wr.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gk.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wv.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://zt.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sp.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://do.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://br.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fn.hahajie.cn

================================================================================
来源：http://ua.nicolike.cn

B. 流程控制
来源：http://zr.lnxyls.cn

================================================================================
来源：http://bo.colortex.cn

[B01] 条件判断 if / else
来源：http://wo.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ew.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fv.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zu.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wo.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mu.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wl.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ar.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zf.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ri.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://by.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vx.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uw.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dk.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cm.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ct.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.521024.cn

[B03] switch / match / case
来源：http://qu.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://os.szxytkj.cn


<!-- 参考信息 -->