代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pe.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yk.haigaiapp.cn

【文件统计】
来源：http://bh.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gw.hahajie.cn

--------------------------------------------------------------------------------
来源：http://io.szsharing.cn

目  录
来源：http://zx.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://tm.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fg.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wc.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ge.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ec.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://so.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://js.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dm.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kp.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xm.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cw.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uf.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lq.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ae.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ks.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://al.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tl.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pf.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qo.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pe.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rq.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ay.bjjhwx.cn

================================================================================
来源：http://nj.521024.cn

A. 基础语法与类型
来源：http://sz.gzmigu.cn

================================================================================
来源：http://am.chemitech.net.cn

[A01] Hello World
来源：http://wr.shxzskj.cn

Py:   print("Hello, World!")
来源：http://tq.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://aj.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://zp.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bu.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://tp.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://jx.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://at.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xi.huanxung.cn

[A02] 变量声明与赋值
来源：http://rz.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://om.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tv.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ih.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://of.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://pp.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://mr.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://hf.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://og.yuexingan06.cn

[A03] 常量定义
来源：http://go.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://st.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://al.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://wb.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://qt.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://vq.szsharing.cn

Go:   const PI = 3.14159
来源：http://pg.hnjuh.cn

Ruby: PI = 3.14159
来源：http://vy.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://rx.shxzskj.cn

[A04] 判断变量类型
来源：http://nj.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nr.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vs.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pm.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://sh.nicolike.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://za.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uj.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ij.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ah.colortex.cn

[A05] 整数除法与取模
来源：http://ta.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uq.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ps.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lx.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fx.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://av.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://me.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://sf.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://yd.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://sw.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://bc.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dy.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://go.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fb.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wd.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jt.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ad.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ym.szsharing.cn

[A07] 数字转字符串
来源：http://ej.huixinmuqiang.cn

Py:   str(42)
来源：http://wf.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://ex.colortex.cn

JS:   String(42); (42).toString()
来源：http://kt.colortex.cn

TS:   String(42)
来源：http://ny.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://al.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://nk.nszjky.cn

Ruby: 42.to_s
来源：http://ck.panjiajie.cn

C#:   42.ToString()
来源：http://ud.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://js.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ps.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ri.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vx.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iz.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fg.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bz.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ul.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://as.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://sm.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kc.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cq.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bp.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ck.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fx.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qu.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bh.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lc.szsharing.cn

[A10] 生成随机数
来源：http://ex.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://gp.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://rb.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nl.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wy.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://yg.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qu.shxzskj.cn

Ruby: rand(1..100)
来源：http://na.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://cv.newstarts.cn

[A11] 条件表达式（三元）
来源：http://nc.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://bv.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ua.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ny.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ar.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://nq.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://at.szsharing.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kt.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vf.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://ii.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gl.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wo.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://ib.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://xn.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://bi.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://un.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://dv.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://jn.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://da.nicolike.cn

Py:   "第一行\n第二行"
来源：http://bs.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://jx.nszjky.cn

JS:   "第一行\n第二行"
来源：http://jd.hahajie.cn

TS:   "第一行\n第二行"
来源：http://yk.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://cp.szsharing.cn

Go:   "第一行\n第二行"
来源：http://uq.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://ci.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://ce.yuexingan06.cn

[A14] 注释写法
来源：http://ft.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ey.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kz.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://ih.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://vo.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zf.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://si.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lk.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://kj.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ev.nszjky.cn

Py:   value = data or "默认值"
来源：http://ge.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ku.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://kr.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://eh.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qw.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://cx.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://bg.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://hw.shxzskj.cn

[A16] 真假值判断规则
来源：http://je.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dm.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ze.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://il.nicolike.cn

TS:   if (!x) {}
来源：http://jx.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cj.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tc.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jz.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ku.yuexingan06.cn

[A17] 位运算
来源：http://lu.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bb.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ic.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hr.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vo.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://mg.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ax.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://hg.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://km.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pa.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://ei.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://md.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://up.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://rk.hnjuh.cn

[A19] 交换两个变量
来源：http://ou.szxytkj.cn

Py:   a, b = b, a
来源：http://cm.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jq.521024.cn

JS:   [a, b] = [b, a];
来源：http://ck.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://cz.521024.cn

Java: int t = a; a = b; b = t;
来源：http://sf.bookmarksfly.cn

Go:   a, b = b, a
来源：http://yr.muxihuayi.cn

Ruby: a, b = b, a
来源：http://rc.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://vm.nicolike.cn

[A20] 读取标准输入
来源：http://lw.9csxet.cn

Py:   name = input("请输入：")
来源：http://dq.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tt.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wv.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://lr.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://jp.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hq.huanxung.cn

Ruby: gets.chomp
来源：http://jb.gzmigu.cn

C#:   Console.ReadLine();
来源：http://ec.szsharing.cn

[A21] 保留指定小数位输出
来源：http://hu.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://ub.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tc.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://hw.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://ir.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://wg.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ae.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://cc.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://fv.muxihuayi.cn

[A22] 获取字符串长度
来源：http://oj.shxzukj.cn

Py:   len(s)
来源：http://yy.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rg.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gu.shxzskj.cn

TS:   s.length
来源：http://fu.hahajie.cn

Java: s.length()
来源：http://zc.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yp.panjiajie.cn

Ruby: s.length
来源：http://pt.haigaiapp.cn

C#:   s.Length
来源：http://ix.lnxyls.cn

[A23] 大小写转换
来源：http://rh.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aq.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ij.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rv.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ga.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://co.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://at.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mn.szxytkj.cn

[A24] 去除首尾空白
来源：http://uk.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vj.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bz.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sd.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hb.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ni.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://pf.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vl.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ip.wgjwhj.cn

[A25] 字符串比较
来源：http://pv.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://cs.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://do.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fb.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bk.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ur.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nz.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yf.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ro.huanxung.cn

[A26] 类型转换总览
来源：http://lr.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://io.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://av.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mn.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://tt.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ud.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fj.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://id.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yd.colortex.cn

================================================================================
来源：http://rv.szsharing.cn

B. 流程控制
来源：http://cf.yuntaijiaju.cn

================================================================================
来源：http://tj.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ri.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jh.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ek.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kh.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nx.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pp.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vf.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ij.asd995.cn

[B02] 多分支 else if / elif
来源：http://mm.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ey.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wf.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dd.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iq.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uw.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.nicolike.cn

[B03] switch / match / case
来源：http://pd.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qg.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gy.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fl.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qb.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nh.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vf.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fy.shxzskj.cn

[B04] for 计数循环
来源：http://me.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://lx.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ar.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://db.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wv.szxytkj.cn


<!-- 参考信息 -->