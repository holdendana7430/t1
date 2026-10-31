代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dd.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qs.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gf.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xs.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oq.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bo.haigaiapp.cn

【文件统计】
来源：http://qb.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sa.9csxet.cn

--------------------------------------------------------------------------------
来源：http://rn.newstarts.cn

目  录
来源：http://tq.521024.cn

--------------------------------------------------------------------------------
来源：http://iu.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hl.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nd.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sk.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fy.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zr.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://am.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lj.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://va.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zi.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hw.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cw.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hf.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sl.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xx.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yw.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sy.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lh.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hb.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tn.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gn.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mg.9csxet.cn

================================================================================
来源：http://mc.newstarts.cn

A. 基础语法与类型
来源：http://he.bjjhwx.cn

================================================================================
来源：http://dx.panjiajie.cn

[A01] Hello World
来源：http://qq.shxzskj.cn

Py:   print("Hello, World!")
来源：http://hl.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://rt.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://tu.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mf.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://zh.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://we.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://qn.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mg.huanxung.cn

[A02] 变量声明与赋值
来源：http://wz.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aa.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://is.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://td.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gp.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://es.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://gl.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://ip.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hg.huixinmuqiang.cn

[A03] 常量定义
来源：http://xs.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gh.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://jf.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://nc.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://lh.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://ao.shxzskj.cn

Go:   const PI = 3.14159
来源：http://gh.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://ql.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://yu.jctech888.com.cn

[A04] 判断变量类型
来源：http://ii.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nn.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vw.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zu.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://ca.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wd.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://at.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ch.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://mv.wgjwhj.cn

[A05] 整数除法与取模
来源：http://jg.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ul.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://le.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://um.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tb.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://rw.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://of.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://yt.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://va.colortex.cn

[A06] 字符串转数字
来源：http://fa.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://ax.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tc.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fg.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gf.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yq.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gp.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ri.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pe.chemitech.net.cn

[A07] 数字转字符串
来源：http://rc.shxzukj.cn

Py:   str(42)
来源：http://tp.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://tf.9csxet.cn

JS:   String(42); (42).toString()
来源：http://xj.yuntaijiaju.cn

TS:   String(42)
来源：http://nw.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lr.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://fr.jctech888.com.cn

Ruby: 42.to_s
来源：http://rj.muxihuayi.cn

C#:   42.ToString()
来源：http://ec.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://jm.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lr.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cw.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oz.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vk.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://um.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gq.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sx.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nb.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://hk.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sj.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ek.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zn.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://er.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wq.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gg.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gd.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lq.wgjwhj.cn

[A10] 生成随机数
来源：http://mt.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://ne.9csxet.cn

PHP:  random_int(1, 100);
来源：http://lr.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ya.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bw.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://tx.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mc.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://kn.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://jh.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://hb.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ju.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xh.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qj.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bw.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://gf.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hg.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vw.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://co.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://td.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ek.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zv.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://ih.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://bz.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://nl.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yl.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://ye.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://ea.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://va.colortex.cn

Py:   "第一行\n第二行"
来源：http://yg.colortex.cn

PHP:  "第一行\n第二行"
来源：http://gd.521024.cn

JS:   "第一行\n第二行"
来源：http://kn.huanxung.cn

TS:   "第一行\n第二行"
来源：http://gm.nicolike.cn

Java: "第一行\n第二行"
来源：http://ia.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://mk.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://jb.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://tg.szsharing.cn

[A14] 注释写法
来源：http://rv.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dp.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kl.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://ug.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://ev.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ik.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://ny.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://le.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://tp.lnxyls.cn

[A15] 空值判断与默认值
来源：http://jl.521024.cn

Py:   value = data or "默认值"
来源：http://wf.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://wp.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://id.521024.cn

TS:   const value = data ?? "默认值";
来源：http://yu.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fr.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://zi.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://gs.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://tr.wgjwhj.cn

[A16] 真假值判断规则
来源：http://eq.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cg.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vc.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ps.9csxet.cn

TS:   if (!x) {}
来源：http://uh.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ez.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aq.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uo.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.lnxyls.cn

[A17] 位运算
来源：http://qs.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ze.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eu.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jy.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vg.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lj.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://cn.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://ve.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://cz.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ul.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ve.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://wq.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ix.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://tc.521024.cn

C#:   (int)'A'; (char)65
来源：http://ya.asd995.cn

[A19] 交换两个变量
来源：http://ty.newstarts.cn

Py:   a, b = b, a
来源：http://xw.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hd.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ct.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://me.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://kl.chemitech.net.cn

Go:   a, b = b, a
来源：http://pm.szxytkj.cn

Ruby: a, b = b, a
来源：http://zi.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://bs.newstarts.cn

[A20] 读取标准输入
来源：http://eq.nszjky.cn

Py:   name = input("请输入：")
来源：http://rp.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nk.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ic.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://rx.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://jk.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nd.jctech888.com.cn

Ruby: gets.chomp
来源：http://ey.asd995.cn

C#:   Console.ReadLine();
来源：http://qa.newstarts.cn

[A21] 保留指定小数位输出
来源：http://ly.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://fp.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://md.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://jd.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://et.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://gt.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ep.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://cz.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://yn.panjiajie.cn

[A22] 获取字符串长度
来源：http://fj.lnxyls.cn

Py:   len(s)
来源：http://ox.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fq.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zj.haigaiapp.cn

TS:   s.length
来源：http://ti.huixiangedu.cn

Java: s.length()
来源：http://vd.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jq.shxzskj.cn

Ruby: s.length
来源：http://nm.szsharing.cn

C#:   s.Length
来源：http://ul.jianghongdianzi.cn

[A23] 大小写转换
来源：http://kt.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ki.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://km.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zr.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wc.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://py.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jx.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://en.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ce.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://pu.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://by.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hc.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vu.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://et.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bh.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cb.nszjky.cn

[A25] 字符串比较
来源：http://zc.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://le.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hi.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qc.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qe.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ip.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kt.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hw.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bg.asd995.cn

[A26] 类型转换总览
来源：http://lt.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://km.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qd.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://id.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://wt.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ct.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ml.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bc.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gp.shxzskj.cn

================================================================================
来源：http://qw.szxytkj.cn

B. 流程控制
来源：http://ps.9csxet.cn

================================================================================
来源：http://ya.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://io.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mh.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ha.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jy.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://za.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qx.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ge.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dq.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ra.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://ny.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mb.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bf.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gw.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wo.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qk.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xq.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bl.nicolike.cn

[B03] switch / match / case
来源：http://py.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qe.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dv.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://db.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hq.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uw.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xc.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hv.shxzskj.cn

[B04] for 计数循环
来源：http://wu.521024.cn


<!-- 参考信息 -->