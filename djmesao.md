代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yj.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sp.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lr.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tn.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fx.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rv.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ze.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zd.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hq.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kq.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lg.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bu.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://az.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ni.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uj.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eg.newstarts.cn

================================================================================
来源：http://pf.gzmigu.cn

A. 基础语法与类型
来源：http://gy.yuntaijiaju.cn

================================================================================
来源：http://xl.panjiajie.cn

[A01] Hello World
来源：http://bu.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://sz.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://ss.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://nt.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sh.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://fg.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://dh.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://zu.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bw.nszjky.cn

[A02] 变量声明与赋值
来源：http://gu.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ue.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tk.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://al.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nf.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://dr.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://rv.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://tr.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qi.lnxyls.cn

[A03] 常量定义
来源：http://kp.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ig.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://ok.newstarts.cn

JS:   const PI = 3.14159;
来源：http://vb.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://ki.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://rj.colortex.cn

Go:   const PI = 3.14159
来源：http://ga.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://ti.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ww.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://sg.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cf.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wt.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yh.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://pn.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://me.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://td.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oz.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://nu.wgjwhj.cn

[A05] 整数除法与取模
来源：http://um.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://td.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nh.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qd.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jm.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://sd.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://wn.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://aw.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://ev.newstarts.cn

[A06] 字符串转数字
来源：http://cz.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://yz.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cu.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oc.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wa.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hw.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gb.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pv.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xr.szsharing.cn

[A07] 数字转字符串
来源：http://im.szxytkj.cn

Py:   str(42)
来源：http://vr.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://wc.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://mk.colortex.cn

TS:   String(42)
来源：http://ga.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dc.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://dq.wgjwhj.cn

Ruby: 42.to_s
来源：http://hx.chemitech.net.cn

C#:   42.ToString()
来源：http://bs.lnxyls.cn

[A08] 取整与四舍五入
来源：http://pp.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tm.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ud.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qs.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aj.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ui.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jb.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hx.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wl.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://ef.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eq.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wt.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cy.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pf.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nm.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ho.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ez.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xn.huixinmuqiang.cn

[A10] 生成随机数
来源：http://tx.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://ep.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://mi.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mj.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tj.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://gi.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://en.nicolike.cn

Ruby: rand(1..100)
来源：http://bb.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://bz.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://re.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://zl.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ce.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qq.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gu.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zm.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jr.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ue.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://de.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://mt.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ng.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gw.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://px.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ie.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://rp.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mh.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://ma.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ub.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bw.521024.cn

Py:   "第一行\n第二行"
来源：http://ia.colortex.cn

PHP:  "第一行\n第二行"
来源：http://xx.asd995.cn

JS:   "第一行\n第二行"
来源：http://fp.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://sa.asd995.cn

Java: "第一行\n第二行"
来源：http://wa.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://uh.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://zo.szsharing.cn

C#:   "第一行\n第二行"
来源：http://cm.asd995.cn

[A14] 注释写法
来源：http://hy.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mw.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vi.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://ac.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://ty.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://me.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://vx.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dx.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://ib.lnxyls.cn

[A15] 空值判断与默认值
来源：http://mh.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://ax.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://ao.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://wa.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://eg.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kp.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://wk.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://cc.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://qh.newstarts.cn

[A16] 真假值判断规则
来源：http://ew.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://br.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vl.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vj.jctech888.com.cn

TS:   if (!x) {}
来源：http://nj.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://be.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cy.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xw.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xo.nszjky.cn

[A17] 位运算
来源：http://ax.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ps.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://so.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cq.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yd.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://bm.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://cy.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://lw.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ct.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ey.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://fm.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dk.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://nq.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://gs.huanxung.cn

[A19] 交换两个变量
来源：http://gh.lnxyls.cn

Py:   a, b = b, a
来源：http://os.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ku.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://vx.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://pw.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://rs.newstarts.cn

Go:   a, b = b, a
来源：http://iz.jctech888.com.cn

Ruby: a, b = b, a
来源：http://hd.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://zc.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://it.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://qk.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vm.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wb.asd995.cn

TS:   // Node.js：readline 模块
来源：http://dk.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://xm.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://go.chemitech.net.cn

Ruby: gets.chomp
来源：http://dy.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ye.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://gf.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://qt.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://be.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://cb.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://rl.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://xj.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qr.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://nn.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://gb.9csxet.cn

[A22] 获取字符串长度
来源：http://oc.9csxet.cn

Py:   len(s)
来源：http://ly.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yq.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://si.huixinmuqiang.cn

TS:   s.length
来源：http://ad.jctech888.com.cn

Java: s.length()
来源：http://rc.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pg.szxytkj.cn

Ruby: s.length
来源：http://pg.shtwfgs.cn

C#:   s.Length
来源：http://ni.nszjky.cn

[A23] 大小写转换
来源：http://jj.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wy.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rt.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dl.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cf.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fm.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://py.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ru.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ty.newstarts.cn

[A24] 去除首尾空白
来源：http://mi.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://px.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kp.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jw.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ab.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pz.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://le.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bm.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xp.panjiajie.cn

[A25] 字符串比较
来源：http://sd.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://wo.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qd.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hp.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nd.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yi.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cc.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tl.521024.cn

[A26] 类型转换总览
来源：http://xa.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xh.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ok.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wp.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://xg.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xm.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yu.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jf.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pn.nszjky.cn

================================================================================
来源：http://bi.lnxyls.cn

B. 流程控制
来源：http://cy.shxzukj.cn

================================================================================
来源：http://xw.newstarts.cn

[B01] 条件判断 if / else
来源：http://fb.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wi.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sn.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bu.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rh.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://le.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gr.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mu.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ps.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://qi.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yk.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gn.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bt.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vi.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uz.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://at.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.gzmigu.cn

[B03] switch / match / case
来源：http://cv.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ti.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lq.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ip.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dk.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ci.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oa.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bm.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hg.521024.cn

[B04] for 计数循环
来源：http://ut.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://kv.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yh.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bl.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://na.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pt.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ax.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://mb.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vd.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://zk.nicolike.cn

Py:   for item in arr: print(item)
来源：http://qd.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nk.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mn.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sq.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://at.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yb.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://za.colortex.cn


<!-- 参考信息 -->