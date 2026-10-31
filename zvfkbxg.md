代发 wailian999

================================================================================
来源：http://gl.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://pb.szsharing.cn

Common Programming Examples Cheat Book
来源：http://ur.chemitech.net.cn

================================================================================
来源：http://bg.chemitech.net.cn

【收录内容】
来源：http://fv.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uw.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tt.gzmigu.cn

SQL · Bash · C · C++
来源：http://me.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://si.colortex.cn

【使用说明】
来源：http://je.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sb.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mx.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ds.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cu.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ev.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jj.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yb.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ex.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fy.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xv.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kj.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://da.yuntaijiaju.cn

【文件统计】
来源：http://ye.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ga.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ke.nszjky.cn

目  录
来源：http://do.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://wj.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sf.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qj.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ns.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vb.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zx.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jh.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://td.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ch.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ad.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ch.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mn.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cp.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oy.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ha.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ns.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ne.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sp.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yu.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dt.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dw.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kl.shxzskj.cn

================================================================================
来源：http://zb.shtwfgs.cn

A. 基础语法与类型
来源：http://ua.hahajie.cn

================================================================================
来源：http://pg.colortex.cn

[A01] Hello World
来源：http://tp.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ue.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://vj.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://qn.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://qc.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://uf.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://xs.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ls.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://ek.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ct.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://is.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qt.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nn.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://eu.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://ot.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://yl.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pd.asd995.cn

[A03] 常量定义
来源：http://fq.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uc.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://kv.huanxung.cn

JS:   const PI = 3.14159;
来源：http://kg.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://td.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://vz.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://jb.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://vx.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://dn.lnxyls.cn

[A04] 判断变量类型
来源：http://tt.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wa.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rx.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wd.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://pg.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pf.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mr.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dx.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://ry.shxzukj.cn

[A05] 整数除法与取模
来源：http://qa.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ev.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ph.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vo.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bd.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://vm.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://ea.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://nc.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://dn.newstarts.cn

[A06] 字符串转数字
来源：http://qj.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://mw.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rp.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gb.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sj.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oa.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fg.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jf.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xs.shxzukj.cn

[A07] 数字转字符串
来源：http://zz.shtwfgs.cn

Py:   str(42)
来源：http://jo.521024.cn

PHP:  (string) 42; strval(42)
来源：http://ss.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://ao.hnjuh.cn

TS:   String(42)
来源：http://ze.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qn.asd995.cn

Go:   strconv.Itoa(42)
来源：http://fn.yuexingan06.cn

Ruby: 42.to_s
来源：http://fq.haigaiapp.cn

C#:   42.ToString()
来源：http://fo.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://ue.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gd.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ix.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://af.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vb.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zg.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kq.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ww.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vo.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://zh.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wq.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hu.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://go.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mb.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hh.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dv.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lv.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://if.shxzukj.cn

[A10] 生成随机数
来源：http://vv.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://yg.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://tu.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ck.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ed.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://sp.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bz.panjiajie.cn

Ruby: rand(1..100)
来源：http://wh.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://sz.huanxung.cn

[A11] 条件表达式（三元）
来源：http://dj.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://uh.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://th.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bi.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://re.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://jp.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jr.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iy.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ak.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://dg.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bg.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hw.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://gi.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://jq.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://yw.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ua.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://zw.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://tl.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://of.szsharing.cn

Py:   "第一行\n第二行"
来源：http://yu.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://dr.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://rz.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://bt.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://hh.colortex.cn

Go:   "第一行\n第二行"
来源：http://qu.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://tb.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://lr.jianghongdianzi.cn

[A14] 注释写法
来源：http://io.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://by.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://br.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://qe.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://cb.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qq.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://jr.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ol.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://hl.newstarts.cn

[A15] 空值判断与默认值
来源：http://vl.shxzskj.cn

Py:   value = data or "默认值"
来源：http://dx.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://fo.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://or.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://av.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ax.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://qw.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ae.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://tl.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ei.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hr.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eb.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://un.huanxung.cn

TS:   if (!x) {}
来源：http://hc.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pk.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://je.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ss.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zz.muxihuayi.cn

[A17] 位运算
来源：http://xr.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://op.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cw.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mk.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cf.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rt.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://oi.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://dm.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://vz.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nu.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mf.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://xv.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sk.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://ez.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://vh.muxihuayi.cn

[A19] 交换两个变量
来源：http://ua.hnjuh.cn

Py:   a, b = b, a
来源：http://gc.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://et.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://rz.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://il.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://cp.huixiangedu.cn

Go:   a, b = b, a
来源：http://za.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://ab.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://xl.hahajie.cn

[A20] 读取标准输入
来源：http://vv.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://yb.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://as.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yi.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://cy.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://nx.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ol.bookmarksfly.cn

Ruby: gets.chomp
来源：http://md.colortex.cn

C#:   Console.ReadLine();
来源：http://oq.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://dw.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://ux.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pu.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://bp.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://xs.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://nx.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xl.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://ng.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://eh.jctech888.com.cn

[A22] 获取字符串长度
来源：http://oy.chemitech.net.cn

Py:   len(s)
来源：http://fd.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pd.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://si.gzmigu.cn

TS:   s.length
来源：http://cl.huanxung.cn

Java: s.length()
来源：http://vf.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vz.shxzskj.cn

Ruby: s.length
来源：http://dh.yuexingan06.cn

C#:   s.Length
来源：http://rw.521024.cn

[A23] 大小写转换
来源：http://aj.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zn.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tj.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iy.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rb.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jj.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dq.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://td.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kb.yuexingan06.cn

[A24] 去除首尾空白
来源：http://kn.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ty.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ud.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ts.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cu.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ba.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://cc.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sh.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://js.chemitech.net.cn

[A25] 字符串比较
来源：http://pq.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://ws.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oc.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bc.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qv.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dy.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nf.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://le.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ta.asd995.cn

[A26] 类型转换总览
来源：http://fq.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lg.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hs.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mf.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://hx.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kx.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yw.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bk.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ls.asd995.cn

================================================================================
来源：http://gw.nszjky.cn

B. 流程控制
来源：http://ud.521024.cn

================================================================================
来源：http://zj.asd995.cn

[B01] 条件判断 if / else
来源：http://yv.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nd.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cg.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wm.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jt.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ce.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ig.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vg.huanxung.cn

[B02] 多分支 else if / elif
来源：http://rw.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eb.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://od.szxytkj.cn


<!-- 参考信息 -->