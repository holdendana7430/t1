代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kt.yuntaijiaju.cn

【使用说明】
来源：http://xz.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tr.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uz.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ya.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ma.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ei.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mx.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xe.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hw.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zf.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ye.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nv.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://db.9csxet.cn

【文件统计】
来源：http://aq.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://od.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://rv.hahajie.cn

目  录
来源：http://ka.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://yt.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vu.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wg.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vh.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ar.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://np.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gv.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xq.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kw.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qh.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pz.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zl.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mv.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sy.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ra.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rk.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ie.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tg.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jf.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wu.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xu.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xd.wgjwhj.cn

================================================================================
来源：http://mx.shxzskj.cn

A. 基础语法与类型
来源：http://ai.lnxyls.cn

================================================================================
来源：http://ri.huixiangedu.cn

[A01] Hello World
来源：http://di.shxzukj.cn

Py:   print("Hello, World!")
来源：http://wb.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://ad.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://jb.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ua.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://tx.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://zb.asd995.cn

Ruby: puts "Hello, World!"
来源：http://cf.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uz.lnxyls.cn

[A02] 变量声明与赋值
来源：http://gf.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eu.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fb.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sa.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yk.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://hb.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://nz.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://zv.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mm.muxihuayi.cn

[A03] 常量定义
来源：http://br.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rj.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://kt.nicolike.cn

JS:   const PI = 3.14159;
来源：http://td.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://al.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://lp.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://wx.newstarts.cn

Ruby: PI = 3.14159
来源：http://pu.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://co.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://ao.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zs.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ms.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://se.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://ey.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uv.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tl.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uf.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://re.hahajie.cn

[A05] 整数除法与取模
来源：http://la.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wl.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vv.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vc.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vl.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://xq.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://ns.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://bp.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ke.jctech888.com.cn

[A06] 字符串转数字
来源：http://rl.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://eo.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hw.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ta.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hi.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kh.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vc.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ot.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vl.huanxung.cn

[A07] 数字转字符串
来源：http://rs.szsharing.cn

Py:   str(42)
来源：http://ey.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://pr.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://pf.shtwfgs.cn

TS:   String(42)
来源：http://cu.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pe.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://kg.hahajie.cn

Ruby: 42.to_s
来源：http://wo.jctech888.com.cn

C#:   42.ToString()
来源：http://jf.asd995.cn

[A08] 取整与四舍五入
来源：http://qu.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ta.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qk.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nh.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xf.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uo.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ho.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dd.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iu.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://ro.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://me.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rc.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dy.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ub.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ah.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ur.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zw.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vf.newstarts.cn

[A10] 生成随机数
来源：http://fc.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://mq.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://vu.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://by.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ld.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://mv.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xp.huixiangedu.cn

Ruby: rand(1..100)
来源：http://xc.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://qv.asd995.cn

[A11] 条件表达式（三元）
来源：http://ul.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://ja.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sc.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jm.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://is.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://vc.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jy.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://up.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ul.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://gr.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gj.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uo.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://op.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://iu.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://ch.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://za.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://ls.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://kd.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hd.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://xx.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://lr.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://yr.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://hj.hnjuh.cn

Java: "第一行\n第二行"
来源：http://jy.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://el.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://bt.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://hc.shtwfgs.cn

[A14] 注释写法
来源：http://lw.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://li.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gf.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://yr.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://vb.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fp.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://bl.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://il.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://jg.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://ex.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://ey.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://kk.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://yt.521024.cn

TS:   const value = data ?? "默认值";
来源：http://bj.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://on.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://ho.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ax.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://vp.panjiajie.cn

[A16] 真假值判断规则
来源：http://vt.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iu.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eh.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iz.shxzskj.cn

TS:   if (!x) {}
来源：http://md.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ww.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sh.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vr.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://di.9csxet.cn

[A17] 位运算
来源：http://xs.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hc.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fd.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fn.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dc.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pr.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nl.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://si.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://at.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://aa.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://hp.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bl.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yj.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://pr.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gy.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://fe.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://zb.nicolike.cn

[A19] 交换两个变量
来源：http://yw.hahajie.cn

Py:   a, b = b, a
来源：http://pm.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lx.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://gm.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://wu.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://ug.jctech888.com.cn

Go:   a, b = b, a
来源：http://dt.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://km.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://yz.colortex.cn

[A20] 读取标准输入
来源：http://jv.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://dh.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rl.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wy.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://qw.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ck.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jy.newstarts.cn

Ruby: gets.chomp
来源：http://pc.521024.cn

C#:   Console.ReadLine();
来源：http://ss.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://uh.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://cw.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jo.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://yd.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://pf.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://ww.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lb.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://jq.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://wj.newstarts.cn

[A22] 获取字符串长度
来源：http://wu.wgjwhj.cn

Py:   len(s)
来源：http://eq.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wz.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ja.shtwfgs.cn

TS:   s.length
来源：http://mn.newstarts.cn

Java: s.length()
来源：http://jz.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ax.asd995.cn

Ruby: s.length
来源：http://xp.shxzukj.cn

C#:   s.Length
来源：http://za.panjiajie.cn

[A23] 大小写转换
来源：http://ae.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tp.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ad.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ih.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://io.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ne.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://is.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zi.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ng.9csxet.cn

[A24] 去除首尾空白
来源：http://og.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nu.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ic.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gk.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yy.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uc.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://cw.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ox.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://li.nicolike.cn

[A25] 字符串比较
来源：http://sd.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://gu.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://th.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ds.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xp.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uy.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sl.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ln.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uz.haigaiapp.cn

[A26] 类型转换总览
来源：http://uq.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xw.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lp.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qn.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://xd.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pg.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://za.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dc.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yg.hnjuh.cn

================================================================================
来源：http://ee.521024.cn

B. 流程控制
来源：http://xb.szxytkj.cn

================================================================================
来源：http://up.gzmigu.cn

[B01] 条件判断 if / else
来源：http://pc.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nt.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://og.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yp.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oc.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wi.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://po.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://de.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bc.521024.cn

[B02] 多分支 else if / elif
来源：http://ek.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uz.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xt.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jx.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fj.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nc.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hg.shtwfgs.cn

[B03] switch / match / case
来源：http://to.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xm.jctech888.com.cn


<!-- 参考信息 -->