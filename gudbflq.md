代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zq.hnjuh.cn

【使用说明】
来源：http://cv.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nv.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://on.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pk.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ax.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zr.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fu.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nj.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ob.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nh.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dj.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://us.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://km.yuntaijiaju.cn

【文件统计】
来源：http://sl.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ik.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://jo.jianghongdianzi.cn

目  录
来源：http://jw.newstarts.cn

--------------------------------------------------------------------------------
来源：http://xn.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ff.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fs.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fz.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pp.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ug.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cx.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jd.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kf.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eq.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sb.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mw.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bt.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sn.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ab.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zu.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xv.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ge.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sc.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dz.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sv.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ca.shxzskj.cn

================================================================================
来源：http://co.huixinmuqiang.cn

A. 基础语法与类型
来源：http://xh.szsharing.cn

================================================================================
来源：http://xn.lnxyls.cn

[A01] Hello World
来源：http://js.newstarts.cn

Py:   print("Hello, World!")
来源：http://xx.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://sd.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://hi.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tn.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://sk.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://fz.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://qp.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fx.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://gd.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kb.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dz.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pg.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zy.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://yg.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://ek.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://ma.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gy.bjjhwx.cn

[A03] 常量定义
来源：http://xe.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tg.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://sd.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ny.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://bz.asd995.cn

Java: static final double PI = 3.14159;
来源：http://uq.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://xp.shxzukj.cn

Ruby: PI = 3.14159
来源：http://tb.521024.cn

C#:   const double PI = 3.14159;
来源：http://wo.jctech888.com.cn

[A04] 判断变量类型
来源：http://do.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tk.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ex.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gn.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://zm.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jj.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hk.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vf.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://nt.panjiajie.cn

[A05] 整数除法与取模
来源：http://oq.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hw.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://eo.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://za.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xd.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://rw.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://xx.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://vp.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://tx.huanxung.cn

[A06] 字符串转数字
来源：http://vk.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://fo.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mc.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zs.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pz.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qr.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bb.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://de.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pt.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://pg.panjiajie.cn

Py:   str(42)
来源：http://md.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://rn.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ol.shxzskj.cn

TS:   String(42)
来源：http://ln.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ve.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://pq.shtwfgs.cn

Ruby: 42.to_s
来源：http://ry.yuntaijiaju.cn

C#:   42.ToString()
来源：http://ck.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://pn.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oo.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ok.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bz.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ck.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pw.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rj.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ua.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vk.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://wc.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xf.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ao.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dc.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mu.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ho.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gn.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kn.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mz.szxytkj.cn

[A10] 生成随机数
来源：http://pl.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://gk.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://gm.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ce.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ed.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://ei.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mx.jctech888.com.cn

Ruby: rand(1..100)
来源：http://hk.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://bj.huanxung.cn

[A11] 条件表达式（三元）
来源：http://ix.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://wz.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ce.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ya.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ec.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://wd.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://et.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nj.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rg.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://mj.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qb.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dz.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://bm.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://ke.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://ys.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mp.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://tl.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://uf.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://be.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://bd.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ye.9csxet.cn

JS:   "第一行\n第二行"
来源：http://he.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://df.panjiajie.cn

Java: "第一行\n第二行"
来源：http://ru.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://cc.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://zp.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://qd.yuexingan06.cn

[A14] 注释写法
来源：http://ui.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://km.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wa.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://am.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://gi.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ap.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://ct.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xc.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://sb.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://bq.gzmigu.cn

Py:   value = data or "默认值"
来源：http://pv.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://zx.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ls.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://fm.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lp.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://aq.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://qw.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://aq.szsharing.cn

[A16] 真假值判断规则
来源：http://rv.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bb.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wu.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xt.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://qb.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fc.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wm.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pm.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://je.yuntaijiaju.cn

[A17] 位运算
来源：http://jv.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hd.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mk.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kz.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bo.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://vd.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://sb.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://xh.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ad.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jn.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://go.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tc.521024.cn

Ruby: "A".ord; 65.chr
来源：http://wz.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://vs.chemitech.net.cn

[A19] 交换两个变量
来源：http://vk.shtwfgs.cn

Py:   a, b = b, a
来源：http://rv.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rh.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://yo.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://fa.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://lg.lnxyls.cn

Go:   a, b = b, a
来源：http://lf.shxzskj.cn

Ruby: a, b = b, a
来源：http://pp.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://rg.shxzukj.cn

[A20] 读取标准输入
来源：http://wx.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://cw.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rc.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://mk.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://xq.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://so.gzmigu.cn

Ruby: gets.chomp
来源：http://ie.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://ru.szsharing.cn

[A21] 保留指定小数位输出
来源：http://ho.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://ga.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xn.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://pw.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://mz.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://rb.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yq.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://qc.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://my.haigaiapp.cn

[A22] 获取字符串长度
来源：http://yp.huixinmuqiang.cn

Py:   len(s)
来源：http://wc.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://je.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fv.gzmigu.cn

TS:   s.length
来源：http://wo.hahajie.cn

Java: s.length()
来源：http://jn.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vb.jctech888.com.cn

Ruby: s.length
来源：http://sv.haigaiapp.cn

C#:   s.Length
来源：http://kw.huixiangedu.cn

[A23] 大小写转换
来源：http://dl.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ix.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rv.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zi.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hc.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gi.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lq.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xv.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gd.asd995.cn

[A24] 去除首尾空白
来源：http://pi.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xt.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mn.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ek.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nm.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zz.521024.cn

Go:   strings.TrimSpace(s)
来源：http://qu.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uy.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zb.panjiajie.cn

[A25] 字符串比较
来源：http://su.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://fm.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ay.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kp.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://om.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://es.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wq.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bi.haigaiapp.cn

[A26] 类型转换总览
来源：http://wm.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ua.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cb.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mg.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://yn.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lg.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wd.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tq.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dv.huixiangedu.cn

================================================================================
来源：http://mq.lnxyls.cn

B. 流程控制
来源：http://po.szsharing.cn

================================================================================
来源：http://uj.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://ip.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aq.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ko.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mc.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cn.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dd.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ay.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ru.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wp.hahajie.cn

[B02] 多分支 else if / elif
来源：http://jp.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ci.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rf.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ba.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://th.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tt.nicolike.cn

[B03] switch / match / case
来源：http://wg.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ss.nszjky.cn


<!-- 参考信息 -->