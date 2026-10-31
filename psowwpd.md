代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://vz.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iv.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zg.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ui.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fn.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vv.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://gg.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zd.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://op.asd995.cn

JS:   `Hello, ${name}!`
来源：http://zp.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://de.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://os.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sy.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://zm.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://xp.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://if.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://yo.asd995.cn

PHP:  "第一行\n第二行"
来源：http://vb.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://pv.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://fm.shxzskj.cn

Java: "第一行\n第二行"
来源：http://zb.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://fi.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://mb.newstarts.cn

C#:   "第一行\n第二行"
来源：http://ou.huixiangedu.cn

[A14] 注释写法
来源：http://tz.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tj.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tv.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://gb.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://st.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kw.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://wt.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ay.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://dp.lnxyls.cn

[A15] 空值判断与默认值
来源：http://vm.hnjuh.cn

Py:   value = data or "默认值"
来源：http://bq.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://va.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://aa.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://pv.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lr.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://gg.nszjky.cn

Ruby: value = data || "默认值"
来源：http://jc.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ht.gzmigu.cn

[A16] 真假值判断规则
来源：http://zi.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xr.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zt.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ch.gzmigu.cn

TS:   if (!x) {}
来源：http://df.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bj.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ru.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vr.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kh.jianghongdianzi.cn

[A17] 位运算
来源：http://wb.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vy.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pd.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dp.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ch.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bo.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ay.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://ji.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://jb.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://md.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rb.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cd.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://gt.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ef.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://rw.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://qt.9csxet.cn

[A19] 交换两个变量
来源：http://sq.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://bo.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uz.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://fq.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://qv.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://mg.chemitech.net.cn

Go:   a, b = b, a
来源：http://mz.colortex.cn

Ruby: a, b = b, a
来源：http://lx.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://zm.hahajie.cn

[A20] 读取标准输入
来源：http://ru.shxzukj.cn

Py:   name = input("请输入：")
来源：http://dc.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sy.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kt.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://cs.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://vb.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ht.colortex.cn

Ruby: gets.chomp
来源：http://jp.hnjuh.cn

C#:   Console.ReadLine();
来源：http://rw.newstarts.cn

[A21] 保留指定小数位输出
来源：http://kc.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://st.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fw.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://lu.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://sz.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://vp.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ud.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://xv.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ll.hnjuh.cn

[A22] 获取字符串长度
来源：http://tc.jianghongdianzi.cn

Py:   len(s)
来源：http://nh.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cm.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dy.9csxet.cn

TS:   s.length
来源：http://bw.gzmigu.cn

Java: s.length()
来源：http://eu.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mc.9csxet.cn

Ruby: s.length
来源：http://mo.haigaiapp.cn

C#:   s.Length
来源：http://zi.hnjuh.cn

[A23] 大小写转换
来源：http://bc.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zo.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zj.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uo.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fb.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gb.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pg.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ai.huanxung.cn

[A24] 去除首尾空白
来源：http://yj.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://af.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://en.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zy.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tl.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pn.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://ou.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hp.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dg.nicolike.cn

[A25] 字符串比较
来源：http://gw.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ce.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zg.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ce.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vw.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fu.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gy.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://no.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mi.haigaiapp.cn

[A26] 类型转换总览
来源：http://wn.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://of.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fd.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uk.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://zm.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ol.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://co.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ms.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sy.hahajie.cn

================================================================================
来源：http://qa.hahajie.cn

B. 流程控制
来源：http://nv.hahajie.cn

================================================================================
来源：http://aw.szxytkj.cn

[B01] 条件判断 if / else
来源：http://sa.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zp.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wr.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qe.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://st.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vg.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cb.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kk.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gn.huanxung.cn

[B02] 多分支 else if / elif
来源：http://sj.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ro.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zb.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uy.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oo.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xk.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://by.colortex.cn

[B03] switch / match / case
来源：http://mu.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xn.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qq.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bd.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://as.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ii.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qr.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yk.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zu.lnxyls.cn

[B04] for 计数循环
来源：http://wh.521024.cn

Py:   for i in range(10): print(i)
来源：http://yv.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zp.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iw.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ne.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nz.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qr.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://io.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://by.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://za.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ip.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mi.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xs.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sk.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tb.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://it.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://rp.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ev.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ah.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ld.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://os.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qb.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vp.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ye.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ld.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zq.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jx.shtwfgs.cn

[B07] while 循环
来源：http://hd.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://iv.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rc.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://qe.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://zz.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://fh.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ux.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://oi.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://qf.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://ku.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://dq.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bt.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://wo.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://qn.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://bs.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iz.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bn.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://oo.chemitech.net.cn

[B09] break 与 continue
来源：http://gq.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sr.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ph.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jl.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vl.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dz.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://it.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://jy.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://km.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cn.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xy.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vh.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ws.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zv.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wt.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lh.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ly.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://cj.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://cv.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ab.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gu.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xg.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ml.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://ie.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.chemitech.net.cn

[B12] 跳出多层循环
来源：http://wu.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eu.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ei.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uy.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aa.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ps.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cs.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vk.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lh.asd995.cn

[B13] 判断是否为数字
来源：http://bx.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ko.panjiajie.cn

PHP:  is_numeric($x)
来源：http://xi.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ra.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zv.huixiangedu.cn

Java: x instanceof Number
来源：http://ex.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gk.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://my.newstarts.cn

C#:   x is int or double or decimal
来源：http://ap.9csxet.cn

[B14] 判断值是否在集合内
来源：http://jc.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://li.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ax.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://sy.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://eu.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vp.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sz.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jh.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xc.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://ne.shxzukj.cn

Py:   a and b or not c
来源：http://xa.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://lu.shtwfgs.cn

JS:   a && b || !c
来源：http://wr.panjiajie.cn

TS:   a && b || !c
来源：http://xz.hahajie.cn

Java: a && b || !c
来源：http://cf.shxzukj.cn

Go:   a && b || !c
来源：http://hy.bookmarksfly.cn

Ruby: a && b || !c
来源：http://qa.gzmigu.cn

C#:   a && b || !c
来源：http://vg.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zl.jctech888.com.cn

Py:   if not data: return
来源：http://ui.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://fi.hnjuh.cn

JS:   if (!data) return;
来源：http://qg.huixiangedu.cn

TS:   if (!data) return;
来源：http://kp.hnjuh.cn

Java: if (data == null) return;
来源：http://er.shtwfgs.cn

Go:   if data == nil { return }
来源：http://rb.jctech888.com.cn

Ruby: return if data.nil?
来源：http://xz.yuexingan06.cn

C#:   if (data == null) return;
来源：http://bm.newstarts.cn

================================================================================
来源：http://ja.nszjky.cn

C. 函数与作用域
来源：http://tk.asd995.cn

================================================================================
来源：http://gg.jctech888.com.cn

[C01] 定义函数
来源：http://sh.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://kp.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fu.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ic.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cz.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ee.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yz.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://sz.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lx.yuexingan06.cn


<!-- 参考信息 -->