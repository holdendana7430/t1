代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nk.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zy.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iy.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dg.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hw.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xl.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kj.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wz.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ov.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cg.bookmarksfly.cn

【文件统计】
来源：http://ue.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mo.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://bg.muxihuayi.cn

目  录
来源：http://cf.asd995.cn

--------------------------------------------------------------------------------
来源：http://dz.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nc.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gx.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://um.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dm.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yn.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ss.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pi.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aw.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qm.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rb.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ep.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uf.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ha.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jk.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gy.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sc.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://od.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ce.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gu.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rq.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nu.newstarts.cn

================================================================================
来源：http://sp.muxihuayi.cn

A. 基础语法与类型
来源：http://pi.newstarts.cn

================================================================================
来源：http://qg.panjiajie.cn

[A01] Hello World
来源：http://db.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ql.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://jr.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://ce.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gi.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://en.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://wf.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://wz.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://az.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://of.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uh.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://if.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dv.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zn.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://wy.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://tm.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cb.yuntaijiaju.cn

[A03] 常量定义
来源：http://ld.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xn.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://om.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ly.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://un.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://xb.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://ft.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://mp.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://vc.yuexingan06.cn

[A04] 判断变量类型
来源：http://bu.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ud.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wk.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sx.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://ol.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ow.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ty.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vv.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://fu.bjjhwx.cn

[A05] 整数除法与取模
来源：http://hx.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jy.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cd.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wt.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pf.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://gv.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://dm.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ge.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://ej.lnxyls.cn

[A06] 字符串转数字
来源：http://de.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://tj.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rf.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xo.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ar.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sk.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jh.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://me.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xg.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://dr.huanxung.cn

Py:   str(42)
来源：http://lt.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://to.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://or.jctech888.com.cn

TS:   String(42)
来源：http://yi.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mt.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://kq.colortex.cn

Ruby: 42.to_s
来源：http://ey.bjjhwx.cn

C#:   42.ToString()
来源：http://mb.newstarts.cn

[A08] 取整与四舍五入
来源：http://vw.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fh.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dc.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ac.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bf.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://im.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://up.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zc.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ks.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://nj.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aj.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mb.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sv.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ve.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fi.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jb.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vt.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jk.shtwfgs.cn

[A10] 生成随机数
来源：http://og.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://kr.nicolike.cn

PHP:  random_int(1, 100);
来源：http://bp.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pr.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bw.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://ef.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hb.521024.cn

Ruby: rand(1..100)
来源：http://br.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://dt.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://al.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://pc.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xg.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fj.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sd.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://xr.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wm.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ru.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://od.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://ro.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xl.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ns.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://vw.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://kv.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://sb.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yr.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://zh.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://js.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mt.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://pp.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://fo.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://ub.9csxet.cn

TS:   "第一行\n第二行"
来源：http://ah.hnjuh.cn

Java: "第一行\n第二行"
来源：http://gn.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://tf.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://hq.521024.cn

C#:   "第一行\n第二行"
来源：http://qg.colortex.cn

[A14] 注释写法
来源：http://ln.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cv.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://un.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://sk.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://dh.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hh.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://cr.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wu.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://ac.shxzskj.cn

[A15] 空值判断与默认值
来源：http://zs.hnjuh.cn

Py:   value = data or "默认值"
来源：http://zf.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://gf.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://ze.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://mx.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ae.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://sr.asd995.cn

Ruby: value = data || "默认值"
来源：http://pr.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://pw.nicolike.cn

[A16] 真假值判断规则
来源：http://ab.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mz.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ul.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xw.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://yg.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bx.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dd.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fd.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uc.panjiajie.cn

[A17] 位运算
来源：http://ww.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uf.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tg.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bk.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vx.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xb.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kj.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uv.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://nk.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://zp.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://oi.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kb.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nw.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://ba.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qj.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://ex.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://si.nszjky.cn

[A19] 交换两个变量
来源：http://yf.9csxet.cn

Py:   a, b = b, a
来源：http://rv.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://is.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://ih.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://zk.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://la.shtwfgs.cn

Go:   a, b = b, a
来源：http://je.shxzukj.cn

Ruby: a, b = b, a
来源：http://dh.521024.cn

C#:   (a, b) = (b, a);
来源：http://wo.newstarts.cn

[A20] 读取标准输入
来源：http://vw.colortex.cn

Py:   name = input("请输入：")
来源：http://rc.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rk.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wb.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ws.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://us.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vi.hahajie.cn

Ruby: gets.chomp
来源：http://ui.521024.cn

C#:   Console.ReadLine();
来源：http://ra.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ta.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://vq.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kt.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://db.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://op.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://li.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ku.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://bj.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://mf.nszjky.cn

[A22] 获取字符串长度
来源：http://sj.hahajie.cn

Py:   len(s)
来源：http://nr.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://an.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pa.shtwfgs.cn

TS:   s.length
来源：http://vd.hnjuh.cn

Java: s.length()
来源：http://fe.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gh.hnjuh.cn

Ruby: s.length
来源：http://ls.huixiangedu.cn

C#:   s.Length
来源：http://yu.colortex.cn

[A23] 大小写转换
来源：http://kw.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ht.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qk.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jb.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qi.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gf.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gr.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dz.521024.cn

[A24] 去除首尾空白
来源：http://sa.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://li.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ik.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fi.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ge.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sd.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://zc.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oq.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wc.muxihuayi.cn

[A25] 字符串比较
来源：http://hx.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://pu.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://la.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dm.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vj.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bx.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xc.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qv.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jp.shtwfgs.cn

[A26] 类型转换总览
来源：http://cr.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uz.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jj.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xo.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://qc.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bo.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lx.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hu.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dm.gzmigu.cn

================================================================================
来源：http://ep.gzmigu.cn

B. 流程控制
来源：http://qe.shxzukj.cn

================================================================================
来源：http://yg.colortex.cn

[B01] 条件判断 if / else
来源：http://hi.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hp.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vw.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://my.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vk.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qq.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nf.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vg.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pg.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ox.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dv.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ls.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ly.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wt.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oe.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.colortex.cn

[B03] switch / match / case
来源：http://ut.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://an.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xi.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://os.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yj.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qp.szsharing.cn


<!-- 参考信息 -->