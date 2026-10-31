代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ez.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ua.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nd.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gi.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fp.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fz.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eh.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eb.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lh.szsharing.cn

【文件统计】
来源：http://zl.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://da.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://vr.huanxung.cn

目  录
来源：http://sy.huanxung.cn

--------------------------------------------------------------------------------
来源：http://lr.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yq.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lr.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vv.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ke.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gq.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cc.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yq.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://au.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ww.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yb.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nx.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hw.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://or.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cv.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ml.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dp.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vp.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hy.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sn.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cb.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nw.bjjhwx.cn

================================================================================
来源：http://eg.nszjky.cn

A. 基础语法与类型
来源：http://by.panjiajie.cn

================================================================================
来源：http://ci.szsharing.cn

[A01] Hello World
来源：http://rd.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://gg.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://hb.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://ko.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jt.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://kb.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ag.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://mg.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vo.hnjuh.cn

[A02] 变量声明与赋值
来源：http://ya.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lz.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ds.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ps.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cj.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://wf.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://kc.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://kv.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://po.wgjwhj.cn

[A03] 常量定义
来源：http://xg.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kj.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://um.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://kb.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://st.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://wn.huanxung.cn

Go:   const PI = 3.14159
来源：http://um.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://hq.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://xl.haigaiapp.cn

[A04] 判断变量类型
来源：http://dz.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://as.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://op.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jk.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://ss.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xx.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bb.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nc.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://pl.bjjhwx.cn

[A05] 整数除法与取模
来源：http://re.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mz.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cl.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lr.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ng.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://vq.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://mc.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://oj.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://cw.hnjuh.cn

[A06] 字符串转数字
来源：http://xh.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://ot.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gu.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lg.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hu.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dr.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gr.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jl.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ss.colortex.cn

[A07] 数字转字符串
来源：http://gg.bjjhwx.cn

Py:   str(42)
来源：http://du.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://sl.huanxung.cn

JS:   String(42); (42).toString()
来源：http://vq.jianghongdianzi.cn

TS:   String(42)
来源：http://jw.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hi.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://tk.9csxet.cn

Ruby: 42.to_s
来源：http://hf.shxzukj.cn

C#:   42.ToString()
来源：http://ja.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://ti.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fi.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rq.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://po.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hg.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xz.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qp.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tq.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tf.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://fo.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sl.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://go.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pq.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wx.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vj.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pq.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ch.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gu.huixinmuqiang.cn

[A10] 生成随机数
来源：http://xr.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://br.szsharing.cn

PHP:  random_int(1, 100);
来源：http://ay.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yu.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uy.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://fi.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://av.9csxet.cn

Ruby: rand(1..100)
来源：http://oq.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://ho.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://bs.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://so.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://db.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ox.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wd.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://mz.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bl.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rf.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yw.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://pd.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hu.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zd.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://uo.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://rp.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://qg.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tk.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://as.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://fm.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bp.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://dn.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://pr.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://vy.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://jb.gzmigu.cn

Java: "第一行\n第二行"
来源：http://xx.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://nv.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://dx.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://xf.nicolike.cn

[A14] 注释写法
来源：http://ny.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://et.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dl.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://fu.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://rk.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ba.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ut.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xd.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://gd.hahajie.cn

[A15] 空值判断与默认值
来源：http://tu.hnjuh.cn

Py:   value = data or "默认值"
来源：http://af.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://dy.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://xc.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://uz.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gb.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ya.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://hw.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://jf.shxzukj.cn

[A16] 真假值判断规则
来源：http://qc.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hi.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tl.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eq.szsharing.cn

TS:   if (!x) {}
来源：http://xz.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fx.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yv.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wh.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eh.hahajie.cn

[A17] 位运算
来源：http://us.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uh.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hw.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uh.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://au.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hn.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://pv.asd995.cn

Py:   ord("A"); chr(65)
来源：http://yj.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://by.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kl.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fi.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://qm.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pn.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://kk.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://ey.asd995.cn

[A19] 交换两个变量
来源：http://ya.shxzskj.cn

Py:   a, b = b, a
来源：http://lf.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ki.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://qf.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://ff.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://wm.panjiajie.cn

Go:   a, b = b, a
来源：http://pd.bjjhwx.cn

Ruby: a, b = b, a
来源：http://tl.521024.cn

C#:   (a, b) = (b, a);
来源：http://tb.shxzukj.cn

[A20] 读取标准输入
来源：http://zj.hahajie.cn

Py:   name = input("请输入：")
来源：http://rd.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ms.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ci.colortex.cn

TS:   // Node.js：readline 模块
来源：http://nf.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://rx.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cf.gzmigu.cn

Ruby: gets.chomp
来源：http://yp.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://sx.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://xf.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://wz.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oq.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://wu.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://xq.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://go.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qj.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://vg.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://fq.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://ey.muxihuayi.cn

Py:   len(s)
来源：http://cj.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ul.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wv.9csxet.cn

TS:   s.length
来源：http://kz.bjjhwx.cn

Java: s.length()
来源：http://oo.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://au.hnjuh.cn

Ruby: s.length
来源：http://wp.haigaiapp.cn

C#:   s.Length
来源：http://yq.huixiangedu.cn

[A23] 大小写转换
来源：http://nq.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ih.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qg.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xq.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xc.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gm.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nx.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sv.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pq.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://su.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gz.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uz.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bf.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xv.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://et.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://vg.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uo.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ep.bjjhwx.cn

[A25] 字符串比较
来源：http://mq.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://nn.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://no.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hr.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://is.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rf.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bl.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tt.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iv.szsharing.cn

[A26] 类型转换总览
来源：http://pj.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bi.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qq.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mc.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://jj.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fz.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pa.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ck.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fd.huixiangedu.cn

================================================================================
来源：http://gt.shxzskj.cn

B. 流程控制
来源：http://qh.shxzskj.cn

================================================================================
来源：http://ik.asd995.cn

[B01] 条件判断 if / else
来源：http://sy.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zc.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zk.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hj.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rj.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gt.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dn.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wj.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lg.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://wn.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wq.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ug.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xl.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lf.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ol.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.huixiangedu.cn

[B03] switch / match / case
来源：http://yf.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ne.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gc.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://la.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ic.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ha.asd995.cn


<!-- 参考信息 -->