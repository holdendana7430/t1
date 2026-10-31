代发 wailian999

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oy.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hx.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ub.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bg.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mv.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tw.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hg.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jy.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ze.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tf.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bi.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ja.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ok.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zz.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sl.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wz.huanxung.cn

================================================================================
来源：http://my.shxzskj.cn

A. 基础语法与类型
来源：http://mq.nszjky.cn

================================================================================
来源：http://co.9csxet.cn

[A01] Hello World
来源：http://at.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://fu.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://fs.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://oz.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uv.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://cc.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://xf.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://lo.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xz.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://ou.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vb.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sc.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pg.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ba.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://el.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://xd.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://jv.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jj.jianghongdianzi.cn

[A03] 常量定义
来源：http://qg.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jk.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://fq.hahajie.cn

JS:   const PI = 3.14159;
来源：http://fn.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://fc.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://ay.hnjuh.cn

Go:   const PI = 3.14159
来源：http://sx.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://ui.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://sh.hnjuh.cn

[A04] 判断变量类型
来源：http://nb.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bx.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vv.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pg.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://hn.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tc.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yu.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://om.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://vk.wgjwhj.cn

[A05] 整数除法与取模
来源：http://lj.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rb.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://co.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vw.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cu.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://ch.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://ne.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://tz.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://hu.asd995.cn

[A06] 字符串转数字
来源：http://yb.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://ts.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ta.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dx.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rh.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cl.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ab.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gn.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ut.shxzukj.cn

[A07] 数字转字符串
来源：http://dd.panjiajie.cn

Py:   str(42)
来源：http://et.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://kl.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://qh.shtwfgs.cn

TS:   String(42)
来源：http://eq.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://if.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://cm.newstarts.cn

Ruby: 42.to_s
来源：http://vw.9csxet.cn

C#:   42.ToString()
来源：http://ee.hahajie.cn

[A08] 取整与四舍五入
来源：http://za.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rn.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://df.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gk.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kw.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zv.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mf.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dp.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kd.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://wb.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gy.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pm.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jd.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://un.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uo.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://za.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jn.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wt.shxzukj.cn

[A10] 生成随机数
来源：http://cv.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://ma.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://rd.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yt.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xq.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://mw.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fg.shtwfgs.cn

Ruby: rand(1..100)
来源：http://uz.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://jw.colortex.cn

[A11] 条件表达式（三元）
来源：http://uf.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qx.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iw.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sd.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ge.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://jl.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ty.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://az.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ts.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://md.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zo.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rb.521024.cn

JS:   `Hello, ${name}!`
来源：http://ku.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://nh.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://id.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yq.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://up.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://lf.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mx.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://sh.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://kf.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://rt.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://te.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://gp.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://eo.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://zb.nicolike.cn

C#:   "第一行\n第二行"
来源：http://bw.nszjky.cn

[A14] 注释写法
来源：http://mm.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zo.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kk.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://so.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://if.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qm.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://hk.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ro.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://tm.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://sp.hahajie.cn

Py:   value = data or "默认值"
来源：http://gy.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://sj.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://ex.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://by.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ff.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://ts.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://ql.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://sk.lnxyls.cn

[A16] 真假值判断规则
来源：http://sb.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zu.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cc.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zo.newstarts.cn

TS:   if (!x) {}
来源：http://gp.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ee.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://na.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gr.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pg.huanxung.cn

[A17] 位运算
来源：http://di.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://od.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ic.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mw.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fs.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pf.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lo.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ij.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://dw.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://rf.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yc.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fn.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://nn.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bl.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://in.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://sn.521024.cn

[A19] 交换两个变量
来源：http://vm.nszjky.cn

Py:   a, b = b, a
来源：http://qi.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sh.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://se.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://vv.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://kd.panjiajie.cn

Go:   a, b = b, a
来源：http://pj.shxzskj.cn

Ruby: a, b = b, a
来源：http://ft.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://af.hnjuh.cn

[A20] 读取标准输入
来源：http://ov.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://nw.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ix.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://va.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://uf.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://lx.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kf.panjiajie.cn

Ruby: gets.chomp
来源：http://mn.nicolike.cn

C#:   Console.ReadLine();
来源：http://wh.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://or.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://fq.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bd.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://ey.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ab.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://xk.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vx.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://if.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://sy.szsharing.cn

[A22] 获取字符串长度
来源：http://xi.muxihuayi.cn

Py:   len(s)
来源：http://ms.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ta.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ql.panjiajie.cn

TS:   s.length
来源：http://no.jianghongdianzi.cn

Java: s.length()
来源：http://tf.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ob.colortex.cn

Ruby: s.length
来源：http://kt.yuntaijiaju.cn

C#:   s.Length
来源：http://ve.huixiangedu.cn

[A23] 大小写转换
来源：http://uf.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nc.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bg.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://js.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hg.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tw.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gs.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dm.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://os.shtwfgs.cn

[A24] 去除首尾空白
来源：http://xb.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uz.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qz.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qi.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rn.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rl.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://mu.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wv.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jz.lnxyls.cn

[A25] 字符串比较
来源：http://pd.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://zn.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dy.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mn.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pa.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qu.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://at.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vx.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gv.shtwfgs.cn

[A26] 类型转换总览
来源：http://ny.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wk.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://as.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zb.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://hl.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vo.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bf.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://du.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tj.shxzukj.cn

================================================================================
来源：http://nd.muxihuayi.cn

B. 流程控制
来源：http://zi.521024.cn

================================================================================
来源：http://cd.hahajie.cn

[B01] 条件判断 if / else
来源：http://jd.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cf.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://md.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ve.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cl.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jm.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vh.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tb.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ys.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://fq.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qa.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ua.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iv.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xb.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xq.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eu.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://li.gzmigu.cn

[B03] switch / match / case
来源：http://ib.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kv.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qv.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://em.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://md.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ii.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tf.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ku.shxzskj.cn

[B04] for 计数循环
来源：http://xj.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://bv.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lj.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nm.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vg.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vx.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ib.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://gq.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yr.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://ag.521024.cn

Py:   for item in arr: print(item)
来源：http://vd.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qs.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dc.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ag.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://de.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://sj.jctech888.com.cn


<!-- 参考信息 -->