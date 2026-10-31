代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eh.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gh.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ae.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mw.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mk.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vg.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qq.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pd.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://co.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pa.lnxyls.cn

【文件统计】
来源：http://qk.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cq.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://fi.hahajie.cn

目  录
来源：http://yz.nszjky.cn

--------------------------------------------------------------------------------
来源：http://qe.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xi.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://we.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ao.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ah.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sh.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fw.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sk.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fi.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qb.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dh.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ut.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kj.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zg.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://to.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pr.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ms.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ll.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ck.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fd.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://va.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ah.panjiajie.cn

================================================================================
来源：http://vs.bjjhwx.cn

A. 基础语法与类型
来源：http://nv.yuntaijiaju.cn

================================================================================
来源：http://az.jianghongdianzi.cn

[A01] Hello World
来源：http://eq.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://bu.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://nd.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://je.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jg.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://fl.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://wq.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://dx.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oh.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://dp.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://li.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rb.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hk.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ys.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://qj.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://uk.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://gp.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ty.bjjhwx.cn

[A03] 常量定义
来源：http://cy.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ye.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ri.9csxet.cn

JS:   const PI = 3.14159;
来源：http://vt.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://hc.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://oa.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://hb.nszjky.cn

Ruby: PI = 3.14159
来源：http://aq.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://ox.jctech888.com.cn

[A04] 判断变量类型
来源：http://rv.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tg.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cp.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xd.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://jj.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vg.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xb.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gs.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://fy.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://ni.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://al.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xv.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hn.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xp.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://pj.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://eo.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ob.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://cp.colortex.cn

[A06] 字符串转数字
来源：http://yy.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://dg.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kt.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ri.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://st.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bj.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xv.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vu.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dd.9csxet.cn

[A07] 数字转字符串
来源：http://qk.nicolike.cn

Py:   str(42)
来源：http://uh.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://kj.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://ip.yuntaijiaju.cn

TS:   String(42)
来源：http://bs.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://or.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://tl.bookmarksfly.cn

Ruby: 42.to_s
来源：http://ry.panjiajie.cn

C#:   42.ToString()
来源：http://ib.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://uu.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://te.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ay.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ke.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jx.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tp.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://od.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eq.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ym.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://eg.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ib.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mr.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ly.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://no.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://md.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ot.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nv.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tz.huixiangedu.cn

[A10] 生成随机数
来源：http://jo.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://gp.szsharing.cn

PHP:  random_int(1, 100);
来源：http://bc.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sn.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rn.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://dg.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iw.hnjuh.cn

Ruby: rand(1..100)
来源：http://gw.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://ei.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://wx.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://mu.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://be.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://af.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ea.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://il.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bn.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dh.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vf.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://sy.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xz.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kk.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://as.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://qf.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://pw.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kz.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://fw.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://wx.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hq.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://yi.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://tv.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://ex.szsharing.cn

TS:   "第一行\n第二行"
来源：http://kl.asd995.cn

Java: "第一行\n第二行"
来源：http://hd.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://vm.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://de.newstarts.cn

C#:   "第一行\n第二行"
来源：http://gn.szxytkj.cn

[A14] 注释写法
来源：http://je.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qa.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tr.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ko.521024.cn

TS:   // 单行；/* 多行 */
来源：http://qy.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tb.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://ap.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dc.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://ni.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://ev.shxzskj.cn

Py:   value = data or "默认值"
来源：http://pu.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://cc.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://ri.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://fs.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ti.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://yt.521024.cn

Ruby: value = data || "默认值"
来源：http://px.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://yc.szxytkj.cn

[A16] 真假值判断规则
来源：http://cz.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vg.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://no.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jy.szxytkj.cn

TS:   if (!x) {}
来源：http://ba.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ne.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uh.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wg.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uy.panjiajie.cn

[A17] 位运算
来源：http://yw.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hh.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://um.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ag.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://up.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fh.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://wc.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ad.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://jh.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://he.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://as.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://dm.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wq.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://ie.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://jr.chemitech.net.cn

[A19] 交换两个变量
来源：http://hw.newstarts.cn

Py:   a, b = b, a
来源：http://jd.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ru.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://si.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://ch.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://dl.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://fu.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ac.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://pn.wgjwhj.cn

[A20] 读取标准输入
来源：http://zm.hnjuh.cn

Py:   name = input("请输入：")
来源：http://gt.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ok.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pk.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://kl.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://bg.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cj.huanxung.cn

Ruby: gets.chomp
来源：http://ch.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://sp.szsharing.cn

[A21] 保留指定小数位输出
来源：http://pe.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ky.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mc.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://gj.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://hc.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://es.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zi.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://rv.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://qg.huixiangedu.cn

[A22] 获取字符串长度
来源：http://us.yuntaijiaju.cn

Py:   len(s)
来源：http://yd.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jg.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bx.521024.cn

TS:   s.length
来源：http://lp.colortex.cn

Java: s.length()
来源：http://jw.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nr.huixiangedu.cn

Ruby: s.length
来源：http://tr.huixiangedu.cn

C#:   s.Length
来源：http://gg.colortex.cn

[A23] 大小写转换
来源：http://lo.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bh.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kl.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vh.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wt.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bz.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qt.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wr.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nj.szxytkj.cn

[A24] 去除首尾空白
来源：http://wj.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jk.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ho.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://al.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://el.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://qf.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ax.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ul.huanxung.cn

[A25] 字符串比较
来源：http://uh.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://nj.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sb.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iu.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gu.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zs.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ek.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lw.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fm.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://lo.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nt.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://in.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yb.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://jh.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cx.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mk.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vz.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cl.szxytkj.cn

================================================================================
来源：http://ph.asd995.cn

B. 流程控制
来源：http://re.huixinmuqiang.cn

================================================================================
来源：http://pe.521024.cn

[B01] 条件判断 if / else
来源：http://mw.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ds.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nw.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xu.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ym.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aj.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vn.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dt.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hv.asd995.cn

[B02] 多分支 else if / elif
来源：http://yr.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tv.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ug.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yf.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wz.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hu.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.nszjky.cn

[B03] switch / match / case
来源：http://ov.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://up.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ua.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bt.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dx.szxytkj.cn


<!-- 参考信息 -->