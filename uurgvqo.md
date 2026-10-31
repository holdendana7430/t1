代发 wailian999

================================================================================
来源：http://pz.panjiajie.cn

A. 基础语法与类型
来源：http://xe.huixiangedu.cn

================================================================================
来源：http://rw.shxzukj.cn

[A01] Hello World
来源：http://tk.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://zg.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://mp.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://wc.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jb.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://jk.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ll.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://ud.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yw.colortex.cn

[A02] 变量声明与赋值
来源：http://tc.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xv.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kc.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ao.hnjuh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://su.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://ww.521024.cn

Go:   name := "Alex"; age := 20
来源：http://vx.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://bz.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yc.bookmarksfly.cn

[A03] 常量定义
来源：http://hi.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://df.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://nb.colortex.cn

JS:   const PI = 3.14159;
来源：http://nl.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://mg.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://mm.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://au.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://rx.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://gc.colortex.cn

[A04] 判断变量类型
来源：http://hr.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fz.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mk.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pf.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ng.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kt.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qi.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tm.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://ax.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://fz.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cn.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bk.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hw.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qs.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://fi.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://dd.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ll.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://jx.gzmigu.cn

[A06] 字符串转数字
来源：http://tu.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://pc.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pq.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aw.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://on.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pe.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cf.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ks.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hf.bookmarksfly.cn

[A07] 数字转字符串
来源：http://uu.yuntaijiaju.cn

Py:   str(42)
来源：http://jy.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://gh.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://xs.jianghongdianzi.cn

TS:   String(42)
来源：http://pb.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yn.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://jz.nszjky.cn

Ruby: 42.to_s
来源：http://fq.nicolike.cn

C#:   42.ToString()
来源：http://hp.521024.cn

[A08] 取整与四舍五入
来源：http://lg.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kn.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pi.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vl.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gf.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yy.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cj.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vf.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dp.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://uh.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bk.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dw.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uq.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eu.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ot.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ug.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pw.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zj.yuntaijiaju.cn

[A10] 生成随机数
来源：http://rn.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://fu.nszjky.cn

PHP:  random_int(1, 100);
来源：http://jz.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kh.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kr.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://cs.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zt.jctech888.com.cn

Ruby: rand(1..100)
来源：http://gy.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://ej.9csxet.cn

[A11] 条件表达式（三元）
来源：http://mb.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://ns.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nv.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zk.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vb.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://gr.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yk.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lk.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://je.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://wv.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ep.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kn.asd995.cn

JS:   `Hello, ${name}!`
来源：http://gi.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://ut.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ow.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://do.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://jo.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://ab.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jj.huanxung.cn

Py:   "第一行\n第二行"
来源：http://tw.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://uu.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://kn.huanxung.cn

TS:   "第一行\n第二行"
来源：http://xk.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://yr.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bz.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://ni.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://dh.yuntaijiaju.cn

[A14] 注释写法
来源：http://hi.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://de.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yw.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://gy.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://aw.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://af.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://ke.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ni.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://oy.hahajie.cn

[A15] 空值判断与默认值
来源：http://bq.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://ft.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://fb.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://hw.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://pl.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sl.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://ma.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://rd.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://px.hnjuh.cn

[A16] 真假值判断规则
来源：http://hd.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ck.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nn.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rs.huanxung.cn

TS:   if (!x) {}
来源：http://xc.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pj.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dq.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wg.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vl.gzmigu.cn

[A17] 位运算
来源：http://bx.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vk.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xr.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://id.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pa.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kr.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://yo.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://gf.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://cf.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://le.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ny.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://rs.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jg.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://zz.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://hy.hnjuh.cn

[A19] 交换两个变量
来源：http://nm.shxzukj.cn

Py:   a, b = b, a
来源：http://tf.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://km.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://zh.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://uy.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://qk.521024.cn

Go:   a, b = b, a
来源：http://mq.panjiajie.cn

Ruby: a, b = b, a
来源：http://kc.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://pu.haigaiapp.cn

[A20] 读取标准输入
来源：http://da.asd995.cn

Py:   name = input("请输入：")
来源：http://zy.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ty.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gm.asd995.cn

TS:   // Node.js：readline 模块
来源：http://zn.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ig.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dd.9csxet.cn

Ruby: gets.chomp
来源：http://ix.hahajie.cn

C#:   Console.ReadLine();
来源：http://mt.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://tk.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://im.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dq.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://dw.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ev.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://tm.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jk.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://fq.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://fz.huixiangedu.cn

[A22] 获取字符串长度
来源：http://eb.gzmigu.cn

Py:   len(s)
来源：http://qb.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ng.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bo.huanxung.cn

TS:   s.length
来源：http://vn.jianghongdianzi.cn

Java: s.length()
来源：http://rz.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mc.newstarts.cn

Ruby: s.length
来源：http://ss.bjjhwx.cn

C#:   s.Length
来源：http://ez.yuexingan06.cn

[A23] 大小写转换
来源：http://ad.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ss.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bg.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hh.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yp.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ua.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hy.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://av.haigaiapp.cn

[A24] 去除首尾空白
来源：http://mx.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cf.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://om.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gs.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bv.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ev.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://cc.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hk.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vw.muxihuayi.cn

[A25] 字符串比较
来源：http://nn.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://nf.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iu.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pq.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mz.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zc.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pb.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bl.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mi.nszjky.cn

[A26] 类型转换总览
来源：http://eb.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://na.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rz.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jj.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://no.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dv.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pm.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qu.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zk.jctech888.com.cn

================================================================================
来源：http://we.newstarts.cn

B. 流程控制
来源：http://zu.muxihuayi.cn

================================================================================
来源：http://ry.szsharing.cn

[B01] 条件判断 if / else
来源：http://hv.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rh.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lw.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zd.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tl.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dr.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://px.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nm.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fy.newstarts.cn

[B02] 多分支 else if / elif
来源：http://dl.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wr.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bq.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aa.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fa.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.lnxyls.cn

[B03] switch / match / case
来源：http://nc.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mv.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lp.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://it.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bf.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fa.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ed.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pm.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mm.gzmigu.cn

[B04] for 计数循环
来源：http://if.asd995.cn

Py:   for i in range(10): print(i)
来源：http://fu.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aq.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://av.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gq.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sk.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fa.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://cv.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cz.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://au.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://mv.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eg.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bk.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tu.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qa.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nz.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://tz.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ul.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://ie.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bv.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yp.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lg.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://du.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://og.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cz.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jv.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aj.yuntaijiaju.cn

[B07] while 循环
来源：http://mk.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://wg.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ue.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://mt.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://co.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://fz.hahajie.cn


<!-- 参考信息 -->