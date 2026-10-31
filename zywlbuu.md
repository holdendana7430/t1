代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://if.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zv.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://co.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hs.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jq.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://on.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xh.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ka.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ni.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vf.muxihuayi.cn

【文件统计】
来源：http://hh.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gs.colortex.cn

--------------------------------------------------------------------------------
来源：http://cn.shxzskj.cn

目  录
来源：http://so.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://vg.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jd.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vo.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jh.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://at.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mx.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ls.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wf.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://st.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rl.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lw.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rl.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dq.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rz.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uc.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lp.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://me.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wy.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sw.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xi.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gd.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://br.jctech888.com.cn

================================================================================
来源：http://ha.haigaiapp.cn

A. 基础语法与类型
来源：http://lf.wgjwhj.cn

================================================================================
来源：http://es.hahajie.cn

[A01] Hello World
来源：http://wp.panjiajie.cn

Py:   print("Hello, World!")
来源：http://ej.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://hk.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://rv.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zf.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://mx.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://sr.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://sk.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sl.hnjuh.cn

[A02] 变量声明与赋值
来源：http://ol.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://we.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hg.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ch.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://op.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://ey.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://mb.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://vr.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://it.bookmarksfly.cn

[A03] 常量定义
来源：http://jm.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uk.521024.cn

PHP:  const PI = 3.14159;
来源：http://ru.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://wh.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://re.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://tv.shxzskj.cn

Go:   const PI = 3.14159
来源：http://am.nicolike.cn

Ruby: PI = 3.14159
来源：http://nd.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://vt.521024.cn

[A04] 判断变量类型
来源：http://qx.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ul.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yu.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wz.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://xt.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://am.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://af.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yk.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://pq.asd995.cn

[A05] 整数除法与取模
来源：http://qs.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zx.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ua.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tn.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ok.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://ak.521024.cn

Go:   7 / 2; 7 % 2
来源：http://ck.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://nm.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://pm.shtwfgs.cn

[A06] 字符串转数字
来源：http://bb.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://ri.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ak.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vr.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dj.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xb.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://im.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xo.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ua.muxihuayi.cn

[A07] 数字转字符串
来源：http://wj.szsharing.cn

Py:   str(42)
来源：http://cr.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://qh.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://bo.lnxyls.cn

TS:   String(42)
来源：http://ca.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bq.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://vc.wgjwhj.cn

Ruby: 42.to_s
来源：http://yt.huanxung.cn

C#:   42.ToString()
来源：http://nx.huanxung.cn

[A08] 取整与四舍五入
来源：http://jm.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qg.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oc.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ez.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uj.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bp.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tn.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yf.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mc.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://xr.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nc.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://io.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qn.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://en.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ql.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lq.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://er.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fa.panjiajie.cn

[A10] 生成随机数
来源：http://ys.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://qk.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://rz.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sv.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vt.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://xp.chemitech.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mu.521024.cn

Ruby: rand(1..100)
来源：http://xm.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://sa.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://vr.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://zo.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vo.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gj.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nf.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://iq.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hb.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sl.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://co.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://at.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fu.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ry.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://ax.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://py.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://kf.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wy.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://gw.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://bf.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nw.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://wy.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://zi.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://he.9csxet.cn

TS:   "第一行\n第二行"
来源：http://ig.szxytkj.cn

Java: "第一行\n第二行"
来源：http://pp.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://fy.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://kp.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://ip.nicolike.cn

[A14] 注释写法
来源：http://li.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xo.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kt.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://nu.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://jo.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ms.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://dd.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yp.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://bx.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://wj.521024.cn

Py:   value = data or "默认值"
来源：http://rd.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://xb.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://mb.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://nf.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yw.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://pa.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ad.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://rc.huixiangedu.cn

[A16] 真假值判断规则
来源：http://vx.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wj.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yb.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://de.bjjhwx.cn

TS:   if (!x) {}
来源：http://rt.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ra.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aa.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bk.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xd.panjiajie.cn

[A17] 位运算
来源：http://fc.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fd.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ss.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hg.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wk.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hh.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ns.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fq.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://kp.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://go.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://lr.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ou.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hq.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://ho.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zz.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://zp.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://ck.szxytkj.cn

[A19] 交换两个变量
来源：http://xu.huanxung.cn

Py:   a, b = b, a
来源：http://dp.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ib.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://le.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://kq.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://bc.lnxyls.cn

Go:   a, b = b, a
来源：http://kv.shxzukj.cn

Ruby: a, b = b, a
来源：http://gw.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://di.bjjhwx.cn

[A20] 读取标准输入
来源：http://el.gzmigu.cn

Py:   name = input("请输入：")
来源：http://vh.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ej.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sj.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://dl.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://wi.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jg.nicolike.cn

Ruby: gets.chomp
来源：http://wn.newstarts.cn

C#:   Console.ReadLine();
来源：http://ic.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ic.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://mr.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rh.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://vq.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://fm.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://xh.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jp.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://jx.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://sc.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://mb.muxihuayi.cn

Py:   len(s)
来源：http://yq.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ss.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ii.szxytkj.cn

TS:   s.length
来源：http://ki.asd995.cn

Java: s.length()
来源：http://ay.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bh.521024.cn

Ruby: s.length
来源：http://nv.szsharing.cn

C#:   s.Length
来源：http://ma.shxzskj.cn

[A23] 大小写转换
来源：http://td.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fe.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aw.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uk.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jl.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hp.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zo.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fo.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://el.colortex.cn

[A24] 去除首尾空白
来源：http://vo.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qg.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ra.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cb.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rv.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ss.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://se.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ex.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zi.muxihuayi.cn

[A25] 字符串比较
来源：http://vj.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://gd.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jr.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://el.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sr.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wn.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yc.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ym.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://cr.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pq.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ik.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jc.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://jd.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://to.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ph.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dz.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jt.lnxyls.cn

================================================================================
来源：http://ry.huixiangedu.cn

B. 流程控制
来源：http://iu.bookmarksfly.cn

================================================================================
来源：http://wd.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://ub.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ec.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vm.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://je.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dj.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bz.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rg.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hx.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://wm.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rr.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://st.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bc.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pz.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zt.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lg.muxihuayi.cn

[B03] switch / match / case
来源：http://iu.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mi.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nn.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://co.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fo.nszjky.cn


<!-- 参考信息 -->