代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://wq.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rt.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://js.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pe.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nx.521024.cn

[A07] 数字转字符串
来源：http://ul.huixinmuqiang.cn

Py:   str(42)
来源：http://ky.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://gu.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://jh.yuntaijiaju.cn

TS:   String(42)
来源：http://fo.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cg.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://xn.gzmigu.cn

Ruby: 42.to_s
来源：http://qb.colortex.cn

C#:   42.ToString()
来源：http://we.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://fc.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oz.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ze.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tj.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lb.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qq.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yw.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wc.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tx.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://ry.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mn.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tl.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jc.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sg.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://if.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rx.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pt.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dx.szsharing.cn

[A10] 生成随机数
来源：http://or.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://et.521024.cn

PHP:  random_int(1, 100);
来源：http://vc.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://si.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oj.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://hj.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ge.gzmigu.cn

Ruby: rand(1..100)
来源：http://ge.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://yw.nszjky.cn

[A11] 条件表达式（三元）
来源：http://qw.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://jo.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ah.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wy.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kv.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ar.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mk.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ds.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jn.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://sm.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ii.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ch.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://wl.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://bo.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://tu.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bu.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://bd.colortex.cn

C#:   $"Hello, {name}!"
来源：http://yi.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://un.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://jh.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://mi.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://ci.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://ef.shxzskj.cn

Java: "第一行\n第二行"
来源：http://mf.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://lc.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://jo.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://oe.huixinmuqiang.cn

[A14] 注释写法
来源：http://jk.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oi.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uw.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://qd.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://lk.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://az.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://dl.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://td.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://fd.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://dh.9csxet.cn

Py:   value = data or "默认值"
来源：http://ky.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://nz.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://az.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://xk.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://js.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://ov.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://lt.521024.cn

C#:   var value = data ?? "默认值";
来源：http://eu.wgjwhj.cn

[A16] 真假值判断规则
来源：http://pn.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kb.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cd.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yf.chemitech.net.cn

TS:   if (!x) {}
来源：http://bc.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wg.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lv.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hx.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nk.hnjuh.cn

[A17] 位运算
来源：http://bv.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iq.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cj.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bg.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dy.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uv.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gz.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://we.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://ka.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://gx.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://vu.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xd.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ct.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://yy.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ey.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://ra.colortex.cn

C#:   (int)'A'; (char)65
来源：http://xm.hahajie.cn

[A19] 交换两个变量
来源：http://uz.asd995.cn

Py:   a, b = b, a
来源：http://rm.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pa.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://lq.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://en.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://pe.huixiangedu.cn

Go:   a, b = b, a
来源：http://cp.nszjky.cn

Ruby: a, b = b, a
来源：http://dj.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ij.colortex.cn

[A20] 读取标准输入
来源：http://vd.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://jj.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oc.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kd.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://ab.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://cj.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ne.9csxet.cn

Ruby: gets.chomp
来源：http://fq.shxzukj.cn

C#:   Console.ReadLine();
来源：http://nj.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://yx.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://bo.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ds.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://vv.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://ti.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://fc.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://by.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://jg.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://yf.521024.cn

[A22] 获取字符串长度
来源：http://cl.jctech888.com.cn

Py:   len(s)
来源：http://hw.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zk.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rh.muxihuayi.cn

TS:   s.length
来源：http://ov.hahajie.cn

Java: s.length()
来源：http://pn.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rn.szsharing.cn

Ruby: s.length
来源：http://gu.yuexingan06.cn

C#:   s.Length
来源：http://dd.chemitech.net.cn

[A23] 大小写转换
来源：http://km.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iu.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vx.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oj.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fn.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gm.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kk.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rn.lnxyls.cn

[A24] 去除首尾空白
来源：http://pj.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://co.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cd.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mg.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oi.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zg.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://wp.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kz.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wm.yuexingan06.cn

[A25] 字符串比较
来源：http://wh.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://to.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jg.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zq.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://av.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eh.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xs.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wz.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qz.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://yv.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hh.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fk.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ay.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://ki.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lu.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://je.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://se.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yw.hahajie.cn

================================================================================
来源：http://th.szxytkj.cn

B. 流程控制
来源：http://cb.hahajie.cn

================================================================================
来源：http://ue.9csxet.cn

[B01] 条件判断 if / else
来源：http://ta.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cz.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pg.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://er.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rj.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ae.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wu.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ac.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://em.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://vf.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jh.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tq.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vw.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ib.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ed.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.chemitech.net.cn

[B03] switch / match / case
来源：http://pb.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://if.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uz.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fq.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ua.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eb.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mg.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pi.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lj.asd995.cn

[B04] for 计数循环
来源：http://ve.521024.cn

Py:   for i in range(10): print(i)
来源：http://uw.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bv.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wh.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fy.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nz.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ie.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://vy.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://it.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://zz.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://ge.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ds.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ks.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rm.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qa.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cc.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://ys.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vc.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://ul.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yh.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xv.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ua.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oz.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://if.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hr.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://di.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wr.nszjky.cn

[B07] while 循环
来源：http://ss.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://qk.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vf.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://ha.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://ef.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://lw.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fm.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://gk.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ha.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://lc.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://mt.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cu.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://rj.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://xp.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://sb.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rp.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zk.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://uj.asd995.cn

[B09] break 与 continue
来源：http://es.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ln.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xn.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fo.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://va.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ph.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://oi.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ht.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pz.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cj.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ey.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sq.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vp.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sd.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://to.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ch.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://qo.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://nl.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ib.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ou.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://io.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ra.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ix.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ha.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://cf.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mv.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://is.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rq.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lt.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wv.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cx.9csxet.cn

[B13] 判断是否为数字
来源：http://ei.521024.cn

Py:   isinstance(x, (int, float))
来源：http://ql.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://bx.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gn.chemitech.net.cn


<!-- 参考信息 -->