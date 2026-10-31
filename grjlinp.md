代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kp.huixinmuqiang.cn

【使用说明】
来源：http://mu.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dv.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ur.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ab.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aa.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lq.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aw.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://na.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qz.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oo.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sn.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ar.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qb.bjjhwx.cn

【文件统计】
来源：http://cl.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kg.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://pj.yuexingan06.cn

目  录
来源：http://wd.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ya.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hn.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gn.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xi.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ax.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uy.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bw.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ag.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uv.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tx.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zr.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sp.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cv.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gq.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ix.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cg.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mv.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kr.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dt.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mr.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jr.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://km.jianghongdianzi.cn

================================================================================
来源：http://lh.gzmigu.cn

A. 基础语法与类型
来源：http://ff.szxytkj.cn

================================================================================
来源：http://tl.panjiajie.cn

[A01] Hello World
来源：http://qf.szxytkj.cn

Py:   print("Hello, World!")
来源：http://ar.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://cb.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://hf.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tz.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://jb.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://if.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://ep.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ie.hahajie.cn

[A02] 变量声明与赋值
来源：http://hi.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://px.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jo.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://um.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fx.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://iz.521024.cn

Go:   name := "Alex"; age := 20
来源：http://zm.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://mm.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uz.hahajie.cn

[A03] 常量定义
来源：http://ui.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sp.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://qs.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://xq.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://ym.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://xc.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://rt.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://dd.521024.cn

C#:   const double PI = 3.14159;
来源：http://iy.hahajie.cn

[A04] 判断变量类型
来源：http://xk.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fg.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jx.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nm.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://ul.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kz.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gv.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qp.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://ol.gzmigu.cn

[A05] 整数除法与取模
来源：http://iu.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lz.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bc.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://us.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dj.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://bu.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://zj.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://pv.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://xn.shtwfgs.cn

[A06] 字符串转数字
来源：http://zd.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://gh.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gv.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gz.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kq.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zo.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gb.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ys.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xw.szsharing.cn

[A07] 数字转字符串
来源：http://ih.newstarts.cn

Py:   str(42)
来源：http://kl.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://zk.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://nc.bookmarksfly.cn

TS:   String(42)
来源：http://zb.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fn.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://yc.521024.cn

Ruby: 42.to_s
来源：http://gb.bjjhwx.cn

C#:   42.ToString()
来源：http://sw.521024.cn

[A08] 取整与四舍五入
来源：http://oq.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jy.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bx.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zh.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kg.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vw.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hx.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gb.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gm.521024.cn

[A09] 绝对值与最大最小值
来源：http://vm.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cf.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ku.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kt.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ds.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fs.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fm.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ct.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ke.521024.cn

[A10] 生成随机数
来源：http://qp.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://qf.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://rd.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tr.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ae.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://fh.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vw.hnjuh.cn

Ruby: rand(1..100)
来源：http://wj.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://zq.asd995.cn

[A11] 条件表达式（三元）
来源：http://iv.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ax.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://al.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xq.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rk.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://dt.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pg.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lp.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kk.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://zg.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zs.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tk.asd995.cn

JS:   `Hello, ${name}!`
来源：http://sk.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://fg.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://me.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jj.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://cn.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ci.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ra.colortex.cn

Py:   "第一行\n第二行"
来源：http://fr.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ne.nszjky.cn

JS:   "第一行\n第二行"
来源：http://sr.nszjky.cn

TS:   "第一行\n第二行"
来源：http://vz.521024.cn

Java: "第一行\n第二行"
来源：http://uy.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://lm.asd995.cn

Ruby: "第一行\n第二行"
来源：http://tq.9csxet.cn

C#:   "第一行\n第二行"
来源：http://pq.hahajie.cn

[A14] 注释写法
来源：http://ij.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zp.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ab.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://by.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://ky.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cp.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://gy.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oc.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://dl.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://sh.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://ka.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://vr.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://na.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://mq.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mm.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://bc.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ea.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://qn.shtwfgs.cn

[A16] 真假值判断规则
来源：http://dw.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://of.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qh.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cs.huixiangedu.cn

TS:   if (!x) {}
来源：http://ly.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qf.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ep.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ox.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mj.9csxet.cn

[A17] 位运算
来源：http://bw.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rk.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ip.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pe.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yp.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lk.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://su.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://xp.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://gk.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://az.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ds.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pq.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ly.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sn.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://ci.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://hi.lnxyls.cn

[A19] 交换两个变量
来源：http://uj.gzmigu.cn

Py:   a, b = b, a
来源：http://hs.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://fe.521024.cn

TS:   [a, b] = [b, a];
来源：http://ml.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://sb.colortex.cn

Go:   a, b = b, a
来源：http://we.hnjuh.cn

Ruby: a, b = b, a
来源：http://hg.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://ji.gzmigu.cn

[A20] 读取标准输入
来源：http://zo.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://bj.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ve.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wq.521024.cn

TS:   // Node.js：readline 模块
来源：http://ku.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://nw.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lz.huixiangedu.cn

Ruby: gets.chomp
来源：http://ek.newstarts.cn

C#:   Console.ReadLine();
来源：http://ly.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://ki.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ni.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tc.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://wa.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://pq.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://sf.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ps.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://ed.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ob.chemitech.net.cn

[A22] 获取字符串长度
来源：http://jp.asd995.cn

Py:   len(s)
来源：http://rz.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kz.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ua.shxzskj.cn

TS:   s.length
来源：http://ld.haigaiapp.cn

Java: s.length()
来源：http://bv.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qy.nszjky.cn

Ruby: s.length
来源：http://ru.9csxet.cn

C#:   s.Length
来源：http://ql.chemitech.net.cn

[A23] 大小写转换
来源：http://pi.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ps.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://py.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fm.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hx.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pa.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mn.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qk.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fd.521024.cn

[A24] 去除首尾空白
来源：http://rk.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lk.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kt.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://md.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wi.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zj.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://pm.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cy.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nx.521024.cn

[A25] 字符串比较
来源：http://yu.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ze.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ch.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fg.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ls.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vi.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ch.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://le.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bh.szsharing.cn

[A26] 类型转换总览
来源：http://lm.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ix.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zv.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uc.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://kd.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ba.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ey.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vf.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nu.huixinmuqiang.cn

================================================================================
来源：http://lt.9csxet.cn

B. 流程控制
来源：http://tc.panjiajie.cn

================================================================================
来源：http://yr.lnxyls.cn

[B01] 条件判断 if / else
来源：http://ez.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jc.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ni.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ed.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cc.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ux.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lq.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jg.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uy.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://fd.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xw.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aq.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wk.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pr.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ys.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ou.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fa.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.lnxyls.cn

[B03] switch / match / case
来源：http://kx.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cq.bjjhwx.cn


<!-- 参考信息 -->