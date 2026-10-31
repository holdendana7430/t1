代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pj.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yf.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://es.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yk.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gi.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vs.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xz.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fl.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wn.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nn.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wu.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ga.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nh.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lc.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nn.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xa.521024.cn

================================================================================
来源：http://bp.bookmarksfly.cn

A. 基础语法与类型
来源：http://xq.hahajie.cn

================================================================================
来源：http://ll.szsharing.cn

[A01] Hello World
来源：http://oe.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://dt.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://ou.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://vy.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zv.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://wu.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://gv.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://dn.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lf.asd995.cn

[A02] 变量声明与赋值
来源：http://rd.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tb.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ll.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jg.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ui.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://vz.521024.cn

Go:   name := "Alex"; age := 20
来源：http://el.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://xx.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ui.shtwfgs.cn

[A03] 常量定义
来源：http://qj.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://su.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://xe.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://pz.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://tg.asd995.cn

Java: static final double PI = 3.14159;
来源：http://lc.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://yi.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://vd.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://gm.colortex.cn

[A04] 判断变量类型
来源：http://de.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ok.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xs.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aw.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://od.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ty.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://my.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wx.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://lk.muxihuayi.cn

[A05] 整数除法与取模
来源：http://dl.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ng.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kt.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qf.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ar.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://ey.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://hm.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://tk.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://bo.hnjuh.cn

[A06] 字符串转数字
来源：http://wu.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://ev.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gv.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lc.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gv.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vb.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zl.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://os.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eb.bjjhwx.cn

[A07] 数字转字符串
来源：http://dd.yuexingan06.cn

Py:   str(42)
来源：http://mi.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://py.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://ak.bjjhwx.cn

TS:   String(42)
来源：http://tt.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dj.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://fw.newstarts.cn

Ruby: 42.to_s
来源：http://mr.yuexingan06.cn

C#:   42.ToString()
来源：http://oy.nszjky.cn

[A08] 取整与四舍五入
来源：http://ib.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tk.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mj.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ui.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rq.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ie.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dw.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lv.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yq.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://hr.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tt.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://es.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fk.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jk.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://db.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://em.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ys.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bv.panjiajie.cn

[A10] 生成随机数
来源：http://za.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://cp.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://hm.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ck.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zl.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://mo.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tm.jctech888.com.cn

Ruby: rand(1..100)
来源：http://lm.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://gz.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://fs.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://pw.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ru.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gy.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ya.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://dd.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vq.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xj.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eg.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://bg.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ku.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cv.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://iz.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://hd.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://yq.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fn.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://yz.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://om.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ar.szsharing.cn

Py:   "第一行\n第二行"
来源：http://px.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://fs.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://jp.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://gs.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://dy.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://uj.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://xn.nszjky.cn

C#:   "第一行\n第二行"
来源：http://sd.panjiajie.cn

[A14] 注释写法
来源：http://zs.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bs.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bh.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://mt.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://ad.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://es.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://zl.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ub.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://vz.szxytkj.cn

[A15] 空值判断与默认值
来源：http://cq.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ur.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://np.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://jr.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://yw.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zj.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://sj.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://nc.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://tj.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ig.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mh.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pv.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rl.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://sq.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sv.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hi.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oi.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://he.9csxet.cn

[A17] 位运算
来源：http://ym.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lb.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uf.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fk.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bg.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vf.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dk.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ct.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://kz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://tp.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://nq.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fc.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://gz.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xw.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://sn.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://dh.nicolike.cn

[A19] 交换两个变量
来源：http://de.hnjuh.cn

Py:   a, b = b, a
来源：http://cj.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ia.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://pk.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://gk.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://wo.nszjky.cn

Go:   a, b = b, a
来源：http://ex.nicolike.cn

Ruby: a, b = b, a
来源：http://iy.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://go.hnjuh.cn

[A20] 读取标准输入
来源：http://rs.panjiajie.cn

Py:   name = input("请输入：")
来源：http://rq.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ce.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dp.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://mv.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://db.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ku.haigaiapp.cn

Ruby: gets.chomp
来源：http://ga.szsharing.cn

C#:   Console.ReadLine();
来源：http://fs.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://ks.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://lf.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ct.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ko.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://fj.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://zz.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qh.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://gz.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://qv.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://qk.jctech888.com.cn

Py:   len(s)
来源：http://cn.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kn.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hg.9csxet.cn

TS:   s.length
来源：http://jx.nicolike.cn

Java: s.length()
来源：http://ry.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ln.gzmigu.cn

Ruby: s.length
来源：http://yx.shtwfgs.cn

C#:   s.Length
来源：http://sb.jianghongdianzi.cn

[A23] 大小写转换
来源：http://xc.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xo.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://px.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jl.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vp.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nd.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qw.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qb.colortex.cn

[A24] 去除首尾空白
来源：http://gv.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rv.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://to.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gl.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://is.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sx.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://zj.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ud.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ox.nicolike.cn

[A25] 字符串比较
来源：http://qj.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://fs.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iv.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ya.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kl.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://th.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sj.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ah.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ct.shxzskj.cn

[A26] 类型转换总览
来源：http://yi.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://et.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dk.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rt.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://kn.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xd.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://im.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hj.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yr.nszjky.cn

================================================================================
来源：http://cg.huixinmuqiang.cn

B. 流程控制
来源：http://ha.muxihuayi.cn

================================================================================
来源：http://yd.hnjuh.cn

[B01] 条件判断 if / else
来源：http://nb.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pv.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://do.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kf.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qj.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bo.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fp.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zw.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vm.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://md.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tz.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zw.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://df.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zc.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yx.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ce.shtwfgs.cn

[B03] switch / match / case
来源：http://wh.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lj.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sq.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ty.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sm.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xb.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mf.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nn.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ol.jianghongdianzi.cn

[B04] for 计数循环
来源：http://eb.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ac.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ov.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xs.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://do.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://im.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://io.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://lo.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://je.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://xr.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://ye.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dj.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vu.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wb.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jj.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pp.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://gv.szsharing.cn


<!-- 参考信息 -->