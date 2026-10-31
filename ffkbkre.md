代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vu.colortex.cn

【使用说明】
来源：http://cx.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gz.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kx.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ki.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hg.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mu.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qj.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rg.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fd.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ok.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jg.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wu.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nr.hahajie.cn

【文件统计】
来源：http://un.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://an.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ka.newstarts.cn

目  录
来源：http://vc.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://zt.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://di.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lk.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nk.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kr.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mb.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zf.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sw.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kt.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kt.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bo.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qw.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zn.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ai.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ob.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://us.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ag.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ur.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hv.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rf.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xq.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bn.muxihuayi.cn

================================================================================
来源：http://dc.lnxyls.cn

A. 基础语法与类型
来源：http://iv.muxihuayi.cn

================================================================================
来源：http://be.szsharing.cn

[A01] Hello World
来源：http://sp.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://mh.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://yo.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://eu.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ja.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://vg.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://da.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://fi.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dg.gzmigu.cn

[A02] 变量声明与赋值
来源：http://hd.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://et.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tq.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oy.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vy.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://mx.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://rk.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://ri.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cr.muxihuayi.cn

[A03] 常量定义
来源：http://ah.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://um.asd995.cn

PHP:  const PI = 3.14159;
来源：http://cu.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://gh.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://bo.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://mb.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://hn.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://zl.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://ik.9csxet.cn

[A04] 判断变量类型
来源：http://ud.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ut.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fc.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hm.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://za.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rx.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ah.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bp.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://pb.shxzskj.cn

[A05] 整数除法与取模
来源：http://he.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ls.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zk.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dp.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rk.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://lt.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://am.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://bz.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://vb.bookmarksfly.cn

[A06] 字符串转数字
来源：http://he.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://qg.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nt.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qq.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rt.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xd.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bg.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gt.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lf.gzmigu.cn

[A07] 数字转字符串
来源：http://ny.9csxet.cn

Py:   str(42)
来源：http://ji.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://sn.521024.cn

JS:   String(42); (42).toString()
来源：http://dn.haigaiapp.cn

TS:   String(42)
来源：http://tn.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rg.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://tz.lnxyls.cn

Ruby: 42.to_s
来源：http://gs.hahajie.cn

C#:   42.ToString()
来源：http://tt.nszjky.cn

[A08] 取整与四舍五入
来源：http://qc.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://we.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rp.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yz.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fv.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uy.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://az.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://te.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://um.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cf.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://du.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oi.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jh.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ne.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yj.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ar.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bb.bookmarksfly.cn

[A10] 生成随机数
来源：http://ud.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://gq.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://yu.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jd.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sc.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://jr.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ob.haigaiapp.cn

Ruby: rand(1..100)
来源：http://gs.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://bm.nicolike.cn

[A11] 条件表达式（三元）
来源：http://yl.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://bd.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cw.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dw.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nx.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://za.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tp.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bl.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pt.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://gm.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://df.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bf.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://qr.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://xh.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://iu.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fa.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://nn.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://ja.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ro.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://lo.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://hw.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://sr.nszjky.cn

TS:   "第一行\n第二行"
来源：http://vs.szxytkj.cn

Java: "第一行\n第二行"
来源：http://ue.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ln.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://qf.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://oj.jianghongdianzi.cn

[A14] 注释写法
来源：http://le.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wv.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xs.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://zr.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://vx.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vs.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://fc.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pk.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://rq.colortex.cn

[A15] 空值判断与默认值
来源：http://td.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://is.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://xz.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ir.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://cz.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ft.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://so.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://xs.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://mz.lnxyls.cn

[A16] 真假值判断规则
来源：http://ig.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ni.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qz.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ey.huixiangedu.cn

TS:   if (!x) {}
来源：http://dq.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hs.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eg.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ua.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hr.jianghongdianzi.cn

[A17] 位运算
来源：http://tm.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mb.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mv.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jn.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yk.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://np.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gr.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ym.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ue.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://rs.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://bh.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://mx.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nd.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ou.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://uw.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://le.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://gy.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://mr.bookmarksfly.cn

[A19] 交换两个变量
来源：http://sm.hnjuh.cn

Py:   a, b = b, a
来源：http://dl.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mr.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://pm.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://kg.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://cb.huanxung.cn

Go:   a, b = b, a
来源：http://qq.shtwfgs.cn

Ruby: a, b = b, a
来源：http://cb.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://aa.hnjuh.cn

[A20] 读取标准输入
来源：http://rr.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://su.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zs.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tz.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://dn.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://nb.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cf.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://bx.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ha.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://pd.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://uj.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cn.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://wu.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://wz.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://pr.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tt.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://ln.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://rw.9csxet.cn

[A22] 获取字符串长度
来源：http://gk.haigaiapp.cn

Py:   len(s)
来源：http://vp.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gq.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mo.yuexingan06.cn

TS:   s.length
来源：http://eq.shtwfgs.cn

Java: s.length()
来源：http://yc.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rd.huixiangedu.cn

Ruby: s.length
来源：http://yn.lnxyls.cn

C#:   s.Length
来源：http://oa.yuexingan06.cn

[A23] 大小写转换
来源：http://td.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://un.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ku.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ie.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mv.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ws.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uv.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uq.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pw.chemitech.net.cn

[A24] 去除首尾空白
来源：http://vz.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wi.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pb.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sy.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cc.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hf.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://gp.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zy.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rp.shxzukj.cn

[A25] 字符串比较
来源：http://fj.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://oh.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://us.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ex.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kd.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pi.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yp.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bo.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dh.shtwfgs.cn

[A26] 类型转换总览
来源：http://uv.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mt.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bh.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oy.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://oc.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tl.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rk.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ts.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qa.huixiangedu.cn

================================================================================
来源：http://mq.huixinmuqiang.cn

B. 流程控制
来源：http://ie.bookmarksfly.cn

================================================================================
来源：http://qd.shxzskj.cn

[B01] 条件判断 if / else
来源：http://rm.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rr.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aa.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pq.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bz.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fm.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iq.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mc.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://he.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://jk.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://df.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gw.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ls.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ub.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pt.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fx.yuexingan06.cn

[B03] switch / match / case
来源：http://mj.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fo.muxihuayi.cn


<!-- 参考信息 -->