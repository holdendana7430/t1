代发 wailian999

JS:   const PI = 3.14159;
来源：http://bu.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://uk.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://fd.nszjky.cn

Go:   const PI = 3.14159
来源：http://cg.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://jl.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://fp.asd995.cn

[A04] 判断变量类型
来源：http://tv.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xw.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gu.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pj.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ir.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wo.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ym.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hi.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://zl.wgjwhj.cn

[A05] 整数除法与取模
来源：http://yd.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://br.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ci.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bz.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bw.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://lk.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://ya.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://rj.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://zy.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ck.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://cu.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hq.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zd.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oa.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nh.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nh.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bc.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vr.9csxet.cn

[A07] 数字转字符串
来源：http://rv.shtwfgs.cn

Py:   str(42)
来源：http://xw.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ov.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://gd.yuntaijiaju.cn

TS:   String(42)
来源：http://eu.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fb.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://re.colortex.cn

Ruby: 42.to_s
来源：http://yr.huixiangedu.cn

C#:   42.ToString()
来源：http://oh.gzmigu.cn

[A08] 取整与四舍五入
来源：http://kp.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lv.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qt.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gw.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qh.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eg.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kb.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cd.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cs.asd995.cn

[A09] 绝对值与最大最小值
来源：http://lc.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dq.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yy.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hu.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lr.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oh.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lw.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cd.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bs.muxihuayi.cn

[A10] 生成随机数
来源：http://xy.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://fq.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://bq.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yy.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fd.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://sh.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jk.521024.cn

Ruby: rand(1..100)
来源：http://ku.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://oh.asd995.cn

[A11] 条件表达式（三元）
来源：http://ow.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://id.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ok.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wb.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sx.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://co.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ho.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zk.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://do.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://wt.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cu.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wj.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://zj.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://mp.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://hp.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jy.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://fr.521024.cn

C#:   $"Hello, {name}!"
来源：http://hd.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ny.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://sq.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://ro.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://tl.szsharing.cn

TS:   "第一行\n第二行"
来源：http://nr.newstarts.cn

Java: "第一行\n第二行"
来源：http://iq.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://uv.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://te.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://pt.yuntaijiaju.cn

[A14] 注释写法
来源：http://xa.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kc.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fl.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://xt.521024.cn

TS:   // 单行；/* 多行 */
来源：http://fa.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jc.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://cy.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rp.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://aa.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://tg.hahajie.cn

Py:   value = data or "默认值"
来源：http://qm.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://le.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://st.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://wt.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ux.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://hn.9csxet.cn

Ruby: value = data || "默认值"
来源：http://ll.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://he.yuexingan06.cn

[A16] 真假值判断规则
来源：http://ro.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uh.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eu.huanxung.cn

TS:   if (!x) {}
来源：http://ur.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ug.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://on.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sr.9csxet.cn

[A17] 位运算
来源：http://xu.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bx.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lv.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pk.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zs.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rl.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://du.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://ft.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://ku.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://vr.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dv.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ce.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://cu.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vf.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://bv.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://hc.huanxung.cn

[A19] 交换两个变量
来源：http://mk.gzmigu.cn

Py:   a, b = b, a
来源：http://zn.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hi.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://zx.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://dl.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://kc.nicolike.cn

Go:   a, b = b, a
来源：http://ga.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://bu.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://zd.hahajie.cn

[A20] 读取标准输入
来源：http://pa.colortex.cn

Py:   name = input("请输入：")
来源：http://be.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yd.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hu.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://or.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://cg.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://es.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://al.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ql.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://mw.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://bg.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jo.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://rp.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://gy.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ml.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oi.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://tq.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://kz.hnjuh.cn

[A22] 获取字符串长度
来源：http://lo.haigaiapp.cn

Py:   len(s)
来源：http://py.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://no.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xg.huanxung.cn

TS:   s.length
来源：http://nj.wgjwhj.cn

Java: s.length()
来源：http://bj.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lt.chemitech.net.cn

Ruby: s.length
来源：http://gx.bjjhwx.cn

C#:   s.Length
来源：http://kq.hnjuh.cn

[A23] 大小写转换
来源：http://rq.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dx.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lp.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dz.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fz.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fg.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mw.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ph.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cg.asd995.cn

[A24] 去除首尾空白
来源：http://hl.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ip.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mt.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ps.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ev.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://qc.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://my.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kf.lnxyls.cn

[A25] 字符串比较
来源：http://fv.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://cc.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rz.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yz.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qs.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tx.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ij.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://np.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mc.nszjky.cn

[A26] 类型转换总览
来源：http://xi.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bf.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://md.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ie.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://cu.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pl.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://de.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uq.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pq.huixinmuqiang.cn

================================================================================
来源：http://bo.gzmigu.cn

B. 流程控制
来源：http://ea.hahajie.cn

================================================================================
来源：http://er.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://jw.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wz.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ma.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hl.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ys.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lw.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://an.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xw.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vk.9csxet.cn

[B02] 多分支 else if / elif
来源：http://if.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ym.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fd.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vn.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pr.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gy.newstarts.cn

[B03] switch / match / case
来源：http://qk.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ff.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ql.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tl.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ys.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://if.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://si.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lf.bjjhwx.cn

[B04] for 计数循环
来源：http://cu.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://le.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vb.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ni.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cr.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jh.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://gq.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yk.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://nc.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://pd.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gk.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yv.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://us.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mq.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wg.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://jc.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eo.521024.cn

[B06] 遍历字典 / 对象
来源：http://lw.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fh.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hq.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iw.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ff.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ox.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iq.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rb.colortex.cn

[B07] while 循环
来源：http://at.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://xt.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zt.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://ux.521024.cn

TS:   while (i < 10) { i++; }
来源：http://ka.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://nr.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ju.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ng.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ps.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://zm.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://hd.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vo.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://vs.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://kv.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://fn.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gq.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ly.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://mn.szsharing.cn

[B09] break 与 continue
来源：http://zk.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lk.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sc.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sa.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eq.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uc.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bu.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rb.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://hs.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jr.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nu.yuntaijiaju.cn


<!-- 参考信息 -->