代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uf.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://va.hnjuh.cn

【文件统计】
来源：http://kz.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mi.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://gu.muxihuayi.cn

目  录
来源：http://fg.521024.cn

--------------------------------------------------------------------------------
来源：http://gr.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gh.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sd.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fx.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lf.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sj.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jf.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pe.shtwfgs.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vw.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jv.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ar.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vb.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fe.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zv.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wo.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vn.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xu.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xt.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cu.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ev.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jd.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://st.muxihuayi.cn

================================================================================
来源：http://yz.huixinmuqiang.cn

A. 基础语法与类型
来源：http://gt.hahajie.cn

================================================================================
来源：http://fr.shxzukj.cn

[A01] Hello World
来源：http://am.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://wj.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://zw.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://xb.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://af.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://ea.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://vj.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://vh.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zq.newstarts.cn

[A02] 变量声明与赋值
来源：http://zk.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wt.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uv.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cs.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ou.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://qi.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://ae.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://mk.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pk.9csxet.cn

[A03] 常量定义
来源：http://jy.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ie.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://bl.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://it.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://as.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://hx.nszjky.cn

Go:   const PI = 3.14159
来源：http://es.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://ad.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://cc.9csxet.cn

[A04] 判断变量类型
来源：http://se.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hn.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hh.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hi.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://uo.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sx.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://al.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vj.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ay.bjjhwx.cn

[A05] 整数除法与取模
来源：http://ii.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fr.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cs.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yc.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hn.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://mk.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://cr.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://vt.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://ix.huixiangedu.cn

[A06] 字符串转数字
来源：http://yt.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://lr.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rz.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jn.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ut.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hr.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vk.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sa.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ft.huixiangedu.cn

[A07] 数字转字符串
来源：http://dn.jctech888.com.cn

Py:   str(42)
来源：http://ol.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://il.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://nx.bookmarksfly.cn

TS:   String(42)
来源：http://di.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lw.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://uy.panjiajie.cn

Ruby: 42.to_s
来源：http://kg.huixinmuqiang.cn

C#:   42.ToString()
来源：http://me.shxzukj.cn

[A08] 取整与四舍五入
来源：http://br.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ut.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ww.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hx.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nh.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sq.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nl.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ig.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dv.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://fk.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cx.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://on.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://my.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pf.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ch.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bz.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://un.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qb.jianghongdianzi.cn

[A10] 生成随机数
来源：http://tt.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://jl.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://bw.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tl.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://re.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://gf.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lo.shtwfgs.cn

Ruby: rand(1..100)
来源：http://kl.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://vk.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://fi.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://ik.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gr.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aq.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tl.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://bq.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mp.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ta.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rl.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://fo.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gy.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ee.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://lk.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://lh.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://kh.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zc.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://ur.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://oc.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nl.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://rt.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://qy.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://mb.521024.cn

TS:   "第一行\n第二行"
来源：http://hc.asd995.cn

Java: "第一行\n第二行"
来源：http://gm.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://eh.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://gd.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://jb.wgjwhj.cn

[A14] 注释写法
来源：http://jh.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pv.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nk.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://bs.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://ga.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://es.521024.cn

Go:   // 单行；/* 多行 */
来源：http://pu.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vk.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://or.colortex.cn

[A15] 空值判断与默认值
来源：http://qz.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://jr.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://jw.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://vp.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://xl.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gs.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ts.hahajie.cn

Ruby: value = data || "默认值"
来源：http://ll.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://kj.521024.cn

[A16] 真假值判断规则
来源：http://bc.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://st.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fw.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pg.newstarts.cn

TS:   if (!x) {}
来源：http://kl.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://id.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pr.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vy.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qo.asd995.cn

[A17] 位运算
来源：http://hk.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tm.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pd.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aa.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dx.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://ni.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://cm.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://yq.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tg.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.521024.cn

Java: (int) 'A'; (char) 65
来源：http://tv.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aq.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://wp.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://ex.haigaiapp.cn

[A19] 交换两个变量
来源：http://zb.shxzukj.cn

Py:   a, b = b, a
来源：http://au.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ma.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://jr.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://zl.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://nc.nszjky.cn

Go:   a, b = b, a
来源：http://ul.hahajie.cn

Ruby: a, b = b, a
来源：http://hu.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://rs.chemitech.net.cn

[A20] 读取标准输入
来源：http://hu.panjiajie.cn

Py:   name = input("请输入：")
来源：http://gc.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zo.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ao.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://ts.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://yc.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qf.huanxung.cn

Ruby: gets.chomp
来源：http://fs.nszjky.cn

C#:   Console.ReadLine();
来源：http://rp.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://qq.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://ql.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bb.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://tj.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://kq.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://fm.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ds.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://pc.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://mb.colortex.cn

[A22] 获取字符串长度
来源：http://mw.hahajie.cn

Py:   len(s)
来源：http://uj.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sy.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fi.huixinmuqiang.cn

TS:   s.length
来源：http://jc.huixiangedu.cn

Java: s.length()
来源：http://jj.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wb.hnjuh.cn

Ruby: s.length
来源：http://nf.huixinmuqiang.cn

C#:   s.Length
来源：http://go.szsharing.cn

[A23] 大小写转换
来源：http://zw.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vj.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gg.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rd.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cm.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cg.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rs.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yb.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bl.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://jm.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sd.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://le.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jn.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yx.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mt.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://ng.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dm.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://me.gzmigu.cn

[A25] 字符串比较
来源：http://vf.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://nq.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ou.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sf.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sy.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pd.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xs.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vt.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ub.jctech888.com.cn

[A26] 类型转换总览
来源：http://bj.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ef.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zt.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wz.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://rt.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xd.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://df.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nr.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bk.szsharing.cn

================================================================================
来源：http://wy.muxihuayi.cn

B. 流程控制
来源：http://lg.bjjhwx.cn

================================================================================
来源：http://nq.colortex.cn

[B01] 条件判断 if / else
来源：http://wd.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lc.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ts.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uu.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mh.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://my.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ft.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wy.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xn.asd995.cn

[B02] 多分支 else if / elif
来源：http://pr.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eb.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hf.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ys.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wc.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vy.colortex.cn

[B03] switch / match / case
来源：http://eh.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gs.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://me.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kh.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vj.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tp.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mf.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zb.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gk.521024.cn

[B04] for 计数循环
来源：http://iz.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://rz.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ze.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kg.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://td.newstarts.cn


<!-- 参考信息 -->