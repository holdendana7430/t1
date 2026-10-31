代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gf.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://co.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://od.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fk.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ek.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kd.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ys.hahajie.cn

[A05] 整数除法与取模
来源：http://fu.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cy.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ct.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kd.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fg.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://ox.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://fv.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dv.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://lf.shxzskj.cn

[A06] 字符串转数字
来源：http://mr.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://zb.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xp.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jb.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cg.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://on.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cy.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yb.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rc.hahajie.cn

[A07] 数字转字符串
来源：http://ty.521024.cn

Py:   str(42)
来源：http://md.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://fd.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://ni.chemitech.net.cn

TS:   String(42)
来源：http://ax.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bs.521024.cn

Go:   strconv.Itoa(42)
来源：http://ff.yuexingan06.cn

Ruby: 42.to_s
来源：http://jf.gzmigu.cn

C#:   42.ToString()
来源：http://se.szsharing.cn

[A08] 取整与四舍五入
来源：http://da.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://au.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dv.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cj.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://py.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wk.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qc.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eb.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vs.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://mp.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ta.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nz.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xl.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ej.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lr.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://de.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yr.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nu.szsharing.cn

[A10] 生成随机数
来源：http://pf.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://hg.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://zp.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rj.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rd.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://az.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xx.huanxung.cn

Ruby: rand(1..100)
来源：http://fd.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://ul.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://ts.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://bf.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rc.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ez.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gx.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://rq.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sw.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tj.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hv.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://wf.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rz.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lk.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://om.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://uh.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://fz.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ok.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://qv.asd995.cn

C#:   $"Hello, {name}!"
来源：http://xi.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vt.newstarts.cn

Py:   "第一行\n第二行"
来源：http://jr.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://ab.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://os.nszjky.cn

TS:   "第一行\n第二行"
来源：http://ul.521024.cn

Java: "第一行\n第二行"
来源：http://sf.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://jv.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://ku.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://jj.yuexingan06.cn

[A14] 注释写法
来源：http://tg.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sm.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gd.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ek.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://hm.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rh.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://ca.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rb.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://mx.szxytkj.cn

[A15] 空值判断与默认值
来源：http://hu.szsharing.cn

Py:   value = data or "默认值"
来源：http://lm.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://mh.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://wj.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://xc.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ry.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://bf.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://rc.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://mj.wgjwhj.cn

[A16] 真假值判断规则
来源：http://dx.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xe.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nq.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://go.wgjwhj.cn

TS:   if (!x) {}
来源：http://lq.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ko.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rr.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ly.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nt.chemitech.net.cn

[A17] 位运算
来源：http://dj.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ez.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sm.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rn.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ks.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ex.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ly.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kc.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://gz.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://hc.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://bp.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dg.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mb.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://mc.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tm.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://wl.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://va.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://ye.wgjwhj.cn

Py:   a, b = b, a
来源：http://zo.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dd.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://qn.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://wi.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://xi.wgjwhj.cn

Go:   a, b = b, a
来源：http://lg.panjiajie.cn

Ruby: a, b = b, a
来源：http://wm.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://gy.lnxyls.cn

[A20] 读取标准输入
来源：http://un.lnxyls.cn

Py:   name = input("请输入：")
来源：http://yh.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://et.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kn.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://ys.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://gm.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xw.shxzukj.cn

Ruby: gets.chomp
来源：http://oo.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://pz.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://tp.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://xx.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mx.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://ky.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://yn.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://wc.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sw.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://ld.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://kp.newstarts.cn

[A22] 获取字符串长度
来源：http://jn.9csxet.cn

Py:   len(s)
来源：http://gn.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://am.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ul.shxzskj.cn

TS:   s.length
来源：http://vn.bjjhwx.cn

Java: s.length()
来源：http://wo.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tt.jctech888.com.cn

Ruby: s.length
来源：http://yh.huanxung.cn

C#:   s.Length
来源：http://nu.hnjuh.cn

[A23] 大小写转换
来源：http://aj.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gu.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eo.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bt.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sj.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eg.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vc.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cd.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://da.bjjhwx.cn

[A24] 去除首尾空白
来源：http://bh.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qa.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jc.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eq.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://of.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zl.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://bi.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cy.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://we.panjiajie.cn

[A25] 字符串比较
来源：http://ee.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://rl.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cc.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yb.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wl.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aq.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gp.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qm.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lg.bjjhwx.cn

[A26] 类型转换总览
来源：http://ai.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xt.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ez.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nu.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://lv.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ew.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bj.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ae.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hx.bjjhwx.cn

================================================================================
来源：http://fr.haigaiapp.cn

B. 流程控制
来源：http://ws.colortex.cn

================================================================================
来源：http://gy.szsharing.cn

[B01] 条件判断 if / else
来源：http://lc.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://te.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ws.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hq.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ak.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fc.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gh.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ze.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ij.nicolike.cn

[B02] 多分支 else if / elif
来源：http://ox.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ne.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://co.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fq.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ya.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dp.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.hnjuh.cn

[B03] switch / match / case
来源：http://wi.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sw.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qt.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oi.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mk.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kk.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pk.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ru.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vn.newstarts.cn

[B04] for 计数循环
来源：http://ni.colortex.cn

Py:   for i in range(10): print(i)
来源：http://tn.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ai.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pq.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pk.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pj.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cy.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://la.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dh.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://tx.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://jq.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wf.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zs.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vl.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zo.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qa.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://en.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wd.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ew.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ny.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sx.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://le.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qi.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oj.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yz.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://al.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eb.9csxet.cn

[B07] while 循环
来源：http://wv.9csxet.cn

Py:   while i < 10: i += 1
来源：http://my.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ht.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://yq.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://bh.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://qq.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://au.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://it.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://qt.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://gx.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://zf.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ej.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://dg.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://nw.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://qv.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ug.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mv.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://wz.panjiajie.cn

[B09] break 与 continue
来源：http://ip.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zw.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kz.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sq.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ze.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cn.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aw.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jd.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://js.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yw.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lu.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://be.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zb.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pc.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yq.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xo.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xx.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://ri.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://qq.wgjwhj.cn


<!-- 参考信息 -->