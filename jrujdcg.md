代发 wailian999

================================================================================
来源：http://fc.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://ek.9csxet.cn

Common Programming Examples Cheat Book
来源：http://th.wgjwhj.cn

================================================================================
来源：http://mx.yuntaijiaju.cn

【收录内容】
来源：http://as.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xg.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rz.bjjhwx.cn

SQL · Bash · C · C++
来源：http://mw.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mo.yuexingan06.cn

【使用说明】
来源：http://ty.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ev.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uh.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vo.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tz.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yq.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zg.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fj.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wi.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fz.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hh.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eg.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bh.muxihuayi.cn

【文件统计】
来源：http://cp.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rm.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://fe.huanxung.cn

目  录
来源：http://fb.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://np.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gb.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mg.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kk.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pq.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bb.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ku.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zc.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ha.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oc.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://am.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://be.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fk.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jq.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pd.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lr.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oa.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mz.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xu.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hc.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vs.jctech888.com.cn

================================================================================
来源：http://mp.huanxung.cn

A. 基础语法与类型
来源：http://cl.panjiajie.cn

================================================================================
来源：http://ez.muxihuayi.cn

[A01] Hello World
来源：http://ym.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://ta.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://oc.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://li.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eu.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://zt.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://bp.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://iu.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xu.newstarts.cn

[A02] 变量声明与赋值
来源：http://yx.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qy.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zd.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vi.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kd.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://sd.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://up.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://gq.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ko.521024.cn

[A03] 常量定义
来源：http://wv.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://th.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://gx.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ts.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://zr.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://hb.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://lh.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://up.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://gy.gzmigu.cn

[A04] 判断变量类型
来源：http://ev.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lt.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qp.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lk.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://gq.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hk.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tm.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ft.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://bu.nszjky.cn

[A05] 整数除法与取模
来源：http://wd.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ss.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cz.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nr.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tx.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://li.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://ke.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://od.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://rt.colortex.cn

[A06] 字符串转数字
来源：http://qo.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://mq.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cq.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cb.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ep.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kn.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ne.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sv.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jb.huixiangedu.cn

[A07] 数字转字符串
来源：http://qo.nicolike.cn

Py:   str(42)
来源：http://mq.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://ru.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://jp.chemitech.net.cn

TS:   String(42)
来源：http://zl.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ma.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://gl.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://cw.jianghongdianzi.cn

C#:   42.ToString()
来源：http://yj.szsharing.cn

[A08] 取整与四舍五入
来源：http://kl.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uj.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iv.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xj.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cs.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lf.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fw.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://re.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yv.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://iw.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wu.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bu.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sp.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zg.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qn.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qx.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yl.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vk.bjjhwx.cn

[A10] 生成随机数
来源：http://xg.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://qn.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://sh.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xt.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bk.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://bv.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ja.panjiajie.cn

Ruby: rand(1..100)
来源：http://tc.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://sc.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://zu.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://kk.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://il.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tb.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nc.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://uo.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ji.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pr.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ik.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://lo.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sj.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dy.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://kk.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ms.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://lc.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zr.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://tg.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://cf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vg.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://of.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://qp.521024.cn

JS:   "第一行\n第二行"
来源：http://wc.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://hg.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://lk.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://rt.colortex.cn

Ruby: "第一行\n第二行"
来源：http://gw.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://nl.newstarts.cn

[A14] 注释写法
来源：http://vp.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://or.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mo.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://el.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://wv.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ix.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://ul.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eo.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://wb.nszjky.cn

[A15] 空值判断与默认值
来源：http://yv.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ce.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://ai.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://xl.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://ei.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kw.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://gi.huanxung.cn

Ruby: value = data || "默认值"
来源：http://fb.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://sh.colortex.cn

[A16] 真假值判断规则
来源：http://xy.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ez.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hw.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dt.huixiangedu.cn

TS:   if (!x) {}
来源：http://cq.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oj.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jh.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jd.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ys.9csxet.cn

[A17] 位运算
来源：http://zz.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ye.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lp.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uc.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ql.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sd.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nx.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://tn.colortex.cn

Py:   ord("A"); chr(65)
来源：http://fd.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://pz.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wj.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eg.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://iu.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xe.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://uz.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://nm.hnjuh.cn

[A19] 交换两个变量
来源：http://xx.wgjwhj.cn

Py:   a, b = b, a
来源：http://lk.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sn.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://hc.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://js.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://lf.gzmigu.cn

Go:   a, b = b, a
来源：http://js.jctech888.com.cn

Ruby: a, b = b, a
来源：http://dh.521024.cn

C#:   (a, b) = (b, a);
来源：http://xz.yuexingan06.cn

[A20] 读取标准输入
来源：http://ap.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://au.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fh.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ac.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://uv.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://an.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qb.jctech888.com.cn

Ruby: gets.chomp
来源：http://fa.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://yw.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://rt.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://pg.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ji.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://xm.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://tw.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://zl.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qc.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://zp.521024.cn

C#:   3.14159.ToString("F2")
来源：http://tw.lnxyls.cn

[A22] 获取字符串长度
来源：http://uh.lnxyls.cn

Py:   len(s)
来源：http://gd.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sr.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jq.huixiangedu.cn

TS:   s.length
来源：http://uc.hahajie.cn

Java: s.length()
来源：http://es.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bn.szxytkj.cn

Ruby: s.length
来源：http://sv.chemitech.net.cn

C#:   s.Length
来源：http://uj.521024.cn

[A23] 大小写转换
来源：http://jy.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jq.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eq.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gu.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nb.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sf.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qb.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ts.muxihuayi.cn

[A24] 去除首尾空白
来源：http://ce.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tg.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dl.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zu.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ry.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ev.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://bt.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tr.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ip.huanxung.cn

[A25] 字符串比较
来源：http://uq.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://ee.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wc.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rl.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oc.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vq.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cj.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ua.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oy.shtwfgs.cn

[A26] 类型转换总览
来源：http://gn.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ko.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fk.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://de.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://up.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ww.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wd.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gg.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wa.yuexingan06.cn

================================================================================
来源：http://dn.yuntaijiaju.cn

B. 流程控制
来源：http://eh.jctech888.com.cn

================================================================================
来源：http://jo.szxytkj.cn

[B01] 条件判断 if / else
来源：http://zc.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bc.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ho.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bx.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zi.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lu.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://in.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aj.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jl.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://uw.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sl.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nz.lnxyls.cn


<!-- 参考信息 -->