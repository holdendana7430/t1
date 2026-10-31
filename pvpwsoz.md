代发 wailian999

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vf.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mk.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wb.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gc.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mq.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ch.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ss.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gc.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ne.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pf.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fg.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ds.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ic.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bb.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yk.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gy.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hw.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mv.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://od.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vg.nszjky.cn

================================================================================
来源：http://xb.huixinmuqiang.cn

A. 基础语法与类型
来源：http://ys.shtwfgs.cn

================================================================================
来源：http://bu.bjjhwx.cn

[A01] Hello World
来源：http://ej.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://yb.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://vh.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://xd.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lz.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://al.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://um.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://eq.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://er.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://ee.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iw.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://as.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mp.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zn.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://bk.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://po.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://vx.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://il.haigaiapp.cn

[A03] 常量定义
来源：http://eo.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xb.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://lg.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://lf.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://dw.colortex.cn

Java: static final double PI = 3.14159;
来源：http://js.panjiajie.cn

Go:   const PI = 3.14159
来源：http://up.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://pe.asd995.cn

C#:   const double PI = 3.14159;
来源：http://en.lnxyls.cn

[A04] 判断变量类型
来源：http://ga.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cz.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ko.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://av.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://fv.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yx.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kw.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://am.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://ms.lnxyls.cn

[A05] 整数除法与取模
来源：http://ns.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ph.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vx.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vd.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jp.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://kf.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://as.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://gl.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://zq.gzmigu.cn

[A06] 字符串转数字
来源：http://uo.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://lo.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uw.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wx.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bo.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://md.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lv.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hr.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rj.bjjhwx.cn

[A07] 数字转字符串
来源：http://yw.shxzukj.cn

Py:   str(42)
来源：http://fy.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://oi.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://fl.jctech888.com.cn

TS:   String(42)
来源：http://sy.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uv.colortex.cn

Go:   strconv.Itoa(42)
来源：http://qo.bjjhwx.cn

Ruby: 42.to_s
来源：http://oz.hahajie.cn

C#:   42.ToString()
来源：http://cf.huanxung.cn

[A08] 取整与四舍五入
来源：http://wt.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xg.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yb.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ow.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nu.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iz.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yg.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hb.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ji.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://fa.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://df.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://se.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ey.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zw.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wj.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lm.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hh.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://di.szsharing.cn

[A10] 生成随机数
来源：http://gs.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://pt.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://ai.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ol.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hs.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://rg.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://st.szsharing.cn

Ruby: rand(1..100)
来源：http://la.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://pl.9csxet.cn

[A11] 条件表达式（三元）
来源：http://fx.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://rh.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yq.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hg.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://if.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://iu.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://na.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jx.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xe.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://aq.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ys.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tv.asd995.cn

JS:   `Hello, ${name}!`
来源：http://ht.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://gl.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ld.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ev.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://wu.asd995.cn

C#:   $"Hello, {name}!"
来源：http://vf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xg.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://fn.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ce.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://xk.asd995.cn

TS:   "第一行\n第二行"
来源：http://sg.hnjuh.cn

Java: "第一行\n第二行"
来源：http://qy.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://ec.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://bm.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://rz.newstarts.cn

[A14] 注释写法
来源：http://oa.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ly.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mo.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ug.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://kw.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://he.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://gj.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ox.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://rm.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://fc.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://lx.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://av.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://nj.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://nl.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ae.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://hq.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://wz.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://lu.jctech888.com.cn

[A16] 真假值判断规则
来源：http://ep.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mt.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sx.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ib.shtwfgs.cn

TS:   if (!x) {}
来源：http://bz.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kg.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ks.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://so.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qh.szxytkj.cn

[A17] 位运算
来源：http://ik.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vv.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wq.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cd.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uq.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qe.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vt.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ih.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://dc.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://aw.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://un.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ci.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://ag.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://go.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://ol.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://ie.jctech888.com.cn

[A19] 交换两个变量
来源：http://va.szxytkj.cn

Py:   a, b = b, a
来源：http://rh.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kk.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://rd.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://ug.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://vz.muxihuayi.cn

Go:   a, b = b, a
来源：http://hh.newstarts.cn

Ruby: a, b = b, a
来源：http://xl.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://qp.wgjwhj.cn

[A20] 读取标准输入
来源：http://ab.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://iz.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gm.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nk.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://mh.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://zi.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://id.szxytkj.cn

Ruby: gets.chomp
来源：http://rf.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://jl.huanxung.cn

[A21] 保留指定小数位输出
来源：http://tx.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://mq.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cw.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://zn.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://fm.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://mu.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://og.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://wj.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://cf.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://aw.muxihuayi.cn

Py:   len(s)
来源：http://tk.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xf.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://up.521024.cn

TS:   s.length
来源：http://wl.hnjuh.cn

Java: s.length()
来源：http://fq.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://on.shxzukj.cn

Ruby: s.length
来源：http://wh.9csxet.cn

C#:   s.Length
来源：http://iw.wgjwhj.cn

[A23] 大小写转换
来源：http://rh.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lp.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zq.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vq.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jo.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pw.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yz.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tc.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fo.nszjky.cn

[A24] 去除首尾空白
来源：http://mu.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uq.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dd.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yo.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oy.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vt.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://yn.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cu.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://am.hahajie.cn

[A25] 字符串比较
来源：http://ap.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ue.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fu.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nz.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iw.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ed.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ir.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kv.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jj.nszjky.cn

[A26] 类型转换总览
来源：http://rz.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ie.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pj.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hn.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://ns.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qk.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mn.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lz.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xt.huanxung.cn

================================================================================
来源：http://aq.bjjhwx.cn

B. 流程控制
来源：http://ab.shxzskj.cn

================================================================================
来源：http://ap.nszjky.cn

[B01] 条件判断 if / else
来源：http://fz.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ns.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ax.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bz.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ye.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lm.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uq.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rf.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cs.nszjky.cn

[B02] 多分支 else if / elif
来源：http://ik.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ek.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qe.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vb.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ow.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dx.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.haigaiapp.cn

[B03] switch / match / case
来源：http://kg.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://go.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qb.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://js.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sw.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fx.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yj.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ls.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sq.szsharing.cn

[B04] for 计数循环
来源：http://fs.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://fm.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zd.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qj.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aq.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fj.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ax.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ov.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cz.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ay.asd995.cn

Py:   for item in arr: print(item)
来源：http://bp.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ax.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ra.muxihuayi.cn


<!-- 参考信息 -->