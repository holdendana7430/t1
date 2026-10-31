代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://cj.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ut.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://vp.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fa.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hx.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://lx.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://rh.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://pj.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mu.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://bv.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://nk.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ba.9csxet.cn

Py:   "第一行\n第二行"
来源：http://ij.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://vt.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://sh.szsharing.cn

TS:   "第一行\n第二行"
来源：http://ko.shxzskj.cn

Java: "第一行\n第二行"
来源：http://sv.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://bb.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://eb.hahajie.cn

C#:   "第一行\n第二行"
来源：http://tk.jctech888.com.cn

[A14] 注释写法
来源：http://fs.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ai.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wb.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://pr.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://fa.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eq.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://yt.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ap.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://so.szsharing.cn

[A15] 空值判断与默认值
来源：http://ty.shxzskj.cn

Py:   value = data or "默认值"
来源：http://sq.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://og.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://sg.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://kk.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xk.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://hy.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://xw.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://cx.szsharing.cn

[A16] 真假值判断规则
来源：http://jy.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wl.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fq.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kb.huixiangedu.cn

TS:   if (!x) {}
来源：http://gi.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wo.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://st.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ie.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xa.szxytkj.cn

[A17] 位运算
来源：http://fd.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bo.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yg.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://om.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ny.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cb.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ii.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://yo.colortex.cn

Py:   ord("A"); chr(65)
来源：http://qg.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://st.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ra.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jw.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://mg.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sc.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://fo.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://mz.bookmarksfly.cn

[A19] 交换两个变量
来源：http://qw.shxzukj.cn

Py:   a, b = b, a
来源：http://hr.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rs.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://cd.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://oc.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://rt.bjjhwx.cn

Go:   a, b = b, a
来源：http://cr.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://cc.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://au.huixiangedu.cn

[A20] 读取标准输入
来源：http://hf.szxytkj.cn

Py:   name = input("请输入：")
来源：http://ew.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dy.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ao.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://au.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://he.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vw.jctech888.com.cn

Ruby: gets.chomp
来源：http://ft.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://by.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://jz.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://kp.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yz.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://dl.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://mz.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://dp.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uk.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://hm.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://sq.gzmigu.cn

[A22] 获取字符串长度
来源：http://ky.chemitech.net.cn

Py:   len(s)
来源：http://hb.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lx.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zm.szsharing.cn

TS:   s.length
来源：http://pa.huixiangedu.cn

Java: s.length()
来源：http://bj.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://po.szsharing.cn

Ruby: s.length
来源：http://fp.gzmigu.cn

C#:   s.Length
来源：http://xz.nicolike.cn

[A23] 大小写转换
来源：http://iw.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mo.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bj.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cy.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sz.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nt.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://us.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gs.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hm.gzmigu.cn

[A24] 去除首尾空白
来源：http://bw.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fk.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iq.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://se.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hf.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://if.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://ib.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eu.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jw.shtwfgs.cn

[A25] 字符串比较
来源：http://sp.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://oh.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yl.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pz.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vb.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wy.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aq.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ja.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yx.muxihuayi.cn

[A26] 类型转换总览
来源：http://yt.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wv.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sp.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://db.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://df.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://do.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tq.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bo.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sp.huixinmuqiang.cn

================================================================================
来源：http://aa.jctech888.com.cn

B. 流程控制
来源：http://qg.jctech888.com.cn

================================================================================
来源：http://vj.huanxung.cn

[B01] 条件判断 if / else
来源：http://iq.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kp.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bi.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kp.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hw.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rd.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://da.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fe.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vf.hahajie.cn

[B02] 多分支 else if / elif
来源：http://lz.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lr.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ft.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vx.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cx.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://no.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.shxzskj.cn

[B03] switch / match / case
来源：http://ir.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gk.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rj.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jg.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mp.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ed.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tz.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rq.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qz.jctech888.com.cn

[B04] for 计数循环
来源：http://fx.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://zq.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ea.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uu.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://no.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ys.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://az.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://en.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://xa.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://rd.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xf.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mj.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fc.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qm.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sw.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://so.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ur.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://wt.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bu.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kk.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yp.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qf.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://di.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kp.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cq.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yk.hnjuh.cn

[B07] while 循环
来源：http://wp.hahajie.cn

Py:   while i < 10: i += 1
来源：http://af.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ek.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://wt.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://fj.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://gg.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ja.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://rw.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ws.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://ms.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://nd.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xd.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://mx.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://iy.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://fy.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jt.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hg.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ab.jctech888.com.cn

[B09] break 与 continue
来源：http://ox.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tx.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pe.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bx.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gh.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ud.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zs.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://mt.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cq.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://an.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cj.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mr.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rz.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qj.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tv.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ko.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://fx.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://bk.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ey.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ij.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://to.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uk.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ud.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://kb.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jj.nszjky.cn

[B12] 跳出多层循环
来源：http://dc.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rh.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lv.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://je.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dg.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gn.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kq.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jn.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ta.jctech888.com.cn

[B13] 判断是否为数字
来源：http://lr.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://af.nicolike.cn

PHP:  is_numeric($x)
来源：http://bn.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ri.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sk.asd995.cn

Java: x instanceof Number
来源：http://yf.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yq.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://ct.colortex.cn

C#:   x is int or double or decimal
来源：http://md.huanxung.cn

[B14] 判断值是否在集合内
来源：http://sh.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cj.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uc.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://zq.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://dk.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sn.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kh.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wx.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uh.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://co.hnjuh.cn

Py:   a and b or not c
来源：http://kh.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://ug.yuexingan06.cn

JS:   a && b || !c
来源：http://gk.hahajie.cn

TS:   a && b || !c
来源：http://zi.wgjwhj.cn

Java: a && b || !c
来源：http://yo.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ih.bjjhwx.cn

Ruby: a && b || !c
来源：http://og.szsharing.cn

C#:   a && b || !c
来源：http://dz.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kp.muxihuayi.cn

Py:   if not data: return
来源：http://uj.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://in.muxihuayi.cn

JS:   if (!data) return;
来源：http://or.bookmarksfly.cn

TS:   if (!data) return;
来源：http://fs.newstarts.cn

Java: if (data == null) return;
来源：http://yu.521024.cn

Go:   if data == nil { return }
来源：http://xt.huanxung.cn

Ruby: return if data.nil?
来源：http://lo.gzmigu.cn

C#:   if (data == null) return;
来源：http://wi.bjjhwx.cn

================================================================================
来源：http://wu.szsharing.cn

C. 函数与作用域
来源：http://rk.newstarts.cn

================================================================================
来源：http://ke.yuexingan06.cn

[C01] 定义函数
来源：http://je.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://vh.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eq.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ko.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rz.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pv.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cp.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://bk.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nt.asd995.cn

[C02] 默认参数
来源：http://ry.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://aa.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nf.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://wx.gzmigu.cn


<!-- 参考信息 -->