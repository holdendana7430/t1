代发 wailian999

--------------------------------------------------------------------------------
来源：http://ds.jctech888.com.cn

目  录
来源：http://qo.asd995.cn

--------------------------------------------------------------------------------
来源：http://nl.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tf.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qo.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iv.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oo.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xo.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tp.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rw.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uz.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lm.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vv.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gp.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ef.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://se.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hu.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pu.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ng.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yu.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lg.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mz.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lr.szsharing.cn

================================================================================
来源：http://fa.wgjwhj.cn

A. 基础语法与类型
来源：http://km.wgjwhj.cn

================================================================================
来源：http://ir.nszjky.cn

[A01] Hello World
来源：http://vd.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://wc.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://az.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://gn.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lo.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://cs.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://ld.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://uc.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zj.szxytkj.cn

[A02] 变量声明与赋值
来源：http://gy.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yw.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ga.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://db.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bu.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://cd.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://xm.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://vn.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ou.chemitech.net.cn

[A03] 常量定义
来源：http://lr.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lu.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://rg.szsharing.cn

JS:   const PI = 3.14159;
来源：http://tg.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://hu.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ul.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://yd.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://cr.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://yt.szsharing.cn

[A04] 判断变量类型
来源：http://wh.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lc.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xw.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yy.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://hw.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jm.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://we.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ch.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://xh.huanxung.cn

[A05] 整数除法与取模
来源：http://di.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ls.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vu.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pk.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hv.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ny.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://zn.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://am.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://pw.panjiajie.cn

[A06] 字符串转数字
来源：http://xt.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://zy.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xc.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://in.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yp.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ux.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cu.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zk.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jq.shxzskj.cn

[A07] 数字转字符串
来源：http://hq.huanxung.cn

Py:   str(42)
来源：http://vw.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://xi.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://cx.bjjhwx.cn

TS:   String(42)
来源：http://mt.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wf.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://po.bookmarksfly.cn

Ruby: 42.to_s
来源：http://jj.haigaiapp.cn

C#:   42.ToString()
来源：http://ps.nszjky.cn

[A08] 取整与四舍五入
来源：http://yn.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mr.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ef.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ph.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qm.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vj.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yj.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ut.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ek.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://co.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ns.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ov.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qe.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vw.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sr.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qm.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uv.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ix.asd995.cn

[A10] 生成随机数
来源：http://oh.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://sm.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ln.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ba.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://by.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://cb.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bd.shxzskj.cn

Ruby: rand(1..100)
来源：http://hx.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://qn.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://en.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://fb.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dp.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hl.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wz.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ha.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bm.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sd.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://th.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://wz.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ay.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://um.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://qy.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://bi.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ax.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vu.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://ck.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://jy.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://no.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://ws.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://ws.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://za.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://kh.hnjuh.cn

Java: "第一行\n第二行"
来源：http://nz.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://hl.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://do.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://lw.chemitech.net.cn

[A14] 注释写法
来源：http://as.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ci.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lg.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://ir.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://xg.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dw.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://gy.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://za.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://og.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://yy.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://bp.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://vs.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://ft.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://kg.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zz.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ei.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://av.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://gt.huixiangedu.cn

[A16] 真假值判断规则
来源：http://di.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hy.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mw.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nr.9csxet.cn

TS:   if (!x) {}
来源：http://lq.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ky.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tk.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://um.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nd.colortex.cn

[A17] 位运算
来源：http://sv.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://do.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jq.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aa.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fp.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://px.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://rz.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://vx.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ca.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uc.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qr.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://ti.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nm.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://zx.asd995.cn

C#:   (int)'A'; (char)65
来源：http://jk.muxihuayi.cn

[A19] 交换两个变量
来源：http://zp.bookmarksfly.cn

Py:   a, b = b, a
来源：http://vy.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pu.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://zx.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://dy.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://zx.bjjhwx.cn

Go:   a, b = b, a
来源：http://ne.wgjwhj.cn

Ruby: a, b = b, a
来源：http://rv.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://vl.jctech888.com.cn

[A20] 读取标准输入
来源：http://lx.521024.cn

Py:   name = input("请输入：")
来源：http://pr.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cf.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bo.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://hy.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://dc.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ef.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://sm.9csxet.cn

C#:   Console.ReadLine();
来源：http://yq.521024.cn

[A21] 保留指定小数位输出
来源：http://aj.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://dk.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kc.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://oc.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://yl.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://lg.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://se.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://mw.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://aa.shtwfgs.cn

[A22] 获取字符串长度
来源：http://ww.panjiajie.cn

Py:   len(s)
来源：http://vs.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sc.wgjwhj.cn

TS:   s.length
来源：http://bz.chemitech.net.cn

Java: s.length()
来源：http://dk.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oy.jctech888.com.cn

Ruby: s.length
来源：http://qn.haigaiapp.cn

C#:   s.Length
来源：http://xz.shxzskj.cn

[A23] 大小写转换
来源：http://ko.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pr.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yc.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bo.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xj.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zf.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nn.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rd.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yo.shtwfgs.cn

[A24] 去除首尾空白
来源：http://xi.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fr.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fm.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vs.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yx.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yv.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://ay.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xf.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ki.nszjky.cn

[A25] 字符串比较
来源：http://cc.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://yq.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lv.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ek.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wp.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yc.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nx.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sh.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ml.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://gy.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fw.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vf.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fl.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://lz.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qo.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xc.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aa.bookmarksfly.cn

================================================================================
来源：http://cz.521024.cn

B. 流程控制
来源：http://fn.colortex.cn

================================================================================
来源：http://xl.szsharing.cn

[B01] 条件判断 if / else
来源：http://vv.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hr.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wp.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wz.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vs.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mm.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nl.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://se.asd995.cn

[B02] 多分支 else if / elif
来源：http://am.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qs.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ts.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bl.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uj.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ct.panjiajie.cn

[B03] switch / match / case
来源：http://pj.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yu.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cj.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://av.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rf.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gy.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bk.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lm.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gk.asd995.cn

[B04] for 计数循环
来源：http://ia.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://lk.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://do.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ln.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bk.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ow.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jn.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://uf.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xm.lnxyls.cn


<!-- 参考信息 -->