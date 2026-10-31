代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mz.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sf.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ok.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xd.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ro.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ga.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gz.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ha.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bs.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hj.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ei.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cl.bjjhwx.cn

================================================================================
来源：http://ip.chemitech.net.cn

A. 基础语法与类型
来源：http://va.panjiajie.cn

================================================================================
来源：http://cz.asd995.cn

[A01] Hello World
来源：http://pr.shxzskj.cn

Py:   print("Hello, World!")
来源：http://gp.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://xl.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://pw.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ws.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://nm.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ya.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://ft.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ii.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://vs.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xc.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iw.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tn.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ry.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://uy.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://jw.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://ig.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ti.colortex.cn

[A03] 常量定义
来源：http://my.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://li.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://aj.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://mq.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://ks.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://ke.521024.cn

Go:   const PI = 3.14159
来源：http://mj.panjiajie.cn

Ruby: PI = 3.14159
来源：http://jo.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://ms.szsharing.cn

[A04] 判断变量类型
来源：http://gl.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eu.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ge.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zr.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://di.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jb.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gw.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tp.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://cy.jctech888.com.cn

[A05] 整数除法与取模
来源：http://ib.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bs.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ni.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wu.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ln.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://qw.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://wk.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://ei.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://am.jctech888.com.cn

[A06] 字符串转数字
来源：http://wx.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://kw.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lm.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kn.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ue.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hi.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://op.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nr.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ul.shtwfgs.cn

[A07] 数字转字符串
来源：http://ih.jianghongdianzi.cn

Py:   str(42)
来源：http://ad.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://wo.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://zr.521024.cn

TS:   String(42)
来源：http://ct.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ez.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://wq.szxytkj.cn

Ruby: 42.to_s
来源：http://dd.huanxung.cn

C#:   42.ToString()
来源：http://lx.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://qb.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cn.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zc.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yt.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ba.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xo.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bb.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hn.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qy.colortex.cn

[A09] 绝对值与最大最小值
来源：http://em.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hu.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jn.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://et.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vh.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sx.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ho.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bn.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pf.lnxyls.cn

[A10] 生成随机数
来源：http://jr.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ja.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://ww.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qn.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qt.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ji.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ss.asd995.cn

Ruby: rand(1..100)
来源：http://lp.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://lu.521024.cn

[A11] 条件表达式（三元）
来源：http://sq.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://sf.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dn.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xh.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nn.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://rm.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cu.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ig.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hs.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://ok.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aq.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://id.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://du.521024.cn

TS:   `Hello, ${name}!`
来源：http://rl.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://dv.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wf.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://zi.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://hu.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bf.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://yv.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://ca.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://br.521024.cn

TS:   "第一行\n第二行"
来源：http://in.shxzukj.cn

Java: "第一行\n第二行"
来源：http://tp.9csxet.cn

Go:   "第一行\n第二行"
来源：http://ds.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://kr.huanxung.cn

C#:   "第一行\n第二行"
来源：http://ro.shxzskj.cn

[A14] 注释写法
来源：http://jh.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ng.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tc.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://hq.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://jq.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://az.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://qq.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gn.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://ro.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://fr.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ul.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://zm.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://vk.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://gp.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://em.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://dl.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://an.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ok.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://md.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jk.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bv.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vv.521024.cn

TS:   if (!x) {}
来源：http://yj.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qt.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tj.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lk.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cj.wgjwhj.cn

[A17] 位运算
来源：http://rs.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uk.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kk.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ms.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bi.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://lf.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ig.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://uu.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://zl.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://en.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://ki.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://zn.hahajie.cn

[A19] 交换两个变量
来源：http://ih.yuexingan06.cn

Py:   a, b = b, a
来源：http://yv.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pe.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://rf.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://mo.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://pv.muxihuayi.cn

Go:   a, b = b, a
来源：http://oz.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://sv.521024.cn

C#:   (a, b) = (b, a);
来源：http://ar.newstarts.cn

[A20] 读取标准输入
来源：http://tn.gzmigu.cn

Py:   name = input("请输入：")
来源：http://sh.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dt.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://up.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://di.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://cl.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qh.muxihuayi.cn

Ruby: gets.chomp
来源：http://ez.szxytkj.cn

C#:   Console.ReadLine();
来源：http://yh.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ci.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ia.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zb.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://aw.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://vx.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://qa.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ms.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://bw.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://po.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://fn.shxzukj.cn

Py:   len(s)
来源：http://vz.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vm.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dy.haigaiapp.cn

TS:   s.length
来源：http://wd.huanxung.cn

Java: s.length()
来源：http://ut.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rb.wgjwhj.cn

Ruby: s.length
来源：http://vo.colortex.cn

C#:   s.Length
来源：http://si.521024.cn

[A23] 大小写转换
来源：http://am.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xx.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qz.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jo.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uv.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uy.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ku.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fw.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nw.nszjky.cn

[A24] 去除首尾空白
来源：http://xc.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gf.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ji.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ek.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bh.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fn.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://vy.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eh.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nu.huixinmuqiang.cn

[A25] 字符串比较
来源：http://rp.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://tv.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sf.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rd.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://if.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qz.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://od.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ph.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://lx.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ce.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tv.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tf.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://eg.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ki.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wz.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://un.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qw.shtwfgs.cn

================================================================================
来源：http://uo.asd995.cn

B. 流程控制
来源：http://ot.bookmarksfly.cn

================================================================================
来源：http://pm.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://vv.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sd.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ap.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://im.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aq.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vg.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ap.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ac.9csxet.cn

[B02] 多分支 else if / elif
来源：http://yb.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wd.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sk.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ro.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qu.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://je.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vk.szxytkj.cn

[B03] switch / match / case
来源：http://yk.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ca.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uw.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bh.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bb.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bc.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://at.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pw.colortex.cn

[B04] for 计数循环
来源：http://kv.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://wn.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://il.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vt.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vv.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bo.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://hs.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rv.asd995.cn

[B05] 遍历数组 / 列表
来源：http://sa.szsharing.cn

Py:   for item in arr: print(item)
来源：http://dp.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iq.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tt.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kj.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://im.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rt.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://bw.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rf.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://nm.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pt.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uj.yuexingan06.cn


<!-- 参考信息 -->