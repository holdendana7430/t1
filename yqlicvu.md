代发 wailian999

================================================================================
来源：http://wv.9csxet.cn

A. 基础语法与类型
来源：http://gi.newstarts.cn

================================================================================
来源：http://zs.shxzskj.cn

[A01] Hello World
来源：http://gy.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ko.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://ug.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://hv.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uc.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://iu.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://ud.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://dw.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://do.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://mj.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rk.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yv.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://in.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ed.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://il.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://jp.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://ze.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zc.nicolike.cn

[A03] 常量定义
来源：http://mv.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://df.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://qb.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ne.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://vx.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://fv.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://op.nszjky.cn

Ruby: PI = 3.14159
来源：http://uq.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://bs.jctech888.com.cn

[A04] 判断变量类型
来源：http://al.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pt.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ye.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nt.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://eb.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zl.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jh.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sz.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://fw.panjiajie.cn

[A05] 整数除法与取模
来源：http://cr.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ts.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zr.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nk.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ag.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://pw.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://zi.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://wi.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://ev.szsharing.cn

[A06] 字符串转数字
来源：http://vz.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://ue.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fo.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ae.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hx.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kp.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mx.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ev.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bi.521024.cn

[A07] 数字转字符串
来源：http://bs.521024.cn

Py:   str(42)
来源：http://cx.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://hb.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://em.shxzskj.cn

TS:   String(42)
来源：http://zs.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ky.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://zc.newstarts.cn

Ruby: 42.to_s
来源：http://jb.hahajie.cn

C#:   42.ToString()
来源：http://ud.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://vd.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xg.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lu.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zt.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ar.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pa.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://np.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mm.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hx.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://oz.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ed.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ka.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bi.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ds.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://on.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rq.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yj.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ii.huixiangedu.cn

[A10] 生成随机数
来源：http://tk.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://bs.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://qf.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://we.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rc.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://gg.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pk.newstarts.cn

Ruby: rand(1..100)
来源：http://xv.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://hv.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://qb.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://kr.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mz.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mz.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lq.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://dk.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ga.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rp.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ua.521024.cn

[A12] 字符串插值 / 格式化
来源：http://ba.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ja.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fv.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://qi.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://cm.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://jl.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ke.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://xh.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://sg.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ac.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://ay.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://qr.huanxung.cn

JS:   "第一行\n第二行"
来源：http://ry.huanxung.cn

TS:   "第一行\n第二行"
来源：http://st.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://gm.colortex.cn

Go:   "第一行\n第二行"
来源：http://ha.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://uc.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://cd.colortex.cn

[A14] 注释写法
来源：http://lt.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tu.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ji.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://vk.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://vn.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://np.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://dy.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lj.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://zw.nszjky.cn

[A15] 空值判断与默认值
来源：http://we.hnjuh.cn

Py:   value = data or "默认值"
来源：http://mv.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://eo.521024.cn

JS:   const value = data ?? "默认值";
来源：http://il.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://bf.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cc.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://oz.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://dw.521024.cn

C#:   var value = data ?? "默认值";
来源：http://og.szxytkj.cn

[A16] 真假值判断规则
来源：http://ty.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ts.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://el.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ud.szsharing.cn

TS:   if (!x) {}
来源：http://br.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xy.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wi.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gj.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ro.shxzukj.cn

[A17] 位运算
来源：http://vo.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jw.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://em.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tk.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mm.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nz.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://tf.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://pv.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ui.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fj.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hy.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://sx.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rs.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://zz.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://sz.yuexingan06.cn

[A19] 交换两个变量
来源：http://iz.jctech888.com.cn

Py:   a, b = b, a
来源：http://xa.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rt.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ju.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://kc.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://nx.521024.cn

Go:   a, b = b, a
来源：http://co.asd995.cn

Ruby: a, b = b, a
来源：http://qi.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://mo.muxihuayi.cn

[A20] 读取标准输入
来源：http://in.lnxyls.cn

Py:   name = input("请输入：")
来源：http://wc.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qs.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wi.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://ew.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://tj.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ka.newstarts.cn

Ruby: gets.chomp
来源：http://eh.szxytkj.cn

C#:   Console.ReadLine();
来源：http://kl.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://xj.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://hi.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xz.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://mx.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://lj.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://bu.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qg.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://dj.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://uj.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://mr.muxihuayi.cn

Py:   len(s)
来源：http://mz.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ei.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sd.yuexingan06.cn

TS:   s.length
来源：http://cz.jctech888.com.cn

Java: s.length()
来源：http://tz.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dw.muxihuayi.cn

Ruby: s.length
来源：http://pl.colortex.cn

C#:   s.Length
来源：http://pa.huixiangedu.cn

[A23] 大小写转换
来源：http://hf.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hk.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dp.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kb.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rz.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://st.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dl.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lr.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ed.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://ar.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://et.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eg.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dn.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tf.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xd.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://op.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rg.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yw.szxytkj.cn

[A25] 字符串比较
来源：http://qr.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://ts.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qs.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nb.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hs.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://le.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dt.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://id.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rd.muxihuayi.cn

[A26] 类型转换总览
来源：http://gy.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://an.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kk.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uo.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://zd.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wy.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zn.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tv.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ix.yuntaijiaju.cn

================================================================================
来源：http://sm.newstarts.cn

B. 流程控制
来源：http://nh.hahajie.cn

================================================================================
来源：http://bt.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://by.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xg.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://be.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hr.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uf.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://of.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xl.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zq.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zg.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ut.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dg.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gy.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zr.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://my.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jq.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rj.jianghongdianzi.cn

[B03] switch / match / case
来源：http://xk.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fs.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tu.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hq.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hi.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gt.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zx.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yn.jctech888.com.cn

[B04] for 计数循环
来源：http://ql.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ai.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://et.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tf.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sp.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yz.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://by.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://ip.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gd.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://aw.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ns.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iu.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hw.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rk.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ci.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mo.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://nf.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://si.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://fd.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ib.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ku.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vj.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yl.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tx.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://er.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ae.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oa.chemitech.net.cn

[B07] while 循环
来源：http://wh.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://rp.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qs.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://wc.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://mu.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ca.szsharing.cn


<!-- 参考信息 -->