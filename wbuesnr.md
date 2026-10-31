代发 wailian999

================================================================================
来源：http://do.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://fc.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://st.jctech888.com.cn

================================================================================
来源：http://qc.nicolike.cn

【收录内容】
来源：http://wu.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yd.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gk.szxytkj.cn

SQL · Bash · C · C++
来源：http://bk.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cu.nicolike.cn

【使用说明】
来源：http://qa.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xs.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rp.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://no.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://le.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yh.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://si.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bo.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ar.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xa.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jm.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bv.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pm.nszjky.cn

【文件统计】
来源：http://wk.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cl.newstarts.cn

--------------------------------------------------------------------------------
来源：http://qf.yuntaijiaju.cn

目  录
来源：http://gn.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://fg.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xa.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://js.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wl.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ei.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nh.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rq.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qy.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fi.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jv.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fm.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yt.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kj.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tb.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vt.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ne.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ok.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aj.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hg.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://io.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cl.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sf.haigaiapp.cn

================================================================================
来源：http://xt.shtwfgs.cn

A. 基础语法与类型
来源：http://xe.jianghongdianzi.cn

================================================================================
来源：http://ds.lnxyls.cn

[A01] Hello World
来源：http://bf.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://dq.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://pb.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://nj.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zm.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://nl.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://jv.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://fc.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gy.nszjky.cn

[A02] 变量声明与赋值
来源：http://to.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fj.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nn.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yv.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tt.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://jz.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://mt.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://lo.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jd.newstarts.cn

[A03] 常量定义
来源：http://bs.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hx.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://xy.szsharing.cn

JS:   const PI = 3.14159;
来源：http://in.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://fo.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://zn.521024.cn

Go:   const PI = 3.14159
来源：http://ph.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://us.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://vv.bookmarksfly.cn

[A04] 判断变量类型
来源：http://jj.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://go.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ob.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fp.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://vh.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ug.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cl.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rd.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://jx.chemitech.net.cn

[A05] 整数除法与取模
来源：http://kf.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mv.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dh.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nc.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tf.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://ta.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://wp.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://rx.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://mp.newstarts.cn

[A06] 字符串转数字
来源：http://lh.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://rb.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ly.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zb.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nj.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fm.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://df.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wx.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ip.szxytkj.cn

[A07] 数字转字符串
来源：http://dr.huixiangedu.cn

Py:   str(42)
来源：http://oa.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://fz.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://iz.shxzskj.cn

TS:   String(42)
来源：http://ja.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oj.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://ol.bjjhwx.cn

Ruby: 42.to_s
来源：http://jh.huixiangedu.cn

C#:   42.ToString()
来源：http://bn.gzmigu.cn

[A08] 取整与四舍五入
来源：http://rj.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://st.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ht.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sv.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dc.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ic.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yw.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ns.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mg.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://lb.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ns.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nh.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nx.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dt.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ft.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eu.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cu.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bk.bjjhwx.cn

[A10] 生成随机数
来源：http://sf.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://fd.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://uy.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tk.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mw.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://sg.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bu.szsharing.cn

Ruby: rand(1..100)
来源：http://kk.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://bf.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://bl.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://jp.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ci.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ri.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dd.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ii.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kh.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qd.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lf.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://ft.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xq.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ix.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://uo.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://xl.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://pu.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fb.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://cd.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://bh.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yw.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://up.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://qo.521024.cn

JS:   "第一行\n第二行"
来源：http://zd.9csxet.cn

TS:   "第一行\n第二行"
来源：http://pf.newstarts.cn

Java: "第一行\n第二行"
来源：http://vi.hahajie.cn

Go:   "第一行\n第二行"
来源：http://ig.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://gm.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://sd.nicolike.cn

[A14] 注释写法
来源：http://ca.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gj.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fz.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://dk.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://fu.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mr.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://rq.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pg.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://ag.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://nd.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://qg.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ac.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://da.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://wi.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nw.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://xl.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://zj.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://hd.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://ku.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ck.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jl.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cw.szsharing.cn

TS:   if (!x) {}
来源：http://rx.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gp.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kd.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rk.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ko.huixiangedu.cn

[A17] 位运算
来源：http://jn.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xu.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gp.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kz.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vy.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uz.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://av.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ia.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://df.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://gt.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://fi.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ph.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://np.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://ur.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vp.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://gn.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://hk.yuexingan06.cn

[A19] 交换两个变量
来源：http://rs.panjiajie.cn

Py:   a, b = b, a
来源：http://sd.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xt.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://gd.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://lk.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://op.szsharing.cn

Go:   a, b = b, a
来源：http://lk.asd995.cn

Ruby: a, b = b, a
来源：http://yf.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://tj.bjjhwx.cn

[A20] 读取标准输入
来源：http://ro.szsharing.cn

Py:   name = input("请输入：")
来源：http://pa.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ur.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bc.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://wc.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://yl.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ud.haigaiapp.cn

Ruby: gets.chomp
来源：http://cw.nicolike.cn

C#:   Console.ReadLine();
来源：http://qf.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://gt.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://tc.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ol.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://ki.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://xv.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://sr.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lf.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://yb.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://zj.jctech888.com.cn

[A22] 获取字符串长度
来源：http://fr.newstarts.cn

Py:   len(s)
来源：http://wt.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yx.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mp.jianghongdianzi.cn

TS:   s.length
来源：http://fa.szsharing.cn

Java: s.length()
来源：http://fm.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hb.newstarts.cn

Ruby: s.length
来源：http://dv.bjjhwx.cn

C#:   s.Length
来源：http://ff.shxzukj.cn

[A23] 大小写转换
来源：http://ol.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ph.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gx.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ew.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ah.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ai.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vc.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lt.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oc.huixiangedu.cn

[A24] 去除首尾空白
来源：http://vd.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jr.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hv.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hn.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ob.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yq.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://mn.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yr.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ji.bookmarksfly.cn

[A25] 字符串比较
来源：http://da.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://er.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zr.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pm.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qu.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yb.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bb.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nx.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://of.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://sz.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gk.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://si.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dp.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://cb.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bq.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yf.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://za.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yi.shxzskj.cn

================================================================================
来源：http://wu.jianghongdianzi.cn

B. 流程控制
来源：http://ex.haigaiapp.cn

================================================================================
来源：http://lo.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://mi.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rl.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ci.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iz.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gl.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dk.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ns.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hq.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fq.hahajie.cn

[B02] 多分支 else if / elif
来源：http://lp.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zk.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sb.panjiajie.cn


<!-- 参考信息 -->