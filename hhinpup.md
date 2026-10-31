代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ww.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jo.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gh.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vm.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://it.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xg.nszjky.cn

【文件统计】
来源：http://ml.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kv.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://zi.hahajie.cn

目  录
来源：http://ti.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://lx.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ib.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dw.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bm.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zr.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mb.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bh.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gt.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xj.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://he.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ni.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://op.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kv.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nj.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rz.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gr.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://so.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yk.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sd.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xj.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ta.szxytkj.cn

================================================================================
来源：http://kz.gzmigu.cn

A. 基础语法与类型
来源：http://jy.shxzskj.cn

================================================================================
来源：http://ue.huanxung.cn

[A01] Hello World
来源：http://fv.nszjky.cn

Py:   print("Hello, World!")
来源：http://zc.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://fe.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://se.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ez.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://sx.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ne.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://pz.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yy.shxzskj.cn

[A02] 变量声明与赋值
来源：http://ga.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ay.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jf.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fg.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qp.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://sd.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://ww.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://lc.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qb.huixinmuqiang.cn

[A03] 常量定义
来源：http://yu.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nm.colortex.cn

PHP:  const PI = 3.14159;
来源：http://mw.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://vk.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://lo.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://nr.shxzskj.cn

Go:   const PI = 3.14159
来源：http://zu.szsharing.cn

Ruby: PI = 3.14159
来源：http://ry.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://lt.szxytkj.cn

[A04] 判断变量类型
来源：http://kc.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ev.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dz.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://we.521024.cn

TS:   typeof x; x instanceof Date
来源：http://na.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ov.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fi.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sj.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://dw.9csxet.cn

[A05] 整数除法与取模
来源：http://mw.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mu.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wq.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tt.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ep.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://la.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://bm.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://gx.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://fn.shxzskj.cn

[A06] 字符串转数字
来源：http://sm.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://ge.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ib.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xn.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sl.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mx.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zy.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ex.colortex.cn

[A07] 数字转字符串
来源：http://lc.hnjuh.cn

Py:   str(42)
来源：http://kp.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://ff.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://hk.9csxet.cn

TS:   String(42)
来源：http://th.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ji.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://vb.hnjuh.cn

Ruby: 42.to_s
来源：http://rs.hahajie.cn

C#:   42.ToString()
来源：http://xa.hahajie.cn

[A08] 取整与四舍五入
来源：http://gr.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pe.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ge.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xz.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yw.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uz.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vg.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bi.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pd.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://sm.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://or.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yy.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ya.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ou.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mb.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dc.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kx.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hf.szxytkj.cn

[A10] 生成随机数
来源：http://dt.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ft.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://fj.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jl.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://js.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://oc.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ku.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://fd.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://nc.szsharing.cn

[A11] 条件表达式（三元）
来源：http://pi.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://zk.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cr.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://en.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cv.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ky.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xk.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://em.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://el.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://xl.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hn.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gt.asd995.cn

JS:   `Hello, ${name}!`
来源：http://vk.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://mw.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://re.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ht.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://ob.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://oq.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eh.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://wo.asd995.cn

PHP:  "第一行\n第二行"
来源：http://bz.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://wf.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://ya.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://gf.colortex.cn

Go:   "第一行\n第二行"
来源：http://se.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://wx.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://oo.asd995.cn

[A14] 注释写法
来源：http://rv.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ij.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tp.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://aj.521024.cn

TS:   // 单行；/* 多行 */
来源：http://ea.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bv.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://kn.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fd.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://gl.9csxet.cn

[A15] 空值判断与默认值
来源：http://vp.nszjky.cn

Py:   value = data or "默认值"
来源：http://mi.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://db.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://fo.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://pt.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://db.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://ti.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://su.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://hr.panjiajie.cn

[A16] 真假值判断规则
来源：http://ql.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mo.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hy.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xe.nszjky.cn

TS:   if (!x) {}
来源：http://oo.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ov.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nl.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ru.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qr.hnjuh.cn

[A17] 位运算
来源：http://or.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ci.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://se.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hw.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://po.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yg.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://lc.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://hq.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://qr.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bf.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wj.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://bs.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lf.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://pl.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://uw.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://te.nszjky.cn

Py:   a, b = b, a
来源：http://ko.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ds.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://uf.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://zr.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://qn.nicolike.cn

Go:   a, b = b, a
来源：http://rl.asd995.cn

Ruby: a, b = b, a
来源：http://rb.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://if.hahajie.cn

[A20] 读取标准输入
来源：http://ep.nicolike.cn

Py:   name = input("请输入：")
来源：http://hs.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ep.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qq.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://uh.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://qh.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qn.hahajie.cn

Ruby: gets.chomp
来源：http://kz.lnxyls.cn

C#:   Console.ReadLine();
来源：http://hr.521024.cn

[A21] 保留指定小数位输出
来源：http://ao.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://cj.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hx.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://yw.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ym.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://zl.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gv.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://dk.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://qt.szsharing.cn

[A22] 获取字符串长度
来源：http://ex.jctech888.com.cn

Py:   len(s)
来源：http://oi.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uh.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uh.gzmigu.cn

TS:   s.length
来源：http://ms.lnxyls.cn

Java: s.length()
来源：http://fa.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tt.yuntaijiaju.cn

Ruby: s.length
来源：http://rv.nicolike.cn

C#:   s.Length
来源：http://jc.shxzukj.cn

[A23] 大小写转换
来源：http://ep.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lq.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ix.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yt.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ae.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nq.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mh.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vk.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zh.9csxet.cn

[A24] 去除首尾空白
来源：http://lo.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wf.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mx.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pc.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pw.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gk.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://le.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qb.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mh.jctech888.com.cn

[A25] 字符串比较
来源：http://zq.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://sj.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ct.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ra.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ly.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ys.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cj.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uf.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xb.bookmarksfly.cn

[A26] 类型转换总览
来源：http://ey.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uj.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xp.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yj.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://jv.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cq.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gc.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://js.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dg.9csxet.cn

================================================================================
来源：http://co.gzmigu.cn

B. 流程控制
来源：http://uh.hnjuh.cn

================================================================================
来源：http://yn.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://kd.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nx.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pu.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xv.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qw.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xn.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wi.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ap.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ad.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://ts.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ny.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://od.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kr.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mx.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gd.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://md.bookmarksfly.cn

[B03] switch / match / case
来源：http://cz.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wp.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fc.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bu.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gj.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fq.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ut.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lh.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hi.shxzukj.cn

[B04] for 计数循环
来源：http://pz.chemitech.net.cn


<!-- 参考信息 -->