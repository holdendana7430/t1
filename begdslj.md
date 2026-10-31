代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ix.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xk.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ew.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vl.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://op.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bq.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fz.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jt.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hs.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uj.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qg.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zy.szsharing.cn

================================================================================
来源：http://cb.lnxyls.cn

A. 基础语法与类型
来源：http://bw.yuexingan06.cn

================================================================================
来源：http://ij.wgjwhj.cn

[A01] Hello World
来源：http://lf.hnjuh.cn

Py:   print("Hello, World!")
来源：http://et.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://di.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://es.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vu.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://bt.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://kv.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://xy.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dr.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://lf.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ts.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jv.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zl.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bb.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://yf.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://vq.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://kg.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xu.haigaiapp.cn

[A03] 常量定义
来源：http://ko.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pv.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://jk.huanxung.cn

JS:   const PI = 3.14159;
来源：http://av.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://yu.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://co.hnjuh.cn

Go:   const PI = 3.14159
来源：http://ts.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://ad.colortex.cn

C#:   const double PI = 3.14159;
来源：http://mr.chemitech.net.cn

[A04] 判断变量类型
来源：http://mm.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ep.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ci.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gr.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://dt.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tu.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gt.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ia.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://cc.shxzskj.cn

[A05] 整数除法与取模
来源：http://ar.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://od.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qx.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ni.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jt.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://lj.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://rx.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://ql.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://mv.shtwfgs.cn

[A06] 字符串转数字
来源：http://hm.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://ti.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nl.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fh.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pg.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rk.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jt.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://in.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fn.gzmigu.cn

[A07] 数字转字符串
来源：http://ue.jianghongdianzi.cn

Py:   str(42)
来源：http://aj.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://oi.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://id.hnjuh.cn

TS:   String(42)
来源：http://ep.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cr.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://gq.shtwfgs.cn

Ruby: 42.to_s
来源：http://sm.hnjuh.cn

C#:   42.ToString()
来源：http://wc.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://jd.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ok.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wz.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wg.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fg.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jc.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rp.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lk.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://em.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://kp.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nd.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ru.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pv.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qf.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fm.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zf.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://do.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hq.newstarts.cn

[A10] 生成随机数
来源：http://ln.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://wf.9csxet.cn

PHP:  random_int(1, 100);
来源：http://ax.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kx.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ac.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://xr.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cc.hnjuh.cn

Ruby: rand(1..100)
来源：http://rv.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://sv.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://jo.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://zi.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://is.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sv.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qs.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://an.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ob.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fi.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ac.521024.cn

[A12] 字符串插值 / 格式化
来源：http://hy.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vd.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gm.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://cf.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://zb.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ef.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rg.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://pl.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://zo.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wi.szsharing.cn

Py:   "第一行\n第二行"
来源：http://iv.asd995.cn

PHP:  "第一行\n第二行"
来源：http://nz.asd995.cn

JS:   "第一行\n第二行"
来源：http://dz.szsharing.cn

TS:   "第一行\n第二行"
来源：http://df.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://yl.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://aj.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://dm.colortex.cn

C#:   "第一行\n第二行"
来源：http://ms.szxytkj.cn

[A14] 注释写法
来源：http://yc.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oo.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fz.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://ud.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://jg.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://at.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://qc.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ll.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://sx.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://de.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://qp.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://nw.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://bm.521024.cn

TS:   const value = data ?? "默认值";
来源：http://mx.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uk.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://ni.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://ta.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://te.lnxyls.cn

[A16] 真假值判断规则
来源：http://mq.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fw.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dn.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kq.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://zm.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ap.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rc.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bd.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lw.newstarts.cn

[A17] 位运算
来源：http://op.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sa.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iy.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ok.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fe.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rp.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lr.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://td.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://un.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://ea.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://sv.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dx.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qr.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://xt.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zj.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://lf.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://ij.nicolike.cn

[A19] 交换两个变量
来源：http://xu.panjiajie.cn

Py:   a, b = b, a
来源：http://rp.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bu.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://nq.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://ea.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://wk.huixiangedu.cn

Go:   a, b = b, a
来源：http://rj.panjiajie.cn

Ruby: a, b = b, a
来源：http://nw.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://zs.haigaiapp.cn

[A20] 读取标准输入
来源：http://ns.panjiajie.cn

Py:   name = input("请输入：")
来源：http://md.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sq.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hd.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://dj.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://ru.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ah.shtwfgs.cn

Ruby: gets.chomp
来源：http://ci.asd995.cn

C#:   Console.ReadLine();
来源：http://ww.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://st.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://an.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vn.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://zi.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://fu.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://oz.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oq.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://xu.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://ds.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://wl.colortex.cn

Py:   len(s)
来源：http://fc.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qt.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tj.bookmarksfly.cn

TS:   s.length
来源：http://ic.shxzukj.cn

Java: s.length()
来源：http://gm.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://su.szsharing.cn

Ruby: s.length
来源：http://gs.szsharing.cn

C#:   s.Length
来源：http://ma.bookmarksfly.cn

[A23] 大小写转换
来源：http://uw.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rz.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wv.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sr.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qb.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yr.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hs.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ov.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wa.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://qp.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bt.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pm.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://we.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gz.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rt.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://cn.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gg.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ey.bjjhwx.cn

[A25] 字符串比较
来源：http://tn.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://ro.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cu.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ej.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lz.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://os.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lp.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dc.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mo.muxihuayi.cn

[A26] 类型转换总览
来源：http://vo.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oq.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fg.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nt.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ub.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xo.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bo.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jp.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cb.shxzukj.cn

================================================================================
来源：http://ml.panjiajie.cn

B. 流程控制
来源：http://ko.asd995.cn

================================================================================
来源：http://fr.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://wq.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pz.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ao.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wd.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dl.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://un.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mc.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ib.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://dq.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kl.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ma.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fw.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zd.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qk.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vi.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.wgjwhj.cn

[B03] switch / match / case
来源：http://zq.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xi.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zg.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xr.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zp.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ig.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dj.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tc.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uw.lnxyls.cn

[B04] for 计数循环
来源：http://pq.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://ha.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vl.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dl.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zi.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zy.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ue.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://ht.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rm.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://hs.521024.cn

Py:   for item in arr: print(item)
来源：http://jk.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qq.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://az.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vt.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mf.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jl.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://gl.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fn.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://ya.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xa.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.chemitech.net.cn


<!-- 参考信息 -->