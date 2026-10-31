代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://di.hahajie.cn

【使用说明】
来源：http://vt.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://us.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bn.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://db.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ah.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wt.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aj.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ds.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nd.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rf.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sb.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yd.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ql.bjjhwx.cn

【文件统计】
来源：http://gi.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pw.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://gy.gzmigu.cn

目  录
来源：http://gl.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://nd.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dt.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ge.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hm.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oo.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://id.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ly.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sp.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gt.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bi.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hu.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ac.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dd.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://db.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://op.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dm.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ds.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iy.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xk.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://on.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ct.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bk.asd995.cn

================================================================================
来源：http://hu.jianghongdianzi.cn

A. 基础语法与类型
来源：http://zu.nszjky.cn

================================================================================
来源：http://tn.huixiangedu.cn

[A01] Hello World
来源：http://ne.shxzukj.cn

Py:   print("Hello, World!")
来源：http://hl.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://iu.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://oe.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ua.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://ng.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://fr.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://yo.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mz.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://yw.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tn.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yo.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qx.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pw.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://df.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://so.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://mx.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rf.panjiajie.cn

[A03] 常量定义
来源：http://mz.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ir.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://az.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://ne.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://yl.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://hr.shxzukj.cn

Go:   const PI = 3.14159
来源：http://mh.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://dp.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://ek.shxzukj.cn

[A04] 判断变量类型
来源：http://ff.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sg.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xo.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rv.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://ah.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jb.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rh.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qd.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://rc.bjjhwx.cn

[A05] 整数除法与取模
来源：http://ok.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://im.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sz.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bo.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jy.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://vj.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://oy.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://so.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://jc.bjjhwx.cn

[A06] 字符串转数字
来源：http://aj.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://ye.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hu.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rp.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gv.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ay.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uu.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hx.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qb.asd995.cn

[A07] 数字转字符串
来源：http://hf.bjjhwx.cn

Py:   str(42)
来源：http://cr.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://qi.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://tq.shtwfgs.cn

TS:   String(42)
来源：http://ih.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tp.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://yi.jctech888.com.cn

Ruby: 42.to_s
来源：http://yq.hnjuh.cn

C#:   42.ToString()
来源：http://wf.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://pi.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jc.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bn.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nd.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fn.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gm.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cw.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hv.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vw.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://ij.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gf.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gx.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fr.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pa.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sl.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pm.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://du.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eb.bookmarksfly.cn

[A10] 生成随机数
来源：http://mu.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://pu.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://xp.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xg.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lm.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://yi.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vu.yuexingan06.cn

Ruby: rand(1..100)
来源：http://fu.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://my.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://xu.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://nv.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fw.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://df.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qb.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://hv.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lz.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aq.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eb.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ht.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xv.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fk.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://cj.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://rj.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://zi.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ee.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://hf.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://as.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dd.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://kl.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://we.colortex.cn

JS:   "第一行\n第二行"
来源：http://si.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://xw.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ev.asd995.cn

Go:   "第一行\n第二行"
来源：http://ld.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://xp.nszjky.cn

C#:   "第一行\n第二行"
来源：http://pi.huixiangedu.cn

[A14] 注释写法
来源：http://ax.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ur.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jd.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://xn.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://dh.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yv.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://lr.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bu.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://vh.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://op.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://yb.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://xh.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://wl.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://qk.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bf.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://vd.huanxung.cn

Ruby: value = data || "默认值"
来源：http://wm.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://mo.shxzukj.cn

[A16] 真假值判断规则
来源：http://tw.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yg.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sx.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cq.521024.cn

TS:   if (!x) {}
来源：http://rz.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xd.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bh.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rx.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kb.nicolike.cn

[A17] 位运算
来源：http://cg.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ks.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tx.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eb.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bu.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nc.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wl.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://nc.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://cu.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://kb.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://gq.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pl.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://oi.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://lk.nszjky.cn

[A19] 交换两个变量
来源：http://sk.bjjhwx.cn

Py:   a, b = b, a
来源：http://zo.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ln.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://dh.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://wt.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://ry.szxytkj.cn

Go:   a, b = b, a
来源：http://gd.wgjwhj.cn

Ruby: a, b = b, a
来源：http://bo.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://gs.muxihuayi.cn

[A20] 读取标准输入
来源：http://wh.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ff.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mq.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://td.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://cr.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://fs.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zp.chemitech.net.cn

Ruby: gets.chomp
来源：http://me.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://po.newstarts.cn

[A21] 保留指定小数位输出
来源：http://cq.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://cd.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dx.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://ue.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://gn.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://pr.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ew.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://zk.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ox.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://rh.jctech888.com.cn

Py:   len(s)
来源：http://fs.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uy.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sl.bjjhwx.cn

TS:   s.length
来源：http://rj.yuexingan06.cn

Java: s.length()
来源：http://ci.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qq.gzmigu.cn

Ruby: s.length
来源：http://wf.shxzskj.cn

C#:   s.Length
来源：http://kl.jctech888.com.cn

[A23] 大小写转换
来源：http://xy.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sd.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xk.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://il.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wg.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://en.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sf.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://li.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fj.asd995.cn

[A24] 去除首尾空白
来源：http://ay.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pq.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rl.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xd.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ct.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fs.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ma.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gd.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bz.hnjuh.cn

[A25] 字符串比较
来源：http://ms.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://pd.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://my.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xv.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ns.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rk.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uv.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ve.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ns.shxzskj.cn

[A26] 类型转换总览
来源：http://hr.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qp.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sd.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sa.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://fq.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jq.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tm.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://of.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ff.shxzskj.cn

================================================================================
来源：http://ww.chemitech.net.cn

B. 流程控制
来源：http://zh.panjiajie.cn

================================================================================
来源：http://bz.shxzukj.cn

[B01] 条件判断 if / else
来源：http://le.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yw.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zg.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sw.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wq.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wk.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ez.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ky.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ws.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://ny.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tx.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yy.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wn.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rv.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kj.chemitech.net.cn

[B03] switch / match / case
来源：http://dw.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://en.521024.cn


<!-- 参考信息 -->