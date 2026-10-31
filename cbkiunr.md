代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eo.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://yz.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ie.szsharing.cn

Ruby: rand(1..100)
来源：http://pp.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://do.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://bw.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ob.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rw.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tr.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ii.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://hh.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ue.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://re.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iv.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://az.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dp.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vv.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://mp.521024.cn

TS:   `Hello, ${name}!`
来源：http://vy.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ah.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dk.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://rl.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://bn.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://it.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://vs.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://xv.asd995.cn

JS:   "第一行\n第二行"
来源：http://dj.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://un.shxzskj.cn

Java: "第一行\n第二行"
来源：http://gi.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://jx.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ew.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://yk.gzmigu.cn

[A14] 注释写法
来源：http://rf.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yw.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ly.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://fi.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://st.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sq.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://wb.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dg.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://jr.huanxung.cn

[A15] 空值判断与默认值
来源：http://qy.panjiajie.cn

Py:   value = data or "默认值"
来源：http://gj.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://fq.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://tj.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://le.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://na.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://wd.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://co.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://fc.haigaiapp.cn

[A16] 真假值判断规则
来源：http://hm.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vl.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jf.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qu.lnxyls.cn

TS:   if (!x) {}
来源：http://vu.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qw.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pz.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zn.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ks.hnjuh.cn

[A17] 位运算
来源：http://fv.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rm.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://av.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xw.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pa.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://wd.colortex.cn

Py:   ord("A"); chr(65)
来源：http://ve.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://gg.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fm.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mx.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://it.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qi.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://jz.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://go.hnjuh.cn

[A19] 交换两个变量
来源：http://pt.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://ki.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://no.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://az.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://uz.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://bv.huanxung.cn

Go:   a, b = b, a
来源：http://bi.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://nn.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://ta.nicolike.cn

[A20] 读取标准输入
来源：http://yp.szxytkj.cn

Py:   name = input("请输入：")
来源：http://pg.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bx.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jv.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://vr.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://op.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ka.panjiajie.cn

Ruby: gets.chomp
来源：http://jg.asd995.cn

C#:   Console.ReadLine();
来源：http://md.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://fy.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://sp.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://de.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://eh.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://sw.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://gh.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oj.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://ru.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://bp.szsharing.cn

[A22] 获取字符串长度
来源：http://sk.szsharing.cn

Py:   len(s)
来源：http://lq.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xl.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ae.gzmigu.cn

TS:   s.length
来源：http://do.bookmarksfly.cn

Java: s.length()
来源：http://bb.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tb.huixiangedu.cn

Ruby: s.length
来源：http://lq.chemitech.net.cn

C#:   s.Length
来源：http://ye.wgjwhj.cn

[A23] 大小写转换
来源：http://eo.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jj.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fe.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://az.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jl.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://io.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wu.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://je.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zp.shtwfgs.cn

[A24] 去除首尾空白
来源：http://um.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dv.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sr.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uf.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ph.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ao.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://jz.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cg.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hy.wgjwhj.cn

[A25] 字符串比较
来源：http://wd.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://uv.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lc.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oi.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pl.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rj.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wp.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lf.yuexingan06.cn

[A26] 类型转换总览
来源：http://im.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gi.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lz.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bu.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://bb.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rl.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jt.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mj.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uj.asd995.cn

================================================================================
来源：http://mg.huanxung.cn

B. 流程控制
来源：http://wn.huanxung.cn

================================================================================
来源：http://oj.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://bm.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yb.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ni.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://am.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://au.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ym.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wz.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qa.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gf.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://dj.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sp.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rk.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tl.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://da.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ic.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ds.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.gzmigu.cn

[B03] switch / match / case
来源：http://ey.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://df.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lj.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oq.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mt.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fd.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uk.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yb.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gb.bjjhwx.cn

[B04] for 计数循环
来源：http://ng.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://hu.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nn.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fg.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ax.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://np.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://in.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://ux.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mi.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://bo.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ap.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mu.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kk.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hh.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xh.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sz.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://es.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iw.colortex.cn

[B06] 遍历字典 / 对象
来源：http://dx.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pe.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mv.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://es.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ur.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sb.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://al.bookmarksfly.cn

[B07] while 循环
来源：http://cv.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://tn.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sd.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://zc.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://kk.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://cl.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iv.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://zv.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://lm.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://as.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://gr.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ay.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xr.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://wp.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://my.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://si.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zp.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ht.asd995.cn

[B09] break 与 continue
来源：http://to.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iu.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dm.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yv.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wp.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://no.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://hl.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hi.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://va.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xz.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rr.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://km.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mu.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oa.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://wx.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://jr.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://vf.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://be.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jr.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dq.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://np.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://zy.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://da.hnjuh.cn

[B12] 跳出多层循环
来源：http://et.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mi.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ve.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yx.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qq.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cc.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yu.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ti.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ds.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://yj.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://im.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cw.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fy.lnxyls.cn

Java: x instanceof Number
来源：http://bd.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bj.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://pw.nszjky.cn

C#:   x is int or double or decimal
来源：http://rp.nszjky.cn

[B14] 判断值是否在集合内
来源：http://mr.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wa.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eb.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://og.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://wn.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xl.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qk.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pt.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ct.huanxung.cn

[B15] 布尔运算与取反
来源：http://qx.nicolike.cn

Py:   a and b or not c
来源：http://yx.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://vw.panjiajie.cn

JS:   a && b || !c
来源：http://rh.newstarts.cn

TS:   a && b || !c
来源：http://bj.shtwfgs.cn

Java: a && b || !c
来源：http://ks.colortex.cn

Go:   a && b || !c
来源：http://oo.shxzskj.cn

Ruby: a && b || !c
来源：http://lm.huixinmuqiang.cn

C#:   a && b || !c
来源：http://zw.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ga.chemitech.net.cn

Py:   if not data: return
来源：http://qy.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://gf.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://lk.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://rx.521024.cn

Java: if (data == null) return;
来源：http://yu.shxzukj.cn

Go:   if data == nil { return }
来源：http://tr.huixiangedu.cn

Ruby: return if data.nil?
来源：http://sq.asd995.cn

C#:   if (data == null) return;
来源：http://kn.nszjky.cn

================================================================================
来源：http://ji.shxzskj.cn

C. 函数与作用域
来源：http://pm.huixiangedu.cn

================================================================================
来源：http://fy.lnxyls.cn

[C01] 定义函数
来源：http://gp.colortex.cn


<!-- 参考信息 -->