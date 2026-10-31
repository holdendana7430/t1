代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://da.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ds.chemitech.net.cn

【文件统计】
来源：http://qn.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oy.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://rc.jianghongdianzi.cn

目  录
来源：http://zc.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://od.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fx.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ol.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zo.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oj.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yu.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ea.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ue.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dw.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hm.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ic.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://if.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oh.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://up.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cg.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nh.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://va.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wn.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fs.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jo.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gl.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kp.panjiajie.cn

================================================================================
来源：http://gs.huixinmuqiang.cn

A. 基础语法与类型
来源：http://qu.shxzukj.cn

================================================================================
来源：http://qs.panjiajie.cn

[A01] Hello World
来源：http://ux.shxzukj.cn

Py:   print("Hello, World!")
来源：http://dn.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://ve.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://un.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ep.521024.cn

Java: System.out.println("Hello, World!");
来源：http://yd.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://fc.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://mb.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xk.shxzskj.cn

[A02] 变量声明与赋值
来源：http://xc.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fv.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fq.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://so.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aa.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://hy.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://dz.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://cb.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sx.shxzskj.cn

[A03] 常量定义
来源：http://yi.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nd.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://tm.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://ay.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://ay.asd995.cn

Java: static final double PI = 3.14159;
来源：http://pl.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://dn.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://va.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://xn.jctech888.com.cn

[A04] 判断变量类型
来源：http://gy.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nr.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ot.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://au.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://hd.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ii.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fj.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lf.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://nj.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://xz.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lt.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hy.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jm.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ov.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://ke.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://zq.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://uk.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://mk.hahajie.cn

[A06] 字符串转数字
来源：http://ru.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://mu.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gd.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rm.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ph.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cn.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tm.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zp.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vj.bookmarksfly.cn

[A07] 数字转字符串
来源：http://fg.yuexingan06.cn

Py:   str(42)
来源：http://ug.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://kg.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://vg.muxihuayi.cn

TS:   String(42)
来源：http://ju.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xg.colortex.cn

Go:   strconv.Itoa(42)
来源：http://bt.muxihuayi.cn

Ruby: 42.to_s
来源：http://oc.wgjwhj.cn

C#:   42.ToString()
来源：http://dy.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://wz.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vg.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rq.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ng.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://st.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ol.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qg.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://no.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rn.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://qd.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dv.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zx.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uw.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yk.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ax.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ec.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ub.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ds.bjjhwx.cn

[A10] 生成随机数
来源：http://bi.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://lc.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://rv.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yz.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rf.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://hu.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mt.hahajie.cn

Ruby: rand(1..100)
来源：http://gh.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://mv.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://mf.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qx.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ku.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://np.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dd.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://ld.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lf.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ci.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ol.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://az.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yq.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zo.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://xm.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://lg.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://iv.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jc.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://je.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://wi.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bu.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ss.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://rc.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://yb.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://ke.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ua.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://va.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://ly.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://xy.gzmigu.cn

[A14] 注释写法
来源：http://lk.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bd.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ih.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://vz.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://yj.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ub.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://bw.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mz.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://dw.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://kc.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://zp.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://by.521024.cn

JS:   const value = data ?? "默认值";
来源：http://hq.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://kk.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bu.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.nszjky.cn

Ruby: value = data || "默认值"
来源：http://vx.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://mi.panjiajie.cn

[A16] 真假值判断规则
来源：http://uz.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://un.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pz.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ml.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://ue.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://be.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jz.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pw.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wh.newstarts.cn

[A17] 位运算
来源：http://rd.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yl.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tj.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dg.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://be.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://af.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ue.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://js.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://im.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://rp.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oq.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ms.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://dj.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cu.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ze.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ax.bookmarksfly.cn

[A19] 交换两个变量
来源：http://ku.nszjky.cn

Py:   a, b = b, a
来源：http://sk.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nb.521024.cn

JS:   [a, b] = [b, a];
来源：http://es.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://ze.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://av.hnjuh.cn

Go:   a, b = b, a
来源：http://aa.haigaiapp.cn

Ruby: a, b = b, a
来源：http://sy.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://io.nicolike.cn

[A20] 读取标准输入
来源：http://gc.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://hx.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ne.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ik.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://pq.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://sw.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vf.hahajie.cn

Ruby: gets.chomp
来源：http://gn.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://fx.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://yc.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://kg.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xi.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://sb.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://uu.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://wj.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zf.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mp.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://de.asd995.cn

[A22] 获取字符串长度
来源：http://hn.yuexingan06.cn

Py:   len(s)
来源：http://bf.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gy.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ke.shxzukj.cn

TS:   s.length
来源：http://ws.newstarts.cn

Java: s.length()
来源：http://ay.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sl.newstarts.cn

Ruby: s.length
来源：http://wz.jctech888.com.cn

C#:   s.Length
来源：http://du.nszjky.cn

[A23] 大小写转换
来源：http://cl.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vj.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bj.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ws.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gp.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lx.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cj.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://km.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fw.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://xs.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pf.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://el.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rw.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mz.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://ei.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wt.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cn.chemitech.net.cn

[A25] 字符串比较
来源：http://hd.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ei.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://so.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ky.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hg.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ay.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mp.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ve.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mc.colortex.cn

[A26] 类型转换总览
来源：http://ua.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iq.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cc.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://we.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://dd.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xw.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yl.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hy.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uo.shxzskj.cn

================================================================================
来源：http://rg.bookmarksfly.cn

B. 流程控制
来源：http://zs.haigaiapp.cn

================================================================================
来源：http://ba.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ko.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yn.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nq.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ax.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oa.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xd.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ro.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vb.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zv.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://er.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bs.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://id.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bh.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iv.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fr.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://np.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.huixiangedu.cn

[B03] switch / match / case
来源：http://tf.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eq.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ms.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fi.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bq.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sw.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ul.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://re.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yu.huanxung.cn

[B04] for 计数循环
来源：http://eh.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://bd.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tb.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nv.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cx.521024.cn


<!-- 参考信息 -->