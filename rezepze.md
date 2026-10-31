代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wv.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uu.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bv.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zr.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://el.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jv.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iw.wgjwhj.cn

================================================================================
来源：http://ux.szsharing.cn

A. 基础语法与类型
来源：http://on.colortex.cn

================================================================================
来源：http://te.bookmarksfly.cn

[A01] Hello World
来源：http://qn.asd995.cn

Py:   print("Hello, World!")
来源：http://zd.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://lk.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://ne.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rb.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://xk.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://tx.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://xy.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sq.huanxung.cn

[A02] 变量声明与赋值
来源：http://my.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rv.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rc.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://em.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ch.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://tr.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://iz.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://tq.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qa.yuntaijiaju.cn

[A03] 常量定义
来源：http://up.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rl.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://mg.nicolike.cn

JS:   const PI = 3.14159;
来源：http://yw.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://vx.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://nm.gzmigu.cn

Go:   const PI = 3.14159
来源：http://iu.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://xe.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://lt.shxzskj.cn

[A04] 判断变量类型
来源：http://ab.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ht.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xk.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ay.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://eo.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ry.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lc.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gp.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://us.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://wn.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cl.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vm.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ev.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bx.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://lf.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://fs.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://cc.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://bk.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://pj.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://xj.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dz.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pt.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hz.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://is.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ak.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ac.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gt.gzmigu.cn

[A07] 数字转字符串
来源：http://sm.panjiajie.cn

Py:   str(42)
来源：http://tj.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://vb.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://iy.huanxung.cn

TS:   String(42)
来源：http://qx.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xj.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://sb.szxytkj.cn

Ruby: 42.to_s
来源：http://xi.gzmigu.cn

C#:   42.ToString()
来源：http://ay.shxzukj.cn

[A08] 取整与四舍五入
来源：http://ka.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://an.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ti.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jn.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nc.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ce.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yu.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ic.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pb.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://wv.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bv.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zl.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vr.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cr.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ex.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zn.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lt.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uj.521024.cn

[A10] 生成随机数
来源：http://bv.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://lt.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://do.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gp.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xq.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://rm.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cn.wgjwhj.cn

Ruby: rand(1..100)
来源：http://yy.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://xc.szsharing.cn

[A11] 条件表达式（三元）
来源：http://hc.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://aw.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bn.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yv.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ax.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://ft.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ml.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://op.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pt.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://gi.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kb.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xt.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://be.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://dj.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://qv.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://df.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://iq.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://wc.521024.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iq.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://yl.colortex.cn

PHP:  "第一行\n第二行"
来源：http://hy.hahajie.cn

JS:   "第一行\n第二行"
来源：http://nt.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://md.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://go.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://ot.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://vo.nszjky.cn

C#:   "第一行\n第二行"
来源：http://ia.9csxet.cn

[A14] 注释写法
来源：http://ba.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pr.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://na.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://wv.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://uq.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mc.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://ih.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://po.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://kt.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://fa.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://hr.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://nf.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://ch.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://uu.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hu.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://vs.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://rm.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://zh.nszjky.cn

[A16] 真假值判断规则
来源：http://ji.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sw.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vt.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cx.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://av.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://na.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iq.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ga.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bq.shxzukj.cn

[A17] 位运算
来源：http://cz.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ix.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://we.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://no.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oa.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qb.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rn.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xf.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://vu.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://jn.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://fh.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aa.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jv.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://jw.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gh.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://mu.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://zr.panjiajie.cn

[A19] 交换两个变量
来源：http://ub.gzmigu.cn

Py:   a, b = b, a
来源：http://vh.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qx.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://rm.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://bx.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://nd.shxzskj.cn

Go:   a, b = b, a
来源：http://lp.huixiangedu.cn

Ruby: a, b = b, a
来源：http://cj.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://gb.colortex.cn

[A20] 读取标准输入
来源：http://uj.hnjuh.cn

Py:   name = input("请输入：")
来源：http://gt.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xh.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://rn.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://ot.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://le.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://xr.panjiajie.cn

C#:   Console.ReadLine();
来源：http://ak.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://bf.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://po.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mr.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://bs.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://rv.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://gg.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sj.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ta.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://xk.521024.cn

[A22] 获取字符串长度
来源：http://nk.hahajie.cn

Py:   len(s)
来源：http://fe.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jr.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xf.hnjuh.cn

TS:   s.length
来源：http://te.nicolike.cn

Java: s.length()
来源：http://jf.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ll.shtwfgs.cn

Ruby: s.length
来源：http://tt.shtwfgs.cn

C#:   s.Length
来源：http://gs.colortex.cn

[A23] 大小写转换
来源：http://rc.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zd.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yn.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mo.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sr.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ff.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yg.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xg.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jj.hahajie.cn

[A24] 去除首尾空白
来源：http://hg.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uu.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uc.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uu.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ld.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uq.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://ke.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ov.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rh.colortex.cn

[A25] 字符串比较
来源：http://ta.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://jb.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ne.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://im.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gy.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sj.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qc.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cn.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wm.shtwfgs.cn

[A26] 类型转换总览
来源：http://mb.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mj.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://co.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ux.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://yl.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vm.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://un.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rk.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lv.muxihuayi.cn

================================================================================
来源：http://or.colortex.cn

B. 流程控制
来源：http://kr.gzmigu.cn

================================================================================
来源：http://uw.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://vi.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pi.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ks.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tz.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nd.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://id.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hm.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://st.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sa.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://yx.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rs.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dx.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vi.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rj.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gz.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.gzmigu.cn

[B03] switch / match / case
来源：http://nx.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://el.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gj.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kc.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ac.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yc.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ci.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zt.bookmarksfly.cn

[B04] for 计数循环
来源：http://kq.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ai.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ei.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yz.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qm.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://kq.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://md.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://qf.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ni.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zp.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kw.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://av.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://si.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oj.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://dh.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sp.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://pw.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bi.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gp.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ny.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cx.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fo.chemitech.net.cn


<!-- 参考信息 -->