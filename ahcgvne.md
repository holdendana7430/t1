代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qi.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cf.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tp.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://to.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rv.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pi.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pi.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nd.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qk.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ex.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mz.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rz.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bm.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oo.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bi.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lv.szxytkj.cn

================================================================================
来源：http://ed.panjiajie.cn

A. 基础语法与类型
来源：http://qv.szsharing.cn

================================================================================
来源：http://pk.nszjky.cn

[A01] Hello World
来源：http://ta.colortex.cn

Py:   print("Hello, World!")
来源：http://gt.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://od.asd995.cn

JS:   console.log("Hello, World!");
来源：http://qg.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pc.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://py.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://gt.521024.cn

Ruby: puts "Hello, World!"
来源：http://er.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tx.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://cy.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hd.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ws.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://aw.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tn.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://uk.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://ev.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://zg.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wf.shtwfgs.cn

[A03] 常量定义
来源：http://wf.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xh.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ij.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://as.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://wo.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://ak.lnxyls.cn

Go:   const PI = 3.14159
来源：http://mu.panjiajie.cn

Ruby: PI = 3.14159
来源：http://vg.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://hz.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://tn.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tq.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://su.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fh.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://cf.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fn.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hj.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uj.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://wf.panjiajie.cn

[A05] 整数除法与取模
来源：http://tn.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fw.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zv.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vn.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wf.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://aw.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://lp.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://nq.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://rq.nicolike.cn

[A06] 字符串转数字
来源：http://ld.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://yk.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zw.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cg.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xm.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://if.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rb.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kl.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://de.szsharing.cn

[A07] 数字转字符串
来源：http://jl.shxzskj.cn

Py:   str(42)
来源：http://nq.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://hd.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://zl.lnxyls.cn

TS:   String(42)
来源：http://wo.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xs.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://wt.9csxet.cn

Ruby: 42.to_s
来源：http://ce.9csxet.cn

C#:   42.ToString()
来源：http://ov.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://gy.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ss.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vs.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ul.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cr.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fa.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://so.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nc.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dx.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://mk.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cr.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://by.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sm.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sc.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hl.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hi.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cs.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ln.yuntaijiaju.cn

[A10] 生成随机数
来源：http://wl.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://bq.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://zy.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ig.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zv.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://op.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vo.haigaiapp.cn

Ruby: rand(1..100)
来源：http://vz.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://kd.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://tk.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://mg.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://al.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tz.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dr.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://rg.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rw.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cj.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gw.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://lc.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jc.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zz.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://ku.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://wi.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://mk.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sb.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://vd.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://zh.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fg.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://ri.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://pr.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://cm.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://re.colortex.cn

Java: "第一行\n第二行"
来源：http://gr.newstarts.cn

Go:   "第一行\n第二行"
来源：http://vs.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://jn.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://kj.colortex.cn

[A14] 注释写法
来源：http://qn.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ox.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ht.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://dh.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://dh.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ho.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://lx.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tn.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://fx.nszjky.cn

[A15] 空值判断与默认值
来源：http://mj.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://zo.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://fg.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://xn.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://la.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://no.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://kv.521024.cn

Ruby: value = data || "默认值"
来源：http://zk.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://pr.nicolike.cn

[A16] 真假值判断规则
来源：http://hh.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://te.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xb.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bv.haigaiapp.cn

TS:   if (!x) {}
来源：http://xp.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ak.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pn.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nr.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qg.huanxung.cn

[A17] 位运算
来源：http://jm.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bw.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://az.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qb.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ay.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://kt.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://un.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://bp.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ph.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vz.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://mh.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qp.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://py.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://ii.9csxet.cn

[A19] 交换两个变量
来源：http://oz.chemitech.net.cn

Py:   a, b = b, a
来源：http://vu.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jo.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://cc.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://xt.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://sd.gzmigu.cn

Go:   a, b = b, a
来源：http://wn.newstarts.cn

Ruby: a, b = b, a
来源：http://ac.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://iw.hahajie.cn

[A20] 读取标准输入
来源：http://zd.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://vo.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wq.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zb.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://zf.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ea.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ws.nszjky.cn

Ruby: gets.chomp
来源：http://nn.shxzskj.cn

C#:   Console.ReadLine();
来源：http://tu.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://qf.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://cu.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jz.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://nf.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://ol.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://xa.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://od.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://yv.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://uu.asd995.cn

[A22] 获取字符串长度
来源：http://id.lnxyls.cn

Py:   len(s)
来源：http://fr.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qc.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cp.haigaiapp.cn

TS:   s.length
来源：http://tm.szxytkj.cn

Java: s.length()
来源：http://hg.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kf.haigaiapp.cn

Ruby: s.length
来源：http://dh.bjjhwx.cn

C#:   s.Length
来源：http://xf.nszjky.cn

[A23] 大小写转换
来源：http://jm.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jh.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vx.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ic.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wt.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://az.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uq.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rc.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://no.shxzukj.cn

[A24] 去除首尾空白
来源：http://ai.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ir.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ga.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cw.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cl.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tt.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://lk.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qi.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fx.huixinmuqiang.cn

[A25] 字符串比较
来源：http://kd.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://pf.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kp.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hh.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mr.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://do.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fh.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bl.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ak.nszjky.cn

[A26] 类型转换总览
来源：http://ri.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zf.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rn.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dj.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://sy.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oq.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pr.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pk.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hl.bjjhwx.cn

================================================================================
来源：http://mo.huixiangedu.cn

B. 流程控制
来源：http://ve.jctech888.com.cn

================================================================================
来源：http://wi.gzmigu.cn

[B01] 条件判断 if / else
来源：http://tb.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xi.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://st.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nf.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ca.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://en.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zd.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lb.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pr.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://mg.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hg.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zp.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qt.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hf.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mj.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yc.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fk.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.muxihuayi.cn

[B03] switch / match / case
来源：http://rf.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dy.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://re.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bc.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tt.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wl.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ct.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vd.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sz.haigaiapp.cn

[B04] for 计数循环
来源：http://hg.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://cv.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wm.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ab.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cw.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nu.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://dp.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kl.asd995.cn

[B05] 遍历数组 / 列表
来源：http://vm.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://kb.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nm.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gy.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kb.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ag.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://if.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://qt.shtwfgs.cn


<!-- 参考信息 -->