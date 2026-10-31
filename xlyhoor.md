代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oy.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://li.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pc.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qu.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uv.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eu.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wz.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yi.lnxyls.cn

================================================================================
来源：http://vi.521024.cn

A. 基础语法与类型
来源：http://vq.colortex.cn

================================================================================
来源：http://uy.asd995.cn

[A01] Hello World
来源：http://hg.huanxung.cn

Py:   print("Hello, World!")
来源：http://zc.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://ce.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://qh.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kw.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://lr.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://cr.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://qa.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oj.nszjky.cn

[A02] 变量声明与赋值
来源：http://lr.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ya.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wr.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dp.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rm.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://bu.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://ks.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://yn.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://of.huixiangedu.cn

[A03] 常量定义
来源：http://ou.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cy.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://jw.szsharing.cn

JS:   const PI = 3.14159;
来源：http://dl.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://qh.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://rd.521024.cn

Go:   const PI = 3.14159
来源：http://zi.szsharing.cn

Ruby: PI = 3.14159
来源：http://gm.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://qm.hnjuh.cn

[A04] 判断变量类型
来源：http://cp.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bl.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wq.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oc.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://gq.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nm.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pw.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://go.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://tv.wgjwhj.cn

[A05] 整数除法与取模
来源：http://cw.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pu.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tw.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hc.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nq.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://vd.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://zh.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://te.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://fn.szsharing.cn

[A06] 字符串转数字
来源：http://uo.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://bc.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ft.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fw.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qr.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yw.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hq.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bv.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://po.muxihuayi.cn

[A07] 数字转字符串
来源：http://jg.huixinmuqiang.cn

Py:   str(42)
来源：http://xp.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://lr.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://wb.huixinmuqiang.cn

TS:   String(42)
来源：http://se.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lk.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://gt.521024.cn

Ruby: 42.to_s
来源：http://rq.gzmigu.cn

C#:   42.ToString()
来源：http://bq.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://nt.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yl.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cz.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ae.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eb.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bd.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xz.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vs.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://no.521024.cn

[A09] 绝对值与最大最小值
来源：http://er.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mv.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xr.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://il.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jn.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://el.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aa.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xd.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tb.bjjhwx.cn

[A10] 生成随机数
来源：http://qp.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://tn.9csxet.cn

PHP:  random_int(1, 100);
来源：http://ll.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kk.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oc.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://sr.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jz.hnjuh.cn

Ruby: rand(1..100)
来源：http://yq.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://mc.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://zx.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://dx.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lg.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hf.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://if.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://vt.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nd.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ig.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lb.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://sx.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vs.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ao.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://tk.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://ve.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://lb.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ad.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://xu.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://kw.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gy.szsharing.cn

Py:   "第一行\n第二行"
来源：http://bd.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://ys.nicolike.cn

JS:   "第一行\n第二行"
来源：http://aq.colortex.cn

TS:   "第一行\n第二行"
来源：http://mg.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://oc.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://mh.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://ez.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://xv.szxytkj.cn

[A14] 注释写法
来源：http://jr.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aq.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://aa.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://qp.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://io.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oj.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://zs.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qc.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://op.nszjky.cn

[A15] 空值判断与默认值
来源：http://cs.gzmigu.cn

Py:   value = data or "默认值"
来源：http://hs.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ow.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://be.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://mb.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ay.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://um.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://vx.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://fo.521024.cn

[A16] 真假值判断规则
来源：http://xp.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pr.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xv.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gh.szxytkj.cn

TS:   if (!x) {}
来源：http://rl.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vd.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zk.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bv.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vb.nicolike.cn

[A17] 位运算
来源：http://xj.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cm.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ug.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bc.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tk.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mu.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://te.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://pr.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://kr.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://qr.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yc.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vf.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://pb.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xw.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://xk.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://hr.muxihuayi.cn

[A19] 交换两个变量
来源：http://lf.wgjwhj.cn

Py:   a, b = b, a
来源：http://tt.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://id.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://gn.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://fw.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://jq.hnjuh.cn

Go:   a, b = b, a
来源：http://ck.nszjky.cn

Ruby: a, b = b, a
来源：http://lv.521024.cn

C#:   (a, b) = (b, a);
来源：http://sn.huanxung.cn

[A20] 读取标准输入
来源：http://la.nszjky.cn

Py:   name = input("请输入：")
来源：http://lo.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vk.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tv.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://bc.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ol.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://da.shxzukj.cn

Ruby: gets.chomp
来源：http://ne.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://rb.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://sa.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://uv.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ot.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://rq.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://om.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://aw.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jb.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://ij.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ez.jctech888.com.cn

[A22] 获取字符串长度
来源：http://nf.huanxung.cn

Py:   len(s)
来源：http://up.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ch.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dr.gzmigu.cn

TS:   s.length
来源：http://ut.newstarts.cn

Java: s.length()
来源：http://xp.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dm.gzmigu.cn

Ruby: s.length
来源：http://wr.wgjwhj.cn

C#:   s.Length
来源：http://wz.nicolike.cn

[A23] 大小写转换
来源：http://ph.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vc.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yv.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hb.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ix.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pg.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sy.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fp.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mq.yuexingan06.cn

[A24] 去除首尾空白
来源：http://yj.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nq.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kn.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fk.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ot.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qz.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://yg.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zm.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nr.yuntaijiaju.cn

[A25] 字符串比较
来源：http://hx.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://rj.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kj.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nr.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pp.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kx.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lr.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cq.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dj.huixiangedu.cn

[A26] 类型转换总览
来源：http://te.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xr.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kd.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sj.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://re.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ly.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wz.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fc.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rh.shxzskj.cn

================================================================================
来源：http://ih.huanxung.cn

B. 流程控制
来源：http://os.shxzukj.cn

================================================================================
来源：http://wi.nicolike.cn

[B01] 条件判断 if / else
来源：http://dj.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dt.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xg.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hv.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zs.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ee.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ce.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://do.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://us.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ie.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eb.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qa.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wq.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zy.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yl.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zi.haigaiapp.cn

[B03] switch / match / case
来源：http://tw.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ou.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://he.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://az.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://le.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dg.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bc.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://al.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ps.nszjky.cn

[B04] for 计数循环
来源：http://kl.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://cv.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ah.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bx.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jt.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mt.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://bx.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mt.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://uz.hahajie.cn

Py:   for item in arr: print(item)
来源：http://op.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qx.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gs.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zq.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://us.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://db.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://bs.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wn.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://mt.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nd.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tz.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fg.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ov.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xe.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kb.huanxung.cn


<!-- 参考信息 -->