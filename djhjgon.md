代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mr.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xk.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kb.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zc.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://db.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mm.nicolike.cn

【文件统计】
来源：http://zt.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://do.jianghongdianzi.cn

目  录
来源：http://jv.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://wz.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qp.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://br.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ro.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ag.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://di.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uy.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lw.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yv.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xa.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sr.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xr.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dr.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dz.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tj.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cb.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eu.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bg.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dz.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ac.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ke.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ti.jctech888.com.cn

================================================================================
来源：http://vf.hahajie.cn

A. 基础语法与类型
来源：http://tj.wgjwhj.cn

================================================================================
来源：http://ut.colortex.cn

[A01] Hello World
来源：http://if.szxytkj.cn

Py:   print("Hello, World!")
来源：http://hj.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://gd.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://ow.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tj.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://tm.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://on.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://fw.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wa.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://mz.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jb.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dn.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rt.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ul.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://rd.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://sb.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://nl.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cl.shxzukj.cn

[A03] 常量定义
来源：http://qx.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kl.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://sx.hahajie.cn

JS:   const PI = 3.14159;
来源：http://hd.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://hn.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://ix.gzmigu.cn

Go:   const PI = 3.14159
来源：http://cm.521024.cn

Ruby: PI = 3.14159
来源：http://ii.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://aj.szxytkj.cn

[A04] 判断变量类型
来源：http://nm.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hm.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hm.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bh.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://yx.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://na.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nb.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dx.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://gt.muxihuayi.cn

[A05] 整数除法与取模
来源：http://te.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sa.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bv.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kf.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uf.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://az.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://im.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://eu.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://hs.521024.cn

[A06] 字符串转数字
来源：http://mr.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://zz.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gp.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jq.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ix.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tb.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rs.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yv.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sf.shxzskj.cn

[A07] 数字转字符串
来源：http://ma.bjjhwx.cn

Py:   str(42)
来源：http://rf.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://ol.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://tp.hnjuh.cn

TS:   String(42)
来源：http://nq.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hh.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://ou.9csxet.cn

Ruby: 42.to_s
来源：http://yd.shtwfgs.cn

C#:   42.ToString()
来源：http://bd.shxzskj.cn

[A08] 取整与四舍五入
来源：http://ht.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://av.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://go.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vr.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bf.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hk.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ge.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rj.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sf.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://go.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://go.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://an.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://it.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mk.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ra.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ln.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pz.asd995.cn

[A10] 生成随机数
来源：http://ae.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://qq.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://bs.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fb.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wo.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://ab.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://br.jctech888.com.cn

Ruby: rand(1..100)
来源：http://xc.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://co.nicolike.cn

[A11] 条件表达式（三元）
来源：http://bl.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://jn.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bt.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eb.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wv.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ot.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wd.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zy.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://az.521024.cn

[A12] 字符串插值 / 格式化
来源：http://te.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xj.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://an.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://it.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ru.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://bj.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mc.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://oe.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://rf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://en.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://be.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://ay.huanxung.cn

JS:   "第一行\n第二行"
来源：http://nq.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://cs.huanxung.cn

Java: "第一行\n第二行"
来源：http://mq.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://bp.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://hi.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://nn.nszjky.cn

[A14] 注释写法
来源：http://os.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://po.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yq.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://xn.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://xd.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nr.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://dk.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hd.521024.cn

C#:   // 单行；/* 多行 */
来源：http://ik.521024.cn

[A15] 空值判断与默认值
来源：http://hg.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://zo.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://yb.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://oo.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://ae.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://is.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://wx.521024.cn

Ruby: value = data || "默认值"
来源：http://zm.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://mp.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://qx.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fr.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dq.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bz.huanxung.cn

TS:   if (!x) {}
来源：http://hn.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rh.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vp.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tk.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aq.jianghongdianzi.cn

[A17] 位运算
来源：http://zb.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ix.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bx.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fa.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gr.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://md.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fj.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zl.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://se.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://ps.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://fn.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ya.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ka.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://mv.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uo.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://db.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://oc.nszjky.cn

[A19] 交换两个变量
来源：http://eo.9csxet.cn

Py:   a, b = b, a
来源：http://zp.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://if.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://tz.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://hr.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://os.haigaiapp.cn

Go:   a, b = b, a
来源：http://hx.huanxung.cn

Ruby: a, b = b, a
来源：http://wn.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://zt.gzmigu.cn

[A20] 读取标准输入
来源：http://hy.shxzukj.cn

Py:   name = input("请输入：")
来源：http://my.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rt.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hr.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ap.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://zu.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pz.chemitech.net.cn

Ruby: gets.chomp
来源：http://uq.hnjuh.cn

C#:   Console.ReadLine();
来源：http://mn.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://hn.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://zf.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gl.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://sk.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://jz.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://dq.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cp.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://ae.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://mh.muxihuayi.cn

[A22] 获取字符串长度
来源：http://su.shxzukj.cn

Py:   len(s)
来源：http://fg.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mb.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ki.bookmarksfly.cn

TS:   s.length
来源：http://bp.jctech888.com.cn

Java: s.length()
来源：http://by.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lb.shtwfgs.cn

Ruby: s.length
来源：http://mb.nszjky.cn

C#:   s.Length
来源：http://bp.shtwfgs.cn

[A23] 大小写转换
来源：http://cp.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oe.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xx.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://li.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gd.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cp.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ku.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sm.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://he.nicolike.cn

[A24] 去除首尾空白
来源：http://rn.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nn.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uf.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iy.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jg.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yg.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://zd.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xy.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bt.shxzukj.cn

[A25] 字符串比较
来源：http://qn.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://ht.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://av.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wd.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vz.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sd.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wy.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tf.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yf.asd995.cn

[A26] 类型转换总览
来源：http://sp.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ty.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rt.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ng.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ma.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xn.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dz.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nk.lnxyls.cn

================================================================================
来源：http://xs.nicolike.cn

B. 流程控制
来源：http://pi.wgjwhj.cn

================================================================================
来源：http://pm.9csxet.cn

[B01] 条件判断 if / else
来源：http://ip.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ht.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tc.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tb.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cj.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vw.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ej.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ex.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lk.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://fp.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://du.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ep.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kg.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hs.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dp.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rs.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lx.colortex.cn

[B03] switch / match / case
来源：http://ok.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ko.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://he.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://og.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hl.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gp.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sg.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pi.jianghongdianzi.cn

[B04] for 计数循环
来源：http://tm.haigaiapp.cn


<!-- 参考信息 -->