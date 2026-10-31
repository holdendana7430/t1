代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mm.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ei.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ks.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hf.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hi.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sq.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gm.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jg.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ne.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ym.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yk.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bu.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bj.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qy.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kv.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ud.lnxyls.cn

================================================================================
来源：http://zs.shxzukj.cn

A. 基础语法与类型
来源：http://dq.muxihuayi.cn

================================================================================
来源：http://jn.lnxyls.cn

[A01] Hello World
来源：http://me.hahajie.cn

Py:   print("Hello, World!")
来源：http://bo.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://dq.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://ro.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://za.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://kd.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ie.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://qu.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://se.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://la.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fw.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://db.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ex.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ia.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ev.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://yk.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://zf.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://do.huixinmuqiang.cn

[A03] 常量定义
来源：http://wq.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://of.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://on.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://mn.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://tl.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://li.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://uq.newstarts.cn

Ruby: PI = 3.14159
来源：http://st.asd995.cn

C#:   const double PI = 3.14159;
来源：http://wr.newstarts.cn

[A04] 判断变量类型
来源：http://os.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xe.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yf.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jk.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ki.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://av.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sd.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xh.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://cx.hnjuh.cn

[A05] 整数除法与取模
来源：http://gf.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://db.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://co.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gc.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ed.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://qu.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://wq.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://td.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://se.bjjhwx.cn

[A06] 字符串转数字
来源：http://bl.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://zy.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jj.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bq.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mx.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vd.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://du.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://if.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cy.colortex.cn

[A07] 数字转字符串
来源：http://wg.yuexingan06.cn

Py:   str(42)
来源：http://cl.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://av.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://li.bjjhwx.cn

TS:   String(42)
来源：http://ja.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yf.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://um.asd995.cn

Ruby: 42.to_s
来源：http://jp.shxzskj.cn

C#:   42.ToString()
来源：http://po.asd995.cn

[A08] 取整与四舍五入
来源：http://jz.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pj.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://te.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qg.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hc.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://li.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lb.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ch.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tn.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://ng.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ha.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zm.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gt.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kq.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jv.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xa.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dc.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dz.9csxet.cn

[A10] 生成随机数
来源：http://th.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://be.9csxet.cn

PHP:  random_int(1, 100);
来源：http://qt.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xm.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zn.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://dw.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tw.szsharing.cn

Ruby: rand(1..100)
来源：http://uf.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://rg.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://so.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://un.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xw.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vh.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://aj.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://vp.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kt.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ko.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bv.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://kc.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fn.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jo.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://if.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://iw.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://gp.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gg.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://ry.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://eg.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yn.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://by.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://qy.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://rk.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://ns.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://kl.521024.cn

Go:   "第一行\n第二行"
来源：http://zo.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://rd.huanxung.cn

C#:   "第一行\n第二行"
来源：http://dg.jianghongdianzi.cn

[A14] 注释写法
来源：http://rr.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yb.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hj.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://ft.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://qq.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cd.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://yo.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cm.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://tb.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://pg.shxzskj.cn

Py:   value = data or "默认值"
来源：http://nl.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://sd.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://pn.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://bu.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ru.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://md.9csxet.cn

Ruby: value = data || "默认值"
来源：http://nf.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://dl.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://hq.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oh.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qj.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nb.bjjhwx.cn

TS:   if (!x) {}
来源：http://kb.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ul.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://el.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tr.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://si.chemitech.net.cn

[A17] 位运算
来源：http://mq.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zw.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wa.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xi.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pc.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hp.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oq.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ex.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://zu.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://nc.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://pt.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rl.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yv.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://da.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ti.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://sx.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://xm.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://hi.bjjhwx.cn

Py:   a, b = b, a
来源：http://dg.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dh.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://ha.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://dh.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://no.huanxung.cn

Go:   a, b = b, a
来源：http://vl.colortex.cn

Ruby: a, b = b, a
来源：http://bb.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://zq.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://nw.lnxyls.cn

Py:   name = input("请输入：")
来源：http://ki.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rc.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sc.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://nc.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://sv.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://we.bookmarksfly.cn

Ruby: gets.chomp
来源：http://sl.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ie.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://di.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://ch.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lx.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://lu.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://vr.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://iy.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yk.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://mi.521024.cn

C#:   3.14159.ToString("F2")
来源：http://vi.shtwfgs.cn

[A22] 获取字符串长度
来源：http://fy.colortex.cn

Py:   len(s)
来源：http://os.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yn.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dg.hahajie.cn

TS:   s.length
来源：http://kp.jctech888.com.cn

Java: s.length()
来源：http://pr.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lm.panjiajie.cn

Ruby: s.length
来源：http://wg.szsharing.cn

C#:   s.Length
来源：http://pl.panjiajie.cn

[A23] 大小写转换
来源：http://bg.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rz.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jv.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ig.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fi.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yv.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eh.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fs.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cm.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://nu.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cw.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uo.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lx.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uz.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vs.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://en.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vd.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xc.huixiangedu.cn

[A25] 字符串比较
来源：http://da.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://eg.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gr.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jf.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cs.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ju.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ao.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tk.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yl.huanxung.cn

[A26] 类型转换总览
来源：http://qt.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ce.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sh.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xj.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://to.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://po.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://of.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dk.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jl.szxytkj.cn

================================================================================
来源：http://pi.wgjwhj.cn

B. 流程控制
来源：http://lg.bjjhwx.cn

================================================================================
来源：http://yc.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://vy.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rt.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ju.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://em.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ex.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kk.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ey.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://me.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ja.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ex.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kw.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ng.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tb.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sp.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hm.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rc.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://za.shtwfgs.cn

[B03] switch / match / case
来源：http://kt.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://re.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rq.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lj.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zd.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dm.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bp.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vv.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://om.jctech888.com.cn

[B04] for 计数循环
来源：http://qu.521024.cn

Py:   for i in range(10): print(i)
来源：http://qx.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gw.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xq.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sz.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://xu.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://px.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://wx.nicolike.cn

Py:   for item in arr: print(item)
来源：http://et.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tp.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xr.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yr.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pv.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ev.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://zk.chemitech.net.cn


<!-- 参考信息 -->