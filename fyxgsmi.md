代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gp.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xq.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ym.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fn.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jj.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://de.szsharing.cn

【文件统计】
来源：http://rs.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lw.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://qu.panjiajie.cn

目  录
来源：http://fx.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://kp.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xb.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zl.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rm.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mz.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bq.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nd.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://om.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gq.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ln.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ni.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qh.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ym.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mq.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vu.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hf.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cq.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pl.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rr.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bs.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qq.asd995.cn

================================================================================
来源：http://an.huixinmuqiang.cn

A. 基础语法与类型
来源：http://nu.bookmarksfly.cn

================================================================================
来源：http://oz.nszjky.cn

[A01] Hello World
来源：http://xk.colortex.cn

Py:   print("Hello, World!")
来源：http://ms.521024.cn

PHP:  echo "Hello, World!";
来源：http://yy.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ce.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qi.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://fr.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://ff.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://ff.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rt.asd995.cn

[A02] 变量声明与赋值
来源：http://wr.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://li.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bj.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wj.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ae.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://if.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://pb.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://pf.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nw.muxihuayi.cn

[A03] 常量定义
来源：http://ii.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ck.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://nn.9csxet.cn

JS:   const PI = 3.14159;
来源：http://jx.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://az.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://nk.szxytkj.cn

Go:   const PI = 3.14159
来源：http://sx.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://dt.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://yi.yuexingan06.cn

[A04] 判断变量类型
来源：http://xe.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sc.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wc.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fj.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://lh.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ib.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kv.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nh.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://hd.nszjky.cn

[A05] 整数除法与取模
来源：http://ca.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ui.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://no.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fh.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://si.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://dd.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://to.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://qq.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://nw.9csxet.cn

[A06] 字符串转数字
来源：http://to.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://vr.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wk.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fj.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vn.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ck.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vq.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yq.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rm.9csxet.cn

[A07] 数字转字符串
来源：http://gi.haigaiapp.cn

Py:   str(42)
来源：http://ea.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://ss.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://kn.muxihuayi.cn

TS:   String(42)
来源：http://ki.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oi.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://ol.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://dj.huixiangedu.cn

C#:   42.ToString()
来源：http://yc.szsharing.cn

[A08] 取整与四舍五入
来源：http://mu.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bz.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wa.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://en.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ll.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pw.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xe.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xi.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ai.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://cu.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://up.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kn.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://va.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pg.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vd.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xk.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lq.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ib.wgjwhj.cn

[A10] 生成随机数
来源：http://zo.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ko.hahajie.cn

PHP:  random_int(1, 100);
来源：http://yf.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sa.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://of.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://zx.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mr.huixiangedu.cn

Ruby: rand(1..100)
来源：http://ji.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://ll.nicolike.cn

[A11] 条件表达式（三元）
来源：http://vx.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://dg.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ym.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yt.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wq.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://bu.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wm.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tx.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sw.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://ya.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wp.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yv.521024.cn

JS:   `Hello, ${name}!`
来源：http://ei.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://tz.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://dj.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fv.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://zu.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://fx.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uv.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://rf.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://py.szsharing.cn

JS:   "第一行\n第二行"
来源：http://xl.colortex.cn

TS:   "第一行\n第二行"
来源：http://bl.nszjky.cn

Java: "第一行\n第二行"
来源：http://up.huanxung.cn

Go:   "第一行\n第二行"
来源：http://ze.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://hb.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://oj.shxzukj.cn

[A14] 注释写法
来源：http://hf.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lu.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gs.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://fx.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://qb.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pe.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://hc.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kl.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://nq.asd995.cn

[A15] 空值判断与默认值
来源：http://du.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://xm.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://mw.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://mx.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://pd.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://up.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://cl.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://ew.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://vs.nicolike.cn

[A16] 真假值判断规则
来源：http://tz.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ay.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pf.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xz.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://ly.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zt.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gh.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kw.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wc.bookmarksfly.cn

[A17] 位运算
来源：http://cu.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sv.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hm.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bl.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ed.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qu.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jo.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://jw.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://pc.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://qv.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nu.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wr.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://kf.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://po.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://pc.asd995.cn

C#:   (int)'A'; (char)65
来源：http://jc.bookmarksfly.cn

[A19] 交换两个变量
来源：http://md.shxzukj.cn

Py:   a, b = b, a
来源：http://ni.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ol.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://dx.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://go.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://jr.szxytkj.cn

Go:   a, b = b, a
来源：http://jh.haigaiapp.cn

Ruby: a, b = b, a
来源：http://yc.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://fz.muxihuayi.cn

[A20] 读取标准输入
来源：http://wd.9csxet.cn

Py:   name = input("请输入：")
来源：http://aa.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ur.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gn.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://zc.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://hv.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ta.bjjhwx.cn

Ruby: gets.chomp
来源：http://id.newstarts.cn

C#:   Console.ReadLine();
来源：http://tl.szsharing.cn

[A21] 保留指定小数位输出
来源：http://ic.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://wh.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zd.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ix.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://xg.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://nu.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ll.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://pu.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ph.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://sx.muxihuayi.cn

Py:   len(s)
来源：http://rd.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tk.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sh.shtwfgs.cn

TS:   s.length
来源：http://va.nicolike.cn

Java: s.length()
来源：http://rb.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jw.panjiajie.cn

Ruby: s.length
来源：http://ze.szxytkj.cn

C#:   s.Length
来源：http://az.muxihuayi.cn

[A23] 大小写转换
来源：http://yu.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yq.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gb.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ji.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oj.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fu.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://od.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://me.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ye.chemitech.net.cn

[A24] 去除首尾空白
来源：http://km.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://at.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nr.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wa.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://et.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bp.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://kx.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lk.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xa.bookmarksfly.cn

[A25] 字符串比较
来源：http://hu.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://cb.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bh.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jv.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mh.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vg.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gw.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mi.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hj.bookmarksfly.cn

[A26] 类型转换总览
来源：http://ow.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yx.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ar.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nu.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://lm.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fa.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tf.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://in.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eg.muxihuayi.cn

================================================================================
来源：http://po.gzmigu.cn

B. 流程控制
来源：http://zs.yuexingan06.cn

================================================================================
来源：http://rg.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://tw.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fh.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tg.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yl.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uu.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://km.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://py.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hc.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ye.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://qo.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gw.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kl.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sp.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://en.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dz.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://te.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.szxytkj.cn

[B03] switch / match / case
来源：http://lg.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jb.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jm.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bn.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rl.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uh.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zb.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sh.huanxung.cn

[B04] for 计数循环
来源：http://dm.yuexingan06.cn


<!-- 参考信息 -->