代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://sq.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://vm.colortex.cn

Ruby: puts "Hello, World!"
来源：http://ej.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hf.panjiajie.cn

[A02] 变量声明与赋值
来源：http://wr.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ac.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sx.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://np.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cb.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://ha.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://jf.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://xr.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sa.nicolike.cn

[A03] 常量定义
来源：http://rl.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://do.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://ex.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://vj.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://hd.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://jz.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://xe.shxzukj.cn

Ruby: PI = 3.14159
来源：http://oa.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://lu.bjjhwx.cn

[A04] 判断变量类型
来源：http://mt.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vu.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tj.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ym.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://be.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tj.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xb.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fx.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://im.hnjuh.cn

[A05] 整数除法与取模
来源：http://de.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jm.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pm.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mf.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ib.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://tv.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://it.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://et.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://ks.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://pf.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://hi.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gf.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oy.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kn.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lx.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tp.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ct.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jz.newstarts.cn

[A07] 数字转字符串
来源：http://vp.yuntaijiaju.cn

Py:   str(42)
来源：http://aa.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://bu.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://ek.521024.cn

TS:   String(42)
来源：http://rj.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dx.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://qq.gzmigu.cn

Ruby: 42.to_s
来源：http://eq.huixiangedu.cn

C#:   42.ToString()
来源：http://ee.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://uy.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jm.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pg.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bm.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nh.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://se.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vd.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dp.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gq.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://ca.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qy.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ay.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tz.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kx.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://te.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pl.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://li.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ag.huanxung.cn

[A10] 生成随机数
来源：http://zl.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://xw.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://br.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fk.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://pc.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jf.shtwfgs.cn

Ruby: rand(1..100)
来源：http://wd.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://hs.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://ym.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://ya.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yu.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eu.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ap.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://fe.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://go.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ms.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ir.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://oj.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fy.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uw.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://qe.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://as.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://vc.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oq.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ha.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://uq.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rw.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://wa.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://au.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://tu.hahajie.cn

TS:   "第一行\n第二行"
来源：http://ye.newstarts.cn

Java: "第一行\n第二行"
来源：http://xi.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://kv.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://dy.521024.cn

C#:   "第一行\n第二行"
来源：http://it.hahajie.cn

[A14] 注释写法
来源：http://da.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://av.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ra.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://cg.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://gw.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gd.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://uv.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ra.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://ek.gzmigu.cn

[A15] 空值判断与默认值
来源：http://zs.9csxet.cn

Py:   value = data or "默认值"
来源：http://xq.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://od.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://sp.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://ma.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://as.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://vl.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://vh.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://ft.bjjhwx.cn

[A16] 真假值判断规则
来源：http://iu.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ln.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qg.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sw.shxzukj.cn

TS:   if (!x) {}
来源：http://jo.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yo.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wl.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fb.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ck.nicolike.cn

[A17] 位运算
来源：http://mu.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ag.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xv.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uq.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yy.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xa.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ir.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://tb.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://sz.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://rp.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ro.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qi.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://lt.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ay.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://qc.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://xq.haigaiapp.cn

[A19] 交换两个变量
来源：http://ei.521024.cn

Py:   a, b = b, a
来源：http://cb.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oy.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://ye.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://er.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://wc.colortex.cn

Go:   a, b = b, a
来源：http://ps.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://zb.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://uv.szsharing.cn

[A20] 读取标准输入
来源：http://bc.521024.cn

Py:   name = input("请输入：")
来源：http://dz.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ux.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yg.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://en.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://yf.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hf.9csxet.cn

Ruby: gets.chomp
来源：http://rf.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://tf.szsharing.cn

[A21] 保留指定小数位输出
来源：http://gz.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://tw.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lk.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://un.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://rb.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://tx.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://by.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://om.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://mh.colortex.cn

[A22] 获取字符串长度
来源：http://ay.jctech888.com.cn

Py:   len(s)
来源：http://om.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://il.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jb.yuntaijiaju.cn

TS:   s.length
来源：http://pj.asd995.cn

Java: s.length()
来源：http://nm.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hi.shxzskj.cn

Ruby: s.length
来源：http://pj.chemitech.net.cn

C#:   s.Length
来源：http://dl.shxzskj.cn

[A23] 大小写转换
来源：http://cg.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yf.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gi.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xn.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iy.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jy.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qm.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://de.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nq.szsharing.cn

[A24] 去除首尾空白
来源：http://if.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lv.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qa.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xh.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pg.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ov.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://hk.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zo.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ci.hnjuh.cn

[A25] 字符串比较
来源：http://rh.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://nf.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://up.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://it.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wz.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nc.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ng.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xi.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oh.9csxet.cn

[A26] 类型转换总览
来源：http://nz.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hp.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ql.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qh.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://rp.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ib.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ig.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://py.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kd.chemitech.net.cn

================================================================================
来源：http://fd.521024.cn

B. 流程控制
来源：http://uh.huanxung.cn

================================================================================
来源：http://xb.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://sq.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fn.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vd.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fx.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dq.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ys.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sy.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://re.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://kk.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nm.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tz.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hg.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vl.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dt.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ud.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.521024.cn

[B03] switch / match / case
来源：http://gw.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nx.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ez.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ou.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oy.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qo.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://co.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zp.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://re.huanxung.cn

[B04] for 计数循环
来源：http://fg.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://hl.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zy.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cn.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bk.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ge.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://db.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aw.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://ei.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://wh.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fd.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bq.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wr.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cu.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ty.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://uc.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vg.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://ut.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dp.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fj.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bs.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sq.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kq.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qb.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ri.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wj.szxytkj.cn

[B07] while 循环
来源：http://qn.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://ey.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vv.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://gs.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://nh.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://yy.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zu.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://gb.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://fm.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://zk.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://lg.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ji.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://wv.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://os.nszjky.cn


<!-- 参考信息 -->