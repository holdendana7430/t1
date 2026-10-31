代发 wailian999

--------------------------------------------------------------------------------
来源：http://ov.huanxung.cn

目  录
来源：http://oz.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ss.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uy.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nk.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fu.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zx.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://au.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ss.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://od.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ux.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wi.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wa.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ls.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wr.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kz.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mz.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xh.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iw.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pf.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zu.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fz.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://br.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qw.chemitech.net.cn

================================================================================
来源：http://pl.colortex.cn

A. 基础语法与类型
来源：http://cl.bookmarksfly.cn

================================================================================
来源：http://qd.colortex.cn

[A01] Hello World
来源：http://ru.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://do.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://ia.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://gy.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xl.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://nr.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://gb.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://ye.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gk.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://qg.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://so.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ro.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kb.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nd.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://rt.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://bh.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://qp.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fs.szsharing.cn

[A03] 常量定义
来源：http://bu.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nc.lnxyls.cn

PHP:  const PI = 3.14159;
来源：http://zg.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://zn.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://cr.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://uk.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://gg.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://nr.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://wo.shxzukj.cn

[A04] 判断变量类型
来源：http://hy.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yh.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ep.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ds.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://pk.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lr.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hf.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hp.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://sl.colortex.cn

[A05] 整数除法与取模
来源：http://le.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nu.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hf.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ke.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://km.521024.cn

Java: 7 / 2; 7 % 2
来源：http://xy.521024.cn

Go:   7 / 2; 7 % 2
来源：http://tq.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://rb.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://fn.nicolike.cn

[A06] 字符串转数字
来源：http://xp.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://kr.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://za.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oa.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ft.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wl.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hn.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zx.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xg.lnxyls.cn

[A07] 数字转字符串
来源：http://cm.9csxet.cn

Py:   str(42)
来源：http://yj.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://dy.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://bw.521024.cn

TS:   String(42)
来源：http://ub.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vu.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://ht.9csxet.cn

Ruby: 42.to_s
来源：http://nb.yuexingan06.cn

C#:   42.ToString()
来源：http://hk.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://bz.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ls.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ee.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://se.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://er.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ua.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wn.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qd.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://de.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://zm.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sg.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dk.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eq.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vp.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pe.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bz.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kt.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vq.szxytkj.cn

[A10] 生成随机数
来源：http://jq.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://aw.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://ci.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ju.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dq.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://bk.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://be.muxihuayi.cn

Ruby: rand(1..100)
来源：http://uz.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://ny.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ai.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://wx.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nc.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ew.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pd.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://nk.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gp.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ib.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bk.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://tl.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xg.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ca.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://nw.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://eq.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://mx.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nt.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://za.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://gl.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gv.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://iz.521024.cn

PHP:  "第一行\n第二行"
来源：http://pz.newstarts.cn

JS:   "第一行\n第二行"
来源：http://rw.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://dw.huanxung.cn

Java: "第一行\n第二行"
来源：http://tx.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://zw.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://zu.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://hz.shxzskj.cn

[A14] 注释写法
来源：http://yk.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gd.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jn.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://yj.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://is.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xa.521024.cn

Go:   // 单行；/* 多行 */
来源：http://nh.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ku.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://yb.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ux.9csxet.cn

Py:   value = data or "默认值"
来源：http://bx.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://qp.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://os.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://ql.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ev.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zv.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://nr.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://ev.wgjwhj.cn

[A16] 真假值判断规则
来源：http://ko.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uz.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vn.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://re.shxzskj.cn

TS:   if (!x) {}
来源：http://pn.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lu.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ca.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ij.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pq.haigaiapp.cn

[A17] 位运算
来源：http://ae.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ny.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ev.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://df.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zu.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iu.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ou.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gf.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://me.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://ty.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://bi.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hv.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zo.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://fm.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bb.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://ak.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://mq.asd995.cn

[A19] 交换两个变量
来源：http://pi.huixiangedu.cn

Py:   a, b = b, a
来源：http://wv.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gp.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://bs.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://oi.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://zq.bookmarksfly.cn

Go:   a, b = b, a
来源：http://dh.shxzukj.cn

Ruby: a, b = b, a
来源：http://nc.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://yg.huixiangedu.cn

[A20] 读取标准输入
来源：http://vs.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ab.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://og.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dk.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://yz.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://oe.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sf.newstarts.cn

Ruby: gets.chomp
来源：http://ur.newstarts.cn

C#:   Console.ReadLine();
来源：http://ik.newstarts.cn

[A21] 保留指定小数位输出
来源：http://mw.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://qi.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yl.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://qe.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://yc.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://bz.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vr.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://or.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://tg.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://xa.chemitech.net.cn

Py:   len(s)
来源：http://wn.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jw.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://od.jctech888.com.cn

TS:   s.length
来源：http://cj.gzmigu.cn

Java: s.length()
来源：http://fo.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sm.panjiajie.cn

Ruby: s.length
来源：http://li.yuexingan06.cn

C#:   s.Length
来源：http://or.shxzskj.cn

[A23] 大小写转换
来源：http://tk.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mu.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wd.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jn.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cn.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bd.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ow.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ah.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ng.colortex.cn

[A24] 去除首尾空白
来源：http://dg.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://um.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bc.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kn.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cj.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vu.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://tx.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jo.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oe.nszjky.cn

[A25] 字符串比较
来源：http://xr.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://xn.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jj.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eu.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ym.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wr.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ap.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zc.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ra.shxzskj.cn

[A26] 类型转换总览
来源：http://wj.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ck.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iu.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ry.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://bg.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bi.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sn.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wg.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nk.nicolike.cn

================================================================================
来源：http://pi.huixiangedu.cn

B. 流程控制
来源：http://at.shxzskj.cn

================================================================================
来源：http://la.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://gu.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qr.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kb.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://du.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://um.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://im.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qz.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ol.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mj.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ij.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rs.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xn.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://th.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wx.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mj.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bt.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://no.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.bjjhwx.cn

[B03] switch / match / case
来源：http://ws.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bd.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ii.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vo.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ab.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zf.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yl.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xd.9csxet.cn

[B04] for 计数循环
来源：http://pt.colortex.cn

Py:   for i in range(10): print(i)
来源：http://ku.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yj.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qx.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nz.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jt.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://at.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ef.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wb.hahajie.cn


<!-- 参考信息 -->