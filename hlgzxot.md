代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jj.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ml.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://or.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vn.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eb.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ba.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zy.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ri.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qn.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zq.yuntaijiaju.cn

【文件统计】
来源：http://dw.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bl.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://nk.jctech888.com.cn

目  录
来源：http://mm.colortex.cn

--------------------------------------------------------------------------------
来源：http://bg.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rz.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fz.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bw.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lq.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cm.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pa.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dy.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zy.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nq.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hg.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hd.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zo.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tp.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qn.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mm.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rd.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://es.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ri.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://em.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hp.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dm.yuntaijiaju.cn

================================================================================
来源：http://le.jianghongdianzi.cn

A. 基础语法与类型
来源：http://rq.9csxet.cn

================================================================================
来源：http://ok.nicolike.cn

[A01] Hello World
来源：http://ok.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://iu.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://uk.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ol.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://co.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://si.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://db.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://ty.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fa.shxzukj.cn

[A02] 变量声明与赋值
来源：http://mt.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uh.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xa.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ab.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://px.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://vb.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://ph.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://yh.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kc.shtwfgs.cn

[A03] 常量定义
来源：http://qb.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kk.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://wf.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://uv.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://ee.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://az.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://st.shxzukj.cn

Ruby: PI = 3.14159
来源：http://rs.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://hu.bjjhwx.cn

[A04] 判断变量类型
来源：http://aq.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tt.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ts.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rb.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://sj.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rh.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ga.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hd.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://xj.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://md.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gr.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://su.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vg.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dl.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://xq.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://hj.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://fl.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://ae.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://hk.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://is.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zx.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://za.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://os.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tc.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ur.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hd.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qm.shtwfgs.cn

[A07] 数字转字符串
来源：http://me.hnjuh.cn

Py:   str(42)
来源：http://lj.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://tc.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://sj.hahajie.cn

TS:   String(42)
来源：http://uq.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ra.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://hl.huixiangedu.cn

Ruby: 42.to_s
来源：http://kl.huixiangedu.cn

C#:   42.ToString()
来源：http://ah.hahajie.cn

[A08] 取整与四舍五入
来源：http://go.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rm.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dt.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fp.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lz.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gj.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dc.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://po.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ba.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ja.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://in.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ma.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jt.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ud.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jr.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sm.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mw.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wh.hahajie.cn

[A10] 生成随机数
来源：http://ka.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://st.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://fr.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xg.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://si.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://vz.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xd.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://ks.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://pl.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://kq.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://ci.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ac.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bg.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tp.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://gg.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://em.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tw.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sg.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://hr.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sm.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ai.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://ed.asd995.cn

TS:   `Hello, ${name}!`
来源：http://aw.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://we.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ig.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://km.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://cj.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://aw.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://ba.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://vr.szsharing.cn

JS:   "第一行\n第二行"
来源：http://px.nicolike.cn

TS:   "第一行\n第二行"
来源：http://iw.asd995.cn

Java: "第一行\n第二行"
来源：http://wb.nicolike.cn

Go:   "第一行\n第二行"
来源：http://sb.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://fw.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://nx.9csxet.cn

[A14] 注释写法
来源：http://wp.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sl.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eg.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://he.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://bj.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tq.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://md.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ok.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://uj.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ls.panjiajie.cn

Py:   value = data or "默认值"
来源：http://jr.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://ts.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://gl.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://dc.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iq.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://fa.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://gl.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://wl.hnjuh.cn

[A16] 真假值判断规则
来源：http://ix.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kl.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gy.shxzskj.cn

TS:   if (!x) {}
来源：http://rp.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bi.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ay.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ab.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cw.gzmigu.cn

[A17] 位运算
来源：http://am.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oc.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://od.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xe.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ps.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wd.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ty.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yr.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ve.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://jr.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://xh.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://bv.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ob.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cg.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://sf.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kz.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ce.asd995.cn

C#:   (int)'A'; (char)65
来源：http://dj.panjiajie.cn

[A19] 交换两个变量
来源：http://no.wgjwhj.cn

Py:   a, b = b, a
来源：http://gh.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cz.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://nb.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://by.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://eo.panjiajie.cn

Go:   a, b = b, a
来源：http://py.521024.cn

Ruby: a, b = b, a
来源：http://nk.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://ce.jctech888.com.cn

[A20] 读取标准输入
来源：http://ez.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://sf.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cq.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zl.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://lw.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://jj.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gh.newstarts.cn

Ruby: gets.chomp
来源：http://iw.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://cp.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://tt.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://nc.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xb.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://zg.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://fs.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://jx.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xe.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://jg.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://wl.muxihuayi.cn

[A22] 获取字符串长度
来源：http://jk.9csxet.cn

Py:   len(s)
来源：http://mp.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mh.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://it.521024.cn

TS:   s.length
来源：http://yc.jctech888.com.cn

Java: s.length()
来源：http://nt.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fb.muxihuayi.cn

Ruby: s.length
来源：http://we.9csxet.cn

C#:   s.Length
来源：http://ja.gzmigu.cn

[A23] 大小写转换
来源：http://eu.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gi.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://je.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lk.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yc.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mi.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ii.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qe.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://le.haigaiapp.cn

[A24] 去除首尾空白
来源：http://fa.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nx.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://in.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://la.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mf.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uu.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hf.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://st.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rd.jctech888.com.cn

[A25] 字符串比较
来源：http://si.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://tn.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nv.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aw.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dg.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lq.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vp.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cn.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ef.colortex.cn

[A26] 类型转换总览
来源：http://ol.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zj.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ey.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wa.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ka.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qi.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://od.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wf.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ey.jctech888.com.cn

================================================================================
来源：http://rq.panjiajie.cn

B. 流程控制
来源：http://aq.colortex.cn

================================================================================
来源：http://pa.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://am.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mg.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ue.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iu.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jf.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gh.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://db.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pw.521024.cn

[B02] 多分支 else if / elif
来源：http://kf.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rb.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fe.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gb.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zk.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.asd995.cn

[B03] switch / match / case
来源：http://hy.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ly.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lm.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nt.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ij.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rd.muxihuayi.cn


<!-- 参考信息 -->