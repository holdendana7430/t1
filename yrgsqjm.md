代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vt.shtwfgs.cn

【使用说明】
来源：http://io.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fx.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pb.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ma.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pk.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tk.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lf.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dr.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ac.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cj.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gi.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bx.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pz.gzmigu.cn

【文件统计】
来源：http://vq.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oc.9csxet.cn

--------------------------------------------------------------------------------
来源：http://it.bjjhwx.cn

目  录
来源：http://pg.nszjky.cn

--------------------------------------------------------------------------------
来源：http://na.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oc.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bj.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mh.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iv.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ao.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rp.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ef.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pu.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mh.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xr.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gn.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pk.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gu.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dy.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rb.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ts.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ty.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wd.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xa.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mz.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nu.lnxyls.cn

================================================================================
来源：http://fk.hnjuh.cn

A. 基础语法与类型
来源：http://bb.huixiangedu.cn

================================================================================
来源：http://tq.muxihuayi.cn

[A01] Hello World
来源：http://lk.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ki.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://ev.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://ju.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://na.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://qe.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://jc.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://ef.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sx.newstarts.cn

[A02] 变量声明与赋值
来源：http://fe.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qc.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ig.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jo.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yz.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://bq.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://ny.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://mb.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jt.colortex.cn

[A03] 常量定义
来源：http://qy.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pc.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://bb.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://fp.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://gr.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://gk.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://lj.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://wk.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://jv.gzmigu.cn

[A04] 判断变量类型
来源：http://br.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ln.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tv.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hs.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://zk.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wt.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zn.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zh.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://sq.hahajie.cn

[A05] 整数除法与取模
来源：http://yk.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rv.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wk.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vi.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wu.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://jq.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://bh.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://oi.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://qg.colortex.cn

[A06] 字符串转数字
来源：http://lb.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://kr.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hd.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bf.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://od.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wf.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kd.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://do.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ha.nicolike.cn

[A07] 数字转字符串
来源：http://sa.shxzukj.cn

Py:   str(42)
来源：http://gg.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://sz.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://jp.bjjhwx.cn

TS:   String(42)
来源：http://is.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mo.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://hx.hnjuh.cn

Ruby: 42.to_s
来源：http://mo.huixinmuqiang.cn

C#:   42.ToString()
来源：http://cn.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://yp.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jc.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ao.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hi.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qa.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fo.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bb.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://go.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ug.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://cq.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ck.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ca.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iu.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://la.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zs.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rn.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dz.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://du.haigaiapp.cn

[A10] 生成随机数
来源：http://jn.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://xr.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://xp.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tf.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gz.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://ej.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ck.shxzukj.cn

Ruby: rand(1..100)
来源：http://jn.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://ri.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://jr.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://fg.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xg.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ux.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ya.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://sn.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://su.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vj.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://az.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://br.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ed.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ty.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://dj.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://iz.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://da.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oa.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://cp.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://qn.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sx.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://ee.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://mx.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://lq.szsharing.cn

TS:   "第一行\n第二行"
来源：http://ih.lnxyls.cn

Java: "第一行\n第二行"
来源：http://gg.newstarts.cn

Go:   "第一行\n第二行"
来源：http://nf.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://uk.szsharing.cn

C#:   "第一行\n第二行"
来源：http://wa.shxzskj.cn

[A14] 注释写法
来源：http://km.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vf.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hd.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://sd.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://qe.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dt.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://sf.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ue.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://di.shxzskj.cn

[A15] 空值判断与默认值
来源：http://vl.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://iv.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://ti.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://vv.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://tg.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rj.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.huanxung.cn

Ruby: value = data || "默认值"
来源：http://vg.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://yz.huixiangedu.cn

[A16] 真假值判断规则
来源：http://tc.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ch.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gu.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pp.bookmarksfly.cn

TS:   if (!x) {}
来源：http://wf.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lp.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pz.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qr.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ff.yuexingan06.cn

[A17] 位运算
来源：http://xt.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kc.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://js.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ab.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tm.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rn.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://qi.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://bv.521024.cn

PHP:  ord("A"); chr(65)
来源：http://fy.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cv.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ss.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://wr.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xr.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://kt.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://gp.nicolike.cn

[A19] 交换两个变量
来源：http://rr.gzmigu.cn

Py:   a, b = b, a
来源：http://hj.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rn.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://rs.asd995.cn

TS:   [a, b] = [b, a];
来源：http://kp.521024.cn

Java: int t = a; a = b; b = t;
来源：http://ix.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://aj.shtwfgs.cn

Ruby: a, b = b, a
来源：http://cd.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://pb.haigaiapp.cn

[A20] 读取标准输入
来源：http://mo.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ku.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ph.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rg.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://sw.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://bp.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jb.9csxet.cn

Ruby: gets.chomp
来源：http://yo.hahajie.cn

C#:   Console.ReadLine();
来源：http://qe.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ey.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://of.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cm.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ci.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://qd.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://xc.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sq.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://mk.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://jz.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://vn.jianghongdianzi.cn

Py:   len(s)
来源：http://hy.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bu.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uz.9csxet.cn

TS:   s.length
来源：http://pa.haigaiapp.cn

Java: s.length()
来源：http://ou.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gn.gzmigu.cn

Ruby: s.length
来源：http://dr.hnjuh.cn

C#:   s.Length
来源：http://py.chemitech.net.cn

[A23] 大小写转换
来源：http://fb.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ru.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lo.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kb.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ly.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mm.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ni.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ah.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bj.colortex.cn

[A24] 去除首尾空白
来源：http://nn.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kx.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fw.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ik.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ky.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qf.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ng.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jb.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pw.szxytkj.cn

[A25] 字符串比较
来源：http://lz.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ar.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ow.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jt.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yl.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bw.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hn.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lx.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mz.szxytkj.cn

[A26] 类型转换总览
来源：http://io.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ge.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://va.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mw.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://pl.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://by.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wy.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vh.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://cm.jianghongdianzi.cn

B. 流程控制
来源：http://em.shtwfgs.cn

================================================================================
来源：http://zs.shxzskj.cn

[B01] 条件判断 if / else
来源：http://mv.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://im.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bs.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yp.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lq.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ea.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wl.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dr.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mu.9csxet.cn

[B02] 多分支 else if / elif
来源：http://pi.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cs.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://za.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pb.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wf.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jo.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.newstarts.cn

[B03] switch / match / case
来源：http://ht.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ot.nicolike.cn


<!-- 参考信息 -->