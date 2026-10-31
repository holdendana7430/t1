代发 wailian999

JS:   String(42); (42).toString()
来源：http://gp.nicolike.cn

TS:   String(42)
来源：http://ne.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ns.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://nk.hahajie.cn

Ruby: 42.to_s
来源：http://eh.muxihuayi.cn

C#:   42.ToString()
来源：http://jj.panjiajie.cn

[A08] 取整与四舍五入
来源：http://ew.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pm.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://md.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gq.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gv.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uj.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ux.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://he.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zv.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://cu.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nw.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ez.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ku.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ks.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hr.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nu.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qh.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sl.wgjwhj.cn

[A10] 生成随机数
来源：http://qy.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://dl.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://xi.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://co.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://us.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://ge.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://do.szxytkj.cn

Ruby: rand(1..100)
来源：http://gx.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://nl.nicolike.cn

[A11] 条件表达式（三元）
来源：http://fx.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ur.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://od.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ss.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vg.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://kq.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ix.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ck.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dx.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://wy.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uw.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://em.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://rh.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://wy.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://xm.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jz.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://ny.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://rw.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://td.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://zd.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://am.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://to.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://jx.lnxyls.cn

Java: "第一行\n第二行"
来源：http://ly.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://yf.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://vv.colortex.cn

C#:   "第一行\n第二行"
来源：http://kx.chemitech.net.cn

[A14] 注释写法
来源：http://bo.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kz.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ja.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://us.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://nv.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://am.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://cb.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ck.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://um.szxytkj.cn

[A15] 空值判断与默认值
来源：http://si.colortex.cn

Py:   value = data or "默认值"
来源：http://xb.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://go.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://lj.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://tr.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pp.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://ze.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://sr.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://jq.chemitech.net.cn

[A16] 真假值判断规则
来源：http://yu.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gq.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dy.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://no.gzmigu.cn

TS:   if (!x) {}
来源：http://nr.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qi.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zy.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ey.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ey.9csxet.cn

[A17] 位运算
来源：http://ug.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pf.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tx.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wo.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jj.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sr.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://ol.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://dx.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://rm.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ex.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cf.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://iu.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sa.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://bi.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://tl.9csxet.cn

[A19] 交换两个变量
来源：http://mc.gzmigu.cn

Py:   a, b = b, a
来源：http://id.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ml.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://wh.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://bw.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://wg.panjiajie.cn

Go:   a, b = b, a
来源：http://cw.colortex.cn

Ruby: a, b = b, a
来源：http://pl.521024.cn

C#:   (a, b) = (b, a);
来源：http://yl.bookmarksfly.cn

[A20] 读取标准输入
来源：http://ng.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://ka.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ef.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cf.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://qh.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://sq.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ag.panjiajie.cn

Ruby: gets.chomp
来源：http://jw.521024.cn

C#:   Console.ReadLine();
来源：http://zl.asd995.cn

[A21] 保留指定小数位输出
来源：http://bm.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://gi.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://je.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://jp.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://go.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://ja.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oy.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://oz.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://cz.shtwfgs.cn

[A22] 获取字符串长度
来源：http://en.haigaiapp.cn

Py:   len(s)
来源：http://hl.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kk.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wk.shxzskj.cn

TS:   s.length
来源：http://af.yuntaijiaju.cn

Java: s.length()
来源：http://rp.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pf.chemitech.net.cn

Ruby: s.length
来源：http://fj.9csxet.cn

C#:   s.Length
来源：http://ov.haigaiapp.cn

[A23] 大小写转换
来源：http://vg.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gu.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tw.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ug.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ix.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ch.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ge.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gy.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sb.szsharing.cn

[A24] 去除首尾空白
来源：http://in.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://du.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yv.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qf.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uj.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ip.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://df.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jm.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pj.huixiangedu.cn

[A25] 字符串比较
来源：http://tp.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://xl.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sx.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rl.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kl.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://na.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oh.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ue.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wz.521024.cn

[A26] 类型转换总览
来源：http://gt.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nr.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fi.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lh.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://cx.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ns.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lg.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zz.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xr.colortex.cn

================================================================================
来源：http://xa.panjiajie.cn

B. 流程控制
来源：http://gd.bjjhwx.cn

================================================================================
来源：http://yo.colortex.cn

[B01] 条件判断 if / else
来源：http://gw.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oo.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jy.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://my.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tc.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yk.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qf.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ax.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cr.colortex.cn

[B02] 多分支 else if / elif
来源：http://cb.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wu.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vp.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ts.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ux.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pd.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vl.lnxyls.cn

[B03] switch / match / case
来源：http://mg.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uw.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://on.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bl.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ju.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bl.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eg.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fi.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ue.hnjuh.cn

[B04] for 计数循环
来源：http://bj.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://rm.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ug.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://in.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tv.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ko.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xx.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://oi.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://be.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://pd.asd995.cn

Py:   for item in arr: print(item)
来源：http://wh.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://al.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rt.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lj.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eo.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jt.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://nv.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ck.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://xq.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zf.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ik.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gt.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://te.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sm.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ft.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hn.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://au.jianghongdianzi.cn

[B07] while 循环
来源：http://ki.asd995.cn

Py:   while i < 10: i += 1
来源：http://pj.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jd.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://ov.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://hp.colortex.cn

Java: while (i < 10) { i++; }
来源：http://ei.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xz.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ud.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://tl.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://rj.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://uj.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ld.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://aj.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://uf.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://zc.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xq.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vy.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://qa.bjjhwx.cn

[B09] break 与 continue
来源：http://fb.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://st.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ho.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bk.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zz.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://gh.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fl.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tt.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bd.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gi.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gg.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mf.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ry.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ph.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://mo.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://wc.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://sg.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://og.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xd.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ev.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://by.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://do.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jr.9csxet.cn

[B12] 跳出多层循环
来源：http://ja.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pu.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ak.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cp.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ho.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zh.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hp.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nw.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oy.chemitech.net.cn

[B13] 判断是否为数字
来源：http://vb.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://qs.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://kk.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ft.521024.cn

Java: x instanceof Number
来源：http://ak.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ye.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ja.521024.cn

C#:   x is int or double or decimal
来源：http://ow.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://or.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ur.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bg.szxytkj.cn


<!-- 参考信息 -->