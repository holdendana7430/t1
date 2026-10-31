代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bc.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cj.newstarts.cn

【文件统计】
来源：http://ld.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ih.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://gh.muxihuayi.cn

目  录
来源：http://xw.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ww.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uy.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fs.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sr.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vy.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jf.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://to.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ce.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wd.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lw.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dt.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xe.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ld.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lg.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ot.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://om.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yh.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bq.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hb.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://is.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hx.chemitech.net.cn

================================================================================
来源：http://qf.asd995.cn

A. 基础语法与类型
来源：http://zc.hnjuh.cn

================================================================================
来源：http://fd.nicolike.cn

[A01] Hello World
来源：http://om.nicolike.cn

Py:   print("Hello, World!")
来源：http://xb.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://ry.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://qi.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://um.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://xo.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://gc.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://xe.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yf.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ve.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xh.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oe.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gw.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qg.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://bt.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://qw.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://dw.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zf.huixinmuqiang.cn

[A03] 常量定义
来源：http://sj.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rn.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://ap.9csxet.cn

JS:   const PI = 3.14159;
来源：http://qa.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://un.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://mm.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://wh.shxzukj.cn

Ruby: PI = 3.14159
来源：http://ri.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://yu.huixiangedu.cn

[A04] 判断变量类型
来源：http://jh.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tw.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://go.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zk.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://bp.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nm.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hp.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oy.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://km.yuexingan06.cn

[A05] 整数除法与取模
来源：http://le.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tx.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xz.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lf.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mq.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://gb.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://pm.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://pz.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://jj.szxytkj.cn

[A06] 字符串转数字
来源：http://lc.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://yk.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://be.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ct.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yf.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bf.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xx.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mm.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oi.yuexingan06.cn

[A07] 数字转字符串
来源：http://ii.bjjhwx.cn

Py:   str(42)
来源：http://xy.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://tw.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://wk.colortex.cn

TS:   String(42)
来源：http://rh.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wi.asd995.cn

Go:   strconv.Itoa(42)
来源：http://wj.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://vp.szsharing.cn

C#:   42.ToString()
来源：http://fs.shxzskj.cn

[A08] 取整与四舍五入
来源：http://qe.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yw.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bn.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ym.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iv.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ya.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nz.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bm.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nx.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://ht.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ig.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gy.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lz.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zq.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ku.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gp.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sb.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ef.chemitech.net.cn

[A10] 生成随机数
来源：http://yu.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://qs.colortex.cn

PHP:  random_int(1, 100);
来源：http://zh.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gc.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://bu.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fm.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://eg.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://xi.nszjky.cn

[A11] 条件表达式（三元）
来源：http://nf.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://hh.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vv.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vt.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xc.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://at.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zs.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sw.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xr.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://ii.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://md.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tt.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://ga.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ze.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://pn.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://id.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://vv.asd995.cn

C#:   $"Hello, {name}!"
来源：http://ua.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fw.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://jd.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://om.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://js.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://us.hahajie.cn

Java: "第一行\n第二行"
来源：http://yy.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://rc.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://ee.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://hr.jctech888.com.cn

[A14] 注释写法
来源：http://qc.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bd.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iz.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://go.521024.cn

TS:   // 单行；/* 多行 */
来源：http://zd.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://id.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://gs.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://aj.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://wt.9csxet.cn

[A15] 空值判断与默认值
来源：http://mi.newstarts.cn

Py:   value = data or "默认值"
来源：http://vc.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ga.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://gz.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://ws.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uf.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://qz.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://kr.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://pn.shxzskj.cn

[A16] 真假值判断规则
来源：http://ar.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wh.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ug.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qp.muxihuayi.cn

TS:   if (!x) {}
来源：http://kb.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sv.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://si.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qn.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lr.shxzskj.cn

[A17] 位运算
来源：http://gv.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dy.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jv.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jv.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wb.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wn.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://kb.521024.cn

Py:   ord("A"); chr(65)
来源：http://ho.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://vs.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ml.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ri.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://qz.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ax.521024.cn

Ruby: "A".ord; 65.chr
来源：http://sg.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://un.huixiangedu.cn

[A19] 交换两个变量
来源：http://md.shxzukj.cn

Py:   a, b = b, a
来源：http://ce.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yn.asd995.cn

JS:   [a, b] = [b, a];
来源：http://hf.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://cn.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://zg.szxytkj.cn

Go:   a, b = b, a
来源：http://cf.szsharing.cn

Ruby: a, b = b, a
来源：http://bn.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://fq.szsharing.cn

[A20] 读取标准输入
来源：http://bb.shxzukj.cn

Py:   name = input("请输入：")
来源：http://ue.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jt.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oc.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://fk.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://xg.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xp.muxihuayi.cn

Ruby: gets.chomp
来源：http://xp.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://fk.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://rb.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://fv.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://se.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ao.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://cx.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://fh.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ij.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ik.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://qc.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://fz.521024.cn

Py:   len(s)
来源：http://kh.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sx.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wd.nszjky.cn

TS:   s.length
来源：http://fr.newstarts.cn

Java: s.length()
来源：http://ya.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sk.huanxung.cn

Ruby: s.length
来源：http://ly.huanxung.cn

C#:   s.Length
来源：http://rc.lnxyls.cn

[A23] 大小写转换
来源：http://gh.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rw.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tw.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jo.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://om.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ha.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yd.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hd.gzmigu.cn

[A24] 去除首尾空白
来源：http://kz.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iq.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zl.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rr.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sw.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ew.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://bk.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oi.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yr.muxihuayi.cn

[A25] 字符串比较
来源：http://hk.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://pt.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fy.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qd.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hl.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://va.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ls.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lu.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hu.haigaiapp.cn

[A26] 类型转换总览
来源：http://qf.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vz.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gy.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jx.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://pv.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ee.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ar.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uh.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pe.newstarts.cn

================================================================================
来源：http://py.shxzukj.cn

B. 流程控制
来源：http://qy.wgjwhj.cn

================================================================================
来源：http://ag.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://sb.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fk.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sc.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://if.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://so.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sd.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://if.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bg.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ce.colortex.cn

[B02] 多分支 else if / elif
来源：http://bm.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bw.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yo.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gy.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hs.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jt.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fk.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ix.hahajie.cn

[B03] switch / match / case
来源：http://lo.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ud.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vq.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tb.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tf.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aa.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xp.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cq.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jr.gzmigu.cn

[B04] for 计数循环
来源：http://lx.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://rd.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fx.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tf.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oi.szxytkj.cn


<!-- 参考信息 -->