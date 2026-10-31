代发 wailian999

Ruby: PI = 3.14159
来源：http://td.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://io.chemitech.net.cn

[A04] 判断变量类型
来源：http://uc.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bo.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://md.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pp.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://bp.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fu.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wn.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mj.521024.cn

C#:   x.GetType().Name; x is int
来源：http://wr.haigaiapp.cn

[A05] 整数除法与取模
来源：http://zh.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vd.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gt.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lc.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fi.521024.cn

Java: 7 / 2; 7 % 2
来源：http://sa.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://iq.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://be.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://fh.hnjuh.cn

[A06] 字符串转数字
来源：http://cx.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://ao.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yz.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ev.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dn.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://od.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oz.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sh.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nb.shxzskj.cn

[A07] 数字转字符串
来源：http://na.521024.cn

Py:   str(42)
来源：http://rc.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://uu.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://aq.shxzukj.cn

TS:   String(42)
来源：http://ga.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fa.asd995.cn

Go:   strconv.Itoa(42)
来源：http://ls.521024.cn

Ruby: 42.to_s
来源：http://vl.huanxung.cn

C#:   42.ToString()
来源：http://ot.szxytkj.cn

[A08] 取整与四舍五入
来源：http://wn.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fg.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qr.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tq.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dv.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vx.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kr.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vf.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vg.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://pu.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xd.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://av.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dg.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://br.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ax.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ml.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://da.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sl.hnjuh.cn

[A10] 生成随机数
来源：http://hi.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ze.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://tv.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ga.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sb.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://zh.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vw.lnxyls.cn

Ruby: rand(1..100)
来源：http://qz.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://dx.newstarts.cn

[A11] 条件表达式（三元）
来源：http://pn.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://mf.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hi.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sf.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sv.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://sj.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ni.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pc.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sh.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://la.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dj.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://im.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://hd.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://mj.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://nw.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pp.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://qy.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://yf.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uo.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://lg.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://vi.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://bz.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://sd.lnxyls.cn

Java: "第一行\n第二行"
来源：http://nd.huanxung.cn

Go:   "第一行\n第二行"
来源：http://ek.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://yz.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ha.shtwfgs.cn

[A14] 注释写法
来源：http://yh.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fd.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wq.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://ce.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://nr.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ro.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://so.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ix.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://xg.szsharing.cn

[A15] 空值判断与默认值
来源：http://tm.newstarts.cn

Py:   value = data or "默认值"
来源：http://wr.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://kr.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://no.521024.cn

TS:   const value = data ?? "默认值";
来源：http://ip.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eu.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://pk.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://uf.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://lu.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://nm.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uu.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fx.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xx.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://gs.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fn.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://um.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zy.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ij.jctech888.com.cn

[A17] 位运算
来源：http://il.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gb.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zq.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ct.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vq.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cs.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qf.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qj.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lr.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://do.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://pi.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://rl.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yf.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://nb.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ab.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://mr.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://hf.lnxyls.cn

[A19] 交换两个变量
来源：http://pz.huanxung.cn

Py:   a, b = b, a
来源：http://qr.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ro.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://bs.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://xe.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://tr.hnjuh.cn

Go:   a, b = b, a
来源：http://ow.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://jg.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://cd.shxzukj.cn

[A20] 读取标准输入
来源：http://kd.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://ev.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ui.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ag.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://zh.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://rt.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bp.newstarts.cn

Ruby: gets.chomp
来源：http://ui.nicolike.cn

C#:   Console.ReadLine();
来源：http://zx.9csxet.cn

[A21] 保留指定小数位输出
来源：http://cn.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://cu.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dc.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://sq.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://hq.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://df.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xq.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://rc.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://yw.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://kb.huixiangedu.cn

Py:   len(s)
来源：http://bi.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ik.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kz.szxytkj.cn

TS:   s.length
来源：http://aq.newstarts.cn

Java: s.length()
来源：http://dh.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vj.haigaiapp.cn

Ruby: s.length
来源：http://sc.huixinmuqiang.cn

C#:   s.Length
来源：http://nq.shtwfgs.cn

[A23] 大小写转换
来源：http://lz.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fd.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vs.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rh.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pv.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ku.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://os.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yc.gzmigu.cn

[A24] 去除首尾空白
来源：http://bo.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gx.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://id.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://td.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wv.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wg.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://pm.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dx.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yg.shxzukj.cn

[A25] 字符串比较
来源：http://gr.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://oq.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ie.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eo.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eo.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yx.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pd.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pv.shtwfgs.cn

[A26] 类型转换总览
来源：http://ix.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dj.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uz.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rm.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://ag.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://os.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hd.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vj.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ty.newstarts.cn

================================================================================
来源：http://ey.nszjky.cn

B. 流程控制
来源：http://zx.jianghongdianzi.cn

================================================================================
来源：http://ev.gzmigu.cn

[B01] 条件判断 if / else
来源：http://px.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gu.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kn.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rc.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://db.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bs.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pp.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ms.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://jf.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://it.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gi.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mr.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iv.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hv.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gk.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.newstarts.cn

[B03] switch / match / case
来源：http://ug.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ei.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aj.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://el.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hk.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ok.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lm.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vz.9csxet.cn

[B04] for 计数循环
来源：http://we.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://ti.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ry.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rd.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pa.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ut.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://so.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ul.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://zb.colortex.cn

Py:   for item in arr: print(item)
来源：http://ak.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wo.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mn.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ya.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vf.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qy.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ac.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cq.521024.cn

[B06] 遍历字典 / 对象
来源：http://ra.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wr.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ic.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ey.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rn.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://si.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://td.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ju.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://go.521024.cn

[B07] while 循环
来源：http://vw.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://dm.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://do.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://mb.521024.cn

TS:   while (i < 10) { i++; }
来源：http://ma.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://up.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kq.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://pu.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://xp.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://oc.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://lp.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eg.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://rj.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://bw.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://gd.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yt.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qw.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ag.9csxet.cn

[B09] break 与 continue
来源：http://mo.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ls.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ai.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://my.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://un.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hg.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ym.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uq.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://wd.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ox.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ib.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pa.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pw.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mk.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ml.nicolike.cn


<!-- 参考信息 -->