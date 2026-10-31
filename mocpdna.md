代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sq.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jt.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ae.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tq.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ql.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hc.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cm.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pe.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pr.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fa.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xb.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lj.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://be.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ku.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zr.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zv.asd995.cn

================================================================================
来源：http://jl.huixiangedu.cn

A. 基础语法与类型
来源：http://sa.bjjhwx.cn

================================================================================
来源：http://pb.wgjwhj.cn

[A01] Hello World
来源：http://jt.gzmigu.cn

Py:   print("Hello, World!")
来源：http://mw.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://qv.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://vd.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wi.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://sq.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://cj.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://yn.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bh.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://kp.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wu.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lb.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vp.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yc.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://nm.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://xv.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://vp.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://id.jctech888.com.cn

[A03] 常量定义
来源：http://ax.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hp.asd995.cn

PHP:  const PI = 3.14159;
来源：http://ej.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://sk.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://ma.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://lj.shxzskj.cn

Go:   const PI = 3.14159
来源：http://qi.newstarts.cn

Ruby: PI = 3.14159
来源：http://hz.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://lm.huixiangedu.cn

[A04] 判断变量类型
来源：http://xp.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pu.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fi.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gz.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://dy.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bs.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ch.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wz.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://vz.lnxyls.cn

[A05] 整数除法与取模
来源：http://is.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ol.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kh.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xe.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ca.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://fs.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://yt.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://zl.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://hr.lnxyls.cn

[A06] 字符串转数字
来源：http://pk.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://er.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kb.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://js.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tj.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xa.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yd.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://up.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xm.521024.cn

[A07] 数字转字符串
来源：http://vv.wgjwhj.cn

Py:   str(42)
来源：http://du.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://oc.nicolike.cn

JS:   String(42); (42).toString()
来源：http://vb.chemitech.net.cn

TS:   String(42)
来源：http://au.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gp.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://nw.newstarts.cn

Ruby: 42.to_s
来源：http://zm.colortex.cn

C#:   42.ToString()
来源：http://pz.lnxyls.cn

[A08] 取整与四舍五入
来源：http://sb.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pe.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gp.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bs.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://be.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sz.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ij.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dh.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yn.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://jv.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ml.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xm.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://no.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mw.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rk.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mc.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ex.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wq.muxihuayi.cn

[A10] 生成随机数
来源：http://ca.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://ao.nicolike.cn

PHP:  random_int(1, 100);
来源：http://lh.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jf.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yn.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://gq.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hf.9csxet.cn

Ruby: rand(1..100)
来源：http://ux.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://av.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://ko.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://cr.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://no.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ed.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yk.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://vt.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ns.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ni.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gb.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://tt.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sz.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hx.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://ln.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://kp.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://hv.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://on.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://yb.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://nd.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yn.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://sd.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://yg.9csxet.cn

JS:   "第一行\n第二行"
来源：http://eg.nicolike.cn

TS:   "第一行\n第二行"
来源：http://wm.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://bj.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://jf.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://et.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://bt.szsharing.cn

[A14] 注释写法
来源：http://jc.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pb.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sj.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://ln.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://xq.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xb.521024.cn

Go:   // 单行；/* 多行 */
来源：http://xi.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fe.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://rf.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://ic.huanxung.cn

Py:   value = data or "默认值"
来源：http://ui.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ur.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://oa.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ck.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lj.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://cc.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://go.521024.cn

C#:   var value = data ?? "默认值";
来源：http://tr.hahajie.cn

[A16] 真假值判断规则
来源：http://ew.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qh.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ea.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wj.colortex.cn

TS:   if (!x) {}
来源：http://ax.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xk.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://et.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://aj.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tp.muxihuayi.cn

[A17] 位运算
来源：http://rb.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://se.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wc.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pa.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xe.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wd.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://fd.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://uz.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://my.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fn.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hy.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://cs.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nq.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://vt.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://lo.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://mu.9csxet.cn

Py:   a, b = b, a
来源：http://ac.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fl.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://lz.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://wn.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://it.jctech888.com.cn

Go:   a, b = b, a
来源：http://cl.asd995.cn

Ruby: a, b = b, a
来源：http://ls.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://oe.shxzskj.cn

[A20] 读取标准输入
来源：http://yj.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://qm.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ve.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wo.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://tt.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://gz.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uc.chemitech.net.cn

Ruby: gets.chomp
来源：http://sc.nszjky.cn

C#:   Console.ReadLine();
来源：http://iq.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://fv.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://uh.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nw.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://vw.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://vj.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://nd.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://de.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://qj.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://pz.huixiangedu.cn

[A22] 获取字符串长度
来源：http://re.colortex.cn

Py:   len(s)
来源：http://za.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zu.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bv.nicolike.cn

TS:   s.length
来源：http://pt.hnjuh.cn

Java: s.length()
来源：http://ga.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ji.shtwfgs.cn

Ruby: s.length
来源：http://eu.panjiajie.cn

C#:   s.Length
来源：http://jq.shxzskj.cn

[A23] 大小写转换
来源：http://zm.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bs.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hn.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://su.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gk.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fs.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jy.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sa.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tu.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fu.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cz.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ar.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ud.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ue.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://xf.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xk.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mn.yuntaijiaju.cn

[A25] 字符串比较
来源：http://oo.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://io.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ua.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://au.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mf.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://az.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zc.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qo.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xt.gzmigu.cn

[A26] 类型转换总览
来源：http://tn.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uq.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tj.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ux.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://ff.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xy.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rc.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ik.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://px.gzmigu.cn

================================================================================
来源：http://vn.haigaiapp.cn

B. 流程控制
来源：http://nz.shxzskj.cn

================================================================================
来源：http://zh.nicolike.cn

[B01] 条件判断 if / else
来源：http://xs.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xm.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://no.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vg.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lv.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://do.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ch.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pf.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://te.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://hn.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ak.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zy.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vp.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pu.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mp.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.huanxung.cn

[B03] switch / match / case
来源：http://gw.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pu.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zp.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nv.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pz.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zo.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pt.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cd.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ms.yuexingan06.cn

[B04] for 计数循环
来源：http://oz.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://mo.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ly.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ei.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hl.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ec.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ul.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://zb.nszjky.cn

Py:   for item in arr: print(item)
来源：http://lz.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zi.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ix.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pg.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dk.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uo.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://cc.chemitech.net.cn


<!-- 参考信息 -->