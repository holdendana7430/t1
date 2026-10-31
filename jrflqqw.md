代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://rf.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://on.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hd.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tt.shxzukj.cn

================================================================================
来源：http://oi.szxytkj.cn

A. 基础语法与类型
来源：http://gm.asd995.cn

================================================================================
来源：http://cz.gzmigu.cn

[A01] Hello World
来源：http://ed.hnjuh.cn

Py:   print("Hello, World!")
来源：http://fv.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://yb.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://ad.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wy.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://gt.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://kw.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://cu.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gd.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ck.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cq.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://by.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cl.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://br.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://bs.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://ss.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://jm.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jx.nicolike.cn

[A03] 常量定义
来源：http://kf.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xv.asd995.cn

PHP:  const PI = 3.14159;
来源：http://zd.colortex.cn

JS:   const PI = 3.14159;
来源：http://lj.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://vw.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://tu.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://yj.521024.cn

Ruby: PI = 3.14159
来源：http://hf.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://bd.szxytkj.cn

[A04] 判断变量类型
来源：http://ot.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oo.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lg.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mj.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://rr.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://su.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gw.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://os.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://kf.shxzskj.cn

[A05] 整数除法与取模
来源：http://pj.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lu.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tc.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://im.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rk.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://ub.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://pv.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://tf.521024.cn

C#:   7 / 2; 7 % 2
来源：http://ot.huanxung.cn

[A06] 字符串转数字
来源：http://ji.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://mo.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wp.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ep.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uu.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kx.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ka.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://op.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lu.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://oz.hahajie.cn

Py:   str(42)
来源：http://ip.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ui.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://ig.szxytkj.cn

TS:   String(42)
来源：http://tz.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xx.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ku.newstarts.cn

Ruby: 42.to_s
来源：http://es.jctech888.com.cn

C#:   42.ToString()
来源：http://zs.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://uj.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ez.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ai.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fn.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cw.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wl.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xl.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ao.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bz.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://wq.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xa.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rk.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ur.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pe.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pq.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cb.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kt.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bc.huanxung.cn

[A10] 生成随机数
来源：http://su.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://hu.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://ii.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fd.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eb.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ys.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bj.szsharing.cn

Ruby: rand(1..100)
来源：http://vw.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://sd.9csxet.cn

[A11] 条件表达式（三元）
来源：http://uu.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://rq.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pm.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rx.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://do.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://jx.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xm.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xa.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rk.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://fn.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://np.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zj.colortex.cn

JS:   `Hello, ${name}!`
来源：http://cj.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://nt.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://jz.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bq.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://ca.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://lg.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uj.521024.cn

Py:   "第一行\n第二行"
来源：http://ju.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://yi.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://xe.9csxet.cn

TS:   "第一行\n第二行"
来源：http://le.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://ga.521024.cn

Go:   "第一行\n第二行"
来源：http://qj.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://es.szsharing.cn

C#:   "第一行\n第二行"
来源：http://gy.521024.cn

[A14] 注释写法
来源：http://fz.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zu.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jl.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://fz.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://fg.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ap.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://ho.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ay.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://xa.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://vk.szxytkj.cn

Py:   value = data or "默认值"
来源：http://vr.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://gr.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://xn.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://wb.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ob.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://sv.huanxung.cn

Ruby: value = data || "默认值"
来源：http://yc.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://hr.shtwfgs.cn

[A16] 真假值判断规则
来源：http://wd.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ch.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fw.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cl.panjiajie.cn

TS:   if (!x) {}
来源：http://lv.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ns.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://no.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ni.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wf.shtwfgs.cn

[A17] 位运算
来源：http://fz.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bt.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kh.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hi.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fo.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zw.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://un.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://jn.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://hu.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nu.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mx.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://ew.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ne.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://ww.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://qo.hahajie.cn

[A19] 交换两个变量
来源：http://ce.nicolike.cn

Py:   a, b = b, a
来源：http://ru.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zu.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ak.asd995.cn

TS:   [a, b] = [b, a];
来源：http://fo.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://ew.haigaiapp.cn

Go:   a, b = b, a
来源：http://ly.shxzskj.cn

Ruby: a, b = b, a
来源：http://cn.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://il.haigaiapp.cn

[A20] 读取标准输入
来源：http://cb.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://af.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ou.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ue.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://ha.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://fz.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ge.521024.cn

Ruby: gets.chomp
来源：http://tn.shxzukj.cn

C#:   Console.ReadLine();
来源：http://vm.newstarts.cn

[A21] 保留指定小数位输出
来源：http://lu.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://sn.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wa.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://th.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://nd.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://oa.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ar.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://ql.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://dm.szsharing.cn

[A22] 获取字符串长度
来源：http://ty.jctech888.com.cn

Py:   len(s)
来源：http://sx.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tn.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iq.newstarts.cn

TS:   s.length
来源：http://ew.huanxung.cn

Java: s.length()
来源：http://ci.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fr.newstarts.cn

Ruby: s.length
来源：http://ua.hnjuh.cn

C#:   s.Length
来源：http://de.hnjuh.cn

[A23] 大小写转换
来源：http://ni.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sd.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xw.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zi.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://er.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://er.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hs.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rw.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ib.newstarts.cn

[A24] 去除首尾空白
来源：http://nk.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mm.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://my.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gd.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://su.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zn.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://sy.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jv.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vv.shtwfgs.cn

[A25] 字符串比较
来源：http://rs.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://kh.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rb.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://go.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kb.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hs.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fh.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ay.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zc.nicolike.cn

[A26] 类型转换总览
来源：http://vp.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mb.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tp.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hp.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://me.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yz.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://id.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rz.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ov.9csxet.cn

================================================================================
来源：http://rv.huanxung.cn

B. 流程控制
来源：http://sz.panjiajie.cn

================================================================================
来源：http://gw.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://we.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://if.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uc.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sh.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nt.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vg.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rt.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yc.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://nu.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hd.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kh.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bb.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mx.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.newstarts.cn

[B03] switch / match / case
来源：http://rh.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bl.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ze.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ce.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gz.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jt.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xz.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ox.muxihuayi.cn

[B04] for 计数循环
来源：http://uf.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://rh.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://av.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lp.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://og.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qu.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rz.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://ej.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ih.521024.cn

[B05] 遍历数组 / 列表
来源：http://gf.huanxung.cn

Py:   for item in arr: print(item)
来源：http://gg.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ut.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iz.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sr.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lt.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yo.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ai.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yy.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://hq.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ye.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rc.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hv.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bg.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mp.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://on.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://et.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kk.bookmarksfly.cn

[B07] while 循环
来源：http://vd.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://wm.newstarts.cn


<!-- 参考信息 -->