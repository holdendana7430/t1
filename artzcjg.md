代发 wailian999

JS:   const PI = 3.14159;
来源：http://mm.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://hp.521024.cn

Java: static final double PI = 3.14159;
来源：http://ld.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://zi.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://qx.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://cp.wgjwhj.cn

[A04] 判断变量类型
来源：http://vk.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uo.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ws.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://la.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://am.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://to.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hv.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ar.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://nn.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://bs.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hw.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hb.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hm.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://it.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://rp.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://pm.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://tj.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://st.panjiajie.cn

[A06] 字符串转数字
来源：http://lh.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://ps.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ql.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gn.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cu.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kb.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ig.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eb.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jr.huanxung.cn

[A07] 数字转字符串
来源：http://hh.lnxyls.cn

Py:   str(42)
来源：http://kx.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://fg.colortex.cn

JS:   String(42); (42).toString()
来源：http://cb.gzmigu.cn

TS:   String(42)
来源：http://wn.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ev.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://pi.colortex.cn

Ruby: 42.to_s
来源：http://pw.wgjwhj.cn

C#:   42.ToString()
来源：http://ce.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://ga.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tl.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ow.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uz.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ph.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wy.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nt.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fw.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xh.521024.cn

[A09] 绝对值与最大最小值
来源：http://gs.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cu.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zb.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mi.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rv.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bc.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://te.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bb.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rk.hahajie.cn

[A10] 生成随机数
来源：http://qh.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://ys.newstarts.cn

PHP:  random_int(1, 100);
来源：http://du.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cm.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://ko.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ot.muxihuayi.cn

Ruby: rand(1..100)
来源：http://wq.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://ei.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://lh.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://cx.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qn.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://go.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://or.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://wc.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oc.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wx.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kc.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://bc.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vd.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zk.colortex.cn

JS:   `Hello, ${name}!`
来源：http://sf.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://sd.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://wt.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tk.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://oo.521024.cn

C#:   $"Hello, {name}!"
来源：http://kn.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sa.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://xg.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://wt.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://jc.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://fy.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://qu.newstarts.cn

Go:   "第一行\n第二行"
来源：http://gb.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://cp.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://nu.bookmarksfly.cn

[A14] 注释写法
来源：http://xj.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pt.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ci.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://fd.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ci.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lx.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://ij.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uv.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://aw.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://uv.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ef.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://be.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://rl.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://nx.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uj.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://sf.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://jw.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://ro.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://iz.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ck.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uf.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://at.asd995.cn

TS:   if (!x) {}
来源：http://zl.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lw.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wz.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lr.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sr.bjjhwx.cn

[A17] 位运算
来源：http://xj.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ay.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vs.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hx.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cu.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://po.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mu.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sp.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://tl.colortex.cn

Py:   ord("A"); chr(65)
来源：http://vl.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://an.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lg.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ts.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://lh.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://id.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://fq.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://bt.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://sj.huixiangedu.cn

Py:   a, b = b, a
来源：http://gh.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fe.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://qb.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://un.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://wz.hahajie.cn

Go:   a, b = b, a
来源：http://dq.muxihuayi.cn

Ruby: a, b = b, a
来源：http://yt.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://gl.shxzukj.cn

[A20] 读取标准输入
来源：http://lj.hnjuh.cn

Py:   name = input("请输入：")
来源：http://yk.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://di.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://du.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://hm.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://ys.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dg.huixiangedu.cn

Ruby: gets.chomp
来源：http://qz.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://cj.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://hz.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://lf.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kc.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://fj.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://ym.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://vh.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ph.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://dj.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://iq.shxzukj.cn

[A22] 获取字符串长度
来源：http://wg.asd995.cn

Py:   len(s)
来源：http://nk.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ok.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vz.szxytkj.cn

TS:   s.length
来源：http://fq.nszjky.cn

Java: s.length()
来源：http://hn.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hs.szsharing.cn

Ruby: s.length
来源：http://zj.newstarts.cn

C#:   s.Length
来源：http://wp.shxzukj.cn

[A23] 大小写转换
来源：http://fs.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ho.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qh.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ak.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sv.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ev.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mg.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ch.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nj.asd995.cn

[A24] 去除首尾空白
来源：http://gm.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rm.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ks.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bf.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jx.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://we.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hc.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ze.newstarts.cn

[A25] 字符串比较
来源：http://kb.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://jc.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fm.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://up.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://va.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pi.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oz.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bt.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jf.521024.cn

[A26] 类型转换总览
来源：http://ef.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uk.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iq.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://av.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://sk.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vg.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gh.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fr.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ol.bookmarksfly.cn

================================================================================
来源：http://zm.yuntaijiaju.cn

B. 流程控制
来源：http://jl.521024.cn

================================================================================
来源：http://yn.szsharing.cn

[B01] 条件判断 if / else
来源：http://ga.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aa.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pw.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xk.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xx.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pc.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://np.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jp.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ph.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://sf.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zk.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ce.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nq.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vx.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.yuexingan06.cn

[B03] switch / match / case
来源：http://yv.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://el.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ul.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fj.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vl.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ro.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bd.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ip.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cj.szsharing.cn

[B04] for 计数循环
来源：http://qu.colortex.cn

Py:   for i in range(10): print(i)
来源：http://mh.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bh.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oi.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ke.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ap.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://hp.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vg.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://xs.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://wl.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hn.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ub.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pu.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jo.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rx.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://sg.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ow.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://hx.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uv.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sk.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kq.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ch.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mm.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ow.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yq.muxihuayi.cn

[B07] while 循环
来源：http://bf.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://wk.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vd.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://rr.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://gr.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://nb.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dk.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://cc.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://cl.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://fj.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://qe.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yb.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://vu.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://eb.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://un.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ud.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eu.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://uh.9csxet.cn

[B09] break 与 continue
来源：http://jz.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xy.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rp.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://us.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wy.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wn.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zm.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ae.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xf.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yl.gzmigu.cn


<!-- 参考信息 -->