代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ly.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rf.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yt.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fw.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uv.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zg.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jo.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qf.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qq.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iv.colortex.cn

【文件统计】
来源：http://td.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wv.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://xg.panjiajie.cn

目  录
来源：http://ry.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://fb.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://io.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nm.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wu.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://va.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kr.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lv.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pz.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://id.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ct.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ro.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vw.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lu.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fb.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zw.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ml.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ux.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xf.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xn.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tg.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ur.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ez.wgjwhj.cn

================================================================================
来源：http://fl.shtwfgs.cn

A. 基础语法与类型
来源：http://vz.nszjky.cn

================================================================================
来源：http://jx.newstarts.cn

[A01] Hello World
来源：http://ht.shxzukj.cn

Py:   print("Hello, World!")
来源：http://je.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://zg.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://os.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jz.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://sm.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://zy.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://hy.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://og.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://sa.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vx.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jq.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ad.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wc.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://ov.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://no.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://re.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yt.szxytkj.cn

[A03] 常量定义
来源：http://cc.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mc.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://am.newstarts.cn

JS:   const PI = 3.14159;
来源：http://ng.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://te.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://ca.9csxet.cn

Go:   const PI = 3.14159
来源：http://fk.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://go.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://ax.hnjuh.cn

[A04] 判断变量类型
来源：http://ca.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oz.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fy.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lc.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://ku.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ei.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rf.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pa.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ok.shtwfgs.cn

[A05] 整数除法与取模
来源：http://eg.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://la.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://br.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bb.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ls.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://ii.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://am.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ik.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://gb.bookmarksfly.cn

[A06] 字符串转数字
来源：http://bc.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://js.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zb.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jg.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gs.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mu.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ji.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zl.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ju.wgjwhj.cn

[A07] 数字转字符串
来源：http://gc.bjjhwx.cn

Py:   str(42)
来源：http://zt.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://pk.nszjky.cn

JS:   String(42); (42).toString()
来源：http://am.hahajie.cn

TS:   String(42)
来源：http://hp.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://do.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://ww.lnxyls.cn

Ruby: 42.to_s
来源：http://xz.asd995.cn

C#:   42.ToString()
来源：http://er.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://dx.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cd.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nr.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cp.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jm.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://di.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lj.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fv.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ii.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ud.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vv.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jt.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://la.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ih.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xq.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wd.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://co.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tn.chemitech.net.cn

[A10] 生成随机数
来源：http://qp.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://jn.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ni.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://do.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oc.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ly.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ln.asd995.cn

Ruby: rand(1..100)
来源：http://iy.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://vh.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://jy.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://xw.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yr.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sw.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rm.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://fr.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ra.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gg.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fm.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://cq.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://za.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qr.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://sx.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://zr.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://vp.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eu.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://zm.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://sk.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://id.nicolike.cn

Py:   "第一行\n第二行"
来源：http://zn.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://lr.asd995.cn

JS:   "第一行\n第二行"
来源：http://jj.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://ho.asd995.cn

Java: "第一行\n第二行"
来源：http://zb.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://yb.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://rt.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://yj.gzmigu.cn

[A14] 注释写法
来源：http://tz.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://et.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qv.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://na.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://ep.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zv.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://yz.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ja.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ic.szsharing.cn

[A15] 空值判断与默认值
来源：http://ay.asd995.cn

Py:   value = data or "默认值"
来源：http://tr.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://et.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://tf.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://mr.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rz.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://fn.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://xa.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://ue.shxzskj.cn

[A16] 真假值判断规则
来源：http://vx.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fk.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ao.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://su.muxihuayi.cn

TS:   if (!x) {}
来源：http://tv.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bb.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ii.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qa.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eh.huixinmuqiang.cn

[A17] 位运算
来源：http://jo.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dy.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://px.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lw.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cb.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hx.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yp.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dr.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://yf.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://ug.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://nr.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gw.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://td.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wd.521024.cn

Ruby: "A".ord; 65.chr
来源：http://ae.521024.cn

C#:   (int)'A'; (char)65
来源：http://yp.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://wy.haigaiapp.cn

Py:   a, b = b, a
来源：http://co.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yt.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://ml.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://bf.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://ej.shxzukj.cn

Go:   a, b = b, a
来源：http://xr.hahajie.cn

Ruby: a, b = b, a
来源：http://sr.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://cv.szsharing.cn

[A20] 读取标准输入
来源：http://hc.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://cf.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fs.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ab.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://wv.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://wu.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://py.szxytkj.cn

Ruby: gets.chomp
来源：http://bm.gzmigu.cn

C#:   Console.ReadLine();
来源：http://dr.521024.cn

[A21] 保留指定小数位输出
来源：http://ao.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://po.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ge.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://ik.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://ju.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://ji.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vm.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://oq.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://cx.hnjuh.cn

[A22] 获取字符串长度
来源：http://mg.shxzukj.cn

Py:   len(s)
来源：http://ei.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://io.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://em.hahajie.cn

TS:   s.length
来源：http://wx.lnxyls.cn

Java: s.length()
来源：http://he.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://py.lnxyls.cn

Ruby: s.length
来源：http://rk.huixiangedu.cn

C#:   s.Length
来源：http://cl.jctech888.com.cn

[A23] 大小写转换
来源：http://qc.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vl.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wb.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vo.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jx.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zq.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zo.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kf.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lm.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://xs.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ym.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dz.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zu.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hu.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wd.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://si.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ru.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ti.yuntaijiaju.cn

[A25] 字符串比较
来源：http://vv.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://rp.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ky.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://no.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dx.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gs.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hn.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hx.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ou.nicolike.cn

[A26] 类型转换总览
来源：http://yh.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fd.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ya.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nn.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://wr.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sr.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ob.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wm.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zm.nszjky.cn

================================================================================
来源：http://tp.hahajie.cn

B. 流程控制
来源：http://nf.asd995.cn

================================================================================
来源：http://rr.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ay.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ch.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ym.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ig.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gl.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jt.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gy.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cw.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pe.521024.cn

[B02] 多分支 else if / elif
来源：http://eq.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zj.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ep.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qi.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nd.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ie.muxihuayi.cn

[B03] switch / match / case
来源：http://sj.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xk.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iv.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vb.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vu.shxzskj.cn


<!-- 参考信息 -->