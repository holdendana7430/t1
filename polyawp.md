代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zw.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pq.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bd.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bx.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zf.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kl.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bd.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hp.shxzskj.cn

================================================================================
来源：http://ff.haigaiapp.cn

A. 基础语法与类型
来源：http://ae.hnjuh.cn

================================================================================
来源：http://be.521024.cn

[A01] Hello World
来源：http://bi.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://hd.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://cz.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://yb.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zb.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://cg.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ni.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://qq.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ig.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://la.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ba.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://je.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ga.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hl.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://an.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://dr.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://gt.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dh.gzmigu.cn

[A03] 常量定义
来源：http://bw.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vf.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://ir.521024.cn

JS:   const PI = 3.14159;
来源：http://rj.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://tr.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://ni.panjiajie.cn

Go:   const PI = 3.14159
来源：http://ks.hahajie.cn

Ruby: PI = 3.14159
来源：http://wo.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://lo.yuexingan06.cn

[A04] 判断变量类型
来源：http://lc.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://js.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lo.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ri.521024.cn

TS:   typeof x; x instanceof Date
来源：http://it.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ys.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hd.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vv.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://sp.hnjuh.cn

[A05] 整数除法与取模
来源：http://xa.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yk.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ck.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kl.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xf.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://py.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://wi.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://ai.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://kr.9csxet.cn

[A06] 字符串转数字
来源：http://df.521024.cn

Py:   int("42"); float("3.14")
来源：http://wa.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mo.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://je.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kq.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://me.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://km.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cl.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hh.gzmigu.cn

[A07] 数字转字符串
来源：http://qn.9csxet.cn

Py:   str(42)
来源：http://tq.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://dy.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://jz.yuexingan06.cn

TS:   String(42)
来源：http://dd.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dt.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://em.panjiajie.cn

Ruby: 42.to_s
来源：http://fp.jianghongdianzi.cn

C#:   42.ToString()
来源：http://cg.colortex.cn

[A08] 取整与四舍五入
来源：http://vt.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ce.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ag.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://od.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xg.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oy.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yx.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wy.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wf.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://ch.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bf.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://db.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bo.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wl.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lx.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vf.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fb.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jr.newstarts.cn

[A10] 生成随机数
来源：http://eb.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://dj.nszjky.cn

PHP:  random_int(1, 100);
来源：http://pn.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kq.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://et.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://lq.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://au.shtwfgs.cn

Ruby: rand(1..100)
来源：http://rx.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://wp.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://qo.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://xi.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://oo.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ed.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uu.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://nw.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ag.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pq.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mk.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://dp.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gg.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ct.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://rv.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://zx.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://fk.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ih.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://gk.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://le.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://us.hahajie.cn

Py:   "第一行\n第二行"
来源：http://tf.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://th.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://rz.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://ox.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://mw.hahajie.cn

Go:   "第一行\n第二行"
来源：http://wr.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://np.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://gm.nszjky.cn

[A14] 注释写法
来源：http://ky.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hs.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ba.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://sg.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://ez.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qo.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://gi.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jz.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://qr.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://tl.colortex.cn

Py:   value = data or "默认值"
来源：http://cd.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ay.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://un.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://rz.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ng.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://dm.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://hj.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ja.muxihuayi.cn

[A16] 真假值判断规则
来源：http://im.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vo.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wj.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ad.chemitech.net.cn

TS:   if (!x) {}
来源：http://rf.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jt.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sq.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vn.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://be.shxzskj.cn

[A17] 位运算
来源：http://al.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ot.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xe.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://al.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qi.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ja.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nb.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ff.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://zc.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://oa.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://kb.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qq.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xg.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://nt.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mt.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://fe.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://cf.haigaiapp.cn

[A19] 交换两个变量
来源：http://ue.9csxet.cn

Py:   a, b = b, a
来源：http://uf.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qg.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ji.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://lr.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://ai.shxzukj.cn

Go:   a, b = b, a
来源：http://fo.521024.cn

Ruby: a, b = b, a
来源：http://zl.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://rm.hnjuh.cn

[A20] 读取标准输入
来源：http://dg.asd995.cn

Py:   name = input("请输入：")
来源：http://mi.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://el.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://br.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://yp.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://yy.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ar.yuexingan06.cn

Ruby: gets.chomp
来源：http://yz.9csxet.cn

C#:   Console.ReadLine();
来源：http://ul.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://qy.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://tt.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eb.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://qm.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://nm.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://yo.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ga.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://to.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://vc.wgjwhj.cn

[A22] 获取字符串长度
来源：http://fk.szxytkj.cn

Py:   len(s)
来源：http://im.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ul.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dm.haigaiapp.cn

TS:   s.length
来源：http://sk.hnjuh.cn

Java: s.length()
来源：http://df.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://es.jctech888.com.cn

Ruby: s.length
来源：http://vn.haigaiapp.cn

C#:   s.Length
来源：http://gk.asd995.cn

[A23] 大小写转换
来源：http://tn.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mg.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fu.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ft.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jn.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://na.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ne.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kw.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tb.haigaiapp.cn

[A24] 去除首尾空白
来源：http://hm.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mk.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lw.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dr.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zq.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jh.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://vk.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rl.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://me.newstarts.cn

[A25] 字符串比较
来源：http://kh.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://sn.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qy.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yz.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ej.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aj.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ia.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vc.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://ko.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://su.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nj.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zx.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://tj.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://me.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jp.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://us.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ro.shxzukj.cn

================================================================================
来源：http://fv.szxytkj.cn

B. 流程控制
来源：http://uk.chemitech.net.cn

================================================================================
来源：http://ca.hahajie.cn

[B01] 条件判断 if / else
来源：http://hj.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qj.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yl.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hg.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ww.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lb.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ch.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vf.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://jv.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rw.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pp.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ds.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zz.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sa.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ue.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fk.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bd.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pb.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lr.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eu.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lf.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eg.colortex.cn

[B04] for 计数循环
来源：http://xf.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ri.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zb.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xw.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ei.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xi.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ij.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wc.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://xb.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://tp.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://an.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lb.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bi.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tz.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gq.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://sm.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bc.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://kc.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://et.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ml.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cu.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hg.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sw.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ds.panjiajie.cn


<!-- 参考信息 -->