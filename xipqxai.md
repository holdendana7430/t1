代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vi.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bc.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aq.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ot.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zk.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jm.hnjuh.cn

【文件统计】
来源：http://ul.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tv.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ej.521024.cn

目  录
来源：http://hq.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://kt.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ga.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bb.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lx.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kw.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zt.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wm.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://se.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wz.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ii.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ax.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lb.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bw.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lm.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zv.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oy.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://or.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lo.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://is.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ol.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xt.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://un.yuntaijiaju.cn

================================================================================
来源：http://ap.newstarts.cn

A. 基础语法与类型
来源：http://fb.wgjwhj.cn

================================================================================
来源：http://il.521024.cn

[A01] Hello World
来源：http://ju.9csxet.cn

Py:   print("Hello, World!")
来源：http://zz.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ia.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://qz.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ak.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://ok.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://vp.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://io.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ze.szsharing.cn

[A02] 变量声明与赋值
来源：http://mx.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hd.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kp.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tc.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vd.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://xm.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://gs.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://fr.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vx.yuntaijiaju.cn

[A03] 常量定义
来源：http://jr.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fh.asd995.cn

PHP:  const PI = 3.14159;
来源：http://er.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://ce.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://jm.colortex.cn

Java: static final double PI = 3.14159;
来源：http://uw.9csxet.cn

Go:   const PI = 3.14159
来源：http://qq.asd995.cn

Ruby: PI = 3.14159
来源：http://px.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ou.huanxung.cn

[A04] 判断变量类型
来源：http://tl.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zy.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yj.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kf.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://ip.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fy.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://na.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ol.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://fd.panjiajie.cn

[A05] 整数除法与取模
来源：http://xt.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wf.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ad.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bm.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oe.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://dc.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://oe.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://sa.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://kc.panjiajie.cn

[A06] 字符串转数字
来源：http://ik.asd995.cn

Py:   int("42"); float("3.14")
来源：http://pk.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xr.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kc.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ht.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wu.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zo.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hx.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jy.hahajie.cn

[A07] 数字转字符串
来源：http://hr.panjiajie.cn

Py:   str(42)
来源：http://gb.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://na.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://yd.shxzskj.cn

TS:   String(42)
来源：http://gt.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://er.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://hb.hahajie.cn

Ruby: 42.to_s
来源：http://ji.huanxung.cn

C#:   42.ToString()
来源：http://ek.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://aw.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kk.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xd.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://so.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ci.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zh.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yf.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zq.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wn.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://sp.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vr.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fy.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://og.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qn.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ib.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://el.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sk.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hy.newstarts.cn

[A10] 生成随机数
来源：http://du.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://jc.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://rc.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lr.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ma.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://mm.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kv.haigaiapp.cn

Ruby: rand(1..100)
来源：http://xr.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://vz.huanxung.cn

[A11] 条件表达式（三元）
来源：http://ry.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://wl.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nn.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rx.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cw.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://lo.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ux.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ai.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wf.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://yc.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vq.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uq.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://mv.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://za.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://vo.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kn.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://se.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://kz.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dh.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://yj.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://cb.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://af.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://xh.shxzukj.cn

Java: "第一行\n第二行"
来源：http://mg.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://wu.colortex.cn

Ruby: "第一行\n第二行"
来源：http://cp.9csxet.cn

C#:   "第一行\n第二行"
来源：http://kl.shxzskj.cn

[A14] 注释写法
来源：http://rn.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lq.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nm.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://rt.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://iv.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wt.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://sy.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gl.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://mu.panjiajie.cn

[A15] 空值判断与默认值
来源：http://zo.szxytkj.cn

Py:   value = data or "默认值"
来源：http://mn.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://fv.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://wt.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://fx.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bl.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://ar.9csxet.cn

Ruby: value = data || "默认值"
来源：http://kr.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://tt.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://sb.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wl.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mj.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fl.panjiajie.cn

TS:   if (!x) {}
来源：http://od.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mi.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uc.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wv.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eq.haigaiapp.cn

[A17] 位运算
来源：http://mx.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hw.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://da.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yp.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dt.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://td.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wc.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://bs.asd995.cn

Py:   ord("A"); chr(65)
来源：http://kl.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://da.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yl.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://aw.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ml.521024.cn

Ruby: "A".ord; 65.chr
来源：http://nn.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ui.haigaiapp.cn

[A19] 交换两个变量
来源：http://zg.szsharing.cn

Py:   a, b = b, a
来源：http://go.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cw.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://zi.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://uk.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://eu.haigaiapp.cn

Go:   a, b = b, a
来源：http://sg.521024.cn

Ruby: a, b = b, a
来源：http://mm.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://lo.yuexingan06.cn

[A20] 读取标准输入
来源：http://gc.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://ka.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://un.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ve.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://cz.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://tn.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uc.chemitech.net.cn

Ruby: gets.chomp
来源：http://rc.hahajie.cn

C#:   Console.ReadLine();
来源：http://du.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://zg.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://ju.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jq.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://se.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://fn.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://tw.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zl.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://br.521024.cn

C#:   3.14159.ToString("F2")
来源：http://ew.521024.cn

[A22] 获取字符串长度
来源：http://qy.newstarts.cn

Py:   len(s)
来源：http://at.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nr.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jx.asd995.cn

TS:   s.length
来源：http://jw.9csxet.cn

Java: s.length()
来源：http://oz.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://te.newstarts.cn

Ruby: s.length
来源：http://zq.nicolike.cn

C#:   s.Length
来源：http://hm.yuntaijiaju.cn

[A23] 大小写转换
来源：http://zg.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rl.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eh.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pe.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cf.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jp.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wh.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cu.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ok.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://hc.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aw.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sh.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ir.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ls.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://nl.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tn.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ar.hnjuh.cn

[A25] 字符串比较
来源：http://yc.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://lr.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cu.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cv.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lz.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qp.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rr.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ow.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nw.shxzskj.cn

[A26] 类型转换总览
来源：http://cz.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gh.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ry.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yy.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://vv.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vh.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nj.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://am.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ie.jctech888.com.cn

================================================================================
来源：http://tl.jctech888.com.cn

B. 流程控制
来源：http://cw.521024.cn

================================================================================
来源：http://bl.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://kr.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uv.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nn.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cf.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wd.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hl.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bd.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yd.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tu.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://pe.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://he.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ah.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://au.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zh.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mo.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.wgjwhj.cn

[B03] switch / match / case
来源：http://tn.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uy.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rs.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nn.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vn.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qf.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://py.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gv.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oa.shxzukj.cn

[B04] for 计数循环
来源：http://fa.gzmigu.cn


<!-- 参考信息 -->