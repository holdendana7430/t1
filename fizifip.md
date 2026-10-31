代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zp.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ez.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zp.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://if.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hl.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cz.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vh.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pe.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ha.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yp.muxihuayi.cn

【文件统计】
来源：http://fa.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ya.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zg.panjiajie.cn

目  录
来源：http://zc.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://gb.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oe.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tt.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kf.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nk.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gv.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rc.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ie.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xv.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hu.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sh.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://da.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hg.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kl.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tg.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jg.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lq.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cf.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ba.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bi.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ub.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zb.huixinmuqiang.cn

================================================================================
来源：http://pi.hahajie.cn

A. 基础语法与类型
来源：http://ds.yuntaijiaju.cn

================================================================================
来源：http://xt.shtwfgs.cn

[A01] Hello World
来源：http://rf.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://fl.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://fy.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://cn.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ru.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://vo.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://gc.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://gq.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vx.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://bo.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cy.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://we.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://by.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dp.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://wt.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://jb.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://ce.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://et.newstarts.cn

[A03] 常量定义
来源：http://oy.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cs.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://rr.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://lk.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://cp.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://dw.hnjuh.cn

Go:   const PI = 3.14159
来源：http://xn.lnxyls.cn

Ruby: PI = 3.14159
来源：http://zh.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://fl.lnxyls.cn

[A04] 判断变量类型
来源：http://tk.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gz.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rw.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dq.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://cb.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dz.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rn.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://os.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://db.nicolike.cn

[A05] 整数除法与取模
来源：http://kh.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ls.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zq.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cf.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fa.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://uv.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://tg.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hh.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://is.newstarts.cn

[A06] 字符串转数字
来源：http://dj.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://qe.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ws.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wa.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uq.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uy.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mv.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sz.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hv.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://wy.huixiangedu.cn

Py:   str(42)
来源：http://uu.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://ql.newstarts.cn

JS:   String(42); (42).toString()
来源：http://te.lnxyls.cn

TS:   String(42)
来源：http://qy.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zd.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://re.lnxyls.cn

Ruby: 42.to_s
来源：http://nc.yuntaijiaju.cn

C#:   42.ToString()
来源：http://xd.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://ze.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cf.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sg.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zi.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wg.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ls.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ek.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qd.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tv.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://au.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bh.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sz.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fb.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ap.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ul.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ac.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pq.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://am.hnjuh.cn

[A10] 生成随机数
来源：http://pk.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://lr.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://dx.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://az.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://au.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://qb.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pz.jctech888.com.cn

Ruby: rand(1..100)
来源：http://bd.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://st.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://yd.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://od.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hh.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pk.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lo.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ny.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://io.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uv.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vj.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://gt.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gg.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mq.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://ma.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://tv.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://gt.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ze.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://bt.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://vz.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mv.9csxet.cn

Py:   "第一行\n第二行"
来源：http://th.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://nt.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://tt.nszjky.cn

TS:   "第一行\n第二行"
来源：http://vb.newstarts.cn

Java: "第一行\n第二行"
来源：http://xb.colortex.cn

Go:   "第一行\n第二行"
来源：http://aq.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://ff.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://aj.huanxung.cn

[A14] 注释写法
来源：http://rq.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pm.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ma.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://nx.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://qf.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://az.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://wr.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://si.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://kl.szsharing.cn

[A15] 空值判断与默认值
来源：http://fg.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://ma.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ud.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://cz.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://co.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mu.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://xf.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://ke.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://or.9csxet.cn

[A16] 真假值判断规则
来源：http://in.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wr.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ro.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ui.bookmarksfly.cn

TS:   if (!x) {}
来源：http://te.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qz.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sg.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lr.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ff.haigaiapp.cn

[A17] 位运算
来源：http://xs.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cf.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://se.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sb.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pg.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uj.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bn.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://jp.colortex.cn

Py:   ord("A"); chr(65)
来源：http://fu.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ry.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pt.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ak.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://yz.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ry.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://kl.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://qv.bjjhwx.cn

[A19] 交换两个变量
来源：http://bp.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://id.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ok.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://by.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://db.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://zx.colortex.cn

Go:   a, b = b, a
来源：http://xr.jctech888.com.cn

Ruby: a, b = b, a
来源：http://qr.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://rb.bjjhwx.cn

[A20] 读取标准输入
来源：http://kp.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://xh.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lm.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eb.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://py.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://xt.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nc.asd995.cn

Ruby: gets.chomp
来源：http://gw.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://ak.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://hd.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://fj.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xu.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://bx.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://pn.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://mk.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ca.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://su.521024.cn

C#:   3.14159.ToString("F2")
来源：http://tf.szxytkj.cn

[A22] 获取字符串长度
来源：http://av.bjjhwx.cn

Py:   len(s)
来源：http://mn.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gf.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rp.huixiangedu.cn

TS:   s.length
来源：http://hu.szxytkj.cn

Java: s.length()
来源：http://of.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qj.yuntaijiaju.cn

Ruby: s.length
来源：http://mt.szxytkj.cn

C#:   s.Length
来源：http://ae.shxzskj.cn

[A23] 大小写转换
来源：http://zv.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ei.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ry.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cd.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dp.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xq.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ka.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lx.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ms.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://tt.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://po.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gp.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://at.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rj.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://wv.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iy.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ea.gzmigu.cn

[A25] 字符串比较
来源：http://ib.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://xg.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fw.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kc.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gv.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yq.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sv.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rp.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kr.panjiajie.cn

[A26] 类型转换总览
来源：http://ad.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kq.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://en.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gb.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://zq.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ft.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yv.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lc.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wg.huanxung.cn

================================================================================
来源：http://qw.yuexingan06.cn

B. 流程控制
来源：http://wq.9csxet.cn

================================================================================
来源：http://qw.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://kn.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vr.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mc.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lg.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://js.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://da.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://re.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://za.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://il.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://nd.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qj.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://om.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fm.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fu.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jk.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.bjjhwx.cn

[B03] switch / match / case
来源：http://ld.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ln.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ue.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ho.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xj.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ho.jianghongdianzi.cn


<!-- 参考信息 -->