代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wn.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ot.chemitech.net.cn

【文件统计】
来源：http://aw.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ix.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ar.lnxyls.cn

目  录
来源：http://sm.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://da.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qp.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cl.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zn.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xx.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://no.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xj.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vk.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ql.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gf.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://de.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yj.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tg.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ct.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vl.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yc.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ke.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ox.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rw.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pc.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lk.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tu.jianghongdianzi.cn

================================================================================
来源：http://fk.newstarts.cn

A. 基础语法与类型
来源：http://ah.shtwfgs.cn

================================================================================
来源：http://kj.yuexingan06.cn

[A01] Hello World
来源：http://xs.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://is.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://wk.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://dk.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qm.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://zg.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://tm.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://bs.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ka.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://bl.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fr.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zj.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://au.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zu.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://en.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://kp.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://tq.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xn.huixiangedu.cn

[A03] 常量定义
来源：http://py.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fs.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://la.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://ll.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://ov.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://se.nicolike.cn

Go:   const PI = 3.14159
来源：http://wp.newstarts.cn

Ruby: PI = 3.14159
来源：http://gi.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://ab.bookmarksfly.cn

[A04] 判断变量类型
来源：http://mh.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gz.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jq.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ba.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://rr.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ay.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ya.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kw.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://gh.9csxet.cn

[A05] 整数除法与取模
来源：http://wv.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zr.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ya.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://od.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cl.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://wk.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://qn.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://kl.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://kw.szxytkj.cn

[A06] 字符串转数字
来源：http://ai.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://lj.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nj.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cp.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qk.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cj.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fb.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gq.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cp.hahajie.cn

[A07] 数字转字符串
来源：http://yq.szsharing.cn

Py:   str(42)
来源：http://nw.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://rr.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://eu.wgjwhj.cn

TS:   String(42)
来源：http://ld.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ys.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://ty.szsharing.cn

Ruby: 42.to_s
来源：http://dh.lnxyls.cn

C#:   42.ToString()
来源：http://nb.9csxet.cn

[A08] 取整与四舍五入
来源：http://qe.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cp.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rj.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dv.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hy.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ei.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://my.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ex.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fn.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://dl.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uf.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lc.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mr.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vy.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zw.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wy.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bp.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yn.haigaiapp.cn

[A10] 生成随机数
来源：http://rb.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://vu.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://zi.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qy.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sh.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://mo.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ey.lnxyls.cn

Ruby: rand(1..100)
来源：http://bb.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://dy.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://uh.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://iw.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bw.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hk.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yx.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://eb.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gc.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://as.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ev.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://ei.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aw.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bo.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://xs.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://rj.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://gl.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bd.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://xy.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://fv.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uc.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://ae.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://vu.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://cm.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://dj.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://ob.521024.cn

Go:   "第一行\n第二行"
来源：http://cm.asd995.cn

Ruby: "第一行\n第二行"
来源：http://vr.newstarts.cn

C#:   "第一行\n第二行"
来源：http://lz.asd995.cn

[A14] 注释写法
来源：http://kn.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ae.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lg.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://mx.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://vn.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qv.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://ag.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sc.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://iy.newstarts.cn

[A15] 空值判断与默认值
来源：http://ez.nszjky.cn

Py:   value = data or "默认值"
来源：http://mx.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://kt.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://od.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://en.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yo.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://gn.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://qo.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://jq.asd995.cn

[A16] 真假值判断规则
来源：http://kj.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mv.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rx.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tt.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://jz.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gw.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://js.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://al.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sb.nicolike.cn

[A17] 位运算
来源：http://zb.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gx.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bn.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xv.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hm.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://bn.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://mk.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://kw.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sh.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oo.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://gc.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tj.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://yp.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://se.shtwfgs.cn

[A19] 交换两个变量
来源：http://dt.chemitech.net.cn

Py:   a, b = b, a
来源：http://dq.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hj.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://kh.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://da.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://pz.nicolike.cn

Go:   a, b = b, a
来源：http://vb.nszjky.cn

Ruby: a, b = b, a
来源：http://zt.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://wg.bookmarksfly.cn

[A20] 读取标准输入
来源：http://se.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://nr.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kh.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ou.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://qy.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://cv.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hb.muxihuayi.cn

Ruby: gets.chomp
来源：http://lg.9csxet.cn

C#:   Console.ReadLine();
来源：http://up.hahajie.cn

[A21] 保留指定小数位输出
来源：http://xd.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://mj.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://he.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://qo.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://ti.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://ow.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gg.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://aa.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://mg.lnxyls.cn

[A22] 获取字符串长度
来源：http://em.huanxung.cn

Py:   len(s)
来源：http://cw.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hh.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tq.9csxet.cn

TS:   s.length
来源：http://he.asd995.cn

Java: s.length()
来源：http://oj.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uj.szxytkj.cn

Ruby: s.length
来源：http://hy.shxzskj.cn

C#:   s.Length
来源：http://mr.gzmigu.cn

[A23] 大小写转换
来源：http://qw.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xk.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ms.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vf.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xi.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tw.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ld.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://re.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ay.hahajie.cn

[A24] 去除首尾空白
来源：http://ds.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vy.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mr.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vx.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bs.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://yt.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://by.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bb.gzmigu.cn

[A25] 字符串比较
来源：http://vq.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://xj.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ok.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uu.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ke.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vr.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uf.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nn.9csxet.cn

[A26] 类型转换总览
来源：http://lc.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kp.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://we.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mn.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ov.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vh.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://to.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zd.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sg.shtwfgs.cn

================================================================================
来源：http://se.bjjhwx.cn

B. 流程控制
来源：http://aa.panjiajie.cn

================================================================================
来源：http://zz.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://io.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vp.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yu.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://op.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://np.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://od.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fu.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bc.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iq.huanxung.cn

[B02] 多分支 else if / elif
来源：http://mx.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fz.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://no.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sx.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xy.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dw.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kv.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.hahajie.cn

[B03] switch / match / case
来源：http://xi.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yl.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gl.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pv.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rx.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qn.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wv.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ul.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rh.colortex.cn

[B04] for 计数循环
来源：http://je.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://na.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qe.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ll.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fs.jctech888.com.cn


<!-- 参考信息 -->