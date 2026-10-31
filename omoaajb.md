代发 wailian999

--------------------------------------------------------------------------------
来源：http://qh.nicolike.cn

目  录
来源：http://zt.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://bp.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jv.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://om.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nk.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kb.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fc.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tj.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wy.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tv.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wc.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tr.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lu.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tr.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mm.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://er.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ue.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ah.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dg.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yy.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lm.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://or.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gl.gzmigu.cn

================================================================================
来源：http://sd.muxihuayi.cn

A. 基础语法与类型
来源：http://up.wgjwhj.cn

================================================================================
来源：http://jf.huixiangedu.cn

[A01] Hello World
来源：http://mp.9csxet.cn

Py:   print("Hello, World!")
来源：http://hr.colortex.cn

PHP:  echo "Hello, World!";
来源：http://tb.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://az.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sd.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://za.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://pm.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://nf.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sf.asd995.cn

[A02] 变量声明与赋值
来源：http://ke.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fl.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gr.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ci.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kt.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://hg.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://wy.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://ew.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hs.yuntaijiaju.cn

[A03] 常量定义
来源：http://hv.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hv.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://nz.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://ax.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://my.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://zf.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://wo.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ma.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ac.shtwfgs.cn

[A04] 判断变量类型
来源：http://sb.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mt.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eg.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ta.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://qk.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wb.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pa.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://so.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://nn.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://yj.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lf.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://za.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ft.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pb.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://bo.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://od.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://rq.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://br.shxzukj.cn

[A06] 字符串转数字
来源：http://jo.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://fo.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://om.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vp.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jm.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tp.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ye.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ha.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ri.szsharing.cn

[A07] 数字转字符串
来源：http://yo.asd995.cn

Py:   str(42)
来源：http://uo.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://gg.colortex.cn

JS:   String(42); (42).toString()
来源：http://xf.panjiajie.cn

TS:   String(42)
来源：http://fd.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gk.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://em.lnxyls.cn

Ruby: 42.to_s
来源：http://ds.shtwfgs.cn

C#:   42.ToString()
来源：http://xn.szsharing.cn

[A08] 取整与四舍五入
来源：http://qw.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qq.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vw.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kr.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mm.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fh.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ow.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xx.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cy.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://in.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iu.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hl.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hw.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hq.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yf.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://la.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ew.asd995.cn

[A10] 生成随机数
来源：http://nl.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://pl.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://xz.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ph.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://en.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://in.nicolike.cn

Ruby: rand(1..100)
来源：http://qv.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://dv.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://ku.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://ip.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ce.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fr.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lq.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://av.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ty.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fs.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yd.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://au.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ma.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ko.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://ww.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://cr.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://nt.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jz.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://ok.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://wz.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ex.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://nm.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://vf.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://vl.szsharing.cn

TS:   "第一行\n第二行"
来源：http://zy.lnxyls.cn

Java: "第一行\n第二行"
来源：http://uz.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bu.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://oh.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://mn.nicolike.cn

[A14] 注释写法
来源：http://lh.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bp.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bg.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://oi.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://yk.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mj.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://cb.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pc.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://xr.newstarts.cn

[A15] 空值判断与默认值
来源：http://wh.hnjuh.cn

Py:   value = data or "默认值"
来源：http://nt.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://in.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://na.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://uj.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xf.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://eg.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://xp.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://yt.muxihuayi.cn

[A16] 真假值判断规则
来源：http://gc.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ur.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yc.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yj.shtwfgs.cn

TS:   if (!x) {}
来源：http://dw.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mb.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rt.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yw.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ty.shtwfgs.cn

[A17] 位运算
来源：http://jt.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ng.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ak.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jz.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wg.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cg.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rp.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://wg.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://eu.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://zu.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xr.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ca.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://jn.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cr.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://uu.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://jw.shtwfgs.cn

[A19] 交换两个变量
来源：http://te.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://mt.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ll.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://qf.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://is.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://tn.shtwfgs.cn

Go:   a, b = b, a
来源：http://zd.wgjwhj.cn

Ruby: a, b = b, a
来源：http://fo.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://uj.bookmarksfly.cn

[A20] 读取标准输入
来源：http://of.nicolike.cn

Py:   name = input("请输入：")
来源：http://ai.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://el.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://fc.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://xd.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nl.yuexingan06.cn

Ruby: gets.chomp
来源：http://pr.lnxyls.cn

C#:   Console.ReadLine();
来源：http://pi.huanxung.cn

[A21] 保留指定小数位输出
来源：http://db.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://gs.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bg.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://oz.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://eh.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://cp.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ba.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ed.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://kw.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://lt.hahajie.cn

Py:   len(s)
来源：http://fn.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pe.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uk.nicolike.cn

TS:   s.length
来源：http://gk.9csxet.cn

Java: s.length()
来源：http://bl.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vb.shtwfgs.cn

Ruby: s.length
来源：http://sn.yuntaijiaju.cn

C#:   s.Length
来源：http://tm.nszjky.cn

[A23] 大小写转换
来源：http://bs.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ui.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://py.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ed.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qb.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pq.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jw.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://se.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ci.szsharing.cn

[A24] 去除首尾空白
来源：http://jp.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ua.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sy.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fy.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aq.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://up.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://yo.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fy.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mc.yuexingan06.cn

[A25] 字符串比较
来源：http://cf.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://bb.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tt.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lu.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://le.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nq.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kl.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wq.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wi.colortex.cn

[A26] 类型转换总览
来源：http://fs.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lq.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zn.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dp.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://th.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mz.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jc.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dj.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://io.newstarts.cn

================================================================================
来源：http://ev.newstarts.cn

B. 流程控制
来源：http://ds.9csxet.cn

================================================================================
来源：http://ag.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://oz.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xk.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oc.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vl.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wz.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qr.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://go.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ik.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jz.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://oh.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tr.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bp.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xq.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://si.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.panjiajie.cn

[B03] switch / match / case
来源：http://lm.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jl.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kq.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tg.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xl.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qa.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://el.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qu.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ga.wgjwhj.cn

[B04] for 计数循环
来源：http://hf.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://va.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lm.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dw.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vh.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fp.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iu.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://sg.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://no.chemitech.net.cn


<!-- 参考信息 -->