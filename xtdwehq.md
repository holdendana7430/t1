代发 wailian999

Ruby: PI = 3.14159
来源：http://sv.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://tm.newstarts.cn

[A04] 判断变量类型
来源：http://fe.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ph.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xf.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hu.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://jx.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rv.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pg.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xj.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://mk.huanxung.cn

[A05] 整数除法与取模
来源：http://lv.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tk.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lx.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jh.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lz.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://sk.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://eu.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://sy.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://jz.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://nd.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://io.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kr.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fu.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tn.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tm.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gq.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ad.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qw.bjjhwx.cn

[A07] 数字转字符串
来源：http://uk.szxytkj.cn

Py:   str(42)
来源：http://cd.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://qy.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://yf.chemitech.net.cn

TS:   String(42)
来源：http://up.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mw.asd995.cn

Go:   strconv.Itoa(42)
来源：http://su.wgjwhj.cn

Ruby: 42.to_s
来源：http://oc.szxytkj.cn

C#:   42.ToString()
来源：http://xz.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://zs.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://np.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yr.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xp.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ph.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xw.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://db.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pb.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zt.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://op.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ba.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hs.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jy.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ab.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vp.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aa.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ns.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qu.asd995.cn

[A10] 生成随机数
来源：http://de.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://qe.newstarts.cn

PHP:  random_int(1, 100);
来源：http://pd.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ou.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lb.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://jx.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ri.wgjwhj.cn

Ruby: rand(1..100)
来源：http://it.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://ap.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://qv.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://qw.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rw.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lm.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yy.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://rj.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ou.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ij.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://du.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://mn.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uy.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mr.asd995.cn

JS:   `Hello, ${name}!`
来源：http://av.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://hn.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://lx.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ch.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://nn.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://lz.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ej.colortex.cn

Py:   "第一行\n第二行"
来源：http://is.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://la.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://ws.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://dg.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://pf.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://nt.asd995.cn

Ruby: "第一行\n第二行"
来源：http://rk.asd995.cn

C#:   "第一行\n第二行"
来源：http://bo.chemitech.net.cn

[A14] 注释写法
来源：http://lk.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ze.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zw.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://se.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://yg.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://si.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://dp.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ma.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://bc.newstarts.cn

[A15] 空值判断与默认值
来源：http://qu.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://ay.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://dw.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://gs.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://si.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hm.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://ft.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://uc.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://wb.nszjky.cn

[A16] 真假值判断规则
来源：http://mg.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ec.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qw.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eb.lnxyls.cn

TS:   if (!x) {}
来源：http://xr.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tc.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ie.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yg.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jc.gzmigu.cn

[A17] 位运算
来源：http://no.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://km.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gt.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jd.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bg.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uq.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://oq.colortex.cn

Py:   ord("A"); chr(65)
来源：http://qp.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://br.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qj.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sr.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://qy.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rp.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://jr.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://or.shxzukj.cn

[A19] 交换两个变量
来源：http://xy.shxzskj.cn

Py:   a, b = b, a
来源：http://yw.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ri.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ns.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ty.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://fz.hahajie.cn

Go:   a, b = b, a
来源：http://bv.gzmigu.cn

Ruby: a, b = b, a
来源：http://cv.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://zz.hahajie.cn

[A20] 读取标准输入
来源：http://mb.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://qq.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ko.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ug.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://fu.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://fs.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://le.szxytkj.cn

Ruby: gets.chomp
来源：http://gp.asd995.cn

C#:   Console.ReadLine();
来源：http://uf.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://wj.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://pb.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mu.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://nt.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://fq.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://ai.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xl.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://dc.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ah.shxzskj.cn

[A22] 获取字符串长度
来源：http://ij.huixiangedu.cn

Py:   len(s)
来源：http://ba.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ac.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dt.shtwfgs.cn

TS:   s.length
来源：http://jh.nicolike.cn

Java: s.length()
来源：http://nd.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zu.wgjwhj.cn

Ruby: s.length
来源：http://bo.gzmigu.cn

C#:   s.Length
来源：http://pf.hahajie.cn

[A23] 大小写转换
来源：http://ju.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://od.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hj.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gz.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cp.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ge.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ap.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bd.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kd.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://gh.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ma.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ll.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lk.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bh.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://tp.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ae.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pb.asd995.cn

[A25] 字符串比较
来源：http://oi.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://rv.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mg.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pn.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ie.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ec.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ao.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fu.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yq.haigaiapp.cn

[A26] 类型转换总览
来源：http://je.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ba.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qw.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zd.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://mv.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tr.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ag.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yx.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bj.haigaiapp.cn

================================================================================
来源：http://yy.gzmigu.cn

B. 流程控制
来源：http://or.gzmigu.cn

================================================================================
来源：http://vk.nicolike.cn

[B01] 条件判断 if / else
来源：http://lh.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pb.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ji.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ki.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qn.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ku.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://md.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iu.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ij.nicolike.cn

[B02] 多分支 else if / elif
来源：http://ab.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wx.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uy.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ju.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zh.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sx.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gw.shtwfgs.cn

[B03] switch / match / case
来源：http://rq.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ta.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vc.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vm.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qs.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kl.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://di.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bt.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://co.shtwfgs.cn

[B04] for 计数循环
来源：http://lc.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://nb.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ai.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://px.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lb.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://os.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://fe.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pl.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://qf.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://bn.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ka.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ih.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sl.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mw.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ws.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://cs.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sy.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://uf.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nh.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gr.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cl.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qf.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zl.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ok.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://du.chemitech.net.cn

[B07] while 循环
来源：http://jh.nicolike.cn

Py:   while i < 10: i += 1
来源：http://ia.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://or.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://qe.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://ax.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://jv.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qs.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://uf.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ku.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://qi.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ib.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oz.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://sc.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://gn.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://yq.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dr.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hf.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://gl.huixiangedu.cn

[B09] break 与 continue
来源：http://ey.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zm.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uu.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zd.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yn.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nl.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bz.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xn.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://vj.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uk.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://la.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yf.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ru.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ed.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ef.521024.cn


<!-- 参考信息 -->