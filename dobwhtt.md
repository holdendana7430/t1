代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://im.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ck.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sa.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cj.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qr.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dn.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ki.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ri.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yu.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zn.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yj.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dq.asd995.cn

================================================================================
来源：http://lj.huixiangedu.cn

A. 基础语法与类型
来源：http://bl.szxytkj.cn

================================================================================
来源：http://km.yuexingan06.cn

[A01] Hello World
来源：http://ho.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://pm.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://mg.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://pf.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ny.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://ao.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://mq.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://zt.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eq.panjiajie.cn

[A02] 变量声明与赋值
来源：http://po.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rf.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fw.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wz.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pm.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://qb.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://sk.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://tt.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bg.wgjwhj.cn

[A03] 常量定义
来源：http://jd.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vo.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://jf.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://nn.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://oo.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://ai.gzmigu.cn

Go:   const PI = 3.14159
来源：http://xz.521024.cn

Ruby: PI = 3.14159
来源：http://be.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://hq.shtwfgs.cn

[A04] 判断变量类型
来源：http://pi.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qh.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://on.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ns.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://je.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xq.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ia.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gb.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://yl.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://nd.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rj.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ml.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qb.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mm.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://xm.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://lj.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://jo.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://se.muxihuayi.cn

[A06] 字符串转数字
来源：http://sy.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://fx.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yt.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tm.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ii.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mq.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xn.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cq.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://io.bjjhwx.cn

[A07] 数字转字符串
来源：http://yh.9csxet.cn

Py:   str(42)
来源：http://us.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://uv.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://dy.huixinmuqiang.cn

TS:   String(42)
来源：http://nu.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dg.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://qp.bookmarksfly.cn

Ruby: 42.to_s
来源：http://gv.hnjuh.cn

C#:   42.ToString()
来源：http://hp.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ym.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tx.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xm.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qs.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sq.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uh.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kq.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jk.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://lf.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bp.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dn.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jd.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vz.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sw.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lv.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://we.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jc.shxzskj.cn

[A10] 生成随机数
来源：http://ia.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://gz.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://ok.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jr.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oj.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://oj.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gh.hnjuh.cn

Ruby: rand(1..100)
来源：http://oe.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://rb.newstarts.cn

[A11] 条件表达式（三元）
来源：http://nm.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ck.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://og.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dl.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cr.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://jh.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zm.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sq.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lu.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://jp.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lb.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yw.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://dm.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ro.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://yh.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://de.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://xl.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://ks.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://az.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://fb.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://lt.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://ba.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://tl.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://yg.newstarts.cn

Go:   "第一行\n第二行"
来源：http://ac.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://zx.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ni.haigaiapp.cn

[A14] 注释写法
来源：http://ut.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mv.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ty.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://km.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://em.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ff.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://xa.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ha.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://hr.lnxyls.cn

[A15] 空值判断与默认值
来源：http://gn.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://xo.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://ek.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://vd.521024.cn

TS:   const value = data ?? "默认值";
来源：http://aw.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dl.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://dm.newstarts.cn

Ruby: value = data || "默认值"
来源：http://vg.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://ux.nicolike.cn

[A16] 真假值判断规则
来源：http://vt.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tt.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ro.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://do.szxytkj.cn

TS:   if (!x) {}
来源：http://pv.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cp.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yd.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cu.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kz.nicolike.cn

[A17] 位运算
来源：http://qk.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rt.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dl.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ka.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lo.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hs.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pw.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rg.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://qf.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://wf.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://pc.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fu.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cj.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ko.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lg.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://ft.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://oc.shxzukj.cn

[A19] 交换两个变量
来源：http://ya.hahajie.cn

Py:   a, b = b, a
来源：http://wm.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://om.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://af.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://rz.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://cb.szxytkj.cn

Go:   a, b = b, a
来源：http://kk.bjjhwx.cn

Ruby: a, b = b, a
来源：http://ew.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://zf.jctech888.com.cn

[A20] 读取标准输入
来源：http://du.gzmigu.cn

Py:   name = input("请输入：")
来源：http://lk.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fk.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yy.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://yt.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://tq.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ym.lnxyls.cn

Ruby: gets.chomp
来源：http://ht.lnxyls.cn

C#:   Console.ReadLine();
来源：http://nj.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://lw.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://to.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hl.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://dz.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://go.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://kr.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vl.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://yt.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://yw.szsharing.cn

[A22] 获取字符串长度
来源：http://vk.hnjuh.cn

Py:   len(s)
来源：http://ep.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jc.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cn.panjiajie.cn

TS:   s.length
来源：http://sf.bookmarksfly.cn

Java: s.length()
来源：http://wd.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pr.jctech888.com.cn

Ruby: s.length
来源：http://iv.huixiangedu.cn

C#:   s.Length
来源：http://jl.chemitech.net.cn

[A23] 大小写转换
来源：http://vp.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wu.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uh.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vu.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ix.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zo.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jw.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rg.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ge.shtwfgs.cn

[A24] 去除首尾空白
来源：http://bu.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vr.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pl.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kx.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kd.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ck.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vu.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ay.huixinmuqiang.cn

[A25] 字符串比较
来源：http://vf.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ar.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://va.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kj.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zj.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zy.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://al.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sq.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yc.huanxung.cn

[A26] 类型转换总览
来源：http://tn.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bl.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bd.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hb.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://yx.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ya.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zo.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oa.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://us.huixiangedu.cn

B. 流程控制
来源：http://ds.chemitech.net.cn

================================================================================
来源：http://qy.szxytkj.cn

[B01] 条件判断 if / else
来源：http://vy.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://io.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wg.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hj.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uq.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bc.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wv.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://ez.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oi.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ad.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ho.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lp.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mr.shtwfgs.cn

[B03] switch / match / case
来源：http://gr.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hh.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yn.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eu.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bm.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hy.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://an.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wh.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oo.bjjhwx.cn

[B04] for 计数循环
来源：http://lp.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://vi.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://es.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ws.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vd.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ez.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qm.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://ag.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://du.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ef.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://vq.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bb.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lp.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yv.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bx.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kd.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://xx.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xm.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://ap.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yc.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ml.shtwfgs.cn


<!-- 参考信息 -->