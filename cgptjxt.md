代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nd.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oq.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uq.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nt.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cz.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vn.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://km.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ej.newstarts.cn

================================================================================
来源：http://ay.newstarts.cn

A. 基础语法与类型
来源：http://vy.nszjky.cn

================================================================================
来源：http://un.huanxung.cn

[A01] Hello World
来源：http://go.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://ps.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://qx.521024.cn

JS:   console.log("Hello, World!");
来源：http://fz.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zm.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://lo.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://rm.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://qj.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gj.hnjuh.cn

[A02] 变量声明与赋值
来源：http://dq.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://np.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lb.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dc.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://st.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://xi.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://uo.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://ur.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pp.jctech888.com.cn

[A03] 常量定义
来源：http://wz.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wi.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://gc.asd995.cn

JS:   const PI = 3.14159;
来源：http://hq.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://yz.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://xk.nicolike.cn

Go:   const PI = 3.14159
来源：http://sw.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://vd.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ki.newstarts.cn

[A04] 判断变量类型
来源：http://sg.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tv.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rh.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gn.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://yx.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ay.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dk.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gx.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://yk.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://rv.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ue.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fz.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jl.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xl.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://ju.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://xv.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://qh.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://zy.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://ub.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://zq.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tc.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vc.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nn.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vb.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vj.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ws.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kw.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://dy.hahajie.cn

Py:   str(42)
来源：http://cp.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://iu.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://ac.colortex.cn

TS:   String(42)
来源：http://cy.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://by.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://rh.nszjky.cn

Ruby: 42.to_s
来源：http://qb.shxzukj.cn

C#:   42.ToString()
来源：http://yy.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://wx.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ty.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lu.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mb.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wp.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vj.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ea.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gg.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://js.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ot.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xu.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vx.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ly.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kg.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jl.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dl.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://te.szsharing.cn

[A10] 生成随机数
来源：http://yp.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://nt.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://rq.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mq.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wi.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ta.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tp.hahajie.cn

Ruby: rand(1..100)
来源：http://jo.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://fc.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://la.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://hp.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ro.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qj.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oj.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://pw.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://on.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kw.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qy.521024.cn

[A12] 字符串插值 / 格式化
来源：http://ks.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://by.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zd.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://pd.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://zf.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ns.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qd.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://qj.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://vm.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lo.nicolike.cn

Py:   "第一行\n第二行"
来源：http://fi.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://fv.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ir.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://qr.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ta.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://jp.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://gb.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ea.colortex.cn

[A14] 注释写法
来源：http://so.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://al.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://by.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://zv.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://ls.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ko.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://wy.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://no.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://fl.panjiajie.cn

[A15] 空值判断与默认值
来源：http://oa.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://wx.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://yb.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://gz.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://lt.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xz.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://ke.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://rv.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://at.yuexingan06.cn

[A16] 真假值判断规则
来源：http://pz.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yl.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ak.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mn.lnxyls.cn

TS:   if (!x) {}
来源：http://hl.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wo.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gi.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://om.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cy.521024.cn

[A17] 位运算
来源：http://ha.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xi.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://om.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vq.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dx.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://pg.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://rw.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://tc.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ej.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gk.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://mt.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cz.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://pl.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://lj.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://dt.521024.cn

Py:   a, b = b, a
来源：http://db.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pi.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://sd.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ti.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://gx.521024.cn

Go:   a, b = b, a
来源：http://sl.asd995.cn

Ruby: a, b = b, a
来源：http://nq.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://zk.panjiajie.cn

[A20] 读取标准输入
来源：http://bo.nszjky.cn

Py:   name = input("请输入：")
来源：http://pe.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gh.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zi.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ls.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://ck.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ht.muxihuayi.cn

Ruby: gets.chomp
来源：http://iw.szxytkj.cn

C#:   Console.ReadLine();
来源：http://kx.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://ti.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://jv.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vq.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://xs.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://hu.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://is.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nf.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://uy.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://io.shxzukj.cn

[A22] 获取字符串长度
来源：http://le.muxihuayi.cn

Py:   len(s)
来源：http://na.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mx.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jn.huixiangedu.cn

TS:   s.length
来源：http://wq.szsharing.cn

Java: s.length()
来源：http://jb.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ys.shtwfgs.cn

Ruby: s.length
来源：http://fz.huanxung.cn

C#:   s.Length
来源：http://gd.nszjky.cn

[A23] 大小写转换
来源：http://xk.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kj.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zi.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://si.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dg.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wp.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dx.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qt.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sh.jctech888.com.cn

[A24] 去除首尾空白
来源：http://xi.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gb.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ws.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ix.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rd.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://km.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://qy.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ew.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ps.hnjuh.cn

[A25] 字符串比较
来源：http://fb.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://fe.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xj.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rl.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lo.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hs.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tq.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tw.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://td.colortex.cn

[A26] 类型转换总览
来源：http://le.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uj.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://te.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ap.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://hz.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uf.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uc.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iy.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qt.huixinmuqiang.cn

================================================================================
来源：http://kj.huanxung.cn

B. 流程控制
来源：http://qv.521024.cn

================================================================================
来源：http://mt.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://mp.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eg.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hj.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qs.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rc.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zj.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://on.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vr.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gb.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://qq.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fv.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bx.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fn.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mj.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ph.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.nicolike.cn

[B03] switch / match / case
来源：http://dz.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://to.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vi.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://an.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://up.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ra.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sj.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kl.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gh.521024.cn

[B04] for 计数循环
来源：http://mr.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://jn.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cq.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fo.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vx.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sf.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ir.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://er.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ob.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ix.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://po.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kq.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hv.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://td.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qw.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sq.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://vf.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lj.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://pk.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ia.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wb.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fp.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dk.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ec.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gi.panjiajie.cn


<!-- 参考信息 -->