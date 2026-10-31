代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ls.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ld.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zq.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cr.yuntaijiaju.cn

================================================================================
来源：http://ke.nicolike.cn

A. 基础语法与类型
来源：http://gv.wgjwhj.cn

================================================================================
来源：http://ho.haigaiapp.cn

[A01] Hello World
来源：http://bn.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ns.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://ff.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://zj.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ge.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://rn.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://ke.asd995.cn

Ruby: puts "Hello, World!"
来源：http://qf.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mi.gzmigu.cn

[A02] 变量声明与赋值
来源：http://vd.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hj.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wf.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bo.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cr.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://hr.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://fl.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://gh.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://at.chemitech.net.cn

[A03] 常量定义
来源：http://bp.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oj.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://xr.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://zy.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://tj.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://nn.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://bo.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://jc.521024.cn

C#:   const double PI = 3.14159;
来源：http://wo.wgjwhj.cn

[A04] 判断变量类型
来源：http://wm.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iq.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://os.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ae.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ee.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qv.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://um.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lj.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://xo.jctech888.com.cn

[A05] 整数除法与取模
来源：http://zh.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nx.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ea.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rh.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://id.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://ni.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://cp.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://in.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://xi.jctech888.com.cn

[A06] 字符串转数字
来源：http://rx.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://tx.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kr.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ls.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://in.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wf.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xc.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qk.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iy.szsharing.cn

[A07] 数字转字符串
来源：http://ab.colortex.cn

Py:   str(42)
来源：http://om.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://ze.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://cz.gzmigu.cn

TS:   String(42)
来源：http://qy.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zd.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://wm.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://rj.hahajie.cn

C#:   42.ToString()
来源：http://wt.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://iv.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lb.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cv.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gc.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ym.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iq.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://be.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jh.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hn.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://ij.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qa.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mi.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hw.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ek.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yv.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pl.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mz.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bi.bjjhwx.cn

[A10] 生成随机数
来源：http://qo.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://pa.521024.cn

PHP:  random_int(1, 100);
来源：http://bd.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ye.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zu.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://tb.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aw.muxihuayi.cn

Ruby: rand(1..100)
来源：http://fn.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://gn.hahajie.cn

[A11] 条件表达式（三元）
来源：http://up.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://em.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://op.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wp.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mc.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zy.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ct.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nl.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vi.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://km.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://na.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://db.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://uo.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://qv.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://jn.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ub.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://zq.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://ba.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kc.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://cg.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://wv.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://kx.colortex.cn

TS:   "第一行\n第二行"
来源：http://ie.lnxyls.cn

Java: "第一行\n第二行"
来源：http://jm.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://qj.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://di.521024.cn

C#:   "第一行\n第二行"
来源：http://eo.huixinmuqiang.cn

[A14] 注释写法
来源：http://eq.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vh.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pj.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://sn.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ff.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ua.521024.cn

Go:   // 单行；/* 多行 */
来源：http://mi.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fq.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://sa.szsharing.cn

[A15] 空值判断与默认值
来源：http://vi.lnxyls.cn

Py:   value = data or "默认值"
来源：http://gi.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://gg.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://yl.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://mj.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gi.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://he.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://we.521024.cn

C#:   var value = data ?? "默认值";
来源：http://vp.szsharing.cn

[A16] 真假值判断规则
来源：http://cd.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oh.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fa.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bp.wgjwhj.cn

TS:   if (!x) {}
来源：http://vs.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bs.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cg.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ag.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ox.yuexingan06.cn

[A17] 位运算
来源：http://yq.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ae.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lx.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vg.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://og.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wg.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://vh.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://bc.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://ut.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://em.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gw.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://pf.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ow.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://zk.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://hs.521024.cn

[A19] 交换两个变量
来源：http://xn.lnxyls.cn

Py:   a, b = b, a
来源：http://vs.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nv.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://wo.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://im.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://jb.9csxet.cn

Go:   a, b = b, a
来源：http://pw.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://jk.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://gu.huanxung.cn

[A20] 读取标准输入
来源：http://xe.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ed.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ga.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://wv.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ie.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gz.521024.cn

Ruby: gets.chomp
来源：http://my.newstarts.cn

C#:   Console.ReadLine();
来源：http://zw.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ui.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://lz.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tf.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://lk.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ta.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://ti.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zb.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://qe.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://pp.shxzskj.cn

[A22] 获取字符串长度
来源：http://sp.hnjuh.cn

Py:   len(s)
来源：http://pj.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wb.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pa.colortex.cn

TS:   s.length
来源：http://gx.chemitech.net.cn

Java: s.length()
来源：http://iu.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fe.huanxung.cn

Ruby: s.length
来源：http://bg.gzmigu.cn

C#:   s.Length
来源：http://ao.panjiajie.cn

[A23] 大小写转换
来源：http://xh.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cj.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pf.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://or.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hv.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tu.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eu.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qy.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gs.shtwfgs.cn

[A24] 去除首尾空白
来源：http://ot.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ii.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rk.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fr.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://im.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vs.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://nx.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rs.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fu.hnjuh.cn

[A25] 字符串比较
来源：http://ia.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://vf.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ta.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hr.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nd.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qk.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ru.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://in.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://di.chemitech.net.cn

[A26] 类型转换总览
来源：http://lg.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zv.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bz.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rf.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://nn.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xb.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zr.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ab.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cr.wgjwhj.cn

================================================================================
来源：http://lb.chemitech.net.cn

B. 流程控制
来源：http://kk.wgjwhj.cn

================================================================================
来源：http://em.hnjuh.cn

[B01] 条件判断 if / else
来源：http://cl.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wz.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tm.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hm.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://no.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pu.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vf.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lt.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xq.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://by.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://at.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://he.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bm.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cl.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cb.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aq.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yn.colortex.cn

[B03] switch / match / case
来源：http://gg.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pq.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://px.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ky.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vn.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bt.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fb.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bo.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://om.asd995.cn

[B04] for 计数循环
来源：http://sj.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://fa.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ep.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kr.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ch.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wx.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://zu.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ib.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://jx.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://uu.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jx.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://em.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://on.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ip.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wh.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ey.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jf.colortex.cn

[B06] 遍历字典 / 对象
来源：http://wz.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://an.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aa.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rc.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gd.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zk.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uh.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wm.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yz.shtwfgs.cn

[B07] while 循环
来源：http://xu.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://af.newstarts.cn


<!-- 参考信息 -->