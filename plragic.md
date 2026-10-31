代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hg.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iq.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gw.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ie.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tb.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ua.huixiangedu.cn

【文件统计】
来源：http://zq.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://an.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hv.huixinmuqiang.cn

目  录
来源：http://gp.521024.cn

--------------------------------------------------------------------------------
来源：http://ut.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lu.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ev.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wd.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nz.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vi.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hc.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pi.shtwfgs.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tb.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ua.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vi.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hk.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xc.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vx.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qx.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://om.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eg.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iw.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bo.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fv.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fk.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xn.huixinmuqiang.cn

================================================================================
来源：http://df.shxzskj.cn

A. 基础语法与类型
来源：http://up.haigaiapp.cn

================================================================================
来源：http://gf.panjiajie.cn

[A01] Hello World
来源：http://tn.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://ed.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://jm.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://rf.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cv.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://rl.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://su.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://ik.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wz.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://ye.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ed.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rx.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fo.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wg.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://sj.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://xy.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://gn.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xz.hahajie.cn

[A03] 常量定义
来源：http://he.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://so.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://jy.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://mq.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://nv.colortex.cn

Java: static final double PI = 3.14159;
来源：http://gr.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://re.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://hz.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://zn.shtwfgs.cn

[A04] 判断变量类型
来源：http://ad.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://im.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yv.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vs.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://ph.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sd.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fi.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mw.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://ml.wgjwhj.cn

[A05] 整数除法与取模
来源：http://co.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nr.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ab.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ha.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ft.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://dr.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://qf.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://rf.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://yy.szsharing.cn

[A06] 字符串转数字
来源：http://aq.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://lv.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kj.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xq.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://il.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jt.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ev.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ax.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pt.haigaiapp.cn

[A07] 数字转字符串
来源：http://jh.gzmigu.cn

Py:   str(42)
来源：http://kv.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://wr.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://pz.haigaiapp.cn

TS:   String(42)
来源：http://gz.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uz.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://ca.nicolike.cn

Ruby: 42.to_s
来源：http://zb.9csxet.cn

C#:   42.ToString()
来源：http://ab.9csxet.cn

[A08] 取整与四舍五入
来源：http://pc.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eo.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xo.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ps.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dy.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kx.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lq.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ko.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sx.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://fh.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hc.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kj.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yj.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xs.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xa.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mf.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qu.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ju.bjjhwx.cn

[A10] 生成随机数
来源：http://jz.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://xw.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://bi.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tm.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xk.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://xy.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xk.lnxyls.cn

Ruby: rand(1..100)
来源：http://ci.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://nr.nicolike.cn

[A11] 条件表达式（三元）
来源：http://gw.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://nj.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pn.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yv.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fo.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://rb.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tc.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lb.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vh.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://ea.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gm.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ya.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://id.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://vx.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://jp.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nn.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://ib.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://ky.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hl.hahajie.cn

Py:   "第一行\n第二行"
来源：http://yt.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://af.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://ot.9csxet.cn

TS:   "第一行\n第二行"
来源：http://yk.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://pp.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ax.colortex.cn

Ruby: "第一行\n第二行"
来源：http://kh.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://fu.521024.cn

[A14] 注释写法
来源：http://vk.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fz.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://bq.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://yw.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kn.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ie.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vx.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://eg.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://dx.huanxung.cn

Py:   value = data or "默认值"
来源：http://kt.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://xl.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://fr.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://pz.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wl.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://yc.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://rp.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://sn.colortex.cn

[A16] 真假值判断规则
来源：http://cd.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pd.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pe.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mb.shxzskj.cn

TS:   if (!x) {}
来源：http://ky.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://co.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cn.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uz.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eu.jctech888.com.cn

[A17] 位运算
来源：http://mt.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ge.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xz.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vs.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nt.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xo.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jp.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xv.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://ol.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://fs.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://ez.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kp.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uo.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://mj.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ck.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://zq.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://mg.haigaiapp.cn

[A19] 交换两个变量
来源：http://ko.9csxet.cn

Py:   a, b = b, a
来源：http://fl.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qi.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://mc.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://bz.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://bd.shxzukj.cn

Go:   a, b = b, a
来源：http://mt.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://iq.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://rx.hahajie.cn

[A20] 读取标准输入
来源：http://vj.shxzskj.cn

Py:   name = input("请输入：")
来源：http://kt.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zg.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lu.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://mh.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://lf.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://of.lnxyls.cn

Ruby: gets.chomp
来源：http://yp.hnjuh.cn

C#:   Console.ReadLine();
来源：http://tz.nicolike.cn

[A21] 保留指定小数位输出
来源：http://rp.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://dx.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ja.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://dj.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://cm.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://vy.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ue.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ew.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ky.nszjky.cn

[A22] 获取字符串长度
来源：http://rt.hnjuh.cn

Py:   len(s)
来源：http://nm.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wa.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tp.szxytkj.cn

TS:   s.length
来源：http://ok.chemitech.net.cn

Java: s.length()
来源：http://ws.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sd.jianghongdianzi.cn

Ruby: s.length
来源：http://tv.szsharing.cn

C#:   s.Length
来源：http://bk.colortex.cn

[A23] 大小写转换
来源：http://ja.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kp.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qa.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wq.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://to.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://po.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zu.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bu.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.muxihuayi.cn

[A24] 去除首尾空白
来源：http://eo.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://io.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kk.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yu.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ey.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://wo.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zo.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://se.szsharing.cn

[A25] 字符串比较
来源：http://sx.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://ra.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wk.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tc.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ij.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qp.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vh.bjjhwx.cn

[A26] 类型转换总览
来源：http://da.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wu.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xc.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mr.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://on.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wx.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://br.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fa.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rm.gzmigu.cn

================================================================================
来源：http://yj.chemitech.net.cn

B. 流程控制
来源：http://zl.lnxyls.cn

================================================================================
来源：http://of.gzmigu.cn

[B01] 条件判断 if / else
来源：http://xh.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sk.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nc.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ob.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://az.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ka.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://we.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hw.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sp.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://kf.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ph.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fl.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ou.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gw.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ri.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ue.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wl.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cv.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kj.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nk.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kk.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ey.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ae.haigaiapp.cn

[B04] for 计数循环
来源：http://tj.hahajie.cn


<!-- 参考信息 -->