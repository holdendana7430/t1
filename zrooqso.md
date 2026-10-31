代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eu.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iq.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iy.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://po.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ns.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fs.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bz.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lk.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dk.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vx.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://om.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cw.jctech888.com.cn

================================================================================
来源：http://ez.muxihuayi.cn

A. 基础语法与类型
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://ei.huixiangedu.cn

[A01] Hello World
来源：http://fo.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://hu.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://dl.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://nk.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qn.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://yp.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://xb.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://ye.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pg.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://lx.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vt.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vn.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yi.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dj.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://te.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://ep.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://ep.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bj.huanxung.cn

[A03] 常量定义
来源：http://yy.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fn.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://hv.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://qf.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://kx.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://ax.9csxet.cn

Go:   const PI = 3.14159
来源：http://pp.521024.cn

Ruby: PI = 3.14159
来源：http://mq.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://lf.panjiajie.cn

[A04] 判断变量类型
来源：http://xw.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bx.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jx.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dv.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://kd.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gl.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://is.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sj.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://ez.shxzskj.cn

[A05] 整数除法与取模
来源：http://br.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fe.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://th.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://za.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tj.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://yn.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://cq.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://bx.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://kg.521024.cn

[A06] 字符串转数字
来源：http://ai.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://vm.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vp.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vu.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gx.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dt.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zl.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ef.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lz.bjjhwx.cn

[A07] 数字转字符串
来源：http://uq.colortex.cn

Py:   str(42)
来源：http://jj.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://ax.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://vb.panjiajie.cn

TS:   String(42)
来源：http://ku.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gv.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://wn.gzmigu.cn

Ruby: 42.to_s
来源：http://og.jctech888.com.cn

C#:   42.ToString()
来源：http://qe.nicolike.cn

[A08] 取整与四舍五入
来源：http://lq.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oq.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qg.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ar.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cm.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://id.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sp.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fq.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sj.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://mr.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fp.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wm.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ha.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bj.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ii.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oa.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wj.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://li.nicolike.cn

[A10] 生成随机数
来源：http://xq.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://yz.nicolike.cn

PHP:  random_int(1, 100);
来源：http://pe.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qy.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yp.chemitech.net.cn

Java: new Random().nextInt(100) + 1
来源：http://yb.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://di.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://sz.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://eg.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://zm.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://jn.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pj.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xt.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ba.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://tr.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ch.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ar.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pn.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://bj.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dg.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jf.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://wh.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://gf.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://mu.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ds.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://lz.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://rl.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qs.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://nb.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://tn.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://bt.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://jv.nicolike.cn

Java: "第一行\n第二行"
来源：http://ii.newstarts.cn

Go:   "第一行\n第二行"
来源：http://af.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://ir.asd995.cn

C#:   "第一行\n第二行"
来源：http://zy.asd995.cn

[A14] 注释写法
来源：http://zc.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://iv.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zy.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://oc.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://fv.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://me.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://eq.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qz.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://zy.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://gr.szxytkj.cn

Py:   value = data or "默认值"
来源：http://vs.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://yj.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://ew.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://ri.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zl.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://bj.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ir.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://fj.nicolike.cn

[A16] 真假值判断规则
来源：http://bi.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oh.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dn.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cc.gzmigu.cn

TS:   if (!x) {}
来源：http://ys.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sk.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://an.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zq.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kk.shtwfgs.cn

[A17] 位运算
来源：http://co.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vb.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://li.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cf.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bh.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ob.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tn.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xi.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://pu.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://ca.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ym.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rr.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://sw.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lv.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://yn.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://rz.huanxung.cn

[A19] 交换两个变量
来源：http://wj.newstarts.cn

Py:   a, b = b, a
来源：http://ol.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lc.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://qe.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://py.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://vk.wgjwhj.cn

Go:   a, b = b, a
来源：http://kv.9csxet.cn

Ruby: a, b = b, a
来源：http://zr.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://fr.shxzukj.cn

[A20] 读取标准输入
来源：http://ks.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://ph.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ab.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ei.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://cc.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://oc.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ol.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://of.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://wl.colortex.cn

[A21] 保留指定小数位输出
来源：http://wj.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://fp.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ns.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://dz.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ni.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://vs.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eg.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://me.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://xh.muxihuayi.cn

[A22] 获取字符串长度
来源：http://ky.szsharing.cn

Py:   len(s)
来源：http://kb.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yd.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vt.521024.cn

TS:   s.length
来源：http://bp.yuexingan06.cn

Java: s.length()
来源：http://ts.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jo.wgjwhj.cn

Ruby: s.length
来源：http://nh.szsharing.cn

C#:   s.Length
来源：http://ho.nszjky.cn

[A23] 大小写转换
来源：http://la.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lp.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fq.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qy.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hd.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cs.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fs.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ed.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gd.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://gp.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jf.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xg.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hy.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zd.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lx.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://xs.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kj.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://br.bjjhwx.cn

[A25] 字符串比较
来源：http://uj.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://oo.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lz.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ko.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://di.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xe.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xj.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bl.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pg.shtwfgs.cn

[A26] 类型转换总览
来源：http://oc.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xm.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vt.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zq.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://la.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eu.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zd.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xk.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jk.asd995.cn

================================================================================
来源：http://ne.9csxet.cn

B. 流程控制
来源：http://xt.huixinmuqiang.cn

================================================================================
来源：http://uq.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://gf.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ka.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ef.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dy.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ki.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xq.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zc.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://no.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wm.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://gb.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wr.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ff.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wm.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ur.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rm.shxzskj.cn

[B03] switch / match / case
来源：http://by.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ry.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fg.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://se.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yo.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cs.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iy.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ll.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vj.asd995.cn

[B04] for 计数循环
来源：http://kd.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://nm.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gh.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ik.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vp.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yi.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://on.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://ht.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://ne.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://hj.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://he.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://de.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ew.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://st.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mj.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://tg.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qc.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://me.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qn.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tj.muxihuayi.cn


<!-- 参考信息 -->