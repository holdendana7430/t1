代发 wailian999

--------------------------------------------------------------------------------
来源：http://zb.bookmarksfly.cn

目  录
来源：http://bb.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ed.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://um.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bs.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://za.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ch.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://es.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lw.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gx.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pe.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xg.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ix.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://je.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jt.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pz.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wi.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jg.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sv.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cv.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://if.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rz.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://me.shtwfgs.cn

================================================================================
来源：http://or.jianghongdianzi.cn

A. 基础语法与类型
来源：http://ss.bookmarksfly.cn

================================================================================
来源：http://xf.huixinmuqiang.cn

[A01] Hello World
来源：http://op.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://pn.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://jy.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ff.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qm.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://vt.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://vv.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://px.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rh.szxytkj.cn

[A02] 变量声明与赋值
来源：http://ix.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ld.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ie.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fs.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dx.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://gm.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://eu.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://yl.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kt.bookmarksfly.cn

[A03] 常量定义
来源：http://ak.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qg.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://um.newstarts.cn

JS:   const PI = 3.14159;
来源：http://vr.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://ca.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://dj.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://gc.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://da.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://vz.asd995.cn

[A04] 判断变量类型
来源：http://lk.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ek.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bf.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://em.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://df.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bp.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yl.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sq.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://oy.colortex.cn

[A05] 整数除法与取模
来源：http://ok.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sd.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://di.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vq.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xv.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://fm.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://ix.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://eq.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://mq.panjiajie.cn

[A06] 字符串转数字
来源：http://ps.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ws.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ap.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ei.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cl.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wa.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zo.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ct.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://if.haigaiapp.cn

[A07] 数字转字符串
来源：http://rm.szxytkj.cn

Py:   str(42)
来源：http://vp.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://qm.hahajie.cn

JS:   String(42); (42).toString()
来源：http://rb.huanxung.cn

TS:   String(42)
来源：http://hd.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zh.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://wo.bjjhwx.cn

Ruby: 42.to_s
来源：http://ru.huixiangedu.cn

C#:   42.ToString()
来源：http://ci.newstarts.cn

[A08] 取整与四舍五入
来源：http://zp.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vs.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dv.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dw.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kf.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://le.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jx.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mb.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zn.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://fb.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rt.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nb.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cq.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sh.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cf.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bh.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iw.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iw.jctech888.com.cn

[A10] 生成随机数
来源：http://ff.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://yw.521024.cn

PHP:  random_int(1, 100);
来源：http://fz.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ti.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jf.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://qr.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bc.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://nd.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://yv.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://ae.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://ig.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bm.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jr.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ys.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ue.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pj.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://er.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://le.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://tm.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nm.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ya.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://fj.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://rn.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://sx.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yh.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://im.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://dk.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hc.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://aa.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://lf.hahajie.cn

JS:   "第一行\n第二行"
来源：http://di.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://dz.szxytkj.cn

Java: "第一行\n第二行"
来源：http://tr.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://xn.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://st.nszjky.cn

C#:   "第一行\n第二行"
来源：http://wm.hahajie.cn

[A14] 注释写法
来源：http://ti.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sv.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rk.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://bo.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://qj.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eo.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://cv.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ut.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://eu.hahajie.cn

[A15] 空值判断与默认值
来源：http://sr.521024.cn

Py:   value = data or "默认值"
来源：http://ax.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://mk.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://ec.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://my.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xr.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fa.colortex.cn

Ruby: value = data || "默认值"
来源：http://nz.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://md.chemitech.net.cn

[A16] 真假值判断规则
来源：http://tb.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nw.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pm.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nh.yuexingan06.cn

TS:   if (!x) {}
来源：http://fr.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uy.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xb.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ws.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xe.bookmarksfly.cn

[A17] 位运算
来源：http://iy.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hl.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mp.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hi.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bb.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jz.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wu.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://za.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://pw.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://mh.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ab.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xf.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://lm.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tm.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ym.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://bi.chemitech.net.cn

[A19] 交换两个变量
来源：http://pb.shxzskj.cn

Py:   a, b = b, a
来源：http://ow.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ll.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://yz.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://pw.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://rh.nicolike.cn

Go:   a, b = b, a
来源：http://ip.9csxet.cn

Ruby: a, b = b, a
来源：http://ri.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://zi.huanxung.cn

[A20] 读取标准输入
来源：http://uj.shxzskj.cn

Py:   name = input("请输入：")
来源：http://qf.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kr.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rl.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://hd.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ki.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yn.hnjuh.cn

Ruby: gets.chomp
来源：http://pn.szxytkj.cn

C#:   Console.ReadLine();
来源：http://su.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://xj.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://oq.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lh.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ct.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://nv.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://pf.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qe.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ka.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://ro.9csxet.cn

[A22] 获取字符串长度
来源：http://mi.huixinmuqiang.cn

Py:   len(s)
来源：http://dj.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hj.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jt.jctech888.com.cn

TS:   s.length
来源：http://zz.chemitech.net.cn

Java: s.length()
来源：http://ij.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://um.huanxung.cn

Ruby: s.length
来源：http://ju.lnxyls.cn

C#:   s.Length
来源：http://jj.bookmarksfly.cn

[A23] 大小写转换
来源：http://zt.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wj.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dn.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zi.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mw.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ih.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eo.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vz.bjjhwx.cn

[A24] 去除首尾空白
来源：http://mg.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pw.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hl.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zd.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cc.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ac.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://na.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ph.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oi.jianghongdianzi.cn

[A25] 字符串比较
来源：http://iu.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://sn.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jl.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pk.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vw.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ah.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vx.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dw.huanxung.cn

[A26] 类型转换总览
来源：http://fy.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ju.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ym.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sn.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://fm.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ba.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cj.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qn.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ik.bjjhwx.cn

================================================================================
来源：http://rf.shxzukj.cn

B. 流程控制
来源：http://zs.hahajie.cn

================================================================================
来源：http://yb.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://rw.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nn.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rw.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ld.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sq.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jf.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vk.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sw.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bm.newstarts.cn

[B02] 多分支 else if / elif
来源：http://vg.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yy.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ev.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jl.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hv.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gi.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gl.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.shtwfgs.cn

[B03] switch / match / case
来源：http://ts.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pb.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kn.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zy.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kv.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vf.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ce.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bd.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ma.chemitech.net.cn

[B04] for 计数循环
来源：http://sp.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://wy.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iq.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ll.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://km.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ty.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://es.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://zu.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dr.huanxung.cn


<!-- 参考信息 -->