代发 wailian999

Ruby: PI = 3.14159
来源：http://zx.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://yt.panjiajie.cn

[A04] 判断变量类型
来源：http://zr.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qo.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nq.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ec.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://bc.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yq.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://na.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hy.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://wr.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://nn.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fh.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ae.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sy.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rz.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://zg.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://vn.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://bd.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://kv.hahajie.cn

[A06] 字符串转数字
来源：http://ft.521024.cn

Py:   int("42"); float("3.14")
来源：http://dy.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gw.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jl.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kq.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://md.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tl.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kp.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fl.shtwfgs.cn

[A07] 数字转字符串
来源：http://ju.szxytkj.cn

Py:   str(42)
来源：http://er.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://bq.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://hb.haigaiapp.cn

TS:   String(42)
来源：http://jn.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vg.asd995.cn

Go:   strconv.Itoa(42)
来源：http://vu.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://vy.lnxyls.cn

C#:   42.ToString()
来源：http://sv.shxzskj.cn

[A08] 取整与四舍五入
来源：http://lo.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ck.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uy.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dp.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wc.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iv.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wb.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jn.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rw.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://nb.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ls.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://og.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vv.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wi.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gn.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gv.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ar.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fy.colortex.cn

[A10] 生成随机数
来源：http://sw.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://ej.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://gi.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xy.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qy.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://hz.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sw.jctech888.com.cn

Ruby: rand(1..100)
来源：http://eb.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://qo.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://rz.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://me.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ik.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ep.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ey.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://hf.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ks.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gf.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qq.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://mb.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gm.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ol.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://em.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://nm.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://rj.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://el.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://gn.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://rp.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jr.huanxung.cn

Py:   "第一行\n第二行"
来源：http://fl.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://pk.521024.cn

JS:   "第一行\n第二行"
来源：http://tm.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://rv.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://uc.nicolike.cn

Go:   "第一行\n第二行"
来源：http://wm.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://rd.asd995.cn

C#:   "第一行\n第二行"
来源：http://id.panjiajie.cn

[A14] 注释写法
来源：http://pq.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uf.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ng.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://bi.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://wr.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pi.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ol.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kd.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://ht.9csxet.cn

[A15] 空值判断与默认值
来源：http://yb.hnjuh.cn

Py:   value = data or "默认值"
来源：http://sj.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://qz.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://wq.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://kt.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qy.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://dg.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://dv.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://mf.521024.cn

[A16] 真假值判断规则
来源：http://up.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ll.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jm.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://il.bjjhwx.cn

TS:   if (!x) {}
来源：http://fs.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ea.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wj.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bz.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cb.shtwfgs.cn

[A17] 位运算
来源：http://uq.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hl.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://de.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ps.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nv.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oi.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ss.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://iv.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://zv.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://ye.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wd.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://il.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://pd.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fg.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://so.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://hi.shxzskj.cn

[A19] 交换两个变量
来源：http://wl.szxytkj.cn

Py:   a, b = b, a
来源：http://yk.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xp.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://iv.asd995.cn

TS:   [a, b] = [b, a];
来源：http://gq.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://bs.huanxung.cn

Go:   a, b = b, a
来源：http://ce.haigaiapp.cn

Ruby: a, b = b, a
来源：http://pu.asd995.cn

C#:   (a, b) = (b, a);
来源：http://qt.hnjuh.cn

[A20] 读取标准输入
来源：http://ck.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://jk.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ml.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kv.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://cn.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://hv.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mo.9csxet.cn

Ruby: gets.chomp
来源：http://yq.szsharing.cn

C#:   Console.ReadLine();
来源：http://vy.nszjky.cn

[A21] 保留指定小数位输出
来源：http://kt.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://ns.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://us.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://zh.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ut.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://py.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ra.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://su.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://wt.521024.cn

[A22] 获取字符串长度
来源：http://am.huixinmuqiang.cn

Py:   len(s)
来源：http://ao.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cs.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://po.bjjhwx.cn

TS:   s.length
来源：http://oa.szsharing.cn

Java: s.length()
来源：http://ar.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lk.shxzukj.cn

Ruby: s.length
来源：http://zc.jctech888.com.cn

C#:   s.Length
来源：http://bx.muxihuayi.cn

[A23] 大小写转换
来源：http://vl.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://na.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tp.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yz.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bx.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cn.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hs.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lq.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zu.newstarts.cn

[A24] 去除首尾空白
来源：http://bn.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dx.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tb.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yu.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://np.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qd.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://el.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kt.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mm.bjjhwx.cn

[A25] 字符串比较
来源：http://hi.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://ws.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lk.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nk.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kf.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ce.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gh.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://no.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ur.huanxung.cn

[A26] 类型转换总览
来源：http://qv.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fi.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dv.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lo.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://nv.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wr.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ic.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nb.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ol.bookmarksfly.cn

================================================================================
来源：http://zc.yuntaijiaju.cn

B. 流程控制
来源：http://sa.gzmigu.cn

================================================================================
来源：http://ku.nszjky.cn

[B01] 条件判断 if / else
来源：http://mp.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nn.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uw.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wm.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://je.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ur.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qu.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gm.nszjky.cn

[B02] 多分支 else if / elif
来源：http://pf.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pj.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gr.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ur.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oz.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ls.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nu.muxihuayi.cn

[B03] switch / match / case
来源：http://lg.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yr.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xf.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ko.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kd.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sw.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ia.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yg.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://db.lnxyls.cn

[B04] for 计数循环
来源：http://hz.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://tc.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jt.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fs.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eh.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://il.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zt.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://jf.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nr.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://zz.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://px.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ft.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kw.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tw.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jp.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yu.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://mp.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iv.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://qp.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tv.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uu.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://va.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sz.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bp.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xp.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nm.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pf.bookmarksfly.cn

[B07] while 循环
来源：http://mz.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://jd.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://of.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://vn.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://mb.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qg.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://tz.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://co.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://xy.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://ur.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qz.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ub.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://vk.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://lp.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jq.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jj.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ke.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rj.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pt.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lw.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ad.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mr.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://vu.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xe.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ne.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yf.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qa.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fl.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vj.bjjhwx.cn


<!-- 参考信息 -->