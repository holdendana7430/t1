代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dw.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ss.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qw.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uo.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ye.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ul.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kq.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://is.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jz.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cw.yuexingan06.cn

【文件统计】
来源：http://fu.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cz.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uh.wgjwhj.cn

目  录
来源：http://tz.colortex.cn

--------------------------------------------------------------------------------
来源：http://ge.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tg.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sf.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://np.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wx.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nn.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://py.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cg.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hv.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ui.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qq.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jt.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nf.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iv.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qw.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zy.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jz.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cb.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lr.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iu.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gn.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ji.newstarts.cn

================================================================================
来源：http://rc.haigaiapp.cn

A. 基础语法与类型
来源：http://ak.hahajie.cn

================================================================================
来源：http://gb.chemitech.net.cn

[A01] Hello World
来源：http://zq.shxzskj.cn

Py:   print("Hello, World!")
来源：http://da.521024.cn

PHP:  echo "Hello, World!";
来源：http://re.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://el.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zi.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ot.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://wv.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://dy.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ol.9csxet.cn

[A02] 变量声明与赋值
来源：http://sa.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://op.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cq.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://de.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ay.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://wq.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://df.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://og.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zf.hahajie.cn

[A03] 常量定义
来源：http://fz.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ep.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://yr.nicolike.cn

JS:   const PI = 3.14159;
来源：http://zg.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ul.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://iu.panjiajie.cn

Go:   const PI = 3.14159
来源：http://fp.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://xg.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://ow.muxihuayi.cn

[A04] 判断变量类型
来源：http://ke.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ze.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rt.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vz.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://ab.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yd.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lj.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xo.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://xd.bjjhwx.cn

[A05] 整数除法与取模
来源：http://gz.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xu.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vg.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ku.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://na.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://gw.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://rh.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://si.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://vb.panjiajie.cn

[A06] 字符串转数字
来源：http://bz.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://zz.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://em.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fp.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://by.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xg.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ww.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ln.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vw.wgjwhj.cn

[A07] 数字转字符串
来源：http://kg.panjiajie.cn

Py:   str(42)
来源：http://nn.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://xt.newstarts.cn

JS:   String(42); (42).toString()
来源：http://pu.yuntaijiaju.cn

TS:   String(42)
来源：http://zb.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://at.colortex.cn

Go:   strconv.Itoa(42)
来源：http://bi.nszjky.cn

Ruby: 42.to_s
来源：http://qt.521024.cn

C#:   42.ToString()
来源：http://lt.panjiajie.cn

[A08] 取整与四舍五入
来源：http://jp.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pu.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://en.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ne.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bl.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kz.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qm.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://re.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pf.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://kj.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://em.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://im.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nz.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aw.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ji.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bq.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cz.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rv.chemitech.net.cn

[A10] 生成随机数
来源：http://ty.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://lh.colortex.cn

PHP:  random_int(1, 100);
来源：http://vr.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sh.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bw.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://do.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mt.hahajie.cn

Ruby: rand(1..100)
来源：http://ma.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://pw.huanxung.cn

[A11] 条件表达式（三元）
来源：http://ap.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://tt.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fc.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://we.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sv.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://rz.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wp.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ua.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uv.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://da.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xm.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ev.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://aa.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://lt.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://gx.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fs.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://zy.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://vt.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mk.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://cu.asd995.cn

PHP:  "第一行\n第二行"
来源：http://dh.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://lw.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://jk.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://ws.nicolike.cn

Go:   "第一行\n第二行"
来源：http://jw.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://wz.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://ud.szsharing.cn

[A14] 注释写法
来源：http://vy.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cz.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hf.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://wo.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://gm.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xj.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://hv.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ml.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://fq.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://mt.asd995.cn

Py:   value = data or "默认值"
来源：http://tv.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://zw.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://sk.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://at.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qx.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://sr.newstarts.cn

Ruby: value = data || "默认值"
来源：http://vm.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://rm.muxihuayi.cn

[A16] 真假值判断规则
来源：http://ia.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bm.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oa.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rv.szsharing.cn

TS:   if (!x) {}
来源：http://vx.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bu.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ac.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bb.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cq.lnxyls.cn

[A17] 位运算
来源：http://rm.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ev.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bs.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sd.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://en.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aa.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tc.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iy.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://oa.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://pw.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://rj.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ah.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wy.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://tz.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nq.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://hh.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://ne.huanxung.cn

[A19] 交换两个变量
来源：http://uw.newstarts.cn

Py:   a, b = b, a
来源：http://sj.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bs.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://ci.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://ax.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ri.haigaiapp.cn

Go:   a, b = b, a
来源：http://wm.szsharing.cn

Ruby: a, b = b, a
来源：http://yq.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://ug.bookmarksfly.cn

[A20] 读取标准输入
来源：http://jn.nszjky.cn

Py:   name = input("请输入：")
来源：http://zk.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yz.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gc.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://rf.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://bt.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://se.szsharing.cn

Ruby: gets.chomp
来源：http://mj.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://iz.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://sg.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://xn.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mz.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://jn.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://gh.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://mo.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jt.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://fq.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://xz.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://bj.wgjwhj.cn

Py:   len(s)
来源：http://gu.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ex.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cb.haigaiapp.cn

TS:   s.length
来源：http://wn.521024.cn

Java: s.length()
来源：http://wy.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://io.huanxung.cn

Ruby: s.length
来源：http://fe.hnjuh.cn

C#:   s.Length
来源：http://lr.haigaiapp.cn

[A23] 大小写转换
来源：http://qo.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yd.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hy.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cu.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lk.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wl.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rm.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dj.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xr.shtwfgs.cn

[A24] 去除首尾空白
来源：http://ok.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://io.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hl.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dr.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kw.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rv.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://jk.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lc.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qi.szsharing.cn

[A25] 字符串比较
来源：http://yo.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://tk.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aa.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qm.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ru.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rk.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bv.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://km.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hw.panjiajie.cn

[A26] 类型转换总览
来源：http://is.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ry.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wt.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bd.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://va.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xj.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xc.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aj.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ey.nicolike.cn

================================================================================
来源：http://rb.chemitech.net.cn

B. 流程控制
来源：http://yj.newstarts.cn

================================================================================
来源：http://up.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://pq.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ww.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://td.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dy.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zu.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sw.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bi.hahajie.cn

[B02] 多分支 else if / elif
来源：http://qs.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qi.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fr.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nm.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iu.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fn.bookmarksfly.cn

[B03] switch / match / case
来源：http://fg.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://le.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sy.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fn.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://no.szsharing.cn


<!-- 参考信息 -->