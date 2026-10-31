代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xb.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bv.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://du.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sk.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yb.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nz.shtwfgs.cn

【文件统计】
来源：http://mp.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uq.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://au.bookmarksfly.cn

目  录
来源：http://vt.asd995.cn

--------------------------------------------------------------------------------
来源：http://he.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://js.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rp.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ik.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vk.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jl.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ob.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gb.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bz.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bg.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qp.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zf.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vx.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xj.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tt.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dh.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zq.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qi.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rh.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ov.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tj.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pf.asd995.cn

================================================================================
来源：http://we.hahajie.cn

A. 基础语法与类型
来源：http://im.yuexingan06.cn

================================================================================
来源：http://ei.huanxung.cn

[A01] Hello World
来源：http://lq.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://qg.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://ci.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://lp.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lo.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://bz.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://ro.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://dc.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cv.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://ag.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ew.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ca.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ur.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ks.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://po.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://iv.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://ju.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wa.shxzukj.cn

[A03] 常量定义
来源：http://hs.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://br.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://nm.521024.cn

JS:   const PI = 3.14159;
来源：http://lc.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://lk.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://nt.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://yq.nszjky.cn

Ruby: PI = 3.14159
来源：http://ai.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://oq.asd995.cn

[A04] 判断变量类型
来源：http://pe.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tq.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ub.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dm.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://ms.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xg.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eo.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ox.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://oz.bjjhwx.cn

[A05] 整数除法与取模
来源：http://ro.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yx.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yw.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://be.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jl.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://ee.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://ek.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://ej.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://gp.colortex.cn

[A06] 字符串转数字
来源：http://wx.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://nu.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nm.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iy.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pl.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ew.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ax.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kb.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mq.hnjuh.cn

[A07] 数字转字符串
来源：http://zw.huanxung.cn

Py:   str(42)
来源：http://fu.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://zk.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://ar.shxzskj.cn

TS:   String(42)
来源：http://du.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://va.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://eg.bookmarksfly.cn

Ruby: 42.to_s
来源：http://do.panjiajie.cn

C#:   42.ToString()
来源：http://ay.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://ic.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kv.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yz.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vb.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rq.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wj.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ez.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ft.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ih.521024.cn

[A09] 绝对值与最大最小值
来源：http://hf.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zt.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qu.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pj.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xo.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rg.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qb.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xi.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xc.nicolike.cn

[A10] 生成随机数
来源：http://wp.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://ok.newstarts.cn

PHP:  random_int(1, 100);
来源：http://uv.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dx.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sv.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://hh.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nx.shtwfgs.cn

Ruby: rand(1..100)
来源：http://gw.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://vu.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ia.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://sa.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://do.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://un.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yj.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://pg.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fx.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fv.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tw.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://vz.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ib.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://he.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://it.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://lx.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://vw.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://un.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://dg.521024.cn

C#:   $"Hello, {name}!"
来源：http://fu.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hu.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://aw.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://iz.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://xt.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://cs.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://it.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://er.521024.cn

Ruby: "第一行\n第二行"
来源：http://tk.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://gm.newstarts.cn

[A14] 注释写法
来源：http://cm.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jl.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rl.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://xv.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://gw.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://au.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://zn.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://je.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ml.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://qr.hahajie.cn

Py:   value = data or "默认值"
来源：http://jf.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ot.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://tz.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://su.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mz.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ku.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ng.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://xa.haigaiapp.cn

[A16] 真假值判断规则
来源：http://rc.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ga.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://et.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aw.jctech888.com.cn

TS:   if (!x) {}
来源：http://cb.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qf.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eb.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pf.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ld.521024.cn

[A17] 位运算
来源：http://ab.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ia.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zf.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fw.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cm.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://th.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://kq.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://yw.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://bd.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kz.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bg.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://vq.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rg.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ai.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://ma.521024.cn

[A19] 交换两个变量
来源：http://gq.haigaiapp.cn

Py:   a, b = b, a
来源：http://nh.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lr.521024.cn

JS:   [a, b] = [b, a];
来源：http://ho.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://nu.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://iy.bookmarksfly.cn

Go:   a, b = b, a
来源：http://ks.panjiajie.cn

Ruby: a, b = b, a
来源：http://bv.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://dc.bookmarksfly.cn

[A20] 读取标准输入
来源：http://tr.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://ys.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ap.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dn.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://uh.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://mw.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://le.huanxung.cn

Ruby: gets.chomp
来源：http://oc.hnjuh.cn

C#:   Console.ReadLine();
来源：http://kf.newstarts.cn

[A21] 保留指定小数位输出
来源：http://kv.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://da.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://td.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://hr.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://gl.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://da.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oy.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://wt.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://lc.9csxet.cn

[A22] 获取字符串长度
来源：http://mr.521024.cn

Py:   len(s)
来源：http://ij.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hb.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://np.asd995.cn

TS:   s.length
来源：http://un.nszjky.cn

Java: s.length()
来源：http://vd.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wp.nicolike.cn

Ruby: s.length
来源：http://bt.bookmarksfly.cn

C#:   s.Length
来源：http://fd.newstarts.cn

[A23] 大小写转换
来源：http://wl.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oj.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ka.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tv.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cc.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ia.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cf.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ra.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lk.colortex.cn

[A24] 去除首尾空白
来源：http://vn.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mj.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rg.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ui.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://db.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://am.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aq.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vr.9csxet.cn

[A25] 字符串比较
来源：http://jx.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://jq.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oe.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xk.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qb.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vo.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ci.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pj.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oy.muxihuayi.cn

[A26] 类型转换总览
来源：http://oh.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ne.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gz.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dg.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://rj.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pz.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qc.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rh.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lz.panjiajie.cn

================================================================================
来源：http://yw.hahajie.cn

B. 流程控制
来源：http://xa.muxihuayi.cn

================================================================================
来源：http://lk.hnjuh.cn

[B01] 条件判断 if / else
来源：http://pe.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fu.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aa.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ys.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://md.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yd.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qw.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hs.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ja.colortex.cn

[B02] 多分支 else if / elif
来源：http://bc.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://em.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tp.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jk.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xp.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hl.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mi.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.yuexingan06.cn

[B03] switch / match / case
来源：http://va.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fl.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mk.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://az.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fh.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pp.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iy.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xc.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ea.jianghongdianzi.cn

[B04] for 计数循环
来源：http://js.yuexingan06.cn


<!-- 参考信息 -->