代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zm.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ds.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ks.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eu.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yg.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vc.shtwfgs.cn

【文件统计】
来源：http://hv.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ye.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://vd.newstarts.cn

目  录
来源：http://dr.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ps.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gr.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://my.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://de.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zv.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://by.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wn.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ux.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pa.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://km.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zf.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mi.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ia.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ua.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://px.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mi.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mc.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://im.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mh.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oc.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dp.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tf.gzmigu.cn

================================================================================
来源：http://zx.shxzskj.cn

A. 基础语法与类型
来源：http://yf.gzmigu.cn

================================================================================
来源：http://cd.bookmarksfly.cn

[A01] Hello World
来源：http://uc.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://db.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://vb.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://qm.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rx.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://nl.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://sp.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://sk.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://la.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://pa.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ti.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rx.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lq.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vn.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://rd.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://ef.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://ag.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://co.shxzukj.cn

[A03] 常量定义
来源：http://sy.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hr.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://kh.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ry.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://pm.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://bt.hahajie.cn

Go:   const PI = 3.14159
来源：http://jt.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://qb.colortex.cn

C#:   const double PI = 3.14159;
来源：http://wq.colortex.cn

[A04] 判断变量类型
来源：http://ri.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zu.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sb.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qw.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://hp.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://db.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fk.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rc.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://rk.shtwfgs.cn

[A05] 整数除法与取模
来源：http://nv.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tc.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mr.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ox.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hd.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://zr.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://wu.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qi.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://vl.haigaiapp.cn

[A06] 字符串转数字
来源：http://mc.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://mf.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hd.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gy.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://em.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ms.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jy.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://da.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hq.bjjhwx.cn

[A07] 数字转字符串
来源：http://xy.gzmigu.cn

Py:   str(42)
来源：http://px.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://rj.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://mr.asd995.cn

TS:   String(42)
来源：http://rp.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ke.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://yu.colortex.cn

Ruby: 42.to_s
来源：http://do.shtwfgs.cn

C#:   42.ToString()
来源：http://mh.panjiajie.cn

[A08] 取整与四舍五入
来源：http://bd.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xh.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ay.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pc.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qz.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ai.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hv.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ll.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fm.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://bu.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mo.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bb.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iz.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bq.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wx.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ml.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://br.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dj.yuexingan06.cn

[A10] 生成随机数
来源：http://up.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://mz.521024.cn

PHP:  random_int(1, 100);
来源：http://jd.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tf.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ut.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://zj.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pz.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://tt.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://id.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://pz.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://vp.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nt.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ef.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://la.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://zk.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ic.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fd.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bh.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ux.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sc.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nf.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://lj.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://xz.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://es.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ea.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://yf.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://an.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iu.asd995.cn

Py:   "第一行\n第二行"
来源：http://px.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://yo.colortex.cn

JS:   "第一行\n第二行"
来源：http://vc.colortex.cn

TS:   "第一行\n第二行"
来源：http://ac.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://ly.521024.cn

Go:   "第一行\n第二行"
来源：http://wk.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://wp.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://hg.nicolike.cn

[A14] 注释写法
来源：http://sa.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lp.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jq.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://up.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://rt.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rh.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://lc.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fv.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://mc.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://zc.shxzskj.cn

Py:   value = data or "默认值"
来源：http://eh.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://zf.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://bp.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://aj.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ce.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://gg.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://kv.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://gs.9csxet.cn

[A16] 真假值判断规则
来源：http://pq.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ag.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sb.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hp.wgjwhj.cn

TS:   if (!x) {}
来源：http://ak.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ew.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wx.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nw.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iw.muxihuayi.cn

[A17] 位运算
来源：http://xn.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fe.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uh.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nw.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qj.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sy.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ot.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bn.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://cz.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://rw.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://kl.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ii.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mw.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://hf.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kb.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://fz.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://wz.hnjuh.cn

[A19] 交换两个变量
来源：http://mv.newstarts.cn

Py:   a, b = b, a
来源：http://wt.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://it.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://mh.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://zv.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://ww.nicolike.cn

Go:   a, b = b, a
来源：http://wh.huanxung.cn

Ruby: a, b = b, a
来源：http://fn.asd995.cn

C#:   (a, b) = (b, a);
来源：http://da.haigaiapp.cn

[A20] 读取标准输入
来源：http://lz.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://ew.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nd.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://al.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://cz.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://oo.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://be.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://pn.newstarts.cn

C#:   Console.ReadLine();
来源：http://fc.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://it.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://lo.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sk.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://sj.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://bu.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://bh.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ze.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://kh.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://nb.jctech888.com.cn

[A22] 获取字符串长度
来源：http://se.bjjhwx.cn

Py:   len(s)
来源：http://zf.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bi.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://es.9csxet.cn

TS:   s.length
来源：http://yd.yuexingan06.cn

Java: s.length()
来源：http://df.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sz.shxzskj.cn

Ruby: s.length
来源：http://zy.szxytkj.cn

C#:   s.Length
来源：http://qo.newstarts.cn

[A23] 大小写转换
来源：http://uk.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wm.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://na.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iz.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ip.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cq.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://li.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://je.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://km.haigaiapp.cn

[A24] 去除首尾空白
来源：http://dh.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qt.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fw.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jr.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://he.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pn.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://yi.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oz.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sp.bjjhwx.cn

[A25] 字符串比较
来源：http://yq.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://kp.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xd.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qs.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ka.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tm.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vk.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hg.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ds.bjjhwx.cn

[A26] 类型转换总览
来源：http://vg.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jn.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uh.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oh.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://md.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hl.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yk.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xc.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://op.521024.cn

================================================================================
来源：http://gs.huixinmuqiang.cn

B. 流程控制
来源：http://kl.szxytkj.cn

================================================================================
来源：http://mk.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://ai.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tx.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lp.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fe.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ml.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cr.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://av.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ug.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uz.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://xu.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ju.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kp.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rj.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qk.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vu.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lg.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dw.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.newstarts.cn

[B03] switch / match / case
来源：http://rc.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zj.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ih.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jg.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ku.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qj.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bw.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fu.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nu.gzmigu.cn

[B04] for 计数循环
来源：http://ok.panjiajie.cn


<!-- 参考信息 -->