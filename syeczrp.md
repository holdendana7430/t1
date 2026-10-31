代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ug.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ek.muxihuayi.cn

【文件统计】
来源：http://nu.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mi.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://xx.wgjwhj.cn

目  录
来源：http://nz.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://pe.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ml.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ue.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qv.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oh.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zx.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gp.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vp.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vg.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zz.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qr.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ce.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bz.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ib.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://me.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://as.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ut.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rv.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fe.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mt.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fv.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ad.9csxet.cn

================================================================================
来源：http://xz.muxihuayi.cn

A. 基础语法与类型
来源：http://iq.asd995.cn

================================================================================
来源：http://wh.lnxyls.cn

[A01] Hello World
来源：http://xr.panjiajie.cn

Py:   print("Hello, World!")
来源：http://to.colortex.cn

PHP:  echo "Hello, World!";
来源：http://es.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://on.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nr.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://fa.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://xe.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://wk.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dz.shxzskj.cn

[A02] 变量声明与赋值
来源：http://wd.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xp.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://io.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ln.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://th.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://xg.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://vk.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://yn.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mu.yuntaijiaju.cn

[A03] 常量定义
来源：http://ki.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ae.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://si.nicolike.cn

JS:   const PI = 3.14159;
来源：http://bc.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://xc.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://qc.colortex.cn

Go:   const PI = 3.14159
来源：http://tp.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://cl.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://fd.panjiajie.cn

[A04] 判断变量类型
来源：http://zr.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wn.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://er.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iy.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://fr.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zu.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mr.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ne.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://zr.szxytkj.cn

[A05] 整数除法与取模
来源：http://uj.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://um.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ha.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://no.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://de.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://bc.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://oy.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://ks.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://ac.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://aq.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://iu.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://su.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mo.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sc.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cs.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vl.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cb.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://as.nicolike.cn

[A07] 数字转字符串
来源：http://hc.haigaiapp.cn

Py:   str(42)
来源：http://rq.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://is.asd995.cn

JS:   String(42); (42).toString()
来源：http://pj.huixiangedu.cn

TS:   String(42)
来源：http://zx.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bg.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ss.chemitech.net.cn

Ruby: 42.to_s
来源：http://dl.yuntaijiaju.cn

C#:   42.ToString()
来源：http://qc.szsharing.cn

[A08] 取整与四舍五入
来源：http://bq.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tb.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kc.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nt.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zk.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gq.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dr.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ku.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://jc.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rg.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zx.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jq.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lc.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lp.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zz.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eg.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pv.panjiajie.cn

[A10] 生成随机数
来源：http://vx.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://lg.9csxet.cn

PHP:  random_int(1, 100);
来源：http://fn.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fb.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tw.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://kj.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bb.huanxung.cn

Ruby: rand(1..100)
来源：http://ir.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://om.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://gu.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://kp.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dt.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ke.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nn.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://ar.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fk.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kw.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://he.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://sp.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hl.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lw.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://oj.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://db.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://nh.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fm.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://tq.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://us.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ub.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://ip.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://do.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://id.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://mi.nszjky.cn

Java: "第一行\n第二行"
来源：http://vb.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ru.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://ov.szsharing.cn

C#:   "第一行\n第二行"
来源：http://aq.yuntaijiaju.cn

[A14] 注释写法
来源：http://mw.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uk.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jw.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://tg.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://xa.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://he.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://gb.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ni.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://qj.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://rt.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://dv.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://mq.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://jj.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://pp.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oh.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://pd.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://wd.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://cl.shxzukj.cn

[A16] 真假值判断规则
来源：http://gk.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kn.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://us.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ga.wgjwhj.cn

TS:   if (!x) {}
来源：http://jc.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rk.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fr.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nd.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hl.shxzskj.cn

[A17] 位运算
来源：http://ru.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ij.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vp.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kb.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mw.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ns.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://oj.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://as.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://bg.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hy.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jf.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://tp.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fr.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://sb.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://jt.panjiajie.cn

[A19] 交换两个变量
来源：http://ai.nicolike.cn

Py:   a, b = b, a
来源：http://po.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tn.colortex.cn

JS:   [a, b] = [b, a];
来源：http://mo.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://gh.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://cs.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ub.yuexingan06.cn

Ruby: a, b = b, a
来源：http://ed.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://wc.521024.cn

[A20] 读取标准输入
来源：http://of.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://sr.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rq.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://di.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://ka.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://vr.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ps.haigaiapp.cn

Ruby: gets.chomp
来源：http://qn.szsharing.cn

C#:   Console.ReadLine();
来源：http://xi.huanxung.cn

[A21] 保留指定小数位输出
来源：http://sl.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://yp.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fj.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ei.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://sg.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://li.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gd.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://lc.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://ii.nicolike.cn

[A22] 获取字符串长度
来源：http://rf.haigaiapp.cn

Py:   len(s)
来源：http://ep.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eo.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rn.huixiangedu.cn

TS:   s.length
来源：http://xp.521024.cn

Java: s.length()
来源：http://uy.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ng.hahajie.cn

Ruby: s.length
来源：http://ar.wgjwhj.cn

C#:   s.Length
来源：http://nd.shxzukj.cn

[A23] 大小写转换
来源：http://of.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fq.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tw.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cb.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vx.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://md.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wm.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xo.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uw.muxihuayi.cn

[A24] 去除首尾空白
来源：http://rp.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tt.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sm.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qt.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pr.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vx.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://yf.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bm.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jj.hahajie.cn

[A25] 字符串比较
来源：http://me.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://dx.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wa.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lm.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cx.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://px.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ud.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uy.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://et.hnjuh.cn

[A26] 类型转换总览
来源：http://lp.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ao.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://db.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cs.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://vu.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dd.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kd.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xu.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kv.bjjhwx.cn

================================================================================
来源：http://ex.yuexingan06.cn

B. 流程控制
来源：http://ta.asd995.cn

================================================================================
来源：http://ze.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://qj.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ch.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://km.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fs.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nv.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ww.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xi.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mc.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://xx.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fr.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wm.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ws.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ww.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tk.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.jianghongdianzi.cn

[B03] switch / match / case
来源：http://jw.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ii.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kg.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ib.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ki.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wd.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yd.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dy.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ou.szsharing.cn

[B04] for 计数循环
来源：http://nl.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://zj.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uo.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nq.shtwfgs.cn


<!-- 参考信息 -->