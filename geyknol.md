代发 wailian999

JS:   const PI = 3.14159;
来源：http://qe.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://ue.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://cr.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://jv.huanxung.cn

Ruby: PI = 3.14159
来源：http://uw.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://rn.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://cb.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oj.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eb.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aj.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ia.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://we.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vv.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cr.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://av.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://ir.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jp.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yq.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ju.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yf.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://ie.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://tz.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://pw.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ho.muxihuayi.cn

[A06] 字符串转数字
来源：http://go.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://vb.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iq.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pm.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://en.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hr.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hx.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qq.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oi.newstarts.cn

[A07] 数字转字符串
来源：http://tb.szxytkj.cn

Py:   str(42)
来源：http://xe.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://kw.521024.cn

JS:   String(42); (42).toString()
来源：http://ls.hahajie.cn

TS:   String(42)
来源：http://jt.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pz.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://rm.szsharing.cn

Ruby: 42.to_s
来源：http://sh.shxzskj.cn

C#:   42.ToString()
来源：http://os.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://yz.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bm.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oa.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://py.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fm.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://is.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sp.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ug.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rj.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://nc.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://br.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gm.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://me.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sl.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hr.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xq.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pp.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kt.szsharing.cn

[A10] 生成随机数
来源：http://it.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://bv.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://xo.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oh.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hr.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://bu.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uh.yuexingan06.cn

Ruby: rand(1..100)
来源：http://hb.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://bf.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://qn.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tu.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tv.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://so.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://da.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://cp.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rm.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ia.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vh.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://jh.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zi.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://id.521024.cn

JS:   `Hello, ${name}!`
来源：http://pm.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://wj.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://kb.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vv.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://jb.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://wz.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://og.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://rb.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://ol.nszjky.cn

JS:   "第一行\n第二行"
来源：http://aa.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://dt.hahajie.cn

Java: "第一行\n第二行"
来源：http://bm.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://jr.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ze.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://eh.hnjuh.cn

[A14] 注释写法
来源：http://dd.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yr.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://al.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://iv.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://yj.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iz.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://vi.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xc.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://br.panjiajie.cn

[A15] 空值判断与默认值
来源：http://sm.szxytkj.cn

Py:   value = data or "默认值"
来源：http://sv.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://cn.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://jg.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://fr.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ev.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://yk.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://pr.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://hf.shtwfgs.cn

[A16] 真假值判断规则
来源：http://zr.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xv.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lu.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ck.9csxet.cn

TS:   if (!x) {}
来源：http://yg.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fb.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oq.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ko.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fm.muxihuayi.cn

[A17] 位运算
来源：http://zg.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://al.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://es.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jm.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ig.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qm.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nk.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ga.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://nx.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://ul.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://yx.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qi.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qr.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://fp.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bl.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://zf.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ss.gzmigu.cn

[A19] 交换两个变量
来源：http://ac.colortex.cn

Py:   a, b = b, a
来源：http://sy.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wh.asd995.cn

JS:   [a, b] = [b, a];
来源：http://iq.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://vn.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://nn.shxzskj.cn

Go:   a, b = b, a
来源：http://sl.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://vx.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://ef.gzmigu.cn

[A20] 读取标准输入
来源：http://ld.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://nd.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dc.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wg.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ep.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://zl.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ui.huixiangedu.cn

Ruby: gets.chomp
来源：http://su.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://tj.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://vj.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://et.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ht.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://bl.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://bq.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://di.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bm.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://ml.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://qw.asd995.cn

[A22] 获取字符串长度
来源：http://bp.huixiangedu.cn

Py:   len(s)
来源：http://qc.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qb.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mj.shxzukj.cn

TS:   s.length
来源：http://se.szsharing.cn

Java: s.length()
来源：http://hh.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nk.yuexingan06.cn

Ruby: s.length
来源：http://nr.shtwfgs.cn

C#:   s.Length
来源：http://is.muxihuayi.cn

[A23] 大小写转换
来源：http://pe.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ic.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://av.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ax.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ju.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fm.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pf.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oh.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vx.huixiangedu.cn

[A24] 去除首尾空白
来源：http://fp.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gm.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sb.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zt.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ju.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yp.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://jo.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gq.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hx.chemitech.net.cn

[A25] 字符串比较
来源：http://db.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://oe.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dc.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ke.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ur.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mh.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sc.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qn.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kn.muxihuayi.cn

[A26] 类型转换总览
来源：http://si.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dg.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tb.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mm.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://wv.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pg.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zg.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zb.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fd.panjiajie.cn

================================================================================
来源：http://vw.hnjuh.cn

B. 流程控制
来源：http://et.huixiangedu.cn

================================================================================
来源：http://gy.huanxung.cn

[B01] 条件判断 if / else
来源：http://sb.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://er.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ph.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://av.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bq.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rr.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wn.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vc.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cc.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://id.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ua.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rb.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yr.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ij.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sl.jianghongdianzi.cn

[B03] switch / match / case
来源：http://qf.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uh.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ua.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tb.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ju.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sf.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vc.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://no.szsharing.cn

[B04] for 计数循环
来源：http://sx.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://dx.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nt.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hc.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cb.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kd.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://go.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://eq.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sm.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://vb.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://pf.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wm.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zt.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fq.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fb.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hj.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ea.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jz.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://nq.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wp.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ms.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eg.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ks.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dd.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lb.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yh.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pj.asd995.cn

[B07] while 循环
来源：http://qb.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://nf.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bu.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://vh.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://wv.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://og.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bn.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://mh.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://jj.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://zx.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://sw.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qk.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://hu.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://lt.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://wb.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bx.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vr.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://jd.521024.cn

[B09] break 与 continue
来源：http://xk.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://li.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xb.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ua.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eq.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ya.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ao.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://me.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.nszjky.cn

[B10] 遍历同时拿索引
来源：http://qf.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://px.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ny.bjjhwx.cn


<!-- 参考信息 -->