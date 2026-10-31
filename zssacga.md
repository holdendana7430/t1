代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uo.panjiajie.cn

【使用说明】
来源：http://wq.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dm.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rc.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wp.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hu.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://af.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://il.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wm.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pq.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fm.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ae.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ca.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ur.yuexingan06.cn

【文件统计】
来源：http://ja.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://kl.lnxyls.cn

目  录
来源：http://hi.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://gj.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ns.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vn.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cl.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tf.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rx.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tr.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ws.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ve.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jx.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vm.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gr.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://af.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sa.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hn.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ge.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lz.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bo.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hl.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://da.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yd.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vq.shxzukj.cn

================================================================================
来源：http://di.yuntaijiaju.cn

A. 基础语法与类型
来源：http://nt.521024.cn

================================================================================
来源：http://pi.hahajie.cn

[A01] Hello World
来源：http://et.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://aj.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://bt.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://ox.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lk.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://uz.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://iy.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://gw.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jx.colortex.cn

[A02] 变量声明与赋值
来源：http://mo.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://it.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yh.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ap.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ax.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ht.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://tb.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://ha.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jh.newstarts.cn

[A03] 常量定义
来源：http://ut.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://st.asd995.cn

PHP:  const PI = 3.14159;
来源：http://re.nszjky.cn

JS:   const PI = 3.14159;
来源：http://dz.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://nm.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://jp.panjiajie.cn

Go:   const PI = 3.14159
来源：http://zo.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://ry.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://fm.lnxyls.cn

[A04] 判断变量类型
来源：http://eh.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jh.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uj.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pt.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://xt.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dt.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gk.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bl.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://en.shxzskj.cn

[A05] 整数除法与取模
来源：http://hf.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rv.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oq.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iz.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://zf.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://co.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://ua.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://ql.521024.cn

[A06] 字符串转数字
来源：http://qf.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://hu.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yv.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lx.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gn.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://th.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yz.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mm.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bt.colortex.cn

[A07] 数字转字符串
来源：http://xp.shxzukj.cn

Py:   str(42)
来源：http://jw.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://ov.huanxung.cn

JS:   String(42); (42).toString()
来源：http://aq.bookmarksfly.cn

TS:   String(42)
来源：http://ti.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sf.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://qk.huanxung.cn

Ruby: 42.to_s
来源：http://vr.huixinmuqiang.cn

C#:   42.ToString()
来源：http://wl.9csxet.cn

[A08] 取整与四舍五入
来源：http://uw.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nz.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bj.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yn.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gx.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xb.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sx.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uw.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://md.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://qr.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://to.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ay.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yw.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gx.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nx.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bn.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ot.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cr.shxzskj.cn

[A10] 生成随机数
来源：http://bp.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://bd.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://yp.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ya.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ul.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://zt.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://et.szxytkj.cn

Ruby: rand(1..100)
来源：http://sd.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://pb.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ms.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://or.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://je.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gl.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ov.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://nb.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vy.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xc.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sk.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://bh.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sc.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pg.521024.cn

JS:   `Hello, ${name}!`
来源：http://cf.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://eq.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://hr.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vh.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://ox.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://aj.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qx.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://wf.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://ps.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://qz.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://mo.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://cq.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://of.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://zi.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://fx.shxzukj.cn

[A14] 注释写法
来源：http://ec.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ds.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ys.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://dr.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://eg.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ic.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://ek.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wh.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://jc.lnxyls.cn

[A15] 空值判断与默认值
来源：http://fe.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://wo.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://aa.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://jd.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://iz.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rq.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://nj.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://pg.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://ze.huixiangedu.cn

[A16] 真假值判断规则
来源：http://hl.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qu.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ox.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ko.szsharing.cn

TS:   if (!x) {}
来源：http://cb.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xk.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bl.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gy.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gd.muxihuayi.cn

[A17] 位运算
来源：http://iu.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jm.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dc.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rc.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://je.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mb.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xy.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://wp.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://ta.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://lr.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sj.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dv.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://op.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rg.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://vs.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://hl.shxzukj.cn

[A19] 交换两个变量
来源：http://wt.shtwfgs.cn

Py:   a, b = b, a
来源：http://fa.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qi.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://bj.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://ka.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://fo.shxzukj.cn

Go:   a, b = b, a
来源：http://vn.9csxet.cn

Ruby: a, b = b, a
来源：http://vw.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://ow.szsharing.cn

[A20] 读取标准输入
来源：http://dt.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://tl.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ex.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://um.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://cr.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://cu.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wm.shxzskj.cn

Ruby: gets.chomp
来源：http://id.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://me.nicolike.cn

[A21] 保留指定小数位输出
来源：http://dr.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://pl.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kx.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ip.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://bx.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://za.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cp.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://kn.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://qo.colortex.cn

[A22] 获取字符串长度
来源：http://eg.huanxung.cn

Py:   len(s)
来源：http://fb.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ue.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://st.bookmarksfly.cn

TS:   s.length
来源：http://ce.chemitech.net.cn

Java: s.length()
来源：http://ty.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wy.nicolike.cn

Ruby: s.length
来源：http://wc.yuexingan06.cn

C#:   s.Length
来源：http://yt.szxytkj.cn

[A23] 大小写转换
来源：http://rm.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kk.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vz.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dr.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xe.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oq.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ns.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ax.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://of.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dm.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qy.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ty.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://op.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lu.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://am.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://re.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://av.nicolike.cn

[A25] 字符串比较
来源：http://ap.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ne.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rs.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cy.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ed.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tf.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rl.hnjuh.cn

[A26] 类型转换总览
来源：http://rg.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zf.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ty.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sf.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://jl.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ob.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oq.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://st.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lh.szxytkj.cn

================================================================================
来源：http://fv.muxihuayi.cn

B. 流程控制
来源：http://uz.shxzskj.cn

================================================================================
来源：http://bw.nszjky.cn

[B01] 条件判断 if / else
来源：http://cz.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ra.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jc.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jf.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ui.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mi.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tk.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cp.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kj.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://vk.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uz.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qn.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://le.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nj.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nw.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.szxytkj.cn

[B03] switch / match / case
来源：http://ox.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kd.wgjwhj.cn


<!-- 参考信息 -->