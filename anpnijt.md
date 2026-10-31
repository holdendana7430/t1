代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qe.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ra.yuntaijiaju.cn

【文件统计】
来源：http://bb.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mk.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ak.lnxyls.cn

目  录
来源：http://gi.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://tm.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ce.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sj.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://um.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ul.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ia.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ff.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sh.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gv.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hk.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hn.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lo.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lc.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kh.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pc.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fy.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://op.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dm.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mc.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dw.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gu.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ei.shtwfgs.cn

================================================================================
来源：http://hh.yuntaijiaju.cn

A. 基础语法与类型
来源：http://oo.huanxung.cn

================================================================================
来源：http://ym.yuntaijiaju.cn

[A01] Hello World
来源：http://ut.hahajie.cn

Py:   print("Hello, World!")
来源：http://rf.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://af.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://hh.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nw.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://uy.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://mt.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ud.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uw.szsharing.cn

[A02] 变量声明与赋值
来源：http://jf.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pz.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ae.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cd.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uc.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://ia.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://sw.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://se.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ji.chemitech.net.cn

[A03] 常量定义
来源：http://dh.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wy.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://ay.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://mp.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://lp.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://kr.nicolike.cn

Go:   const PI = 3.14159
来源：http://lu.huanxung.cn

Ruby: PI = 3.14159
来源：http://nf.521024.cn

C#:   const double PI = 3.14159;
来源：http://hd.huixiangedu.cn

[A04] 判断变量类型
来源：http://jr.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bu.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fm.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iz.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://ww.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://co.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bh.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vm.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://cz.haigaiapp.cn

[A05] 整数除法与取模
来源：http://nz.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oy.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rr.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bs.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hc.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://cv.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://ub.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://zm.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://as.9csxet.cn

[A06] 字符串转数字
来源：http://ay.asd995.cn

Py:   int("42"); float("3.14")
来源：http://rc.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kj.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ut.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fo.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dd.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zm.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wy.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ig.521024.cn

[A07] 数字转字符串
来源：http://wd.jctech888.com.cn

Py:   str(42)
来源：http://yn.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://ib.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://ja.panjiajie.cn

TS:   String(42)
来源：http://wq.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yp.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://sm.bjjhwx.cn

Ruby: 42.to_s
来源：http://rf.shtwfgs.cn

C#:   42.ToString()
来源：http://uq.521024.cn

[A08] 取整与四舍五入
来源：http://wl.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fu.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pl.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hk.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://al.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yb.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bz.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hp.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fo.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://pw.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kh.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://so.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uz.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gi.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nn.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cb.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xp.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gr.shtwfgs.cn

[A10] 生成随机数
来源：http://gt.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://qg.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://oc.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ct.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fl.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://rv.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fy.szxytkj.cn

Ruby: rand(1..100)
来源：http://uk.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://fe.hahajie.cn

[A11] 条件表达式（三元）
来源：http://cb.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://xu.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ud.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hp.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gx.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://iu.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ov.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://as.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://el.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://ma.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xq.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iq.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://ui.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ha.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://il.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qk.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ue.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://ng.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cq.9csxet.cn

Py:   "第一行\n第二行"
来源：http://gg.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ha.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://lx.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://or.9csxet.cn

Java: "第一行\n第二行"
来源：http://ue.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://dd.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://yf.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://km.chemitech.net.cn

[A14] 注释写法
来源：http://lm.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://au.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ri.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://fz.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://fv.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ih.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://ao.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hz.521024.cn

C#:   // 单行；/* 多行 */
来源：http://at.huanxung.cn

[A15] 空值判断与默认值
来源：http://va.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://xy.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://qp.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://cn.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://cb.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://jl.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://uj.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://fs.bjjhwx.cn

[A16] 真假值判断规则
来源：http://kg.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bo.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jj.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vp.yuexingan06.cn

TS:   if (!x) {}
来源：http://ty.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jm.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wb.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uc.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qp.jctech888.com.cn

[A17] 位运算
来源：http://gm.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jj.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lz.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://it.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://en.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zz.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://sx.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://ch.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://pu.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ax.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oy.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://et.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xq.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://la.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://ti.newstarts.cn

[A19] 交换两个变量
来源：http://xl.521024.cn

Py:   a, b = b, a
来源：http://ai.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lh.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://hg.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://vw.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://sz.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://vq.wgjwhj.cn

Ruby: a, b = b, a
来源：http://pb.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://kj.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ej.huanxung.cn

Py:   name = input("请输入：")
来源：http://ym.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xf.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nb.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://kq.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://ut.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wj.newstarts.cn

Ruby: gets.chomp
来源：http://fi.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ev.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://hh.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://mr.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://de.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://ef.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://pi.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://iu.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nu.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://qh.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://ij.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://mo.9csxet.cn

Py:   len(s)
来源：http://uu.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yv.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eb.huixinmuqiang.cn

TS:   s.length
来源：http://bi.szxytkj.cn

Java: s.length()
来源：http://zw.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aq.haigaiapp.cn

Ruby: s.length
来源：http://pk.asd995.cn

C#:   s.Length
来源：http://dg.hnjuh.cn

[A23] 大小写转换
来源：http://oj.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dy.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lg.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bo.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kx.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://en.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nr.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zn.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://te.szxytkj.cn

[A24] 去除首尾空白
来源：http://th.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fx.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ej.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dz.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://an.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hb.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://lp.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qd.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rw.lnxyls.cn

[A25] 字符串比较
来源：http://zr.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://cq.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yn.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ad.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sz.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://is.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cz.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ha.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xq.9csxet.cn

[A26] 类型转换总览
来源：http://ky.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wf.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kb.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lk.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://fu.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bx.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ww.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jj.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ao.panjiajie.cn

================================================================================
来源：http://ai.hnjuh.cn

B. 流程控制
来源：http://am.gzmigu.cn

================================================================================
来源：http://uz.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://xh.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uy.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wa.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lf.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oj.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://is.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qx.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vj.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gw.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://hv.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ih.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bg.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://up.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ff.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pr.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cc.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jz.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rg.wgjwhj.cn

[B03] switch / match / case
来源：http://er.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lo.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wp.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://op.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ij.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mi.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lx.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oj.bookmarksfly.cn

[B04] for 计数循环
来源：http://kp.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://qx.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xq.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hn.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xz.hahajie.cn


<!-- 参考信息 -->