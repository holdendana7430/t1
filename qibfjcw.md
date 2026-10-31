代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xx.nszjky.cn

[A07] 数字转字符串
来源：http://wq.yuexingan06.cn

Py:   str(42)
来源：http://rq.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://qs.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://ak.shxzukj.cn

TS:   String(42)
来源：http://uh.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ea.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://yu.wgjwhj.cn

Ruby: 42.to_s
来源：http://sh.hnjuh.cn

C#:   42.ToString()
来源：http://wr.asd995.cn

[A08] 取整与四舍五入
来源：http://gr.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gn.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tk.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gd.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://av.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ac.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pm.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rl.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ku.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://ss.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zo.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://he.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uk.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tj.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rb.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rs.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cl.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kb.yuntaijiaju.cn

[A10] 生成随机数
来源：http://hx.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ir.colortex.cn

PHP:  random_int(1, 100);
来源：http://bp.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tw.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vj.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ab.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jh.muxihuayi.cn

Ruby: rand(1..100)
来源：http://zt.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://kq.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://nf.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://eu.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mn.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kt.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ei.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ow.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wb.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fp.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sz.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://ux.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ba.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kv.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://iw.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://il.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://xu.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nm.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://lu.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://on.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sh.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://rw.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://it.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://dw.newstarts.cn

TS:   "第一行\n第二行"
来源：http://dc.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://di.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://ub.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://ky.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://ep.hnjuh.cn

[A14] 注释写法
来源：http://nn.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eu.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oi.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://hd.521024.cn

TS:   // 单行；/* 多行 */
来源：http://ne.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ai.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://dj.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sa.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://aa.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://go.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://zx.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://rt.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://dk.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://yn.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gm.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://uf.szsharing.cn

Ruby: value = data || "默认值"
来源：http://qm.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://ac.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://rl.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yy.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vw.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sa.9csxet.cn

TS:   if (!x) {}
来源：http://gk.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gj.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yb.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kh.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bn.szsharing.cn

[A17] 位运算
来源：http://ch.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zo.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ey.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tt.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gb.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hh.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ui.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ze.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://zn.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://hh.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://zi.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xy.521024.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bo.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://at.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gp.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://as.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://cm.panjiajie.cn

[A19] 交换两个变量
来源：http://lc.huanxung.cn

Py:   a, b = b, a
来源：http://vr.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hc.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://uj.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://bf.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://oq.jctech888.com.cn

Go:   a, b = b, a
来源：http://zx.chemitech.net.cn

Ruby: a, b = b, a
来源：http://zk.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://kf.shxzskj.cn

[A20] 读取标准输入
来源：http://xj.hnjuh.cn

Py:   name = input("请输入：")
来源：http://ca.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ey.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ju.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://mj.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://sj.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wb.haigaiapp.cn

Ruby: gets.chomp
来源：http://rs.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://yn.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://al.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://jc.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wl.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://oo.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://si.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://bh.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://du.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://pl.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://at.newstarts.cn

[A22] 获取字符串长度
来源：http://nd.shxzukj.cn

Py:   len(s)
来源：http://lf.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rf.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://le.huanxung.cn

TS:   s.length
来源：http://cu.yuntaijiaju.cn

Java: s.length()
来源：http://lq.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gj.muxihuayi.cn

Ruby: s.length
来源：http://jd.szsharing.cn

C#:   s.Length
来源：http://hd.wgjwhj.cn

[A23] 大小写转换
来源：http://ib.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jq.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kw.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vn.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hx.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nx.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://go.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qg.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vg.nszjky.cn

[A24] 去除首尾空白
来源：http://yc.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gx.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vh.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jw.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gm.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xm.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://di.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ge.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uy.huixiangedu.cn

[A25] 字符串比较
来源：http://ce.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://yn.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qy.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dz.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vr.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lg.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vw.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fh.huanxung.cn

[A26] 类型转换总览
来源：http://qe.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tg.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qd.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kx.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ro.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jz.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://od.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qj.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zy.hnjuh.cn

================================================================================
来源：http://zq.shxzskj.cn

B. 流程控制
来源：http://ub.yuexingan06.cn

================================================================================
来源：http://ym.nicolike.cn

[B01] 条件判断 if / else
来源：http://dz.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vn.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bg.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ul.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tn.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mr.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kl.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ek.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vd.521024.cn

[B02] 多分支 else if / elif
来源：http://vi.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gn.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aj.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://va.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ah.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.asd995.cn

[B03] switch / match / case
来源：http://vw.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bq.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zo.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dz.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tk.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hb.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fb.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hc.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xn.hnjuh.cn

[B04] for 计数循环
来源：http://yr.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://yf.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qw.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xj.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pi.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kn.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sv.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://vc.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ed.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://fb.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://xp.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jw.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vr.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nv.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bv.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nt.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://tc.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://py.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://vh.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mr.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://is.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fd.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lt.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aj.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fw.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gb.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tn.bjjhwx.cn

[B07] while 循环
来源：http://wu.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://ia.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mo.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://im.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://bn.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://oo.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://up.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://lt.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://da.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ak.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://wo.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ll.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://tl.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://on.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://nf.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bs.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hx.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://rx.jianghongdianzi.cn

[B09] break 与 continue
来源：http://we.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ql.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://he.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kb.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mi.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jd.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vu.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wg.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://zz.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yo.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jl.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://es.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jk.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tk.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ap.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ia.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hg.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pd.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://oc.521024.cn

PHP:  range(0, 10, 2);
来源：http://ka.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://he.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ti.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uq.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jg.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://kq.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vt.yuexingan06.cn

[B12] 跳出多层循环
来源：http://aq.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wt.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wo.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://us.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sg.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zy.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wc.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://td.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ug.bjjhwx.cn

[B13] 判断是否为数字
来源：http://li.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://mm.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://wi.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qa.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.wgjwhj.cn

Java: x instanceof Number
来源：http://vh.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://to.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://fy.newstarts.cn


<!-- 参考信息 -->