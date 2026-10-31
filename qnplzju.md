代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://di.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bc.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aq.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vf.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tl.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xh.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kg.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sq.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gf.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ro.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lu.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fd.nicolike.cn

================================================================================
来源：http://op.huixinmuqiang.cn

A. 基础语法与类型
来源：http://wv.gzmigu.cn

================================================================================
来源：http://rv.nszjky.cn

[A01] Hello World
来源：http://kz.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://iq.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://vf.521024.cn

JS:   console.log("Hello, World!");
来源：http://hx.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ce.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://va.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://iy.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://fa.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gq.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://pf.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ri.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xx.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gy.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hy.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://yv.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://mw.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://fl.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fp.nszjky.cn

[A03] 常量定义
来源：http://tz.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mz.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://wo.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://ih.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://ow.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://sh.hnjuh.cn

Go:   const PI = 3.14159
来源：http://jk.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://sx.521024.cn

C#:   const double PI = 3.14159;
来源：http://oj.gzmigu.cn

[A04] 判断变量类型
来源：http://ag.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qk.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jc.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ee.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://pa.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wb.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mj.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://el.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://oo.shtwfgs.cn

[A05] 整数除法与取模
来源：http://cn.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uh.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lp.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ke.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iq.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://zk.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://un.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://en.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://np.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://eo.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://pj.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xt.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zu.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pd.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sj.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ug.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xv.szsharing.cn

[A07] 数字转字符串
来源：http://ww.hahajie.cn

Py:   str(42)
来源：http://ce.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://cd.szsharing.cn

JS:   String(42); (42).toString()
来源：http://no.shxzukj.cn

TS:   String(42)
来源：http://xi.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fm.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://xx.huixiangedu.cn

Ruby: 42.to_s
来源：http://gz.jctech888.com.cn

C#:   42.ToString()
来源：http://wh.hahajie.cn

[A08] 取整与四舍五入
来源：http://gx.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mr.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cd.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aq.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wf.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ve.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bi.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jq.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sm.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://wa.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qn.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ak.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jq.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xg.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xp.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vn.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rq.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cc.shxzskj.cn

[A10] 生成随机数
来源：http://du.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://wd.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://ek.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lr.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://je.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://mr.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rx.huixiangedu.cn

Ruby: rand(1..100)
来源：http://wb.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://dh.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://xa.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://so.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rr.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mm.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yp.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://vl.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sm.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kx.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sj.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://iz.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ho.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gt.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://ra.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://gd.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://yf.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sh.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://hn.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://oe.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://py.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://qu.521024.cn

PHP:  "第一行\n第二行"
来源：http://hr.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://cc.nszjky.cn

TS:   "第一行\n第二行"
来源：http://hr.hahajie.cn

Java: "第一行\n第二行"
来源：http://dj.huanxung.cn

Go:   "第一行\n第二行"
来源：http://pw.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://rv.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://om.shxzskj.cn

[A14] 注释写法
来源：http://fy.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gr.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cr.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://ij.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://kb.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ot.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://cp.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ep.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ab.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://rd.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://nl.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://gh.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://pd.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://uo.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qi.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://og.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://yz.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://tc.9csxet.cn

[A16] 真假值判断规则
来源：http://js.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lz.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wf.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://df.nicolike.cn

TS:   if (!x) {}
来源：http://ri.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://my.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ff.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tk.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zb.szxytkj.cn

[A17] 位运算
来源：http://ka.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mz.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lo.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pu.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fj.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://vm.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://tm.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://ve.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rp.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jg.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://zz.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cl.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://fm.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://up.colortex.cn

[A19] 交换两个变量
来源：http://ij.gzmigu.cn

Py:   a, b = b, a
来源：http://mr.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xw.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://kw.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://hk.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://gk.szsharing.cn

Go:   a, b = b, a
来源：http://ez.9csxet.cn

Ruby: a, b = b, a
来源：http://sw.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://ur.haigaiapp.cn

[A20] 读取标准输入
来源：http://cm.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://ou.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nt.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jf.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://cs.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://yt.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mt.newstarts.cn

Ruby: gets.chomp
来源：http://kd.gzmigu.cn

C#:   Console.ReadLine();
来源：http://dv.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://uk.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://df.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ih.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://op.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://zk.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://kr.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hb.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://vl.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://ar.panjiajie.cn

[A22] 获取字符串长度
来源：http://yl.colortex.cn

Py:   len(s)
来源：http://sz.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fx.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://me.jianghongdianzi.cn

TS:   s.length
来源：http://vs.szsharing.cn

Java: s.length()
来源：http://gv.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nc.huanxung.cn

Ruby: s.length
来源：http://qg.bjjhwx.cn

C#:   s.Length
来源：http://jf.huixinmuqiang.cn

[A23] 大小写转换
来源：http://cm.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qu.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ce.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vb.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pk.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bg.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sq.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kw.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.asd995.cn

[A24] 去除首尾空白
来源：http://hy.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hx.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kl.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vb.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fo.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uh.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://sf.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ov.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nh.shtwfgs.cn

[A25] 字符串比较
来源：http://eo.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://dz.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fh.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ya.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ho.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jn.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wt.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cm.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nu.szxytkj.cn

[A26] 类型转换总览
来源：http://yu.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wf.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gg.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ms.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://iz.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ox.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ux.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ag.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://ol.panjiajie.cn

B. 流程控制
来源：http://vy.bookmarksfly.cn

================================================================================
来源：http://lw.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://ws.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jw.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zt.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kl.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jp.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wz.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rm.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nb.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://we.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rf.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wn.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ke.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://up.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xd.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bs.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://no.nszjky.cn

[B03] switch / match / case
来源：http://df.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jg.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nq.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xj.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qv.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bs.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ju.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://en.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oo.nszjky.cn

[B04] for 计数循环
来源：http://en.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://of.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ku.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sn.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://be.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gz.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://af.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://ll.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wd.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://qc.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://fr.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ty.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xt.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ur.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oi.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ti.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://we.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rt.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://yl.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://at.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rb.nicolike.cn


<!-- 参考信息 -->