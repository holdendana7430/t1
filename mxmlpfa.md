代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xr.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ep.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ws.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ax.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zn.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zz.szxytkj.cn

【文件统计】
来源：http://eh.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fu.nicolike.cn

--------------------------------------------------------------------------------
来源：http://pf.hahajie.cn

目  录
来源：http://qh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://pp.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://li.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://no.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mc.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gl.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bt.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hd.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uw.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ik.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ec.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bp.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xn.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yu.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://im.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://od.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fv.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rn.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bl.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://et.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bv.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pk.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hq.panjiajie.cn

================================================================================
来源：http://sy.yuntaijiaju.cn

A. 基础语法与类型
来源：http://tw.haigaiapp.cn

================================================================================
来源：http://mu.shxzukj.cn

[A01] Hello World
来源：http://lf.szsharing.cn

Py:   print("Hello, World!")
来源：http://dr.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://fx.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://ym.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dn.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://pa.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://vu.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://jz.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pm.colortex.cn

[A02] 变量声明与赋值
来源：http://pm.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gx.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fb.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oc.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wb.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://cu.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://cw.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://qw.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pm.asd995.cn

[A03] 常量定义
来源：http://ks.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jm.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://ge.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://pt.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://yc.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://cw.521024.cn

Go:   const PI = 3.14159
来源：http://lk.panjiajie.cn

Ruby: PI = 3.14159
来源：http://nw.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://em.hahajie.cn

[A04] 判断变量类型
来源：http://rh.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://em.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qv.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cn.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://wi.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://il.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ot.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zc.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://qg.hnjuh.cn

[A05] 整数除法与取模
来源：http://qq.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wj.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ih.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://et.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wv.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://me.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://kj.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://tg.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://uf.huanxung.cn

[A06] 字符串转数字
来源：http://xc.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ba.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pf.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gr.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wu.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ib.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qx.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zi.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qf.nicolike.cn

[A07] 数字转字符串
来源：http://ik.yuntaijiaju.cn

Py:   str(42)
来源：http://mb.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://eb.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://ka.chemitech.net.cn

TS:   String(42)
来源：http://fk.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ze.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://rt.jctech888.com.cn

Ruby: 42.to_s
来源：http://wg.jianghongdianzi.cn

C#:   42.ToString()
来源：http://up.nicolike.cn

[A08] 取整与四舍五入
来源：http://yq.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wd.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yn.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qh.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nh.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tg.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wu.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ao.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ul.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://ug.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://db.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ji.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cp.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oo.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qf.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pw.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zx.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wd.muxihuayi.cn

[A10] 生成随机数
来源：http://aw.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://rc.nszjky.cn

PHP:  random_int(1, 100);
来源：http://ft.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://md.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tn.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://lm.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zj.colortex.cn

Ruby: rand(1..100)
来源：http://iy.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://bc.huanxung.cn

[A11] 条件表达式（三元）
来源：http://hy.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://zt.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://go.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hr.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wc.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://lv.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ew.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cq.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pf.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://ua.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tn.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jj.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://mb.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://ib.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://yg.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zm.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://sp.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://oc.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zn.hahajie.cn

Py:   "第一行\n第二行"
来源：http://ya.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://wj.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://dv.szsharing.cn

TS:   "第一行\n第二行"
来源：http://jb.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://eh.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://iz.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://nw.colortex.cn

C#:   "第一行\n第二行"
来源：http://qc.bookmarksfly.cn

[A14] 注释写法
来源：http://cx.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ua.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ti.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://xw.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://cf.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fw.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://ix.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tz.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://lu.hahajie.cn

[A15] 空值判断与默认值
来源：http://qf.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://qf.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://pv.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://sd.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://jh.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wh.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://or.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://pz.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://kf.huanxung.cn

[A16] 真假值判断规则
来源：http://qs.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hx.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zw.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://is.hnjuh.cn

TS:   if (!x) {}
来源：http://oz.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ff.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sw.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nk.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kt.bjjhwx.cn

[A17] 位运算
来源：http://wr.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qs.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yd.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wd.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ol.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://it.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ze.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gh.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://so.521024.cn

Py:   ord("A"); chr(65)
来源：http://zn.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://yl.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yq.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zc.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://kf.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cd.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://tr.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://tf.gzmigu.cn

[A19] 交换两个变量
来源：http://ae.shxzukj.cn

Py:   a, b = b, a
来源：http://zh.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xa.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://gz.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://qc.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://xq.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://wt.huanxung.cn

Ruby: a, b = b, a
来源：http://xw.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://pl.huixiangedu.cn

[A20] 读取标准输入
来源：http://tm.9csxet.cn

Py:   name = input("请输入：")
来源：http://ne.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vp.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ya.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://gv.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://dh.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mv.wgjwhj.cn

Ruby: gets.chomp
来源：http://bs.hnjuh.cn

C#:   Console.ReadLine();
来源：http://lr.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://ib.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://lj.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dc.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://op.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://xj.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://fr.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cg.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ck.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://qg.521024.cn

[A22] 获取字符串长度
来源：http://tv.shxzskj.cn

Py:   len(s)
来源：http://cn.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yz.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fx.shxzukj.cn

TS:   s.length
来源：http://hw.gzmigu.cn

Java: s.length()
来源：http://gd.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xs.newstarts.cn

Ruby: s.length
来源：http://tw.muxihuayi.cn

C#:   s.Length
来源：http://zc.lnxyls.cn

[A23] 大小写转换
来源：http://ir.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cw.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dp.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mp.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rv.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://un.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gy.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ef.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pk.huanxung.cn

[A24] 去除首尾空白
来源：http://yc.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tx.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wu.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nq.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://el.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jr.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://zf.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://do.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kp.panjiajie.cn

[A25] 字符串比较
来源：http://zr.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ox.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://my.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://df.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tb.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hp.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ql.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gi.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cn.bookmarksfly.cn

[A26] 类型转换总览
来源：http://vh.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jp.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ss.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tr.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://lt.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qc.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://of.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://et.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vb.jctech888.com.cn

================================================================================
来源：http://ic.szsharing.cn

B. 流程控制
来源：http://jw.bjjhwx.cn

================================================================================
来源：http://ip.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://eo.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rn.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mg.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://la.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yn.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dc.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fe.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qr.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://pu.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wy.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://am.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ne.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qi.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fn.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vp.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://po.newstarts.cn

[B03] switch / match / case
来源：http://eo.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qo.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bh.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rf.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pg.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ze.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cr.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qi.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ks.jctech888.com.cn

[B04] for 计数循环
来源：http://wh.bookmarksfly.cn


<!-- 参考信息 -->