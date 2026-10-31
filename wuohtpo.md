代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://la.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wo.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zx.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qo.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mh.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hx.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kr.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://is.huixinmuqiang.cn

================================================================================
来源：http://lt.shxzskj.cn

A. 基础语法与类型
来源：http://ky.jctech888.com.cn

================================================================================
来源：http://vl.colortex.cn

[A01] Hello World
来源：http://kg.hahajie.cn

Py:   print("Hello, World!")
来源：http://zv.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://no.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://zz.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ay.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://iw.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://xn.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://cg.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ss.huanxung.cn

[A02] 变量声明与赋值
来源：http://od.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ca.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uq.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xj.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ia.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://by.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://pt.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://gs.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kc.lnxyls.cn

[A03] 常量定义
来源：http://mw.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ue.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://my.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://eb.521024.cn

TS:   const PI: number = 3.14159;
来源：http://gs.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://iv.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://fi.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://bi.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://kk.wgjwhj.cn

[A04] 判断变量类型
来源：http://vt.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lq.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xl.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zx.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://is.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://os.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bl.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qw.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://uc.9csxet.cn

[A05] 整数除法与取模
来源：http://gu.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bp.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cm.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://px.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://yf.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://my.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://sm.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://nt.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://ij.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://fn.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hn.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lu.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yx.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ou.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vb.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zn.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://um.521024.cn

[A07] 数字转字符串
来源：http://kr.haigaiapp.cn

Py:   str(42)
来源：http://iz.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://gt.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://cn.yuexingan06.cn

TS:   String(42)
来源：http://rw.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ax.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://kz.jctech888.com.cn

Ruby: 42.to_s
来源：http://sy.521024.cn

C#:   42.ToString()
来源：http://xn.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://qp.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bg.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://as.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pl.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ja.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nz.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vc.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xy.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vk.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ze.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cs.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rk.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ub.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ip.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wz.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bz.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lu.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rz.asd995.cn

[A10] 生成随机数
来源：http://kg.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://bg.nszjky.cn

PHP:  random_int(1, 100);
来源：http://gc.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dq.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kg.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://fu.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bv.panjiajie.cn

Ruby: rand(1..100)
来源：http://dr.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://mi.9csxet.cn

[A11] 条件表达式（三元）
来源：http://mi.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://gp.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bu.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xv.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oz.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://yr.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ni.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oz.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mr.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://nk.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ax.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://je.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://zu.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://lu.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://be.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ed.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://wz.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://gm.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vw.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://nn.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://qj.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://lh.9csxet.cn

TS:   "第一行\n第二行"
来源：http://fm.hnjuh.cn

Java: "第一行\n第二行"
来源：http://vv.521024.cn

Go:   "第一行\n第二行"
来源：http://qc.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://oe.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://aj.nicolike.cn

[A14] 注释写法
来源：http://jz.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://od.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://iy.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ni.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://do.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yf.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://up.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://my.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://pd.asd995.cn

[A15] 空值判断与默认值
来源：http://at.hnjuh.cn

Py:   value = data or "默认值"
来源：http://fr.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://cq.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://nt.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://nx.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gr.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ao.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://sd.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://up.asd995.cn

[A16] 真假值判断规则
来源：http://wj.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fb.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nw.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nx.nicolike.cn

TS:   if (!x) {}
来源：http://yr.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yc.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fw.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ls.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xj.bjjhwx.cn

[A17] 位运算
来源：http://qd.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kt.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://li.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kv.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xj.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nm.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://is.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://dg.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://sa.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://yb.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qb.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xm.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://hf.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mn.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://kp.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://bz.szsharing.cn

[A19] 交换两个变量
来源：http://wb.jctech888.com.cn

Py:   a, b = b, a
来源：http://ly.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oe.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://nx.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://rz.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://lj.bjjhwx.cn

Go:   a, b = b, a
来源：http://sd.yuexingan06.cn

Ruby: a, b = b, a
来源：http://xz.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://kk.huanxung.cn

[A20] 读取标准输入
来源：http://bd.newstarts.cn

Py:   name = input("请输入：")
来源：http://aj.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pg.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sa.colortex.cn

TS:   // Node.js：readline 模块
来源：http://xm.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://vp.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://id.bjjhwx.cn

Ruby: gets.chomp
来源：http://bp.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://gm.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://cq.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://vx.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://or.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://ms.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ry.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://yu.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zo.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://wo.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://uu.gzmigu.cn

[A22] 获取字符串长度
来源：http://gk.hahajie.cn

Py:   len(s)
来源：http://mo.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jg.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ke.jctech888.com.cn

TS:   s.length
来源：http://ev.9csxet.cn

Java: s.length()
来源：http://jm.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://we.szsharing.cn

Ruby: s.length
来源：http://ec.521024.cn

C#:   s.Length
来源：http://gl.chemitech.net.cn

[A23] 大小写转换
来源：http://uh.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vy.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dy.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wv.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hx.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qw.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mp.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ah.shxzskj.cn

[A24] 去除首尾空白
来源：http://td.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://if.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zn.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wu.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://po.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qg.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://gj.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pz.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dp.yuexingan06.cn

[A25] 字符串比较
来源：http://jp.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sd.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ez.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xm.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ws.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xi.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vm.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wk.9csxet.cn

[A26] 类型转换总览
来源：http://ze.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ns.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aa.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ll.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://az.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kf.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ek.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jw.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vd.lnxyls.cn

================================================================================
来源：http://lt.hahajie.cn

B. 流程控制
来源：http://vq.newstarts.cn

================================================================================
来源：http://fn.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://gg.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qd.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jb.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://no.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://co.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pt.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ph.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ex.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lc.9csxet.cn

[B02] 多分支 else if / elif
来源：http://ok.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ag.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dd.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lt.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://es.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cq.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.9csxet.cn

[B03] switch / match / case
来源：http://sq.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vv.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fh.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yc.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ok.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wn.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sj.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mb.szxytkj.cn

[B04] for 计数循环
来源：http://fq.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://rk.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qc.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pb.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sl.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vc.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nu.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://fa.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rj.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://in.colortex.cn

Py:   for item in arr: print(item)
来源：http://mb.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://me.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gh.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fs.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eo.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bb.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ln.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fc.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://jl.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lt.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jo.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ur.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gx.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gy.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://am.asd995.cn


<!-- 参考信息 -->