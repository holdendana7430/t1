代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ws.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jo.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pn.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rl.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lv.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qf.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dw.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ud.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xj.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ax.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bo.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wg.asd995.cn

================================================================================
来源：http://ff.bjjhwx.cn

A. 基础语法与类型
来源：http://vy.huanxung.cn

================================================================================
来源：http://nv.gzmigu.cn

[A01] Hello World
来源：http://aj.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://ix.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://kq.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://oi.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dd.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://ns.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://zg.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://kn.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wm.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://sj.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jy.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gx.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gw.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jp.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://hp.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://ht.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://gj.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://if.chemitech.net.cn

[A03] 常量定义
来源：http://uk.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ys.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://yw.521024.cn

JS:   const PI = 3.14159;
来源：http://aa.521024.cn

TS:   const PI: number = 3.14159;
来源：http://rk.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://ry.panjiajie.cn

Go:   const PI = 3.14159
来源：http://yl.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://xz.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://lr.hahajie.cn

[A04] 判断变量类型
来源：http://dz.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wi.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uk.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kv.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://nb.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xx.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eb.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://we.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://ig.colortex.cn

[A05] 整数除法与取模
来源：http://ii.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://og.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ba.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pm.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ps.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://kz.521024.cn

Go:   7 / 2; 7 % 2
来源：http://je.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hu.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://mj.haigaiapp.cn

[A06] 字符串转数字
来源：http://un.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://ls.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rq.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ms.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pz.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gl.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bt.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ie.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://of.gzmigu.cn

[A07] 数字转字符串
来源：http://op.521024.cn

Py:   str(42)
来源：http://cp.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://gn.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://eb.nicolike.cn

TS:   String(42)
来源：http://dw.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rj.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://kp.lnxyls.cn

Ruby: 42.to_s
来源：http://kz.wgjwhj.cn

C#:   42.ToString()
来源：http://af.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://xd.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lc.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://to.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mp.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ue.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://br.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eg.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pp.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://sm.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cy.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cj.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zc.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pq.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fo.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rq.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yx.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pv.gzmigu.cn

[A10] 生成随机数
来源：http://fw.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://tg.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://fo.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gf.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tz.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://hx.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xp.panjiajie.cn

Ruby: rand(1..100)
来源：http://gl.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://xc.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://yl.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://qt.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ew.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ge.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tx.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ut.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fa.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rf.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tz.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://np.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://op.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xr.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://ou.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://fv.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://ig.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gt.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://hq.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://iw.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://si.szsharing.cn

Py:   "第一行\n第二行"
来源：http://ew.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://ir.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://jo.hahajie.cn

TS:   "第一行\n第二行"
来源：http://kf.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://od.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://bt.521024.cn

Ruby: "第一行\n第二行"
来源：http://bc.asd995.cn

C#:   "第一行\n第二行"
来源：http://db.muxihuayi.cn

[A14] 注释写法
来源：http://ih.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rk.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vl.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ng.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://nj.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zv.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://pu.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://no.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://re.shxzukj.cn

[A15] 空值判断与默认值
来源：http://uh.9csxet.cn

Py:   value = data or "默认值"
来源：http://ha.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://rh.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://cj.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://pp.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cm.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://lm.colortex.cn

Ruby: value = data || "默认值"
来源：http://db.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://ss.yuexingan06.cn

[A16] 真假值判断规则
来源：http://pk.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ek.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cy.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fn.chemitech.net.cn

TS:   if (!x) {}
来源：http://qi.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nx.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tc.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hg.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rm.521024.cn

[A17] 位运算
来源：http://kc.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ux.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sf.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gy.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://wv.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://hq.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://aq.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ot.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://si.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://cg.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://av.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ix.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://og.chemitech.net.cn

[A19] 交换两个变量
来源：http://fn.yuexingan06.cn

Py:   a, b = b, a
来源：http://qy.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tr.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://wl.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://tt.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://pq.nszjky.cn

Go:   a, b = b, a
来源：http://fq.gzmigu.cn

Ruby: a, b = b, a
来源：http://ty.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://zr.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://dr.gzmigu.cn

Py:   name = input("请输入：")
来源：http://og.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ry.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bz.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://at.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://mo.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ki.panjiajie.cn

Ruby: gets.chomp
来源：http://zm.lnxyls.cn

C#:   Console.ReadLine();
来源：http://fi.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://bb.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://xa.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bu.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://wi.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://et.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ky.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tz.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://pw.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://hs.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://xg.bjjhwx.cn

Py:   len(s)
来源：http://md.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vz.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lu.hahajie.cn

TS:   s.length
来源：http://ux.panjiajie.cn

Java: s.length()
来源：http://gp.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nx.521024.cn

Ruby: s.length
来源：http://na.hahajie.cn

C#:   s.Length
来源：http://yb.jianghongdianzi.cn

[A23] 大小写转换
来源：http://kv.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rq.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ry.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jx.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nj.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pn.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fh.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qh.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oc.muxihuayi.cn

[A24] 去除首尾空白
来源：http://ao.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ay.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vw.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wr.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rx.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ex.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://lr.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ye.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ys.newstarts.cn

[A25] 字符串比较
来源：http://ve.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://vc.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xm.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pd.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://he.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://er.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jj.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xp.asd995.cn

[A26] 类型转换总览
来源：http://jk.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sx.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bo.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ah.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://xi.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dd.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pn.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://of.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ze.yuexingan06.cn

================================================================================
来源：http://sx.szxytkj.cn

B. 流程控制
来源：http://qw.shxzskj.cn

================================================================================
来源：http://oh.shxzukj.cn

[B01] 条件判断 if / else
来源：http://va.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rv.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wi.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://om.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uc.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://me.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pl.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bo.huanxung.cn

[B02] 多分支 else if / elif
来源：http://xw.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vc.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gg.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xn.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jl.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rs.yuexingan06.cn

[B03] switch / match / case
来源：http://yn.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yh.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zq.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kk.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dv.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ry.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://by.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kq.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ya.szxytkj.cn

[B04] for 计数循环
来源：http://dq.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://aw.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ut.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lj.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ru.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ex.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://tw.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hp.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://yu.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://ak.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bz.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ro.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ia.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://op.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ky.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://es.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mr.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://dd.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://he.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gy.szsharing.cn


<!-- 参考信息 -->