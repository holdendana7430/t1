代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://by.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pt.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yc.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ws.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pn.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hg.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yg.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ux.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dk.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vw.shtwfgs.cn

【文件统计】
来源：http://jn.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pl.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://sp.shxzukj.cn

目  录
来源：http://xy.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ro.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ef.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sf.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jj.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jo.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yk.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ya.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lc.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cr.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zl.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dt.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://en.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jx.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dc.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kc.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ga.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cu.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://so.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ix.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ee.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ap.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pa.yuexingan06.cn

================================================================================
来源：http://ce.muxihuayi.cn

A. 基础语法与类型
来源：http://lv.nicolike.cn

================================================================================
来源：http://if.shxzskj.cn

[A01] Hello World
来源：http://st.panjiajie.cn

Py:   print("Hello, World!")
来源：http://qp.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://xk.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://zu.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bk.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://qg.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://me.521024.cn

Ruby: puts "Hello, World!"
来源：http://tu.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gl.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://xm.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jp.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://al.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://af.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cq.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://jl.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ig.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://qp.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sb.asd995.cn

[A03] 常量定义
来源：http://hr.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uz.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://gr.9csxet.cn

JS:   const PI = 3.14159;
来源：http://mb.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://bn.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ye.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://ol.hnjuh.cn

Ruby: PI = 3.14159
来源：http://df.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://lk.9csxet.cn

[A04] 判断变量类型
来源：http://iw.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dw.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zi.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iq.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://jj.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://np.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nx.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iz.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://re.szxytkj.cn

[A05] 整数除法与取模
来源：http://sb.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ps.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jt.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ih.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wl.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://lf.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://xx.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://fj.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://kp.gzmigu.cn

[A06] 字符串转数字
来源：http://mr.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://wx.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hw.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fn.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vp.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yd.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://si.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vg.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ha.szsharing.cn

[A07] 数字转字符串
来源：http://qk.shxzukj.cn

Py:   str(42)
来源：http://ph.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://hx.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://yk.panjiajie.cn

TS:   String(42)
来源：http://kp.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uq.colortex.cn

Go:   strconv.Itoa(42)
来源：http://it.colortex.cn

Ruby: 42.to_s
来源：http://qk.muxihuayi.cn

C#:   42.ToString()
来源：http://fw.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://vr.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gg.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fc.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ed.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ln.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cd.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tg.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lm.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gl.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://un.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bk.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pw.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dd.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jk.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zm.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cy.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dn.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wa.yuntaijiaju.cn

[A10] 生成随机数
来源：http://rd.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://qw.521024.cn

PHP:  random_int(1, 100);
来源：http://qn.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yx.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fa.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://la.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ye.nicolike.cn

Ruby: rand(1..100)
来源：http://vk.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://va.521024.cn

[A11] 条件表达式（三元）
来源：http://um.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://qy.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qb.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gl.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pv.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ud.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rw.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dv.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://il.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://ik.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ih.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://on.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://bm.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://kr.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://sh.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kx.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://bq.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://jy.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pm.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://hu.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://kb.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://yg.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://wj.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://bo.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://wk.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://qb.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://ks.shxzukj.cn

[A14] 注释写法
来源：http://db.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sk.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gh.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ib.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://ne.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qp.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://gq.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://aa.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://oj.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://oa.hahajie.cn

Py:   value = data or "默认值"
来源：http://fm.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ak.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://og.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://ey.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xm.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://yy.nicolike.cn

Ruby: value = data || "默认值"
来源：http://tl.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://mz.bjjhwx.cn

[A16] 真假值判断规则
来源：http://bb.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dn.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xo.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bo.szsharing.cn

TS:   if (!x) {}
来源：http://ea.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ru.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qf.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pf.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kl.shxzskj.cn

[A17] 位运算
来源：http://no.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://so.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oi.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://or.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vk.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ri.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://op.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://pd.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://yj.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kx.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fu.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://ew.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rg.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://ks.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://je.asd995.cn

[A19] 交换两个变量
来源：http://rh.newstarts.cn

Py:   a, b = b, a
来源：http://su.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nb.521024.cn

JS:   [a, b] = [b, a];
来源：http://rf.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://ie.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://uj.yuexingan06.cn

Go:   a, b = b, a
来源：http://pe.panjiajie.cn

Ruby: a, b = b, a
来源：http://pd.colortex.cn

C#:   (a, b) = (b, a);
来源：http://az.shxzskj.cn

[A20] 读取标准输入
来源：http://vt.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://kg.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tm.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ge.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://ht.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://el.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sy.chemitech.net.cn

Ruby: gets.chomp
来源：http://nb.hahajie.cn

C#:   Console.ReadLine();
来源：http://st.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://jk.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://ak.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ab.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://gr.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://je.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://xd.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ir.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://vg.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://zr.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://cx.shxzskj.cn

Py:   len(s)
来源：http://io.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://av.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ux.hahajie.cn

TS:   s.length
来源：http://kc.lnxyls.cn

Java: s.length()
来源：http://pe.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zf.wgjwhj.cn

Ruby: s.length
来源：http://ni.lnxyls.cn

C#:   s.Length
来源：http://sr.haigaiapp.cn

[A23] 大小写转换
来源：http://wc.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fu.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ct.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aj.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mg.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gf.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fc.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nc.shtwfgs.cn

[A24] 去除首尾空白
来源：http://yl.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xa.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nj.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pw.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ne.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wt.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://zm.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kz.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cq.gzmigu.cn

[A25] 字符串比较
来源：http://ys.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ng.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gm.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ch.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mb.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bw.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fk.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dl.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gw.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://pt.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jt.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hg.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xp.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://yt.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://if.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cl.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qv.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cy.chemitech.net.cn

================================================================================
来源：http://le.shxzskj.cn

B. 流程控制
来源：http://pl.yuexingan06.cn

================================================================================
来源：http://rm.szsharing.cn

[B01] 条件判断 if / else
来源：http://rk.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xe.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nd.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qy.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wt.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ed.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yr.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ma.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ul.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://vm.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ha.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vh.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gk.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nr.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jw.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fh.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.newstarts.cn

[B03] switch / match / case
来源：http://aq.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pv.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ez.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gw.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vl.bjjhwx.cn


<!-- 参考信息 -->