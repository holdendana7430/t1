代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nb.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bc.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hs.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wq.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wp.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ac.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cf.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gc.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://na.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ej.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fr.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jg.huanxung.cn

================================================================================
来源：http://hw.wgjwhj.cn

A. 基础语法与类型
来源：http://mp.nszjky.cn

================================================================================
来源：http://ji.szsharing.cn

[A01] Hello World
来源：http://ku.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://pk.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://lf.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://gs.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zt.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://or.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://do.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://ml.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://is.shxzskj.cn

[A02] 变量声明与赋值
来源：http://if.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vh.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cl.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lv.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ts.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://oa.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://jc.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://co.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zq.shtwfgs.cn

[A03] 常量定义
来源：http://ue.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rw.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://gq.hahajie.cn

JS:   const PI = 3.14159;
来源：http://sy.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://fd.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://sf.hahajie.cn

Go:   const PI = 3.14159
来源：http://qs.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://gb.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://kh.gzmigu.cn

[A04] 判断变量类型
来源：http://jg.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mp.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://re.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hj.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://eq.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pk.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ul.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gd.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://tw.huanxung.cn

[A05] 整数除法与取模
来源：http://xj.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ni.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xa.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zz.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ja.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://ec.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://ed.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://aa.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://qv.newstarts.cn

[A06] 字符串转数字
来源：http://ep.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://ov.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uv.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oc.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zi.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yg.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nw.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ys.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ri.gzmigu.cn

[A07] 数字转字符串
来源：http://bo.muxihuayi.cn

Py:   str(42)
来源：http://lh.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://px.asd995.cn

JS:   String(42); (42).toString()
来源：http://vg.wgjwhj.cn

TS:   String(42)
来源：http://js.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jf.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://eb.hnjuh.cn

Ruby: 42.to_s
来源：http://tm.colortex.cn

C#:   42.ToString()
来源：http://ak.newstarts.cn

[A08] 取整与四舍五入
来源：http://ci.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://th.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://no.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://te.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ih.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ug.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ql.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gv.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mm.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://wh.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xk.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qb.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ef.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cb.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tl.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bg.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mm.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xr.nszjky.cn

[A10] 生成随机数
来源：http://ik.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://gs.nicolike.cn

PHP:  random_int(1, 100);
来源：http://sh.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mn.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oo.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://up.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rh.chemitech.net.cn

Ruby: rand(1..100)
来源：http://ed.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://yt.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://du.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://fn.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wv.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qf.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vl.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://wb.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://co.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ky.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vf.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://tv.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jc.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hf.asd995.cn

JS:   `Hello, ${name}!`
来源：http://no.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://oj.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://mq.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tu.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://wx.asd995.cn

C#:   $"Hello, {name}!"
来源：http://jg.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pw.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ad.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://pj.asd995.cn

JS:   "第一行\n第二行"
来源：http://mv.szsharing.cn

TS:   "第一行\n第二行"
来源：http://fl.newstarts.cn

Java: "第一行\n第二行"
来源：http://fq.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://pe.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://bw.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://qg.nicolike.cn

[A14] 注释写法
来源：http://mw.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cp.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xk.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://wf.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://hd.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lw.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://kl.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ju.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://zt.colortex.cn

[A15] 空值判断与默认值
来源：http://kj.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://yg.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://px.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ti.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://rk.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xr.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://hb.nicolike.cn

Ruby: value = data || "默认值"
来源：http://zr.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://yc.haigaiapp.cn

[A16] 真假值判断规则
来源：http://zz.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yy.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vc.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mk.wgjwhj.cn

TS:   if (!x) {}
来源：http://kt.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ym.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nn.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ci.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ap.chemitech.net.cn

[A17] 位运算
来源：http://nl.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://np.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hd.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iw.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hr.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://cx.colortex.cn

Py:   ord("A"); chr(65)
来源：http://bq.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://ew.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hc.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yn.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://pq.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cw.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://xl.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://og.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://cd.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://pj.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ph.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://cj.colortex.cn

TS:   [a, b] = [b, a];
来源：http://dn.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://go.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://ym.chemitech.net.cn

Ruby: a, b = b, a
来源：http://lu.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://kn.haigaiapp.cn

[A20] 读取标准输入
来源：http://qj.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://wm.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ls.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rr.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://ij.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://ft.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gz.panjiajie.cn

Ruby: gets.chomp
来源：http://tx.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://fg.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://sd.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://br.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gj.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://sr.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://yc.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://hs.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wd.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://po.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://nq.yuexingan06.cn

[A22] 获取字符串长度
来源：http://rr.szsharing.cn

Py:   len(s)
来源：http://ky.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ym.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://al.lnxyls.cn

TS:   s.length
来源：http://cc.hahajie.cn

Java: s.length()
来源：http://oa.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qg.521024.cn

Ruby: s.length
来源：http://fp.9csxet.cn

C#:   s.Length
来源：http://sw.hnjuh.cn

[A23] 大小写转换
来源：http://kl.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lb.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jg.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vw.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ke.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oc.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tq.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ht.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://my.yuexingan06.cn

[A24] 去除首尾空白
来源：http://mt.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hh.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mx.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tl.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qy.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bq.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://su.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wp.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kr.huanxung.cn

[A25] 字符串比较
来源：http://se.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://sz.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yq.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lk.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cq.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yl.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ah.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zf.wgjwhj.cn

[A26] 类型转换总览
来源：http://ta.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xl.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rt.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wq.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://yy.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zm.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jb.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ph.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jw.yuexingan06.cn

================================================================================
来源：http://ky.jctech888.com.cn

B. 流程控制
来源：http://on.jctech888.com.cn

================================================================================
来源：http://pr.521024.cn

[B01] 条件判断 if / else
来源：http://wd.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uc.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://on.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ue.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pp.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rc.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nl.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ws.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lv.nszjky.cn

[B02] 多分支 else if / elif
来源：http://vp.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zz.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vm.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://be.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qk.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qs.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wl.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gg.nszjky.cn

[B03] switch / match / case
来源：http://wc.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hp.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qw.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sa.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nm.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zv.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qj.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eq.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dn.jianghongdianzi.cn

[B04] for 计数循环
来源：http://bz.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://hf.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iy.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ua.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xh.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tx.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cl.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://on.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ns.colortex.cn

[B05] 遍历数组 / 列表
来源：http://uz.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://nf.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://is.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zp.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cu.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zr.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hx.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://sy.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://hg.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://om.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qk.9csxet.cn


<!-- 参考信息 -->