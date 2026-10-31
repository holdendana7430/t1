代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pg.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sj.colortex.cn

【文件统计】
来源：http://az.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fm.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://rg.szxytkj.cn

目  录
来源：http://as.szsharing.cn

--------------------------------------------------------------------------------
来源：http://pg.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vl.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wv.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zh.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rx.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zy.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zq.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qz.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ye.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mq.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cx.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wx.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dm.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ja.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hc.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://th.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lu.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ct.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iu.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lf.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sk.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qx.jianghongdianzi.cn

================================================================================
来源：http://vh.panjiajie.cn

A. 基础语法与类型
来源：http://fw.haigaiapp.cn

================================================================================
来源：http://ma.wgjwhj.cn

[A01] Hello World
来源：http://tw.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://qa.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://dh.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://he.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ym.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://sw.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://hd.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://un.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fg.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://xy.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xa.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qk.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rz.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zd.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ck.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://bm.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://fk.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rs.jctech888.com.cn

[A03] 常量定义
来源：http://re.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://on.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://dg.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://qm.521024.cn

TS:   const PI: number = 3.14159;
来源：http://gw.colortex.cn

Java: static final double PI = 3.14159;
来源：http://uy.hnjuh.cn

Go:   const PI = 3.14159
来源：http://hy.lnxyls.cn

Ruby: PI = 3.14159
来源：http://cj.asd995.cn

C#:   const double PI = 3.14159;
来源：http://za.gzmigu.cn

[A04] 判断变量类型
来源：http://pz.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jx.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oe.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nd.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://ud.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ji.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bs.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hu.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://io.hahajie.cn

[A05] 整数除法与取模
来源：http://lo.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dr.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ch.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gc.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://em.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://ag.521024.cn

Go:   7 / 2; 7 % 2
来源：http://vu.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://tt.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://aq.521024.cn

[A06] 字符串转数字
来源：http://dn.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://zs.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://na.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zb.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uw.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xv.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iq.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ei.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://at.lnxyls.cn

[A07] 数字转字符串
来源：http://ly.jctech888.com.cn

Py:   str(42)
来源：http://qo.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://ry.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://jh.9csxet.cn

TS:   String(42)
来源：http://pu.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rh.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://xi.9csxet.cn

Ruby: 42.to_s
来源：http://pp.bjjhwx.cn

C#:   42.ToString()
来源：http://da.gzmigu.cn

[A08] 取整与四舍五入
来源：http://nf.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uy.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rq.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ca.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://av.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vc.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://es.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wd.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xk.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://gt.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qn.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ka.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ef.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://er.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tz.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qm.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lh.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rg.huixinmuqiang.cn

[A10] 生成随机数
来源：http://ni.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://sw.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://yp.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nh.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xy.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://fs.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vq.shxzukj.cn

Ruby: rand(1..100)
来源：http://mt.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://gu.szsharing.cn

[A11] 条件表达式（三元）
来源：http://wd.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://my.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://md.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://of.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qt.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://bi.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hy.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wf.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wu.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://oa.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pc.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ow.asd995.cn

JS:   `Hello, ${name}!`
来源：http://xf.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://af.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://em.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iy.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://ck.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://es.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uh.colortex.cn

Py:   "第一行\n第二行"
来源：http://df.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://er.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://ar.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://xg.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://fo.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://hk.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://xq.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://vu.haigaiapp.cn

[A14] 注释写法
来源：http://me.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rs.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kp.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://yi.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://wk.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wh.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://fy.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pi.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://oz.colortex.cn

[A15] 空值判断与默认值
来源：http://ry.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://jt.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://rl.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://po.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://xp.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://by.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://jq.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://de.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://kq.jctech888.com.cn

[A16] 真假值判断规则
来源：http://ho.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://td.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lj.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://el.hnjuh.cn

TS:   if (!x) {}
来源：http://kz.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://px.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wg.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yt.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bh.bookmarksfly.cn

[A17] 位运算
来源：http://tm.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nq.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ju.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vg.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ek.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zc.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://no.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hh.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://ov.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://jr.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ko.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kr.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yu.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://fy.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tq.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://ye.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://mx.bjjhwx.cn

[A19] 交换两个变量
来源：http://nr.shtwfgs.cn

Py:   a, b = b, a
来源：http://qq.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ce.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://wg.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://vd.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://iw.9csxet.cn

Go:   a, b = b, a
来源：http://pw.jctech888.com.cn

Ruby: a, b = b, a
来源：http://se.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://zt.wgjwhj.cn

[A20] 读取标准输入
来源：http://ob.colortex.cn

Py:   name = input("请输入：")
来源：http://iz.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://he.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lf.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://xv.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://xr.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cx.szsharing.cn

Ruby: gets.chomp
来源：http://mr.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://fv.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://pv.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ql.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dd.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://lx.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ez.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://fo.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hl.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ku.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://cb.nicolike.cn

[A22] 获取字符串长度
来源：http://ab.lnxyls.cn

Py:   len(s)
来源：http://qs.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fr.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://df.bookmarksfly.cn

TS:   s.length
来源：http://vv.jianghongdianzi.cn

Java: s.length()
来源：http://jy.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pi.huixinmuqiang.cn

Ruby: s.length
来源：http://va.yuntaijiaju.cn

C#:   s.Length
来源：http://wq.nicolike.cn

[A23] 大小写转换
来源：http://xu.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://da.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lw.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hi.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://av.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://il.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wu.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yi.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://in.szsharing.cn

[A24] 去除首尾空白
来源：http://xj.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qb.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iq.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hu.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kc.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hh.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://yh.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ey.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wy.nszjky.cn

[A25] 字符串比较
来源：http://op.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://mb.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://br.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qg.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qk.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ak.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yn.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bs.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oj.wgjwhj.cn

[A26] 类型转换总览
来源：http://sd.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ea.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ex.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qt.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://qy.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yo.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xp.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pt.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ye.huanxung.cn

================================================================================
来源：http://ab.521024.cn

B. 流程控制
来源：http://qp.szxytkj.cn

================================================================================
来源：http://ot.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://vz.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rv.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ir.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fx.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vn.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ti.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qd.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ss.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tv.nszjky.cn

[B02] 多分支 else if / elif
来源：http://pk.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vb.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://te.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ar.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pd.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xs.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rx.jctech888.com.cn

[B03] switch / match / case
来源：http://wm.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://io.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pe.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vb.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kq.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xo.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wz.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ao.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hv.chemitech.net.cn

[B04] for 计数循环
来源：http://uo.asd995.cn

Py:   for i in range(10): print(i)
来源：http://bj.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bp.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xn.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sk.asd995.cn


<!-- 参考信息 -->