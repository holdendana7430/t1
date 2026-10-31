代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://fg.hahajie.cn

[A11] 条件表达式（三元）
来源：http://yq.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://rj.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yx.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uf.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uu.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://dl.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wt.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yf.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wz.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://yp.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tw.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://px.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://xa.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://na.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://gl.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mu.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ps.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://gx.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zx.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://fm.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://bd.hahajie.cn

JS:   "第一行\n第二行"
来源：http://py.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://my.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://lb.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ut.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://dj.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://fg.nicolike.cn

[A14] 注释写法
来源：http://cl.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yw.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nz.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://rg.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://ri.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mb.521024.cn

Go:   // 单行；/* 多行 */
来源：http://cz.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://do.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://go.lnxyls.cn

[A15] 空值判断与默认值
来源：http://af.shxzukj.cn

Py:   value = data or "默认值"
来源：http://bw.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://wd.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://uc.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://xh.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ee.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://qa.newstarts.cn

Ruby: value = data || "默认值"
来源：http://bo.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://mc.szxytkj.cn

[A16] 真假值判断规则
来源：http://sk.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://we.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gs.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xz.shxzukj.cn

TS:   if (!x) {}
来源：http://ww.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zn.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gd.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ww.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://za.shtwfgs.cn

[A17] 位运算
来源：http://ta.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://db.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dt.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lq.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ex.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zo.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xf.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://oz.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://la.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://bc.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qd.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dw.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://be.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qr.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://bq.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://yw.jctech888.com.cn

[A19] 交换两个变量
来源：http://ha.nszjky.cn

Py:   a, b = b, a
来源：http://je.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ff.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ga.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://fd.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://xo.bookmarksfly.cn

Go:   a, b = b, a
来源：http://uu.wgjwhj.cn

Ruby: a, b = b, a
来源：http://wk.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://lo.521024.cn

[A20] 读取标准输入
来源：http://ek.huanxung.cn

Py:   name = input("请输入：")
来源：http://ho.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gb.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://is.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://no.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://tt.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wn.chemitech.net.cn

Ruby: gets.chomp
来源：http://ph.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://ln.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://rz.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://nt.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yq.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://we.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://tf.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://oa.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hb.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://is.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://bd.shxzukj.cn

[A22] 获取字符串长度
来源：http://kw.hahajie.cn

Py:   len(s)
来源：http://lf.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gk.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ev.colortex.cn

TS:   s.length
来源：http://yn.szsharing.cn

Java: s.length()
来源：http://oa.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lz.521024.cn

Ruby: s.length
来源：http://xn.asd995.cn

C#:   s.Length
来源：http://fa.jctech888.com.cn

[A23] 大小写转换
来源：http://zw.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ab.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ar.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vc.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jp.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fn.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sj.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lj.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ft.szxytkj.cn

[A24] 去除首尾空白
来源：http://rz.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ep.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eg.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gy.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ie.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://ep.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iq.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ce.jctech888.com.cn

[A25] 字符串比较
来源：http://ka.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://if.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sg.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ud.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hj.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ts.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qt.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wu.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ct.hahajie.cn

[A26] 类型转换总览
来源：http://gl.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://so.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hn.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oy.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://kk.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://la.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://px.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ap.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://at.yuntaijiaju.cn

================================================================================
来源：http://px.nicolike.cn

B. 流程控制
来源：http://sv.shxzskj.cn

================================================================================
来源：http://uj.9csxet.cn

[B01] 条件判断 if / else
来源：http://fm.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://as.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qe.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ey.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uc.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qs.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lp.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tg.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://od.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://hv.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ck.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ts.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dv.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sx.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jn.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tl.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://un.shxzskj.cn

[B03] switch / match / case
来源：http://os.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xz.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qs.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hy.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://su.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cb.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pc.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fb.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yq.gzmigu.cn

[B04] for 计数循环
来源：http://tt.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://el.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pt.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ae.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dx.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wn.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://il.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://yc.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ti.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://wu.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://gz.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mm.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nv.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tt.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nf.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xp.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://qs.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ps.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://vk.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kx.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://da.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mf.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tj.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ma.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hd.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aa.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eu.huixinmuqiang.cn

[B07] while 循环
来源：http://tw.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://zk.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mz.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://tg.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://oz.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://sz.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ia.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://cc.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://rh.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://tq.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://pd.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pr.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://kx.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://gk.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://oq.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mc.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bf.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ih.yuntaijiaju.cn

[B09] break 与 continue
来源：http://cq.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xk.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://io.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gy.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xv.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eg.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rb.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://yd.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cv.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kh.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ww.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://og.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jn.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cy.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://al.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nq.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://is.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ly.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ef.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://as.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lx.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kk.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jd.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://wx.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rv.jctech888.com.cn

[B12] 跳出多层循环
来源：http://ab.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kz.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ma.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pt.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uo.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cw.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lb.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ek.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://op.muxihuayi.cn

[B13] 判断是否为数字
来源：http://kz.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ku.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://as.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bg.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rg.hahajie.cn

Java: x instanceof Number
来源：http://bq.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bi.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://hl.9csxet.cn

C#:   x is int or double or decimal
来源：http://ke.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://sb.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vk.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lv.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://en.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://jz.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://th.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zz.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cx.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ft.huanxung.cn

[B15] 布尔运算与取反
来源：http://hw.lnxyls.cn

Py:   a and b or not c
来源：http://fa.asd995.cn

PHP:  $a && $b || !$c
来源：http://nm.haigaiapp.cn

JS:   a && b || !c
来源：http://uu.huanxung.cn

TS:   a && b || !c
来源：http://rx.lnxyls.cn

Java: a && b || !c
来源：http://pp.yuexingan06.cn

Go:   a && b || !c
来源：http://cn.haigaiapp.cn

Ruby: a && b || !c
来源：http://tb.nicolike.cn

C#:   a && b || !c
来源：http://tv.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yk.asd995.cn

Py:   if not data: return
来源：http://kb.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://zq.colortex.cn

JS:   if (!data) return;
来源：http://aw.colortex.cn

TS:   if (!data) return;
来源：http://ik.asd995.cn

Java: if (data == null) return;
来源：http://lj.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://ch.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://jf.jctech888.com.cn

C#:   if (data == null) return;
来源：http://zf.jianghongdianzi.cn

================================================================================
来源：http://gq.shxzukj.cn

C. 函数与作用域
来源：http://un.szxytkj.cn

================================================================================
来源：http://df.hahajie.cn

[C01] 定义函数
来源：http://bt.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://qp.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aj.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://bt.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zp.colortex.cn


<!-- 参考信息 -->