代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yb.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ka.shtwfgs.cn

【文件统计】
来源：http://pe.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dy.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ml.panjiajie.cn

目  录
来源：http://oq.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ui.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jt.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ru.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gy.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://st.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lw.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://he.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://do.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oq.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lf.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uq.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qx.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wu.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zc.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dx.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wc.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oj.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mk.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vu.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wm.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kk.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vp.jianghongdianzi.cn

================================================================================
来源：http://wp.chemitech.net.cn

A. 基础语法与类型
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://cm.jctech888.com.cn

[A01] Hello World
来源：http://pz.shxzukj.cn

Py:   print("Hello, World!")
来源：http://cz.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://tc.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://mv.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rv.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://mc.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ni.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://bl.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cv.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://gc.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ar.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sb.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://em.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zj.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://xl.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://gc.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://gq.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tr.bjjhwx.cn

[A03] 常量定义
来源：http://vo.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ec.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://td.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://vf.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://hs.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://lg.szsharing.cn

Go:   const PI = 3.14159
来源：http://jf.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://hj.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://jd.wgjwhj.cn

[A04] 判断变量类型
来源：http://va.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vb.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xf.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xe.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://qc.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://al.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://za.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nu.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://xa.chemitech.net.cn

[A05] 整数除法与取模
来源：http://yq.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ka.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lx.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tt.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tf.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://ot.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://ua.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://rr.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://cj.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://fs.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://jo.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kz.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://li.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wp.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gj.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vd.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tb.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yd.szsharing.cn

[A07] 数字转字符串
来源：http://sz.shxzukj.cn

Py:   str(42)
来源：http://vd.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://ld.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://et.huixinmuqiang.cn

TS:   String(42)
来源：http://sj.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gh.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://wu.gzmigu.cn

Ruby: 42.to_s
来源：http://cc.lnxyls.cn

C#:   42.ToString()
来源：http://wg.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://dw.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vx.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://df.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://du.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xy.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ca.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yi.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pd.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ih.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://jp.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://np.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gx.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sg.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uy.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fq.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jb.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yk.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zw.muxihuayi.cn

[A10] 生成随机数
来源：http://pn.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://cg.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://nz.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ml.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dp.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://wj.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wu.shxzukj.cn

Ruby: rand(1..100)
来源：http://yp.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://ai.9csxet.cn

[A11] 条件表达式（三元）
来源：http://lc.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://nm.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lz.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ya.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ut.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://yq.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zq.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://as.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sr.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://ek.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vk.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gu.colortex.cn

JS:   `Hello, ${name}!`
来源：http://bs.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://qr.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://dd.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xq.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://ez.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://uj.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ta.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://uk.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://qa.huanxung.cn

JS:   "第一行\n第二行"
来源：http://om.asd995.cn

TS:   "第一行\n第二行"
来源：http://tb.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://gd.hahajie.cn

Go:   "第一行\n第二行"
来源：http://hi.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ub.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://po.newstarts.cn

[A14] 注释写法
来源：http://kl.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://po.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tj.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://ej.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://qc.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://um.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://iz.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://za.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://so.hnjuh.cn

[A15] 空值判断与默认值
来源：http://fe.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://fu.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://na.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://sn.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://tn.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nl.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://ou.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://wt.521024.cn

C#:   var value = data ?? "默认值";
来源：http://ed.9csxet.cn

[A16] 真假值判断规则
来源：http://wf.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lh.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://er.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fc.asd995.cn

TS:   if (!x) {}
来源：http://bp.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rj.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jw.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jt.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xt.shtwfgs.cn

[A17] 位运算
来源：http://be.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zs.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jf.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wa.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fq.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yc.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tl.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://ko.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://gj.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://xu.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zp.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hs.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://in.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hu.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://ud.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://kj.nszjky.cn

[A19] 交换两个变量
来源：http://hh.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://hh.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jw.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://gh.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://sk.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://gp.yuexingan06.cn

Go:   a, b = b, a
来源：http://qi.9csxet.cn

Ruby: a, b = b, a
来源：http://at.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://by.jctech888.com.cn

[A20] 读取标准输入
来源：http://rg.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://ev.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ct.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://op.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://kp.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://fh.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://et.colortex.cn

Ruby: gets.chomp
来源：http://fv.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://mi.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://tu.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://pj.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uz.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://cr.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ck.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://mu.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fd.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://lu.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://qw.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ix.bookmarksfly.cn

Py:   len(s)
来源：http://xw.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dn.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ah.szsharing.cn

TS:   s.length
来源：http://se.jctech888.com.cn

Java: s.length()
来源：http://vr.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sg.muxihuayi.cn

Ruby: s.length
来源：http://pp.colortex.cn

C#:   s.Length
来源：http://ig.colortex.cn

[A23] 大小写转换
来源：http://xk.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nk.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yk.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dv.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cf.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gx.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pf.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jg.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wf.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://hh.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rx.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wt.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pk.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xo.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://he.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://uf.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gy.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sp.hahajie.cn

[A25] 字符串比较
来源：http://yx.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://dz.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://px.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ts.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ed.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zi.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vo.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dj.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nw.muxihuayi.cn

[A26] 类型转换总览
来源：http://rq.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mn.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bn.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://op.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://tl.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dw.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ha.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wp.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fh.9csxet.cn

================================================================================
来源：http://fm.jianghongdianzi.cn

B. 流程控制
来源：http://ex.hahajie.cn

================================================================================
来源：http://hm.nicolike.cn

[B01] 条件判断 if / else
来源：http://kc.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qh.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ra.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://so.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jn.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rn.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ox.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ub.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ia.9csxet.cn

[B02] 多分支 else if / elif
来源：http://fx.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ou.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pm.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vm.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zh.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pn.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://me.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://df.gzmigu.cn

[B03] switch / match / case
来源：http://ko.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ft.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ef.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uc.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xw.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sh.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uv.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fy.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bj.panjiajie.cn

[B04] for 计数循环
来源：http://yh.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://si.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jz.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zk.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fn.yuexingan06.cn


<!-- 参考信息 -->