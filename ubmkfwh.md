代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hm.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jc.jctech888.com.cn

【文件统计】
来源：http://il.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pc.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://fc.gzmigu.cn

目  录
来源：http://fl.huanxung.cn

--------------------------------------------------------------------------------
来源：http://or.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tq.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lj.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://of.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ho.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zq.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xr.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ml.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mt.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xi.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oz.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vc.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ns.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jo.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qo.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iu.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ma.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hs.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ig.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ne.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://di.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qc.huanxung.cn

================================================================================
来源：http://ih.panjiajie.cn

A. 基础语法与类型
来源：http://hk.shtwfgs.cn

================================================================================
来源：http://li.bookmarksfly.cn

[A01] Hello World
来源：http://gy.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://wf.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://aw.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://sr.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dq.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://ye.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://as.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://bt.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://an.asd995.cn

[A02] 变量声明与赋值
来源：http://px.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://id.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jd.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ir.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://po.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://af.521024.cn

Go:   name := "Alex"; age := 20
来源：http://ee.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://eb.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hl.muxihuayi.cn

[A03] 常量定义
来源：http://ss.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ec.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://yx.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://lx.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://at.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://jq.shxzskj.cn

Go:   const PI = 3.14159
来源：http://ui.asd995.cn

Ruby: PI = 3.14159
来源：http://up.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://rd.bjjhwx.cn

[A04] 判断变量类型
来源：http://ji.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://om.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bt.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bu.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://qh.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gd.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ns.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dh.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://wi.jctech888.com.cn

[A05] 整数除法与取模
来源：http://mf.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sh.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uc.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ej.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dg.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://ml.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://uz.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://ys.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://hn.szsharing.cn

[A06] 字符串转数字
来源：http://qn.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://rv.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zo.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ju.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lm.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ni.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fx.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qe.lnxyls.cn

[A07] 数字转字符串
来源：http://mm.bookmarksfly.cn

Py:   str(42)
来源：http://ue.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://dr.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://ye.huixiangedu.cn

TS:   String(42)
来源：http://ny.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ii.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://mb.huanxung.cn

Ruby: 42.to_s
来源：http://ie.muxihuayi.cn

C#:   42.ToString()
来源：http://fp.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://qk.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nh.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zq.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qf.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nb.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rb.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ds.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lf.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bh.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://gl.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fk.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cc.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yo.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://co.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sx.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ja.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fh.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hw.nicolike.cn

[A10] 生成随机数
来源：http://xk.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ui.szsharing.cn

PHP:  random_int(1, 100);
来源：http://zn.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fk.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pq.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://fe.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ic.nicolike.cn

Ruby: rand(1..100)
来源：http://gv.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ty.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://oh.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://py.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gd.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nh.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tl.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://zl.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gc.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://se.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aq.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://gn.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://di.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xy.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://mu.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://nv.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://yk.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qa.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://kj.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://zs.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cm.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://xx.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://jb.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://oy.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://qd.nszjky.cn

Java: "第一行\n第二行"
来源：http://zh.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://fl.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://de.newstarts.cn

C#:   "第一行\n第二行"
来源：http://in.chemitech.net.cn

[A14] 注释写法
来源：http://ty.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ao.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://he.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://br.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://uz.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ic.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://cq.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xg.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://yo.szsharing.cn

[A15] 空值判断与默认值
来源：http://jn.szsharing.cn

Py:   value = data or "默认值"
来源：http://xl.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://de.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://da.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://fb.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mi.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://fx.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://uq.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://tq.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://rw.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lr.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pk.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nr.9csxet.cn

TS:   if (!x) {}
来源：http://hf.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bz.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ra.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dt.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xb.lnxyls.cn

[A17] 位运算
来源：http://iq.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rb.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fo.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bn.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mt.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://kr.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://mi.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://mf.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ez.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ax.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://uw.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ht.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://ip.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://lt.panjiajie.cn

[A19] 交换两个变量
来源：http://ww.szsharing.cn

Py:   a, b = b, a
来源：http://as.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jh.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://zy.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://sx.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://vw.bjjhwx.cn

Go:   a, b = b, a
来源：http://oq.gzmigu.cn

Ruby: a, b = b, a
来源：http://ad.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://nc.haigaiapp.cn

[A20] 读取标准输入
来源：http://jh.shxzskj.cn

Py:   name = input("请输入：")
来源：http://nj.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xg.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hs.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://qc.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ei.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zi.huanxung.cn

Ruby: gets.chomp
来源：http://pr.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://sp.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://zg.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://cj.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://he.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://lh.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://ra.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://og.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bn.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://dd.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://yk.muxihuayi.cn

[A22] 获取字符串长度
来源：http://dd.jctech888.com.cn

Py:   len(s)
来源：http://mm.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ek.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qf.hnjuh.cn

TS:   s.length
来源：http://qd.yuntaijiaju.cn

Java: s.length()
来源：http://tu.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xl.huixinmuqiang.cn

Ruby: s.length
来源：http://wl.shtwfgs.cn

C#:   s.Length
来源：http://lz.lnxyls.cn

[A23] 大小写转换
来源：http://ca.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hs.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xw.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vl.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ny.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bn.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xx.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cm.chemitech.net.cn

[A24] 去除首尾空白
来源：http://jn.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kx.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ir.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tc.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bz.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mg.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://js.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gs.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iu.panjiajie.cn

[A25] 字符串比较
来源：http://qz.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://vc.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ul.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qq.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vb.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pb.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qy.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nk.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gq.521024.cn

[A26] 类型转换总览
来源：http://po.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ql.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rg.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qh.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://qy.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lm.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jv.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://da.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xi.shxzukj.cn

================================================================================
来源：http://wu.haigaiapp.cn

B. 流程控制
来源：http://ct.hahajie.cn

================================================================================
来源：http://af.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://uy.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ik.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bf.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ow.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ab.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://di.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yy.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tv.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://uw.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cg.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://om.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fg.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wg.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mr.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ud.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.jctech888.com.cn

[B03] switch / match / case
来源：http://ag.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fd.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wv.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://di.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uo.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ux.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wg.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cz.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qy.hnjuh.cn

[B04] for 计数循环
来源：http://bv.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://rv.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sj.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://es.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://un.panjiajie.cn


<!-- 参考信息 -->