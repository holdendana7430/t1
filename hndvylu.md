代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://jk.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://od.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bz.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ak.huixiangedu.cn

================================================================================
来源：http://gg.jctech888.com.cn

A. 基础语法与类型
来源：http://rw.huixiangedu.cn

================================================================================
来源：http://al.szsharing.cn

[A01] Hello World
来源：http://kk.shxzukj.cn

Py:   print("Hello, World!")
来源：http://km.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://tt.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://mb.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ec.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://xd.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://je.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://gr.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zn.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://sl.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tt.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yk.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dx.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tz.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://pg.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://wn.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://co.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://na.gzmigu.cn

[A03] 常量定义
来源：http://kf.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lx.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://ix.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://mm.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://yu.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://rg.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://ca.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://ts.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://gx.muxihuayi.cn

[A04] 判断变量类型
来源：http://qv.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hl.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wa.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jt.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://ah.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ed.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lz.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rs.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://xf.yuexingan06.cn

[A05] 整数除法与取模
来源：http://hf.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://an.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fp.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ya.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cv.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://yg.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://fi.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://fg.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://wf.wgjwhj.cn

[A06] 字符串转数字
来源：http://nf.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://gb.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pr.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kh.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cd.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wm.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lt.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://el.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ix.haigaiapp.cn

[A07] 数字转字符串
来源：http://gs.panjiajie.cn

Py:   str(42)
来源：http://mn.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://tt.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://mr.wgjwhj.cn

TS:   String(42)
来源：http://hq.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yt.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://mq.bjjhwx.cn

Ruby: 42.to_s
来源：http://rs.521024.cn

C#:   42.ToString()
来源：http://qb.nicolike.cn

[A08] 取整与四舍五入
来源：http://jd.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://th.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vf.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wr.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zo.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uq.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bc.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fx.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yi.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://vi.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vi.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fx.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ek.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wc.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oe.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dm.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pn.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ml.jctech888.com.cn

[A10] 生成随机数
来源：http://mw.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://th.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://vg.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bh.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bl.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://zs.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oh.hahajie.cn

Ruby: rand(1..100)
来源：http://hq.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://za.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://pc.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://la.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gj.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lq.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bp.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://tu.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://de.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xn.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://no.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://yl.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rh.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yt.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://zg.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://wu.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://sl.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ln.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://re.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://pv.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://po.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://vi.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://um.huanxung.cn

JS:   "第一行\n第二行"
来源：http://rt.nszjky.cn

TS:   "第一行\n第二行"
来源：http://wa.panjiajie.cn

Java: "第一行\n第二行"
来源：http://dx.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://vr.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://cv.asd995.cn

C#:   "第一行\n第二行"
来源：http://dx.shtwfgs.cn

[A14] 注释写法
来源：http://oi.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kj.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://sj.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://li.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bu.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://fc.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cd.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://gq.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://oi.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ob.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://zl.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://vx.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://bz.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cz.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://et.9csxet.cn

Ruby: value = data || "默认值"
来源：http://ow.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://un.shxzukj.cn

[A16] 真假值判断规则
来源：http://ec.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bv.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ml.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rh.chemitech.net.cn

TS:   if (!x) {}
来源：http://gm.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://as.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kj.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jv.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ur.newstarts.cn

[A17] 位运算
来源：http://kw.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ik.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://la.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wv.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tf.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ic.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://jv.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://jt.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wp.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fx.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://pg.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nt.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://ug.521024.cn

C#:   (int)'A'; (char)65
来源：http://fx.colortex.cn

[A19] 交换两个变量
来源：http://vy.bookmarksfly.cn

Py:   a, b = b, a
来源：http://ph.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cy.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://bm.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://ks.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://mn.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://qi.haigaiapp.cn

Ruby: a, b = b, a
来源：http://bn.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ct.huanxung.cn

[A20] 读取标准输入
来源：http://bb.szsharing.cn

Py:   name = input("请输入：")
来源：http://ct.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ro.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://si.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://pw.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://oj.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dz.gzmigu.cn

Ruby: gets.chomp
来源：http://uj.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://ip.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://xn.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://kg.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pq.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://cv.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://rs.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://xc.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yf.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://fl.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://fm.newstarts.cn

[A22] 获取字符串长度
来源：http://px.asd995.cn

Py:   len(s)
来源：http://ms.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nn.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zn.wgjwhj.cn

TS:   s.length
来源：http://zb.panjiajie.cn

Java: s.length()
来源：http://zs.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ih.panjiajie.cn

Ruby: s.length
来源：http://vt.bjjhwx.cn

C#:   s.Length
来源：http://ll.huanxung.cn

[A23] 大小写转换
来源：http://au.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mk.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lr.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://br.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fz.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jf.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ta.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wz.newstarts.cn

[A24] 去除首尾空白
来源：http://nz.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://go.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sj.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rq.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cj.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mq.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://zf.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://km.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fn.shxzukj.cn

[A25] 字符串比较
来源：http://eq.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://rz.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uq.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hg.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gl.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vh.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hv.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jf.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://tq.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ju.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gc.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ni.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://lo.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dm.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ql.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kv.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lr.huixiangedu.cn

================================================================================
来源：http://tq.colortex.cn

B. 流程控制
来源：http://df.szxytkj.cn

================================================================================
来源：http://ey.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://wh.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ty.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vu.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pu.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sw.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://po.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zq.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sp.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pa.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://gx.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gj.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lj.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gi.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jh.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://au.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sd.jctech888.com.cn

[B03] switch / match / case
来源：http://yp.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ax.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hu.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://je.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wf.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lx.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zh.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lh.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xd.hnjuh.cn

[B04] for 计数循环
来源：http://pr.521024.cn

Py:   for i in range(10): print(i)
来源：http://rc.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zp.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://me.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qp.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wr.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lc.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://rj.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gk.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://fw.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ti.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pz.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hv.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://py.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kt.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tb.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://yf.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://un.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://xc.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ly.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ax.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rz.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dg.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ot.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xu.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.chemitech.net.cn

[B07] while 循环
来源：http://ez.nszjky.cn

Py:   while i < 10: i += 1
来源：http://vk.bjjhwx.cn


<!-- 参考信息 -->