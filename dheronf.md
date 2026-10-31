代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://az.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zh.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pm.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jf.szsharing.cn

================================================================================
来源：http://lx.nszjky.cn

A. 基础语法与类型
来源：http://rp.chemitech.net.cn

================================================================================
来源：http://co.huanxung.cn

[A01] Hello World
来源：http://kq.hnjuh.cn

Py:   print("Hello, World!")
来源：http://jq.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://iq.asd995.cn

JS:   console.log("Hello, World!");
来源：http://qp.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://to.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://ms.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://lg.colortex.cn

Ruby: puts "Hello, World!"
来源：http://mu.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ni.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://ow.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tk.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gm.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bu.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tn.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://pn.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ls.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://ii.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xp.panjiajie.cn

[A03] 常量定义
来源：http://gg.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://st.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://ry.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://he.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://fw.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://wp.newstarts.cn

Go:   const PI = 3.14159
来源：http://dc.nicolike.cn

Ruby: PI = 3.14159
来源：http://th.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://hq.hahajie.cn

[A04] 判断变量类型
来源：http://av.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rk.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mi.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lk.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://mr.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gr.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gr.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bz.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://rc.521024.cn

[A05] 整数除法与取模
来源：http://uu.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gw.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nj.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kg.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ea.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://wa.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://ss.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://mr.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://uu.huanxung.cn

[A06] 字符串转数字
来源：http://jr.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://im.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eu.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sm.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mi.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sx.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sk.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ll.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ar.huixiangedu.cn

[A07] 数字转字符串
来源：http://my.lnxyls.cn

Py:   str(42)
来源：http://lv.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://il.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://pn.shxzskj.cn

TS:   String(42)
来源：http://jn.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fx.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://du.bjjhwx.cn

Ruby: 42.to_s
来源：http://oc.nicolike.cn

C#:   42.ToString()
来源：http://vc.hahajie.cn

[A08] 取整与四舍五入
来源：http://ug.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pe.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ox.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iq.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fa.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://na.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://er.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gu.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vf.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://hz.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://in.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hp.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wk.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ig.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mw.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mv.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cn.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hn.wgjwhj.cn

[A10] 生成随机数
来源：http://ng.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://jq.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://ea.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wv.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://cp.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gg.shxzskj.cn

Ruby: rand(1..100)
来源：http://yf.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://ns.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://ub.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://lh.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aw.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hv.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rd.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://nf.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bd.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ac.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zp.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://kd.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://op.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ws.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://hn.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://gj.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://nt.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zk.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://vj.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://qr.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lg.9csxet.cn

Py:   "第一行\n第二行"
来源：http://tw.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://lo.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://ya.szsharing.cn

TS:   "第一行\n第二行"
来源：http://eu.nszjky.cn

Java: "第一行\n第二行"
来源：http://tp.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://lo.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://yh.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://to.muxihuayi.cn

[A14] 注释写法
来源：http://ik.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oy.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fq.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://qx.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://wh.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ps.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://uy.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ju.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://br.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://rs.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://um.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://kf.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://hl.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://tw.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xf.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://az.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://re.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://fe.shxzukj.cn

[A16] 真假值判断规则
来源：http://xu.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wf.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://od.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gc.521024.cn

TS:   if (!x) {}
来源：http://wy.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dg.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uz.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://iq.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sh.szxytkj.cn

[A17] 位运算
来源：http://pp.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rq.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://co.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tp.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dh.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lh.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://wq.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://vj.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://hp.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gf.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qj.521024.cn

Java: (int) 'A'; (char) 65
来源：http://zd.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zi.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://dg.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://ks.asd995.cn

[A19] 交换两个变量
来源：http://sj.shxzskj.cn

Py:   a, b = b, a
来源：http://jw.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mj.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://eo.asd995.cn

TS:   [a, b] = [b, a];
来源：http://vm.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://tp.huanxung.cn

Go:   a, b = b, a
来源：http://sc.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://wy.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://cb.521024.cn

[A20] 读取标准输入
来源：http://se.szsharing.cn

Py:   name = input("请输入：")
来源：http://wu.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fz.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jt.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://gq.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://to.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ve.asd995.cn

Ruby: gets.chomp
来源：http://uw.szxytkj.cn

C#:   Console.ReadLine();
来源：http://cl.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://ki.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://dc.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fr.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://ja.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://oz.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://xy.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mq.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://tg.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://xk.hnjuh.cn

[A22] 获取字符串长度
来源：http://fl.szxytkj.cn

Py:   len(s)
来源：http://bt.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tg.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://py.yuexingan06.cn

TS:   s.length
来源：http://kv.muxihuayi.cn

Java: s.length()
来源：http://ry.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ga.hnjuh.cn

Ruby: s.length
来源：http://va.nicolike.cn

C#:   s.Length
来源：http://pb.shtwfgs.cn

[A23] 大小写转换
来源：http://kh.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xx.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kc.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ak.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vg.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wk.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fw.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mq.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sf.szsharing.cn

[A24] 去除首尾空白
来源：http://eu.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mt.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wv.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qv.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://er.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wq.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://vn.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gk.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tg.nicolike.cn

[A25] 字符串比较
来源：http://xi.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://pi.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jp.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qk.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ju.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pm.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://te.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ae.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zc.shtwfgs.cn

[A26] 类型转换总览
来源：http://yu.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jn.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tc.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jn.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://xh.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://he.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://su.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ox.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ar.shxzskj.cn

================================================================================
来源：http://tt.szsharing.cn

B. 流程控制
来源：http://gp.jctech888.com.cn

================================================================================
来源：http://le.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://sp.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ib.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ma.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mu.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sw.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yy.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wu.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://je.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jc.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://ez.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ha.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vv.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ly.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bf.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nd.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.szxytkj.cn

[B03] switch / match / case
来源：http://yf.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yt.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lx.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pc.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uh.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cn.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oa.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://du.muxihuayi.cn

[B04] for 计数循环
来源：http://ia.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://nq.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mv.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ef.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nb.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mc.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zt.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://uf.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ko.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ey.huanxung.cn

Py:   for item in arr: print(item)
来源：http://dp.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ra.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fq.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ns.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fo.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lt.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://et.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pp.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://tf.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ao.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nr.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://en.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zv.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zm.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ju.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zx.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gb.haigaiapp.cn

[B07] while 循环
来源：http://qg.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://zz.nicolike.cn


<!-- 参考信息 -->