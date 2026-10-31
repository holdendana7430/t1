代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qc.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://st.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jy.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nb.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zh.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hb.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ad.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pd.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wk.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cw.huixiangedu.cn

【文件统计】
来源：http://rw.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rc.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://dd.hahajie.cn

目  录
来源：http://gy.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://mc.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qe.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yf.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qm.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jk.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mn.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qd.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lf.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vz.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yw.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ia.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nt.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lv.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://td.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ca.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hb.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tl.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://th.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ba.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oi.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pl.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wn.hahajie.cn

================================================================================
来源：http://pg.jctech888.com.cn

A. 基础语法与类型
来源：http://xk.gzmigu.cn

================================================================================
来源：http://hd.gzmigu.cn

[A01] Hello World
来源：http://ew.newstarts.cn

Py:   print("Hello, World!")
来源：http://pw.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://hl.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://he.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qj.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://ku.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://xu.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://jd.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iz.newstarts.cn

[A02] 变量声明与赋值
来源：http://ka.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zm.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ki.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dd.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zc.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://bh.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://yp.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://xi.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ir.szsharing.cn

[A03] 常量定义
来源：http://aj.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hv.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ce.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://uk.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://pi.colortex.cn

Java: static final double PI = 3.14159;
来源：http://jb.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://mz.lnxyls.cn

Ruby: PI = 3.14159
来源：http://rj.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://im.bookmarksfly.cn

[A04] 判断变量类型
来源：http://fx.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dm.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ye.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ph.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://lw.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://la.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ia.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pr.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://qt.haigaiapp.cn

[A05] 整数除法与取模
来源：http://hf.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oi.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kd.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fr.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dc.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://zq.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://at.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://oj.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://vr.521024.cn

[A06] 字符串转数字
来源：http://dr.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://iw.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ye.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://av.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lc.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vs.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ov.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wy.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iy.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://pq.yuexingan06.cn

Py:   str(42)
来源：http://ty.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://au.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://hc.jctech888.com.cn

TS:   String(42)
来源：http://ci.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zt.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://eu.huanxung.cn

Ruby: 42.to_s
来源：http://dm.szxytkj.cn

C#:   42.ToString()
来源：http://fa.shxzukj.cn

[A08] 取整与四舍五入
来源：http://is.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ku.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ew.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://px.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xh.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://za.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://am.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fd.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dm.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://de.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uy.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ax.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uw.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://od.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uc.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hg.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ow.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ur.jianghongdianzi.cn

[A10] 生成随机数
来源：http://fn.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://sj.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://ji.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yb.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://og.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://aa.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xl.szsharing.cn

Ruby: rand(1..100)
来源：http://hi.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://dj.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://yk.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://xw.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kw.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uf.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dg.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://zs.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yk.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qh.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://an.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://bw.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jx.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bu.521024.cn

JS:   `Hello, ${name}!`
来源：http://dl.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://fl.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://wz.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jj.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://ba.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://bx.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yy.521024.cn

Py:   "第一行\n第二行"
来源：http://cg.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://mz.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://jz.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://us.szxytkj.cn

Java: "第一行\n第二行"
来源：http://rm.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ul.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://tv.9csxet.cn

C#:   "第一行\n第二行"
来源：http://xc.huanxung.cn

[A14] 注释写法
来源：http://jn.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ef.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qm.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://vq.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://cs.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bm.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://xk.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lu.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://na.gzmigu.cn

[A15] 空值判断与默认值
来源：http://hj.panjiajie.cn

Py:   value = data or "默认值"
来源：http://oo.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://uc.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://pu.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://rf.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yi.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://tk.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://hh.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://fd.szsharing.cn

[A16] 真假值判断规则
来源：http://si.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pl.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hc.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fe.nicolike.cn

TS:   if (!x) {}
来源：http://ky.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oz.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cm.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ie.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lu.nszjky.cn

[A17] 位运算
来源：http://nv.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tp.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vf.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cn.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ly.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rn.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tv.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://he.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jw.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://ms.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://xc.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://vt.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sg.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ex.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://wy.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ib.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ex.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://vl.nicolike.cn

[A19] 交换两个变量
来源：http://gi.huixiangedu.cn

Py:   a, b = b, a
来源：http://uq.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cf.521024.cn

JS:   [a, b] = [b, a];
来源：http://oq.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://dq.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://ty.shxzskj.cn

Go:   a, b = b, a
来源：http://pd.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://wl.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://up.shxzukj.cn

[A20] 读取标准输入
来源：http://ow.lnxyls.cn

Py:   name = input("请输入：")
来源：http://tn.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://io.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vg.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://yb.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://uk.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bh.szxytkj.cn

Ruby: gets.chomp
来源：http://bo.gzmigu.cn

C#:   Console.ReadLine();
来源：http://cp.nicolike.cn

[A21] 保留指定小数位输出
来源：http://wl.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://rm.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rh.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ha.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://ow.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://xo.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tk.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://pd.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://hl.hahajie.cn

[A22] 获取字符串长度
来源：http://jn.shxzukj.cn

Py:   len(s)
来源：http://uz.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dq.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ws.panjiajie.cn

TS:   s.length
来源：http://ul.haigaiapp.cn

Java: s.length()
来源：http://yr.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zc.shxzskj.cn

Ruby: s.length
来源：http://nh.hahajie.cn

C#:   s.Length
来源：http://de.shtwfgs.cn

[A23] 大小写转换
来源：http://fo.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yx.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tk.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jc.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qt.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zu.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://me.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oo.gzmigu.cn

[A24] 去除首尾空白
来源：http://ye.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uw.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bg.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mg.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cl.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fi.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://ef.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jf.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lz.wgjwhj.cn

[A25] 字符串比较
来源：http://fs.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://mb.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xo.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iq.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ei.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kx.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mj.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gq.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fb.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://nm.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wa.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://je.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ll.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ss.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fh.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://be.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ha.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sq.bookmarksfly.cn

================================================================================
来源：http://ps.nicolike.cn

B. 流程控制
来源：http://qe.szsharing.cn

================================================================================
来源：http://ka.panjiajie.cn

[B01] 条件判断 if / else
来源：http://dp.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wh.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fx.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yc.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xr.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bw.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tr.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vk.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hx.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://yh.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ji.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ye.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hf.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gb.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bp.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ze.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bf.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xl.shtwfgs.cn

[B03] switch / match / case
来源：http://ur.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mc.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bt.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ao.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pm.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qu.hnjuh.cn


<!-- 参考信息 -->