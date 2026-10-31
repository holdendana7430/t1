代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rn.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qm.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ky.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://db.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ug.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cv.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://me.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pw.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ha.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ld.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gl.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iy.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mc.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ik.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yr.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lm.bjjhwx.cn

================================================================================
来源：http://ul.shxzukj.cn

A. 基础语法与类型
来源：http://eo.panjiajie.cn

================================================================================
来源：http://ii.yuexingan06.cn

[A01] Hello World
来源：http://be.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://mk.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://yz.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ry.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hf.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://zd.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://ef.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://jm.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ph.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://ey.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bb.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uq.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ao.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bs.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://gq.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://is.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://hn.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://io.nszjky.cn

[A03] 常量定义
来源：http://yz.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ig.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://kj.huanxung.cn

JS:   const PI = 3.14159;
来源：http://am.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://uu.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://ij.huanxung.cn

Go:   const PI = 3.14159
来源：http://sv.hahajie.cn

Ruby: PI = 3.14159
来源：http://ie.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://hn.521024.cn

[A04] 判断变量类型
来源：http://tv.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hs.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://af.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mp.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://ap.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://md.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nc.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lc.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://oo.nszjky.cn

[A05] 整数除法与取模
来源：http://tu.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xs.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oo.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zo.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://td.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://vj.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://wd.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://sx.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://hu.yuexingan06.cn

[A06] 字符串转数字
来源：http://pp.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://op.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cj.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oe.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rf.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://an.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kw.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rs.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qh.hahajie.cn

[A07] 数字转字符串
来源：http://bt.bookmarksfly.cn

Py:   str(42)
来源：http://tg.521024.cn

PHP:  (string) 42; strval(42)
来源：http://hi.colortex.cn

JS:   String(42); (42).toString()
来源：http://wv.newstarts.cn

TS:   String(42)
来源：http://oz.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hn.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://tr.muxihuayi.cn

Ruby: 42.to_s
来源：http://gk.haigaiapp.cn

C#:   42.ToString()
来源：http://pi.huanxung.cn

[A08] 取整与四舍五入
来源：http://ya.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uw.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rn.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://el.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sl.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xu.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://od.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zo.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ye.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://pn.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ur.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://je.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fv.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ps.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cw.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ns.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wt.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lu.huixiangedu.cn

[A10] 生成随机数
来源：http://hv.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://kc.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://rm.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eu.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ms.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://kf.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ix.hnjuh.cn

Ruby: rand(1..100)
来源：http://do.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://jc.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://mc.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://hz.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vy.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://th.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ko.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://ub.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mv.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fn.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rx.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://ou.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://op.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hn.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://gm.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://pt.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://hd.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ab.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://fi.colortex.cn

C#:   $"Hello, {name}!"
来源：http://lf.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ub.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://kr.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://fz.newstarts.cn

JS:   "第一行\n第二行"
来源：http://tl.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://gp.shxzskj.cn

Java: "第一行\n第二行"
来源：http://vr.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://yc.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://wg.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://rh.haigaiapp.cn

[A14] 注释写法
来源：http://da.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sn.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sz.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ou.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://dw.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yn.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://ic.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ca.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://wi.nszjky.cn

[A15] 空值判断与默认值
来源：http://pg.szxytkj.cn

Py:   value = data or "默认值"
来源：http://hd.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://gd.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://gs.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://ah.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://va.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://sp.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://qa.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://yt.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ry.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qs.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ls.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lb.muxihuayi.cn

TS:   if (!x) {}
来源：http://ix.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yx.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hp.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xm.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bp.szsharing.cn

[A17] 位运算
来源：http://fe.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mh.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hc.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sy.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rb.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xe.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uq.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://ni.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://be.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://va.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cc.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ta.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://qd.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://av.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://pu.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://rd.gzmigu.cn

[A19] 交换两个变量
来源：http://qv.huanxung.cn

Py:   a, b = b, a
来源：http://ft.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ic.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://tk.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://qq.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://mc.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://sy.gzmigu.cn

Ruby: a, b = b, a
来源：http://ul.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://zn.bjjhwx.cn

[A20] 读取标准输入
来源：http://nw.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://yj.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ha.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://an.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://rm.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://nt.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rv.haigaiapp.cn

Ruby: gets.chomp
来源：http://nx.shxzskj.cn

C#:   Console.ReadLine();
来源：http://to.hahajie.cn

[A21] 保留指定小数位输出
来源：http://gs.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://uz.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vp.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://rq.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://hc.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://ez.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qr.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://dr.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ke.huixiangedu.cn

[A22] 获取字符串长度
来源：http://rk.panjiajie.cn

Py:   len(s)
来源：http://ky.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://in.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ko.panjiajie.cn

TS:   s.length
来源：http://vj.chemitech.net.cn

Java: s.length()
来源：http://mi.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oz.colortex.cn

Ruby: s.length
来源：http://fr.9csxet.cn

C#:   s.Length
来源：http://fr.shxzukj.cn

[A23] 大小写转换
来源：http://ib.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jr.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ef.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mp.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qy.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yo.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iq.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dd.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tz.szsharing.cn

[A24] 去除首尾空白
来源：http://kt.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xa.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iy.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wc.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lw.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bw.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://dm.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jp.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tn.panjiajie.cn

[A25] 字符串比较
来源：http://dn.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://hq.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ua.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tz.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zh.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oo.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oy.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zg.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tb.asd995.cn

[A26] 类型转换总览
来源：http://pe.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vf.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tj.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ia.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://zz.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fy.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hs.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fy.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hp.colortex.cn

================================================================================
来源：http://oa.szsharing.cn

B. 流程控制
来源：http://xw.szxytkj.cn

================================================================================
来源：http://ye.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://iq.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yw.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mh.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wk.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pv.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xf.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ak.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ym.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kq.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://jz.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pr.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dr.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cc.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jo.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sw.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ac.haigaiapp.cn

[B03] switch / match / case
来源：http://zs.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zp.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xv.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nl.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gd.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lo.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wn.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bk.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yv.szxytkj.cn

[B04] for 计数循环
来源：http://zk.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://bs.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yj.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jp.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qz.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vz.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://yc.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jt.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://qw.521024.cn

Py:   for item in arr: print(item)
来源：http://kx.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lc.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tl.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zg.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eu.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://na.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://go.panjiajie.cn


<!-- 参考信息 -->