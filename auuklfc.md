代发 wailian999

================================================================================
来源：http://sf.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://jm.nszjky.cn

Common Programming Examples Cheat Book
来源：http://sv.bookmarksfly.cn

================================================================================
来源：http://ar.asd995.cn

【收录内容】
来源：http://cf.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dr.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ca.szxytkj.cn

SQL · Bash · C · C++
来源：http://jz.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xh.haigaiapp.cn

【使用说明】
来源：http://sd.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ln.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xo.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bt.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vj.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kq.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://an.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ay.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vn.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wk.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ly.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kd.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tw.haigaiapp.cn

【文件统计】
来源：http://mn.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jj.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ah.asd995.cn

目  录
来源：http://jg.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://yk.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nz.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yz.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oy.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://un.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://es.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ew.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ub.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ye.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fo.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qb.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wa.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dm.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rs.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://az.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pl.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ei.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ho.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ib.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bf.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qj.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wq.shxzskj.cn

================================================================================
来源：http://if.yuntaijiaju.cn

A. 基础语法与类型
来源：http://yw.wgjwhj.cn

================================================================================
来源：http://cx.panjiajie.cn

[A01] Hello World
来源：http://ap.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://kr.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://ft.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://dc.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ow.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://cv.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://uv.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://pq.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hl.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://pp.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mu.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://of.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ym.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fg.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://fa.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://ex.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://gn.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xu.bjjhwx.cn

[A03] 常量定义
来源：http://zw.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lx.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://qv.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://yo.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://cc.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://gp.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://uq.szxytkj.cn

Ruby: PI = 3.14159
来源：http://kz.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://wh.shtwfgs.cn

[A04] 判断变量类型
来源：http://ch.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fs.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zf.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nv.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://yg.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zb.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://df.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gu.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://iq.huixiangedu.cn

[A05] 整数除法与取模
来源：http://yf.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dg.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ev.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ld.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ks.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://ec.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://ni.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://vs.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://nr.nszjky.cn

[A06] 字符串转数字
来源：http://ji.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://ef.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mz.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fw.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uv.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bw.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://un.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nz.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ab.szsharing.cn

[A07] 数字转字符串
来源：http://fv.521024.cn

Py:   str(42)
来源：http://dq.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://dv.newstarts.cn

JS:   String(42); (42).toString()
来源：http://kw.muxihuayi.cn

TS:   String(42)
来源：http://wg.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gg.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://qg.gzmigu.cn

Ruby: 42.to_s
来源：http://ds.huixinmuqiang.cn

C#:   42.ToString()
来源：http://kh.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://aq.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hu.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zq.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xt.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aa.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xx.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vx.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jh.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tp.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://kr.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kt.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ap.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wt.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ge.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ei.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vw.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vx.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ja.nszjky.cn

[A10] 生成随机数
来源：http://ie.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://md.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://hw.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://se.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kj.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://fa.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ch.szsharing.cn

Ruby: rand(1..100)
来源：http://rh.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://rw.newstarts.cn

[A11] 条件表达式（三元）
来源：http://ma.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://eo.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wv.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fs.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gi.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://fw.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wm.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sc.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nb.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://af.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://to.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bi.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://my.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://tq.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://ho.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gx.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://yb.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://br.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pe.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://yp.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://tj.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://pm.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://nb.lnxyls.cn

Java: "第一行\n第二行"
来源：http://ce.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://pt.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://tn.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://fo.szsharing.cn

[A14] 注释写法
来源：http://ao.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hn.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lg.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://fi.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://jm.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://we.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://rz.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ll.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://za.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://iq.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ip.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://ih.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://hd.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://dz.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ke.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://zx.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://wm.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://bp.shxzukj.cn

[A16] 真假值判断规则
来源：http://ko.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zl.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://if.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zo.shtwfgs.cn

TS:   if (!x) {}
来源：http://hg.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://np.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://su.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fb.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ov.shtwfgs.cn

[A17] 位运算
来源：http://qb.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tl.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rq.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ue.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gf.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bg.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xk.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://ld.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://vg.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://tx.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://se.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://px.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://ro.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xq.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://an.521024.cn

C#:   (int)'A'; (char)65
来源：http://kj.hahajie.cn

[A19] 交换两个变量
来源：http://de.muxihuayi.cn

Py:   a, b = b, a
来源：http://wb.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lv.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://pu.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://mn.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://iu.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://gy.yuexingan06.cn

Ruby: a, b = b, a
来源：http://uo.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://ar.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://wb.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://bg.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cx.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dq.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://od.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://vk.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dm.9csxet.cn

Ruby: gets.chomp
来源：http://rj.asd995.cn

C#:   Console.ReadLine();
来源：http://iz.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://nc.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://xn.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ji.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://sb.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://qf.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://xz.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ra.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://yv.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://bm.hahajie.cn

[A22] 获取字符串长度
来源：http://sp.panjiajie.cn

Py:   len(s)
来源：http://nv.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sw.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qe.szsharing.cn

TS:   s.length
来源：http://ov.huixiangedu.cn

Java: s.length()
来源：http://rb.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wo.yuexingan06.cn

Ruby: s.length
来源：http://yb.lnxyls.cn

C#:   s.Length
来源：http://dd.lnxyls.cn

[A23] 大小写转换
来源：http://dw.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wm.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sr.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://se.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fq.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rc.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ou.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ez.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wj.hnjuh.cn

[A24] 去除首尾空白
来源：http://ky.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vz.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cu.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ua.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ah.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://md.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://jx.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ku.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lm.shxzukj.cn

[A25] 字符串比较
来源：http://wz.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://vl.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vx.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sf.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cd.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rf.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cy.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://az.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lz.newstarts.cn

[A26] 类型转换总览
来源：http://yd.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iq.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xa.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hs.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://av.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pv.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ds.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zz.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://th.521024.cn

================================================================================
来源：http://hn.huanxung.cn

B. 流程控制
来源：http://el.bjjhwx.cn

================================================================================
来源：http://ff.shxzskj.cn

[B01] 条件判断 if / else
来源：http://ql.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fq.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zr.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pj.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pf.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oh.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qy.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bo.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://yv.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jx.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qx.newstarts.cn


<!-- 参考信息 -->