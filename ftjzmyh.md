代发 wailian999

--------------------------------------------------------------------------------
来源：http://eu.hnjuh.cn

目  录
来源：http://nw.hahajie.cn

--------------------------------------------------------------------------------
来源：http://yk.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ja.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tz.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wy.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wa.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bi.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tw.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lj.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gb.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ss.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ya.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zp.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jx.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eo.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oj.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bq.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sj.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ev.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zr.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sk.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sb.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hi.9csxet.cn

================================================================================
来源：http://tv.panjiajie.cn

A. 基础语法与类型
来源：http://ro.bjjhwx.cn

================================================================================
来源：http://oa.bookmarksfly.cn

[A01] Hello World
来源：http://jv.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://bm.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ww.asd995.cn

JS:   console.log("Hello, World!");
来源：http://cg.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ux.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://gr.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://gk.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://bi.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cw.gzmigu.cn

[A02] 变量声明与赋值
来源：http://gu.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dy.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bt.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fi.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wz.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://wj.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://uf.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://fu.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rf.lnxyls.cn

[A03] 常量定义
来源：http://nc.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xe.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://xg.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ae.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://cq.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://if.gzmigu.cn

Go:   const PI = 3.14159
来源：http://vl.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://xx.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://ri.szsharing.cn

[A04] 判断变量类型
来源：http://zs.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jx.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lm.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pr.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://bp.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kz.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ds.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lq.521024.cn

C#:   x.GetType().Name; x is int
来源：http://yl.newstarts.cn

[A05] 整数除法与取模
来源：http://my.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://en.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://od.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://er.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://in.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://qe.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://xv.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://jv.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://uk.bookmarksfly.cn

[A06] 字符串转数字
来源：http://ql.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://yl.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bz.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ci.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ox.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://na.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uf.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cx.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pg.hnjuh.cn

[A07] 数字转字符串
来源：http://gl.muxihuayi.cn

Py:   str(42)
来源：http://nh.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://hy.newstarts.cn

JS:   String(42); (42).toString()
来源：http://ib.bjjhwx.cn

TS:   String(42)
来源：http://vr.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jb.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://ae.shxzskj.cn

Ruby: 42.to_s
来源：http://fx.panjiajie.cn

C#:   42.ToString()
来源：http://jx.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://fv.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dn.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://at.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jd.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dm.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dq.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pd.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hc.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://au.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://ib.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ak.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ym.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bx.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ir.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mz.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vj.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ug.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eo.colortex.cn

[A10] 生成随机数
来源：http://zi.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://zp.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ue.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dk.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lk.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://bv.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hp.szsharing.cn

Ruby: rand(1..100)
来源：http://hf.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://rj.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://eq.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://ur.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mp.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gx.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uf.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://wl.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ws.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rw.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://od.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://ab.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ca.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tw.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://ns.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://qv.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://ud.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://js.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://sc.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://jn.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ao.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://hu.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://qo.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://ev.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://vl.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://vq.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://kp.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://xx.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://zs.shxzskj.cn

[A14] 注释写法
来源：http://ve.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ib.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ff.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://oh.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://ub.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://of.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://qh.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rx.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://hd.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://il.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://cz.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://fq.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://to.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://um.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://of.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://bj.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://tn.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://lr.huanxung.cn

[A16] 真假值判断规则
来源：http://qj.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xi.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zt.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lt.wgjwhj.cn

TS:   if (!x) {}
来源：http://ba.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://et.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://de.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vj.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pb.nicolike.cn

[A17] 位运算
来源：http://ip.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kj.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tb.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://re.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kz.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ve.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cp.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://am.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://zr.521024.cn

Py:   ord("A"); chr(65)
来源：http://rr.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://ca.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ue.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nc.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://oj.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qb.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://ed.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://ff.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://gy.lnxyls.cn

Py:   a, b = b, a
来源：http://hk.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bn.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://qy.colortex.cn

TS:   [a, b] = [b, a];
来源：http://dy.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://bi.chemitech.net.cn

Go:   a, b = b, a
来源：http://xz.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://vx.521024.cn

C#:   (a, b) = (b, a);
来源：http://ee.szxytkj.cn

[A20] 读取标准输入
来源：http://nk.huanxung.cn

Py:   name = input("请输入：")
来源：http://et.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ai.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mm.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://hh.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://av.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xo.asd995.cn

Ruby: gets.chomp
来源：http://yl.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://rj.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://qu.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://gd.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xt.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://dj.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://tj.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://dj.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uq.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://yk.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://xj.shxzskj.cn

[A22] 获取字符串长度
来源：http://ko.bookmarksfly.cn

Py:   len(s)
来源：http://gm.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jm.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://af.huixiangedu.cn

TS:   s.length
来源：http://az.jianghongdianzi.cn

Java: s.length()
来源：http://qu.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eu.yuexingan06.cn

Ruby: s.length
来源：http://nf.colortex.cn

C#:   s.Length
来源：http://wl.nszjky.cn

[A23] 大小写转换
来源：http://xa.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://on.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ex.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yk.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hd.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://um.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ob.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ls.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qx.gzmigu.cn

[A24] 去除首尾空白
来源：http://gb.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://af.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xq.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xu.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jv.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ot.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://xb.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gl.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zq.muxihuayi.cn

[A25] 字符串比较
来源：http://oo.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://tx.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ae.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gl.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jc.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vf.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sg.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bc.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pi.yuexingan06.cn

[A26] 类型转换总览
来源：http://oo.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zh.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sf.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ty.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://dd.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cj.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hp.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ln.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dh.hnjuh.cn

================================================================================
来源：http://nh.huanxung.cn

B. 流程控制
来源：http://xe.newstarts.cn

================================================================================
来源：http://eq.szsharing.cn

[B01] 条件判断 if / else
来源：http://ma.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bp.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lj.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ng.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://to.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ih.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tz.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hy.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wv.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://kw.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://du.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ba.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xl.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sk.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fs.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.jianghongdianzi.cn

[B03] switch / match / case
来源：http://qb.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ek.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zo.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fj.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ee.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jh.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vn.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pj.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qh.huanxung.cn

[B04] for 计数循环
来源：http://kd.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://ra.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uo.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gk.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://py.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nj.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ww.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://cg.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://to.huixiangedu.cn


<!-- 参考信息 -->