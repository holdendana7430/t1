代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://pf.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ft.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://vy.shxzskj.cn

[A05] 整数除法与取模
来源：http://zk.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nt.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zy.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://na.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mn.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://jm.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://vp.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://rf.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://bq.shtwfgs.cn

[A06] 字符串转数字
来源：http://mz.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://ez.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yu.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ht.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nc.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vr.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dt.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mn.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zu.colortex.cn

[A07] 数字转字符串
来源：http://ib.bjjhwx.cn

Py:   str(42)
来源：http://jq.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://uo.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://rk.shtwfgs.cn

TS:   String(42)
来源：http://yr.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fb.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://lw.yuexingan06.cn

Ruby: 42.to_s
来源：http://ns.wgjwhj.cn

C#:   42.ToString()
来源：http://aj.panjiajie.cn

[A08] 取整与四舍五入
来源：http://ce.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gj.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rd.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cs.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zf.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://go.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wo.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hq.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zy.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://kj.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pz.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cu.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uc.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qk.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ik.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dj.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://es.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tz.yuexingan06.cn

[A10] 生成随机数
来源：http://ym.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://fe.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://lm.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kz.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wm.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://wo.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ql.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://et.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://kk.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://cb.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://we.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jj.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kw.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kr.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://zx.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://il.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uu.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bc.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://fg.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ct.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ql.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://em.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://ui.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://he.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gp.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://mv.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://hi.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://af.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://tm.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://rf.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://su.huanxung.cn

TS:   "第一行\n第二行"
来源：http://qe.lnxyls.cn

Java: "第一行\n第二行"
来源：http://ix.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://pf.521024.cn

Ruby: "第一行\n第二行"
来源：http://ps.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://dv.chemitech.net.cn

[A14] 注释写法
来源：http://tj.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ul.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pv.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://dx.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://fn.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fz.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://rn.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eb.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://dz.shxzukj.cn

[A15] 空值判断与默认值
来源：http://er.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://me.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://hv.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://el.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://xa.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ub.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://mh.nszjky.cn

Ruby: value = data || "默认值"
来源：http://xo.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://vx.wgjwhj.cn

[A16] 真假值判断规则
来源：http://um.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zd.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fx.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ad.panjiajie.cn

TS:   if (!x) {}
来源：http://dw.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uq.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hx.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zg.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xd.haigaiapp.cn

[A17] 位运算
来源：http://km.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ab.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ua.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zf.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tf.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rc.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://xk.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://bq.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://dg.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jr.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://it.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ua.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zt.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://rx.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://nj.jctech888.com.cn

[A19] 交换两个变量
来源：http://tf.nszjky.cn

Py:   a, b = b, a
来源：http://mm.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pw.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://jg.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://wl.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://wt.szsharing.cn

Go:   a, b = b, a
来源：http://bm.nicolike.cn

Ruby: a, b = b, a
来源：http://df.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://mr.521024.cn

[A20] 读取标准输入
来源：http://cx.szsharing.cn

Py:   name = input("请输入：")
来源：http://ta.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ea.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nr.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://rw.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://jl.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gr.hnjuh.cn

Ruby: gets.chomp
来源：http://au.shxzskj.cn

C#:   Console.ReadLine();
来源：http://nt.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ef.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://hc.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xb.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://tq.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://ti.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://kz.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://os.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ek.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://nf.yuexingan06.cn

[A22] 获取字符串长度
来源：http://rt.gzmigu.cn

Py:   len(s)
来源：http://ij.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tu.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://we.newstarts.cn

TS:   s.length
来源：http://hu.chemitech.net.cn

Java: s.length()
来源：http://eg.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fh.panjiajie.cn

Ruby: s.length
来源：http://fd.huixiangedu.cn

C#:   s.Length
来源：http://td.szsharing.cn

[A23] 大小写转换
来源：http://cd.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zl.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kn.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dw.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vd.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bg.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sy.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vi.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jq.wgjwhj.cn

[A24] 去除首尾空白
来源：http://dy.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://le.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zg.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mm.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lf.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kw.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://fe.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ag.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kh.nszjky.cn

[A25] 字符串比较
来源：http://hu.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://zw.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uc.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://br.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://by.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bw.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oz.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pd.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mi.shtwfgs.cn

[A26] 类型转换总览
来源：http://tn.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zh.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ba.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vq.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://cm.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gg.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qj.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vt.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ad.9csxet.cn

================================================================================
来源：http://ve.lnxyls.cn

B. 流程控制
来源：http://wh.szxytkj.cn

================================================================================
来源：http://qt.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://yu.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ir.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zf.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pg.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tb.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hg.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tl.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jj.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rq.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://dn.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cr.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pn.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vb.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://av.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jy.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.asd995.cn

[B03] switch / match / case
来源：http://fv.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tc.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hh.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sp.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gg.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qt.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://am.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://co.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kx.huanxung.cn

[B04] for 计数循环
来源：http://sv.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://jj.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uq.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fr.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qt.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uh.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://al.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://lk.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ec.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://cy.huanxung.cn

Py:   for item in arr: print(item)
来源：http://sp.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sh.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jm.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yx.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bm.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rm.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ix.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ml.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ap.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cr.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xp.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nr.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ir.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fy.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zs.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qd.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yv.bookmarksfly.cn

[B07] while 循环
来源：http://qp.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://me.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tl.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://qo.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://uv.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://cn.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bj.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://sl.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://is.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ty.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://vw.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nq.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://pk.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://jl.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://er.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fm.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bv.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://vr.newstarts.cn

[B09] break 与 continue
来源：http://su.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fk.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://in.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qg.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yr.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tp.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://wt.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ox.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ch.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hi.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sl.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qe.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yl.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mh.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://vj.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://lw.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://ah.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fa.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ws.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pi.szsharing.cn


<!-- 参考信息 -->