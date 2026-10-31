代发 wailian999

--------------------------------------------------------------------------------
来源：http://se.gzmigu.cn

目  录
来源：http://fn.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://cr.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kt.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nj.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uq.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pt.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qc.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xj.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vi.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ry.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xg.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fv.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zy.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://my.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yb.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ra.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vz.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mt.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ui.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://is.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://en.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kl.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ex.colortex.cn

================================================================================
来源：http://ic.521024.cn

A. 基础语法与类型
来源：http://qh.bjjhwx.cn

================================================================================
来源：http://qp.asd995.cn

[A01] Hello World
来源：http://qi.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://eg.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://wn.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://qh.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vj.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://xf.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://aq.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://tc.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rv.asd995.cn

[A02] 变量声明与赋值
来源：http://jq.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iu.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ud.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kq.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://md.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ak.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://ww.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://cv.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://if.jianghongdianzi.cn

[A03] 常量定义
来源：http://je.huanxung.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zm.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://wu.asd995.cn

JS:   const PI = 3.14159;
来源：http://cf.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://ei.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://dv.asd995.cn

Go:   const PI = 3.14159
来源：http://xr.szxytkj.cn

Ruby: PI = 3.14159
来源：http://ih.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://np.bjjhwx.cn

[A04] 判断变量类型
来源：http://ju.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yd.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gb.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fd.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://yz.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kw.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uq.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gu.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://bc.gzmigu.cn

[A05] 整数除法与取模
来源：http://bs.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zh.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jv.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xq.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wt.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://fn.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://ev.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://ee.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://uk.wgjwhj.cn

[A06] 字符串转数字
来源：http://wm.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ll.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zl.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yn.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ee.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wb.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ek.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ye.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wo.wgjwhj.cn

[A07] 数字转字符串
来源：http://vt.newstarts.cn

Py:   str(42)
来源：http://ld.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://xr.szsharing.cn

JS:   String(42); (42).toString()
来源：http://sf.bookmarksfly.cn

TS:   String(42)
来源：http://oi.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nf.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://ti.9csxet.cn

Ruby: 42.to_s
来源：http://ri.szxytkj.cn

C#:   42.ToString()
来源：http://ue.asd995.cn

[A08] 取整与四舍五入
来源：http://wo.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://se.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tj.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://io.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jd.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uv.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vb.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fh.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fa.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://pe.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://db.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zx.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bf.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://en.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pp.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zr.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dg.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aj.szxytkj.cn

[A10] 生成随机数
来源：http://la.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://gy.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://qe.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kc.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gt.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://xl.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oe.chemitech.net.cn

Ruby: rand(1..100)
来源：http://wb.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://qk.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://ap.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://tw.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qg.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bn.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pr.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://fs.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ba.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vk.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vb.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://fr.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qq.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bs.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://ct.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://od.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://wk.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vr.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ji.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://ty.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://md.nicolike.cn

Py:   "第一行\n第二行"
来源：http://db.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://ad.hahajie.cn

JS:   "第一行\n第二行"
来源：http://sw.szsharing.cn

TS:   "第一行\n第二行"
来源：http://qc.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://dj.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://wo.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://gb.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://xr.huanxung.cn

[A14] 注释写法
来源：http://cs.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lu.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xo.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://wb.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://uz.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ph.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://ne.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kl.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://on.szxytkj.cn

[A15] 空值判断与默认值
来源：http://xn.szxytkj.cn

Py:   value = data or "默认值"
来源：http://iz.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://xv.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://bo.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://jk.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wz.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://jy.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://pw.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://pi.jctech888.com.cn

[A16] 真假值判断规则
来源：http://ym.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xg.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rt.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jy.huixiangedu.cn

TS:   if (!x) {}
来源：http://np.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cp.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://px.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lz.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jz.shxzskj.cn

[A17] 位运算
来源：http://vo.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ni.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cx.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wz.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fk.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jc.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dl.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://dx.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://bl.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://ul.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jm.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://in.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://fo.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ay.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://vk.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://xw.haigaiapp.cn

[A19] 交换两个变量
来源：http://zt.shxzukj.cn

Py:   a, b = b, a
来源：http://im.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zn.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://mg.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://fp.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://oh.nicolike.cn

Go:   a, b = b, a
来源：http://hn.huanxung.cn

Ruby: a, b = b, a
来源：http://cn.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://co.yuexingan06.cn

[A20] 读取标准输入
来源：http://ek.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://jd.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hl.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ir.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://lp.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://qq.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zl.muxihuayi.cn

Ruby: gets.chomp
来源：http://ae.hahajie.cn

C#:   Console.ReadLine();
来源：http://ke.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://ot.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://su.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hi.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://vp.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://mw.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://do.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cs.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://pq.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://sm.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://qk.szsharing.cn

Py:   len(s)
来源：http://ra.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nf.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rk.521024.cn

TS:   s.length
来源：http://wh.asd995.cn

Java: s.length()
来源：http://mx.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cw.jctech888.com.cn

Ruby: s.length
来源：http://rd.shtwfgs.cn

C#:   s.Length
来源：http://bj.szxytkj.cn

[A23] 大小写转换
来源：http://ae.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wn.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ev.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://it.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wd.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://og.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mw.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ki.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mt.wgjwhj.cn

[A24] 去除首尾空白
来源：http://xr.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ws.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qn.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yx.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lf.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mw.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://jw.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mc.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ir.wgjwhj.cn

[A25] 字符串比较
来源：http://cj.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://xx.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nq.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://za.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ob.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ge.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kf.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zf.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kv.nicolike.cn

[A26] 类型转换总览
来源：http://wo.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oy.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aa.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://an.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://pw.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kv.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rm.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gz.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sy.bookmarksfly.cn

================================================================================
来源：http://iu.yuexingan06.cn

B. 流程控制
来源：http://zq.wgjwhj.cn

================================================================================
来源：http://rg.nicolike.cn

[B01] 条件判断 if / else
来源：http://ym.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mw.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wl.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rd.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ho.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zh.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yb.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ti.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fw.9csxet.cn

[B02] 多分支 else if / elif
来源：http://od.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xp.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dt.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ke.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eo.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nm.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.shxzukj.cn

[B03] switch / match / case
来源：http://tp.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mm.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qt.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iv.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yg.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oq.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://do.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iq.haigaiapp.cn

[B04] for 计数循环
来源：http://rk.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://yw.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fg.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hd.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mb.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ld.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cd.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://gg.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bm.9csxet.cn


<!-- 参考信息 -->