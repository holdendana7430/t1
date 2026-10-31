代发 wailian999

JS:   String(42); (42).toString()
来源：http://ak.shxzukj.cn

TS:   String(42)
来源：http://iv.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ck.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://sr.newstarts.cn

Ruby: 42.to_s
来源：http://hq.nicolike.cn

C#:   42.ToString()
来源：http://fe.nicolike.cn

[A08] 取整与四舍五入
来源：http://nu.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gq.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cr.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yk.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://us.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kr.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tf.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vn.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ip.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://ss.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uk.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qn.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bn.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://to.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gc.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nn.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tw.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mn.colortex.cn

[A10] 生成随机数
来源：http://ud.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://wh.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://mj.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yv.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uu.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://de.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bz.9csxet.cn

Ruby: rand(1..100)
来源：http://ef.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://fs.asd995.cn

[A11] 条件表达式（三元）
来源：http://wt.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ei.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sr.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jm.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nc.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ni.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rt.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cr.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oy.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://id.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hm.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rf.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://fd.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://ao.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ul.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ex.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://no.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://ui.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fr.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://lk.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://gk.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://se.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://bf.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://jz.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://qm.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://xt.asd995.cn

C#:   "第一行\n第二行"
来源：http://wh.nicolike.cn

[A14] 注释写法
来源：http://si.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zf.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yu.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://qd.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://zs.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://is.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://yn.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ut.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://yt.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://zs.nszjky.cn

Py:   value = data or "默认值"
来源：http://tc.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://nj.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://wn.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://dd.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ny.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://rq.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ua.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://ob.nicolike.cn

[A16] 真假值判断规则
来源：http://dr.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kn.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ip.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sg.wgjwhj.cn

TS:   if (!x) {}
来源：http://nn.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://so.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xx.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hm.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ib.wgjwhj.cn

[A17] 位运算
来源：http://xl.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://es.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qw.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hx.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fs.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uz.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pp.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://pz.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://vb.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://hh.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gg.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ta.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://qp.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oy.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://jd.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://et.hnjuh.cn

[A19] 交换两个变量
来源：http://kb.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://qs.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ww.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://bt.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://pm.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://hz.jctech888.com.cn

Go:   a, b = b, a
来源：http://ye.nicolike.cn

Ruby: a, b = b, a
来源：http://qn.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://uy.chemitech.net.cn

[A20] 读取标准输入
来源：http://vr.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://ts.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ak.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ez.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://tj.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://mk.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tn.yuexingan06.cn

Ruby: gets.chomp
来源：http://ra.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://uj.nicolike.cn

[A21] 保留指定小数位输出
来源：http://yq.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://wz.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vu.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://tk.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://px.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://um.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cb.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://mh.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://de.nszjky.cn

[A22] 获取字符串长度
来源：http://ly.bjjhwx.cn

Py:   len(s)
来源：http://ip.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rm.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rt.yuexingan06.cn

TS:   s.length
来源：http://hw.jianghongdianzi.cn

Java: s.length()
来源：http://zd.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bf.hahajie.cn

Ruby: s.length
来源：http://dv.hahajie.cn

C#:   s.Length
来源：http://xj.521024.cn

[A23] 大小写转换
来源：http://oy.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zz.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zk.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rs.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xz.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pe.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tv.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hy.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ao.colortex.cn

[A24] 去除首尾空白
来源：http://ct.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://if.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yn.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yi.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://an.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iy.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://zk.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ds.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hi.huanxung.cn

[A25] 字符串比较
来源：http://gz.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://tu.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jg.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lr.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ua.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tz.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sd.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qy.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sg.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://no.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ui.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ma.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gi.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://zn.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dc.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pp.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dy.521024.cn

================================================================================
来源：http://nl.shxzskj.cn

B. 流程控制
来源：http://tq.yuexingan06.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://pc.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://um.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ye.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cg.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://up.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mw.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xh.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fs.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mt.nicolike.cn

[B02] 多分支 else if / elif
来源：http://pm.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ng.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eg.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mz.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mz.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ml.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xx.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hh.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.newstarts.cn

[B03] switch / match / case
来源：http://bu.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ph.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lw.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qo.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lp.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vg.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qk.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ji.shxzukj.cn

[B04] for 计数循环
来源：http://bw.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://to.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jd.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://we.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gl.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uu.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ew.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://rn.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yg.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://jh.asd995.cn

Py:   for item in arr: print(item)
来源：http://eb.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rn.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fj.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lb.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iu.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tc.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://xx.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qh.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://ts.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lr.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gw.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sn.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ns.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ix.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://is.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wp.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://le.newstarts.cn

[B07] while 循环
来源：http://tj.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://bc.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qa.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://wc.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://xz.521024.cn

Java: while (i < 10) { i++; }
来源：http://qa.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gr.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://px.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://qc.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://qa.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://st.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xu.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://un.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ql.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://jz.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ts.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lf.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://ok.jctech888.com.cn

[B09] break 与 continue
来源：http://xi.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tp.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://on.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tt.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dk.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mh.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://bc.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vw.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://me.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gu.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rh.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tn.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ky.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lw.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://sc.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://fw.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://xr.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jt.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ar.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wi.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://cx.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hg.jctech888.com.cn

[B12] 跳出多层循环
来源：http://uv.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://df.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yu.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yo.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vk.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ya.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qp.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oy.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ko.hnjuh.cn

[B13] 判断是否为数字
来源：http://et.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://cl.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://rp.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mo.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.shxzukj.cn

Java: x instanceof Number
来源：http://vh.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ri.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://te.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://fn.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ux.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iz.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dy.nszjky.cn


<!-- 参考信息 -->