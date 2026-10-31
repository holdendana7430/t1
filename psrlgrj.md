代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dn.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fr.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yh.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xx.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qu.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xd.huixinmuqiang.cn

【文件统计】
来源：http://pl.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://te.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://kt.huanxung.cn

目  录
来源：http://ag.asd995.cn

--------------------------------------------------------------------------------
来源：http://it.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ez.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wm.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qe.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sq.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dg.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uc.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wv.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://az.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vc.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sg.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nn.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gx.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://no.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://me.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ab.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cv.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xh.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ht.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fl.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hs.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oc.bookmarksfly.cn

================================================================================
来源：http://sl.hahajie.cn

A. 基础语法与类型
来源：http://fm.nicolike.cn

================================================================================
来源：http://ho.muxihuayi.cn

[A01] Hello World
来源：http://ww.gzmigu.cn

Py:   print("Hello, World!")
来源：http://zw.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://hk.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://qg.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://me.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://yg.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://qd.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://jr.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bh.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://vz.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vc.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ga.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rf.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://im.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://gv.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://vi.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://fd.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qa.bjjhwx.cn

[A03] 常量定义
来源：http://in.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://he.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://is.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://if.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://qg.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://ur.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://iv.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ow.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://pq.bjjhwx.cn

[A04] 判断变量类型
来源：http://el.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ke.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://li.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rg.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://vb.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lk.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mp.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xx.521024.cn

C#:   x.GetType().Name; x is int
来源：http://kc.shtwfgs.cn

[A05] 整数除法与取模
来源：http://cs.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uc.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ob.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dn.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ol.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://nn.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://if.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://tr.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://tr.szxytkj.cn

[A06] 字符串转数字
来源：http://jf.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://lc.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rz.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xb.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://md.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cr.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sa.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oq.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wz.szxytkj.cn

[A07] 数字转字符串
来源：http://ys.szsharing.cn

Py:   str(42)
来源：http://ck.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://xc.colortex.cn

JS:   String(42); (42).toString()
来源：http://fp.huanxung.cn

TS:   String(42)
来源：http://yp.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fn.521024.cn

Go:   strconv.Itoa(42)
来源：http://uy.wgjwhj.cn

Ruby: 42.to_s
来源：http://fh.shtwfgs.cn

C#:   42.ToString()
来源：http://yw.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ks.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rk.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fy.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kt.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lw.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ro.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uk.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qq.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wz.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://mq.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mb.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ag.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ql.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jn.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://km.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xs.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ck.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dv.hahajie.cn

[A10] 生成随机数
来源：http://ks.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://tk.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://do.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nk.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xj.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://xt.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yv.hahajie.cn

Ruby: rand(1..100)
来源：http://mu.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://yk.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://xe.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://dd.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xd.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pd.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://li.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://uv.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://le.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gb.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://az.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://xv.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sm.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ri.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://dc.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://xc.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://lc.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ze.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://zr.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://dl.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ou.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://ry.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://ki.9csxet.cn

JS:   "第一行\n第二行"
来源：http://vh.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://wq.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://tu.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://cx.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://hu.asd995.cn

C#:   "第一行\n第二行"
来源：http://ww.lnxyls.cn

[A14] 注释写法
来源：http://yu.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wd.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ki.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://dl.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://iv.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gf.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://da.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fs.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://hi.colortex.cn

[A15] 空值判断与默认值
来源：http://ox.521024.cn

Py:   value = data or "默认值"
来源：http://cf.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://vo.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://uh.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://zy.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://za.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://bi.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://sc.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://yv.newstarts.cn

[A16] 真假值判断规则
来源：http://ly.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nd.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ra.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cb.bookmarksfly.cn

TS:   if (!x) {}
来源：http://bl.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fq.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hq.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fc.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tc.yuntaijiaju.cn

[A17] 位运算
来源：http://ba.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xk.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lg.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oe.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ph.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tq.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://gi.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://qf.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://gw.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ng.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://vs.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yy.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://us.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://wz.haigaiapp.cn

[A19] 交换两个变量
来源：http://yf.bjjhwx.cn

Py:   a, b = b, a
来源：http://mk.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dh.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://rq.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://lw.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://xp.panjiajie.cn

Go:   a, b = b, a
来源：http://lk.yuexingan06.cn

Ruby: a, b = b, a
来源：http://sq.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://if.lnxyls.cn

[A20] 读取标准输入
来源：http://rx.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://pm.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iw.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nw.asd995.cn

TS:   // Node.js：readline 模块
来源：http://zk.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://us.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oh.gzmigu.cn

Ruby: gets.chomp
来源：http://oe.521024.cn

C#:   Console.ReadLine();
来源：http://jf.521024.cn

[A21] 保留指定小数位输出
来源：http://wn.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://ml.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yt.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://gq.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://wa.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://gy.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jj.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://pi.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://wu.nszjky.cn

[A22] 获取字符串长度
来源：http://ef.huixiangedu.cn

Py:   len(s)
来源：http://vw.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rg.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xc.bjjhwx.cn

TS:   s.length
来源：http://gp.nszjky.cn

Java: s.length()
来源：http://kj.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tn.colortex.cn

Ruby: s.length
来源：http://ow.huixinmuqiang.cn

C#:   s.Length
来源：http://wt.nicolike.cn

[A23] 大小写转换
来源：http://kh.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cm.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uw.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iq.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xu.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bo.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ax.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wi.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xi.gzmigu.cn

[A24] 去除首尾空白
来源：http://jk.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zo.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sq.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fx.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rp.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ju.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://bf.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tk.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ac.jianghongdianzi.cn

[A25] 字符串比较
来源：http://ai.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://pz.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dy.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ce.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mc.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oo.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rm.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://el.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qa.panjiajie.cn

[A26] 类型转换总览
来源：http://ou.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hm.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jd.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ow.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://zf.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ko.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nh.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yl.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kh.shtwfgs.cn

================================================================================
来源：http://jo.szxytkj.cn

B. 流程控制
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://cl.huanxung.cn

[B01] 条件判断 if / else
来源：http://bf.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://io.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wt.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://so.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pp.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://km.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nf.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ik.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xj.9csxet.cn

[B02] 多分支 else if / elif
来源：http://tl.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tw.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kk.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ng.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xr.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ef.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fx.9csxet.cn

[B03] switch / match / case
来源：http://mf.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cu.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xn.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ec.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ky.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bd.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wa.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gi.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ub.szxytkj.cn

[B04] for 计数循环
来源：http://vf.jianghongdianzi.cn


<!-- 参考信息 -->