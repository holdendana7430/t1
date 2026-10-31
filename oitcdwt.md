代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qg.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uw.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ev.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dn.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wa.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ul.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jo.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nn.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wm.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cb.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://po.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sc.huixinmuqiang.cn

================================================================================
来源：http://yv.szsharing.cn

A. 基础语法与类型
来源：http://tz.nszjky.cn

================================================================================
来源：http://ti.szsharing.cn

[A01] Hello World
来源：http://hq.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://rm.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://qt.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://xf.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sh.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://nf.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://nb.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://tg.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sn.colortex.cn

[A02] 变量声明与赋值
来源：http://qh.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qe.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wd.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cf.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ad.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://bw.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://du.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://cy.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rm.chemitech.net.cn

[A03] 常量定义
来源：http://ql.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lg.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://zx.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://gk.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://fy.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://ye.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://vk.newstarts.cn

Ruby: PI = 3.14159
来源：http://kr.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://tu.chemitech.net.cn

[A04] 判断变量类型
来源：http://ai.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gz.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xx.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mx.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ia.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fj.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qw.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hn.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://cw.nicolike.cn

[A05] 整数除法与取模
来源：http://qc.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mv.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qs.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jr.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bj.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://dg.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://ek.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://vx.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://jk.lnxyls.cn

[A06] 字符串转数字
来源：http://dt.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://kv.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://su.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://au.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://na.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fz.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ow.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://em.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sz.shxzukj.cn

[A07] 数字转字符串
来源：http://nl.huixinmuqiang.cn

Py:   str(42)
来源：http://kk.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://xi.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://dy.huixiangedu.cn

TS:   String(42)
来源：http://oa.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vj.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://be.jctech888.com.cn

Ruby: 42.to_s
来源：http://mw.asd995.cn

C#:   42.ToString()
来源：http://jc.shxzukj.cn

[A08] 取整与四舍五入
来源：http://om.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wm.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bq.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://at.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jr.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rk.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mo.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://co.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://si.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://fm.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://el.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fh.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zh.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yh.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ob.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fu.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xf.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nf.panjiajie.cn

[A10] 生成随机数
来源：http://zi.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://jf.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://mz.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ky.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kx.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://yk.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://je.bjjhwx.cn

Ruby: rand(1..100)
来源：http://vg.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://nw.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://tt.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://jt.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://li.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bx.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tp.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://ay.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fg.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lm.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mf.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://ya.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iu.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ze.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://wk.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://hw.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ht.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rz.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://nm.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://va.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uz.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://rj.colortex.cn

PHP:  "第一行\n第二行"
来源：http://eq.asd995.cn

JS:   "第一行\n第二行"
来源：http://mv.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://ha.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://cy.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://cy.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://gc.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://qg.jctech888.com.cn

[A14] 注释写法
来源：http://yt.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ne.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hd.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://nx.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://jp.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ei.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://ec.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ap.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://me.lnxyls.cn

[A15] 空值判断与默认值
来源：http://gs.szsharing.cn

Py:   value = data or "默认值"
来源：http://sd.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://sg.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://or.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://au.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://an.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://ig.newstarts.cn

Ruby: value = data || "默认值"
来源：http://nh.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://bk.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://oz.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pz.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bp.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nd.panjiajie.cn

TS:   if (!x) {}
来源：http://fs.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://du.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ah.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eh.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://au.nicolike.cn

[A17] 位运算
来源：http://qc.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yh.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://or.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://te.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dg.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cm.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mm.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ca.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://re.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://aa.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://kb.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://hu.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ae.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bh.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://gy.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zz.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://ak.521024.cn

C#:   (int)'A'; (char)65
来源：http://zb.nszjky.cn

[A19] 交换两个变量
来源：http://pv.hnjuh.cn

Py:   a, b = b, a
来源：http://bb.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://co.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://eh.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://iz.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://ch.521024.cn

Go:   a, b = b, a
来源：http://pq.521024.cn

Ruby: a, b = b, a
来源：http://fn.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://ef.asd995.cn

[A20] 读取标准输入
来源：http://jf.szxytkj.cn

Py:   name = input("请输入：")
来源：http://it.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qc.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jy.asd995.cn

TS:   // Node.js：readline 模块
来源：http://dx.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://tp.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yo.gzmigu.cn

Ruby: gets.chomp
来源：http://gc.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://fv.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://rz.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://uj.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ro.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://sd.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://wu.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://om.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kj.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://fm.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://el.hahajie.cn

[A22] 获取字符串长度
来源：http://xv.9csxet.cn

Py:   len(s)
来源：http://au.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://am.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ma.hnjuh.cn

TS:   s.length
来源：http://jh.nszjky.cn

Java: s.length()
来源：http://vl.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pz.gzmigu.cn

Ruby: s.length
来源：http://un.wgjwhj.cn

C#:   s.Length
来源：http://gq.bjjhwx.cn

[A23] 大小写转换
来源：http://we.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nx.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ay.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ic.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fm.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yz.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nm.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ku.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ih.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ql.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yo.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zl.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uu.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zq.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nj.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hw.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aq.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rw.hnjuh.cn

[A25] 字符串比较
来源：http://ym.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://kk.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qd.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mj.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hd.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fa.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jk.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fx.lnxyls.cn

[A26] 类型转换总览
来源：http://ka.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fb.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xd.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://md.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ml.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://az.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dn.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aj.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://en.521024.cn

================================================================================
来源：http://th.nicolike.cn

B. 流程控制
来源：http://sa.shxzukj.cn

================================================================================
来源：http://kf.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://jh.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fh.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qh.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wp.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gf.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mu.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jk.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rs.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ti.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://yi.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dt.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rm.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qk.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yi.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://od.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.9csxet.cn

[B03] switch / match / case
来源：http://fz.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tq.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://it.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fb.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ek.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ad.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oy.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zh.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mm.521024.cn

[B04] for 计数循环
来源：http://dq.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://ao.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ph.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bl.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gf.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xb.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://nd.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fc.colortex.cn

[B05] 遍历数组 / 列表
来源：http://di.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://ai.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bp.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ya.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rp.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iu.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qt.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://lr.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hd.colortex.cn

[B06] 遍历字典 / 对象
来源：http://eb.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lc.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ex.yuexingan06.cn


<!-- 参考信息 -->