代发 wailian999

--------------------------------------------------------------------------------
来源：http://yy.szxytkj.cn

目  录
来源：http://it.nicolike.cn

--------------------------------------------------------------------------------
来源：http://lf.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://md.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bb.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ju.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ej.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bi.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wi.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sm.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nt.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ap.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nd.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lq.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zi.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tb.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dm.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qc.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pf.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lx.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ut.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sf.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hm.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ct.nszjky.cn

================================================================================
来源：http://mw.521024.cn

A. 基础语法与类型
来源：http://sw.szsharing.cn

================================================================================
来源：http://vd.colortex.cn

[A01] Hello World
来源：http://ix.shxzukj.cn

Py:   print("Hello, World!")
来源：http://sp.521024.cn

PHP:  echo "Hello, World!";
来源：http://hj.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://fm.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lp.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://ai.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://pm.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://rz.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gf.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://hw.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kk.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://re.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ez.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jr.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://oq.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://sq.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://cw.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oo.521024.cn

[A03] 常量定义
来源：http://sw.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xs.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://be.9csxet.cn

JS:   const PI = 3.14159;
来源：http://sm.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://ie.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://ar.hahajie.cn

Go:   const PI = 3.14159
来源：http://uy.asd995.cn

Ruby: PI = 3.14159
来源：http://sz.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://fp.hnjuh.cn

[A04] 判断变量类型
来源：http://yo.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cx.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cf.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qd.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://tf.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lq.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ks.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lu.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://fi.newstarts.cn

[A05] 整数除法与取模
来源：http://aw.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cz.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nn.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ux.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ee.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://fc.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://ke.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://rl.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://il.chemitech.net.cn

[A06] 字符串转数字
来源：http://jv.521024.cn

Py:   int("42"); float("3.14")
来源：http://fg.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yq.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kx.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ad.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://df.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xe.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yr.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ir.jctech888.com.cn

[A07] 数字转字符串
来源：http://aw.panjiajie.cn

Py:   str(42)
来源：http://wc.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://zx.huanxung.cn

JS:   String(42); (42).toString()
来源：http://hl.jianghongdianzi.cn

TS:   String(42)
来源：http://ue.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kg.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://fj.nszjky.cn

Ruby: 42.to_s
来源：http://ti.jctech888.com.cn

C#:   42.ToString()
来源：http://jo.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://wx.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://at.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ys.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wq.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bu.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sv.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ub.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lm.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ie.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://xp.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wi.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://we.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gg.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sv.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lz.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ge.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rg.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ji.chemitech.net.cn

[A10] 生成随机数
来源：http://ry.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://te.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://rp.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kf.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://or.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://cv.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vp.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://ch.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://pr.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://cy.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://pt.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ka.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zh.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sg.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://cb.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xo.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hs.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fg.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://xz.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mc.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ok.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://xe.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://vu.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://qk.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dx.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://ek.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://xq.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ss.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://ae.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://yr.colortex.cn

JS:   "第一行\n第二行"
来源：http://pw.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://po.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://yv.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://xk.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://zl.nicolike.cn

C#:   "第一行\n第二行"
来源：http://rr.lnxyls.cn

[A14] 注释写法
来源：http://vu.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://em.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ka.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://pl.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://bg.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://af.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://lv.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oo.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://zp.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://wr.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://kl.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ne.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://ts.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://os.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nz.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://gi.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://ew.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://vx.shxzskj.cn

[A16] 真假值判断规则
来源：http://ma.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rn.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qd.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xd.szxytkj.cn

TS:   if (!x) {}
来源：http://zx.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lb.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rn.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://im.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://co.muxihuayi.cn

[A17] 位运算
来源：http://ne.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qy.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tj.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lv.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uy.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oi.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://of.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ph.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zx.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://fv.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://vw.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://pl.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lq.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://dd.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gp.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://pj.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://ol.nszjky.cn

[A19] 交换两个变量
来源：http://vz.wgjwhj.cn

Py:   a, b = b, a
来源：http://ko.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jh.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://hv.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://rs.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://wh.hnjuh.cn

Go:   a, b = b, a
来源：http://gm.shtwfgs.cn

Ruby: a, b = b, a
来源：http://ea.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://qw.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://om.lnxyls.cn

Py:   name = input("请输入：")
来源：http://wd.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fz.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cg.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://tt.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://az.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wk.asd995.cn

Ruby: gets.chomp
来源：http://ot.hnjuh.cn

C#:   Console.ReadLine();
来源：http://dt.9csxet.cn

[A21] 保留指定小数位输出
来源：http://xm.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://pf.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ck.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://vr.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://gm.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ze.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://do.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://wn.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://pe.gzmigu.cn

[A22] 获取字符串长度
来源：http://xq.gzmigu.cn

Py:   len(s)
来源：http://mg.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://go.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bi.wgjwhj.cn

TS:   s.length
来源：http://eh.jctech888.com.cn

Java: s.length()
来源：http://al.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xw.bookmarksfly.cn

Ruby: s.length
来源：http://hh.nszjky.cn

C#:   s.Length
来源：http://pe.szxytkj.cn

[A23] 大小写转换
来源：http://qr.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://we.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kz.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://th.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lv.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fu.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wo.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jq.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eh.nicolike.cn

[A24] 去除首尾空白
来源：http://ro.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fz.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nv.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kp.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bt.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://of.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bn.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ui.hahajie.cn

[A25] 字符串比较
来源：http://qv.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://xq.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ak.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zs.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bq.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gr.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pb.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zw.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vv.gzmigu.cn

[A26] 类型转换总览
来源：http://yz.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sy.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jr.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gu.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://sn.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kk.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pq.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qz.shxzukj.cn

================================================================================
来源：http://dt.yuexingan06.cn

B. 流程控制
来源：http://ro.haigaiapp.cn

================================================================================
来源：http://wx.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://hn.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kt.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ag.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ty.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nm.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eu.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://se.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dx.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zh.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://ze.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sy.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cb.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zw.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tx.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ti.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://me.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.bjjhwx.cn

[B03] switch / match / case
来源：http://vy.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mi.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yc.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vk.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hb.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yi.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bs.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nl.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jb.lnxyls.cn

[B04] for 计数循环
来源：http://ob.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://hq.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cu.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ql.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aj.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ek.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://te.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ye.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kd.bookmarksfly.cn


<!-- 参考信息 -->