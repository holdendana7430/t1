代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vp.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ok.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iz.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ht.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sk.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ny.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ia.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nz.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://is.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://if.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xf.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uw.wgjwhj.cn

================================================================================
来源：http://tp.szsharing.cn

A. 基础语法与类型
来源：http://dr.muxihuayi.cn

================================================================================
来源：http://fe.nicolike.cn

[A01] Hello World
来源：http://cg.asd995.cn

Py:   print("Hello, World!")
来源：http://np.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://kz.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://ek.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mt.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://iy.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ox.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://gl.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lk.hnjuh.cn

[A02] 变量声明与赋值
来源：http://sn.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wp.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rv.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zp.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vr.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://yq.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://nq.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://kb.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ok.haigaiapp.cn

[A03] 常量定义
来源：http://yj.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ey.colortex.cn

PHP:  const PI = 3.14159;
来源：http://oh.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://hu.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://sr.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://px.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://hz.szsharing.cn

Ruby: PI = 3.14159
来源：http://pp.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://uk.bjjhwx.cn

[A04] 判断变量类型
来源：http://cn.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rx.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rr.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vi.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://md.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cd.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xl.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xw.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://um.muxihuayi.cn

[A05] 整数除法与取模
来源：http://ym.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://at.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xu.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://da.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://no.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://oo.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://dh.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://qg.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://kf.asd995.cn

[A06] 字符串转数字
来源：http://uo.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://bk.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bg.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qe.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ze.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fk.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rg.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zb.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qs.bookmarksfly.cn

[A07] 数字转字符串
来源：http://gu.colortex.cn

Py:   str(42)
来源：http://en.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://qv.colortex.cn

JS:   String(42); (42).toString()
来源：http://ru.shxzukj.cn

TS:   String(42)
来源：http://hu.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gc.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://hw.colortex.cn

Ruby: 42.to_s
来源：http://jb.hnjuh.cn

C#:   42.ToString()
来源：http://tu.hnjuh.cn

[A08] 取整与四舍五入
来源：http://ke.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mi.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mm.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xn.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qq.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jb.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wk.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kt.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qx.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://td.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gv.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yh.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jj.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vx.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hq.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gk.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yj.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mm.huixiangedu.cn

[A10] 生成随机数
来源：http://fl.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://fg.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://lp.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zs.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://km.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://px.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kx.newstarts.cn

Ruby: rand(1..100)
来源：http://fr.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://li.hahajie.cn

[A11] 条件表达式（三元）
来源：http://ey.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ib.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ae.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ib.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ki.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ma.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kv.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eu.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rw.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://md.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bf.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sh.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://gj.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://wk.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://fb.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xp.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://vg.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://or.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cn.szsharing.cn

Py:   "第一行\n第二行"
来源：http://li.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://yq.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://uy.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://sb.lnxyls.cn

Java: "第一行\n第二行"
来源：http://jt.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://bj.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://ay.nszjky.cn

C#:   "第一行\n第二行"
来源：http://ng.shxzukj.cn

[A14] 注释写法
来源：http://fh.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mi.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://es.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://kn.521024.cn

TS:   // 单行；/* 多行 */
来源：http://ki.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fz.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://pg.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zn.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://xv.hahajie.cn

[A15] 空值判断与默认值
来源：http://qd.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://nl.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://sq.521024.cn

JS:   const value = data ?? "默认值";
来源：http://rw.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://kk.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vi.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://af.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://hk.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://sp.wgjwhj.cn

[A16] 真假值判断规则
来源：http://eo.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://za.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jq.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lk.newstarts.cn

TS:   if (!x) {}
来源：http://vu.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nl.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uc.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gv.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fi.521024.cn

[A17] 位运算
来源：http://nf.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ox.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hp.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cs.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wy.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://to.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pt.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nz.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yp.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://do.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://yt.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://qh.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rr.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hb.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://uu.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cg.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://se.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://cm.bookmarksfly.cn

[A19] 交换两个变量
来源：http://cn.szxytkj.cn

Py:   a, b = b, a
来源：http://ll.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ie.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://mf.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://jv.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://os.chemitech.net.cn

Go:   a, b = b, a
来源：http://ck.nicolike.cn

Ruby: a, b = b, a
来源：http://vu.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://ba.nicolike.cn

[A20] 读取标准输入
来源：http://vv.lnxyls.cn

Py:   name = input("请输入：")
来源：http://jf.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rn.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vo.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ag.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://gv.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ex.colortex.cn

Ruby: gets.chomp
来源：http://tl.colortex.cn

C#:   Console.ReadLine();
来源：http://fe.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://qh.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://fv.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uq.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://jg.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://ec.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://xf.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xn.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ag.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://sr.shxzukj.cn

[A22] 获取字符串长度
来源：http://vy.newstarts.cn

Py:   len(s)
来源：http://fw.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vf.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://na.shtwfgs.cn

TS:   s.length
来源：http://rv.shtwfgs.cn

Java: s.length()
来源：http://dh.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://be.szxytkj.cn

Ruby: s.length
来源：http://sz.panjiajie.cn

C#:   s.Length
来源：http://dv.521024.cn

[A23] 大小写转换
来源：http://qq.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ha.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ly.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yc.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jd.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kw.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ag.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://br.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rj.gzmigu.cn

[A24] 去除首尾空白
来源：http://qg.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ew.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bj.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nx.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://my.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://of.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://eu.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xk.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xz.lnxyls.cn

[A25] 字符串比较
来源：http://sl.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://ls.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sj.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lq.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rf.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lc.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ir.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cy.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wj.muxihuayi.cn

[A26] 类型转换总览
来源：http://yr.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cv.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fp.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zj.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://kn.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vr.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://db.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dy.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ty.bookmarksfly.cn

================================================================================
来源：http://zh.jianghongdianzi.cn

B. 流程控制
来源：http://yp.huixinmuqiang.cn

================================================================================
来源：http://to.asd995.cn

[B01] 条件判断 if / else
来源：http://av.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ti.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eg.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nf.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ke.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fd.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qs.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ui.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ow.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://af.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mp.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hd.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wk.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tt.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nb.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.bjjhwx.cn

[B03] switch / match / case
来源：http://qb.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ej.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ve.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bw.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uw.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hw.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zz.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uv.szsharing.cn

[B04] for 计数循环
来源：http://kx.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://xu.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qt.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mp.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zh.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xv.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fx.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://pb.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pj.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ju.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ls.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pc.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://du.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vt.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://la.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tj.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://mv.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nx.asd995.cn

[B06] 遍历字典 / 对象
来源：http://qx.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qs.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bf.gzmigu.cn


<!-- 参考信息 -->