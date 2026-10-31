代发 wailian999

JS:   String(42); (42).toString()
来源：http://fw.szxytkj.cn

TS:   String(42)
来源：http://go.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tb.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://cj.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://yj.yuexingan06.cn

C#:   42.ToString()
来源：http://au.shxzskj.cn

[A08] 取整与四舍五入
来源：http://yx.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fv.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eo.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://na.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jd.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ck.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eq.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xw.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cv.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://qn.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ic.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ls.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ky.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qr.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oj.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uv.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ty.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ch.szxytkj.cn

[A10] 生成随机数
来源：http://vi.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ih.szsharing.cn

PHP:  random_int(1, 100);
来源：http://rk.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zm.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lt.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://ky.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://um.gzmigu.cn

Ruby: rand(1..100)
来源：http://oh.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://on.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://xb.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://lr.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uu.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nq.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nx.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://ak.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lv.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kr.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kv.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://ho.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ch.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ej.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://na.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://zj.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ao.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://re.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://ls.asd995.cn

C#:   $"Hello, {name}!"
来源：http://vv.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.521024.cn

Py:   "第一行\n第二行"
来源：http://kp.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://dj.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://ag.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://jn.hahajie.cn

Java: "第一行\n第二行"
来源：http://to.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://hz.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://oa.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ns.gzmigu.cn

[A14] 注释写法
来源：http://yo.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vm.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fq.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://iz.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://zw.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nx.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://fh.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sl.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://kd.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://fb.panjiajie.cn

Py:   value = data or "默认值"
来源：http://hu.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://zi.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://gu.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://xd.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ab.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://bz.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://nc.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ih.chemitech.net.cn

[A16] 真假值判断规则
来源：http://it.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nz.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bf.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ih.chemitech.net.cn

TS:   if (!x) {}
来源：http://sq.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cp.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ik.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://or.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fw.bjjhwx.cn

[A17] 位运算
来源：http://ul.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tt.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lr.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aa.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cr.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wf.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ua.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://sw.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://mz.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://mj.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yh.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ga.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://mp.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fn.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://wg.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://ll.muxihuayi.cn

[A19] 交换两个变量
来源：http://fv.newstarts.cn

Py:   a, b = b, a
来源：http://iv.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vi.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://wz.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ec.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://do.huixiangedu.cn

Go:   a, b = b, a
来源：http://uk.colortex.cn

Ruby: a, b = b, a
来源：http://wd.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://dx.shxzukj.cn

[A20] 读取标准输入
来源：http://jk.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://hw.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://om.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://un.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://ud.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://wc.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fw.panjiajie.cn

Ruby: gets.chomp
来源：http://au.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://vn.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://ep.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://hu.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://is.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://so.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://iz.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://cv.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qh.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://pd.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://wz.asd995.cn

[A22] 获取字符串长度
来源：http://si.nszjky.cn

Py:   len(s)
来源：http://ou.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ow.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://py.jianghongdianzi.cn

TS:   s.length
来源：http://mp.9csxet.cn

Java: s.length()
来源：http://sj.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ea.hahajie.cn

Ruby: s.length
来源：http://ro.yuntaijiaju.cn

C#:   s.Length
来源：http://db.newstarts.cn

[A23] 大小写转换
来源：http://ez.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mh.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fu.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://py.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://st.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vr.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hs.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cg.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ym.hahajie.cn

[A24] 去除首尾空白
来源：http://pn.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hm.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nx.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://io.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cx.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xo.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://bb.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gp.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lr.yuntaijiaju.cn

[A25] 字符串比较
来源：http://zf.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://xb.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://si.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qp.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cu.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rq.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ma.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xi.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rl.lnxyls.cn

[A26] 类型转换总览
来源：http://nd.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://up.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xy.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dc.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://ud.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://de.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ok.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vj.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://as.jianghongdianzi.cn

================================================================================
来源：http://zf.szsharing.cn

B. 流程控制
来源：http://cl.szxytkj.cn

================================================================================
来源：http://lg.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://lx.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yb.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://td.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ji.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dm.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wh.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dk.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vf.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ir.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bc.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ue.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lf.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tx.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xh.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jo.bookmarksfly.cn

[B03] switch / match / case
来源：http://pk.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ah.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iz.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hb.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sw.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zt.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jo.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nq.huanxung.cn

[B04] for 计数循环
来源：http://rs.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://qh.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ji.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eu.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xz.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cw.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://by.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://bi.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rp.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://wt.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://ko.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://on.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xj.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eh.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ju.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gs.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://gi.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ec.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://fc.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dg.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ls.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tn.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hi.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qj.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kq.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ru.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hv.huixinmuqiang.cn

[B07] while 循环
来源：http://jx.newstarts.cn

Py:   while i < 10: i += 1
来源：http://gs.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fg.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ox.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://co.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://dr.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://je.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ws.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://af.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://iz.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://pe.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mx.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://lk.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://dv.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://nv.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ga.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ce.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://gp.jianghongdianzi.cn

[B09] break 与 continue
来源：http://za.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ze.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uv.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xb.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bd.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xq.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://dy.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wh.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ly.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ok.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tv.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dg.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gi.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cx.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rq.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://ni.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://rl.asd995.cn

PHP:  range(0, 10, 2);
来源：http://fb.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eg.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gn.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pd.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xx.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://tk.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yy.shxzukj.cn

[B12] 跳出多层循环
来源：http://ln.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wa.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kq.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bj.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bw.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jq.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://re.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wj.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uj.hahajie.cn

[B13] 判断是否为数字
来源：http://cy.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://qi.szxytkj.cn

PHP:  is_numeric($x)
来源：http://qi.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ot.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bt.wgjwhj.cn

Java: x instanceof Number
来源：http://qr.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vq.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://wu.huanxung.cn

C#:   x is int or double or decimal
来源：http://yx.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://li.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lo.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tc.bjjhwx.cn


<!-- 参考信息 -->