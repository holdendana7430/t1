代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://or.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qm.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ss.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ts.shxzskj.cn

================================================================================
来源：http://rj.hnjuh.cn

A. 基础语法与类型
来源：http://pr.hahajie.cn

================================================================================
来源：http://ej.haigaiapp.cn

[A01] Hello World
来源：http://mr.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ey.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://hx.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://qx.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cl.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://rp.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://cw.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://rh.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gs.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://qp.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ui.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zn.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cy.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ia.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://pj.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://qg.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://et.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ht.huanxung.cn

[A03] 常量定义
来源：http://mz.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yu.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://mr.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://lr.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://hy.521024.cn

Java: static final double PI = 3.14159;
来源：http://uq.szxytkj.cn

Go:   const PI = 3.14159
来源：http://wm.newstarts.cn

Ruby: PI = 3.14159
来源：http://vz.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://rc.newstarts.cn

[A04] 判断变量类型
来源：http://qr.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ho.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qd.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gv.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://he.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mx.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://to.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kk.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://rk.shxzskj.cn

[A05] 整数除法与取模
来源：http://by.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xs.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ka.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ce.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kr.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://ia.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://hh.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://hr.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://fs.asd995.cn

[A06] 字符串转数字
来源：http://sa.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://jc.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gd.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vl.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://px.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://al.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vf.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://um.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yn.wgjwhj.cn

[A07] 数字转字符串
来源：http://kx.wgjwhj.cn

Py:   str(42)
来源：http://rz.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://yt.huanxung.cn

JS:   String(42); (42).toString()
来源：http://jr.shxzskj.cn

TS:   String(42)
来源：http://et.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://up.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://az.chemitech.net.cn

Ruby: 42.to_s
来源：http://uh.huixiangedu.cn

C#:   42.ToString()
来源：http://dc.shxzukj.cn

[A08] 取整与四舍五入
来源：http://av.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dn.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fb.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bi.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aj.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://js.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nn.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gs.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bx.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://ay.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fn.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ym.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mc.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oi.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ww.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cu.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nf.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bh.newstarts.cn

[A10] 生成随机数
来源：http://er.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://tl.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://mc.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bf.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hj.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://yu.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lh.shxzskj.cn

Ruby: rand(1..100)
来源：http://dg.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://mu.szsharing.cn

[A11] 条件表达式（三元）
来源：http://fv.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://lq.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uh.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ex.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://of.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://gr.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yu.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tc.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fu.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://ds.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://av.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://za.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://zq.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://mp.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://et.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zk.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://st.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://ac.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hd.9csxet.cn

Py:   "第一行\n第二行"
来源：http://gy.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://yn.hahajie.cn

JS:   "第一行\n第二行"
来源：http://vs.hahajie.cn

TS:   "第一行\n第二行"
来源：http://ul.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://vw.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ti.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://cr.huanxung.cn

C#:   "第一行\n第二行"
来源：http://vl.colortex.cn

[A14] 注释写法
来源：http://ap.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sb.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wq.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://eo.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://gv.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wi.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://le.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xu.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://oo.colortex.cn

[A15] 空值判断与默认值
来源：http://np.521024.cn

Py:   value = data or "默认值"
来源：http://hm.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://yu.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://gp.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://di.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ul.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://lg.newstarts.cn

Ruby: value = data || "默认值"
来源：http://qi.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://wt.bjjhwx.cn

[A16] 真假值判断规则
来源：http://ba.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dv.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ge.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zg.nszjky.cn

TS:   if (!x) {}
来源：http://kt.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nq.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bs.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wj.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gv.gzmigu.cn

[A17] 位运算
来源：http://lq.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mh.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fq.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qg.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://of.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bm.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oa.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ye.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://yw.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://zm.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://ys.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jq.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dx.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://rs.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kg.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://pf.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://dt.huixiangedu.cn

[A19] 交换两个变量
来源：http://pb.nicolike.cn

Py:   a, b = b, a
来源：http://in.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ya.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://ql.asd995.cn

TS:   [a, b] = [b, a];
来源：http://pe.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://do.nicolike.cn

Go:   a, b = b, a
来源：http://wd.asd995.cn

Ruby: a, b = b, a
来源：http://od.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://lp.huixiangedu.cn

[A20] 读取标准输入
来源：http://wz.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://gf.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ul.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qr.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://wy.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://vd.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://no.muxihuayi.cn

Ruby: gets.chomp
来源：http://we.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ca.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://br.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://fc.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wf.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://gc.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://mo.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ev.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tg.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://hu.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://vc.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://tt.huixiangedu.cn

Py:   len(s)
来源：http://un.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yc.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tk.hahajie.cn

TS:   s.length
来源：http://nn.chemitech.net.cn

Java: s.length()
来源：http://be.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hp.shxzskj.cn

Ruby: s.length
来源：http://pw.asd995.cn

C#:   s.Length
来源：http://fx.szsharing.cn

[A23] 大小写转换
来源：http://wc.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ds.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qx.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://um.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yq.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gp.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qk.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sz.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rr.nicolike.cn

[A24] 去除首尾空白
来源：http://qr.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ck.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pp.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://th.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zy.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ot.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://mg.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ah.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yd.shtwfgs.cn

[A25] 字符串比较
来源：http://nj.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://kn.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://re.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xt.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vh.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gu.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bm.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hc.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://su.gzmigu.cn

[A26] 类型转换总览
来源：http://ph.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xm.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://el.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://em.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://ii.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ee.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ub.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wh.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sp.huixinmuqiang.cn

================================================================================
来源：http://hm.huanxung.cn

B. 流程控制
来源：http://cb.colortex.cn

================================================================================
来源：http://ko.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://rc.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ua.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ji.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wc.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://na.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qi.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pe.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zw.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ag.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://uq.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ix.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oa.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vy.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vy.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.shxzukj.cn

[B03] switch / match / case
来源：http://bf.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rk.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iu.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qa.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gc.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lm.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gi.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zo.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cf.shxzskj.cn

[B04] for 计数循环
来源：http://vb.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://jb.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lu.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sl.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fc.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vg.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ms.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://vb.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qj.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ge.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ez.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sz.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vj.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wn.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qc.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://np.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://km.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sf.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://gl.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dh.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gp.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xp.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jg.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://it.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nk.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sf.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wp.9csxet.cn

[B07] while 循环
来源：http://qv.asd995.cn

Py:   while i < 10: i += 1
来源：http://cr.9csxet.cn


<!-- 参考信息 -->