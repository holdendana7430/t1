代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uk.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wu.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://id.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://an.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://au.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vp.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qw.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cd.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kj.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qg.szsharing.cn

【文件统计】
来源：http://uz.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ud.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ny.hahajie.cn

目  录
来源：http://nm.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qo.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hl.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xv.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cf.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wk.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ya.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://of.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ce.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dc.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wf.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://np.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://co.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pg.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nu.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ek.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zc.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://au.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vh.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lh.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jk.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://js.hnjuh.cn

================================================================================
来源：http://uz.9csxet.cn

A. 基础语法与类型
来源：http://ad.szsharing.cn

================================================================================
来源：http://ar.jianghongdianzi.cn

[A01] Hello World
来源：http://ec.asd995.cn

Py:   print("Hello, World!")
来源：http://rl.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://kj.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://qe.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cq.521024.cn

Java: System.out.println("Hello, World!");
来源：http://bn.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://xp.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://tk.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bt.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://nj.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jl.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lm.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://et.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ew.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ze.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://as.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://te.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bw.yuexingan06.cn

[A03] 常量定义
来源：http://ob.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xt.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://ex.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://xg.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://pz.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://vk.shxzukj.cn

Go:   const PI = 3.14159
来源：http://gf.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://jw.521024.cn

C#:   const double PI = 3.14159;
来源：http://vc.jctech888.com.cn

[A04] 判断变量类型
来源：http://wa.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qt.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ko.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ky.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://xd.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dk.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oo.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tk.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://no.yuexingan06.cn

[A05] 整数除法与取模
来源：http://fg.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vf.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cm.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zd.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bd.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://ea.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://ya.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://il.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://us.521024.cn

[A06] 字符串转数字
来源：http://nn.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://wz.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://so.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ka.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ht.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://az.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nk.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ms.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yj.shxzskj.cn

[A07] 数字转字符串
来源：http://rb.yuntaijiaju.cn

Py:   str(42)
来源：http://zn.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://su.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://fs.chemitech.net.cn

TS:   String(42)
来源：http://um.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nx.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://oa.gzmigu.cn

Ruby: 42.to_s
来源：http://pr.shxzukj.cn

C#:   42.ToString()
来源：http://ka.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://xy.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lb.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ww.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nf.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bj.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bg.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wq.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fz.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gw.colortex.cn

[A09] 绝对值与最大最小值
来源：http://qf.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qk.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ub.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vp.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://go.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ov.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rc.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yi.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vb.jianghongdianzi.cn

[A10] 生成随机数
来源：http://ip.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://lc.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://ee.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mj.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lu.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ti.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qc.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://lr.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://br.9csxet.cn

[A11] 条件表达式（三元）
来源：http://og.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://es.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hm.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xp.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://it.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://cy.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pv.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ec.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xy.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://wn.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ve.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zq.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://gy.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ci.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://qr.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://cf.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://vz.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zg.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://px.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://vb.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://kf.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://op.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://nv.nszjky.cn

Go:   "第一行\n第二行"
来源：http://cr.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://wa.521024.cn

C#:   "第一行\n第二行"
来源：http://jg.9csxet.cn

[A14] 注释写法
来源：http://vm.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://en.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rj.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://zq.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://vi.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qv.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://eb.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eb.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://bx.9csxet.cn

[A15] 空值判断与默认值
来源：http://uh.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://bc.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://ez.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://zv.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://ua.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jf.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://pu.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://nv.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://xl.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://yf.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sg.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://we.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pw.521024.cn

TS:   if (!x) {}
来源：http://ki.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lm.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oi.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://li.shxzskj.cn

[A17] 位运算
来源：http://oj.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uo.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ad.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kw.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ua.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vb.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xk.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://xo.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://wl.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://cj.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://be.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oo.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://uk.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dy.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://ga.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://oc.nszjky.cn

[A19] 交换两个变量
来源：http://go.521024.cn

Py:   a, b = b, a
来源：http://bj.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vd.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://sg.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://eq.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://yu.colortex.cn

Go:   a, b = b, a
来源：http://pc.gzmigu.cn

Ruby: a, b = b, a
来源：http://mv.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://cj.gzmigu.cn

[A20] 读取标准输入
来源：http://rw.hahajie.cn

Py:   name = input("请输入：")
来源：http://pw.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tl.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ci.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://lu.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://co.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lm.shtwfgs.cn

Ruby: gets.chomp
来源：http://cw.szsharing.cn

C#:   Console.ReadLine();
来源：http://xf.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://nh.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://wh.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ht.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://td.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ru.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://ta.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sa.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://bs.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://zg.haigaiapp.cn

[A22] 获取字符串长度
来源：http://oo.panjiajie.cn

Py:   len(s)
来源：http://mm.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xu.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pd.shtwfgs.cn

TS:   s.length
来源：http://qn.shxzukj.cn

Java: s.length()
来源：http://sz.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://af.huixinmuqiang.cn

Ruby: s.length
来源：http://nn.521024.cn

C#:   s.Length
来源：http://sq.muxihuayi.cn

[A23] 大小写转换
来源：http://yg.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rf.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ee.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nt.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://su.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zd.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wi.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ms.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lj.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://hf.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ck.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qx.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sx.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ai.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://hw.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qq.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://er.asd995.cn

[A25] 字符串比较
来源：http://li.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://fs.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zc.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://be.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lm.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://og.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kv.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ce.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mv.nicolike.cn

[A26] 类型转换总览
来源：http://wn.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://np.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zr.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dt.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://uf.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ga.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qb.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hs.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qa.chemitech.net.cn

================================================================================
来源：http://fw.haigaiapp.cn

B. 流程控制
来源：http://ow.bjjhwx.cn

================================================================================
来源：http://me.shxzukj.cn

[B01] 条件判断 if / else
来源：http://el.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sb.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zr.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sw.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dk.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bi.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bx.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jr.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qu.asd995.cn

[B02] 多分支 else if / elif
来源：http://ru.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vw.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cc.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nh.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aj.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uh.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eu.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ct.shxzskj.cn

[B03] switch / match / case
来源：http://id.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://la.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gz.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kt.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wa.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oc.521024.cn


<!-- 参考信息 -->