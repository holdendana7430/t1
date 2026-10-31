代发 wailian999

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dr.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cc.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://po.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rj.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ny.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ks.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xg.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lo.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gw.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kv.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xy.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wj.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://an.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://li.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mx.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kf.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ug.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xp.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kr.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pe.nicolike.cn

================================================================================
来源：http://ob.huixiangedu.cn

A. 基础语法与类型
来源：http://ms.yuexingan06.cn

================================================================================
来源：http://up.9csxet.cn

[A01] Hello World
来源：http://rb.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://pv.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://bt.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://vn.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lh.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://uo.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://dq.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://ku.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xb.szxytkj.cn

[A02] 变量声明与赋值
来源：http://lk.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ru.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sn.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lw.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dl.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://vf.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://ba.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://zl.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vd.colortex.cn

[A03] 常量定义
来源：http://db.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dv.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://cj.nicolike.cn

JS:   const PI = 3.14159;
来源：http://tk.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://ls.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://xg.hnjuh.cn

Go:   const PI = 3.14159
来源：http://pi.shxzukj.cn

Ruby: PI = 3.14159
来源：http://mg.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://qh.bookmarksfly.cn

[A04] 判断变量类型
来源：http://uk.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xx.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zo.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nt.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://qk.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ec.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xt.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gi.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://dm.panjiajie.cn

[A05] 整数除法与取模
来源：http://rh.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iy.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://os.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bb.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kn.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://kt.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://po.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://uj.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://im.asd995.cn

[A06] 字符串转数字
来源：http://pt.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://jj.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lz.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xb.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vy.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://as.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fp.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dg.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ys.hahajie.cn

[A07] 数字转字符串
来源：http://bg.nicolike.cn

Py:   str(42)
来源：http://ko.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://dn.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://xo.yuntaijiaju.cn

TS:   String(42)
来源：http://wa.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://op.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://oi.muxihuayi.cn

Ruby: 42.to_s
来源：http://zi.521024.cn

C#:   42.ToString()
来源：http://ea.huanxung.cn

[A08] 取整与四舍五入
来源：http://zd.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ec.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bl.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pa.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rt.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zj.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pu.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hw.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xt.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://gf.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tm.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ij.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pf.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kw.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gw.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ml.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ek.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://in.shxzskj.cn

[A10] 生成随机数
来源：http://df.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://xm.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://dy.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ow.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zx.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://kt.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://po.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://gu.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://xt.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://ef.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tl.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pg.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pp.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zu.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://nh.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ew.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kt.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://js.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://cn.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vx.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ts.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://ka.colortex.cn

TS:   `Hello, ${name}!`
来源：http://hz.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://lb.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jy.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://jb.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://oc.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rt.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://nz.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://xx.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://yr.colortex.cn

TS:   "第一行\n第二行"
来源：http://rb.szsharing.cn

Java: "第一行\n第二行"
来源：http://mk.asd995.cn

Go:   "第一行\n第二行"
来源：http://jc.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://mp.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://qq.bookmarksfly.cn

[A14] 注释写法
来源：http://oq.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cs.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vq.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://gf.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://tp.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://of.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://jm.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ul.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://lv.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://bk.9csxet.cn

Py:   value = data or "默认值"
来源：http://gg.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://lo.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://uq.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://jn.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oy.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://ge.szsharing.cn

Ruby: value = data || "默认值"
来源：http://ps.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://ox.shtwfgs.cn

[A16] 真假值判断规则
来源：http://cv.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pn.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tf.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nv.szsharing.cn

TS:   if (!x) {}
来源：http://ek.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://le.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ra.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fh.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gr.shxzskj.cn

[A17] 位运算
来源：http://ik.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vk.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iw.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nr.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vg.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zv.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ur.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://sj.asd995.cn

Py:   ord("A"); chr(65)
来源：http://bk.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://mw.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://za.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://to.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://qt.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kt.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://by.colortex.cn

C#:   (int)'A'; (char)65
来源：http://gb.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://yt.asd995.cn

Py:   a, b = b, a
来源：http://dr.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ha.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://br.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://ts.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://lx.hahajie.cn

Go:   a, b = b, a
来源：http://kh.colortex.cn

Ruby: a, b = b, a
来源：http://mh.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://zs.wgjwhj.cn

[A20] 读取标准输入
来源：http://xj.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://dg.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oe.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mt.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://jx.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://sw.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ay.haigaiapp.cn

Ruby: gets.chomp
来源：http://wt.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ls.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ha.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ds.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jf.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://kh.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://oc.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://jj.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mr.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://fh.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://hb.haigaiapp.cn

[A22] 获取字符串长度
来源：http://mg.bjjhwx.cn

Py:   len(s)
来源：http://ac.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qy.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oj.szsharing.cn

TS:   s.length
来源：http://es.nicolike.cn

Java: s.length()
来源：http://pc.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gs.lnxyls.cn

Ruby: s.length
来源：http://cc.muxihuayi.cn

C#:   s.Length
来源：http://uv.newstarts.cn

[A23] 大小写转换
来源：http://pb.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ti.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gj.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://el.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://em.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fq.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vm.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nm.shtwfgs.cn

[A24] 去除首尾空白
来源：http://hr.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fp.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yc.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xg.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xn.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ao.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://nl.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nb.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lh.bookmarksfly.cn

[A25] 字符串比较
来源：http://hf.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://cj.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://la.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hf.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ky.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ir.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ar.wgjwhj.cn

[A26] 类型转换总览
来源：http://dj.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fz.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vb.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ml.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ca.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vu.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eq.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hy.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gl.521024.cn

================================================================================
来源：http://dd.huixinmuqiang.cn

B. 流程控制
来源：http://yn.lnxyls.cn

================================================================================
来源：http://kn.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ra.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://he.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xr.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nr.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pl.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bx.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hf.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yf.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jx.521024.cn

[B02] 多分支 else if / elif
来源：http://lk.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cp.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gd.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oq.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sz.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ee.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.nicolike.cn

[B03] switch / match / case
来源：http://ya.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oz.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qh.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tl.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yi.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qy.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dp.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ne.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://br.newstarts.cn

[B04] for 计数循环
来源：http://za.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://if.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pg.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gg.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jo.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zp.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vu.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://bq.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xw.colortex.cn

[B05] 遍历数组 / 列表
来源：http://zx.huanxung.cn

Py:   for item in arr: print(item)
来源：http://yp.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wt.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ng.yuexingan06.cn


<!-- 参考信息 -->