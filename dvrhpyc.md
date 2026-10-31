代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dh.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vj.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ly.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bv.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bf.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lo.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sa.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://nx.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bs.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ob.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ji.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qh.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pd.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zg.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tn.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bz.nszjky.cn

[A10] 生成随机数
来源：http://qu.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://lp.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://jj.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://db.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dv.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://yf.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mx.chemitech.net.cn

Ruby: rand(1..100)
来源：http://we.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://bp.huanxung.cn

[A11] 条件表达式（三元）
来源：http://wd.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://px.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kn.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vf.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hv.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://gm.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eb.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jm.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ko.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://pj.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rx.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uu.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://iu.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://gg.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://he.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wu.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://fd.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://al.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://za.asd995.cn

Py:   "第一行\n第二行"
来源：http://lt.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://nz.521024.cn

JS:   "第一行\n第二行"
来源：http://pp.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://xp.shxzukj.cn

Java: "第一行\n第二行"
来源：http://wj.9csxet.cn

Go:   "第一行\n第二行"
来源：http://po.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://la.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://ln.newstarts.cn

[A14] 注释写法
来源：http://gp.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://em.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gm.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://li.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://fw.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gy.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://kn.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cg.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://tw.hnjuh.cn

[A15] 空值判断与默认值
来源：http://qd.9csxet.cn

Py:   value = data or "默认值"
来源：http://be.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ma.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://ex.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://eh.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://er.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ti.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://ak.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://dv.muxihuayi.cn

[A16] 真假值判断规则
来源：http://ku.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kj.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kj.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hj.huixiangedu.cn

TS:   if (!x) {}
来源：http://yd.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vq.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://in.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://en.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.wgjwhj.cn

[A17] 位运算
来源：http://sa.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iv.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ky.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nw.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rb.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sr.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://cx.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://tk.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://ps.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uq.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yh.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://yb.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wa.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://sb.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://rw.hnjuh.cn

[A19] 交换两个变量
来源：http://le.521024.cn

Py:   a, b = b, a
来源：http://we.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yh.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://yr.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://vt.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://zj.huixiangedu.cn

Go:   a, b = b, a
来源：http://ss.wgjwhj.cn

Ruby: a, b = b, a
来源：http://fi.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://va.chemitech.net.cn

[A20] 读取标准输入
来源：http://av.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://im.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ol.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tt.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://yz.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ei.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ir.panjiajie.cn

Ruby: gets.chomp
来源：http://cl.9csxet.cn

C#:   Console.ReadLine();
来源：http://rz.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://rq.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://qs.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wd.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://gn.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://tj.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://xk.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rg.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://my.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://ku.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://fo.haigaiapp.cn

Py:   len(s)
来源：http://nh.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uu.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mp.haigaiapp.cn

TS:   s.length
来源：http://yt.521024.cn

Java: s.length()
来源：http://vx.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xo.yuntaijiaju.cn

Ruby: s.length
来源：http://qu.jianghongdianzi.cn

C#:   s.Length
来源：http://vx.shxzukj.cn

[A23] 大小写转换
来源：http://fk.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hj.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gm.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sr.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mp.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kd.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dm.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tn.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qh.asd995.cn

[A24] 去除首尾空白
来源：http://bc.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oj.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lh.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iq.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ok.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hi.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://tg.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://to.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kc.hahajie.cn

[A25] 字符串比较
来源：http://cp.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://cu.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dq.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oz.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ei.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cg.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://um.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sf.lnxyls.cn

[A26] 类型转换总览
来源：http://cl.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iy.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ew.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tj.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://bw.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uf.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bq.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://im.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wh.yuntaijiaju.cn

================================================================================
来源：http://qs.bookmarksfly.cn

B. 流程控制
来源：http://et.haigaiapp.cn

================================================================================
来源：http://xw.hnjuh.cn

[B01] 条件判断 if / else
来源：http://hv.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oa.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ss.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sa.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vv.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tk.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ks.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://bm.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wa.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dc.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oy.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eg.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tw.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wr.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://su.haigaiapp.cn

[B03] switch / match / case
来源：http://ag.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xq.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aj.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vs.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vg.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nk.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hd.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bc.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mk.bjjhwx.cn

[B04] for 计数循环
来源：http://bp.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://io.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zi.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ts.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mz.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nj.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fn.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://ec.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yc.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://vv.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://dm.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fr.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tq.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sd.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jc.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dv.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://ov.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nf.colortex.cn

[B06] 遍历字典 / 对象
来源：http://lr.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nu.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vc.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://de.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gq.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ba.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dk.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ws.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://re.huixinmuqiang.cn

[B07] while 循环
来源：http://mu.hahajie.cn

Py:   while i < 10: i += 1
来源：http://yk.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nw.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://iq.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ms.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://jr.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qt.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ro.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://ym.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://mz.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://cc.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iv.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://eh.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://qp.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://kd.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vy.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tq.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://ol.chemitech.net.cn

[B09] break 与 continue
来源：http://tn.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cy.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mf.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yv.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dl.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lo.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://qs.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://be.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ab.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bd.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mz.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://di.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mb.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dp.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://im.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://vy.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://dy.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://tv.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zl.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jx.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wo.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rs.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://gf.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://is.jctech888.com.cn

[B12] 跳出多层循环
来源：http://tt.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ry.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ek.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sq.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ln.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ez.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uk.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qr.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://va.szsharing.cn

[B13] 判断是否为数字
来源：http://up.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://zv.gzmigu.cn

PHP:  is_numeric($x)
来源：http://mr.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zl.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://di.haigaiapp.cn

Java: x instanceof Number
来源：http://gn.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fk.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://sg.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://xv.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://dg.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nl.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://au.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://vh.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://rm.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gq.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mq.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xy.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pm.shxzukj.cn

[B15] 布尔运算与取反
来源：http://il.shxzukj.cn

Py:   a and b or not c
来源：http://vt.shxzskj.cn


<!-- 参考信息 -->