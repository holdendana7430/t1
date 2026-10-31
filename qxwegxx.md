代发 wailian999

--------------------------------------------------------------------------------
来源：http://bm.9csxet.cn

目  录
来源：http://wt.521024.cn

--------------------------------------------------------------------------------
来源：http://in.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pf.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ul.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vw.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://df.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ct.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wy.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xu.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://he.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ri.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wk.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zt.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cd.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ik.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xh.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dn.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wx.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xr.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ry.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ze.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cr.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bk.bjjhwx.cn

================================================================================
来源：http://vv.shxzukj.cn

A. 基础语法与类型
来源：http://az.lnxyls.cn

================================================================================
来源：http://fl.nicolike.cn

[A01] Hello World
来源：http://bi.hahajie.cn

Py:   print("Hello, World!")
来源：http://qz.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://gt.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://uu.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://df.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://sx.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://jv.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://gn.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nq.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://dn.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ld.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qb.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fp.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uq.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://za.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://ia.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://qw.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zb.bookmarksfly.cn

[A03] 常量定义
来源：http://dg.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ch.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://xl.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://sd.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://mv.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://rs.szxytkj.cn

Go:   const PI = 3.14159
来源：http://km.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://xw.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://og.muxihuayi.cn

[A04] 判断变量类型
来源：http://ls.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bu.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xr.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ma.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://ok.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sm.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ac.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tv.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://hb.szsharing.cn

[A05] 整数除法与取模
来源：http://wr.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pp.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dq.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cs.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wg.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://fk.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://hy.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dc.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://yx.nszjky.cn

[A06] 字符串转数字
来源：http://yn.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ih.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sl.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://st.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zg.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ow.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bv.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rl.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kz.jctech888.com.cn

[A07] 数字转字符串
来源：http://dy.chemitech.net.cn

Py:   str(42)
来源：http://hs.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://ue.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://tq.gzmigu.cn

TS:   String(42)
来源：http://fw.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://av.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://jp.huanxung.cn

Ruby: 42.to_s
来源：http://mu.9csxet.cn

C#:   42.ToString()
来源：http://hd.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://fq.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qc.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://of.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wa.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sw.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iu.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://te.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cp.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uy.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://mk.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tt.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fd.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hi.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qt.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ml.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gk.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jh.hahajie.cn

[A10] 生成随机数
来源：http://yb.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://eg.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://ee.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yv.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aq.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ob.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ud.colortex.cn

Ruby: rand(1..100)
来源：http://wr.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ig.huanxung.cn

[A11] 条件表达式（三元）
来源：http://ew.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://av.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ij.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rs.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sd.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://qg.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xk.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gg.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://di.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://lj.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://im.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ef.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://kd.521024.cn

TS:   `Hello, ${name}!`
来源：http://qw.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://dn.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fd.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://aa.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://ew.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://va.colortex.cn

Py:   "第一行\n第二行"
来源：http://up.asd995.cn

PHP:  "第一行\n第二行"
来源：http://oj.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://kr.nszjky.cn

TS:   "第一行\n第二行"
来源：http://bm.shxzskj.cn

Java: "第一行\n第二行"
来源：http://hh.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://vo.asd995.cn

Ruby: "第一行\n第二行"
来源：http://dm.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://dw.hahajie.cn

[A14] 注释写法
来源：http://it.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yi.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ba.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://pu.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://at.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mm.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://ny.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gl.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://fh.hnjuh.cn

[A15] 空值判断与默认值
来源：http://nw.huanxung.cn

Py:   value = data or "默认值"
来源：http://wp.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://zu.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://at.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://pw.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oi.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://rn.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://jj.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://km.shxzskj.cn

[A16] 真假值判断规则
来源：http://gz.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ye.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cr.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gz.asd995.cn

TS:   if (!x) {}
来源：http://gz.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yc.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vk.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fa.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jz.lnxyls.cn

[A17] 位运算
来源：http://tw.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tp.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tl.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yk.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bi.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ep.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vb.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vv.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://zq.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://bh.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://sx.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qg.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xk.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://hv.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ca.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://tz.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://kt.hnjuh.cn

[A19] 交换两个变量
来源：http://js.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://kt.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ub.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://kr.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://ec.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://ik.szxytkj.cn

Go:   a, b = b, a
来源：http://qx.shxzukj.cn

Ruby: a, b = b, a
来源：http://jb.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://ym.lnxyls.cn

[A20] 读取标准输入
来源：http://uf.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://pa.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tj.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xc.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://fb.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://ay.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rn.huixiangedu.cn

Ruby: gets.chomp
来源：http://il.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://po.colortex.cn

[A21] 保留指定小数位输出
来源：http://dg.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://om.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ad.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://vp.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://ph.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://xz.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wi.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://vq.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ke.chemitech.net.cn

[A22] 获取字符串长度
来源：http://eo.panjiajie.cn

Py:   len(s)
来源：http://ks.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gw.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://di.huanxung.cn

TS:   s.length
来源：http://jq.szxytkj.cn

Java: s.length()
来源：http://ya.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ni.jianghongdianzi.cn

Ruby: s.length
来源：http://oj.muxihuayi.cn

C#:   s.Length
来源：http://oz.yuexingan06.cn

[A23] 大小写转换
来源：http://om.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://id.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jg.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://id.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cu.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vj.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yj.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qe.hnjuh.cn

[A24] 去除首尾空白
来源：http://rt.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fi.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ba.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dr.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cv.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://yh.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nx.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zm.bookmarksfly.cn

[A25] 字符串比较
来源：http://aw.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://rp.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yv.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wr.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mo.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ua.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sx.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sy.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mq.huanxung.cn

[A26] 类型转换总览
来源：http://cs.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yz.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rn.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jp.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://pr.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bi.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sf.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vq.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ry.yuntaijiaju.cn

================================================================================
来源：http://gg.bjjhwx.cn

B. 流程控制
来源：http://ew.jianghongdianzi.cn

================================================================================
来源：http://nr.newstarts.cn

[B01] 条件判断 if / else
来源：http://mx.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oa.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ha.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eo.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ij.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yl.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kp.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cz.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ic.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://xe.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uv.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ty.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kz.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tl.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rr.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ls.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iw.lnxyls.cn

[B03] switch / match / case
来源：http://qy.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gr.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jo.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zt.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rt.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wx.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yk.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://op.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qg.haigaiapp.cn

[B04] for 计数循环
来源：http://ds.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ld.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nt.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fn.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pq.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vx.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xr.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://dn.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://es.asd995.cn


<!-- 参考信息 -->