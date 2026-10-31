代发 wailian999

JS:   const PI = 3.14159;
来源：http://om.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://df.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://fy.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://bi.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://qy.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://ss.panjiajie.cn

[A04] 判断变量类型
来源：http://iz.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bb.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uy.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://si.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://ep.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hp.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kc.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mu.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://ig.hahajie.cn

[A05] 整数除法与取模
来源：http://qv.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pr.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jx.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://db.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oq.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://ip.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://yb.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://hv.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://nt.9csxet.cn

[A06] 字符串转数字
来源：http://nf.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://aq.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xt.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dl.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mn.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ci.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mj.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jd.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rh.shtwfgs.cn

[A07] 数字转字符串
来源：http://cs.wgjwhj.cn

Py:   str(42)
来源：http://og.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://qn.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://ur.jctech888.com.cn

TS:   String(42)
来源：http://oz.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lu.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://wv.haigaiapp.cn

Ruby: 42.to_s
来源：http://xt.muxihuayi.cn

C#:   42.ToString()
来源：http://ml.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://jv.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sj.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ba.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://er.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ys.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xt.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kt.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uh.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yw.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://iq.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://td.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mc.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ar.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ul.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vc.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bq.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gn.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rj.nszjky.cn

[A10] 生成随机数
来源：http://qg.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://hm.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://mp.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jj.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ls.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://zl.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ls.shxzskj.cn

Ruby: rand(1..100)
来源：http://rj.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://cy.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://bm.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://os.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ja.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tk.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bg.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ru.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://my.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gb.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wd.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://ex.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ok.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fy.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://xd.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://dp.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://nc.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ih.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://ks.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://vx.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tj.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://lk.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://hj.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://vm.9csxet.cn

TS:   "第一行\n第二行"
来源：http://pr.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://oo.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://tt.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://qv.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://sc.jianghongdianzi.cn

[A14] 注释写法
来源：http://pn.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zt.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tf.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://qc.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://lb.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uq.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://ic.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qv.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://cn.nicolike.cn

[A15] 空值判断与默认值
来源：http://wf.gzmigu.cn

Py:   value = data or "默认值"
来源：http://vg.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://sf.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ta.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://fw.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nb.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://wx.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://po.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://rp.nszjky.cn

[A16] 真假值判断规则
来源：http://ip.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://my.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dd.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mm.haigaiapp.cn

TS:   if (!x) {}
来源：http://df.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ex.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nj.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bx.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yc.jianghongdianzi.cn

[A17] 位运算
来源：http://bk.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gq.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zk.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sn.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pl.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zf.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bf.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://ig.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://as.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://zy.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lu.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cr.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://bn.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zc.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ng.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://qp.wgjwhj.cn

[A19] 交换两个变量
来源：http://ww.newstarts.cn

Py:   a, b = b, a
来源：http://qi.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qg.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://di.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://ax.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://dw.shtwfgs.cn

Go:   a, b = b, a
来源：http://tu.nicolike.cn

Ruby: a, b = b, a
来源：http://fk.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://pr.colortex.cn

[A20] 读取标准输入
来源：http://rw.szxytkj.cn

Py:   name = input("请输入：")
来源：http://bf.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://he.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yc.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://zb.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://uy.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oi.hahajie.cn

Ruby: gets.chomp
来源：http://we.shxzskj.cn

C#:   Console.ReadLine();
来源：http://ey.colortex.cn

[A21] 保留指定小数位输出
来源：http://ln.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ob.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cy.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://rs.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://gg.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://oo.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bk.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ts.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://rb.szsharing.cn

[A22] 获取字符串长度
来源：http://jx.521024.cn

Py:   len(s)
来源：http://wo.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xo.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kl.nicolike.cn

TS:   s.length
来源：http://jb.hnjuh.cn

Java: s.length()
来源：http://uc.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hm.huanxung.cn

Ruby: s.length
来源：http://uv.521024.cn

C#:   s.Length
来源：http://tq.521024.cn

[A23] 大小写转换
来源：http://th.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mo.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lt.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qd.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nq.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ou.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fn.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mb.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eg.szxytkj.cn

[A24] 去除首尾空白
来源：http://rj.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mp.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lx.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vo.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zt.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://vq.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://id.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ch.jctech888.com.cn

[A25] 字符串比较
来源：http://fr.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://qj.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vf.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ud.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kc.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cy.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xf.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zj.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dq.hnjuh.cn

[A26] 类型转换总览
来源：http://te.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ws.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mr.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ee.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ue.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qj.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uz.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dd.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cb.gzmigu.cn

================================================================================
来源：http://ca.9csxet.cn

B. 流程控制
来源：http://br.szxytkj.cn

================================================================================
来源：http://ch.asd995.cn

[B01] 条件判断 if / else
来源：http://mw.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ml.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vy.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fd.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vz.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xa.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fd.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ae.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zg.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://mg.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zs.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lg.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pt.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hp.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://by.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qa.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.lnxyls.cn

[B03] switch / match / case
来源：http://lt.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wb.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ni.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nl.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fh.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fi.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://po.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gh.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hr.huixinmuqiang.cn

[B04] for 计数循环
来源：http://qu.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://uv.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yt.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ow.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hc.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vi.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fc.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://ze.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lu.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://bd.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://fp.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qj.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ab.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kd.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://io.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ls.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ks.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cu.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://qb.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ks.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qw.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ds.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zq.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oe.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dh.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dk.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jv.panjiajie.cn

[B07] while 循环
来源：http://bj.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://yv.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bf.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://qj.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ii.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://nv.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uf.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://uz.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://cm.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://yo.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://bt.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vl.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://dx.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://bp.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://bu.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mt.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vg.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://bg.yuexingan06.cn

[B09] break 与 continue
来源：http://eh.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wx.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qm.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lx.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cu.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hm.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.huanxung.cn

[B10] 遍历同时拿索引
来源：http://ix.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ep.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://df.yuexingan06.cn


<!-- 参考信息 -->