代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wa.bjjhwx.cn

[A07] 数字转字符串
来源：http://tt.szxytkj.cn

Py:   str(42)
来源：http://wy.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://ff.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://rt.shtwfgs.cn

TS:   String(42)
来源：http://nq.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kz.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://em.muxihuayi.cn

Ruby: 42.to_s
来源：http://se.shxzukj.cn

C#:   42.ToString()
来源：http://mc.shxzskj.cn

[A08] 取整与四舍五入
来源：http://zb.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ag.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ya.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ca.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fw.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vb.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ue.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ul.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gs.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://zm.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ae.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yq.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zi.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ej.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pp.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cc.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://px.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yf.lnxyls.cn

[A10] 生成随机数
来源：http://cc.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://fx.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://ef.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dr.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ky.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://kp.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fv.muxihuayi.cn

Ruby: rand(1..100)
来源：http://uk.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://tj.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://cg.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://oa.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fg.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hj.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lj.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://wb.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://re.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sm.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xx.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://ns.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://at.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rv.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://yp.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://yl.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://sv.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://my.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://zk.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://sa.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ww.szsharing.cn

Py:   "第一行\n第二行"
来源：http://co.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://qr.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://ug.hahajie.cn

TS:   "第一行\n第二行"
来源：http://iw.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://vy.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://zi.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://wb.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://qu.nszjky.cn

[A14] 注释写法
来源：http://ln.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kk.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tt.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://sl.521024.cn

TS:   // 单行；/* 多行 */
来源：http://vz.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mx.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://hv.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hj.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://vq.lnxyls.cn

[A15] 空值判断与默认值
来源：http://op.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://le.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://ly.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://le.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://by.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://in.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://gm.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://zw.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://vb.nicolike.cn

[A16] 真假值判断规则
来源：http://yt.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ul.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fr.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qv.huixiangedu.cn

TS:   if (!x) {}
来源：http://wu.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://no.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zd.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ym.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lw.jctech888.com.cn

[A17] 位运算
来源：http://zg.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tw.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iz.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gq.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cy.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ls.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jm.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ve.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://qd.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://hx.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://mz.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aq.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ll.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://rn.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zy.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://tn.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://pu.shtwfgs.cn

[A19] 交换两个变量
来源：http://zy.nszjky.cn

Py:   a, b = b, a
来源：http://xp.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ij.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://mf.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://sh.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ap.hahajie.cn

Go:   a, b = b, a
来源：http://cd.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://mh.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://hl.bjjhwx.cn

[A20] 读取标准输入
来源：http://uy.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://yt.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gg.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://at.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://nr.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://fn.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nf.hnjuh.cn

Ruby: gets.chomp
来源：http://it.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://po.newstarts.cn

[A21] 保留指定小数位输出
来源：http://ns.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://yf.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qg.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://wn.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://mt.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ag.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vl.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://ya.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://os.szsharing.cn

[A22] 获取字符串长度
来源：http://qn.huanxung.cn

Py:   len(s)
来源：http://no.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xs.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qb.huixiangedu.cn

TS:   s.length
来源：http://nj.chemitech.net.cn

Java: s.length()
来源：http://gt.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yq.shtwfgs.cn

Ruby: s.length
来源：http://on.szsharing.cn

C#:   s.Length
来源：http://zn.huanxung.cn

[A23] 大小写转换
来源：http://fv.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ku.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oh.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ta.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fc.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fd.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gj.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vl.chemitech.net.cn

[A24] 去除首尾空白
来源：http://zb.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gn.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dl.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ow.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rh.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jr.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://vy.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bf.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nw.wgjwhj.cn

[A25] 字符串比较
来源：http://in.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ok.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tt.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ru.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://og.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uo.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://in.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nn.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dm.wgjwhj.cn

[A26] 类型转换总览
来源：http://qr.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://if.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eu.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bf.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://bs.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://at.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rf.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dh.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://mp.szsharing.cn

B. 流程控制
来源：http://ji.bjjhwx.cn

================================================================================
来源：http://ob.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://lw.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lc.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ub.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bm.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gt.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ve.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xr.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mm.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gy.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://qv.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mx.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ee.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bu.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bf.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mu.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ar.shxzukj.cn

[B03] switch / match / case
来源：http://co.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qx.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ph.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dn.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bx.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bn.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lw.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ts.muxihuayi.cn

[B04] for 计数循环
来源：http://jx.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://jp.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bt.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vs.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://os.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bq.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://gy.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wz.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://bn.521024.cn

Py:   for item in arr: print(item)
来源：http://ew.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qe.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qf.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gp.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fa.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xj.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://um.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yd.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://wn.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://js.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vc.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rk.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mn.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uo.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yq.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wl.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eh.huanxung.cn

[B07] while 循环
来源：http://of.newstarts.cn

Py:   while i < 10: i += 1
来源：http://ct.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fe.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://dc.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://qo.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://yu.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sr.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://oz.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://eu.521024.cn

[B08] do-while（至少执行一次）
来源：http://sr.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ob.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zf.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://hn.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://gs.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://re.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://al.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zx.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://oa.huixinmuqiang.cn

[B09] break 与 continue
来源：http://jm.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wz.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://my.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fo.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bt.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://on.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://rm.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kw.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dg.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kq.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kx.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aw.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://li.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ap.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ut.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://xq.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://au.521024.cn

PHP:  range(0, 10, 2);
来源：http://vr.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jj.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mc.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sm.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://zq.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ac.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://wg.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://as.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://co.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rw.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://md.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bs.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dd.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ac.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ds.muxihuayi.cn

[B13] 判断是否为数字
来源：http://yu.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://bs.asd995.cn

PHP:  is_numeric($x)
来源：http://yq.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qr.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qe.9csxet.cn

Java: x instanceof Number
来源：http://kf.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ir.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://bo.huanxung.cn


<!-- 参考信息 -->