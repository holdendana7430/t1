代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jc.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ew.yuntaijiaju.cn

【文件统计】
来源：http://xk.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qv.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://gh.newstarts.cn

目  录
来源：http://tu.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://jp.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tt.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ha.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gj.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kp.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qq.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dl.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cs.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ut.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pr.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fb.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ul.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fa.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kk.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mf.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qd.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tq.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mh.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oq.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wn.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qh.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mp.hahajie.cn

================================================================================
来源：http://go.shtwfgs.cn

A. 基础语法与类型
来源：http://aq.huanxung.cn

================================================================================
来源：http://sb.9csxet.cn

[A01] Hello World
来源：http://mp.panjiajie.cn

Py:   print("Hello, World!")
来源：http://xh.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://al.colortex.cn

JS:   console.log("Hello, World!");
来源：http://ja.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sk.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://hh.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://du.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://tt.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mz.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://rv.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wl.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ip.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ry.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gi.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://cg.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://nn.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://vv.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bt.shxzukj.cn

[A03] 常量定义
来源：http://tk.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lw.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://hd.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://rw.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://zw.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://qi.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://kl.colortex.cn

Ruby: PI = 3.14159
来源：http://sc.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://bq.szxytkj.cn

[A04] 判断变量类型
来源：http://hl.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ll.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://re.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ai.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://jk.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ac.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qk.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://th.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://ws.wgjwhj.cn

[A05] 整数除法与取模
来源：http://xy.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fu.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zx.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kd.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hb.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://we.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://ba.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://ou.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://qc.hnjuh.cn

[A06] 字符串转数字
来源：http://vw.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://gz.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xt.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yl.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oc.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mv.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jl.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wn.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vw.nicolike.cn

[A07] 数字转字符串
来源：http://kg.bjjhwx.cn

Py:   str(42)
来源：http://st.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://qa.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://hd.hnjuh.cn

TS:   String(42)
来源：http://um.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fv.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://ty.szsharing.cn

Ruby: 42.to_s
来源：http://rp.newstarts.cn

C#:   42.ToString()
来源：http://mt.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://sa.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ta.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oc.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gl.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vh.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://he.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xh.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yz.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zd.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ev.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zv.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nb.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://po.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ol.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cn.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sa.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uc.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wj.shxzskj.cn

[A10] 生成随机数
来源：http://bv.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://gq.9csxet.cn

PHP:  random_int(1, 100);
来源：http://na.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tc.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lh.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://xl.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://du.9csxet.cn

Ruby: rand(1..100)
来源：http://nj.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://fq.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://ih.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ky.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kw.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hg.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rk.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://gs.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://af.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://el.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cf.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://un.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jt.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ae.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://fg.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://li.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://hg.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://py.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://xl.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://rc.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ha.szsharing.cn

Py:   "第一行\n第二行"
来源：http://kt.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://nh.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://jo.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://sn.9csxet.cn

Java: "第一行\n第二行"
来源：http://kn.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ds.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://jc.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://vw.shxzukj.cn

[A14] 注释写法
来源：http://me.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bd.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vj.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://dm.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://fo.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tq.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://sf.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://it.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://da.asd995.cn

[A15] 空值判断与默认值
来源：http://pt.hnjuh.cn

Py:   value = data or "默认值"
来源：http://qj.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://kj.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://vv.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://ky.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jl.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://oj.szsharing.cn

Ruby: value = data || "默认值"
来源：http://vb.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://zs.panjiajie.cn

[A16] 真假值判断规则
来源：http://ax.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uw.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rt.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hc.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://sp.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zl.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rk.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qo.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bp.muxihuayi.cn

[A17] 位运算
来源：http://wg.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wk.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lj.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cg.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rj.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pa.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tm.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nq.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://td.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://zg.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://zn.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nj.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ld.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://ct.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://em.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://mn.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://se.huixiangedu.cn

[A19] 交换两个变量
来源：http://db.nicolike.cn

Py:   a, b = b, a
来源：http://fq.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bq.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://rv.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://dh.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://cw.hnjuh.cn

Go:   a, b = b, a
来源：http://jy.shxzskj.cn

Ruby: a, b = b, a
来源：http://rm.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://kx.huixiangedu.cn

[A20] 读取标准输入
来源：http://ae.szsharing.cn

Py:   name = input("请输入：")
来源：http://ck.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gr.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yf.asd995.cn

TS:   // Node.js：readline 模块
来源：http://ap.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://cg.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qx.wgjwhj.cn

Ruby: gets.chomp
来源：http://nu.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://bt.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://zk.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://tx.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wm.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ih.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://eh.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://cx.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gs.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://xy.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://mj.huanxung.cn

[A22] 获取字符串长度
来源：http://ia.asd995.cn

Py:   len(s)
来源：http://db.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://db.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xt.hahajie.cn

TS:   s.length
来源：http://mg.shxzskj.cn

Java: s.length()
来源：http://ph.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ou.chemitech.net.cn

Ruby: s.length
来源：http://xh.nszjky.cn

C#:   s.Length
来源：http://pe.nszjky.cn

[A23] 大小写转换
来源：http://oj.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ru.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://se.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pf.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ap.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iv.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ra.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tq.lnxyls.cn

[A24] 去除首尾空白
来源：http://pn.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ug.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cr.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mb.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uj.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cw.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://tl.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jz.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rb.nicolike.cn

[A25] 字符串比较
来源：http://tn.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://jj.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bn.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fc.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zs.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://su.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://io.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lr.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uf.bjjhwx.cn

[A26] 类型转换总览
来源：http://xo.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fz.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qo.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tj.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://ju.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hf.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jw.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qk.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ds.bjjhwx.cn

================================================================================
来源：http://uo.newstarts.cn

B. 流程控制
来源：http://hj.bjjhwx.cn

================================================================================
来源：http://ch.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://gy.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gm.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cl.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bf.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nl.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nn.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bp.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iz.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zs.huanxung.cn

[B02] 多分支 else if / elif
来源：http://sm.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bv.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mh.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ed.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ei.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kf.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.jianghongdianzi.cn

[B03] switch / match / case
来源：http://el.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qs.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mn.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tn.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cp.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cf.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yt.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uh.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ib.hnjuh.cn

[B04] for 计数循环
来源：http://lg.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://rj.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tc.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sf.hahajie.cn


<!-- 参考信息 -->