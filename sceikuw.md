代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mf.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fb.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://to.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wz.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qn.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lf.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qk.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://om.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ra.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yo.huanxung.cn

【文件统计】
来源：http://pd.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xo.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://og.huanxung.cn

目  录
来源：http://ah.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ub.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eo.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://og.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mh.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rg.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dw.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pc.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hc.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dn.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ya.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://li.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rm.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jc.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://da.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://en.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mb.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ti.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pn.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sc.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kt.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dr.wgjwhj.cn

================================================================================
来源：http://ca.hnjuh.cn

A. 基础语法与类型
来源：http://pe.521024.cn

================================================================================
来源：http://xi.bookmarksfly.cn

[A01] Hello World
来源：http://cw.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://xe.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://ky.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://ra.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tv.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://vr.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://uv.colortex.cn

Ruby: puts "Hello, World!"
来源：http://pv.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dm.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://hq.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bh.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://op.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yu.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ia.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://dj.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://ne.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://qu.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oa.jctech888.com.cn

[A03] 常量定义
来源：http://fd.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vw.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://mw.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://xx.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://gb.colortex.cn

Java: static final double PI = 3.14159;
来源：http://ih.colortex.cn

Go:   const PI = 3.14159
来源：http://gr.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://el.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://sy.521024.cn

[A04] 判断变量类型
来源：http://mw.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tr.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://os.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ku.521024.cn

TS:   typeof x; x instanceof Date
来源：http://et.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ow.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pd.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lt.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://vc.yuexingan06.cn

[A05] 整数除法与取模
来源：http://cv.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kb.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://or.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://va.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yb.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://vb.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://pi.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://rz.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://qo.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://oq.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://tw.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zm.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ed.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ds.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jl.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mm.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jv.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ol.shtwfgs.cn

[A07] 数字转字符串
来源：http://kp.nszjky.cn

Py:   str(42)
来源：http://rr.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://wu.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ki.nicolike.cn

TS:   String(42)
来源：http://gc.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wu.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://dg.bookmarksfly.cn

Ruby: 42.to_s
来源：http://lv.shxzskj.cn

C#:   42.ToString()
来源：http://ez.nszjky.cn

[A08] 取整与四舍五入
来源：http://lg.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zb.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ty.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sa.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tr.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gu.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ba.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vq.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ff.asd995.cn

[A09] 绝对值与最大最小值
来源：http://hh.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ak.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qu.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kg.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tb.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://er.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ed.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pw.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://os.nicolike.cn

[A10] 生成随机数
来源：http://vi.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://we.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://zt.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rl.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://az.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://ji.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zb.shxzukj.cn

Ruby: rand(1..100)
来源：http://fs.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://ey.colortex.cn

[A11] 条件表达式（三元）
来源：http://jb.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ut.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ca.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pi.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ug.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://zi.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://et.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wt.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mn.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://rd.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xa.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://md.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://uq.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://fm.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://hd.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bb.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://yu.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://va.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mv.asd995.cn

Py:   "第一行\n第二行"
来源：http://ch.colortex.cn

PHP:  "第一行\n第二行"
来源：http://ta.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://xj.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://bh.colortex.cn

Java: "第一行\n第二行"
来源：http://xc.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://op.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://ff.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://hn.lnxyls.cn

[A14] 注释写法
来源：http://nu.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pj.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xz.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://gy.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://yq.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://za.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://kq.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ao.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://ww.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://pq.panjiajie.cn

Py:   value = data or "默认值"
来源：http://xb.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://ef.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://hi.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://zy.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://om.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://lg.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://jq.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://as.asd995.cn

[A16] 真假值判断规则
来源：http://za.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ot.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://la.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bq.szxytkj.cn

TS:   if (!x) {}
来源：http://wd.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://le.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ic.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kr.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uy.hahajie.cn

[A17] 位运算
来源：http://ld.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zk.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://if.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ao.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vw.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tj.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iy.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bz.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://qq.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://rr.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://rc.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xm.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ar.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://id.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://em.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://by.521024.cn

C#:   (int)'A'; (char)65
来源：http://or.szsharing.cn

[A19] 交换两个变量
来源：http://pk.wgjwhj.cn

Py:   a, b = b, a
来源：http://nd.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ja.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://cu.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://nm.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://pm.huixiangedu.cn

Go:   a, b = b, a
来源：http://dx.nicolike.cn

Ruby: a, b = b, a
来源：http://ju.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://ef.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ib.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://ej.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gn.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://at.521024.cn

TS:   // Node.js：readline 模块
来源：http://gx.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://ki.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vq.wgjwhj.cn

Ruby: gets.chomp
来源：http://ml.521024.cn

C#:   Console.ReadLine();
来源：http://ve.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://uq.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://sm.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wo.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://ko.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://zl.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://ar.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://es.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://qw.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ra.bjjhwx.cn

[A22] 获取字符串长度
来源：http://vv.bookmarksfly.cn

Py:   len(s)
来源：http://xt.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://io.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ei.huixiangedu.cn

TS:   s.length
来源：http://sg.yuexingan06.cn

Java: s.length()
来源：http://kl.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sw.nszjky.cn

Ruby: s.length
来源：http://db.jctech888.com.cn

C#:   s.Length
来源：http://gx.chemitech.net.cn

[A23] 大小写转换
来源：http://sh.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pm.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oi.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://el.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ri.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ge.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xn.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mi.nicolike.cn

[A24] 去除首尾空白
来源：http://ip.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vi.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pi.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uq.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lv.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dv.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://dr.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xi.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://na.nszjky.cn

[A25] 字符串比较
来源：http://ex.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://zd.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wy.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://th.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://er.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mr.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rq.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cg.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://ew.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bc.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bt.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yi.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://io.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fm.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iy.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ax.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yc.panjiajie.cn

================================================================================
来源：http://td.szsharing.cn

B. 流程控制
来源：http://oo.asd995.cn

================================================================================
来源：http://tt.hnjuh.cn

[B01] 条件判断 if / else
来源：http://yx.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vs.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fh.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ik.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fq.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bd.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pi.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gn.newstarts.cn

[B02] 多分支 else if / elif
来源：http://kh.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xf.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tv.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pd.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fu.nszjky.cn

[B03] switch / match / case
来源：http://eo.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kj.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rl.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bg.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://je.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hx.nicolike.cn


<!-- 参考信息 -->