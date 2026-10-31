代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iq.colortex.cn

【使用说明】
来源：http://px.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://go.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tm.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tq.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lh.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ar.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ul.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fi.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ni.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bn.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cd.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jp.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kc.nszjky.cn

【文件统计】
来源：http://vv.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bd.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://rn.nszjky.cn

目  录
来源：http://wu.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://sj.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xh.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kw.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fx.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dy.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://is.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://se.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ix.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://af.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ip.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://or.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cd.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qz.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tg.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://os.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dl.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jd.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ra.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ue.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bj.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fe.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://op.jianghongdianzi.cn

================================================================================
来源：http://wg.huanxung.cn

A. 基础语法与类型
来源：http://lz.colortex.cn

================================================================================
来源：http://dr.hnjuh.cn

[A01] Hello World
来源：http://zo.shxzukj.cn

Py:   print("Hello, World!")
来源：http://va.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://oy.colortex.cn

JS:   console.log("Hello, World!");
来源：http://ur.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://np.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://fy.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://gj.521024.cn

Ruby: puts "Hello, World!"
来源：http://sj.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qg.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://zy.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ps.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tz.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wi.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lk.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://ox.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://wr.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://ex.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zf.wgjwhj.cn

[A03] 常量定义
来源：http://az.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ty.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://aa.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://dk.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://xk.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://rb.asd995.cn

Go:   const PI = 3.14159
来源：http://uj.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://qd.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://kw.shxzukj.cn

[A04] 判断变量类型
来源：http://oo.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eu.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cr.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pq.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://gf.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://je.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fa.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://le.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://pj.hnjuh.cn

[A05] 整数除法与取模
来源：http://bn.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ll.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qp.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mj.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nf.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://hb.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://kn.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://fd.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://xd.wgjwhj.cn

[A06] 字符串转数字
来源：http://wj.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://xc.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nu.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mh.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://te.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://in.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ax.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cc.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tr.nszjky.cn

[A07] 数字转字符串
来源：http://rw.nicolike.cn

Py:   str(42)
来源：http://uq.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://bt.hahajie.cn

JS:   String(42); (42).toString()
来源：http://zp.huixinmuqiang.cn

TS:   String(42)
来源：http://wl.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pp.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://vl.gzmigu.cn

Ruby: 42.to_s
来源：http://ze.nicolike.cn

C#:   42.ToString()
来源：http://mi.szsharing.cn

[A08] 取整与四舍五入
来源：http://iw.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://se.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jd.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://so.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jh.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pi.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nh.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://si.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://au.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://vw.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xt.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rw.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://he.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kj.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ga.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tx.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lt.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xt.shxzskj.cn

[A10] 生成随机数
来源：http://eu.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ez.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://en.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ia.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://wf.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uh.asd995.cn

Ruby: rand(1..100)
来源：http://id.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://qr.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://oz.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://yi.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wc.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gy.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jc.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://qx.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://af.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nv.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oj.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://ds.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xx.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aa.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://bi.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://tn.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://gu.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gm.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://vq.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://vn.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uq.hahajie.cn

Py:   "第一行\n第二行"
来源：http://wl.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://ue.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://xu.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://mk.gzmigu.cn

Java: "第一行\n第二行"
来源：http://cc.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://tn.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://rr.newstarts.cn

C#:   "第一行\n第二行"
来源：http://mk.colortex.cn

[A14] 注释写法
来源：http://zl.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ic.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bq.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://le.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://pb.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gc.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://vw.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lo.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://db.gzmigu.cn

[A15] 空值判断与默认值
来源：http://hu.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://en.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://nj.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://dg.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://xo.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zk.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://of.asd995.cn

Ruby: value = data || "默认值"
来源：http://xe.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://qn.huanxung.cn

[A16] 真假值判断规则
来源：http://sr.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://va.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yl.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zo.wgjwhj.cn

TS:   if (!x) {}
来源：http://uz.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ke.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nb.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pw.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hi.szxytkj.cn

[A17] 位运算
来源：http://xb.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dw.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ht.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wv.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wp.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://od.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://dc.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://yk.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://on.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fk.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mt.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://tq.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://do.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://tm.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://qc.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://zz.szsharing.cn

Py:   a, b = b, a
来源：http://td.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mv.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://dn.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://dn.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://em.9csxet.cn

Go:   a, b = b, a
来源：http://ut.shtwfgs.cn

Ruby: a, b = b, a
来源：http://na.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://wz.bjjhwx.cn

[A20] 读取标准输入
来源：http://bt.newstarts.cn

Py:   name = input("请输入：")
来源：http://gw.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ow.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ic.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://qn.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://lm.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pi.lnxyls.cn

Ruby: gets.chomp
来源：http://zt.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://pg.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://ba.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://iw.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ls.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ph.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://uf.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://mj.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kj.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://mi.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://rs.shxzukj.cn

[A22] 获取字符串长度
来源：http://vk.chemitech.net.cn

Py:   len(s)
来源：http://eo.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ke.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ut.gzmigu.cn

TS:   s.length
来源：http://jx.nszjky.cn

Java: s.length()
来源：http://jd.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lo.shxzskj.cn

Ruby: s.length
来源：http://ld.shxzukj.cn

C#:   s.Length
来源：http://br.haigaiapp.cn

[A23] 大小写转换
来源：http://dk.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rf.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iz.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mi.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fo.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ty.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ia.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ro.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vk.shtwfgs.cn

[A24] 去除首尾空白
来源：http://vk.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://da.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zg.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yd.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ov.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://go.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oi.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bw.yuntaijiaju.cn

[A25] 字符串比较
来源：http://yt.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xd.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gs.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cg.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gr.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ka.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://me.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ku.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://fk.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://em.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://um.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ew.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://bz.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gg.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jm.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sx.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bh.bookmarksfly.cn

================================================================================
来源：http://pe.9csxet.cn

B. 流程控制
来源：http://gz.chemitech.net.cn

================================================================================
来源：http://gp.hahajie.cn

[B01] 条件判断 if / else
来源：http://xh.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ve.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gs.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gz.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bb.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://po.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qc.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xl.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://co.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://nj.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yc.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hj.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lo.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zx.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ij.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.lnxyls.cn

[B03] switch / match / case
来源：http://jb.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rw.shxzukj.cn


<!-- 参考信息 -->