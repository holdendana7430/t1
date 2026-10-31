代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://fh.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tk.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xg.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sy.521024.cn

================================================================================
来源：http://wr.huixiangedu.cn

A. 基础语法与类型
来源：http://qh.shtwfgs.cn

================================================================================
来源：http://cy.yuexingan06.cn

[A01] Hello World
来源：http://hb.nicolike.cn

Py:   print("Hello, World!")
来源：http://hf.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://xs.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://uw.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dl.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://fn.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://jg.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://qt.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://md.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://gd.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ra.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yl.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hw.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lg.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://bz.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://va.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://xh.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://el.gzmigu.cn

[A03] 常量定义
来源：http://tu.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nn.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://ya.colortex.cn

JS:   const PI = 3.14159;
来源：http://vr.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://hi.colortex.cn

Java: static final double PI = 3.14159;
来源：http://zf.shxzukj.cn

Go:   const PI = 3.14159
来源：http://xf.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://ui.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://jw.colortex.cn

[A04] 判断变量类型
来源：http://xl.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tn.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nz.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rl.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://rp.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ud.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lr.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hg.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://vb.521024.cn

[A05] 整数除法与取模
来源：http://us.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wr.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hs.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ck.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jl.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://jx.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://oy.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://lg.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://ml.hahajie.cn

[A06] 字符串转数字
来源：http://kx.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://cq.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qm.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nn.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rj.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ej.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://er.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pi.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://go.521024.cn

[A07] 数字转字符串
来源：http://xx.hahajie.cn

Py:   str(42)
来源：http://cu.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://ez.asd995.cn

JS:   String(42); (42).toString()
来源：http://ms.huanxung.cn

TS:   String(42)
来源：http://wo.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zt.asd995.cn

Go:   strconv.Itoa(42)
来源：http://xi.newstarts.cn

Ruby: 42.to_s
来源：http://wf.bookmarksfly.cn

C#:   42.ToString()
来源：http://hj.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://yn.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ya.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lt.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ha.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://an.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ou.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gv.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sr.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fh.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://iq.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vx.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zr.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qk.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jj.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://no.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pg.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lk.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oy.shxzskj.cn

[A10] 生成随机数
来源：http://xu.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://kd.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://ww.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bk.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uq.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://ak.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pw.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://xd.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://vs.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://yp.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ka.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sr.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ye.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pg.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://oa.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://we.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lz.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sy.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://uv.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wq.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ta.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://ny.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://ga.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://of.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sa.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://uj.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://la.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gr.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://ti.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://ci.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://lx.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://lg.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://jy.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://aw.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://us.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://au.hnjuh.cn

[A14] 注释写法
来源：http://nz.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pr.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mn.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://pw.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://cj.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ok.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://iz.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bf.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://gq.asd995.cn

[A15] 空值判断与默认值
来源：http://kq.szxytkj.cn

Py:   value = data or "默认值"
来源：http://lu.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://mc.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://uv.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://xu.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lc.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://tc.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://ly.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://eh.wgjwhj.cn

[A16] 真假值判断规则
来源：http://qv.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qr.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pa.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kb.wgjwhj.cn

TS:   if (!x) {}
来源：http://gz.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bt.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cn.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ae.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ql.newstarts.cn

[A17] 位运算
来源：http://ez.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://et.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qe.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gd.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vj.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nd.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nn.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://ut.521024.cn

Py:   ord("A"); chr(65)
来源：http://tb.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://dr.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bp.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ke.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://iy.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mg.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://ql.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://wb.nicolike.cn

[A19] 交换两个变量
来源：http://bt.asd995.cn

Py:   a, b = b, a
来源：http://sj.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hk.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://uu.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ib.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://fv.panjiajie.cn

Go:   a, b = b, a
来源：http://zt.yuexingan06.cn

Ruby: a, b = b, a
来源：http://nb.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://fq.nicolike.cn

[A20] 读取标准输入
来源：http://vp.shxzukj.cn

Py:   name = input("请输入：")
来源：http://hl.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ph.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bm.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://zb.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://gp.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.wgjwhj.cn

Ruby: gets.chomp
来源：http://ub.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://ks.colortex.cn

[A21] 保留指定小数位输出
来源：http://nc.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://ya.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ju.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://gy.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://kh.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://lt.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bu.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mt.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://vn.nszjky.cn

[A22] 获取字符串长度
来源：http://iv.huixinmuqiang.cn

Py:   len(s)
来源：http://tm.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jj.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rx.yuexingan06.cn

TS:   s.length
来源：http://bh.szsharing.cn

Java: s.length()
来源：http://hy.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qb.hahajie.cn

Ruby: s.length
来源：http://yc.newstarts.cn

C#:   s.Length
来源：http://ow.bjjhwx.cn

[A23] 大小写转换
来源：http://pt.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wo.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pm.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://es.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uu.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fi.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ff.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ve.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://on.jctech888.com.cn

[A24] 去除首尾空白
来源：http://dg.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bn.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ne.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vq.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wp.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sj.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://ej.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fy.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kz.shxzukj.cn

[A25] 字符串比较
来源：http://ib.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://oy.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dl.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yc.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sq.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dx.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xg.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://up.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sj.nszjky.cn

[A26] 类型转换总览
来源：http://od.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fv.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bl.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://vb.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ch.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ok.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lq.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kf.hahajie.cn

================================================================================
来源：http://jl.nszjky.cn

B. 流程控制
来源：http://wq.asd995.cn

================================================================================
来源：http://lt.shxzukj.cn

[B01] 条件判断 if / else
来源：http://za.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sx.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://my.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sj.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mw.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mj.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wl.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jb.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vu.521024.cn

[B02] 多分支 else if / elif
来源：http://ax.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wj.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cz.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tp.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ou.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ti.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.hahajie.cn

[B03] switch / match / case
来源：http://vf.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mq.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ix.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gc.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xw.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gd.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gm.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xr.bjjhwx.cn

[B04] for 计数循环
来源：http://vk.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://yw.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ll.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://og.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://up.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yw.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://et.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://jz.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://av.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ix.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://yj.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xe.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tg.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xz.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ab.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sl.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://yr.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://so.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://mr.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://po.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lh.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xq.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mc.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ix.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cu.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kt.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sz.hahajie.cn

[B07] while 循环
来源：http://je.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://qe.shtwfgs.cn


<!-- 参考信息 -->