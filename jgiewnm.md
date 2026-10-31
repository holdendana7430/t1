代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gu.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ey.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://up.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fc.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iq.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lb.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://mz.bjjhwx.cn

[A05] 整数除法与取模
来源：http://rs.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mr.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://os.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zc.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qq.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://ia.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://vv.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://tl.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://cx.nicolike.cn

[A06] 字符串转数字
来源：http://xi.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://ab.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rh.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hv.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iv.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ec.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bx.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tx.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yp.chemitech.net.cn

[A07] 数字转字符串
来源：http://nb.szxytkj.cn

Py:   str(42)
来源：http://gv.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://qj.asd995.cn

JS:   String(42); (42).toString()
来源：http://uw.newstarts.cn

TS:   String(42)
来源：http://yl.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ux.asd995.cn

Go:   strconv.Itoa(42)
来源：http://en.nszjky.cn

Ruby: 42.to_s
来源：http://ee.521024.cn

C#:   42.ToString()
来源：http://gq.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://rl.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ul.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ek.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://di.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vh.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ss.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rp.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cz.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://um.asd995.cn

[A09] 绝对值与最大最小值
来源：http://ps.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://os.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hn.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jx.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kp.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gb.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://be.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ke.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fb.huixinmuqiang.cn

[A10] 生成随机数
来源：http://ln.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://ci.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://fi.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vo.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cd.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://qo.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nb.newstarts.cn

Ruby: rand(1..100)
来源：http://xq.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://uq.hahajie.cn

[A11] 条件表达式（三元）
来源：http://hf.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://vy.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://so.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kf.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xr.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://cj.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://st.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gp.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iv.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://ks.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nt.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vq.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://qb.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://tx.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://qi.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pv.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://zz.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://ju.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ub.newstarts.cn

Py:   "第一行\n第二行"
来源：http://rk.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://kp.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://xb.newstarts.cn

TS:   "第一行\n第二行"
来源：http://hk.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://qg.nicolike.cn

Go:   "第一行\n第二行"
来源：http://hb.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://hv.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://ku.shxzskj.cn

[A14] 注释写法
来源：http://jp.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tr.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ul.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://wu.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://sj.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qh.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://ym.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fh.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://vg.colortex.cn

[A15] 空值判断与默认值
来源：http://ou.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://ff.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://kc.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://yn.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ha.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mx.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://zr.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://ps.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://pc.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://kh.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lu.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zx.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://po.9csxet.cn

TS:   if (!x) {}
来源：http://bh.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dt.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vy.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lj.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oi.asd995.cn

[A17] 位运算
来源：http://cl.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ha.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jt.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://of.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://am.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://un.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://qz.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://ju.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ez.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vb.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ic.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eu.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://te.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://qn.wgjwhj.cn

[A19] 交换两个变量
来源：http://pl.yuexingan06.cn

Py:   a, b = b, a
来源：http://ln.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ty.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://jl.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://rk.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://jp.bjjhwx.cn

Go:   a, b = b, a
来源：http://zh.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://ys.asd995.cn

C#:   (a, b) = (b, a);
来源：http://bf.newstarts.cn

[A20] 读取标准输入
来源：http://sv.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://kk.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://py.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ir.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://ds.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://be.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ec.newstarts.cn

Ruby: gets.chomp
来源：http://ss.gzmigu.cn

C#:   Console.ReadLine();
来源：http://sj.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://es.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://fk.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rq.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://nf.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://yc.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://wi.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ff.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ue.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://om.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://qk.wgjwhj.cn

Py:   len(s)
来源：http://mn.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iz.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qe.hahajie.cn

TS:   s.length
来源：http://uf.nszjky.cn

Java: s.length()
来源：http://ba.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bf.colortex.cn

Ruby: s.length
来源：http://yf.panjiajie.cn

C#:   s.Length
来源：http://rl.bjjhwx.cn

[A23] 大小写转换
来源：http://mf.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hf.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ll.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xo.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ts.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wr.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wy.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wp.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vw.jctech888.com.cn

[A24] 去除首尾空白
来源：http://rr.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ai.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ol.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vz.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vd.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ff.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://rq.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ap.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xc.hahajie.cn

[A25] 字符串比较
来源：http://og.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://iu.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cl.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rg.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pq.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://au.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://na.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vu.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wh.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://dn.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lq.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ww.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qr.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://fi.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gr.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ix.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hu.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zu.newstarts.cn

================================================================================
来源：http://wv.hnjuh.cn

B. 流程控制
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://wm.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://zg.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eq.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rp.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kv.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nb.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://av.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pi.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sn.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://dd.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ux.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hq.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://au.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://of.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gk.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.muxihuayi.cn

[B03] switch / match / case
来源：http://vp.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ut.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sh.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ry.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hi.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jw.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iv.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://re.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mc.yuntaijiaju.cn

[B04] for 计数循环
来源：http://fz.asd995.cn

Py:   for i in range(10): print(i)
来源：http://my.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wf.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cf.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ps.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://au.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qv.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://fq.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nj.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ng.nicolike.cn

Py:   for item in arr: print(item)
来源：http://bm.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xv.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ow.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gg.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gs.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iq.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://lk.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dk.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://dc.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xw.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xf.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xj.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rj.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sy.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ts.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gy.shxzskj.cn

[B07] while 循环
来源：http://ef.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ie.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://je.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://az.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://zj.colortex.cn

Java: while (i < 10) { i++; }
来源：http://cf.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://py.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://yn.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://mg.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://hz.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://pj.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jn.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://uk.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://vn.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://no.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bx.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nb.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ld.haigaiapp.cn

[B09] break 与 continue
来源：http://kk.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://af.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rz.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ex.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ml.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xx.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rf.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://by.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://bl.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yg.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ch.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ub.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xw.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fx.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qd.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hg.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ml.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://bt.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://kq.bjjhwx.cn


<!-- 参考信息 -->