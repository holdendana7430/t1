代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://og.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uv.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zb.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hr.lnxyls.cn

================================================================================
来源：http://qv.huixinmuqiang.cn

A. 基础语法与类型
来源：http://qm.jctech888.com.cn

================================================================================
来源：http://gd.huanxung.cn

[A01] Hello World
来源：http://so.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://lx.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://kj.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://yc.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bm.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://rf.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://rf.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://bk.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ge.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://oh.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jz.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gt.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zz.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cd.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://rh.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://oi.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://nx.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ey.yuexingan06.cn

[A03] 常量定义
来源：http://qs.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hv.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://bn.szsharing.cn

JS:   const PI = 3.14159;
来源：http://pm.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://op.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://qh.9csxet.cn

Go:   const PI = 3.14159
来源：http://ii.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://zx.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://gu.shxzskj.cn

[A04] 判断变量类型
来源：http://km.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vf.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ik.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oj.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://rz.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vo.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vh.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ht.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://kc.colortex.cn

[A05] 整数除法与取模
来源：http://sn.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ea.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qs.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xy.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lz.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://uv.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://ew.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://rc.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://hi.521024.cn

[A06] 字符串转数字
来源：http://bb.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://la.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://es.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xd.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yu.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rs.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kx.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://il.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lq.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://lx.jianghongdianzi.cn

Py:   str(42)
来源：http://jt.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://eu.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://dn.nicolike.cn

TS:   String(42)
来源：http://wv.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cd.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://ta.huanxung.cn

Ruby: 42.to_s
来源：http://ff.newstarts.cn

C#:   42.ToString()
来源：http://ij.nicolike.cn

[A08] 取整与四舍五入
来源：http://wt.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dz.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ao.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://af.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ie.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iq.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ev.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wt.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uj.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://iy.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zs.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sg.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gg.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qb.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nr.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ur.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wr.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qq.szsharing.cn

[A10] 生成随机数
来源：http://el.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://ct.hahajie.cn

PHP:  random_int(1, 100);
来源：http://wu.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qi.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sg.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://no.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xu.huixiangedu.cn

Ruby: rand(1..100)
来源：http://yr.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://gw.szsharing.cn

[A11] 条件表达式（三元）
来源：http://cn.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://dn.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zc.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qh.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iz.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zr.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qv.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ll.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mk.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://sz.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qf.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jl.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://yh.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://hx.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://nu.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jb.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://ft.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://qr.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qj.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://lz.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://qj.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://tl.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://cz.szsharing.cn

Java: "第一行\n第二行"
来源：http://zs.9csxet.cn

Go:   "第一行\n第二行"
来源：http://yy.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://ue.szsharing.cn

C#:   "第一行\n第二行"
来源：http://us.szxytkj.cn

[A14] 注释写法
来源：http://xc.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ul.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fl.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://nm.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://ww.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tp.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://fs.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vc.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://gi.szsharing.cn

[A15] 空值判断与默认值
来源：http://bq.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://jh.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://by.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://sx.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://dy.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ih.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://my.colortex.cn

Ruby: value = data || "默认值"
来源：http://qm.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://yg.gzmigu.cn

[A16] 真假值判断规则
来源：http://zu.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jb.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mw.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wg.gzmigu.cn

TS:   if (!x) {}
来源：http://wa.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wy.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ht.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eq.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://be.yuexingan06.cn

[A17] 位运算
来源：http://ef.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vp.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://io.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://va.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://he.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cd.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ha.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sc.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://io.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://ph.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://fm.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dj.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dt.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://qv.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bo.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ak.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://zf.colortex.cn

[A19] 交换两个变量
来源：http://yr.bookmarksfly.cn

Py:   a, b = b, a
来源：http://hd.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hk.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://xa.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://ju.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://et.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://gx.hnjuh.cn

Ruby: a, b = b, a
来源：http://yh.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://jl.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://sm.gzmigu.cn

Py:   name = input("请输入：")
来源：http://hn.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hi.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vw.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://as.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://hb.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ch.jctech888.com.cn

Ruby: gets.chomp
来源：http://nq.lnxyls.cn

C#:   Console.ReadLine();
来源：http://nt.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://ra.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://vi.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nf.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://ef.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://rg.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://aj.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://in.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://tu.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://um.521024.cn

[A22] 获取字符串长度
来源：http://wm.colortex.cn

Py:   len(s)
来源：http://gc.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://se.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pi.panjiajie.cn

TS:   s.length
来源：http://ip.huixiangedu.cn

Java: s.length()
来源：http://nn.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zf.szxytkj.cn

Ruby: s.length
来源：http://bv.colortex.cn

C#:   s.Length
来源：http://rv.panjiajie.cn

[A23] 大小写转换
来源：http://iw.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rw.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jf.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pk.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rr.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xa.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://si.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jb.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://al.hahajie.cn

[A24] 去除首尾空白
来源：http://gj.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yr.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kg.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ak.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iq.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ha.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://fl.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ou.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yb.gzmigu.cn

[A25] 字符串比较
来源：http://kh.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://pv.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xt.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rg.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://my.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cd.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tl.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ax.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ih.newstarts.cn

[A26] 类型转换总览
来源：http://zt.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hm.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yf.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ae.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://dn.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wu.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dy.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cq.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wn.nicolike.cn

================================================================================
来源：http://en.bjjhwx.cn

B. 流程控制
来源：http://fq.huixiangedu.cn

================================================================================
来源：http://ii.szxytkj.cn

[B01] 条件判断 if / else
来源：http://mq.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pc.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sj.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hj.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://le.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xp.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nk.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fg.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zm.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://dt.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ul.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rv.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qi.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vx.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ya.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://of.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.szxytkj.cn

[B03] switch / match / case
来源：http://vx.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nx.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dy.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qh.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ys.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qb.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lt.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rf.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://je.bookmarksfly.cn

[B04] for 计数循环
来源：http://mf.asd995.cn

Py:   for i in range(10): print(i)
来源：http://lb.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hb.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ie.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mh.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ii.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jq.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://lm.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vb.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://sk.huanxung.cn

Py:   for item in arr: print(item)
来源：http://jr.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://go.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ka.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bq.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mm.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vd.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://bh.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ok.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://ze.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yf.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vb.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oz.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://so.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xp.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pq.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rm.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gm.newstarts.cn

[B07] while 循环
来源：http://at.asd995.cn

Py:   while i < 10: i += 1
来源：http://se.nicolike.cn


<!-- 参考信息 -->