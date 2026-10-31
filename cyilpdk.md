代发 wailian999

--------------------------------------------------------------------------------
来源：http://aw.asd995.cn

目  录
来源：http://yu.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ex.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://so.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mn.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://an.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://if.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tk.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wa.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://md.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dr.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gm.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pn.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://el.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sf.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cw.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://il.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ye.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cy.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yp.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kf.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ng.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sv.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://to.huixiangedu.cn

================================================================================
来源：http://qc.nicolike.cn

A. 基础语法与类型
来源：http://fd.muxihuayi.cn

================================================================================
来源：http://yy.huixinmuqiang.cn

[A01] Hello World
来源：http://lz.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://qs.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://fk.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://ls.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mp.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://tp.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://or.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://gv.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vl.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://ra.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uh.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://si.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ql.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fk.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://bk.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://da.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://gu.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bp.newstarts.cn

[A03] 常量定义
来源：http://mi.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eo.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://xc.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://hw.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://gg.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://ok.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://gc.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://wd.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://rx.shtwfgs.cn

[A04] 判断变量类型
来源：http://ro.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jz.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dz.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eq.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://ck.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://te.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vm.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gb.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://os.muxihuayi.cn

[A05] 整数除法与取模
来源：http://zz.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mk.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zv.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lj.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dq.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://wx.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://zv.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ye.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://ay.9csxet.cn

[A06] 字符串转数字
来源：http://mk.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://xs.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gm.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ls.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wx.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://md.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uk.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lm.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://um.jctech888.com.cn

[A07] 数字转字符串
来源：http://ib.9csxet.cn

Py:   str(42)
来源：http://op.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://gc.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://rj.wgjwhj.cn

TS:   String(42)
来源：http://me.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zy.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://wl.chemitech.net.cn

Ruby: 42.to_s
来源：http://aj.huanxung.cn

C#:   42.ToString()
来源：http://ml.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://lx.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ns.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ul.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ez.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tu.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jf.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bz.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qn.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lk.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://de.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oa.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://os.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ni.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sc.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nn.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zl.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sm.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xg.newstarts.cn

[A10] 生成随机数
来源：http://yw.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://ye.colortex.cn

PHP:  random_int(1, 100);
来源：http://kh.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lb.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zu.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://jj.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gx.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://kp.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://mh.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://zv.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://zi.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aq.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ws.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cs.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://cv.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://en.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qx.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dd.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://bj.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tp.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lt.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://pt.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://kd.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ol.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ik.521024.cn

Ruby: "Hello, #{name}!"
来源：http://vi.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://yf.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uf.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://rm.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://kw.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://rb.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://gr.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ba.hahajie.cn

Go:   "第一行\n第二行"
来源：http://ym.asd995.cn

Ruby: "第一行\n第二行"
来源：http://wl.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://ov.nicolike.cn

[A14] 注释写法
来源：http://yk.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ba.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ir.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://kf.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://af.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ph.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://ma.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dr.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://sj.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://fa.szsharing.cn

Py:   value = data or "默认值"
来源：http://dw.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://xj.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://bv.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://ye.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://af.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://ur.521024.cn

Ruby: value = data || "默认值"
来源：http://zr.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://fn.newstarts.cn

[A16] 真假值判断规则
来源：http://jx.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://af.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jp.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ob.hnjuh.cn

TS:   if (!x) {}
来源：http://ec.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xi.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ih.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uy.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cu.jctech888.com.cn

[A17] 位运算
来源：http://ib.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lc.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wd.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xy.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iu.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fv.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qp.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://mz.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://da.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://ox.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://of.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mu.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://tr.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sb.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://dr.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://aj.asd995.cn

[A19] 交换两个变量
来源：http://cp.wgjwhj.cn

Py:   a, b = b, a
来源：http://aq.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nc.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://fs.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://lp.521024.cn

Java: int t = a; a = b; b = t;
来源：http://en.wgjwhj.cn

Go:   a, b = b, a
来源：http://wr.9csxet.cn

Ruby: a, b = b, a
来源：http://ty.521024.cn

C#:   (a, b) = (b, a);
来源：http://ec.newstarts.cn

[A20] 读取标准输入
来源：http://aw.gzmigu.cn

Py:   name = input("请输入：")
来源：http://vu.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mp.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sk.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://ne.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://sl.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ro.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://ea.panjiajie.cn

C#:   Console.ReadLine();
来源：http://bl.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://fy.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://aj.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bb.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://sy.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://od.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://yu.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ff.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://rm.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://iq.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://om.nszjky.cn

Py:   len(s)
来源：http://xs.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sw.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ik.bookmarksfly.cn

TS:   s.length
来源：http://ax.hahajie.cn

Java: s.length()
来源：http://kg.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://np.shxzukj.cn

Ruby: s.length
来源：http://el.shxzskj.cn

C#:   s.Length
来源：http://fr.huixinmuqiang.cn

[A23] 大小写转换
来源：http://wt.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jl.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yn.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pr.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ty.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tq.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xs.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wg.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uj.lnxyls.cn

[A24] 去除首尾空白
来源：http://kn.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tq.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xm.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rz.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gt.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://pt.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rp.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hv.wgjwhj.cn

[A25] 字符串比较
来源：http://he.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ns.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yn.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ne.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ls.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dn.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eu.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ou.hnjuh.cn

[A26] 类型转换总览
来源：http://lb.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://il.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xx.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vv.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://ab.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vg.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lg.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wc.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ut.huanxung.cn

================================================================================
来源：http://qq.bookmarksfly.cn

B. 流程控制
来源：http://tz.yuntaijiaju.cn

================================================================================
来源：http://fm.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://py.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vt.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://go.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://df.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ki.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vj.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://od.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gs.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xe.521024.cn

[B02] 多分支 else if / elif
来源：http://on.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rp.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bk.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sh.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yt.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ut.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://df.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nn.chemitech.net.cn

[B03] switch / match / case
来源：http://kt.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gw.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nn.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sj.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://th.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nv.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mm.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bl.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lr.jianghongdianzi.cn

[B04] for 计数循环
来源：http://re.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://kn.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://if.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hc.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://on.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tc.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://bu.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yk.nszjky.cn


<!-- 参考信息 -->