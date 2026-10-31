代发 wailian999

Ruby: 42.to_s
来源：http://ys.bjjhwx.cn

C#:   42.ToString()
来源：http://ag.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://eq.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aw.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ap.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rw.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cs.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oa.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hv.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ye.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://om.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://zb.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cf.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hp.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qg.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jh.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hs.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mb.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iu.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yp.nicolike.cn

[A10] 生成随机数
来源：http://kz.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://le.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://vr.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vg.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wi.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://or.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rq.lnxyls.cn

Ruby: rand(1..100)
来源：http://ko.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://uo.colortex.cn

[A11] 条件表达式（三元）
来源：http://yd.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://lq.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mu.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uf.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dp.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ox.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ec.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://za.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jl.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://hj.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ez.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://al.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://et.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://ak.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://hj.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pc.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://wd.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://lz.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://di.szsharing.cn

Py:   "第一行\n第二行"
来源：http://xa.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://uu.9csxet.cn

JS:   "第一行\n第二行"
来源：http://rb.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://yl.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://nw.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://jy.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://qu.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://wk.jianghongdianzi.cn

[A14] 注释写法
来源：http://zt.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ex.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xz.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ym.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://jt.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xe.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://zu.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://we.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://qx.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://vg.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://js.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://ic.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://yg.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://tb.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gj.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://ew.hahajie.cn

Ruby: value = data || "默认值"
来源：http://yp.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ng.shtwfgs.cn

[A16] 真假值判断规则
来源：http://nc.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jw.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sp.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uk.nszjky.cn

TS:   if (!x) {}
来源：http://ju.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qf.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://we.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qe.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gf.yuexingan06.cn

[A17] 位运算
来源：http://qo.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wy.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pe.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wc.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pm.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://ix.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://ra.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://xu.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pv.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gn.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://mp.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vl.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://nb.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://mf.shxzukj.cn

[A19] 交换两个变量
来源：http://cv.jctech888.com.cn

Py:   a, b = b, a
来源：http://zz.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tn.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://ng.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://mw.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://ua.yuexingan06.cn

Go:   a, b = b, a
来源：http://yp.521024.cn

Ruby: a, b = b, a
来源：http://za.colortex.cn

C#:   (a, b) = (b, a);
来源：http://qy.gzmigu.cn

[A20] 读取标准输入
来源：http://ld.521024.cn

Py:   name = input("请输入：")
来源：http://bj.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pp.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bj.521024.cn

TS:   // Node.js：readline 模块
来源：http://ky.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://zh.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mu.bookmarksfly.cn

Ruby: gets.chomp
来源：http://xz.9csxet.cn

C#:   Console.ReadLine();
来源：http://mn.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://qb.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://wl.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qf.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://di.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://ot.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://ds.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wa.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://dj.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://rn.nicolike.cn

[A22] 获取字符串长度
来源：http://jy.asd995.cn

Py:   len(s)
来源：http://mh.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tp.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kl.szxytkj.cn

TS:   s.length
来源：http://kv.gzmigu.cn

Java: s.length()
来源：http://cg.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xl.lnxyls.cn

Ruby: s.length
来源：http://aq.asd995.cn

C#:   s.Length
来源：http://gc.bjjhwx.cn

[A23] 大小写转换
来源：http://ot.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rp.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jj.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://av.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hg.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yl.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://af.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sj.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lt.huixiangedu.cn

[A24] 去除首尾空白
来源：http://di.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sq.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rk.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wo.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bs.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ga.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://ke.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qb.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bw.yuntaijiaju.cn

[A25] 字符串比较
来源：http://ge.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://ki.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gh.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gb.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tz.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ke.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ot.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zx.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qs.521024.cn

[A26] 类型转换总览
来源：http://yb.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yt.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lv.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://od.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://jn.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mt.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fn.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lr.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ij.bookmarksfly.cn

================================================================================
来源：http://qn.jctech888.com.cn

B. 流程控制
来源：http://gs.nicolike.cn

================================================================================
来源：http://mh.9csxet.cn

[B01] 条件判断 if / else
来源：http://qa.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vb.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kf.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sv.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yd.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ut.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hj.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qg.szsharing.cn

[B02] 多分支 else if / elif
来源：http://lz.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lk.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qg.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ac.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ci.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wi.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ie.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.colortex.cn

[B03] switch / match / case
来源：http://nu.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sy.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fu.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xf.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aa.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ae.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zz.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vi.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ya.jctech888.com.cn

[B04] for 计数循环
来源：http://xw.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://ak.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://in.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cr.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ke.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lf.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ux.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://pr.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://de.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://zm.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://oy.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bc.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ju.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pz.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nu.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lx.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://dt.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yl.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ru.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vg.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kc.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ud.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hx.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://md.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qn.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nf.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://et.yuntaijiaju.cn

[B07] while 循环
来源：http://uw.9csxet.cn

Py:   while i < 10: i += 1
来源：http://fd.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dq.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://hb.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://qt.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ge.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ps.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://nx.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://es.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://lf.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://gu.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gs.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://zm.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://fw.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://bq.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jd.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ir.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://om.colortex.cn

[B09] break 与 continue
来源：http://aw.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ew.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uu.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nd.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zd.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iw.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ui.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dq.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gh.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qt.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://si.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ny.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tn.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vf.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qo.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://zy.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://sz.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://cc.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mo.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://od.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ye.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hx.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://ch.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lv.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://aq.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hk.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pt.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fh.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tp.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://om.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gy.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tu.newstarts.cn

[B13] 判断是否为数字
来源：http://tt.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://iu.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://ur.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://om.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dr.shtwfgs.cn

Java: x instanceof Number
来源：http://mr.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dz.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://jx.nszjky.cn

C#:   x is int or double or decimal
来源：http://qf.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://kt.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oj.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tf.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://vh.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://yh.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nj.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kj.bookmarksfly.cn


<!-- 参考信息 -->