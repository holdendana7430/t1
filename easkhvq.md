代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kt.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pe.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vl.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ex.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mj.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://us.lnxyls.cn

【文件统计】
来源：http://hc.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wj.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ob.szsharing.cn

目  录
来源：http://md.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://lp.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hq.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kt.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yc.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fj.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kd.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dv.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dk.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bz.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ms.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lt.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qv.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ql.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pa.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rc.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ti.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dj.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://be.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aq.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bj.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rf.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ok.bookmarksfly.cn

================================================================================
来源：http://xl.chemitech.net.cn

A. 基础语法与类型
来源：http://ro.jctech888.com.cn

================================================================================
来源：http://jm.shxzskj.cn

[A01] Hello World
来源：http://pb.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://pp.521024.cn

PHP:  echo "Hello, World!";
来源：http://uo.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://dd.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aq.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://mt.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://jt.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://de.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tk.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ek.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://me.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tl.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bb.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fu.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ot.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://bt.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://au.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xh.panjiajie.cn

[A03] 常量定义
来源：http://xj.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ka.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://hq.9csxet.cn

JS:   const PI = 3.14159;
来源：http://zk.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://dh.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://wc.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ut.shxzskj.cn

Ruby: PI = 3.14159
来源：http://dt.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://sg.shxzukj.cn

[A04] 判断变量类型
来源：http://sr.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uq.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lb.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ud.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ev.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yw.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yr.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uh.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://kn.chemitech.net.cn

[A05] 整数除法与取模
来源：http://or.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tg.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uw.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hp.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rw.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://xx.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://sg.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://ux.521024.cn

C#:   7 / 2; 7 % 2
来源：http://ob.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ky.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://gv.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ax.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iv.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ox.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ci.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://or.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ko.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yd.huixiangedu.cn

[A07] 数字转字符串
来源：http://tj.huixiangedu.cn

Py:   str(42)
来源：http://la.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://ey.colortex.cn

JS:   String(42); (42).toString()
来源：http://by.nszjky.cn

TS:   String(42)
来源：http://hn.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sg.521024.cn

Go:   strconv.Itoa(42)
来源：http://yo.gzmigu.cn

Ruby: 42.to_s
来源：http://vu.asd995.cn

C#:   42.ToString()
来源：http://ih.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://so.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ve.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wj.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xs.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ab.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fc.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yv.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gs.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fs.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://ml.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eo.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ua.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://at.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lk.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mz.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cn.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cp.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xw.bjjhwx.cn

[A10] 生成随机数
来源：http://sp.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://cs.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://au.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kq.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bh.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://zo.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sg.9csxet.cn

Ruby: rand(1..100)
来源：http://bs.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://us.huanxung.cn

[A11] 条件表达式（三元）
来源：http://bw.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://wj.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mv.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bf.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ze.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://rp.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kz.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zm.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oz.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://lw.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ux.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tw.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://pd.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://co.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://lw.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tu.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://ge.asd995.cn

C#:   $"Hello, {name}!"
来源：http://ly.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://on.colortex.cn

Py:   "第一行\n第二行"
来源：http://al.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://wl.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://ci.szsharing.cn

TS:   "第一行\n第二行"
来源：http://nv.gzmigu.cn

Java: "第一行\n第二行"
来源：http://ul.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://al.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://wm.huanxung.cn

C#:   "第一行\n第二行"
来源：http://jl.huixinmuqiang.cn

[A14] 注释写法
来源：http://ev.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ti.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vz.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://hr.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://dy.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jt.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://ns.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vf.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://an.colortex.cn

[A15] 空值判断与默认值
来源：http://pf.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://fu.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://dd.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://gj.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://rd.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ya.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://yf.9csxet.cn

Ruby: value = data || "默认值"
来源：http://aw.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://rl.shxzukj.cn

[A16] 真假值判断规则
来源：http://jn.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wh.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://up.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zx.gzmigu.cn

TS:   if (!x) {}
来源：http://qh.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://se.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://au.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qc.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zw.huixiangedu.cn

[A17] 位运算
来源：http://rt.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nw.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bv.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mp.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kp.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ny.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://tr.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://vv.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://vk.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pi.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fa.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://oy.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ae.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://dh.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://be.huixiangedu.cn

[A19] 交换两个变量
来源：http://la.shxzukj.cn

Py:   a, b = b, a
来源：http://ct.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xt.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://br.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ve.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ev.jctech888.com.cn

Go:   a, b = b, a
来源：http://tj.colortex.cn

Ruby: a, b = b, a
来源：http://xd.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://es.colortex.cn

[A20] 读取标准输入
来源：http://ge.shxzukj.cn

Py:   name = input("请输入：")
来源：http://sw.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fn.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://en.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://xo.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://mg.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vh.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://by.shxzskj.cn

C#:   Console.ReadLine();
来源：http://fk.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://vw.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://ar.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ap.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://xx.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://kw.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://dd.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xo.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://wh.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://bx.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://vj.colortex.cn

Py:   len(s)
来源：http://wx.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rt.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kt.szsharing.cn

TS:   s.length
来源：http://ug.bjjhwx.cn

Java: s.length()
来源：http://bj.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tx.chemitech.net.cn

Ruby: s.length
来源：http://ws.huanxung.cn

C#:   s.Length
来源：http://wc.huixiangedu.cn

[A23] 大小写转换
来源：http://tw.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xr.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sn.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xf.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mt.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xh.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ke.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xh.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lo.huixiangedu.cn

[A24] 去除首尾空白
来源：http://pj.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kc.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ly.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wm.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hv.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sn.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://hg.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lf.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wg.yuntaijiaju.cn

[A25] 字符串比较
来源：http://vw.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://kf.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ly.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zf.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fc.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gu.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ym.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zp.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vw.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://qj.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nk.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ci.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://li.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://uz.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mu.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qr.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kl.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ed.bjjhwx.cn

================================================================================
来源：http://xz.hnjuh.cn

B. 流程控制
来源：http://fr.521024.cn

================================================================================
来源：http://hy.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://zl.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kj.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ub.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rj.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vg.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bo.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fh.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sx.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://um.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ym.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yo.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://on.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://io.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ti.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ub.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.newstarts.cn

[B03] switch / match / case
来源：http://mq.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://db.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://er.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oq.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pq.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ir.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sl.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pc.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cf.hnjuh.cn

[B04] for 计数循环
来源：http://bo.bookmarksfly.cn


<!-- 参考信息 -->