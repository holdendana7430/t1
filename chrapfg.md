代发 wailian999

--------------------------------------------------------------------------------
来源：http://fd.jctech888.com.cn

目  录
来源：http://hi.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uo.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nu.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ob.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wh.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iz.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ka.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kt.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yp.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qm.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lt.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xf.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jm.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ew.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ti.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://re.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qh.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sk.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jj.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wy.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://it.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ej.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vm.bjjhwx.cn

================================================================================
来源：http://me.521024.cn

A. 基础语法与类型
来源：http://gi.huixinmuqiang.cn

================================================================================
来源：http://en.bjjhwx.cn

[A01] Hello World
来源：http://nc.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://rj.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://cl.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://wd.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ir.521024.cn

Java: System.out.println("Hello, World!");
来源：http://ml.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ct.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://zb.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://le.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://bd.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ql.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mn.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://be.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://od.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://ws.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://wz.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://wh.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://in.shtwfgs.cn

[A03] 常量定义
来源：http://xd.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hx.colortex.cn

PHP:  const PI = 3.14159;
来源：http://jt.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://fr.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://ln.asd995.cn

Java: static final double PI = 3.14159;
来源：http://dz.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://jv.szxytkj.cn

Ruby: PI = 3.14159
来源：http://oh.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://sj.panjiajie.cn

[A04] 判断变量类型
来源：http://mo.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kk.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zt.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mx.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://gr.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tm.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kb.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dr.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://sh.asd995.cn

[A05] 整数除法与取模
来源：http://il.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gq.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gv.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vd.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qb.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://ms.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://tf.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://yc.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://ae.lnxyls.cn

[A06] 字符串转数字
来源：http://lq.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://so.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://th.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kl.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ey.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mq.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jw.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uq.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vv.nszjky.cn

[A07] 数字转字符串
来源：http://to.shxzukj.cn

Py:   str(42)
来源：http://sw.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://bu.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://ez.jctech888.com.cn

TS:   String(42)
来源：http://pv.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cu.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://bl.shxzukj.cn

Ruby: 42.to_s
来源：http://qx.wgjwhj.cn

C#:   42.ToString()
来源：http://ce.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://wd.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qw.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bx.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mk.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cf.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kl.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qn.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ay.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ls.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://ks.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xo.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qx.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xz.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oo.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lf.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://el.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gc.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ar.huanxung.cn

[A10] 生成随机数
来源：http://qa.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://pf.asd995.cn

PHP:  random_int(1, 100);
来源：http://ye.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://il.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hg.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://pf.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bg.newstarts.cn

Ruby: rand(1..100)
来源：http://gw.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://oy.521024.cn

[A11] 条件表达式（三元）
来源：http://hd.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://rv.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gv.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://av.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bg.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://lu.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ud.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gh.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vw.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://rh.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://in.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fm.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://ka.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://ig.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://we.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wq.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://md.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://mb.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jg.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://zl.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://mk.9csxet.cn

JS:   "第一行\n第二行"
来源：http://zb.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://de.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://fm.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://sk.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://tx.9csxet.cn

C#:   "第一行\n第二行"
来源：http://lu.yuntaijiaju.cn

[A14] 注释写法
来源：http://ut.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gu.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://en.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ph.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://qk.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yj.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://nb.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ti.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://gz.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ff.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://rn.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://rg.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://qq.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://ka.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vh.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://no.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://sj.521024.cn

C#:   var value = data ?? "默认值";
来源：http://sa.newstarts.cn

[A16] 真假值判断规则
来源：http://jj.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wl.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mh.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yd.gzmigu.cn

TS:   if (!x) {}
来源：http://dq.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ct.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ga.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bv.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dp.bjjhwx.cn

[A17] 位运算
来源：http://lt.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ek.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nq.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://se.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://br.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qg.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wm.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://po.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://ay.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://co.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ub.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pw.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ej.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pr.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://iz.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://fc.nszjky.cn

[A19] 交换两个变量
来源：http://ye.hnjuh.cn

Py:   a, b = b, a
来源：http://ay.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ah.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://tq.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://rw.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://ll.chemitech.net.cn

Go:   a, b = b, a
来源：http://qv.asd995.cn

Ruby: a, b = b, a
来源：http://ek.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://pd.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://lc.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://db.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zc.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mm.521024.cn

TS:   // Node.js：readline 模块
来源：http://oz.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://ph.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lb.hnjuh.cn

Ruby: gets.chomp
来源：http://vj.gzmigu.cn

C#:   Console.ReadLine();
来源：http://uz.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://av.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://ks.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ox.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://zb.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://ua.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://hk.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://en.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://zs.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://ao.szxytkj.cn

[A22] 获取字符串长度
来源：http://jd.shxzskj.cn

Py:   len(s)
来源：http://ni.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ms.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gd.muxihuayi.cn

TS:   s.length
来源：http://pp.panjiajie.cn

Java: s.length()
来源：http://pu.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zt.shtwfgs.cn

Ruby: s.length
来源：http://tm.asd995.cn

C#:   s.Length
来源：http://ys.huanxung.cn

[A23] 大小写转换
来源：http://pa.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rh.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vd.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vp.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lp.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ff.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wa.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cc.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wu.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fv.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mq.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ew.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ym.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dj.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pb.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://dv.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dt.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xy.wgjwhj.cn

[A25] 字符串比较
来源：http://dn.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ri.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bw.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rf.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yp.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ry.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uj.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eq.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pb.szsharing.cn

[A26] 类型转换总览
来源：http://fx.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hp.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lq.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xl.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://pg.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vf.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qi.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iy.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wi.jctech888.com.cn

================================================================================
来源：http://fp.muxihuayi.cn

B. 流程控制
来源：http://gx.panjiajie.cn

================================================================================
来源：http://ob.hahajie.cn

[B01] 条件判断 if / else
来源：http://ec.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vp.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zm.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bd.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jp.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://on.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mo.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ij.hahajie.cn

[B02] 多分支 else if / elif
来源：http://mf.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fl.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cl.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zp.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jt.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pm.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ep.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.shtwfgs.cn

[B03] switch / match / case
来源：http://oa.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://we.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bb.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vu.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tu.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://le.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bu.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iv.szxytkj.cn

[B04] for 计数循环
来源：http://cv.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://jo.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nj.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://me.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nd.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kb.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ce.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://jq.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rt.nszjky.cn


<!-- 参考信息 -->