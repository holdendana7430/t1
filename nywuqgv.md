代发 wailian999

Ruby: PI = 3.14159
来源：http://iu.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://ro.hnjuh.cn

[A04] 判断变量类型
来源：http://jo.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ld.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jo.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fk.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://xr.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zi.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ec.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hk.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://ci.newstarts.cn

[A05] 整数除法与取模
来源：http://ad.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lp.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zw.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://co.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pg.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://oj.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://wx.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://uu.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://hl.hnjuh.cn

[A06] 字符串转数字
来源：http://xg.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://ja.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lh.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zp.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wp.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tn.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://na.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cl.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oa.yuexingan06.cn

[A07] 数字转字符串
来源：http://kh.nszjky.cn

Py:   str(42)
来源：http://eh.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://uh.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://oa.jctech888.com.cn

TS:   String(42)
来源：http://rd.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pu.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://jg.shxzukj.cn

Ruby: 42.to_s
来源：http://xb.szxytkj.cn

C#:   42.ToString()
来源：http://jn.shxzskj.cn

[A08] 取整与四舍五入
来源：http://iy.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kl.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fo.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dn.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ct.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dn.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sk.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tk.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rt.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://jj.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://id.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qi.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tj.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ug.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sl.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ix.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ic.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vz.hahajie.cn

[A10] 生成随机数
来源：http://qm.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://aw.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://hy.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bj.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://av.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://qu.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vf.huanxung.cn

Ruby: rand(1..100)
来源：http://or.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://mc.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://kp.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://cm.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ri.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://du.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bh.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://vp.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oq.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gn.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hy.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://dd.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wo.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sf.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://ek.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://vt.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://vf.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://di.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://sm.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://vr.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kv.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://gd.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://xv.nicolike.cn

JS:   "第一行\n第二行"
来源：http://qs.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://se.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ty.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://to.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://li.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://pc.yuexingan06.cn

[A14] 注释写法
来源：http://tq.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ya.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fg.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://oa.521024.cn

TS:   // 单行；/* 多行 */
来源：http://qz.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mh.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://uj.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jf.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://an.lnxyls.cn

[A15] 空值判断与默认值
来源：http://kp.hahajie.cn

Py:   value = data or "默认值"
来源：http://fr.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://ad.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://jm.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://bx.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vn.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ix.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://br.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://fb.shtwfgs.cn

[A16] 真假值判断规则
来源：http://xt.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ts.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pq.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oi.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://wg.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://go.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qj.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uz.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fb.shxzukj.cn

[A17] 位运算
来源：http://sw.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://de.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ub.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pc.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oi.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pa.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jt.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://cj.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://pn.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://gu.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nv.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://px.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://so.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pq.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://ms.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://zp.9csxet.cn

[A19] 交换两个变量
来源：http://ck.hahajie.cn

Py:   a, b = b, a
来源：http://iq.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pv.colortex.cn

JS:   [a, b] = [b, a];
来源：http://ct.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://fs.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://ys.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://mv.shxzukj.cn

Ruby: a, b = b, a
来源：http://ld.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://mr.9csxet.cn

[A20] 读取标准输入
来源：http://mi.hahajie.cn

Py:   name = input("请输入：")
来源：http://ik.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eq.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mi.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ku.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://mq.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ol.szxytkj.cn

Ruby: gets.chomp
来源：http://cw.newstarts.cn

C#:   Console.ReadLine();
来源：http://zh.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://om.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://ss.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fj.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://tl.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://gc.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://ib.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://po.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://eu.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://vv.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://vd.haigaiapp.cn

Py:   len(s)
来源：http://ib.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://so.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eo.yuntaijiaju.cn

TS:   s.length
来源：http://kz.hnjuh.cn

Java: s.length()
来源：http://fc.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vn.huanxung.cn

Ruby: s.length
来源：http://yz.colortex.cn

C#:   s.Length
来源：http://pa.panjiajie.cn

[A23] 大小写转换
来源：http://gx.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mo.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ot.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://et.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iz.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fc.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jg.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fl.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://ua.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uk.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cp.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ip.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://si.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xy.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://gy.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cx.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yy.huixinmuqiang.cn

[A25] 字符串比较
来源：http://cj.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://wf.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sl.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aq.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cn.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vq.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fi.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://el.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pg.wgjwhj.cn

[A26] 类型转换总览
来源：http://nb.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tb.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bq.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qu.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://dn.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dw.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://st.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bh.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bt.huixiangedu.cn

================================================================================
来源：http://ij.9csxet.cn

B. 流程控制
来源：http://en.bookmarksfly.cn

================================================================================
来源：http://ff.lnxyls.cn

[B01] 条件判断 if / else
来源：http://mf.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xk.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eh.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qs.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sh.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://er.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://or.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hm.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nd.newstarts.cn

[B02] 多分支 else if / elif
来源：http://dl.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cv.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rb.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rf.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://he.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qb.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vg.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.asd995.cn

[B03] switch / match / case
来源：http://xr.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gh.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xj.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dr.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bg.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fe.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dc.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xz.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kr.jianghongdianzi.cn

[B04] for 计数循环
来源：http://sp.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://ab.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zx.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uu.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xy.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ai.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xm.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://bn.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mc.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://of.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://bp.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nj.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kt.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mh.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eu.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://on.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://fr.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ea.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://cx.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tb.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ep.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uj.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jy.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vy.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://in.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sx.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jx.hnjuh.cn

[B07] while 循环
来源：http://xd.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://gs.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gg.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://va.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://st.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://be.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ni.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://fh.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://hm.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ye.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ul.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://df.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://we.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://xi.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://lo.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lw.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hl.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://um.lnxyls.cn

[B09] break 与 continue
来源：http://ga.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sh.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gq.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sd.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fx.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fj.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://eu.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ns.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jd.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ec.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oi.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hn.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gt.haigaiapp.cn


<!-- 参考信息 -->