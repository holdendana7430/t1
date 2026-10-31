代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cl.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ab.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vx.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eb.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hj.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ed.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yq.gzmigu.cn

================================================================================
来源：http://dp.521024.cn

A. 基础语法与类型
来源：http://fk.muxihuayi.cn

================================================================================
来源：http://wh.gzmigu.cn

[A01] Hello World
来源：http://ya.panjiajie.cn

Py:   print("Hello, World!")
来源：http://mz.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://aa.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://cy.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xc.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://eh.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://mx.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://rm.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qq.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://gs.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://it.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tn.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fv.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ca.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://zn.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://li.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://as.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nd.521024.cn

[A03] 常量定义
来源：http://yl.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kf.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://ng.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://wh.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://mv.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://wo.shxzskj.cn

Go:   const PI = 3.14159
来源：http://nf.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://xh.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://xf.newstarts.cn

[A04] 判断变量类型
来源：http://oi.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tl.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ff.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vu.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://dt.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ql.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jd.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yk.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://uu.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://te.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://df.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vk.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://to.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gc.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://bw.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://up.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://ez.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://si.521024.cn

[A06] 字符串转数字
来源：http://yk.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://ai.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nu.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gs.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sj.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lr.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xr.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ju.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nn.jctech888.com.cn

[A07] 数字转字符串
来源：http://lv.jianghongdianzi.cn

Py:   str(42)
来源：http://xs.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://mv.nicolike.cn

JS:   String(42); (42).toString()
来源：http://rn.jianghongdianzi.cn

TS:   String(42)
来源：http://pb.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ad.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://kw.huanxung.cn

Ruby: 42.to_s
来源：http://wd.huixiangedu.cn

C#:   42.ToString()
来源：http://sz.asd995.cn

[A08] 取整与四舍五入
来源：http://hp.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gg.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://co.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xm.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nt.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pt.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cp.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hc.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://su.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://ec.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tz.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://au.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xr.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bn.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kn.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yp.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wu.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gi.huixinmuqiang.cn

[A10] 生成随机数
来源：http://fc.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://qx.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://ji.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jy.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eu.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://hx.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bp.szxytkj.cn

Ruby: rand(1..100)
来源：http://nw.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://yf.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://ye.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ru.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eh.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wi.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://np.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://nk.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wr.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mz.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gp.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://rk.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yc.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ux.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://nw.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://bu.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://ss.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sc.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://ta.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://wj.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hs.huanxung.cn

Py:   "第一行\n第二行"
来源：http://jk.asd995.cn

PHP:  "第一行\n第二行"
来源：http://bq.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://zu.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://rr.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://ch.nicolike.cn

Go:   "第一行\n第二行"
来源：http://tk.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://kh.newstarts.cn

C#:   "第一行\n第二行"
来源：http://ea.nicolike.cn

[A14] 注释写法
来源：http://bd.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://df.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oo.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ad.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://mn.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nb.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://ss.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sk.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://wt.521024.cn

[A15] 空值判断与默认值
来源：http://ty.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://zb.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://tv.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://ln.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://dy.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fj.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://bx.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://ne.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://dy.hahajie.cn

[A16] 真假值判断规则
来源：http://zc.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yn.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rf.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qr.asd995.cn

TS:   if (!x) {}
来源：http://ac.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cj.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://db.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://me.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ir.panjiajie.cn

[A17] 位运算
来源：http://bk.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rr.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fh.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rb.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hf.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dj.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ps.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://wc.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://br.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ga.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pc.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mn.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://fa.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qj.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://nk.colortex.cn

C#:   (int)'A'; (char)65
来源：http://hw.9csxet.cn

[A19] 交换两个变量
来源：http://io.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://mo.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rp.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://dz.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://lb.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://je.colortex.cn

Go:   a, b = b, a
来源：http://br.lnxyls.cn

Ruby: a, b = b, a
来源：http://rs.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://nl.huanxung.cn

[A20] 读取标准输入
来源：http://gg.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://gv.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uo.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://td.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://nv.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://om.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cw.wgjwhj.cn

Ruby: gets.chomp
来源：http://fi.szsharing.cn

C#:   Console.ReadLine();
来源：http://au.colortex.cn

[A21] 保留指定小数位输出
来源：http://zb.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://yq.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oh.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://lk.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://eg.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ht.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sm.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://fu.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://hf.szxytkj.cn

[A22] 获取字符串长度
来源：http://gf.newstarts.cn

Py:   len(s)
来源：http://uh.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eg.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sz.shtwfgs.cn

TS:   s.length
来源：http://oy.jianghongdianzi.cn

Java: s.length()
来源：http://wa.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nk.chemitech.net.cn

Ruby: s.length
来源：http://zh.szsharing.cn

C#:   s.Length
来源：http://br.jctech888.com.cn

[A23] 大小写转换
来源：http://vx.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ey.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ma.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pw.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rx.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vh.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sq.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zc.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uq.shxzukj.cn

[A24] 去除首尾空白
来源：http://da.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qt.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mh.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sb.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sf.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ye.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://vc.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dd.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wj.shxzukj.cn

[A25] 字符串比较
来源：http://ik.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://go.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nc.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cb.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xu.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hp.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ps.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ju.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nx.521024.cn

[A26] 类型转换总览
来源：http://oa.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dt.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ll.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pu.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://he.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hu.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ca.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vf.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rf.colortex.cn

================================================================================
来源：http://dm.lnxyls.cn

B. 流程控制
来源：http://tc.9csxet.cn

================================================================================
来源：http://xg.szxytkj.cn

[B01] 条件判断 if / else
来源：http://vb.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://op.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ff.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://go.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fw.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xb.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cn.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xq.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nl.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://lo.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qj.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fg.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pl.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xw.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xu.asd995.cn

[B03] switch / match / case
来源：http://pe.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lf.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yx.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ve.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ae.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oh.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ty.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jd.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dh.huixiangedu.cn

[B04] for 计数循环
来源：http://xq.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://xa.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://la.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xl.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sv.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://od.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://zd.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://az.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ip.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ve.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xa.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kw.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sz.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pu.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uu.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://mz.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aq.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://nb.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ix.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wg.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lg.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kj.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sy.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pt.lnxyls.cn


<!-- 参考信息 -->