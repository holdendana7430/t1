代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ru.huixiangedu.cn

[A07] 数字转字符串
来源：http://qi.nicolike.cn

Py:   str(42)
来源：http://zb.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://lg.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://pi.jianghongdianzi.cn

TS:   String(42)
来源：http://ms.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jp.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://md.szsharing.cn

Ruby: 42.to_s
来源：http://ea.shtwfgs.cn

C#:   42.ToString()
来源：http://pa.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://pq.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dy.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zc.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kw.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zr.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wt.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yp.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vv.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zr.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://xz.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kp.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mm.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cx.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vo.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zz.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cg.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ju.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ow.9csxet.cn

[A10] 生成随机数
来源：http://hq.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://do.nszjky.cn

PHP:  random_int(1, 100);
来源：http://bu.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ga.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rj.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://ol.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tv.huanxung.cn

Ruby: rand(1..100)
来源：http://ms.521024.cn

C#:   new Random().Next(1, 101)
来源：http://gf.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://kd.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://sk.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tb.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xn.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sm.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://hn.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wf.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zf.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://za.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://rk.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://db.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yq.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://ma.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://pk.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://cg.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ce.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://de.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://we.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zw.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://og.asd995.cn

PHP:  "第一行\n第二行"
来源：http://md.nszjky.cn

JS:   "第一行\n第二行"
来源：http://lf.asd995.cn

TS:   "第一行\n第二行"
来源：http://ir.szxytkj.cn

Java: "第一行\n第二行"
来源：http://ce.newstarts.cn

Go:   "第一行\n第二行"
来源：http://uq.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://uq.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://yg.521024.cn

[A14] 注释写法
来源：http://ks.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ai.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mi.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://qk.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://if.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ws.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://sy.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bz.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://gk.shxzskj.cn

[A15] 空值判断与默认值
来源：http://vn.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://mg.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://uv.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://zv.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://dv.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xq.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://ki.nicolike.cn

Ruby: value = data || "默认值"
来源：http://ui.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://rz.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://cz.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gp.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pk.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sg.szxytkj.cn

TS:   if (!x) {}
来源：http://tq.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mr.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cu.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ks.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ew.shtwfgs.cn

[A17] 位运算
来源：http://uw.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mt.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nd.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://si.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oy.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kn.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qm.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://qe.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://up.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://xu.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sd.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yq.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://rp.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://js.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://yq.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://dm.bookmarksfly.cn

[A19] 交换两个变量
来源：http://jo.panjiajie.cn

Py:   a, b = b, a
来源：http://ra.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iy.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://yc.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://io.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://hj.nicolike.cn

Go:   a, b = b, a
来源：http://xl.hnjuh.cn

Ruby: a, b = b, a
来源：http://px.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://pq.gzmigu.cn

[A20] 读取标准输入
来源：http://qn.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://jz.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dg.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oj.colortex.cn

TS:   // Node.js：readline 模块
来源：http://nz.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://jx.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oi.colortex.cn

Ruby: gets.chomp
来源：http://df.521024.cn

C#:   Console.ReadLine();
来源：http://wl.asd995.cn

[A21] 保留指定小数位输出
来源：http://iz.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hr.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://nr.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://ka.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://su.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qj.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ck.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ew.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://jy.szxytkj.cn

Py:   len(s)
来源：http://hy.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kb.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ns.hahajie.cn

TS:   s.length
来源：http://fz.jianghongdianzi.cn

Java: s.length()
来源：http://xe.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://so.hnjuh.cn

Ruby: s.length
来源：http://oa.jctech888.com.cn

C#:   s.Length
来源：http://tj.nicolike.cn

[A23] 大小写转换
来源：http://uv.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gm.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ue.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pu.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://se.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ux.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gm.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cu.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ot.lnxyls.cn

[A24] 去除首尾空白
来源：http://pm.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ne.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ed.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hn.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oe.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xd.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://xz.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ox.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qc.yuexingan06.cn

[A25] 字符串比较
来源：http://xq.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://ne.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zn.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kp.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yj.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vb.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zy.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ur.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vj.shxzskj.cn

[A26] 类型转换总览
来源：http://du.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zb.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dr.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zu.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://nn.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dm.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pl.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gb.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qv.chemitech.net.cn

================================================================================
来源：http://tr.hnjuh.cn

B. 流程控制
来源：http://oi.shxzukj.cn

================================================================================
来源：http://my.newstarts.cn

[B01] 条件判断 if / else
来源：http://wb.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vz.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ts.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qk.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sz.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uq.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vg.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://un.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fx.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://zy.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wa.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ex.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nc.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gi.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bb.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sv.bookmarksfly.cn

[B03] switch / match / case
来源：http://bb.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jh.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wt.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wn.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ae.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hr.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zu.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kd.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://um.shxzukj.cn

[B04] for 计数循环
来源：http://jq.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://cq.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mh.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jd.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tq.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tf.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://sd.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sc.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://mq.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://kp.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dd.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yr.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xm.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vr.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vy.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://uf.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pt.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://xm.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dw.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uk.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ze.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kx.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qx.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mc.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qr.newstarts.cn

[B07] while 循环
来源：http://xj.521024.cn

Py:   while i < 10: i += 1
来源：http://sc.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ja.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://sd.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://kq.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ct.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gy.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://xm.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://ha.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://mz.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://mx.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://re.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://xx.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://ia.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://vf.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gf.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ps.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://bg.nszjky.cn

[B09] break 与 continue
来源：http://qc.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ws.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nt.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oa.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kf.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pp.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ja.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sg.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vc.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ck.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pv.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://de.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://un.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ez.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ey.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://fv.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://jx.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://tw.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zb.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bj.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fb.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ep.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://bp.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bk.shtwfgs.cn

[B12] 跳出多层循环
来源：http://fx.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ez.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dw.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ac.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://of.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nc.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eb.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sq.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uz.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://dm.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://of.gzmigu.cn

PHP:  is_numeric($x)
来源：http://cf.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fi.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qe.haigaiapp.cn

Java: x instanceof Number
来源：http://zq.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hw.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://vu.hahajie.cn


<!-- 参考信息 -->